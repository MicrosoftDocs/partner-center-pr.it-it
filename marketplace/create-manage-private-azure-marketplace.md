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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Creare e gestire le Azure Marketplace private nel portale di Azure

Il Azure Marketplace consente agli amministratori di controllare le soluzioni di terze parti che gli utenti possono usare. Ciò consente all'utente di distribuire solo le offerte approvate dall'amministratore e conformi ai criteri aziendali. Con il Azure Marketplace privato, gli utenti possono cercare nel negozio online le offerte conformi da acquistare e distribuire.

Come amministratore del Marketplace (ruolo assegnato), si inizierà con uno Store privato disabilitato e vuoto in cui è possibile aggiungere le offerte e i piani approvati. Questo articolo illustra come assegnare il ruolo necessario, creare un archivio privato, gestire gli elementi, approvare le richieste degli utenti e abilitare l'Azure Marketplace privato per gli utenti.

> [!NOTE]
> - Il Azure Marketplace privato è a livello di tenant, quindi tutti gli utenti nel tenant visualizzano lo stesso elenco curato.
> - Tutte le soluzioni Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) vengono aggiunte automaticamente a private Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Assegnare il ruolo di amministratore del Marketplace

Il tenant amministratore globale deve assegnare il ruolo di amministratore del **Marketplace** all'amministratore Azure Marketplace che gestirà l'archivio privato.

>[!IMPORTANT]
> L'accesso alla Azure Marketplace privata è disponibile solo per gli amministratori IT con il ruolo di amministratore del Marketplace assegnato.

### <a name="prerequisites"></a>Prerequisiti

Questi prerequisiti sono necessari prima di poter assegnare il ruolo di amministratore del Marketplace a un utente nell'ambito del tenant:

- Si ha accesso a un **amministratore globale** utente.
- Il tenant ha almeno una sottoscrizione (può essere di qualsiasi tipo).
- All amministratore globale utente viene assegnato il **ruolo Collaboratore** o superiore per la sottoscrizione scelta.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Assegnare il ruolo di amministratore del Marketplace con controllo di accesso (IAM)

1. Accedere al [portale di Azure](https://portal.azure.com/).

1. Selezionare **Tutti i servizi** e quindi **Marketplace.**

1. Selezionare **Marketplace privato** dal menu a sinistra.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Mostra l'opzione di menu marketplace privato sul lato sinistro del Marketplace.":::

1. Selezionare **Controllo di accesso (IAM) per** assegnare il ruolo di amministratore del Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Mostra la schermata di controllo di accesso di I A M.":::

1. Selezionare **Aggiungi** > **Aggiungi assegnazione di ruolo**.

1. In **Ruolo scegliere** Amministratore del **Marketplace.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Mostra il menu Assegnazione di ruolo.":::

1. Selezionare l'utente desiderato nell'elenco a discesa, quindi selezionare **Fine.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Assegnare il ruolo di amministratore del Marketplace con PowerShell

Usare lo script di PowerShell seguente per assegnare il ruolo di amministratore del Marketplace. richiede i parametri seguenti:

- **TenantId:** ID del tenant nell'ambito (il ruolo di amministratore del Marketplace è assegnabile nell'ambito del tenant).
- **Id sottoscrizione:** Sottoscrizione di cui all'amministratore globale è assegnato **il ruolo Collaboratore** o superiore.
- **GlobalAdminUsername:** Nome utente dell'amministratore globale.
- **UsernameToAssignRoleFor:** Nome utente a cui verrà assegnato il ruolo di amministratore del Marketplace.

> [!NOTE]
> Per gli utenti guest invitati nel tenant, potrebbero essere necessario fino a 48 ore prima che il proprio account sia disponibile per l'assegnazione del ruolo di amministratore del Marketplace. Per altre informazioni, vedere Properties of an Azure Active Directory B2B collaboration user (Proprietà di [un utente di Collaborazione B2B).](/azure/active-directory/b2b/user-properties)

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

