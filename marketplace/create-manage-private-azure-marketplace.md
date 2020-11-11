---
title: Creare e gestire Azure Marketplace privato in portale di Azure
description: Informazioni sulla creazione e sulla gestione di Azure Marketplace privato (anteprima) nel portale di Azure.
ms.prod: marketplace-customer
ms.topic: article
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 1333bb2c8830cec83d7b7f05890af818d5c0ce5b
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/11/2020
ms.locfileid: "94487704"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="7b7f4-103">Creare e gestire Azure Marketplace privato (anteprima) nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="7b7f4-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="7b7f4-104">Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="7b7f4-105">Questa operazione viene eseguita consentendo di distribuire solo le offerte approvate e conformi ai criteri dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="7b7f4-106">Con Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi per l'acquisto e la distribuzione.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="7b7f4-107">In qualità di amministratore del Marketplace (ruolo assegnato), si inizierà con un archivio privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="7b7f4-108">Questo articolo illustra come creare, gestire e abilitare Azure Marketplace privato per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="7b7f4-109">Note:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-109">Notes:</span></span>

- <span data-ttu-id="7b7f4-110">Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant vedranno lo stesso elenco curato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="7b7f4-111">Tutte le soluzioni Microsoft vengono aggiunte automaticamente ad Azure Marketplace privato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="7b7f4-112">Assegnare il ruolo di amministratore del Marketplace</span><span class="sxs-lookup"><span data-stu-id="7b7f4-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="7b7f4-113">L'amministratore globale del tenant deve assegnare il ruolo di **amministratore del Marketplace** all'amministratore di Azure Marketplace privato che gestirà l'archivio privato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="7b7f4-114">L'accesso alla gestione privata di Azure Marketplace è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="7b7f4-115">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="7b7f4-115">Prerequisites</span></span>

