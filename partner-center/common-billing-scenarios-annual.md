---
title: 'Fatturazione annuale : scenari comuni'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Partner Center fatturazione annuale: quando si aggiungono nuove sottoscrizioni, si aggiungono licenze prima della data di fatturazione, si modifica la quantità di licenze o si sospende/riattivano le sottoscrizioni.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6392094e000b899e0545655ecf9ed6117535f7f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148704"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Scenari comuni di fatturazione annuale in Partner Center

**Ruoli appropriati:** agente di amministrazione | Amministratore fatturazione | Agente del supporto | Agente di vendita

Questi scenari [di fatturazione comuni di esempio](common-billing-scenarios.md) sono applicabili se si usa la fatturazione annuale Partner Center.

## <a name="new-annual-subscription"></a>Nuova sottoscrizione annuale

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione annuale. Il file di riconciliazione basato su licenza del 15 gennaio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Aggiungere la licenza dopo la data dell'anniversario della sottoscrizione ma prima della data di fatturazione

Si acquista una nuova sottoscrizione l'11/02/17 con una licenza di $ 211,20/anno. L'anniversario della sottoscrizione viene impostato come l'11 di ogni mese. Il sistema di fatturazione Microsoft crea le righe di fatturazione seguenti:

- Addebito di $211,20 per il periodo 2/11/17 - 10/2/18.

Il 17/2/17 si acquista una seconda licenza. La data di fatturazione è il 14/2/17. Vengono generati una fattura e un file di riconciliazione. Il file di riconciliazione conterrà le righe di fatturazione seguenti:

|Data di inizio addebito  |Data di fine addebito  |Tipo di addebito  |Unit Price |Quantity | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Ripartizione delle tariffe all'acquisto |211.20 |1 | 211.20 |

In occasione dell'anniversario della sottoscrizione, l'11/3/17, il sistema di fatturazione Microsoft crea le righe di fatturazione seguenti per l'aumento delle licenze il 17/12/2:

- Credito di $ 211,20 per il periodo 11/2/17 - 10/2/18.
- $ 0,58 addebito prorate per licenza per una licenza per il periodo 2/11/17 – 2/11/17.
- $ 15,62 addebito prorate per licenza per due licenze per il periodo 2/12/17 – 10/3/2017.
- Addebito prorato di $ 195,00 per licenza per due licenze per il periodo 11/03/2017 – 10/02/2018.

L'11/2/17 si acquista una sottoscrizione. Il 17/2/12 si aggiunge una licenza. La data di fatturazione è il 14/2/17. L'11/2/18 la sottoscrizione viene rinnovata.

La data di fatturazione successiva è il 14/3/17 e vengono generati una fattura e un file di riconciliazione. Il file di riconciliazione conterrà le righe di fatturazione seguenti:

|Data di inizio addebito  |Data di fine addebito  |Tipo di addebito  |Unit Price |Quantity | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Ripartizione dell'istanza del ciclo |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Ripartizione dell'istanza del ciclo |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Ripartizione dell'istanza del ciclo |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Ripartizione dell'istanza del ciclo |195.00 |2 |390.00 |

Il 11/2/18 l'abbonamento viene rinnovato per un altro periodo di 12 mesi.

## <a name="change-license-quantity"></a>Cambia la quantità di licenze

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione annuale. Il file di riconciliazione basato su licenza del 15 gennaio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48.00|1|48.00

Il 1° febbraio si aumenta la quantità di licenze da uno a due. Il file di riconciliazione basato su licenza del 15 febbraio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione dell'istanza del ciclo|-48.00|1|-48.00
1/13/2018|31/1/2018|Ripartizione dell'istanza del ciclo|2.47|1|2.47
2/1/2018|1/12/2019|Ripartizione dell'istanza del ciclo|44.98|2|89.96

Il prezzo annuale è 48,00, che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Il periodo di servizio 13/13/2018 - 31/1/2018 è di 19 giorni.

Pertanto, prezzo unitario = 2,47 (19x0,13x1)

Il periodo di servizio è di 346 giorni dal 1/2/2018 al 12/1/12/2019.

Pertanto, prezzo unitario = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione annuale. Il file di riconciliazione basato su licenza del 15 gennaio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48.00|1|48.00

Il 1° febbraio si sospende la sottoscrizione. Il file di riconciliazione basato su licenza del 15 febbraio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Commissione di annullamento|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Sospendere dopo 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione annuale. Il file di riconciliazione basato su licenza del 15 gennaio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48.00|1|48.00

Il file di riconciliazione basato su licenza del 15 febbraio non conterrà alcuna riga di fatturazione per questa sottoscrizione.
Il 1° marzo si sospende la sottoscrizione. Il file di riconciliazione basato su licenza del 15 marzo conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Commissione di annullamento|-41.34|1|-41.34

Il prezzo annuale è 48,00, che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Il periodo di servizio 3/1/2018 - 12/01/2019 è di 318 giorni.

Pertanto, prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito, il prezzo unitario è -41,34.

## <a name="suspend-and-reactivate"></a>Sospendere e riattivare

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione annuale. Il file di riconciliazione basato su licenza del 15 gennaio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48.00|1|48.00

Il 1° febbraio si sospende la sottoscrizione. Il file di riconciliazione basato su licenza del 15 febbraio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Commissione di annullamento|-48.00|1|-48.00

Il 1° marzo si riattiva la sottoscrizione. Il file di riconciliazione basato su licenza del 15 marzo conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|41.34|1|41.34

Il prezzo annuale è 48,00, che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono disponibili 318 giorni nel periodo di servizio 01/03/2018 - 12/01/2019.

Pertanto, prezzo unitario = 41,34 (318x0,13x1).
