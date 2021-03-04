---
title: Creare e gestire Azure Marketplace privato nel portale di Azure
description: Informazioni sulla creazione e sulla gestione di Azure Marketplace privato (anteprima) nel portale di Azure. Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "101757071"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="ec314-104">Creare e gestire Azure Marketplace privato nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="ec314-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="ec314-105">Azure Marketplace privato consente agli amministratori di gestire le soluzioni di terze parti che possono essere usate dagli utenti.</span><span class="sxs-lookup"><span data-stu-id="ec314-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="ec314-106">Questa operazione viene eseguita consentendo all'utente di distribuire solo le offerte approvate dall'amministratore ed essere conformi ai criteri dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="ec314-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="ec314-107">Con Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi per l'acquisto e la distribuzione.</span><span class="sxs-lookup"><span data-stu-id="ec314-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="ec314-108">In qualità di amministratore del Marketplace (ruolo assegnato), si inizierà con un archivio privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati.</span><span class="sxs-lookup"><span data-stu-id="ec314-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="ec314-109">Questo articolo illustra come assegnare il ruolo necessario, creare un archivio privato, gestire gli elementi, approvare le richieste degli utenti e abilitare Azure Marketplace privato per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="ec314-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="ec314-110">Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant vedranno lo stesso elenco curato.</span><span class="sxs-lookup"><span data-stu-id="ec314-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="ec314-111">Tutte le soluzioni Microsoft (incluse le [distribuzioni Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) vengono aggiunte automaticamente ad Azure Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="ec314-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="ec314-112">Assegnare il ruolo di amministratore del Marketplace</span><span class="sxs-lookup"><span data-stu-id="ec314-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="ec314-113">L'amministratore globale del tenant deve assegnare il ruolo di **amministratore del Marketplace** all'amministratore di Azure Marketplace privato che gestirà l'archivio privato.</span><span class="sxs-lookup"><span data-stu-id="ec314-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="ec314-114">L'accesso alla gestione privata di Azure Marketplace è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.</span><span class="sxs-lookup"><span data-stu-id="ec314-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="ec314-115">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="ec314-115">Prerequisites</span></span>

<span data-ttu-id="ec314-116">Questi prerequisiti sono necessari per poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant:</span><span class="sxs-lookup"><span data-stu-id="ec314-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="ec314-117">Si ha accesso a un utente **amministratore globale** .</span><span class="sxs-lookup"><span data-stu-id="ec314-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="ec314-118">Il tenant ha almeno una sottoscrizione (può essere qualsiasi tipo).</span><span class="sxs-lookup"><span data-stu-id="ec314-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="ec314-119">All'utente amministratore globale viene assegnato il ruolo **collaboratore** o superiore per la sottoscrizione scelta.</span><span class="sxs-lookup"><span data-stu-id="ec314-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="ec314-120">Assegnare il ruolo di amministratore del Marketplace con controllo di accesso (IAM)</span><span class="sxs-lookup"><span data-stu-id="ec314-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="ec314-121">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ec314-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="ec314-122">Selezionare **tutti i servizi** e quindi **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="ec314-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="ec314-123">Scegliere **Marketplace privato** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="ec314-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="ec314-124">[![Mostra l'opzione di menu Marketplace privato sul lato sinistro del Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="ec314-125">Selezionare **controllo di accesso (IAM)** per assegnare il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra la schermata di controllo di accesso A M.":::

1. <span data-ttu-id="ec314-127">Selezionare **Aggiungi** > **Aggiungi assegnazione di ruolo**.</span><span class="sxs-lookup"><span data-stu-id="ec314-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="ec314-128">In **ruolo** scegliere **amministrazione del Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="ec314-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Consente di visualizzare il menu assegnazione ruolo.":::

