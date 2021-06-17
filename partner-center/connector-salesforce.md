---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare le segnalazioni Partner Center con Salesforce CRM. I venditori possono quindi eseguire il co-selling con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276978"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connettore di co-selling per CRM Salesforce - Panoramica

**Ruoli appropriati:** amministratore delle segnalazioni | Amministratore di sistema o a personalizzatore di sistema in CRM

Partner Center connettore di co-selling consente ai venditori di co-selling con Microsoft dall'interno dei sistemi CRM. Non sarà necessario eseguire il training per usare le Partner Center per gestire le trattative di co-selling. Usando i connettori di co-selling, puoi creare una nuova segnalazione di co-selling per coinvolgere un venditore Microsoft, ricevere segnalazioni dal venditore Microsoft, accettare/rifiutare le segnalazioni, modificare i dati delle trattative, ad esempio il valore della trattativa e la data di chiusura.  È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft su queste trattative di co-selling. È possibile eseguire tutte le segnalazioni mentre si lavora all'interno del sistema CRM preferito anziché in Partner Center. 

La soluzione è basata su Microsoft Power Automate e usa Partner Center API.

## <a name="before-you-install---pre-requisites"></a>Prima di installare : prerequisiti

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|Microsoft Partner Network ID |È necessario un ID MPN valido|Per partecipare [a MPN](https://partner.microsoft.com/)|
|Pronto per il co-selling|La soluzione IP/Servizi deve essere pronta per il co-selling.|[Vendere con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Account del Centro per i partner|L'ID MPN associato al tenant Partner Center deve corrispondere all'ID MPN associato alla soluzione di co-selling. Verificare che sia possibile visualizzare le segnalazioni di co-selling Partner Center portale prima di distribuire i connettori.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore delle segnalazioni|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|Il ruolo utente CRM è Amministratore di sistema o A personalizzatore sistema|[Assegnare ruoli in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Un account [di Power Automate](https://flow.microsoft.com) per l'amministratore di sistema CRM o l'asonalizzazione del sistema. Tale utente deve accedere [al](https://flow.microsoft.com) Power Automate almeno una volta prima dell'installazione.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installazione del pacchetto Salesforce per i campi personalizzati Microsoft 

Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve identificare chiaramente i campi di segnalazione specifici di Microsoft. Questa delimitazione offre ai team venditori dei partner la possibilità di decidere quali segnalazioni condividere con Microsoft per il co-selling.

1. In Salesforce attivare Note **e** aggiungerlo all'elenco correlato alle opportunità. 
[Riferimento](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Attivare **i team opportunity** seguendo questa procedura: 
    - In Configurazione usare la casella **Ricerca rapida per** individuare Opportunity Team Settings (Impostazioni team opportunità).
    - Definire le impostazioni in base alle esigenze.
[Riferimento](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. In Salesforce installare campi e oggetti personalizzati usando il programma [di installazione del pacchetto](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Usare questa opzione per installare il pacchetto in qualsiasi società.

>[!NOTE]
>Se si sta installando in una sandbox, è necessario sostituire la parte iniziale dell'URL con http://test.salesforce.com

4. In Salesforce aggiungere Soluzioni Microsoft **all'elenco Correlato** alle opportunità. Dopo l'aggiunta, selezionare **l'icona della chiave inglese** e aggiornare le proprietà

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: eseguire il test prima di iniziare a essere live

Prima di installare, configurare e personalizzare la soluzione Power Automate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza crm di staging.

- Installare la soluzione Microsoft Power Automate in un ambiente di gestione temporanea o in un'istanza di CRM.

- Creare una copia della soluzione ed eseguire la configurazione e Power Automate le personalizzazioni del flusso nell'ambiente di gestione temporanea.

- Testare la soluzione in un'istanza di staging/CRM.

- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installare la Partner Center delle segnalazioni per Salesforce CRM

1. Passare a [Power Automate](https://flow.microsoft.com) e selezionare **Ambienti nell'angolo** superiore destro. Verranno mostrate le istanze crm disponibili.

2. Selezionare l'istanza di CRM appropriata nell'elenco a discesa nell'angolo superiore destro.

3. Selezionare **Soluzioni** sulla barra di spostamento a sinistra.

4. Selezionare il **collegamento Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Aprire AppSource.":::

5. Cercare Partner Center **Referrals Connectors for Salesforce** nella schermata popup.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. Selezionare il **pulsante Scarica adesso** e quindi **Continua.**

7. Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.  Accettare termini e condizioni.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CrmS disponibile.":::

8. Si verrà quindi indirizzati alla **pagina Gestisci le** soluzioni.  Passare a "Partner Center segnalazioni" usando i pulsanti freccia nella parte inferiore della pagina. **L'installazione** pianificata dovrebbe essere visualizzata Partner Center soluzione Segnalazioni. L'installazione può richiedere 10-15 minuti.

9. Al termine dell'installazione, tornare [all'Power Automate](https://flow.microsoft.com) e selezionare **Soluzioni nell'area** di spostamento a sinistra. Si noti **che Partner Center delle segnalazioni per Salesforce** è disponibile nell'elenco Soluzioni.

10. Selezionare **Partner Center referrals Synchronization for Salesforce (Sincronizzazione delle segnalazioni per Salesforce).** Sono disponibili Power Automate seguenti flussi ed entità:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flussi di Salesforce.":::



## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare [a Power Automate](https://flow.microsoft.com/).

2. **Nell'elenco a** discesa Ambienti nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la Power Automate soluzione.
3. Sarà necessario creare connessioni che associano i tre account utente:
    - Partner Center utente con le credenziali di amministratore delle segnalazioni
    - Eventi del Centro per i partner
    - Amministratore CRM con i Power Automate nella soluzione.
4. Selezionare **Connessioni** dalla barra di spostamento a sinistra e selezionare la soluzione "segnalazioni Partner Center" dall'elenco.

5. Creare una connessione facendo clic **su Crea una connessione**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Creare una connessione.":::

- Cercare Partner Center segnalazioni (anteprima) nella barra di ricerca nell'angolo in alto a destra.

- Creare una connessione per l'Partner Center utente con il ruolo credenziali di amministratore delle segnalazioni.

-  Creare quindi una connessione Partner Center eventi per l'utente Partner Center con le credenziali di amministratore delle segnalazioni.

- Creare una connessione per Salesforce per l'utente amministratore di CRM.

-  Dopo aver aggiunto tutte le connessioni, nell'ambiente dovrebbero essere presenti le connessioni seguenti:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Osservare le connessioni.":::

### <a name="edit-the-connections"></a>Modificare le connessioni

1. Tornare alla pagina Soluzioni e selezionare **Soluzione predefinita.**  Selezionare **Riferimento alla connessione (anteprima)** facendo clic su **Tutti**.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniziare la modifica del connettore.":::

2. Modificare ognuna delle connessioni singolarmente selezionando l'icona con i tre puntini. Aggiungere le connessioni pertinenti.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modificare i connettori.":::

3. Attivare i flussi nella sequenza seguente:

- Partner Center Webhook Registration (Insider Preview)
- Creare una segnalazione di co-selling - Salesforce per Partner Center (Insider Preview)
- Partner Center microsoft co-selling referral updates to Salesforce (Insider Preview)
- Partner Center a Salesforce (Insider Preview)
- Da Salesforce a Partner Center (Insider Preview)
- Opportunità di salesforce per Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API webhook per la registrazione per gli eventi di modifica delle risorse

Le PARTNER CENTER Webhook consentono di registrarsi per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Per registrare l'URL, **selezionare Partner Center webhook registration (Insider Preview) Power Automate** flusso.

2. Aggiungere connessioni per (a.) Partner Center utente con credenziali di amministratore delle segnalazioni (b.) Partner Center eventi come evidenziato di seguito

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Grilletto.":::

3. Quando si apportano questi aggiornamenti, viene visualizzato

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook.":::

4. Salvare le modifiche e selezionare **Attiva**.

   Per abilitare Partner Center webhook per l'ascolto delle modifiche degli eventi, seguire questa procedura:

5. Selezionare **Partner Center a Salesforce CRM (Insider Preview)**.

6. Selezionare **l'icona** Modifica e selezionare **Quando viene ricevuta una richiesta HTTP.**

7. Selezionare **l'icona** Copia per copiare l'URL HTTP POST specificato.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiare l'URL.":::

8. Selezionare ora il flusso di Partner Center webhook (Insider Preview) Power Automate e selezionare **Esegui**.

9. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e selezionare **Continua.**

10. Immettere i dettagli seguenti:

    1. **Endpoint trigger HTTP:** URL copiato dal passaggio precedente

    2. **Eventi da registrare:**"referral-created" e "referral-updated"

    3. **Sovrascrivi gli endpoint del trigger esistenti se presenti:** Sì (in questo modo vengono sovrascritti tutti gli endpoint esistenti).

11. Selezionare **Esegui** e quindi **Fare clic su Fine.**

Il webhook può ora restare in ascolto degli eventi di creazione e aggiornamento.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

Quando le segnalazioni di co-selling vengono sincronizzate tra Partner Center e il sistema CRM, i campi sincronizzati Partner Center PC sono elencati qui.

Spesso i sistemi CRM sono altamente personalizzati. È possibile personalizzare i Power Automate flusso. Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei Power Automate flusso.  Vengono forniti mapping da Microsoft Partner Center a CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.

È possibile personalizzare più passaggi di Power Automate flusso di lavoro in base alle esigenze. Di seguito sono riportati esempi di personalizzazioni disponibili:

1. Per personalizzare i campi per gli eventi di creazione o aggiornamento nel Partner Center alla sincronizzazione delle segnalazioni di CRM:

   1. Selezionare Partner Center a Salesforce CRM (Insider Preview).

   2. Selezionare **Modifica** per modificare o personalizzare il flusso Power Automate dati.

   3. Selezionare **(Ambito) Sincronizzare il lead o l'opportunità.**

2. Per personalizzare i mapping dei campi CRM per la creazione di eventi, selezionare Se si tratta di una **nuova opportunità condivisa, quindi**. Selezionare il passaggio secondario **in caso affermativa** e quindi espandere **Creazione di una nuova opportunità in CRM**. È possibile modificare i mapping in questa sezione usando la Guida al mapping dei campi.

   1. Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare il passaggio "(Ambito) Sincronizzare il lead o l'opportunità".

   2. Selezionare **Se si tratta di un aggiornamento di un'opportunità, quindi**. Selezionare il passaggio secondario **in caso affermativa** e quindi espandere Se la differenza tra gli oggetti opportunità in Partner Center **e CRM, quindi**.  

   3. Selezionare **Se sì seguito** da Aggiorna opportunità **esistente**

3. Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per gli eventi di aggiornamento:

   1. Selezionare **Modifica**  per modificare o personalizzare il flusso Power Automate dati.

   2. Selezionare **(Ambito) Sincronizzare l'opportunità.**

   3. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per gli eventi di aggiornamento, selezionare Se esiste una differenza tra gli oggetti lead **in Partner Center e CRM, quindi**.

   4. Selezionare il passaggio secondario **in caso affermativa,** quindi espandere il passaggio **Aggiornare una segnalazione con i dati dell'opportunità**.

   È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.

4. Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per la creazione di eventi?

   1. Selezionare **Modifica**  per modificare o personalizzare il flusso Power Automate dati.

   2. Selezionare **(Ambito) Sincronizzazione delle segnalazioni.**

   3. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea segnalazione Microsoft**.

È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronizzazione delle segnalazioni di co-selling bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power Automate, è possibile testare la sincronizzazione delle segnalazioni di co-selling tra Salesforce CRM e Partner Center.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve delimitare chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione offre ai team venditori la possibilità di decidere quali segnalazioni condividere con Microsoft per la co-selling.

Un set di campi personalizzati è disponibile come parte dell'entità opportunità Partner Center di sincronizzazione delle **segnalazioni** per la soluzione Salesforce CRM. Un utente amministratore di CRM dovrà creare una sezione CRM separata con i **campi** personalizzati Opportunità.

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizza con Partner Center**: indica se sincronizzare l'opportunità con Microsoft Partner Center

- **Identificatore di riferimento:** campo dell'identificatore di sola lettura per la segnalazione Partner Center Microsoft

- **Collegamento alla segnalazione:** collegamento di sola lettura alla segnalazione in Microsoft Partner Center

- **Come può essere utile Microsoft:** Guida necessaria a Microsoft per la segnalazione

- **Products**: elenco di prodotti associati a questa opportunità

- **Audit:** un'istanza di sola audit trail per la sincronizzazione con Partner Center segnalazioni

### <a name="scenarios"></a>Scenari:

1. Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in CRM e sincronizzata in Partner Center:

   1. Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella **sezione Opportunità** di CRM.

   2. Assicurarsi che la sezione seguente sia presente quando si crea una "Nuova opportunità" nell'ambiente Salesforce CRM

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce.":::

   3. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

       - "Sync with Partner Center": Sì
       - "Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:
       - Prodotti: ID soluzione del prodotto

   4. Dopo aver impostato l'opzione Sincronizza  **con Partner Center** su Sì **,** attendere 10 minuti, accedere all'account Partner Center utente. Le segnalazioni verranno sincronizzate con Salesforce CRM.

   5. Quando l'opzione "Sincronizza con Partner Center" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account Partner Center personale.

   6. Le opportunità sincronizzate correttamente con Partner Center verranno identificate con ✔icon in Salesforce CRM.

2. Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in Microsoft Partner Center sincronizzata nell'ambiente Salesforce CRM:

    1. Accedere al dashboard [Partner Center.](https://partner.microsoft.com/dashboard/home)

    2. Selezionare **Segnalazioni** dal menu a sinistra.

    3. Creare una nuova segnalazione di co-selling da Partner Center facendo clic sull'opzione "New deal".

    4. Accedere all'ambiente Salesforce CRM.

    5. Passare a **Apri opportunità**. La segnalazione creata in Microsoft Partner Center è ora sincronizzata in Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata opportunità di Salesforce.":::

    6. Quando si seleziona una segnalazione sincronizzata, i dettagli della visualizzazione scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)

- [Webhook del Centro per i partner](/partner-center/develop/partner-center-webhooks)
