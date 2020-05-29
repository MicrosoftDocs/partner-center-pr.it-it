---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Salesforce CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 128ae914ef76ba0e1431b0aa7319442b51677973
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145105"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Co-selling Connector per Salesforce CRM-Panoramica

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM. Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling. Utilizzando i connettori di co-selling, è possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.  È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling. È possibile eseguire tutte le attività di riferimento quando si lavora all'interno del CRM scelto piuttosto che nel centro per i partner. 

La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.


## <a name="before-you-install---pre-requisites"></a>Prima di installare-prerequisiti

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |È necessario un ID MPN valido|Per aggiungere [MPN](https://partner.microsoft.com/)|
|Co-selling pronto|La soluzione IP/servizi deve essere pronta per il co-selling.|[Vendi con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Account del Centro per i partner|L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling. Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|CRM Salesforce|Il ruolo utente CRM è amministratore sistema o sistema verbi|[Assegnare ruoli in Salesforce CRM](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizzare l'account di flusso|Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema. L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM

1. Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro. Vengono visualizzate le istanze di CRM disponibili.

2. Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra. 

3. Selezionare **soluzioni** sulla barra di spostamento a sinistra.

4. Fare clic sul collegamento **Apri AppSource** nel menu in alto.

![Apri AppSource](images/cosellconnectors/openappsource.png)

5. Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.  

![Salesforce](images/salesforce/salesforce1.png)

6. Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**. 

7. Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.  Accettare i termini e le condizioni.

![DISPONGONO disponibili](images/salesforce/available-crm.png)

8. Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .  Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina. L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner. L'installazione può richiedere 10-15 minuti. 

9. Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra. Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.

10. Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Salesforce**. Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:

![Flussi di Salesforce](images/salesforce/salesforce-flows.png)

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: testare prima di iniziare

Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.

- Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.

- Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.

- Testare la soluzione in un'istanza di staging/CRM.

- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione. 

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).

2. Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.

3. Sarà necessario creare connessioni che associano i tre account utente: 

- Utente del centro per i partner con credenziali di amministratore per i riferimenti 
- Eventi del Centro per i partner
- L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione. 

    a. Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.

    b. Creare una connessione facendo clic su **Crea una connessione**. 

    ![Creare la connessione](images/cosellconnectors/createconnection.png)

    c. Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.

    d. Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.

    e. Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.
    
    f. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.

4. Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner. Salvare le modifiche.

5. **Attivare** i flussi di automazione dell'alimentazione.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API webhook per registrare gli eventi di modifica delle risorse

Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .

2. Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito

![Trigger](images/cosellconnectors/triggerflow.png)

3. Quando si effettuano questi aggiornamenti, viene visualizzato

![Webhook](images/cosellconnectors/webhook1.png)

4. Salvare le modifiche e selezionare **attiva**. 

Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:

5. Selezionare **centro per i partner per Salesforce CRM (insider Preview)**.

6. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

7. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

![Copia l'URL](images/salesforce/copy-url.png)

8. Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.

9. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.

10. Immettere i dettagli seguenti: 

    a. **Endpoint trigger http**: URL copiato dal passaggio precedente

    b. **Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"

    c. Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti). 

11. Selezionare **Esegui** , quindi fare clic su **fine.**

Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.

Spesso i sistemi CRM sono altamente personalizzati. È possibile personalizzare i flussi di automazione dell'alimentazione. Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.  Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.

È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze. Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:

1. Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM: 

    a. Selezionare Centro per i partner per Salesforce CRM (insider Preview).

    b. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

    c. Selezionare **(ambito) sincronizzare il lead o l'opportunità**.

2. Per personalizzare i mapping dei campi CRM per creare eventi, selezionare **se è nuova opportunità condivisa, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**. È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.

    d. Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".

    e. Selezionare **se è un aggiornamento a un'opportunità, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.  

    f. Selezionare **se sì** seguito da **Aggiorna opportunità esistente**
       
3. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:

    a. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

    b. Selezionare **(ambito) sincronizzare l'opportunità**.

    c. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**. 

    d. Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.

È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

4. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?

   a. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   b. Selezionare **(ambito) sincronizzare i riferimenti.**

   c. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**. 

È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Creare una sezione separata nel layout delle opportunità di Salesforce CRM

Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft. In questo modo, i team dei venditori possono decidere quali riferimenti condividere con Microsoft per il co-selling.

Un set di campi personalizzati è disponibile nell'ambito della sincronizzazione dei riferimenti del centro per i partner per **Salesforce CRM.** Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .
L'utente amministratore di Salesforce CRM dovrà creare una sezione CRM separata.

I campi personalizzati seguenti devono far parte della sezione CRM:

• **Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft

• **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft

• **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft

• **Come può essere utile Microsoft?** Guida richiesta da Microsoft per il riferimento

• **Prodotti**: elenco dei prodotti associati a questa opportunità

• **Audit**: audit trail di sola lettura per la sincronizzazione con il riferimento al centro per i partner Microsoft

### <a name="set-up-fields-and-relationships"></a>Configurare campi e relazioni

1. Accedere all'account di Salesforce e passare a **opportunità**. 

2. Fare clic sulle opzioni **installazione** e **modifica oggetto** per aggiungere i campi necessari.


3. Selezionare i **campi & le relazioni** dal percorso di spostamento a sinistra

![Campi](images/salesforce/fields1.png)

4. Aggiungere i campi seguenti nella tabella "Fields & Relationship":

|**Etichetta campo**   |**Nome campo**|**Tipo di dati**|**Indicizzata**|
|---------------------|:-------------------|:--------------|:----------------|
|Sincronizza con il centro per i partner|Sync-with-partner-Center-c|CheckBox (impostazione predefinita deselezionata)||
|Prodotti|Prodotti-c|testo (255)||
|Referral | Referral_Identifier__c|Testo (100) (ID esterno)|sì|
|Collegamento di riferimento| Referral_Link__c_|URL (255)||
|Audit| Audit__c|Area di testo lungo (100.000) (riga visibile 4)||
|Come può essere utile Microsoft?|How_can_Microsoft_help__c|Picklist|

* Valori elenco a discesa:

• Proposta di valore specifico del carico di lavoro

• Architettura tecnica del cliente

• Modello di prova o demo

• Virgolette o licenze

• Esito positivo post-vendite cliente

• Generale o altro

5. i campi vengono creati in "Fields & relationships"

![Campi creati](images/salesforce/fields2.png)

6. Nel layout opportunity creare una sezione separata con i campi elencati sopra. 

    • Questa sezione dovrebbe essere disponibile per i venditori nel layout opportunità


![Layout di campi del centro per i partner](images/salesforce/pc-fields-layout.png)

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronizzazione del riferimento bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Salesforce CRM e il centro per i partner.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione consente ai team dei venditori di decidere quali riferimenti desiderano condividere con Microsoft per la co-selling.

Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Salesforce CRM. Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft

- **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft

- **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft

- **Come è possibile eseguire la Guida Microsoft**per informazioni su come richiedere Microsoft per il riferimento

- **Prodotti**: elenco dei prodotti associati a questa opportunità

- **Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner


### <a name="scenarios"></a>SCENARI

1. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:

    a. Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella sezione **opportunità** del CRM.

    b. Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Salesforce CRM

    ![Ambiente Salesforce](images/salesforce/salesforce-scenario-1.png)

   

    c. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

    - "Sincronizza con il centro per i partner": Sì

    - "Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:

   

    - Prodotti: ID soluzione del prodotto

    d. Dopo aver impostato l'opzione opportunity **Sync with partner Center** su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Salesforce CRM.

    e. Quando l'opzione "Sincronizza con il centro per i partner" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account del centro per i partner.

    f. Le opportunità che vengono sincronizzate correttamente con partner Center verranno identificate con ✔ icona in Salesforce CRM.

2. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Salesforce CRM: 

    a. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

    b. Selezionare **riferimenti** dal menu a sinistra.

    c. Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".

    d. Accedere all'ambiente Salesforce CRM. 

    e. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Salesforce CRM.

    ![Schermata di opportunità di Salesforce](images/salesforce/salesforce-casino-e.png)

    f. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.





## <a name="next-steps"></a>Passaggi successivi

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](https://docs.microsoft.com/-automate/)

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)

- [Webhook del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)