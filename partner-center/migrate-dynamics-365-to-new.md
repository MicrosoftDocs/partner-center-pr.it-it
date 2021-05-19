---
title: Eseguire la migrazione di Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione di offerte Dynamics 365 Business Edition qualificate a versioni più recenti prima della scadenza.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151526"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Eseguire la migrazione delle offerte di Dynamics 365 Business Edition a versioni più recenti

**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente di amministrazione | Agente di vendita

A partire dal 1° gennaio 2019, i clienti con sottoscrizioni a Dynamics 365 Business Edition non possono più rinnovare queste offerte legacy; Le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione verrà modificato in "Scadenza [data]" da "Rinnovo automatico il [data]".

Per garantire la continuità per i clienti, è consigliabile eseguire la transizione di quelli con sottoscrizioni in scadenza a un'opzione supportata, elencata di seguito. È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.

Se si usa l'API (EITHER o Partner Center), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto renew = False. Le sottoscrizioni in questione verranno impostate su auto renew=False il 1° gennaio 2019. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Le edizioni di Dynamics 365 Business in fase di ritiro

- Dynamics 365 for Finance and Operations, Business edition
- Dynamics 365 for Team Members, Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central : nuove offerte di Dynamics 365 Business Edition

Con le nuove offerte di Dynamics Business Central, i clienti possono connettere i dati finanziari, le vendite, il servizio e le operazioni per semplificare i processi aziendali, migliorare le interazioni dei clienti e prendere decisioni migliori. Dynamics 365 Business Central è basato sul cloud e disponibile solo tramite Cloud Solution Provider partner del programma CSP.)
I clienti di Dynamics 365 Business Edition sono idonei a ricevere prezzi di transizione scontati per le nuove offerte business central fino al 30 giugno 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

 Per spostare i clienti da SKU ritirati a SKU più recenti, è necessario eseguire i passaggi seguenti in questo ordine:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Acquistare il nuovo piano per il cliente

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente da spostare nella nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione.**
3. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.** 

Il cliente avrà ora sia la sottoscrizione precedente che quella nuova. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.
2. Selezionare **Utenti e licenze.**
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi **selezionare Gestisci licenze.** 
4. Nella **pagina** Gestisci licenze deselezionare la casella di controllo Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Piano Dynamics 365 for Sales/Customer Engagement dalla licenza Basic - Offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente. 
5. Selezionare **Submit** (Invia). Questa operazione verrà creata per ogni utente che necessita della nuova licenza. 

Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente. 

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.
2. Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione precedente su **Sospeso e** selezionare **Invia.**

La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva. Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni. Il cliente non incorrerà in costi aggiuntivi per la sottoscrizione precedente.
