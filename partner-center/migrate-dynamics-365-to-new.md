---
title: Eseguire la migrazione edizione di Dynamics 365 Business offre alle versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Le sottoscrizioni di Dynamics 365 edizione Business non è più possono essere rinnovate.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968284"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Eseguire la migrazione edizione di Dynamics 365 Business offre alle versioni più recenti 

**Si applica a**

- Centro per i partner

Effettivi 1 gennaio 2019, i clienti con sottoscrizioni Dynamics 365 Business Edition non è più possono rinnovare in queste offerte legacy; le sottoscrizioni esistenti non verranno rinnovati automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà a "Data di scadenza [Data]" da "Rinnovo automatico il [Data]".

Per garantire la continuità, è opportuno trasferire quelli con sottoscrizioni in scadenza a delle opzioni supportate elencati di seguito. Ti consigliamo di far sottoscrivere ai clienti nuove sottoscrizioni prima della data di scadenza annuale della sottoscrizione, al fine di evitare eventuali interruzioni del servizio.

Se si utilizza l'API (CREST o centro per i Partner), puoi trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme automatico = False proprietà. Le sottoscrizioni in questione verranno impostate su auto renew = False il 1 gennaio 2019. Puoi trasferire i clienti a un nuovo piano in qualsiasi momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Le edizioni Business di Dynamics 365 viene ritirato

- Dynamics 365 per Finance and Operations, edizione Business
- Dynamics 365 for Team Members, edizione Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business centrale - le nuove offerte Dynamics 365 Business Edition

Con le nuove offerte Dynamics Business centrale, i clienti possono connettere i loro dati finanziari, vendite, servizio e le operazioni per semplificare i processi aziendali, migliorare interazioni con i clienti e prendere le decisioni migliori. Dynamics 365 Business centrale è disponibile tramite solo partner del programma Cloud Solution Provider (CSP) e basati sul cloud.
Dynamics 365 clienti edizione Business sono idonei alla ricezione transizione scontate prezzi per il nuovo centrale di Business offre fino al 30 giugno 2020.

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

 Spostare i clienti da SKU ritirati a quelli più recenti richiede la procedura seguente in questo ordine:

- Acquistare il nuovo abbonamento
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Il nuovo piano di acquisto per il cliente

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente da trasferire alla nuova sottoscrizione.
2. Seleziona **Aggiungi sottoscrizione**.
3. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**. 

Il cliente verrà ora avere sia la sottoscrizione precedente e quello nuovo. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.
2. Seleziona **Utenti e licenze**.
3. Per riassegnare una licenza a un utente, seleziona l'utente e quindi seleziona **Gestisci licenze**. 
4. Nella pagina **Gestisci licenze** , cancellare il Dynamics 365 for Sales / piano di coinvolgimento dei clienti da Basic (offrire qualificati) casella di controllo della licenza e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente. 
5. Seleziona **Invia**. Lo farai per ogni utente che richiede la nuova licenza. 

Dopo avere spostato le licenze alla nuova sottoscrizione puoi annullare la sottoscrizione precedente. 

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.
2. Nella pagina dei dettagli della sottoscrizione imposta la sottoscrizione precedente in **sospeso** e seleziona **Invia**.

La sottoscrizione precedente viene ora sospesa e la nuova sottoscrizione diventa attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non incorrere costi aggiuntivi necessari per la sottoscrizione precedente.