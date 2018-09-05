---
title: Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365 | Centro per i partner
description: L'edizione Microsoft Office 365 Enterprise E4 è stata ritirata il 7 aprile 2017. Scopri come eseguire la migrazione degli abbonamenti del cliente alle nuove versioni di Office 365.
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 545cfa5c635c9093cd0261bf35e01ba2823571ef
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876931"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365

**Si applica a**

-  Centro per i partner

Il piano Office 365 Enterprise E4 è stato ritirato il 7 aprile 2017. Dopo tale data, non sarà possibile acquistare nuovi abbonamenti a Office 365 E4 e gli abbonamenti E4 esistenti non verranno rinnovati automaticamente alla scadenza.

Gli abbonamenti E4 verranno annullati alla scadenza. Per garantire la continuità, è opportuno trasferire i clienti con abbonamenti E4 in scadenza a una delle opzioni SKU supportate indicate di seguito. Si consiglia di trasferire i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento al fine di evitare eventuali interruzioni del servizio. 

>**Nota** Entrambi gli SKU di Office 365 Enterprise E4, commerciale e per enti pubblici, sono stati ritirati.
 
Nella pagina dei dettagli dell'abbonamento, lo stato dell'abbonamento E4 è passato a "Data di scadenza [data]" da "Rinnovo automatico il [data]". 

Se usi l'API (CREST o Centro per i partner), puoi individuare gli abbonamenti in scadenza valutando la data di scadenza dell'abbonamento insieme alla proprietà auto renew = False. 

Gli abbonamenti E4 verranno impostati su auto renew=False il 7 aprile 2017. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Piani di sostituzione dell'edizione Office 365 Enterprise E4

Puoi scegliere di mantenere le stesse funzionalità di E4 oppure proporre ai clienti di trarre vantaggio dalle nuove funzionalità di Office 365 e Skype for Business Online. I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice dell'elenco di offerte nel Centro per i partner. È possibile sostituire Secure Product Enterprise E3 o Secure Productive Enterprise E5 nelle opzioni seguenti di Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.

- Opzione 1: Office 365 Enterprise E5

- Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Opzione 3: Office 365 Enterprise E3 + Skype for Business più CAL (a parità di prezzo e funzionalità con E4)

- Opzione 4: Office 365 Enterprise E3


| Funzionalità | Opzione 1 | Opzione 2 | Opzione 3 | Opzione 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Offre tutte le funzionalità incluse in Office 365 Enterprise E4? | Sì | Sì | Sì | No |
| Numeri di telefono gestiti in Office 365? | Sì | Sì | No | No |
| Numeri di telefono gestiti in locale e in Office 365 (distribuzione ibrida)? | Sì | Sì | No | No |
| Opzione per aggiungere un piano per le chiamate vocali PSTN? | Sì | Sì | No | No |
| Servizi di conferenza PSTN? | Sì | No | No | No |
| Strumenti avanzati per collaborazione, analisi e sicurezza? | Sì | No | No | No |
| Report interattivi, dashboard ed effetti di visualizzazione dei dati? | Sì | No | No | No | 
| Maggiore controllo sulla sicurezza e sulla conformità dei dati con controlli avanzati integrati per la privacy, la trasparenza e gli utenti? | Sì | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai suoi partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione dei loro abbonamenti da SKU destinati a essere ritirati. La migrazione dei clienti da SKU ritirati a quelli più recenti richiede la procedura seguente:

-   Acquistare il nuovo abbonamento
-   Riassegnare le licenze utente correnti
-   Annullare l'abbonamento precedente

Attieniti a questa procedura per eseguire la migrazione dell'abbonamento a Office 365 Enterprise E4 di un cliente a una delle opzioni incluse nella tabella precedente.

### <a name="step-1---purchase-the-new-subscription"></a>Passaggio 1: Acquistare il nuovo abbonamento

1. Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi seleziona **Aggiungi sottoscrizioni**.

2. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.

   Il cliente dovrebbe ora avere il vecchio e il nuovo abbonamento, ovvero il vecchio abbonamento a Office 365 Enterprise E4 e il nuovo abbonamento 'di destinazione', ad esempio, l'Opzione 1: Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Passaggio 2: Riassegnare le licenze utente del cliente

1. Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi seleziona **Utenti e licenze**. Viene aperta la pagina Utenti e licenze del cliente.

2. Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.

3. Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza di **Office 365 Enterprise E4** e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente.

4. Seleziona **Invia**. Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.

5. Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare l'abbonamento ritirato al livello principale del cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Passaggio 3: Annullare l'abbonamento precedente

1. Nel menu **Dashboard** seleziona **Clienti**. Seleziona il cliente da trasferire e l'abbonamento da annullare.

2. Nella pagina dei dettagli sull'abbonamento imposta lo stato su **Sospeso**.

3. Seleziona **Invia**.

L'abbonamento precedente viene sospeso e quello nuovo diventa attivo. Per l'abbonamento sospeso verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per l'abbonamento precedente.



 