<span data-ttu-id="7b7f4-116">Per poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant, è necessario soddisfare i prerequisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="7b7f4-117">Si ha accesso a un utente **amministratore globale** .</span><span class="sxs-lookup"><span data-stu-id="7b7f4-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="7b7f4-118">Il tenant ha almeno una sottoscrizione (può essere qualsiasi tipo).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="7b7f4-119">All'utente amministratore globale viene assegnato il ruolo **collaboratore** o superiore per la sottoscrizione scelta nel passaggio 2.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="7b7f4-120">L'accesso con privilegi elevati all'utente amministratore globale è impostato su **Sì** (vedere [elevate-Access-Global-Admin](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="7b7f4-121">Assegnare il ruolo di amministratore del Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="7b7f4-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="7b7f4-122">Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace; sono necessari i parametri seguenti:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="7b7f4-123">**TenantId:** L'ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="7b7f4-124">**SubscriptionId:** Una sottoscrizione di cui l'amministratore globale ha un ruolo **collaboratore** o un livello superiore assegnato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="7b7f4-125">**GlobalAdminUsername:** Nome utente dell'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="7b7f4-126">**UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="7b7f4-127">Per gli utenti Guest invitati al tenant, potrebbero essere necessarie fino a 48 ore prima che l'account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="7b7f4-128">Per altre informazioni, vedere [proprietà di un Azure Active Directory utente di collaborazione B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="7b7f4-129">Per ulteriori informazioni sui cmdlet contenuti nel modulo AZ. Portal PowerShell, vedere [Microsoft Azure PowerShell: cmdlet del dashboard del portale](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="7b7f4-130">Crea Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="7b7f4-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="7b7f4-131">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7b7f4-132">Selezionare **tutti i servizi** e quindi **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portale di Azure finestra principale.":::

3. <span data-ttu-id="7b7f4-134">Selezionare **Marketplace privato** dalle opzioni a sinistra.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selezionare Marketplace privato nella finestra principale portale di Azure.":::

4. <span data-ttu-id="7b7f4-136">Selezionare **inizia a creare** Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selezionare inizia nella finestra principale portale di Azure.":::

    <span data-ttu-id="7b7f4-138">Se per questo tenant è già presente Azure Marketplace privato, per impostazione predefinita verrà selezionato **gestione Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="7b7f4-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="7b7f4-139">Al termine, sarà presente un Azure Marketplace privato vuoto e disabilitato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Schermata privata vuota di Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="7b7f4-141">Aggiungi elementi dalla raccolta</span><span class="sxs-lookup"><span data-stu-id="7b7f4-141">Add items from gallery</span></span>

<span data-ttu-id="7b7f4-142">Un elemento è una combinazione di un'offerta e un piano.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="7b7f4-143">È possibile cercare e aggiungere un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7b7f4-144">Selezionare **Aggiungi elementi**.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-144">Select **Add items**.</span></span>

2. <span data-ttu-id="7b7f4-145">Sfogliare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Esplorare la raccolta o usare il campo di ricerca.":::

3. <span data-ttu-id="7b7f4-147">Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco dei consentiti.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="7b7f4-148">Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani richiesti.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aggiornare i piani richiesti.":::

4. <span data-ttu-id="7b7f4-150">Selezionare **done** in basso a sinistra dopo aver effettuato le selezioni.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="7b7f4-151">**Gli elementi aggiunti** al Marketplace saranno disponibili solo per le offerte non Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="7b7f4-152">Le offerte Microsoft sono consentite per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="7b7f4-153">Modifica piani di elementi</span><span class="sxs-lookup"><span data-stu-id="7b7f4-153">Edit item plans</span></span>

<span data-ttu-id="7b7f4-154">È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7b7f4-155">Nella colonna **piani** rivedere i piani disponibili dal menu a discesa per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="7b7f4-156">Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Selezionando o deselezionando la casella di controllo per l'elemento richiesto.":::

> [!NOTE]
> <span data-ttu-id="7b7f4-158">Per ogni offerta è necessario almeno un piano selezionato affinché l'aggiornamento venga eseguito.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="7b7f4-159">Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="7b7f4-160">Elimina offerte</span><span class="sxs-lookup"><span data-stu-id="7b7f4-160">Delete offers</span></span>

<span data-ttu-id="7b7f4-161">Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="7b7f4-162">Abilita/Disabilita Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="7b7f4-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="7b7f4-163">Nella pagina Gestisci Marketplace viene visualizzato uno di questi banner, che mostra lo stato corrente di Azure Marketplace privato:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Disabilitare il banner di stato":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Abilita banner di stato":::

<span data-ttu-id="7b7f4-166">È possibile abilitare o disabilitare Azure Marketplace privato in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="7b7f4-167">Se disabilitato, selezionare **Abilita Marketplace privato** per abilitare.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="7b7f4-168">Se abilitata, selezionare **Disabilita Marketplace privato** per disabilitare.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="7b7f4-169">Esplorazione di Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="7b7f4-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="7b7f4-170">Quando Azure Marketplace privato è abilitato, gli utenti vedranno quali piani sono consentiti dall'amministratore del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="7b7f4-171">Un avviso verde **consentito** indica un'offerta partner (non Microsoft) consentita.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="7b7f4-172">Un avviso blu **consentito** indica un'offerta Microsoft consentita.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="7b7f4-173">Gli utenti possono filtrare tra le offerte che non sono consentite:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opzione di filtro.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="7b7f4-175">Acquistare o distribuire in Azure Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="7b7f4-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="7b7f4-176">Anche se l'esperienza della pagina dei dettagli sul prodotto è simile a quella del Marketplace pubblico di Azure, esistono tre scenari privati specifici di Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="7b7f4-177">Quando un utente seleziona un piano consentito, viene abilitato il pulsante **Crea** :</span><span class="sxs-lookup"><span data-stu-id="7b7f4-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Banner offerta che consente di creare un piano.":::

- <span data-ttu-id="7b7f4-179">Quando un utente seleziona un piano non consentito, un banner rileva che il piano non è consentito e il pulsante **Crea** è disabilitato.</span><span class="sxs-lookup"><span data-stu-id="7b7f4-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Non è possibile creare il banner dell'offerta notando un piano.":::

- <span data-ttu-id="7b7f4-181">Se la selezione di un piano del prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva quali piani sono consentiti e il pulsante **Crea** è abilitato:</span><span class="sxs-lookup"><span data-stu-id="7b7f4-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner dell'offerta che indica che è possibile creare un piano e visualizzare i piani disponibili.":::

## <a name="contact-support"></a><span data-ttu-id="7b7f4-183">Contattare il supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="7b7f4-183">Contact support</span></span>

<span data-ttu-id="7b7f4-184">Per il supporto di Azure Marketplace, visitare [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="7b7f4-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
