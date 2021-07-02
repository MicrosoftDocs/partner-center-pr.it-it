---
title: Creare e gestire le Azure Marketplace private nel portale di Azure
description: Informazioni sulla creazione e la gestione di Azure Marketplace privato (anteprima) nella portale di Azure. La Azure Marketplace privata (anteprima) consente agli amministratori di controllare le soluzioni di terze parti che gli utenti possono usare.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173697"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="7de01-104">Creare e gestire le Azure Marketplace private nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="7de01-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="7de01-105">Il Azure Marketplace consente agli amministratori di controllare le soluzioni di terze parti che gli utenti possono usare.</span><span class="sxs-lookup"><span data-stu-id="7de01-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="7de01-106">Ciò consente all'utente di distribuire solo le offerte approvate dall'amministratore e conformi ai criteri aziendali.</span><span class="sxs-lookup"><span data-stu-id="7de01-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="7de01-107">Con il Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi da acquistare e distribuire.</span><span class="sxs-lookup"><span data-stu-id="7de01-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="7de01-108">Come amministratore del Marketplace (ruolo assegnato), si inizierà con uno Store privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati.</span><span class="sxs-lookup"><span data-stu-id="7de01-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="7de01-109">Questo articolo illustra come assegnare il ruolo necessario, creare un archivio privato, gestire gli elementi, approvare le richieste degli utenti e abilitare l'Azure Marketplace privato per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="7de01-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="7de01-110">Il Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant visualizzano lo stesso elenco curato.</span><span class="sxs-lookup"><span data-stu-id="7de01-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="7de01-111">Tutte le soluzioni Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) vengono aggiunte automaticamente a private Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="7de01-112">Assegnare il ruolo di amministratore del Marketplace</span><span class="sxs-lookup"><span data-stu-id="7de01-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="7de01-113">Il tenant amministratore globale deve assegnare il ruolo di amministratore del **Marketplace** all'amministratore Azure Marketplace che gestirà l'archivio privato.</span><span class="sxs-lookup"><span data-stu-id="7de01-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="7de01-114">L'accesso alla Azure Marketplace privata è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.</span><span class="sxs-lookup"><span data-stu-id="7de01-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="7de01-115">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="7de01-115">Prerequisites</span></span>

<span data-ttu-id="7de01-116">Questi prerequisiti sono necessari prima di poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant:</span><span class="sxs-lookup"><span data-stu-id="7de01-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="7de01-117">Si ha accesso a un **amministratore globale** utente.</span><span class="sxs-lookup"><span data-stu-id="7de01-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="7de01-118">Il tenant ha almeno una sottoscrizione (può essere di qualsiasi tipo).</span><span class="sxs-lookup"><span data-stu-id="7de01-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="7de01-119">All amministratore globale utente viene assegnato il **ruolo Collaboratore** o superiore per la sottoscrizione scelta.</span><span class="sxs-lookup"><span data-stu-id="7de01-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="7de01-120">Assegnare il ruolo di amministratore del Marketplace con controllo di accesso (IAM)</span><span class="sxs-lookup"><span data-stu-id="7de01-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="7de01-121">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7de01-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="7de01-122">Selezionare **Tutti i servizi** e quindi **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="7de01-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="7de01-123">Selezionare **Marketplace privato** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="7de01-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra l'opzione di menu marketplace privato sul lato sinistro del Marketplace.":::

1. <span data-ttu-id="7de01-125">Selezionare **Controllo di accesso (IAM) per** assegnare il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra la schermata di controllo di accesso di I A M.":::

1. <span data-ttu-id="7de01-127">Selezionare **Aggiungi** > **Aggiungi assegnazione di ruolo**.</span><span class="sxs-lookup"><span data-stu-id="7de01-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="7de01-128">In **Ruolo scegliere** Amministratore del **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="7de01-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra il menu Assegnazione di ruolo.":::

