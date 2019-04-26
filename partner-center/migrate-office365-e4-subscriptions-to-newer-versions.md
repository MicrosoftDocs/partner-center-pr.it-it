---
title: Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365 | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
description: L'edizione Microsoft Office 365 Enterprise E4 è stata ritirata il 7 aprile 2017. Scopri come eseguire la migrazione degli abbonamenti del cliente alle nuove versioni di Office 365.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e14ffbfaeaec64e8ccf3612cba9ed0f27aa31968
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134381"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365

**Si applica a**

-  Centro per i partner

Il piano Office 365 Enterprise E4 è stato ritirato il 7 aprile 2017. Dopo tale data, non sarà possibile acquistare nuovi abbonamenti a Office 365 E4 e gli abbonamenti E4 esistenti non verranno rinnovati automaticamente alla scadenza.

Gli abbonamenti E4 verranno annullati alla scadenza. Per garantire la continuità, è opportuno trasferire i clienti con abbonamenti E4 in scadenza a una delle opzioni SKU supportate indicate di seguito. Si consiglia di far passare i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento, al fine di evitare eventuali interruzioni del servizio. 

> [!NOTE]  
>  Sono stati ritirati sia Office 365 Enterprise E4 commerciale e gli SKU per enti pubblici.
 
Nella pagina dei dettagli dell'abbonamento, lo stato dell'abbonamento E4 è passato a "Data di scadenza [data]" da "Rinnovo automatico il [data]". 

Se usi l'API (CREST o Centro per i partner), puoi individuare gli abbonamenti in scadenza valutando la data di scadenza dell'abbonamento insieme alla proprietà auto renew = False. 

Gli abbonamenti E4 verranno impostati su auto renew=False il 7 aprile 2017. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Piani di sostituzione dell'edizione Office 365 Enterprise E4

Puoi scegliere di mantenere le stesse funzionalità di E4 oppure proporre ai clienti di trarre vantaggio dalle nuove funzionalità di Office 365 e Skype for Business Online. I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice dell'elenco di offerte nel Centro per i partner. È possibile sostituire Secure Product Enterprise E3 o Secure Productive Enterprise E5 nelle opzioni seguenti di Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.

- Opzione 1: Office 365 Enterprise E5

- Opzione 2: Office 365 Enterprise E3 + Skype per Business Cloud PBX

- Opzione 3: Office 365 Enterprise E3 + Skype for Business e CAL (parità di funzionalità e prezzo con E4)

- Opzione 4: Office 365 Enterprise E3


| Funzionalità | Opzione 1 | Opzione 2 | Opzione 3 | Opzione 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Offre tutte le funzionalità incluse in Office 365 Enterprise E4? | Yes | Yes | Yes | No |
| Numeri di telefono gestiti in Office 365? | Yes | Yes | No | No |
| Numeri di telefono gestiti in locale e in Office 365 (distribuzione ibrida)? | Yes | Yes | No | No |
| Opzione per aggiungere un piano per le chiamate vocali PSTN? | Yes | Yes | No | No |
| Servizi di conferenza PSTN? | Yes | No | No | No |
| Strumenti avanzati per collaborazione, analisi e sicurezza? | Yes | No | No | No |
| Report interattivi, dashboard ed effetti di visualizzazione dei dati? | Yes | No | No | No | 
| Maggiore controllo sulla sicurezza e sulla conformità dei dati con controlli avanzati integrati per la privacy, la trasparenza e gli utenti? | Yes | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai suoi partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione dei loro abbonamenti da SKU destinati a essere ritirati. La migrazione dei clienti da SKU ritirati a quelli più recenti richiede la procedura seguente:

-   Acquistare la nuova sottoscrizione
-   Riassegnare le licenze utente correnti
-   Annullare la sottoscrizione precedente

Attieniti a questa procedura per eseguire la migrazione dell'abbonamento a Office 365 Enterprise E4 di un cliente a una delle opzioni incluse nella tabella precedente.

### <a name="step-1---purchase-the-new-subscription"></a>Passaggio 1: Acquistare il nuovo abbonamento

1. Dal **Centro per i Partner** dal menu **clienti**, seleziona il cliente desideri spostare e quindi selezionare **aggiungere sottoscrizioni**.

2. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.

   Il cliente dovrebbe ora avere il vecchio e il nuovo abbonamento, ovvero il vecchio abbonamento a Office 365 Enterprise E4 e il nuovo abbonamento 'di destinazione', ad esempio, l'Opzione 1: Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Passaggio 2: Riassegnare le licenze utente del cliente

1. Dal **Centro per i Partner** dal menu **clienti**, seleziona il cliente desideri spostare e quindi selezionare **utenti e licenze**. Viene aperta la pagina Utenti e licenze del cliente.

2. Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.

3. Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza di **Office 365 Enterprise E4** e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente.

4. Seleziona **Invia**. Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.

5. Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare l'abbonamento ritirato al livello principale del cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Passaggio 3: Annullare l'abbonamento precedente

1. Dal **Centro per i Partner** dal menu **clienti**. Seleziona il cliente da trasferire e l'abbonamento da annullare.

2. Nella pagina dei dettagli sull'abbonamento imposta lo stato su **Sospeso**.

3. Seleziona **Invia**.

L'abbonamento precedente viene sospeso e quello nuovo diventa attivo. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.



 



