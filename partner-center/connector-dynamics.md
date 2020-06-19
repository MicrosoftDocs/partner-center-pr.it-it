---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Dynamics 365 CRM
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 3b5170edaaadca3c4045e7ebed174b5d52b06bdd
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991648"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Co-selling Connector per Dynamics 365 CRM-Panoramica

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM. Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling. Usare i connettori di co-selling, per creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare/rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura. È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling. È possibile eseguire tutti i riferimenti all'interno del CRM scelto, anziché nel centro per i partner. 

La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.

## <a name="before-you-install---pre-requisites"></a>Prima di installare-prerequisiti

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |È necessario un ID MPN valido|Per aggiungere [MPN](https://partner.microsoft.com/)|
|Coselling pronto|La soluzione IP/servizi deve essere pronta per il co-selling.|[Vendi con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Account del Centro per i partner|L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling. Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|Il ruolo utente CRM è amministratore sistema o sistema verbi|[Assegnare i ruoli in Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizzare l'account di flusso|Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema. L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 (soluzione Power automatici)

1. Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro. In questo passaggio vengono visualizzate le istanze di CRM disponibili.

2. Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.

3. Selezionare **soluzioni** sulla barra di spostamento a sinistra.

4. Fare clic sul collegamento **Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. Cercare i **connettori dei riferimenti del centro per i partner per Dynamics 365** nella schermata popup.  

6. Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.

7. Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.  Accettare i termini e le condizioni.

8. Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .  Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina. L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner. L'installazione può richiedere 10-15 minuti. 

9. Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra. Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Dynamics 365** è disponibile nell'elenco soluzioni.

10. Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**. Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="DISPONGONO disponibili":::

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: testare prima di iniziare

Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.

- Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.
- Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.
- Testare la soluzione in un'istanza di staging/CRM. 
- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione. 

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).

2. Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.

3. È necessario creare connessioni che associano i tre account utente:

   - Utente del centro per i partner con credenziali di amministratore per i riferimenti

   - Eventi del Centro per i partner

   - L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.

      1. Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.

      2. Creare una connessione facendo clic su **Crea una connessione**.

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Creare la connessione":::

      3. Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.

      4. Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.

      5. Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.

      6. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.

4. Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner. Salvare le modifiche.

5. **Attivare** i flussi di automazione dell'alimentazione.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API webhook per registrare gli eventi di modifica delle risorse

Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .

2. Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Quando si effettuano questi aggiornamenti, viene visualizzato

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. Salvare le modifiche e selezionare **attiva**.

   Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:

5. Selezionare **centro per i partner per Dynamics 365 (insider Preview)**.

6. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

7. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copia l'URL":::

8. Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.

9. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.

10. Immettere i dettagli seguenti:

    1. **Endpoint trigger http**: URL copiato dal passaggio precedente

    2. **Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"

    3. Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).

11. Selezionare **Esegui** , quindi fare clic su **fine.**

Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.

Spesso i sistemi CRM sono altamente personalizzati. È possibile personalizzare i flussi di automazione dell'alimentazione. Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.  Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.

È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze. Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:

1. Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM: 

    a. Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).

    b. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

    c. Selezionare **(ambito) sincronizzare il lead o l'opportunità**.

2. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**. È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.

    d. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".

    e. Selezionare **se è un aggiornamento a un'opportunità, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.  

    f. Selezionare **se sì** seguito da **Aggiorna opportunità esistente**

3. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:

    a. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

    b. Selezionare **(ambito) sincronizzare l'opportunità**.

    c. Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare **se c'è differenza tra gli oggetti lead in Partner Center e CRM, quindi**. 

    d. Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.

   È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

4. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?

   a. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   b. Selezionare **(ambito) sincronizzare i riferimenti.**

   c. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.

   È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronizzazione del riferimento bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 e centro per i partner.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM, la soluzione Power automatizzate delimita chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione consente ai team dei venditori di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.

Un set di campi personalizzati è disponibile come parte dell'entità **opportunity** . Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft

- **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft

- **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft

- In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento

- **Prodotti**: elenco dei prodotti associati a questa opportunità

- **Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner

### <a name="scenarios"></a>SCENARI

1. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:

   1. Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.

   2. Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Opportunità":::

   3. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Sincronizza con il centro per i partner**: Sì

      - **Come può essere utile Microsoft?**: selezionare una delle opzioni seguenti:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Selezioni della Guida":::

      - **Prodotti**: ID soluzione del prodotto

   4. Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti e quindi accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Dynamics 365.

   5. Analogamente, per un'opportunità con l'opzione "Sync with partner Center" impostata su "Yes", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.

   6. Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.

2. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:

   1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

   2. Selezionare **riferimenti** dal menu a sinistra.

   3. Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".

   4. Accedere al proprio ambiente Dynamics 365 CRM.

   5. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.

   6. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](https://docs.microsoft.com/power-automate/)

- [Webhook del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)