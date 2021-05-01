---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
description: Sincronizzare le segnalazioni Partner Center con il connettore di co-selling per Dynamics 365 CRM. È quindi possibile co-vendere con Microsoft dall'interno del sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: c399e00394208ec29dd59a41afe7cce1b1d07253
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284333"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Panoramica del connettore di co-selling per Dynamics 365 CRM

**Ruoli appropriati**

- Amministratore delle segnalazioni
- Amministratore di sistema o a personalizzatore di sistema in CRM

Partner Center i connettori di co-selling consentono ai venditori di co-vendere con Microsoft dall'interno dei sistemi CRM. Non sarà necessario eseguire il training per usare i Partner Center per gestire le trattative di co-selling. Usare i connettori di co-selling per creare una nuova segnalazione di co-selling per coinvolgere un venditore Microsoft, ricevere segnalazioni dal venditore Microsoft, accettare o rifiutare le segnalazioni e modificare i dati delle trattative, ad esempio il valore dell'offerta e la data di chiusura. È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft su queste offerte di co-selling. È possibile gestire tutte le segnalazioni nel CRM preferito anziché in Partner Center.

La soluzione è basata su Power Automate e usa Partner Center API.

## <a name="prerequisites"></a>Prerequisiti

Prima di installare la soluzione, assicurarsi di soddisfare i prerequisiti seguenti.

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network (MPN) |È necessario un ID MPN valido.|[Partecipare alla rete partner](https://partner.microsoft.com/)|
|Pronto per il co-selling|La soluzione IP/Servizi deve essere pronta per il co-selling.|[Vendere con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Account del Centro per i partner|L'ID MPN associato al tenant Partner Center deve essere uguale all'ID MPN associato alla soluzione di co-selling. Verificare che sia possibile visualizzare le segnalazioni di co-selling nel portale Partner Center prima di distribuire i connettori.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore delle segnalazioni.|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Il ruolo utente CRM è Amministratore di sistema o A personalizzatore sistema.|[Assegnare ruoli in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate account del flusso di lavoro|Creare un nuovo ambiente di produzione con un database per il test, la gestione temporanea e la produzione. Se si dispone di un ambiente di produzione esistente con un database, è possibile riutilizzarlo. L'utente che installerà la soluzione connettore deve avere una licenza Power Automate e l'accesso a questo ambiente. È possibile monitorare lo stato di avanzamento e ottenere altre informazioni [in](https://flow.microsoft.com/) Power Automate se l'installazione non riesce. Selezionare **Visualizza cronologia** in **Soluzioni.**|[Creare o gestire l'ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installare Partner Center delle segnalazioni per Dynamics 365 (Power Automate soluzione)

1. Passare a [Power Automate](https://flow.microsoft.com)e selezionare **Ambienti** nell'angolo in alto a destra. Questo passaggio mostra le istanze crm disponibili.

1. Selezionare l'istanza di CRM appropriata nell'elenco a discesa nell'angolo superiore destro.

1. Selezionare **Soluzioni** a sinistra.

1. Selezionare il **collegamento Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Screenshot che mostra Open AppSource.":::

1. Cercare Partner Center **Referrals Connectors per Dynamics 365** nella schermata popup.  

1. Selezionare il **pulsante Scarica adesso** e quindi continua. 

1. Viene visualizzata una pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione. Accettare i termini e le condizioni.

1. È possibile monitorare lo stato di avanzamento e, se l'installazione non riesce, è possibile ottenere altri dettagli Power Automate selezionando **Visualizza cronologia** in **Soluzioni**.

1. Al termine dell'installazione, tornare a [Power Automate](https://flow.microsoft.com) e selezionare **Soluzioni** a sinistra. Partner Center la sincronizzazione delle segnalazioni **per Dynamics 365** è ora disponibile nell'elenco **Soluzioni.**

1. Selezionare **Partner Center sincronizzazione delle segnalazioni per Dynamics 365.** Sono disponibili Power Automate seguenti flussi ed entità.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot che mostra i CPM disponibili.":::

## <a name="test-before-you-go-live"></a>Eseguire il test prima di iniziare a eseguire il test

Prima di installare, configurare e personalizzare la soluzione Power Automate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza crm di staging. È necessario:

- Installare la soluzione Power Automate in un'istanza CRM dell'ambiente di staging.
- Configurare e personalizzare la soluzione Power Automate in un ambiente di staging.
- Testare la soluzione in un'istanza CRM di staging.
- Al termine di un test, importare come soluzione gestita nell'istanza di produzione.

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power Automate](https://flow.microsoft.com/).

1. **Nell'elenco a** discesa Ambienti nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la Power Automate soluzione.

1. È necessario creare connessioni che associano i tre account utente:

   - Partner Center utente con credenziali di amministratore di Referrals
   - Eventi del Centro per i partner
   - Amministratore di CRM con Power Automate flussi nella soluzione

   1. Selezionare **Connessioni** a sinistra e selezionare la soluzione Partner Center **referral dall'elenco.**

   1. Creare una connessione selezionando **Crea una connessione**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot che mostra La creazione di una connessione.":::

   1. Cercare Partner Center **segnalazioni (anteprima)** nella barra di ricerca nell'angolo in alto a destra.

   1. Creare una connessione per l'Partner Center utente con il ruolo credenziali di amministratore delle segnalazioni.

   1. Creare quindi una connessione Partner Center eventi per l'utente Partner Center con le credenziali di amministratore di Segnalazioni.

   1. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore di CRM.
     
   1. Dopo aver aggiunto tutte le connessioni, nell'ambiente dovrebbero essere presenti le connessioni seguenti.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Screenshot che mostra le connessioni.":::

## <a name="edit-the-connections"></a>Modificare le connessioni

1. Tornare alla pagina **Soluzioni** e selezionare **Soluzione predefinita.** Selezionare **Riferimento alla connessione (anteprima)** selezionando **Tutti.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot che mostra la modifica delle connessioni.":::

1. Modificare ognuna delle connessioni singolarmente selezionando l'icona con i puntini di sospensione. Aggiungere le connessioni pertinenti.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Screenshot che mostra le connessioni elencate.":::

1.  Tornare alla  pagina Soluzioni, selezionare **Partner Center Referrals Synchronization for Dynamics 365 (Sincronizzazione** delle segnalazioni per Dynamics 365) e attivare il flusso selezionando l'icona con i puntini di sospensione accanto a ogni flusso nella sequenza seguente. Se si verificano problemi durante l'attivazione del flusso, vedere [Passaggi di personalizzazione](connector-dynamics.md#customize-synchronization-steps) e [Passaggi per la risoluzione dei problemi.](connectors-troubleshoot.md)

Attivare i flussi nella sequenza seguente:

- Partner Center Webhook Registration (Insider Preview)
- Creare segnalazioni di co-selling - Dynamics 365 to Partner Center (Insider Preview)
- [Personalizza] Creare o ottenere dettagli dal flusso di Dynamics 365
- Partner Center a Dynamics 365 - Helper (Insider Preview)
- Partner Center microsoft co-selling referral updates to Dynamics 365 (Insider Preview)
- Partner Center a Dynamics 365 (Insider Preview)
- Da Dynamics 365 a Partner Center (Insider Preview)
- Dynamics 365 Opportunity to Partner Center (Insider Preview)
- Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API del webhook per la registrazione per gli eventi di modifica delle risorse

È possibile usare le API Partner Center webhook per registrarsi per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Selezionare **Partner Center a Dynamics 365 (Insider Preview)**.

1. Selezionare **l'icona** Modifica e selezionare **Quando viene ricevuta una richiesta HTTP.**

1. Selezionare **l'icona** Copia per copiare l'URL HTTP POST specificato.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot che mostra l'uso dei webhook per registrare le modifiche alle risorse.":::

1. Selezionare il **Partner Center webhook (Insider Preview)** Power Automate flusso e quindi selezionare **Esegui**.

1. Assicurarsi che la **finestra Esegui** flusso si apra nel riquadro destro e selezionare **Continua**.

1. Immettere i dettagli seguenti:

   - **Endpoint trigger HTTP:** questo URL è stato copiato da un passaggio precedente.
   - **Eventi da registrare:** selezionare tutti gli eventi disponibili (**referral-created**, **referral-updated**, **related-referral-created** e **related-referral-updated**).
   - **Sovrascrivere gli endpoint trigger esistenti, se presenti?**: Sì. È possibile registrare un solo URL per un determinato evento webhook.

1. Selezionare **Esegui flusso** e quindi Fare clic su **Fine.**

Il webhook può ora restare in ascolto, creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

I sistemi CRM sono altamente personalizzati ed è possibile personalizzare la soluzione Power Automate in base alla configurazione crm. Quando le segnalazioni di co-selling vengono sincronizzate tra Partner Center e il sistema CRM, i campi sincronizzati nel PC Partner Center sono elencati nella Guida al mapping dei campi [personalizzati.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate in [Personalizzare] Creare o ottenere dettagli dal flusso di **Dynamics 365** o dalle variabili di ambiente. Non aggiornare altri flussi nella soluzione Power Automate perché può influire sugli aggiornamenti futuri della soluzione.

Sono disponibili le personalizzazioni seguenti:

- **Visualizza segno di** spunta nel nome dell'opportunità: per impostazione predefinita, accanto al nome dell'opportunità verrà visualizzato un segno di spunta per indicare che la sincronizzazione tra Partner Center e Dynamics 365 CRM viene eseguita correttamente. Analogamente, se la sincronizzazione non riesce, verrà visualizzato un segno di spunta incrociato. Per evitare di aggiungere un segno di spunta o un segno di spunta nel nome dell'opportunità, impostare il valore corrente di Visualizza segno di spunta nella variabile di ambiente **nome** opportunità su No.
- **Valore trattativa:** per impostazione predefinita, il valore della trattativa Partner Center verrà sincronizzato da e verso **estimatedvalue** in CRM. Se nel CRM è presente un campo diverso per il valore della trattativa da cui eseguire la sincronizzazione:

  - Aggiornare il **nome del campo** Valore trattativa nella variabile di ambiente Dynamics 365 con il nome del campo crm. Assicurarsi di specificare il nome del campo, non il nome visualizzato.
  - Modifica [Personalizza] Crea o Ottieni dettagli dal flusso di Dynamics **365** e passa **a** Crea o aggiorna opportunità **in** CRM e aggiorna Crea una nuova opportunità e Aggiorna le azioni opportunità esistenti per assegnare il valore **DealValue** al campo corretto in CRM.  Rimuovere anche **l'assegnazione DealValue** dal **campo Estimated Revenue** .

- **Codice paese dell'account** cliente: è obbligatorio specificare un codice paese di due lettere (ISO 3166) quando si crea una nuova segnalazione. Per impostazione predefinita, il codice paese verrà sincronizzato  con e dal campo address1_country dell'account nel CRM. Se nel CRM è presente un campo diverso da cui eseguire la sincronizzazione del codice paese:

   - Per un campo di codice paese non di ricerca nell'account che contiene un codice di due lettere:
     - Aggiornare il **nome del campo Customer Account Country Code** nella variabile di ambiente Dynamics 365 con il nome del campo crm. Assicurarsi di specificare il nome del campo, non il nome visualizzato.
     - Modificare [Personalizza] Crea o Ottieni dettagli dal flusso **dynamics 365** e passare **a** Crea o ottieni **account** cliente nell'azione CRM per assegnare un valore Country al campo corretto nel CRM. Rimuovere inoltre **l'assegnazione del** valore Country dal **campo Address 1: Country/Region (Indirizzo 1: Paese/area** geografica).

   - Per un campo di codice paese basato sulla ricerca nell'account:
     - Aggiungere un nuovo campo personalizzato nell'account e popolarlo automaticamente con un codice paese di due lettere (ISO 3166) in base al valore selezionato nel campo basato su ricerca e viceversa.
     - Seguire i passaggi precedenti per il campo codice paese non di ricerca per sincronizzare un nuovo campo personalizzato da CRM a e da Partner Center.

- Campi **opportunità:** se sono presenti campi obbligatori in **Opportunità** che devono essere popolati, modificare [Personalizza] Crea o Ottieni dettagli dal flusso di **Dynamics 365** e passare **a** Crea o aggiorna opportunità **in** CRM e aggiornare l'azione Crea una nuova opportunità per assegnare valori ai campi obbligatori in base ai requisiti aziendali.
- Campi **lead:** se nel  lead sono presenti campi obbligatori che devono essere popolati, modificare [Personalizza] Crea o Ottieni dettagli dal flusso **dynamics 365** e passare a Crea o aggiorna lead **in** CRM e aggiornare Crea un nuovo lead **per** assegnare valori ai campi obbligatori in base ai requisiti aziendali.
- **Account cliente:** quando una nuova segnalazione viene sincronizzata da Partner Center a CRM, la soluzione Power Automate tenta di cercare un account esistente nel sistema CRM usando il nome della società e il codice postale del cliente. Se non ne trova uno, verrà creato un nuovo account cliente nel sistema CRM. Per aggiornare i criteri di ricerca e i dettagli di creazione del nuovo account, modificare [Personalizza] Crea o Ottieni dettagli dal flusso **di Dynamics 365** e passare a Crea o ottieni **l'account** cliente nell'azione CRM e Crea **account cliente**.

## <a name="update-environment-variable"></a>Aggiornare la variabile di ambiente

Per aggiornare il valore di una variabile di ambiente:

1. Passare alla **pagina Soluzioni** e selezionare Soluzione **predefinita.** Selezionare **Variabile di** ambiente selezionando **Tutti.**

1. Selezionare la variabile di ambiente per il valore che deve essere aggiornato e selezionare **Modifica** usando l'icona con i puntini di sospensione.

1. Aggiornare **il valore** corrente (non aggiornare il valore **predefinito)** usando l'opzione Nuovo **valore** e specificando il valore. Il valore deve corrispondere al tipo di dati della variabile. Ad esempio, il tipo di dati Sì o No accetterà il valore Sì o No.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Screenshot che mostra l'aggiornamento delle variabili di ambiente.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronizzazione delle segnalazioni di co-selling bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power Automate, è possibile testare la sincronizzazione delle segnalazioni di co-selling tra Dynamics 365 e Partner Center.

### <a name="prerequisites"></a>Prerequisiti

Per sincronizzare le segnalazioni Partner Center e Dynamics 365 CRM, la soluzione Power Automate delimita chiaramente i campi di segnalazione specifici di Microsoft. Questa identificazione offre ai team venditori la possibilità di decidere quali segnalazioni vogliono condividere con Microsoft per il co-selling.

Nell'ambito dell'installazione della soluzione verrà aggiunto un set di campi e oggetti personalizzati. Un utente amministratore di CRM dovrà creare una sezione CRM separata con i **campi personalizzati** Opportunità.

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizza con Partner Center:** indica se sincronizzare l'opportunità con Partner Center. Per impostazione predefinita, il valore di questo campo è No e deve essere impostato in modo esplicito su Sì dal venditore per condividere un'opportunità con Microsoft. Le nuove segnalazioni condivise da Partner Center a CRM avranno questo valore di campo impostato su Sì.
- **Identificatore di riferimento:** campo dell'identificatore di sola lettura per la Partner Center riferimento.
- **Collegamento alla segnalazione:** collegamento di sola lettura alla segnalazione in Partner Center.
- **Come può essere utile Microsoft?**: Guida necessaria a Microsoft per la segnalazione. Per creare una segnalazione di co-selling, selezionare la Guida appropriata richiesta da Microsoft. Un contatto del cliente deve essere associato all'opportunità di creare una segnalazione di co-selling. Per creare una segnalazione di non co-selling, non selezionare questo campo. Una segnalazione di non co-selling può essere convertita in una segnalazione di co-selling in qualsiasi momento selezionando l'opzione appropriata per la guida necessaria.
- **Visibilità delle segnalazioni di Microsoft Partner Center:** selezionare la visibilità per la Partner Center segnalazione. Rendendolo visibile ai venditori Microsoft, una segnalazione di non co-selling potrebbe essere convertita in co-selling. Quando è necessaria la Guida Microsoft, la segnalazione è visibile ai venditori Microsoft per impostazione predefinita. Dopo che questo campo è stato contrassegnato come visibile, non può essere ripristinato.
- **Identificatore Microsoft CRM:** quando un riferimento di co-selling viene creato e accettato da Microsoft, questo campo verrà popolato con l'identificatore CRM di Microsoft.
- **Prodotti: Obsoleto:** non usare questo campo o aggiungerlo alla sezione CRM. È disponibile solo per la compatibilità con le versioni precedenti. Usare Partner Center soluzioni personalizzate.
- **Audit:** un'istanza di sola audit trail per la sincronizzazione con Partner Center segnalazioni.
- **Microsoft Partner Center Solutions:** oggetto personalizzato per associare all'opportunità soluzioni pronte per il co-selling o soluzioni Microsoft. È possibile aggiungere o rimuovere una o più soluzioni dall'opportunità. È obbligatorio aggiungere all'opportunità almeno una soluzione Microsoft o pronta per il co-selling prima di condividerla con Microsoft. Per associare questo oggetto all'opportunità, aggiornare il **modulo Opportunità** in CRM.

  Selezionare la scheda appropriata nel **modulo Opportunità** e aggiungere una griglia secondaria come illustrato di seguito.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot che mostra il modulo Opportunità.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot che mostra le soluzioni Microsoft.":::

- Dopo aver aggiunto le soluzioni Microsoft, è possibile prepopolare i dettagli della soluzione pronta per il co-selling in modo che i venditori non devono aggiungerle. Per aggiungere i dettagli di una nuova soluzione, passare all'oggetto Dettagli soluzione Microsoft in CRM e selezionare Aggiungi **record** per aggiungere una voce o usare il caricamento di **Excel** per aggiungere più voci.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Screenshot che mostra i dettagli della nuova soluzione Microsoft.":::

### <a name="scenarios"></a>Scenari

1. Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in CRM e sincronizzata in Partner Center:

   1. Accedere all'ambiente Dynamics 365 CRM con l'utente che ha visibilità nella **sezione Opportunità** di CRM.

   1. Assicurarsi che la **sezione Microsoft Partner Center** sia presente quando si crea una nuova opportunità nell'ambiente Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Screenshot che mostra Nuova opportunità.":::

   1. Per sincronizzare questa opportunità con Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Come può essere utile Microsoft?**: per creare una segnalazione di co-selling, selezionare un'opzione di assistenza appropriata.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Screenshot che mostra come ottenere i campi appropriati nella visualizzazione scheda.":::

      - **Contatto cliente:** per creare una segnalazione di co-selling, aggiungere un contatto cliente all'opportunità.
      - **Sincronizza con Partner Center**: Sì.
      - **Soluzioni Microsoft:** per condividere una segnalazione con Microsoft, aggiungere all'opportunità una soluzione Valida pronta per il co-selling o Microsoft.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Screenshot che mostra l'ID soluzione.":::

   1. Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sincronizza** con Partner Center impostata su Sì, attendere 10 minuti. Accedere quindi all'account Partner Center locale. Le segnalazioni verranno sincronizzate con Dynamics 365 e **l'identificatore di riferimento**. **Il collegamento di** riferimento verrà popolato. Se si verifica un errore, il **campo Controllo** verrà popolato con le informazioni sull'errore.
     
    1. Analogamente, per un'opportunità con l'opzione Sincronizza con **Partner Center** impostata su Sì, se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account Partner Center dati.

    1. Le opportunità sincronizzate correttamente con Partner Center verranno identificate con ✔icon in Dynamics 365.

1. Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata Partner Center e sincronizzata nell'ambiente Dynamics 365:

   1. Accedere al dashboard [Partner Center.](https://partner.microsoft.com/dashboard/home)

   1. Selezionare **Segnalazioni** dal menu a sinistra.

   1. Creare una nuova segnalazione di co-selling da Partner Center selezionando **l'opzione New deal (Nuovo** accordo).

   1. Accedere all'ambiente Dynamics 365 CRM.

   1. Passare a **Apri opportunità**. La segnalazione creata in Partner Center è ora sincronizzata in Dynamics 365 CRM.

   1. Quando si seleziona una segnalazione sincronizzata, i dettagli della visualizzazione scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)
- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
- [Altre informazioni sulla piattaforma microsoft Power Automate](/power-automate/)
- [Webhook del Centro per i partner](/partner-center/develop/partner-center-webhooks)
