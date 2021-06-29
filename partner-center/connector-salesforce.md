---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare le segnalazioni Partner Center con Salesforce CRM. I venditori possono quindi co-selling con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029105"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connettore di co-selling per CRM Salesforce - Panoramica

**Ruoli appropriati:** amministratore delle segnalazioni | Amministratore di sistema o a personalizzatore di sistema in CRM

Partner Center connettore di co-selling consente ai venditori di co-selling con Microsoft dall'interno dei sistemi CRM. Non sarà necessario eseguire il training per usare le Partner Center per gestire le trattative di co-selling. Usando i connettori di co-selling, puoi creare una nuova segnalazione di co-selling per coinvolgere un venditore Microsoft, ricevere segnalazioni dal venditore Microsoft, accettare/rifiutare le segnalazioni, modificare i dati delle trattative, ad esempio il valore della trattativa e la data di chiusura.  È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft su queste trattative di co-selling. È possibile eseguire tutte le segnalazioni mentre si lavora all'interno del sistema CRM preferito anziché in Partner Center.

La soluzione è basata su Microsoft Power Automate e usa Partner Center API.

## <a name="before-you-install---pre-requisites"></a>Prima di installare : prerequisiti

|**Argomenti**|**Dettagli**|**Collegamenti**|
|--------------|--------------------|------|
|Microsoft Partner Network ID |È necessario un ID MPN valido|Per partecipare [a MPN](https://partner.microsoft.com/)|
|Pronto per il co-selling|La soluzione IP/Servizi deve essere pronta per il co-selling.|[Vendere con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Account del Centro per i partner|L'ID MPN associato al tenant Partner Center deve corrispondere all'ID MPN associato alla soluzione di co-selling. Verificare che sia possibile visualizzare le segnalazioni di co-selling Partner Center portale prima di distribuire i connettori.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore delle segnalazioni|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Il ruolo utente CRM è Amministratore di sistema o A personalizzatore sistema|[Assegnare ruoli in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Creare un nuovo ambiente di produzione con un database per il test, la gestione temporanea e la produzione. Se si dispone di un ambiente di produzione esistente con un database, è possibile riutilizzarlo. L'utente che installerà la soluzione connettore deve avere una licenza Power Automate e l'accesso a questo ambiente. È possibile monitorare lo stato di avanzamento e ottenere altre informazioni [in](https://flow.microsoft.com/) Power Automate se l'installazione non riesce. Selezionare **Visualizza cronologia** in **Soluzioni.**|[Creare o gestire l'ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installazione del pacchetto Salesforce per i campi personalizzati Microsoft

Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve identificare chiaramente i campi di segnalazione specifici di Microsoft. Questa delimitazione offre ai team dei venditori dei partner la possibilità di decidere quali segnalazioni condividere con Microsoft per il co-selling.

1. In Salesforce attivare Notes **e** aggiungerlo all'elenco correlato alle opportunità. [Riferimento](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Attivare **i team opportunity** seguendo questa procedura:
    - In Configurazione usare la casella **Ricerca rapida per** individuare Le impostazioni del team di opportunità.
    - Definire le impostazioni in base alle esigenze. [Riferimento](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. In Salesforce installare campi e oggetti personalizzati usando il programma [di installazione del pacchetto](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Usare questo programma di installazione per installare il pacchetto in qualsiasi società.

    >[!NOTE]
    >Se si sta installando in una sandbox, è necessario sostituire la parte iniziale dell'URL con `http://test.salesforce.com` .

1. In Salesforce aggiungere Soluzioni Microsoft **all'elenco Correlato** alle opportunità. Dopo l'aggiunta, selezionare **l'icona della chiave inglese** e aggiornare le proprietà

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: eseguire il test prima di iniziare a essere live

Prima di installare, configurare e personalizzare la soluzione Power Automate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza crm di staging.

- Installare la soluzione Microsoft Power Automate in un ambiente di gestione temporanea o in un'istanza di CRM.

- Creare una copia della soluzione ed eseguire la configurazione e Power Automate del flusso nell'ambiente di gestione temporanea.

- Testare la soluzione in un'istanza di staging/CRM.

- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installare la Partner Center delle segnalazioni per Salesforce CRM

1. Passare a [Power Automate](https://flow.microsoft.com) e selezionare **Ambienti nell'angolo** superiore destro. Verranno mostrate le istanze crm disponibili.

1. Selezionare l'istanza di CRM appropriata nell'elenco a discesa nell'angolo superiore destro.

1. Selezionare **Soluzioni** nella barra di spostamento a sinistra.

1. Selezionare il **collegamento Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Aprire AppSource":::

1. Cercare Partner Center **Referrals Connectors for Salesforce** nella schermata popup.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Screenshot di Scarica adesso.":::

1. Selezionare il **pulsante Scarica adesso** e quindi continua. 

1. Nella pagina successiva selezionare l'ambiente Salesforce CRM per installare l'applicazione. Accettare i termini e le condizioni.

1. Si verrà quindi indirizzati alla **pagina Gestisci le** soluzioni.  Passare a "Partner Center segnalazioni" usando i pulsanti freccia nella parte inferiore della pagina. **L'installazione** pianificata dovrebbe essere visualizzata Partner Center soluzione Segnalazioni. L'installazione può richiedere 10-15 minuti.

1. Al termine dell'installazione, tornare [all'Power Automate](https://flow.microsoft.com) e selezionare **Soluzioni nell'area** di spostamento a sinistra. Si noti **che Partner Center delle segnalazioni per Salesforce** è ora disponibile nell'elenco Soluzioni.

1. Selezionare **Partner Center referrals Synchronization for Salesforce (Sincronizzazione delle segnalazioni per Salesforce).** Sono disponibili Power Automate seguenti flussi ed entità:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Flussi di Salesforce":::

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare [a Power Automate](https://flow.microsoft.com/).

1. **Nell'elenco a** discesa Ambienti nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la Power Automate soluzione.

1. Sarà necessario creare connessioni che associano i tre account utente:

   - Partner Center utente con le credenziali di amministratore delle segnalazioni
   - Eventi del Centro per i partner
   - Amministratore CRM con i Power Automate di distribuzione nella soluzione

   1. Selezionare **Connessioni** dalla barra di spostamento a sinistra e selezionare la **Partner Center Segnalazioni** dall'elenco.

   1. Creare una connessione selezionando **Crea una connessione**.

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot che mostra La creazione di una connessione.":::

   1. Cercare Partner Center **segnalazioni (anteprima)** nella barra di ricerca nell'angolo in alto a destra.

   1. Creare una connessione per l'Partner Center utente con il ruolo credenziali di amministratore delle segnalazioni.

   1. Creare quindi una connessione Partner Center eventi per l'utente Partner Center con le credenziali di amministratore delle segnalazioni.

   1. Creare una connessione per Salesforce per l'utente amministratore di CRM.
  
   1. Creare una connessione per Microsoft Dataverse per l'utente amministratore di CRM.

   1. Dopo aver aggiunto tutte le connessioni, nell'ambiente dovrebbero essere presenti le connessioni seguenti:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Screenshot che mostra come osservare le connessioni.":::

### <a name="edit-the-connections"></a>Modificare le connessioni

1. Tornare alla pagina **Soluzioni** e selezionare **Soluzione predefinita.** Selezionare **Riferimento alla connessione (anteprima)** facendo clic su **Tutti**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot che mostra la modifica delle connessioni.":::

1. Modificare ognuna delle connessioni singolarmente selezionando l'icona con i puntini di sospensione. Aggiungere le connessioni pertinenti.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Screenshot che mostra come modificare i connettori.":::

1. Attivare i flussi nella sequenza seguente:
   - Partner Center Webhook Registration (Insider Preview)
   - [Personalizza] Creare o ottenere dettagli da Salesforce
   - Creare co-selling Referral-Salesforce Partner Center (Insider Preview)
   - Partner Center microsoft co-selling referral updates to Salesforce (Insider Preview)  
   - Partner Center a Salesforce (Insider Preview)
   - Da Salesforce a Partner Center (Insider Preview)
   - Opportunità di salesforce per Partner Center (Insider Preview)
   - Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API del webhook per la registrazione per gli eventi di modifica delle risorse

È possibile usare le API Partner Center webhook per registrarsi per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Selezionare **Partner Center a Salesforce CRM (Insider Preview).**

1. Selezionare **l'icona Modifica** e selezionare **Quando viene ricevuta una richiesta HTTP.**

1. Selezionare **l'icona** Copia per copiare **l'URL HTTP POST specificato.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Screenshot che mostra come copiare l'URL.":::

1. Selezionare il **Partner Center webhook (Insider Preview)** Power Automate flusso e quindi selezionare **Esegui**.

1. Assicurarsi che la **finestra Esegui** flusso si apra nel riquadro destro e selezionare **Continua**.

1. Immettere i dettagli seguenti:

   - **Endpoint trigger HTTP:** questo URL è stato copiato da un passaggio precedente.
   - **Eventi da registrare:** selezionare tutti gli eventi disponibili (**referral-created**, **referral-updated**, **related-referral-created** e **related-referral-updated**).
   - **Sovrascrivere gli endpoint trigger esistenti, se presenti?**: Sì. È possibile registrare un solo URL per un determinato evento webhook.

1. Selezionare **Esegui flusso** e quindi Fare clic su **Fine.**

Il webhook può ora restare in ascolto, creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

I sistemi CRM sono altamente personalizzati ed è possibile personalizzare la soluzione Power Automate in base alla configurazione di CRM. Quando le segnalazioni di co-selling vengono sincronizzate tra Partner Center e il sistema CRM, i campi sincronizzati nel PC Partner Center sono elencati nella Guida al mapping dei campi [personalizzati](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate in **[Personalizza]** Creare o ottenere dettagli da Salesforce o variabili di ambiente. Non aggiornare altri flussi nella soluzione Power Automate perché può influire sugli aggiornamenti futuri della soluzione.

Sono disponibili le personalizzazioni seguenti:

- **Visualizza segno di spunta nel** nome dell'opportunità: per impostazione predefinita, accanto al nome dell'opportunità verrà visualizzato un segno di spunta per indicare che la sincronizzazione tra Partner Center e Salesforce CRM viene eseguita correttamente. Analogamente, se la sincronizzazione ha esito negativo, verrà visualizzato un segno incrociato. Per evitare di aggiungere un segno di spunta o un segno di spunta nel nome dell'opportunità, impostare il valore corrente del segno di spunta Visualizza nella variabile di ambiente **nome** opportunità su No.

- **Nome fase:**

  - **Nome fase attiva:** questa è la fase della pipeline di vendita di un'opportunità in Salesforce.  Rappresenta una fase attiva ed è equivalente a una segnalazione nello stato accettato Partner Center. Questa può essere la fase successiva nella pipeline di vendita dopo la fase di attesa. Spostando la fase di vendita dell'opportunità dalla fase di attesa alla fase attiva, la segnalazione verrà accettata Partner Center le modifiche inizieranno la sincronizzazione.

  - **Nome fase di attesa:** nome della fase nella pipeline di vendita di un'opportunità in Salesforce. Rappresenta una fase di attesa. Le nuove segnalazioni di co-selling condivise da Microsoft non ancora accettate verranno impostate su questa fase in Salesforce. Le modifiche apportate a un'opportunità durante la fase di attesa non verranno sincronizzate con Partner Center. Se si sposta la fase di vendita dell'opportunità fuori da questa fase di attesa, verrà accettata la segnalazione Partner Center le modifiche inizieranno la sincronizzazione.

- **Codice paese dell'account** cliente: è obbligatorio specificare un codice paese di due lettere (ISO 3166) quando si crea una nuova segnalazione. Per impostazione predefinita, il codice paese verrà sincronizzato con e dal campo **BillingCountry** dell'account in Salesforce. Se si dispone di un campo diverso in Salesforce per il codice paese da cui eseguire la sincronizzazione:

  - Per un campo codice paese non di ricerca nell'account che contiene un codice di due lettere:

    - Aggiornare il **nome del campo Customer Account Country Code** nella variabile di ambiente Salesforce con il nome del campo crm. Assicurarsi di specificare il nome del campo, non il nome visualizzato.

    - Modificare **[Personalizza]** Crea o Ottieni dettagli da Salesforce e passare a Crea o ottieni account cliente nell'azione **CRM** per assegnare un valore **Country** al campo corretto in CRM. Rimuovere anche **l'assegnazione di** valore Country da **BillingCountry**.

  - Per un campo codice paese basato su ricerca nell'account:

    - Aggiungere un nuovo campo personalizzato nell'account e popolarlo automaticamente con un codice paese di due lettere (ISO 3166) in base al valore selezionato nel campo basato su ricerca e viceversa.

    - Seguire i passaggi precedenti per il campo codice paese non di ricerca per sincronizzare un nuovo campo personalizzato da CRM a e da Partner Center.

- **Valore dell'offerta:** per impostazione predefinita, il valore dell'Partner Center verrà sincronizzato da e verso **Amount** nel CRM. Se nel CRM è presente un campo diverso da cui eseguire la sincronizzazione del valore dell'offerta:

  - Aggiornare il **nome del campo** Valore deal nella variabile di ambiente Salesforce con il nome del campo crm. Assicurarsi di specificare il nome del campo, non il nome visualizzato.

  - Modificare **[Personalizza]** Crea o Ottieni dettagli da Salesforce e passare **a** Crea o  aggiorna opportunità **in** CRM e aggiornare le azioni Crea una nuova opportunità e Aggiorna opportunità esistenti per assegnare **DealValue** al campo corretto in Salesforce.

- **Codice valuta del valore dell'offerta:** nome del campo del codice valuta del valore dell'offerta in Salesforce. Questo nome API di campo verrà usato per ottenere il codice valuta del valore dell'offerta di Opportunity durante la creazione o l'aggiornamento della segnalazione in Microsoft Partner Center. Se il campo codice valuta valore trattativa è diverso dal campo **predefinito CurrencyIsoCode**, aggiornare il valore corrente di questa variabile di ambiente.

  - Aggiornare il **nome del campo Valuta** valore deal nella variabile di ambiente Salesforce con il nome del campo crm. Assicurarsi di specificare il nome del campo, non il nome visualizzato.

  - Modificare **[Personalizza]** Crea o Ottieni dettagli da Salesforce e passare **a** Crea o  aggiorna opportunità **in** CRM e aggiornare le azioni Crea una nuova opportunità e Aggiorna opportunità esistente per assegnare **DealValueCurrency** al campo corretto in Salesforce.

- **Sincronizza opportunità di co-selling:** se l'opzione è impostata su **sì,** verranno sincronizzate solo le opportunità di co-selling e condivisione della pipeline Partner Center a Salesforce. Se impostato su **no,** le opportunità di condivisione di lead, co-selling e pipeline verranno sincronizzate Partner Center a Salesforce. Questa variabile non ha alcun impatto sulle opportunità sincronizzate da Salesforce a Partner Center.

## <a name="update-environment-variable"></a>Aggiornare la variabile di ambiente

Per aggiornare il valore di una variabile di ambiente:

1. Passare alla pagina **Soluzioni** e selezionare **Soluzione predefinita**. Selezionare **Variabile di** ambiente selezionando **Tutti**.

1. Selezionare la variabile di ambiente per il valore che deve essere aggiornato e selezionare **Modifica** usando l'icona con i puntini di sospensione.

1. Aggiornare **il valore** corrente (non aggiornare il valore **predefinito)** usando l'opzione Nuovo **valore** e specificando il valore . Il valore deve corrispondere al tipo di dati della variabile. Ad esempio, il tipo di dati Sì o No accetterà il valore Sì o No.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Screenshot che mostra Aggiornare le variabili di ambiente.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronizzazione delle segnalazioni di co-selling bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power Automate, è possibile testare la sincronizzazione delle segnalazioni di co-selling tra Salesforce CRM e Partner Center.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve delimitare chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione offre ai team venditori la possibilità di decidere quali segnalazioni condividere con Microsoft per la co-selling.

Un set di campi personalizzati è disponibile come parte dell'entità opportunità Partner Center di sincronizzazione delle **segnalazioni** per la soluzione Salesforce CRM. Un utente amministratore di CRM dovrà creare una sezione CRM separata con i **campi** personalizzati Opportunità.

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizza con Partner Center:** indica se sincronizzare l'opportunità con Partner Center. Per impostazione predefinita, il valore di questo campo è No e deve essere impostato in modo esplicito su Sì dal venditore per condividere un'opportunità con Microsoft. Le nuove segnalazioni condivise da Partner Center a CRM avranno questo valore di campo impostato su Sì.

- **Identificatore di riferimento:** campo dell'identificatore di sola lettura per microsoft Partner Center riferimento.

- **Collegamento alla segnalazione:** collegamento di sola lettura alla segnalazione in Microsoft Partner Center.

- **Come può essere utile Microsoft:** guida necessaria a Microsoft per la segnalazione. Per creare una segnalazione di co-selling, selezionare la Guida appropriata richiesta da Microsoft. Un contatto del cliente deve essere associato all'opportunità di creare una segnalazione di co-selling. Per creare una segnalazione di non co-selling, non selezionare questo campo. Una segnalazione di non co-selling può essere convertita in una segnalazione di co-selling in qualsiasi momento selezionando l'opzione appropriata per la guida necessaria.

- **Visibilità delle segnalazioni di Microsoft Partner Center:** selezionare la visibilità per la Partner Center segnalazione. Rendendola visibile ai venditori Microsoft, una segnalazione di co-selling potrebbe essere convertita in co-selling. Quando è richiesta assistenza Microsoft, la segnalazione è visibile ai venditori Microsoft per impostazione predefinita. Dopo che questo campo è stato contrassegnato come visibile, non può essere ripristinato.

- **Identificatore Microsoft CRM:** quando microsoft crea e accetta una segnalazione di co-selling, questo campo viene popolato con l'identificatore CRM di Microsoft.

- **Microsoft Partner Center Solutions:** oggetto personalizzato per associare all'opportunità soluzioni pronte per il co-selling o soluzioni Microsoft. È possibile aggiungere o rimuovere una o più soluzioni dall'opportunità. È obbligatorio aggiungere all'opportunità almeno una soluzione Microsoft o pronta per il co-selling prima di condividerla con Microsoft. Per associare questo oggetto all'opportunità, aggiornare il **modulo Opportunità** in CRM.

- **Controllo:** un'audit trail di sola lettura per la sincronizzazione con Partner Center segnalazioni

### <a name="scenarios"></a>Scenari

1. Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in CRM e sincronizzata in Partner Center:

   1. Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella **sezione Opportunità** di CRM.

   1. Assicurarsi che la sezione **Microsoft Partner Center** sia presente quando si crea una **nuova opportunità** nell'ambiente Salesforce CRM.

   1. Le opportunità che vengono sincronizzate correttamente con Partner Center verranno identificate con ✔'icona in Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Screenshot dell'ambiente Salesforce.":::

   1. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Come può essere utile Microsoft?**: per creare una segnalazione di co-selling, selezionare un'opzione di assistenza appropriata.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Screenshot che mostra come ottenere i campi appropriati nella visualizzazione scheda.":::

      - **Sincronizza con Partner Center:** Sì
      - **Contatto cliente:** per creare una segnalazione di co-selling, aggiungere un contatto cliente all'opportunità.
      - **Soluzioni Microsoft:** per condividere una segnalazione con Microsoft, aggiungere all'opportunità una soluzione Valida pronta per il co-selling o Microsoft.

   1. Dopo aver impostato l'opzione **Sincronizza con Partner Center** su Sì, attendere 10 minuti e accedere all'account Partner Center servizio.  Le segnalazioni verranno sincronizzate con Salesforce CRM e il collegamento alla segnalazione verrà popolato. Se si verifica un errore, il campo Controllo verrà popolato con le informazioni sull'errore.

   1. Analogamente, quando l'opzione **Sincronizza con Partner Center** è impostata su Sì , se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account Partner Center personale. 

2. Sincronizzazione dei riferimenti quando la segnalazione viene creata o aggiornata in Microsoft Partner Center sincronizzata nell'ambiente Salesforce CRM:

    1. Accedere al [dashboard Partner Center.](https://partner.microsoft.com/dashboard/home)

    1. Selezionare **Segnalazioni** dal menu a sinistra.

    1. Creare una nuova segnalazione di co-selling Partner Center facendo clic sull'opzione "Nuova trattativa".

    1. Accedere all'ambiente Salesforce CRM.

    1. Passare a **Open Opportunities (Apri opportunità).** La segnalazione creata in Microsoft Partner Center è ora sincronizzata in Salesforce CRM.

    1. Quando si seleziona una segnalazione sincronizzata, i dettagli della visualizzazione scheda vengono popolati.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Screenshot della pagina dell'opportunità salesforce.":::

>[!NOTE]
>**Serve aiuto per la distribuzione?**
>Per assistenza con la distribuzione del connettore di segnalazione di co-selling, è possibile coinvolgere un consulente tecnico partner. Possono fornire assistenza per la distribuzione e procedure consigliate per una corretta implementazione.
>
>Per altre informazioni, vedere [Come inviare una richiesta tecnica di prevendita e servizi di distribuzione](technical-benefits.md)

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)

- [Webhook del Centro per i partner](/partner-center/develop/partner-center-webhooks)
