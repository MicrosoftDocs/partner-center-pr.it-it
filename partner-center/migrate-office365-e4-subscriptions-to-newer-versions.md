---
title: Eseguire la migrazione delle sottoscrizioni di Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office'edizione 365 Enterprise E4 è stata ritirata a partire dal 7 aprile 2017. Informazioni su come eseguire la migrazione delle sottoscrizioni dei clienti alle versioni più recenti di Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151560"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore | Agente di vendita

Il piano Office 365 Enterprise E4 è stato ritirato, a partire dal 7 aprile 2017. Non è più possibile acquistare nuove sottoscrizioni di Office 365 E4 dopo questa data e le sottoscrizioni E4 esistenti non verranno rinnovate automaticamente alla scadenza.

Al termine delle sottoscrizioni E4, verranno annullate. Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni E4 in scadenza a un'opzione SKU supportata, elencata di seguito. È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti. 

> [!NOTE]  
> Gli SKU commerciali e per enti pubblici di Office 365 Enterprise E4 vengono ritirati.
 
Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione E4 è stato modificato in "Scadenza alla [data]" da "Rinnovo automatico il [data]". 

Se si usa l'API (STEMM o Partner Center), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà rinnovo automatico = False. 

Le sottoscrizioni E4 verranno impostate su auto renew=False nel 7 aprile 2017. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Piani di sostituzione dell'edizione Office 365 Enterprise E4

È possibile scegliere di mantenere le stesse funzionalità con E4 o fare in modo che i clienti possano sfruttare le funzionalità e le funzionalità più nuove in Office 365 e Skype for Business Online. I dettagli dei prezzi sono disponibili nel listino prezzi e nella matrice del listino Partner Center. Secure Product Enterprise E3 o Secure Productive Enterprise E5 possono essere sostituiti rispettivamente nelle opzioni seguenti per Office 365 Enterprise E3 o Office 365 Enterprise E5.

- Opzione 1: Office 365 Enterprise E5

- Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Opzione 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (prezzo e funzionalità pari a E4)

- Opzione 4: Office 365 Enterprise E3


| Funzionalità | Opzione 1 | Opzione 2 | Opzione 3 | Opzione 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Ottenere tutte le funzionalità incluse in Office 365 Enterprise E4? | Sì | Sì | Sì | No |
| Numeri di telefono gestiti in Office 365? | Sì | Sì | No | No |
| I numeri di telefono sono gestiti sia in locale che in Office 365 (distribuzione ibrida)? | Sì | Sì | No | No |
| Opzione per aggiungere un piano di chiamate vocali PSTN? | Sì | Sì | No | No |
| Servizi di conferenza PSTN? | Sì | No | No | No |
| Strumenti avanzati per collaborazione, analisi e sicurezza? | Sì | No | No | No |
| Report interattivi, dashboard e visualizzazioni dei dati? | Sì | No | No | No | 
| Maggiore controllo sulla sicurezza dei dati e sulla conformità con la privacy, la trasparenza e i controlli utente perfezionati? | Sì | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai partner. In questi casi, potrebbe essere necessario aggiornare i clienti a nuovi servizi o eseguire la migrazione delle sottoscrizioni dagli SKU che verranno arrestati. La migrazione dei clienti da SKU ritirati a SKU più recenti richiede i passaggi seguenti:

-   Acquistare la nuova sottoscrizione
-   Riassegnare le licenze utente correnti
-   Annullare la sottoscrizione precedente

Seguire questa procedura per eseguire la migrazione della sottoscrizione di Office 365 Enterprise E4 di un cliente a una delle opzioni nella tabella precedente.

### <a name="step-1---purchase-the-new-subscription"></a>Passaggio 1- Acquistare la nuova sottoscrizione

1. Dal menu **Partner Center** selezionare **Clienti,** selezionare il cliente che si vuole spostare e quindi **selezionare Aggiungi sottoscrizioni**.

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia**.

   Il cliente deve ora avere sottoscrizioni sia nuove che vecchie, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione "di destinazione", ad esempio Opzione 1 - Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Passaggio 2: Riassegnare le licenze degli utenti del cliente

1. Nel menu **Partner Center** selezionare **Clienti,** selezionare il cliente che si vuole spostare e quindi **selezionare Utenti e licenze.** Verrà visualizzata la pagina Utenti e licenze del cliente.

2. Per riassegnare le licenze utente, selezionare l'utente da riassegnare e quindi selezionare **Gestisci licenze.**

3. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Licenza di **Office 365 Enterprise E4** e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente.

4. Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.

5. Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

Dopo aver spostate le licenze utente nel nuovo servizio, è possibile annullare in modo sicuro la sottoscrizione ritirata a livello di cliente superiore.

### <a name="step-3---cancel-the-old-subscription"></a>Passaggio 3: Annullare la sottoscrizione precedente

1. Dal menu **Partner Center** selezionare **Clienti.** Selezionare il cliente da spostare e selezionare la sottoscrizione da annullare.

2. Nella pagina dei dettagli della sottoscrizione impostare lo stato della sottoscrizione su **Sospeso.**

3. Selezionare **Submit** (Invia).

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione è attiva. Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.



 