1. <span data-ttu-id="7de01-130">Selezionare l'utente desiderato nell'elenco a discesa, quindi selezionare **Fine.**</span><span class="sxs-lookup"><span data-stu-id="7de01-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="7de01-131">Assegnare il ruolo di amministratore del Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="7de01-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="7de01-132">Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace. richiede i parametri seguenti:</span><span class="sxs-lookup"><span data-stu-id="7de01-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="7de01-133">**TenantId:** ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).</span><span class="sxs-lookup"><span data-stu-id="7de01-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="7de01-134">**Id sottoscrizione:** Sottoscrizione di cui all'amministratore globale è assegnato **il ruolo Collaboratore** o superiore.</span><span class="sxs-lookup"><span data-stu-id="7de01-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="7de01-135">**GlobalAdminUsername:** Nome utente dell'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="7de01-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="7de01-136">**UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="7de01-137">Per gli utenti guest invitati nel tenant, potrebbero essere necessario fino a 48 ore prima che il proprio account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="7de01-138">Per altre informazioni, vedere Properties of an Azure Active Directory B2B collaboration user (Proprietà di [un utente di Collaborazione B2B).](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="7de01-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="7de01-139">Per altre informazioni sui cmdlet contenuti nel modulo PowerShell Az.Portal, [vedere Microsoft Azure PowerShell: Cmdlet del dashboard del portale.](/powershell/module/az.portal/)</span><span class="sxs-lookup"><span data-stu-id="7de01-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="7de01-140">Creare un Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7de01-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="7de01-141">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7de01-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7de01-142">Selezionare **Tutti i servizi** e quindi **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="7de01-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra la portale di Azure finestra principale.":::

3. <span data-ttu-id="7de01-144">Selezionare **Marketplace privato** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="7de01-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="7de01-145">Selezionare **Informazioni di base** per creare un Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).</span><span class="sxs-lookup"><span data-stu-id="7de01-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Viene illustrato come selezionare il Informazioni di base nella finestra portale di Azure'.":::

    <span data-ttu-id="7de01-147">Se l Azure Marketplace privata esiste già per questo tenant, **per** impostazione predefinita verrà selezionata l'opzione Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="7de01-148">Al termine, si avrà un'istanza privata vuota e disabilitata Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra la schermata Azure Marketplace privato vuota.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="7de01-150">Aggiungere elementi dalla raccolta</span><span class="sxs-lookup"><span data-stu-id="7de01-150">Add items from gallery</span></span>

<span data-ttu-id="7de01-151">Un elemento è una combinazione di un'offerta e di un piano.</span><span class="sxs-lookup"><span data-stu-id="7de01-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="7de01-152">È possibile cercare e aggiungere elementi nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7de01-153">Selezionare **Aggiungi elementi.**</span><span class="sxs-lookup"><span data-stu-id="7de01-153">Select **Add items**.</span></span>

2. <span data-ttu-id="7de01-154">Esplorare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.</span><span class="sxs-lookup"><span data-stu-id="7de01-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Illustra come esplorare la raccolta o usare il campo di ricerca.":::

3. <span data-ttu-id="7de01-156">Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco approvato.</span><span class="sxs-lookup"><span data-stu-id="7de01-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="7de01-157">Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani necessari.</span><span class="sxs-lookup"><span data-stu-id="7de01-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Illustra come aggiornare i piani necessari.":::

4. <span data-ttu-id="7de01-159">Selezionare **Fine** in basso a sinistra dopo aver effettuato le selezioni.</span><span class="sxs-lookup"><span data-stu-id="7de01-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="7de01-160">**Aggiungi elementi** al Marketplace sarà disponibile solo per le offerte non Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7de01-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="7de01-161">Le soluzioni Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) verranno contrassegnate come "Approvate per impostazione predefinita" e non possono essere gestite nel Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="7de01-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="7de01-162">Modificare i piani dell'elemento</span><span class="sxs-lookup"><span data-stu-id="7de01-162">Edit item's plans</span></span>

<span data-ttu-id="7de01-163">È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7de01-164">Nella colonna **Piani** esaminare i piani disponibili nel menu a discesa per tale elemento.</span><span class="sxs-lookup"><span data-stu-id="7de01-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="7de01-165">Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.</span><span class="sxs-lookup"><span data-stu-id="7de01-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra come selezionare o deselezionare la casella di controllo per l'elemento richiesto.":::

   > [!NOTE]
   > <span data-ttu-id="7de01-167">Ogni offerta richiede almeno un piano selezionato per l'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="7de01-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="7de01-168">Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="7de01-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="7de01-169">Eliminare le offerte</span><span class="sxs-lookup"><span data-stu-id="7de01-169">Delete offers</span></span>

<span data-ttu-id="7de01-170">Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.</span><span class="sxs-lookup"><span data-stu-id="7de01-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="7de01-171">Abilitare/disabilitare l'Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7de01-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="7de01-172">Nella pagina Gestisci Marketplace verrà visualizzato uno di questi banner, che mostrano lo stato corrente di Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="7de01-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra il banner &quot;Disabilita stato&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra il banner &quot;Abilita stato&quot;.":::

