---
title: Eseguire la migrazione di Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come eseguire la migrazione delle offerte Dynamics 365 Business Edition qualificate a versioni più recenti prima della scadenza.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436830"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Eseguire la migrazione delle offerte di Dynamics 365 Business Edition a versioni più recenti

**Si applica a**

- Centro per i partner

**Ruoli appropriati**
- Amministratore globale
- Amministratore utenti
- Agente amministratore
- Agente di vendita

A partire dal 1 ° gennaio 2019, i clienti con sottoscrizioni Dynamics 365 Business Edition non possono più rinnovarsi nelle offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".

Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito. È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.

Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false. Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Le edizioni di Dynamics 365 business in fase di ritiro

- Dynamics 365 for Finance and Operations, Business edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central: nuove offerte di Dynamics 365 Business Edition

Grazie alle nuove offerte di Dynamics Business Central, i clienti possono connettere i propri finanziari, le vendite, il servizio e le operazioni per semplificare i processi aziendali, migliorare le interazioni dei clienti e prendere decisioni migliori. Dynamics 365 business Central è basato sul cloud e disponibile solo per i partner di programma Cloud Solution Provider (CSP).
I clienti di Dynamics 365 Business Edition sono idonei a ricevere prezzi di transizione scontati per le nuove offerte business Central fino al 30 giugno 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

 Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:

- Acquistare la nuova sottoscrizione
- Riassegna licenze utente correnti
- Annulla sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Acquistare il nuovo piano per il cliente

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione**.
3. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**). 

Il cliente avrà ora la sottoscrizione precedente e quella nuova. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.
2. Selezionare **utenti e licenze**.
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**. 
4. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando. 
5. Selezionare **Submit** (Invia). Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza. 

Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente. 

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.
2. Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.

La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva. Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni. Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.
