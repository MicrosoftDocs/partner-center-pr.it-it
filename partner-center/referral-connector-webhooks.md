---
title: Usare i webhook per ottenere gli eventi di modifica delle risorse
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare le API webhook per scoprire quando si verificano modifiche alle risorse dei riferimenti
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: riferimenti, API webhook, eventi di modifica delle risorse
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796207"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API webhook per registrare gli eventi di modifica delle risorse

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- System Admin o System verbi per Dynamics 365 CRM o Salesforce CRM


Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

>[!NOTE]
>Questo argomento illustra le API webhook per Dynamics 365 CRM e Salesforce CRM.

1. Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .

2. Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito

![Trigger](images/cosellconnectors/triggerflow.png)

3. Quando si effettuano questi aggiornamenti, viene visualizzato

![Webhook](images/cosellconnectors/webhook1.png)

4. Salvare le modifiche e selezionare **attiva**. 

Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi negli oggetti di riferimento di co-selling/indipendenti IP nel centro per i partner e nei sistemi CRM, seguire questa procedura:

5. Selezionare **centro per i partner per Dynamics 365 (insider Preview)** o **Partner Center a Salesforce (insider Preview)**.

6. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

7. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

![Copia l'URL](images/cosellconnectors/copyurl.png)

8. Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.

9. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.

10. Immettere i dettagli seguenti: 

    a. **Endpoint trigger http**: URL copiato dal passaggio precedente

    b. **Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"

    c. Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).

Il webhook può ora restare in ascolto delle modifiche (creazione e aggiornamento degli eventi). 

11. Selezionare **Esegui** , quindi fare clic su **fine.**

 ## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.

Spesso i sistemi CRM sono altamente personalizzati. È possibile personalizzare i flussi di automazione dell'alimentazione. Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.  Sono disponibili i mapping del centro per i partner Microsoft per CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.

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

    c. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**. 

    d. Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.

È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

4. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?

   a. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   b. Selezionare **(ambito) sincronizzare i riferimenti.**

   c. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**. 

È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronizzazione del riferimento bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile eseguire il test per la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 o Salesforce e centro per i partner.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM o nel centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft. In questo modo, i team dei venditori possono decidere quali riferimenti condividere con Microsoft per il co-selling.

Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Dynamics 365. Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft

- **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft

- **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft

- In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento

- **Prodotti**: elenco dei prodotti associati a questa opportunità

- **Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner

### <a name="scenarios"></a>SCENARI

1. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:

    a. Accedere all'ambiente di Dynamics 365 CRM o all'ambiente Salesforce CRM con l'utente che ha visibilità nella sezione dell' **opportunità** del CRM.

    b. Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365

   ![Opportunità](images/cosellconnectors/opportunity.png)

    c. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

    - "Sincronizza con il centro per i partner": Sì

    - "Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:

    ![Selezioni della Guida](images/cosellconnectors/help.png)

    - Prodotti: ID soluzione del prodotto

    d. Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Dynamics 365.

    e. Di conseguenza, per un'opportunità con l'opzione "Sincronizza con il centro per i partner" impostata su "Sì", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.

    f. Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.

2. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365: 

    a. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

    b. Selezionare **riferimenti** dal menu a sinistra.

    c. Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".

    d. Accedere al proprio ambiente Dynamics 365 CRM. 

    e. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.

    f. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.

 ### <a name="next-steps"></a>Passaggi successivi

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](https://docs.microsoft.com/power-automate/)

- [Eventi webhook del centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
