---
title: Eseguire la migrazione sono disponibili di Dynamics 365 Business Edition alle versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Le sottoscrizioni di Dynamics 365 Business Edition non possono essere rinnovate.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offre, rinnovare le offerte, nuovi SKU di Dynamics 365
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134371"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Eseguire la migrazione edizione di Dynamics 365 Business offre alle versioni più recenti 

**Si applica a**

- Centro per i partner

Efficace 1 gennaio 2019, i clienti con sottoscrizioni di Dynamics 365 Business Edition non è più possono rinnovare in queste offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà per "Expires su [date]" da "Rinnova automaticamente in [date]".

Per garantire continuità aziendale per i clienti, è necessario eseguire la transizione quelli con le sottoscrizioni in scadenza un'opzione supportata, elencati di seguito. Si consiglia di far passare i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento, al fine di evitare eventuali interruzioni del servizio.

Se si usa l'API (CREST o centro per i Partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione con l'automobile vengono rinnovate = False proprietà. Le sottoscrizioni in questione verranno impostate su auto rinnovare = False su 1 gennaio 2019. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Le edizioni Business di Dynamics 365 in fase di ritiro

- Dynamics 365 per Finanza e operazioni, Business edition
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Centrali aziendali di Dynamics - le nuove offerte di Dynamics 365 Business Edition

Con le nuove offerte di Dynamics Business Central, i clienti possono connettere i dati finanziari, vendite, servizio e operazioni per semplificare i processi aziendali, migliorare le interazioni di customer e prendere decisioni più informate. Dynamics 365 Business Central è disponibile tramite solo i partner programma Cloud Solution Provider (CSP) e basato sul cloud.
Dynamics 365 clienti Business Edition sono idonei a ricevere transizione sconti sui prezzi per il nuovo Business Central offre fino al 30 giugno 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

 I clienti lo spostamento dal ritirati SKU quelli più recenti richiede i passaggi seguenti nell'ordine indicato:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Il nuovo piano di acquisto per il cliente

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente che si desidera spostare la nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione**.
3. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**. 

Il cliente avrà la sottoscrizione precedente sia quello nuovo. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.
2. Seleziona **Utenti e licenze**.
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **gestire le licenze**. 
4. Nel **gestire le licenze** pagina, cancellare il di Dynamics 365 for Sales / piano di Engagement dei clienti da Basic (completi dell'offerta) casella di controllo di licenza e selezionare un nuovo piano di servizio per la sottoscrizione cliente stia passando ad. 
5. Seleziona **Invia**. Si eseguirà questa operazione per ogni utente che necessita la nuova licenza. 

Dopo aver spostato le licenze alla nuova sottoscrizione è possibile annullare la sottoscrizione precedente. 

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.
2. Nella pagina di dettagli della sottoscrizione, impostare la sottoscrizione precedente **degli elementi sospesi** e selezionare **Submit**.

La sottoscrizione precedente a questo punto viene sospeso e la nuova sottoscrizione è attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non incorrerà costi aggiuntivi per la sottoscrizione precedente.