1. <span data-ttu-id="ec314-130">Selezionare l'utente desiderato nell'elenco a discesa, quindi fare clic su **fine**.</span><span class="sxs-lookup"><span data-stu-id="ec314-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="ec314-131">Assegnare il ruolo di amministratore del Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="ec314-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="ec314-132">Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace; sono necessari i parametri seguenti:</span><span class="sxs-lookup"><span data-stu-id="ec314-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="ec314-133">**TenantId:** L'ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).</span><span class="sxs-lookup"><span data-stu-id="ec314-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="ec314-134">**SubscriptionId:** Una sottoscrizione di cui l'amministratore globale ha un ruolo **collaboratore** o un livello superiore assegnato.</span><span class="sxs-lookup"><span data-stu-id="ec314-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="ec314-135">**GlobalAdminUsername:** Nome utente dell'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="ec314-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="ec314-136">**UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="ec314-137">Per gli utenti Guest invitati al tenant, potrebbero essere necessarie fino a 48 ore prima che l'account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="ec314-138">Per altre informazioni, vedere [proprietà di un Azure Active Directory utente di collaborazione B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="ec314-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="ec314-139">Per ulteriori informazioni sui cmdlet contenuti nel modulo AZ. Portal PowerShell, vedere [Microsoft Azure PowerShell: cmdlet del dashboard del portale](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="ec314-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="ec314-140">Crea Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="ec314-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="ec314-141">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ec314-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ec314-142">Selezionare **tutti i servizi** e quindi **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="ec314-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra la finestra principale portale di Azure.":::

3. <span data-ttu-id="ec314-144">Scegliere **Marketplace privato** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="ec314-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="ec314-145">Selezionare **inizia a creare** Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).</span><span class="sxs-lookup"><span data-stu-id="ec314-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra come selezionare la finestra principale ' inizia nella portale di Azure '.":::

    <span data-ttu-id="ec314-147">Se per questo tenant è già presente Azure Marketplace privato, per impostazione predefinita verrà selezionato **gestione Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="ec314-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="ec314-148">Al termine, sarà presente un Azure Marketplace privato vuoto e disabilitato.</span><span class="sxs-lookup"><span data-stu-id="ec314-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra la schermata privata vuota di Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="ec314-150">Aggiungi elementi dalla raccolta</span><span class="sxs-lookup"><span data-stu-id="ec314-150">Add items from gallery</span></span>

<span data-ttu-id="ec314-151">Un elemento è una combinazione di un'offerta e un piano.</span><span class="sxs-lookup"><span data-stu-id="ec314-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="ec314-152">È possibile cercare e aggiungere elementi nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="ec314-153">Selezionare **Aggiungi elementi**.</span><span class="sxs-lookup"><span data-stu-id="ec314-153">Select **Add items**.</span></span>

2. <span data-ttu-id="ec314-154">Sfogliare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.</span><span class="sxs-lookup"><span data-stu-id="ec314-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="ec314-155">[![Mostra come esplorare la raccolta o usare il campo di ricerca.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="ec314-156">Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco approvato.</span><span class="sxs-lookup"><span data-stu-id="ec314-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="ec314-157">Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani richiesti.</span><span class="sxs-lookup"><span data-stu-id="ec314-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Viene illustrato come aggiornare i piani richiesti.":::

4. <span data-ttu-id="ec314-159">Selezionare **done** in basso a sinistra dopo aver effettuato le selezioni.</span><span class="sxs-lookup"><span data-stu-id="ec314-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="ec314-160">**Gli elementi aggiunti** al Marketplace saranno disponibili solo per le offerte non Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ec314-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="ec314-161">Le soluzioni Microsoft (incluse le [distribuzioni Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) verranno contrassegnate come "approvate per impostazione predefinita" e non possono essere gestite in Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="ec314-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="ec314-162">Modificare i piani dell'elemento</span><span class="sxs-lookup"><span data-stu-id="ec314-162">Edit item's plans</span></span>

<span data-ttu-id="ec314-163">È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="ec314-164">Nella colonna **piani** rivedere i piani disponibili dal menu a discesa per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="ec314-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="ec314-165">Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.</span><span class="sxs-lookup"><span data-stu-id="ec314-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra come selezionare o deselezionare la casella di controllo per l'elemento richiesto.":::

> [!NOTE]
> <span data-ttu-id="ec314-167">Per ogni offerta è necessario almeno un piano selezionato per l'esecuzione dell'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="ec314-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="ec314-168">Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="ec314-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="ec314-169">Elimina offerte</span><span class="sxs-lookup"><span data-stu-id="ec314-169">Delete offers</span></span>

<span data-ttu-id="ec314-170">Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.</span><span class="sxs-lookup"><span data-stu-id="ec314-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="ec314-171">Abilita/Disabilita Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="ec314-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="ec314-172">Nella pagina Gestisci Marketplace viene visualizzato uno di questi banner, che mostra lo stato corrente di Azure Marketplace privato:</span><span class="sxs-lookup"><span data-stu-id="ec314-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra il banner &quot;Disabilita stato&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra il banner &quot;Abilita stato&quot;.":::

<span data-ttu-id="ec314-175">È possibile abilitare o disabilitare Azure Marketplace privato in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="ec314-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="ec314-176">Se disabilitato, selezionare **Abilita Marketplace privato** per abilitare.</span><span class="sxs-lookup"><span data-stu-id="ec314-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="ec314-177">Se abilitata, selezionare **Disabilita Marketplace privato** per disabilitare.</span><span class="sxs-lookup"><span data-stu-id="ec314-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="ec314-178">Centro notifiche di Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="ec314-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="ec314-179">Il centro notifiche è costituito da tre tipi di notifiche e consente all'amministratore del Marketplace di eseguire azioni in base alla notifica:</span><span class="sxs-lookup"><span data-stu-id="ec314-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="ec314-180">Richieste di approvazione da parte degli utenti per elementi non inclusi nell'elenco approvato (vedere la [richiesta di aggiunta di offerte o piani di](#request-to-add-offers-or-plans) seguito).</span><span class="sxs-lookup"><span data-stu-id="ec314-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="ec314-181">Nuove notifiche dei piani per le offerte che dispongono già di uno o più piani nell'elenco approvato.</span><span class="sxs-lookup"><span data-stu-id="ec314-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="ec314-182">Sono state rimosse le notifiche dei piani per gli elementi presenti nell'elenco approvato, ma sono stati rimossi dal Marketplace globale di Azure.</span><span class="sxs-lookup"><span data-stu-id="ec314-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="ec314-183">Per accedere al centro notifiche:</span><span class="sxs-lookup"><span data-stu-id="ec314-183">To access the notification center:</span></span>

1. <span data-ttu-id="ec314-184">Selezionare **notifiche** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="ec314-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="ec314-185">[![Consente di visualizzare il menu notifiche.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="ec314-186">Selezionare il menu con i puntini di sospensione per altre azioni.</span><span class="sxs-lookup"><span data-stu-id="ec314-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra i risultati del menu altre opzioni.":::

1. <span data-ttu-id="ec314-188">Per le richieste di piano, **Mostra richieste** apre il modulo di richiesta di approvazione, in cui è possibile esaminare tutte le richieste degli utenti per l'offerta specifica.</span><span class="sxs-lookup"><span data-stu-id="ec314-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="ec314-189">Selezionare **approva** o **rifiuta**.</span><span class="sxs-lookup"><span data-stu-id="ec314-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="ec314-190">[![Mostra le opzioni approva e rifiuta.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="ec314-191">Selezionare il piano da approvare dal menu a discesa.</span><span class="sxs-lookup"><span data-stu-id="ec314-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="ec314-192">Aggiungere un commento e selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="ec314-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="ec314-193">Esplorazione di Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="ec314-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="ec314-194">Quando Azure Marketplace privato è abilitato, gli utenti vedranno quali piani sono stati approvati dall'amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="ec314-195">Una notifica di **approvazione** verde indica un'offerta partner (non Microsoft) approvata.</span><span class="sxs-lookup"><span data-stu-id="ec314-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="ec314-196">Un avviso **approvato** da Blue indica un'offerta Microsoft (incluse le [distribuzioni Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)approvate) approvata.</span><span class="sxs-lookup"><span data-stu-id="ec314-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="ec314-197">Gli utenti possono filtrare tra le offerte che non sono approvate:</span><span class="sxs-lookup"><span data-stu-id="ec314-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="ec314-198">[![Mostra l'opzione di filtro.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="ec314-199">Acquistare o distribuire in Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="ec314-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="ec314-200">Anche se l'esperienza della pagina dei dettagli sul prodotto è simile a quella di Azure Marketplace globale, esistono tre scenari privati specifici di Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ec314-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="ec314-201">Quando un utente seleziona un piano approvato, viene abilitato il pulsante **Crea** :</span><span class="sxs-lookup"><span data-stu-id="ec314-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="ec314-202">[![Mostra il banner dell'offerta notando che è possibile creare un piano.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="ec314-203">Se la selezione di un piano del prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva quali piani sono stati approvati e il pulsante **Crea** è abilitato:</span><span class="sxs-lookup"><span data-stu-id="ec314-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="ec314-204">[![Mostra il banner dell'offerta, notando che è possibile creare un piano e visualizzare i piani disponibili.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="ec314-205">Quando un utente seleziona un piano non approvato, un banner annota il piano come non approvato e il pulsante **Crea** è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="ec314-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="ec314-206">L'utente può comunque richiedere di aggiungere il piano all'elenco approvato (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="ec314-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="ec314-207">Richiesta di aggiunta di offerte o piani</span><span class="sxs-lookup"><span data-stu-id="ec314-207">Request to add offers or plans</span></span>

<span data-ttu-id="ec314-208">È possibile richiedere l'aggiunta di un'offerta pubblica o di un piano non approvato in Azure Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="ec314-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="ec314-209">Selezionare la **richiesta da aggiungere** nel banner per aprire il **modulo di richiesta di accesso**.</span><span class="sxs-lookup"><span data-stu-id="ec314-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="ec314-210">[![Mostra il banner con il collegamento ' richiesta di aggiunta '.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="ec314-211">[![Mostra il modulo di richiesta di accesso per le offerte o i piani.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="ec314-212">Selezionare i piani da aggiungere alla richiesta.**qualsiasi piano** indica all'amministratore del Marketplace che non si ha una preferenza per un piano all'interno di un'offerta.</span><span class="sxs-lookup"><span data-stu-id="ec314-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="ec314-213">Aggiungere una **giustificazione** e selezionare la **richiesta** di invio della richiesta.</span><span class="sxs-lookup"><span data-stu-id="ec314-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="ec314-214">[![Mostra il modulo di richiesta di accesso per le offerte o i piani con le voci di esempio.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="ec314-215">Un'indicazione per una richiesta in sospeso verrà visualizzata nel modulo di richiesta di accesso con un'opzione per il **ritiro della richiesta**.</span><span class="sxs-lookup"><span data-stu-id="ec314-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="ec314-216">[![Mostra un elenco di piani approvati o in sospeso con collegamento richiesta di ritiro.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="ec314-217">Una volta inviato, il modulo di richiesta di approvazione verrà inviato al [Centro notifiche](#private-azure-marketplace-notification-center) per l'amministratore del Marketplace per esaminare la richiesta e intraprendere un'azione.</span><span class="sxs-lookup"><span data-stu-id="ec314-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="ec314-218">Domande frequenti (FAQ)</span><span class="sxs-lookup"><span data-stu-id="ec314-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="ec314-219">Si sta già bloccando l'applicazione Marketplace di terze parti tramite criteri di Azure.</span><span class="sxs-lookup"><span data-stu-id="ec314-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="ec314-220">Qual è la differenza?</span><span class="sxs-lookup"><span data-stu-id="ec314-220">How is this different?</span></span>

<span data-ttu-id="ec314-221">Esistono attualmente due modi per limitare i servizi di terze parti in Marketplace:</span><span class="sxs-lookup"><span data-stu-id="ec314-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="ec314-222">Tramite il portale EA o il portale di Azure disabilitare i servizi di terze parti o limitarsi a "solo SKU gratuiti o BYOL".</span><span class="sxs-lookup"><span data-stu-id="ec314-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Viene illustrato come limitare i servizi nel portale di Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Viene illustrato come limitare i servizi nel portale E.":::

2. <span data-ttu-id="ec314-225">Creare criteri di Azure per consentire solo macchine virtuali specifiche.</span><span class="sxs-lookup"><span data-stu-id="ec314-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="ec314-226">Per informazioni dettagliate su come applicare i criteri alle macchine virtuali Windows, vedere [applicare i criteri alle macchine virtuali Windows con Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="ec314-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="ec314-227">Azure Marketplace privato consente una maggiore flessibilità nella limitazione e nel consentire offerte e piani specifici.</span><span class="sxs-lookup"><span data-stu-id="ec314-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="ec314-228">Informa gli utenti finali sulla disponibilità per la distribuzione nella raccolta del Marketplace anche prima di provare a distribuire servizi di terze parti.</span><span class="sxs-lookup"><span data-stu-id="ec314-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="ec314-229">Per consentire la distribuzione di servizi di terze parti, impostare Azure Marketplace su attivato/abilitato nel portale EA e nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="ec314-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="ec314-230">Azure Marketplace privato può curare le soluzioni partner non limitate alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="ec314-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="ec314-231">Azure Marketplace privato può essere curato a livello di piano e può anche impostare "piano corrente e futuro".</span><span class="sxs-lookup"><span data-stu-id="ec314-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="ec314-232">Azure Marketplace privato può informare gli utenti finali sugli elementi che possono e non possono essere distribuiti.</span><span class="sxs-lookup"><span data-stu-id="ec314-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="ec314-233">Qual è la differenza tra un'offerta privata e Azure Marketplace privata?</span><span class="sxs-lookup"><span data-stu-id="ec314-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="ec314-234">Un' **offerta privata** consente agli editori di creare piani visibili solo ai clienti di destinazione.</span><span class="sxs-lookup"><span data-stu-id="ec314-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="ec314-235">In questo modo, è possibile condividere in privato soluzioni personalizzate con prezzi negoziati, termini e condizioni privati e configurazioni specializzate.</span><span class="sxs-lookup"><span data-stu-id="ec314-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="ec314-236">Per informazioni dettagliate, vedere [offerte private nel Marketplace commerciale](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="ec314-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="ec314-237">**Azure Marketplace privato** nella portale di Azure consente agli amministratori di approvare le soluzioni di terze parti che gli utenti possono distribuire.</span><span class="sxs-lookup"><span data-stu-id="ec314-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="ec314-238">Con Azure Marketplace privato, gli utenti possono usufruire dei vantaggi di Azure Marketplace individuando, acquistando e distribuendo offerte conformi.</span><span class="sxs-lookup"><span data-stu-id="ec314-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="ec314-239">Per gestire le offerte private basate su sottoscrizione nel Marketplace privato, l'amministratore del Marketplace deve avere almeno un ruolo di "lettura" per la sottoscrizione specifica.</span><span class="sxs-lookup"><span data-stu-id="ec314-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="ec314-240">È stata aggiunta un'offerta privata a Azure Marketplace privato, perché non viene visualizzata nella scheda Gestisci Marketplace?</span><span class="sxs-lookup"><span data-stu-id="ec314-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="ec314-241">Le offerte private basate su sottoscrizione sono visibili solo per le sottoscrizioni elencate nelle impostazioni dell'offerta privata.</span><span class="sxs-lookup"><span data-stu-id="ec314-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="ec314-242">Per visualizzare l'offerta privata, verificare che nel filtro della sottoscrizione globale siano visualizzate tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="ec314-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="ec314-243">[![Mostra il filtro del Marketplace privato.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ec314-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="ec314-244">Possiamo includere immagini personalizzate in Azure Marketplace privato?</span><span class="sxs-lookup"><span data-stu-id="ec314-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="ec314-245">No.</span><span class="sxs-lookup"><span data-stu-id="ec314-245">No.</span></span> <span data-ttu-id="ec314-246">Azure Marketplace privato consente a tutti gli amministratori IT di gestire e curare soluzioni di terze parti da Azure Marketplace globale.</span><span class="sxs-lookup"><span data-stu-id="ec314-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="ec314-247">Poiché le immagini personalizzate non sono presenti in Azure Marketplace globale, l'amministratore IT non può scegliere le immagini personalizzate.</span><span class="sxs-lookup"><span data-stu-id="ec314-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="ec314-248">Se si desidera condividere immagini personalizzate, utilizzare la [raccolta immagini condivise](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="ec314-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="ec314-249">Guida dettagliata creare una raccolta di immagini condivise (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="ec314-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="ec314-250">Creare una definizione di immagine all'interno di un SIG.</span><span class="sxs-lookup"><span data-stu-id="ec314-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="ec314-251">Il cliente deve scegliere **generalizzato** per il campo stato sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="ec314-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="ec314-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="ec314-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="ec314-253">Importare l'immagine gestita nella raccolta di immagini condivise ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="ec314-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="ec314-254">Le immagini di VM SIG si trovano in una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ec314-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="ec314-255">Per renderlo disponibile ad altre sottoscrizioni, usare una registrazione dell'app ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="ec314-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="ec314-256">Perché è possibile vedere che alcune offerte sono **approvate per impostazione predefinita,** anche se l'editore non è Microsoft?</span><span class="sxs-lookup"><span data-stu-id="ec314-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="ec314-257">Microsoft supporta Linux e la tecnologia open source in Azure.</span><span class="sxs-lookup"><span data-stu-id="ec314-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="ec314-258">Le [distribuzioni di Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) sono supportate in Azure e il prezzo è integrato nelle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="ec314-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="ec314-259">Poiché l'agente Linux di Azure è già preinstallato in Azure Marketplace, viene considerato come un'offerta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ec314-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="ec314-260">Poiché le offerte Microsoft sono approvate per impostazione predefinita, le distribuzioni di Linux approvate non possono essere gestite in Azure Marketplace privato e sono approvate per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="ec314-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="ec314-261">Contattare il supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="ec314-261">Contact support</span></span>

- <span data-ttu-id="ec314-262">Per il supporto di Azure Marketplace, visitare [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="ec314-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
