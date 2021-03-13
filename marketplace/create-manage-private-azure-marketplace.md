---
title: Creare e gestire Azure Marketplace privato nel portale di Azure
description: Informazioni sulla creazione e sulla gestione di Azure Marketplace privato (anteprima) nel portale di Azure. Azure Marketplace privato (anteprima) consente agli amministratori di governare le soluzioni di terze parti che possono essere usate dagli utenti.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: dbd67ee1d4e9775d37318ec6389888f03a50b6ec
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412710"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Creare e gestire Azure Marketplace privato nel portale di Azure

Azure Marketplace privato consente agli amministratori di gestire le soluzioni di terze parti che possono essere usate dagli utenti. Questa operazione viene eseguita consentendo all'utente di distribuire solo le offerte approvate dall'amministratore ed essere conformi ai criteri dell'organizzazione. Con Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi per l'acquisto e la distribuzione.

In qualità di amministratore del Marketplace (ruolo assegnato), si inizierà con un archivio privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati. Questo articolo illustra come assegnare il ruolo necessario, creare un archivio privato, gestire gli elementi, approvare le richieste degli utenti e abilitare Azure Marketplace privato per gli utenti.

> [!NOTE]
> - Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant vedranno lo stesso elenco curato.
> - Tutte le soluzioni Microsoft (incluse le [distribuzioni Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) vengono aggiunte automaticamente ad Azure Marketplace privato.

## <a name="assign-the-marketplace-admin-role"></a>Assegnare il ruolo di amministratore del Marketplace

L'amministratore globale del tenant deve assegnare il ruolo di **amministratore del Marketplace** all'amministratore di Azure Marketplace privato che gestirà l'archivio privato.

>[!IMPORTANT]
> L'accesso alla gestione privata di Azure Marketplace è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.

### <a name="prerequisites"></a>Prerequisiti

Questi prerequisiti sono necessari per poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant:

- Si ha accesso a un utente **amministratore globale** .
- Il tenant ha almeno una sottoscrizione (può essere qualsiasi tipo).
- All'utente amministratore globale viene assegnato il ruolo **collaboratore** o superiore per la sottoscrizione scelta.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Assegnare il ruolo di amministratore del Marketplace con controllo di accesso (IAM)

1. Accedere al [portale di Azure](https://portal.azure.com/).
1. Selezionare **tutti i servizi** e quindi **Marketplace**.
1. Scegliere **Marketplace privato** dal menu a sinistra.

    [![Mostra l'opzione di menu Marketplace privato sul lato sinistro del Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Selezionare **controllo di accesso (IAM)** per assegnare il ruolo di amministratore del Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra la schermata di controllo di accesso A M.":::

1. Selezionare **Aggiungi** > **Aggiungi assegnazione di ruolo**.
1. In **ruolo** scegliere **amministrazione del Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Consente di visualizzare il menu assegnazione ruolo.":::

1. Selezionare l'utente desiderato nell'elenco a discesa, quindi fare clic su **fine**.

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

Per ulteriori informazioni sui cmdlet contenuti nel modulo AZ. Portal PowerShell, vedere [Microsoft Azure PowerShell: cmdlet del dashboard del portale](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Crea Azure Marketplace privato

1. Accedere al [portale di Azure](https://portal.azure.com/).
2. Selezionare **tutti i servizi** e quindi **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra la finestra principale portale di Azure.":::

3. Scegliere **Marketplace privato** dal menu a sinistra.

4. Selezionare **inizia a creare** Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Mostra come selezionare la finestra principale ' inizia nella portale di Azure '.":::

    Se per questo tenant è già presente Azure Marketplace privato, per impostazione predefinita verrà selezionato **gestione Marketplace** .

5. Al termine, sarà presente un Azure Marketplace privato vuoto e disabilitato.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra la schermata privata vuota di Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Aggiungi elementi dalla raccolta

Un elemento è una combinazione di un'offerta e un piano. È possibile cercare e aggiungere elementi nella pagina Gestisci Marketplace.

1. Selezionare **Aggiungi elementi**.

2. Sfogliare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.

    [![Mostra come esplorare la raccolta o usare il campo di ricerca.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco approvato. Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani richiesti.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Viene illustrato come aggiornare i piani richiesti.":::

4. Selezionare **done** in basso a sinistra dopo aver effettuato le selezioni.

>[!Note]
> **Gli elementi aggiunti** al Marketplace saranno disponibili solo per le offerte non Microsoft. Le soluzioni Microsoft (incluse le [distribuzioni Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) verranno contrassegnate come "approvate per impostazione predefinita" e non possono essere gestite in Marketplace privato.

## <a name="edit-items-plans"></a>Modificare i piani dell'elemento

È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.

1. Nella colonna **piani** rivedere i piani disponibili dal menu a discesa per l'elemento.
2. Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra come selezionare o deselezionare la casella di controllo per l'elemento richiesto.":::

> [!NOTE]
> Per ogni offerta è necessario almeno un piano selezionato per l'esecuzione dell'aggiornamento. Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).

## <a name="delete-offers"></a>Elimina offerte

Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.

## <a name="enabledisable-private-azure-marketplace"></a>Abilita/Disabilita Azure Marketplace privato

Nella pagina Gestisci Marketplace viene visualizzato uno di questi banner, che mostra lo stato corrente di Azure Marketplace privato:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra il banner &quot;Disabilita stato&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra il banner &quot;Abilita stato&quot;.":::

È possibile abilitare o disabilitare Azure Marketplace privato in base alle esigenze.

- Se disabilitato, selezionare **Abilita Marketplace privato** per abilitare.
- Se abilitata, selezionare **Disabilita Marketplace privato** per disabilitare.

## <a name="private-azure-marketplace-notification-center"></a>Centro notifiche di Azure Marketplace privato

Il centro notifiche è costituito da tre tipi di notifiche e consente all'amministratore del Marketplace di eseguire azioni in base alla notifica:

- Richieste di approvazione da parte degli utenti per elementi non inclusi nell'elenco approvato (vedere la [richiesta di aggiunta di offerte o piani di](#request-to-add-offers-or-plans) seguito).
- Nuove notifiche dei piani per le offerte che dispongono già di uno o più piani nell'elenco approvato.
- Sono state rimosse le notifiche dei piani per gli elementi presenti nell'elenco approvato, ma sono stati rimossi dal Marketplace globale di Azure.

Per accedere al centro notifiche:

1. Selezionare **notifiche** dal menu a sinistra.

    [![Consente di visualizzare il menu notifiche.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Selezionare il menu con i puntini di sospensione per altre azioni.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra i risultati del menu altre opzioni.":::

1. Per le richieste di piano, **Mostra richieste** apre il modulo di richiesta di approvazione, in cui è possibile esaminare tutte le richieste degli utenti per l'offerta specifica.
1. Selezionare **approva** o **rifiuta**.

    [![Mostra le opzioni approva e rifiuta.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Selezionare il piano da approvare dal menu a discesa.
1. Aggiungere un commento e selezionare **Submit (Invia**).

## <a name="browsing-private-azure-marketplace"></a>Esplorazione di Azure Marketplace privato

Quando Azure Marketplace privato è abilitato, gli utenti vedranno quali piani sono stati approvati dall'amministratore del Marketplace.

- Una notifica di **approvazione** verde indica un'offerta partner (non Microsoft) approvata.
- Un avviso **approvato** da Blue indica un'offerta Microsoft (incluse le [distribuzioni Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)approvate) approvata.

Gli utenti possono filtrare tra le offerte che non sono approvate:

[![Mostra l'opzione di filtro.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Acquistare o distribuire in Azure Marketplace privato

Anche se l'esperienza della pagina dei dettagli sul prodotto è simile a quella di Azure Marketplace globale, esistono tre scenari privati specifici di Azure Marketplace.

- Quando un utente seleziona un piano approvato, viene abilitato il pulsante **Crea** :

    [![Mostra il banner dell'offerta notando che è possibile creare un piano.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Se la selezione di un piano del prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva quali piani sono stati approvati e il pulsante **Crea** è abilitato:

    [![Mostra il banner dell'offerta, notando che è possibile creare un piano e visualizzare i piani disponibili.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Quando un utente seleziona un piano non approvato, un banner annota il piano come non approvato e il pulsante **Crea** è disabilitato. L'utente può comunque richiedere di aggiungere il piano all'elenco approvato (vedere la sezione successiva).

## <a name="request-to-add-offers-or-plans"></a>Richiesta di aggiunta di offerte o piani

È possibile richiedere l'aggiunta di un'offerta pubblica o di un piano non approvato in Azure Marketplace privato.

1. Selezionare la **richiesta da aggiungere** nel banner per aprire il **modulo di richiesta di accesso**.

    [![Mostra il banner con il collegamento ' richiesta di aggiunta '.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Mostra il modulo di richiesta di accesso per le offerte o i piani.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Selezionare i piani da aggiungere alla richiesta.**qualsiasi piano** indica all'amministratore del Marketplace che non si ha una preferenza per un piano all'interno di un'offerta.

1. Aggiungere una **giustificazione** e selezionare la **richiesta** di invio della richiesta.
  
    [![Mostra il modulo di richiesta di accesso per le offerte o i piani con le voci di esempio.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Un'indicazione per una richiesta in sospeso verrà visualizzata nel modulo di richiesta di accesso con un'opzione per il **ritiro della richiesta**.

    [![Mostra un elenco di piani approvati o in sospeso con collegamento richiesta di ritiro.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Una volta inviato, il modulo di richiesta di approvazione verrà inviato al [Centro notifiche](#private-azure-marketplace-notification-center) per l'amministratore del Marketplace per esaminare la richiesta e intraprendere un'azione.

## <a name="frequently-asked-questions-faqs"></a>Domande frequenti (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Si sta già bloccando l'applicazione Marketplace di terze parti tramite criteri di Azure. Qual è la differenza?

Esistono attualmente due modi per limitare i servizi di terze parti in Marketplace:

1. Tramite il portale EA o il portale di Azure disabilitare i servizi di terze parti o limitarsi a "solo SKU gratuiti o BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Viene illustrato come limitare i servizi nel portale di Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Viene illustrato come limitare i servizi nel portale E.":::

2. Creare criteri di Azure per consentire solo macchine virtuali specifiche. Per informazioni dettagliate su come applicare i criteri alle macchine virtuali Windows, vedere [applicare i criteri alle macchine virtuali Windows con Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).

Azure Marketplace privato consente una maggiore flessibilità nella limitazione e nel consentire offerte e piani specifici. Informa gli utenti finali sulla disponibilità per la distribuzione nella raccolta del Marketplace anche prima di provare a distribuire servizi di terze parti. Per consentire la distribuzione di servizi di terze parti, impostare Azure Marketplace su attivato/abilitato nel portale EA e nel portale di Azure.

- Azure Marketplace privato può curare le soluzioni partner non limitate alle macchine virtuali.
- Azure Marketplace privato può essere curato a livello di piano e può anche impostare "piano corrente e futuro".
- Azure Marketplace privato può informare gli utenti finali sugli elementi che possono e non possono essere distribuiti.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Qual è la differenza tra un'offerta privata e Azure Marketplace privata?

Un' **offerta privata** consente agli editori di creare piani visibili solo ai clienti di destinazione. In questo modo, è possibile condividere in privato soluzioni personalizzate con prezzi negoziati, termini e condizioni privati e configurazioni specializzate. Per informazioni dettagliate, vedere [offerte private nel Marketplace commerciale](https://docs.microsoft.com/azure/marketplace/private-offers).

**Azure Marketplace privato** nella portale di Azure consente agli amministratori di approvare le soluzioni di terze parti che gli utenti possono distribuire. Con Azure Marketplace privato, gli utenti possono usufruire dei vantaggi di Azure Marketplace individuando, acquistando e distribuendo offerte conformi. Per gestire le offerte private basate su sottoscrizione nel Marketplace privato, l'amministratore del Marketplace deve avere almeno un ruolo di "lettura" per la sottoscrizione specifica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>È stata aggiunta un'offerta privata a Azure Marketplace privato, perché non viene visualizzata nella scheda Gestisci Marketplace?

Le offerte private basate su sottoscrizione sono visibili solo per le sottoscrizioni elencate nelle impostazioni dell'offerta privata. Per visualizzare l'offerta privata, verificare che nel filtro della sottoscrizione globale siano visualizzate tutte le sottoscrizioni.

[![Mostra il filtro del Marketplace privato.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Possiamo includere immagini personalizzate in Azure Marketplace privato?

No. Azure Marketplace privato consente a tutti gli amministratori IT di gestire e curare soluzioni di terze parti da Azure Marketplace globale. Poiché le immagini personalizzate non sono presenti in Azure Marketplace globale, l'amministratore IT non può scegliere le immagini personalizzate. Se si desidera condividere immagini personalizzate, utilizzare la [raccolta immagini condivise](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).

1. Guida dettagliata creare una raccolta di immagini condivise (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).
2. Creare una definizione di immagine all'interno di un SIG. Il cliente deve scegliere **generalizzato** per il campo stato sistema operativo. ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Importare l'immagine gestita nella raccolta di immagini condivise ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).
4. Le immagini di VM SIG si trovano in una sottoscrizione. Per renderlo disponibile ad altre sottoscrizioni, usare una registrazione dell'app ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Perché è possibile vedere che alcune offerte sono **approvate per impostazione predefinita,** anche se l'editore non è Microsoft?

Microsoft supporta Linux e la tecnologia open source in Azure. Le [distribuzioni di Linux approvate](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) sono supportate in Azure e il prezzo è integrato nelle macchine virtuali. Poiché l'agente Linux di Azure è già preinstallato in Azure Marketplace, viene considerato come un'offerta Microsoft. Poiché le offerte Microsoft sono approvate per impostazione predefinita, le distribuzioni di Linux approvate non possono essere gestite in Azure Marketplace privato e sono approvate per impostazione predefinita.

## <a name="contact-support"></a>Contattare il supporto tecnico

- Per il supporto di Azure Marketplace, visitare [Microsoft Q&A](/answers/products/).
