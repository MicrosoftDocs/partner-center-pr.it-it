---
title: Creare e gestire Azure Marketplace privato in portale di Azure
description: Informazioni sulla creazione e sulla gestione di Azure Marketplace privato (anteprima) nel portale di Azure. Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439251"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Creare e gestire Azure Marketplace privato (anteprima) nel portale di Azure

Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti. Questa operazione viene eseguita consentendo di distribuire solo le offerte approvate e conformi ai criteri dell'organizzazione. Con Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi per l'acquisto e la distribuzione. 

In qualità di amministratore del Marketplace (ruolo assegnato), si inizierà con un archivio privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati. Questo articolo illustra come creare, gestire e abilitare Azure Marketplace privato per gli utenti.

Note:

- Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant vedranno lo stesso elenco curato.
- Tutte le soluzioni Microsoft vengono aggiunte automaticamente ad Azure Marketplace privato.

## <a name="assign-the-marketplace-admin-role"></a>Assegnare il ruolo di amministratore del Marketplace

L'amministratore globale del tenant deve assegnare il ruolo di **amministratore del Marketplace** all'amministratore di Azure Marketplace privato che gestirà l'archivio privato.

>[!IMPORTANT]
> L'accesso alla gestione privata di Azure Marketplace è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.

### <a name="prerequisites"></a>Prerequisiti

Per poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant, è necessario soddisfare i prerequisiti seguenti:

- Si ha accesso a un utente **amministratore globale** .
- Il tenant ha almeno una sottoscrizione (può essere qualsiasi tipo).
- All'utente amministratore globale viene assegnato il ruolo **collaboratore** o superiore per la sottoscrizione scelta.
- L'accesso con privilegi elevati all'utente amministratore globale è impostato su **Sì** (vedere [elevare l'accesso per gestire tutti i gruppi di gestione e le sottoscrizioni di Azure](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Assegnare il ruolo di amministratore del Marketplace con PowerShell

Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace; sono necessari i parametri seguenti:

- **TenantId:** L'ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).
- **SubscriptionId:** Una sottoscrizione di cui l'amministratore globale ha un ruolo **collaboratore** o un livello superiore assegnato.
- **GlobalAdminUsername:** Nome utente dell'amministratore globale.
- **UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.

> [!NOTE]
> Per gli utenti Guest invitati al tenant, potrebbero essere necessarie fino a 48 ore prima che l'account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace. Per altre informazioni, vedere [proprietà di un Azure Active Directory utente di collaborazione B2B](/azure/active-directory/b2b/user-properties).

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

Per ulteriori informazioni sui cmdlet contenuti nel modulo AZ. Portal PowerShell, vedere [Microsoft Azure PowerShell: cmdlet del dashboard del portale](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Crea Azure Marketplace privato

1. Accedere al [portale di Azure](https://portal.azure.com/).
2. Selezionare **tutti i servizi** e quindi **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Portale di Azure finestra principale.":::

3. Selezionare **Marketplace privato** dalle opzioni a sinistra.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selezionare Marketplace privato nella finestra principale portale di Azure.":::

4. Selezionare **inizia a creare** Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selezionare inizia nella finestra principale portale di Azure.":::

    Se per questo tenant è già presente Azure Marketplace privato, per impostazione predefinita verrà selezionato **gestione Marketplace** .

5. Al termine, sarà presente un Azure Marketplace privato vuoto e disabilitato.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Schermata privata vuota di Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Aggiungi elementi dalla raccolta

Un elemento è una combinazione di un'offerta e un piano. È possibile cercare e aggiungere un elemento nella pagina Gestisci Marketplace.

1. Selezionare **Aggiungi elementi**.

2. Sfogliare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Esplorare la raccolta o usare il campo di ricerca.":::

3. Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco dei consentiti. Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani richiesti.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aggiornare i piani richiesti.":::

4. Selezionare **done** in basso a sinistra dopo aver effettuato le selezioni.

>[!Note]
> **Gli elementi aggiunti** al Marketplace saranno disponibili solo per le offerte non Microsoft. Le offerte Microsoft sono consentite per impostazione predefinita.

## <a name="edit-item-plans"></a>Modifica piani di elementi

È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.

1. Nella colonna **piani** rivedere i piani disponibili dal menu a discesa per l'elemento.
2. Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Selezionando o deselezionando la casella di controllo per l'elemento richiesto.":::

> [!NOTE]
> Per ogni offerta è necessario almeno un piano selezionato affinché l'aggiornamento venga eseguito. Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).

## <a name="delete-offers"></a>Elimina offerte

Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.

## <a name="enabledisable-private-azure-marketplace"></a>Abilita/Disabilita Azure Marketplace privato

Nella pagina Gestisci Marketplace viene visualizzato uno di questi banner, che mostra lo stato corrente di Azure Marketplace privato:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Disabilitare il banner di stato":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Abilita banner di stato":::

È possibile abilitare o disabilitare Azure Marketplace privato in base alle esigenze.

1. Se disabilitato, selezionare **Abilita Marketplace privato** per abilitare.
2. Se abilitata, selezionare **Disabilita Marketplace privato** per disabilitare.

## <a name="browsing-private-azure-marketplace"></a>Esplorazione di Azure Marketplace privato

Quando Azure Marketplace privato è abilitato, gli utenti vedranno quali piani sono consentiti dall'amministratore del Marketplace.

- Un avviso verde **consentito** indica un'offerta partner (non Microsoft) consentita.
- Un avviso blu **consentito** indica un'offerta Microsoft consentita.

Gli utenti possono filtrare tra le offerte che non sono consentite:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opzione di filtro.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Acquistare o distribuire in Azure Marketplace privato

Anche se l'esperienza della pagina dei dettagli sul prodotto è simile a quella del Marketplace pubblico di Azure, esistono tre scenari privati specifici di Azure Marketplace.

- Quando un utente seleziona un piano consentito, viene abilitato il pulsante **Crea** :

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Banner offerta che consente di creare un piano.":::

- Quando un utente seleziona un piano non consentito, un banner rileva che il piano non è consentito e il pulsante **Crea** è disabilitato.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Non è possibile creare il banner dell'offerta notando un piano.":::

- Se la selezione di un piano del prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva quali piani sono consentiti e il pulsante **Crea** è abilitato:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner dell'offerta che indica che è possibile creare un piano e visualizzare i piani disponibili.":::

## <a name="contact-support"></a>Contattare il supporto tecnico

Per il supporto di Azure Marketplace, visitare [Microsoft Q&A](/answers/products/). 
