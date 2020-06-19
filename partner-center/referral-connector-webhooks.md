---
title: Usare i webhook per ottenere gli eventi di modifica delle risorse
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare le API webhook del centro per i partner per apprendere quando si verificano le modifiche delle risorse dei riferimenti per Dynamics 365 CRM o Salesforce CRM.
author: LauraBrenner
ms.author: labrenne
keywords: riferimenti, API webhook, eventi di modifica delle risorse
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6d3cf5a4049f96f7eebce8d23c33ca79ad352ce5
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991890"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a>Usare le API webhook per registrare gli eventi di modifica delle risorse per Dynamics 365 CRM e Salesforce CRM

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- System Admin o System verbi per Dynamics 365 CRM o Salesforce CRM

Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

>[!NOTE]
>Questo argomento illustra le API webhook per Dynamics 365 CRM e Salesforce CRM.

## <a name="configure-the-webhook"></a>Configurare il webhook

1. Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .

2. Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Quando si effettuano questi aggiornamenti, viene visualizzato

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. Salvare le modifiche e selezionare **attiva**.

   Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi negli oggetti di riferimento di co-selling/indipendenti IP nel centro per i partner e nei sistemi CRM, seguire questa procedura:

5. Selezionare **centro per i partner per Dynamics 365 (insider Preview)** o **Partner Center a Salesforce (insider Preview)**.

6. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

7. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copia l'URL":::

8. Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.

9. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.

10. Immettere i dettagli seguenti:

    1. **Endpoint trigger http**: URL copiato dal passaggio precedente

    2. **Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"

    3. Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).

    Il webhook può ora restare in ascolto delle modifiche (creazione e aggiornamento degli eventi).

11. Selezionare **Esegui** , quindi fare clic su **fine.**

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.

Spesso i sistemi CRM sono altamente personalizzati. È possibile personalizzare i flussi di automazione dell'alimentazione. Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.  Sono disponibili i mapping del centro per i partner Microsoft per CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.

È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze. Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:

1. Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:

   1. Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).

   2. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   3. Selezionare **(ambito) sincronizzare il lead o l'opportunità**.

2. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**. È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.

   1. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".

   2. Selezionare **se è un aggiornamento a un'opportunità, quindi**. Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.  

   3. Selezionare **se sì** seguito da **Aggiorna opportunità esistente**

3. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:

   1. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   2. Selezionare **(ambito) sincronizzare l'opportunità**.

   3. Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.

   4. Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.

   È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.

4. Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?

   1. Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.

   2. Selezionare **(ambito) sincronizzare i riferimenti.**

   3. Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.

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

   1. Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.

   2. Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Opportunità":::

   3. Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Sincronizza con il centro per i partner**: Sì

      - **Come può essere utile Microsoft?**: selezionare una delle opzioni seguenti:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Selezioni della Guida":::

      - **Prodotti**: ID soluzione del prodotto

   4. Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Dynamics 365.

   5. Di conseguenza, per un'opportunità con l'opzione "Sincronizza con il centro per i partner" impostata su "Sì", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.

   6. Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.

2. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:

   1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

   2. Selezionare **riferimenti** dal menu a sinistra.

   3. Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".

   4. Accedere al proprio ambiente Dynamics 365 CRM.

   5. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.

   6. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](https://docs.microsoft.com/power-automate/)

- [Eventi webhook del centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
