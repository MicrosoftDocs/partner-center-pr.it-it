---
title: Creare e gestire Azure Marketplace privato in portale di Azure
description: Informazioni sulla creazione e sulla gestione di Azure Marketplace privato (anteprima) nel portale di Azure. Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760831"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="32d7b-104">Creare e gestire Azure Marketplace privato (anteprima) nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="32d7b-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="32d7b-105">Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.</span><span class="sxs-lookup"><span data-stu-id="32d7b-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="32d7b-106">Questa operazione viene eseguita consentendo di distribuire solo le offerte approvate e conformi ai criteri dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="32d7b-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="32d7b-107">Con Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi per l'acquisto e la distribuzione.</span><span class="sxs-lookup"><span data-stu-id="32d7b-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="32d7b-108">In qualità di amministratore del Marketplace (ruolo assegnato), si inizierà con un archivio privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati.</span><span class="sxs-lookup"><span data-stu-id="32d7b-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="32d7b-109">Questo articolo illustra come creare, gestire e abilitare Azure Marketplace privato per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="32d7b-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="32d7b-110">Note:</span><span class="sxs-lookup"><span data-stu-id="32d7b-110">Notes:</span></span>

- <span data-ttu-id="32d7b-111">Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant vedranno lo stesso elenco curato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="32d7b-112">Tutte le soluzioni Microsoft vengono aggiunte automaticamente ad Azure Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="32d7b-113">Assegnare il ruolo di amministratore del Marketplace</span><span class="sxs-lookup"><span data-stu-id="32d7b-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="32d7b-114">L'amministratore globale del tenant deve assegnare il ruolo di **amministratore del Marketplace** all'amministratore di Azure Marketplace privato che gestirà l'archivio privato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="32d7b-115">L'accesso alla gestione privata di Azure Marketplace è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="32d7b-116">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="32d7b-116">Prerequisites</span></span>

<span data-ttu-id="32d7b-117">Per poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant, è necessario soddisfare i prerequisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="32d7b-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="32d7b-118">Si ha accesso a un utente **amministratore globale** .</span><span class="sxs-lookup"><span data-stu-id="32d7b-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="32d7b-119">Il tenant ha almeno una sottoscrizione (può essere qualsiasi tipo).</span><span class="sxs-lookup"><span data-stu-id="32d7b-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="32d7b-120">All'utente amministratore globale viene assegnato il ruolo **collaboratore** o superiore per la sottoscrizione scelta.</span><span class="sxs-lookup"><span data-stu-id="32d7b-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="32d7b-121">Assegnare il ruolo di amministratore del Marketplace con IAM</span><span class="sxs-lookup"><span data-stu-id="32d7b-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="32d7b-122">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="32d7b-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="32d7b-123">Selezionare **tutti i servizi** e quindi **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portale di Azure finestra principale.":::

3. <span data-ttu-id="32d7b-125">Selezionare **Marketplace privato** dalle opzioni a sinistra.</span><span class="sxs-lookup"><span data-stu-id="32d7b-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="32d7b-126">Selezionare **controllo di accesso (IAM)** per assegnare il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Schermata di controllo di accesso IAM.":::

1. <span data-ttu-id="32d7b-128">Selezionare **Aggiungi** > **Aggiungi assegnazione di ruolo**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="32d7b-129">In **ruolo** scegliere **amministrazione del Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Menu assegnazione ruolo.":::

1. <span data-ttu-id="32d7b-131">Selezionare l'utente desiderato nell'elenco a discesa, quindi fare clic su **fine**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="32d7b-132">Assegnare il ruolo di amministratore del Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="32d7b-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="32d7b-133">Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace; sono necessari i parametri seguenti:</span><span class="sxs-lookup"><span data-stu-id="32d7b-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="32d7b-134">**TenantId:** L'ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).</span><span class="sxs-lookup"><span data-stu-id="32d7b-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="32d7b-135">**SubscriptionId:** Una sottoscrizione di cui l'amministratore globale ha un ruolo **collaboratore** o un livello superiore assegnato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="32d7b-136">**GlobalAdminUsername:** Nome utente dell'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="32d7b-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="32d7b-137">**UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="32d7b-138">Per gli utenti Guest invitati al tenant, potrebbero essere necessarie fino a 48 ore prima che l'account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="32d7b-139">Per altre informazioni, vedere [proprietà di un Azure Active Directory utente di collaborazione B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="32d7b-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="32d7b-140">Per ulteriori informazioni sui cmdlet contenuti nel modulo AZ. Portal PowerShell, vedere [Microsoft Azure PowerShell: cmdlet del dashboard del portale](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="32d7b-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="32d7b-141">Crea Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="32d7b-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="32d7b-142">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="32d7b-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="32d7b-143">Selezionare **tutti i servizi** e quindi **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portale di Azure finestra principale.":::

3. <span data-ttu-id="32d7b-145">Selezionare **Marketplace privato** dalle opzioni a sinistra.</span><span class="sxs-lookup"><span data-stu-id="32d7b-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selezionare Marketplace privato nella finestra principale portale di Azure.":::

4. <span data-ttu-id="32d7b-147">Selezionare **inizia a creare** Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).</span><span class="sxs-lookup"><span data-stu-id="32d7b-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selezionare inizia nella finestra principale portale di Azure.":::

    <span data-ttu-id="32d7b-149">Se per questo tenant è già presente Azure Marketplace privato, per impostazione predefinita verrà selezionato **gestione Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="32d7b-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="32d7b-150">Al termine, sarà presente un Azure Marketplace privato vuoto e disabilitato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Schermata privata vuota di Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="32d7b-152">Aggiungi elementi dalla raccolta</span><span class="sxs-lookup"><span data-stu-id="32d7b-152">Add items from gallery</span></span>