<span data-ttu-id="7de01-175">È possibile abilitare o disabilitare l'Azure Marketplace privata in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="7de01-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="7de01-176">Se disabilitata, selezionare **Abilita Marketplace privato** per l'abilitazione.</span><span class="sxs-lookup"><span data-stu-id="7de01-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="7de01-177">Se abilitata, selezionare **Disabilita Marketplace privato per** disabilitarla.</span><span class="sxs-lookup"><span data-stu-id="7de01-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="7de01-178">Centro notifiche Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="7de01-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="7de01-179">Il Centro notifiche è costituito da tre tipi di notifiche e consente all'amministratore del Marketplace di eseguire azioni in base alla notifica:</span><span class="sxs-lookup"><span data-stu-id="7de01-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="7de01-180">Richieste di approvazione da parte degli utenti per gli elementi non presenti nell'elenco approvato (vedere Richiedere [l'aggiunta di offerte o piani più](#request-to-add-offers-or-plans) avanti).</span><span class="sxs-lookup"><span data-stu-id="7de01-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="7de01-181">Notifiche del nuovo piano per le offerte che hanno già uno o più piani nell'elenco approvato.</span><span class="sxs-lookup"><span data-stu-id="7de01-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="7de01-182">Sono state rimosse le notifiche del piano per gli elementi presenti nell'elenco approvato, ma che sono stati rimossi dal gruppo Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="7de01-183">Per accedere al centro notifiche:</span><span class="sxs-lookup"><span data-stu-id="7de01-183">To access the notification center:</span></span>

1. <span data-ttu-id="7de01-184">Selezionare **Notifiche** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="7de01-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Visualizza il menu Notifiche.":::

1. <span data-ttu-id="7de01-186">Selezionare il menu con i puntini di sospensione per altre azioni.</span><span class="sxs-lookup"><span data-stu-id="7de01-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra i risultati del menu Altre opzioni.":::

1. <span data-ttu-id="7de01-188">Per le richieste di piano, **Mostra richieste apre** il modulo di richiesta di approvazione in cui è possibile esaminare tutte le richieste utente per l'offerta specifica.</span><span class="sxs-lookup"><span data-stu-id="7de01-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="7de01-189">Selezionare **Approva** o **Rifiuta.**</span><span class="sxs-lookup"><span data-stu-id="7de01-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra le opzioni di approvazione e rifiuto.":::

1. <span data-ttu-id="7de01-191">Selezionare il piano da approvare dal menu a discesa.</span><span class="sxs-lookup"><span data-stu-id="7de01-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="7de01-192">Aggiungere un commento e selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="7de01-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="7de01-193">Esplorazione di Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7de01-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="7de01-194">Quando l'Azure Marketplace è abilitata, gli utenti visualizzano i piani approvati dall'amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="7de01-195">Un avviso **verde Approvato** indica un'offerta partner (non Microsoft) approvata.</span><span class="sxs-lookup"><span data-stu-id="7de01-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="7de01-196">Un avviso **blu Approvato** indica un'offerta Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) approvata.</span><span class="sxs-lookup"><span data-stu-id="7de01-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="7de01-197">Gli utenti possono filtrare le offerte che sono e non sono approvate:</span><span class="sxs-lookup"><span data-stu-id="7de01-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra l'opzione di filtro.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="7de01-199">Acquistare o distribuire in servizi Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7de01-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="7de01-200">Anche se l'esperienza della pagina dei dettagli del prodotto è simile Azure Marketplace globale, esistono tre scenari specifici Azure Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="7de01-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="7de01-201">Quando un utente seleziona un piano approvato, il **pulsante** Crea è abilitato:</span><span class="sxs-lookup"><span data-stu-id="7de01-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra il banner dell'offerta che indica che è possibile creare un piano.":::

- <span data-ttu-id="7de01-203">Se la selezione di un piano di prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva i piani approvati e il **pulsante** Crea è abilitato:</span><span class="sxs-lookup"><span data-stu-id="7de01-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra il banner dell'offerta che indica che è possibile creare un piano e mostra i piani disponibili.":::

- <span data-ttu-id="7de01-205">Quando un utente seleziona un piano non approvato, un banner indica che il piano non è approvato e il **pulsante** Crea è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="7de01-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="7de01-206">L'utente può comunque richiedere di aggiungere il piano all'elenco approvato (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="7de01-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="7de01-207">Richiesta di aggiunta di offerte o piani</span><span class="sxs-lookup"><span data-stu-id="7de01-207">Request to add offers or plans</span></span>

<span data-ttu-id="7de01-208">È possibile richiedere di aggiungere un'offerta o un piano pubblico non attualmente approvato nell'Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="7de01-209">Selezionare **Richiesta da aggiungere nel** banner per aprire il modulo Richiesta di **accesso**.</span><span class="sxs-lookup"><span data-stu-id="7de01-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Mostra il banner con il collegamento &quot;Richiesta di aggiunta&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra il modulo di richiesta di accesso per offerte o piani.":::