Per altre informazioni sui cmdlet contenuti nel modulo PowerShell Az.Portal, [vedere Microsoft Azure PowerShell: Cmdlet del dashboard del portale.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Creare un Azure Marketplace

1. Accedere al [portale di Azure](https://portal.azure.com/).
2. Selezionare **Tutti i servizi** e quindi **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Mostra la portale di Azure finestra principale.":::

3. Selezionare **Marketplace privato** dal menu a sinistra.

4. Selezionare **Informazioni di base** per creare un Azure Marketplace privato (è necessario eseguire questa operazione una sola volta).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Viene illustrato come selezionare il Informazioni di base nella finestra portale di Azure'.":::

    Se l Azure Marketplace privata esiste già per questo tenant, **per** impostazione predefinita verrà selezionata l'opzione Gestisci Marketplace.

5. Al termine, si avrà un'istanza privata vuota e disabilitata Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Mostra la schermata Azure Marketplace privato vuota.":::

## <a name="add-items-from-gallery"></a>Aggiungere elementi dalla raccolta

Un elemento è una combinazione di un'offerta e di un piano. È possibile cercare e aggiungere elementi nella pagina Gestisci Marketplace.

1. Selezionare **Aggiungi elementi.**

2. Esplorare la **raccolta** o usare il campo di ricerca per trovare l'elemento desiderato.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Illustra come esplorare la raccolta o usare il campo di ricerca.":::

3. Per impostazione predefinita, quando si aggiunge una nuova offerta, tutti i piani correnti verranno aggiunti all'elenco approvato. Per modificare la selezione del piano prima di aggiungere gli elementi selezionati, selezionare il menu a discesa nel riquadro dell'offerta e aggiornare i piani necessari.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Illustra come aggiornare i piani necessari.":::

4. Selezionare **Fine** in basso a sinistra dopo aver effettuato le selezioni.

>[!Note]
> **Aggiungi elementi** al Marketplace sarà disponibile solo per le offerte non Microsoft. Le soluzioni Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) verranno contrassegnate come "Approvate per impostazione predefinita" e non possono essere gestite nel Marketplace privato.

## <a name="edit-items-plans"></a>Modificare i piani dell'elemento

È possibile modificare i piani di un elemento nella pagina Gestisci Marketplace.

1. Nella colonna **Piani** esaminare i piani disponibili nel menu a discesa per tale elemento.

2. Selezionare o deselezionare le caselle di controllo per scegliere i piani da rendere disponibili agli utenti.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Mostra come selezionare o deselezionare la casella di controllo per l'elemento richiesto.":::

   > [!NOTE]
   > Ogni offerta richiede almeno un piano selezionato per l'aggiornamento. Per rimuovere tutti i piani correlati a un'offerta, eliminare l'intera offerta (vedere la sezione successiva).

## <a name="delete-offers"></a>Eliminare le offerte

Nella pagina Gestisci Marketplace selezionare la casella di controllo accanto al nome dell'offerta (vedere la schermata precedente) e selezionare **Elimina elementi**.

## <a name="enabledisable-private-azure-marketplace"></a>Abilitare/disabilitare l'Azure Marketplace

Nella pagina Gestisci Marketplace verrà visualizzato uno di questi banner, che mostrano lo stato corrente di Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Mostra il banner &quot;Disabilita stato&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Mostra il banner &quot;Abilita stato&quot;.":::

È possibile abilitare o disabilitare l'Azure Marketplace privata in base alle esigenze.

- Se disabilitata, selezionare **Abilita Marketplace privato** per l'abilitazione.
- Se abilitata, selezionare **Disabilita Marketplace privato per** disabilitarla.

## <a name="private-azure-marketplace-notification-center"></a>Centro notifiche Azure Marketplace privato

Il Centro notifiche è costituito da tre tipi di notifiche e consente all'amministratore del Marketplace di eseguire azioni in base alla notifica:

- Richieste di approvazione da parte degli utenti per gli elementi non presenti nell'elenco approvato (vedere Richiedere [l'aggiunta di offerte o piani più](#request-to-add-offers-or-plans) avanti).
- Notifiche del nuovo piano per le offerte che hanno già uno o più piani nell'elenco approvato.
- Sono state rimosse le notifiche del piano per gli elementi presenti nell'elenco approvato, ma che sono stati rimossi dal gruppo Azure Marketplace.

Per accedere al centro notifiche:

1. Selezionare **Notifiche** dal menu a sinistra.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Visualizza il menu Notifiche.":::

1. Selezionare il menu con i puntini di sospensione per altre azioni.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Mostra i risultati del menu Altre opzioni.":::

1. Per le richieste di piano, **Mostra richieste apre** il modulo di richiesta di approvazione in cui è possibile esaminare tutte le richieste utente per l'offerta specifica.
1. Selezionare **Approva** o **Rifiuta.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Mostra le opzioni di approvazione e rifiuto.":::

1. Selezionare il piano da approvare dal menu a discesa.
1. Aggiungere un commento e selezionare **Invia.**

## <a name="browsing-private-azure-marketplace"></a>Esplorazione di Azure Marketplace

Quando l'Azure Marketplace è abilitata, gli utenti visualizzano i piani approvati dall'amministratore del Marketplace.

- Un avviso **verde Approvato** indica un'offerta partner (non Microsoft) approvata.
- Un avviso **blu Approvato** indica un'offerta Microsoft (incluse [le distribuzioni Linux](/azure/virtual-machines/linux/endorsed-distros)approvate) approvata.

Gli utenti possono filtrare le offerte che sono e non sono approvate:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Mostra l'opzione di filtro.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Acquistare o distribuire in servizi Azure Marketplace

Anche se l'esperienza della pagina dei dettagli del prodotto è simile Azure Marketplace globale, esistono tre scenari specifici Azure Marketplace privato.

- Quando un utente seleziona un piano approvato, il **pulsante** Crea è abilitato:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Mostra il banner dell'offerta che indica che è possibile creare un piano.":::

- Se la selezione di un piano di prodotto non viene visualizzata nella pagina dei dettagli del prodotto, ma l'amministratore ha approvato uno o più piani, un banner rileva i piani approvati e il **pulsante** Crea è abilitato:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Mostra il banner dell'offerta che indica che è possibile creare un piano e mostra i piani disponibili.":::

- Quando un utente seleziona un piano non approvato, un banner indica che il piano non è approvato e il **pulsante** Crea è disabilitato. L'utente può comunque richiedere di aggiungere il piano all'elenco approvato (vedere la sezione successiva).

## <a name="request-to-add-offers-or-plans"></a>Richiesta di aggiunta di offerte o piani

È possibile richiedere di aggiungere un'offerta o un piano pubblico non attualmente approvato nell'Azure Marketplace.

1. Selezionare **Richiesta da aggiungere nel** banner per aprire il modulo Richiesta di **accesso**.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Mostra il banner con il collegamento &quot;Richiesta di aggiunta&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Mostra il modulo di richiesta di accesso per offerte o piani.":::

1. Selezionare i piani da aggiungere alla richiesta **(** Qualsiasi piano indica all'amministratore del Marketplace che non si ha una preferenza per un piano all'interno di un'offerta).

1. Aggiungere una **giustificazione e** selezionare **Richiesta per** inviare la richiesta.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Mostra il modulo di richiesta di accesso per offerte o piani con voci di esempio.":::

1. Un'indicazione per una richiesta in sospeso verrà visualizzata nel modulo Richiesta di accesso con l'opzione **Richiesta di ritiro**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Visualizza un elenco di piani approvati o in sospeso con il collegamento Richiesta di ritiro.":::

> [!NOTE]
> Dopo l'invio, il modulo di [](#private-azure-marketplace-notification-center) richiesta di approvazione verrà inviato al Centro notifiche per l'amministratore del Marketplace per esaminare la richiesta ed eseguire un'azione.

> [!CAUTION]
> L'approvazione nel Marketplace privato non indica l'approvvigionamento di una soluzione.

## <a name="frequently-asked-questions-faqs"></a>Domande frequenti (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Si sta già bloccando l'applicazione di terze parti del Marketplace tramite Criteri di Azure. Che cosa è diverso?

Esistono attualmente due modi per limitare i servizi di terze parti in Marketplace:

1. Tramite EA Portal o il portale di Azure, disabilitare i servizi di terze parti o limitarsi a "Solo SKU gratuiti o BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Illustra come limitare i servizi nel portale di Azure.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Illustra come limitare i servizi nel portale E A.":::

2. Creare un criterio di Azure per consentire solo macchine virtuali specifiche. Per informazioni dettagliate su come applicare i criteri Windows macchine virtuali, vedere Applicare criteri alle macchine virtuali [Windows con Azure Resource Manager](/azure/virtual-machines/windows/policy).

Il Azure Marketplace privato offre maggiore flessibilità per limitare e consentire offerte e piani specifici. Informa gli utenti finali sulla disponibilità per la distribuzione nella raccolta del marketplace anche prima di provare a distribuire servizi di terze parti. Per consentire la distribuzione di servizi di terze parti, impostare Azure Marketplace su Attivato/Abilitato in EA Portal e il portale di Azure.

- I Azure Marketplace possono curare soluzioni partner non limitate alle macchine virtuali.
- I Azure Marketplace possono essere curati a livello di piano e possono anche impostare "Piano corrente e futuro".
- I Azure Marketplace possono informare gli utenti finali in anticipo su ciò che può o non può essere distribuito.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Qual è la differenza tra un'offerta privata e una Azure Marketplace?

**Un'offerta privata** consente agli editori di creare piani visibili solo ai clienti di destinazione. In questo modo possono condividere privatamente soluzioni personalizzate con prezzi negoziati, termini e condizioni privati e configurazioni specializzate. Per informazioni dettagliate, [vedere Offerte private nel marketplace commerciale.](/azure/marketplace/private-offers)

**I Azure Marketplace** privati nel portale di Azure consentono agli amministratori di approvare in modo preliminare le soluzioni di terze parti che gli utenti possono distribuire. Con un'Azure Marketplace privata, gli utenti possono usufruire dei vantaggi dell'Azure Marketplace trovando, acquistando e distribuendo offerte conformi. Per gestire le offerte private basate su sottoscrizioni nel Marketplace privato, l'amministratore del Marketplace deve avere almeno il ruolo di "lettura" per la sottoscrizione specifica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>È stata aggiunta un'offerta privata al Azure Marketplace privato, perché non viene visualizzata nella scheda Gestisci marketplace?

Le offerte private basate su sottoscrizione sono visibili solo per le sottoscrizioni elencate nelle impostazioni dell'offerta privata. Per visualizzare l'offerta privata, verificare che il filtro delle sottoscrizioni globali mostri tutte le sottoscrizioni.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Mostra il filtro del marketplace privato.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>È possibile includere immagini personalizzate in private Azure Marketplace?

No. La Azure Marketplace consente a qualsiasi amministratore IT di gestire e gestire soluzioni di terze parti da soluzioni Azure Marketplace. Poiché le immagini personalizzate non sono in Azure Marketplace globale, l'amministratore IT non può selezionare e scegliere le immagini personalizzate. Se si desidera condividere immagini personalizzate, usare [Raccolta immagini condivise.](/azure/virtual-machines/shared-image-galleries)

1. Guida dettagliata alla creazione di una raccolta di immagini condivise (SIG) (interfaccia[della riga di](/azure/virtual-machines/shared-images-cli)comando, [PowerShell).](/azure/virtual-machines/shared-images-powershell)
2. Creare una definizione di immagine all'interno di un sig. Il cliente deve **scegliere Generalized (Generalizzato)** per il campo OS-state (Stato sistema operativo). ([interfaccia della](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)riga di comando , [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Portare un'immagine gestita in Raccolta immagini condivise (interfaccia[della riga di comando,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)
4. Le immagini di VM SIG risiederebbero in una sottoscrizione. Per renderla disponibile ad altre sottoscrizioni, usare una registrazione dell'app (interfaccia[della riga di comando](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Perché alcune offerte sono approvate **per impostazione predefinita** anche se l'editore non è Microsoft?

Microsoft supporta Linux e la tecnologia open source in Azure. [Le distribuzioni Linux approvate](/azure/virtual-machines/linux/endorsed-distros) sono supportate in Azure e il prezzo è integrato nelle macchine virtuali. Poiché l'agente Linux di Azure è già preinstallato Azure Marketplace, viene considerato come un'offerta Microsoft. Poiché le offerte Microsoft sono approvate per impostazione predefinita, le distribuzioni Linux approvate non possono essere gestite in private Azure Marketplace e sono approvate per impostazione predefinita.

## <a name="contact-support"></a>Contattare il supporto tecnico

- Per Azure Marketplace, visitare il sito [Web Microsoft Q&A.](/answers/products/)