<span data-ttu-id="32d7b-153">Un elemento è una combinazione di un'offerta e un piano.</span><span class="sxs-lookup"><span data-stu-id="32d7b-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="32d7b-154">È possibile cercare e aggiungere un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="32d7b-155">Selezionare **Aggiungi elementi**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-155">Select **Add items**.</span></span>

2. <span data-ttu-id="32d7b-156">Sfogliare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Esplorare la raccolta o usare il campo di ricerca.":::

3. <span data-ttu-id="32d7b-158">Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco dei consentiti.</span><span class="sxs-lookup"><span data-stu-id="32d7b-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="32d7b-159">Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani richiesti.</span><span class="sxs-lookup"><span data-stu-id="32d7b-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aggiornare i piani richiesti.":::

4. <span data-ttu-id="32d7b-161">Selezionare **done** in basso a sinistra dopo aver effettuato le selezioni.</span><span class="sxs-lookup"><span data-stu-id="32d7b-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="32d7b-162">**Gli elementi aggiunti** al Marketplace saranno disponibili solo per le offerte non Microsoft.</span><span class="sxs-lookup"><span data-stu-id="32d7b-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="32d7b-163">Le offerte Microsoft sono consentite per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="32d7b-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="32d7b-164">Modifica piani di elementi</span><span class="sxs-lookup"><span data-stu-id="32d7b-164">Edit item plans</span></span>

<span data-ttu-id="32d7b-165">È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="32d7b-166">Nella colonna **piani** rivedere i piani disponibili dal menu a discesa per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="32d7b-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="32d7b-167">Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.</span><span class="sxs-lookup"><span data-stu-id="32d7b-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Selezionando o deselezionando la casella di controllo per l'elemento richiesto.":::

> [!NOTE]
> <span data-ttu-id="32d7b-169">Per ogni offerta è necessario almeno un piano selezionato affinché l'aggiornamento venga eseguito.</span><span class="sxs-lookup"><span data-stu-id="32d7b-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="32d7b-170">Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="32d7b-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="32d7b-171">Elimina offerte</span><span class="sxs-lookup"><span data-stu-id="32d7b-171">Delete offers</span></span>

<span data-ttu-id="32d7b-172">Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.</span><span class="sxs-lookup"><span data-stu-id="32d7b-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="32d7b-173">Abilita/Disabilita Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="32d7b-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="32d7b-174">Nella pagina Gestisci Marketplace viene visualizzato uno di questi banner, che mostra lo stato corrente di Azure Marketplace privato:</span><span class="sxs-lookup"><span data-stu-id="32d7b-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Disabilitare il banner di stato":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Abilita banner di stato":::

<span data-ttu-id="32d7b-177">È possibile abilitare o disabilitare Azure Marketplace privato in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="32d7b-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="32d7b-178">Se disabilitato, selezionare **Abilita Marketplace privato** per abilitare.</span><span class="sxs-lookup"><span data-stu-id="32d7b-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="32d7b-179">Se abilitata, selezionare **Disabilita Marketplace privato** per disabilitare.</span><span class="sxs-lookup"><span data-stu-id="32d7b-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="32d7b-180">Esplorazione di Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="32d7b-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="32d7b-181">Quando Azure Marketplace privato è abilitato, gli utenti vedranno quali piani sono consentiti dall'amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="32d7b-182">Un avviso verde **consentito** indica un'offerta partner (non Microsoft) consentita.</span><span class="sxs-lookup"><span data-stu-id="32d7b-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="32d7b-183">Un avviso blu **consentito** indica un'offerta Microsoft consentita.</span><span class="sxs-lookup"><span data-stu-id="32d7b-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="32d7b-184">Gli utenti possono filtrare tra le offerte che non sono consentite:</span><span class="sxs-lookup"><span data-stu-id="32d7b-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opzione di filtro.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="32d7b-186">Acquistare o distribuire in Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="32d7b-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="32d7b-187">Anche se l'esperienza della pagina dei dettagli sul prodotto è simile a quella del Marketplace pubblico di Azure, esistono tre scenari privati specifici di Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="32d7b-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="32d7b-188">Quando un utente seleziona un piano consentito, viene abilitato il pulsante **Crea** :</span><span class="sxs-lookup"><span data-stu-id="32d7b-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Banner offerta che consente di creare un piano.":::

- <span data-ttu-id="32d7b-190">Quando un utente seleziona un piano non consentito, un banner rileva che il piano non è consentito e il pulsante **Crea** è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="32d7b-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Non è possibile creare il banner dell'offerta notando un piano.":::

- <span data-ttu-id="32d7b-192">Se la selezione di un piano del prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva quali piani sono consentiti e il pulsante **Crea** è abilitato:</span><span class="sxs-lookup"><span data-stu-id="32d7b-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner dell'offerta che indica che è possibile creare un piano e visualizzare i piani disponibili.":::

## <a name="contact-support"></a><span data-ttu-id="32d7b-194">Contattare il supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="32d7b-194">Contact support</span></span>

<span data-ttu-id="32d7b-195">Per il supporto di Azure Marketplace, visitare [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="32d7b-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
