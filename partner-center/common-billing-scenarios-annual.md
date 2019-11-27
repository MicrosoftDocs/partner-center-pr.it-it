---
title: Scenari di fatturazione comuni | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Scenari di fatturazione comuni nel centro partner per la fatturazione annuale, ad esempio l'aggiunta di nuove sottoscrizioni, l'aggiunta di licenze prima della data di fatturazione, la modifica della quantità di licenze e la sospensione e riattivazione delle sottoscrizioni.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: fatturazione, pagamenti, ordini, utilizzo, fatturazione basata su licenza, data anniversario, termine, annullamento, rinnovo, formula prezzo, file di riconciliazione, file di ricognizione
ms.localizationpriority: medium
ms.openlocfilehash: 91b8e318e2122f9510b160339984cc0743c318ee
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389629"
---
# <a name="annual-billing-scenarios"></a>Scenari di fatturazione annuali

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili se si usa la fatturazione annuale nel centro per i partner.

## <a name="new-annual-subscription"></a>Nuova sottoscrizione annuale

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Aggiungi licenza dopo la data di anniversario della sottoscrizione ma prima della data di fatturazione

Viene acquistata una nuova sottoscrizione il 11/2/17 con una licenza per $211,20/anno. L'anniversario della sottoscrizione è impostato sull'11 di ogni mese. Il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione:

- Addebito di $211,20 per il periodo 2/11/17 - 10/2/18.

Il 12/2/17 è stata acquistata una seconda licenza. La data di fatturazione è 14/2/17. Vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione:

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione delle tariffe all'acquisto |211,20 |1 | 211,20 |

Nell'anniversario della tua sottoscrizione, 11/3/17, il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione per l'aumento della licenza del 12/2/17:

- $211,20 credito per il periodo 2/11/17 – 2/10/18.
- Addebito di $0,58 ripartito per licenza per 1 licenza per il periodo 11/2/17 - 11/2/17.
- Addebito di $15,62 ripartito per licenza per 2 licenze per il periodo 12/2/17 - 10/3/2017.
- Addebito di $195,00 ripartito per licenza per 2 licenze per il periodo 11/3/2017 - 10/2/2018.

Il 11/2/17 è stata acquistata una sottoscrizione. Il 12/2/17 è stata aggiunta una licenza. La data di fatturazione è 14/2/17. Il 11/2/18 viene rinnovata la sottoscrizione.

La prossima data di fatturazione è il 14/3/17 e vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione:

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |-211,20 |1 |-211,20 |
|11/2/2017 |11/2/2017 |Ripartizione dell'istanza del ciclo |0,58 |1 |0,58 |
|12/2/2017 |10/3/2017 |Ripartizione dell'istanza del ciclo |15,62 |2 |31,25 |
|11/3/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |195,00 |2 |390,00 |

Il 11/2/18 la sottoscrizione viene rinnovata per un altro periodo di 12 mesi.

## <a name="change-license-quantity"></a>Modificare la quantità di licenze

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione dell'istanza del ciclo|-48,00|1|-48,00
13/1/2018|31/1/2018|Ripartizione dell'istanza del ciclo|2,47|1|2,47
1/2/2018|12/1/2019|Ripartizione dell'istanza del ciclo|44,98|2|89,96

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 19 giorni nel periodo di servizio 13/1/2018 – 31/1/2018.

Di conseguenza, il prezzo unitario = 2,47 (19x0,13x1)

Ci sono 346 giorni nel periodo di servizio 1/2/2018 – 12/1/2019.

Di conseguenza, il prezzo unitario = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Sospendi dopo 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basata su licenza non conterrà righe di fatturazione per questa sottoscrizione.
Il 1° marzo sospendi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Commissione di annullamento|-41,34|1|-41,34

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019.

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito il prezzo unitario è -41,34.

## <a name="suspend-and-reactivate"></a>Sospendere e riattivare

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

Il 1° marzo riattivi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|41,34|1|41,34

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019.

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1).
