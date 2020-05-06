---
title: Eseguire la migrazione delle sottoscrizioni di Office 365 E4 a versioni più recenti di Office 365 | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 è stato ritirato a partire dal 7 aprile 2017. Informazioni su come eseguire la migrazione delle sottoscrizioni dei clienti a versioni più recenti di Office 365.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 02d383172595e09a4ab0bf9c6db34862fcc17204
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798877"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365

**Si applica a**

-  Centro per i partner

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente amministratore
-   Agente di vendita

Il piano Office 365 Enterprise E4 è stato ritirato, a partire dal 7 aprile 2017. Non è più possibile acquistare nuove sottoscrizioni di Office 365 E4 dopo questa data e le sottoscrizioni E4 esistenti non verranno rinnovate automaticamente alla scadenza.

Quando le sottoscrizioni E4 sono terminate, verranno annullate. Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni E4 in scadenza a un'opzione SKU supportata, elencate di seguito. È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti. 

> [!NOTE]  
>  Gli SKU di Office 365 Enterprise E4 Commercial e government sono stati ritirati.
 
Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione E4 è stato modificato in "scade in data [DATE]" da "auto renews on [DATE]". 

Se si usa l'API (CREST o centro per i partner), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false. 

Le sottoscrizioni E4 verranno impostate su auto Renew = false nel 7 aprile 2017. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Piani di sostituzione di Office 365 Enterprise E4 Edition

È possibile scegliere di mantenere la stessa funzionalità con E4 o chiedere ai clienti di sfruttare le funzionalità e le funzionalità più recenti di Office 365 e Skype for business online. I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner. Secure Product Enterprise E3 o Secure produttiva Enterprise E5 possono essere sostituiti dalle opzioni seguenti per Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.

- Opzione 1: Office 365 Enterprise E5

- Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Opzione 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (parità prezzo e funzionalità con E4)

- Opzione 4: Office 365 Enterprise E3


| Funzionalità | Opzione 1 | Opzione 2 | Opzione 3 | Opzione 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Ottenere tutte le funzionalità incluse in Office 365 Enterprise E4? | Sì | Sì | Sì | No |
| Numeri di telefono gestiti in Office 365? | Sì | Sì | No | No |
| Numeri di telefono gestiti sia in locale che in Office 365 (distribuzione ibrida)? | Sì | Sì | No | No |
| È possibile aggiungere un piano di chiamata vocale PSTN? | Sì | Sì | No | No |
| Conferenze PSTN? | Sì | No | No | No |
| Strumenti avanzati per la collaborazione, l'analisi e la sicurezza? | Sì | No | No | No |
| Report interattivi, dashboard e visualizzazioni dei dati? | Sì | No | No | No | 
| Maggiore controllo sulla sicurezza dei dati e sulla conformità con la privacy incorporata, la trasparenza e i controlli utente perfezionati? | Sì | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate. Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:

-   Acquistare la nuova sottoscrizione
-   Riassegna licenze utente correnti
-   Annullare la sottoscrizione precedente

Seguire questa procedura per eseguire la migrazione della sottoscrizione di Office 365 Enterprise E4 di un cliente a una delle opzioni nella tabella precedente.

### <a name="step-1---purchase-the-new-subscription"></a>Passaggio 1: acquistare la nuova sottoscrizione

1. Dal menu **centro partner** selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).

   Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Passaggio 2: riassegnare le licenze degli utenti del cliente

1. Dal menu **centro** per i partner selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **utenti e licenze**. Verrà visualizzata la pagina utenti e licenze del cliente.

2. Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.

3. Nella pagina **Gestisci licenze** deselezionare la casella di controllo licenza di **Office 365 Enterprise E4** e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.

4. Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.

5. Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

Dopo aver spostato le licenze utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata al livello superiore del cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Passaggio 3: annullare la sottoscrizione precedente

1. Scegliere **clienti**dal menu **centro partner** . Selezionare il cliente da spostare e selezionare la sottoscrizione che si vuole annullare.

2. Nella pagina Dettagli sottoscrizione impostare lo stato della sottoscrizione su **sospeso**.

3. Selezionare **Submit** (Invia).

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione è attiva. Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.



 