1. <span data-ttu-id="7de01-212">Selezionare i piani da aggiungere alla richiesta **(** Qualsiasi piano indica all'amministratore del Marketplace che non si ha una preferenza per un piano all'interno di un'offerta).</span><span class="sxs-lookup"><span data-stu-id="7de01-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="7de01-213">Aggiungere una **giustificazione e** selezionare **Richiesta per** inviare la richiesta.</span><span class="sxs-lookup"><span data-stu-id="7de01-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Mostra il modulo di richiesta di accesso per offerte o piani con voci di esempio.":::

1. <span data-ttu-id="7de01-215">Un'indicazione per una richiesta in sospeso verrà visualizzata nel modulo Richiesta di accesso con l'opzione **Richiesta di ritiro**.</span><span class="sxs-lookup"><span data-stu-id="7de01-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Visualizza un elenco di piani approvati o in sospeso con il collegamento Richiesta di ritiro.":::

> [!NOTE]
> <span data-ttu-id="7de01-217">Dopo l'invio, il modulo di [](#private-azure-marketplace-notification-center) richiesta di approvazione verrà inviato al Centro notifiche per l'amministratore del Marketplace per esaminare la richiesta ed eseguire un'azione.</span><span class="sxs-lookup"><span data-stu-id="7de01-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="7de01-218">L'approvazione nel Marketplace privato non indica l'approvvigionamento di una soluzione.</span><span class="sxs-lookup"><span data-stu-id="7de01-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="7de01-219">Domande frequenti (FAQ)</span><span class="sxs-lookup"><span data-stu-id="7de01-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="7de01-220">Si sta già bloccando l'applicazione di terze parti del Marketplace tramite Criteri di Azure.</span><span class="sxs-lookup"><span data-stu-id="7de01-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="7de01-221">Che cosa è diverso?</span><span class="sxs-lookup"><span data-stu-id="7de01-221">How is this different?</span></span>

<span data-ttu-id="7de01-222">Esistono attualmente due modi per limitare i servizi di terze parti in Marketplace:</span><span class="sxs-lookup"><span data-stu-id="7de01-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="7de01-223">Tramite EA Portal o il portale di Azure, disabilitare i servizi di terze parti o limitarsi a "Solo SKU gratuiti o BYOL".</span><span class="sxs-lookup"><span data-stu-id="7de01-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Illustra come limitare i servizi nel portale di Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Illustra come limitare i servizi nel portale E A.":::

2. <span data-ttu-id="7de01-226">Creare un criterio di Azure per consentire solo macchine virtuali specifiche.</span><span class="sxs-lookup"><span data-stu-id="7de01-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="7de01-227">Per informazioni dettagliate su come applicare i criteri Windows macchine virtuali, vedere Applicare criteri alle macchine virtuali [Windows con Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="7de01-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="7de01-228">Il Azure Marketplace privato offre maggiore flessibilità per limitare e consentire offerte e piani specifici.</span><span class="sxs-lookup"><span data-stu-id="7de01-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="7de01-229">Informa gli utenti finali sulla disponibilità per la distribuzione nella raccolta del marketplace anche prima di provare a distribuire servizi di terze parti.</span><span class="sxs-lookup"><span data-stu-id="7de01-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="7de01-230">Per consentire la distribuzione di servizi di terze parti, impostare Azure Marketplace su Attivato/Abilitato in EA Portal e il portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="7de01-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="7de01-231">I Azure Marketplace possono curare soluzioni partner non limitate alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="7de01-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="7de01-232">I Azure Marketplace possono essere curati a livello di piano e possono anche impostare "Piano corrente e futuro".</span><span class="sxs-lookup"><span data-stu-id="7de01-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="7de01-233">I Azure Marketplace possono informare gli utenti finali in anticipo su ciò che può o non può essere distribuito.</span><span class="sxs-lookup"><span data-stu-id="7de01-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="7de01-234">Qual è la differenza tra un'offerta privata e una Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="7de01-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="7de01-235">**Un'offerta privata** consente agli editori di creare piani visibili solo ai clienti di destinazione.</span><span class="sxs-lookup"><span data-stu-id="7de01-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="7de01-236">In questo modo possono condividere privatamente soluzioni personalizzate con prezzi negoziati, termini e condizioni privati e configurazioni specializzate.</span><span class="sxs-lookup"><span data-stu-id="7de01-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="7de01-237">Per informazioni dettagliate, [vedere Offerte private nel marketplace commerciale.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="7de01-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="7de01-238">**I Azure Marketplace** privati nel portale di Azure consentono agli amministratori di approvare in modo preliminare le soluzioni di terze parti che gli utenti possono distribuire.</span><span class="sxs-lookup"><span data-stu-id="7de01-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="7de01-239">Con un'Azure Marketplace privata, gli utenti possono usufruire dei vantaggi dell'Azure Marketplace trovando, acquistando e distribuendo offerte conformi.</span><span class="sxs-lookup"><span data-stu-id="7de01-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="7de01-240">Per gestire le offerte private basate su sottoscrizioni nel Marketplace privato, l'amministratore del Marketplace deve avere almeno il ruolo di "lettura" per la sottoscrizione specifica.</span><span class="sxs-lookup"><span data-stu-id="7de01-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="7de01-241">È stata aggiunta un'offerta privata al Azure Marketplace privato, perché non viene visualizzata nella scheda Gestisci marketplace?</span><span class="sxs-lookup"><span data-stu-id="7de01-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="7de01-242">Le offerte private basate su sottoscrizione sono visibili solo per le sottoscrizioni elencate nelle impostazioni dell'offerta privata.</span><span class="sxs-lookup"><span data-stu-id="7de01-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="7de01-243">Per visualizzare l'offerta privata, verificare che il filtro delle sottoscrizioni globali mostri tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="7de01-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra il filtro del marketplace privato.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="7de01-245">È possibile includere immagini personalizzate in private Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="7de01-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="7de01-246">No.</span><span class="sxs-lookup"><span data-stu-id="7de01-246">No.</span></span> <span data-ttu-id="7de01-247">La Azure Marketplace consente a qualsiasi amministratore IT di gestire e gestire soluzioni di terze parti da soluzioni Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7de01-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="7de01-248">Poiché le immagini personalizzate non sono in Azure Marketplace globale, l'amministratore IT non può selezionare e scegliere le immagini personalizzate.</span><span class="sxs-lookup"><span data-stu-id="7de01-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="7de01-249">Se si desidera condividere immagini personalizzate, usare [Raccolta immagini condivise.](/azure/virtual-machines/shared-image-galleries)</span><span class="sxs-lookup"><span data-stu-id="7de01-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="7de01-250">Guida dettagliata alla creazione di una raccolta di immagini condivise (SIG) (interfaccia[della riga di](/azure/virtual-machines/shared-images-cli)comando, [PowerShell).](/azure/virtual-machines/shared-images-powershell)</span><span class="sxs-lookup"><span data-stu-id="7de01-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="7de01-251">Creare una definizione di immagine all'interno di un sig.</span><span class="sxs-lookup"><span data-stu-id="7de01-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="7de01-252">Il cliente deve **scegliere Generalized (Generalizzato)** per il campo OS-state (Stato sistema operativo).</span><span class="sxs-lookup"><span data-stu-id="7de01-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="7de01-253">([interfaccia della](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)riga di comando , [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="7de01-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="7de01-254">Portare un'immagine gestita in Raccolta immagini condivise (interfaccia[della riga di comando,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)</span><span class="sxs-lookup"><span data-stu-id="7de01-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="7de01-255">Le immagini di VM SIG risiederebbero in una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="7de01-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="7de01-256">Per renderla disponibile ad altre sottoscrizioni, usare una registrazione dell'app (interfaccia[della riga di comando](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)</span><span class="sxs-lookup"><span data-stu-id="7de01-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="7de01-257">Perché alcune offerte sono approvate **per impostazione predefinita** anche se l'editore non è Microsoft?</span><span class="sxs-lookup"><span data-stu-id="7de01-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="7de01-258">Microsoft supporta Linux e la tecnologia open source in Azure.</span><span class="sxs-lookup"><span data-stu-id="7de01-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="7de01-259">[Le distribuzioni Linux approvate](/azure/virtual-machines/linux/endorsed-distros) sono supportate in Azure e il prezzo è integrato nelle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="7de01-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="7de01-260">Poiché l'agente Linux di Azure è già preinstallato Azure Marketplace, viene considerato come un'offerta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7de01-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="7de01-261">Poiché le offerte Microsoft sono approvate per impostazione predefinita, le distribuzioni Linux approvate non possono essere gestite in private Azure Marketplace e sono approvate per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="7de01-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="7de01-262">Contattare il supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="7de01-262">Contact support</span></span>

- <span data-ttu-id="7de01-263">Per Azure Marketplace, visitare il sito [Web Microsoft Q&A.](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="7de01-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>