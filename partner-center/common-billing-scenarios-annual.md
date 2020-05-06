---
title: Scenari di fatturazione comuni | Centro per i partner
ms.topic: article
ms.date: 11/25/2019
description: 'Vedere fatturazione annuale del centro partner: quando si aggiungono nuove sottoscrizioni, aggiungere le licenze prima della data di fatturazione, modificare la quantità di licenze, sospendere/riattivare le sottoscrizioni.'
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: fatturazione, pagamenti, ordini, utilizzo, fatturazione basata su licenza, data anniversario, termine, annullamento, rinnovo, formula prezzo, file di riconciliazione, file di ricognizione
ms.localizationpriority: medium
ms.openlocfilehash: cbe34dd96c1b119293b73f9324e50340aafb4032
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798549"
---
# <a name="annual-billing-scenarios"></a>Scenari di fatturazione annuali

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di supporto tecnico
- Agente di vendita

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili se si usa la fatturazione annuale nel centro per i partner.

## <a name="new-annual-subscription"></a>Nuova sottoscrizione annuale

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione annuale. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Aggiungi licenza dopo la data di anniversario della sottoscrizione ma prima della data di fatturazione

Si acquista una nuova sottoscrizione il 2/11/17 con una licenza per $211.20/year. L'anniversario della sottoscrizione è impostato come undicesimo di ogni mese. Microsoft Billing System crea le seguenti righe di fatturazione:

- Addebito di $211,20 per il periodo 2/11/17 - 10/2/18.

Il 2/12/17 Acquista una seconda licenza. La data di fatturazione è 2/14/17. Vengono generati una fattura e un file di riconciliazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione:

|Data di inizio addebito  |Data di fine addebito  |Tipo di addebito  |Unit Price |Quantità | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Ripartizione delle tariffe all'acquisto |211,20 |1 | 211,20 |

Nell'anniversario della sottoscrizione 3/11/17, il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione per l'aumento della licenza su 2/12/17:

- $211,20 credito per il periodo 2/11/17 – 2/10/18.
- $0,58 addebitato in modo prorate per licenza per 1 licenza per il periodo 2/11/17 – 2/11/17.
- $15,62 addebitato in modo prorate per licenza per 2 licenze per il periodo 2/12/17-3/10/2017.
- $195,00 addebitato in modo prorate per licenza per 2 licenze per il periodo 3/11/2017-2/10/2018.

Il 2/11/17 Acquista una sottoscrizione. Il 2/12/17 aggiunge una licenza. La data di fatturazione è 2/14/17. Il 2/11/18 di rinnovo della sottoscrizione.

La data di fatturazione successiva è 3/14/17 e viene generata una fattura & file di riconciliazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione:

|Data di inizio addebito  |Data di fine addebito  |Tipo di addebito  |Unit Price |Quantità | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Ripartizione dell'istanza del ciclo |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Ripartizione dell'istanza del ciclo |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Ripartizione dell'istanza del ciclo |15,62 |2 |31,25 |
|3/11/2017 |2/10/2018 |Ripartizione dell'istanza del ciclo |195,00 |2 |390,00 |

Il 2/11/18 la sottoscrizione viene rinnovata per un altro periodo di 12 mesi.

## <a name="change-license-quantity"></a>Cambia la quantità di licenze

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione annuale. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1 ° febbraio si aumenta la quantità di licenze da uno a due. Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione dell'istanza del ciclo|-48,00|1|-48,00
1/13/2018|31/1/2018|Ripartizione dell'istanza del ciclo|2.47|1|2.47
2/1/2018|1/12/2019|Ripartizione dell'istanza del ciclo|44,98|2|89,96

Il prezzo annuo è 48,00, che corrisponde al prezzo giornaliero di 0,13 (48.00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 19 giorni nel periodo di servizio 1/13/2018 – 1/31/2018.

Quindi, prezzo unitario = 2,47 (19x 0.13 x1)

Sono presenti 346 giorni nel periodo di servizio 2/1/2018 – 1/12/2019.

Quindi, prezzo unitario = 44,98 (346x 0.13 x2)

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione annuale. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1 ° febbraio viene sospesa la sottoscrizione. Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Commissione di annullamento|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Sospendi dopo 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione annuale. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basato su licenza non conterrà alcuna riga di fatturazione per questa sottoscrizione.
Il 1 ° marzo viene sospesa la sottoscrizione. Il 15 marzo il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Commissione di annullamento|-41,34|1|-41,34

Il prezzo annuo è 48,00, che corrisponde al prezzo giornaliero di 0,13 (48.00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 318 giorni nel periodo di servizio 3/1/2018 – 1/12/2019.

Quindi, prezzo unitario = 41,34 (318x 0.13 x1). Poiché si tratta di un credito il prezzo unitario è-41,34.

## <a name="suspend-and-reactivate"></a>Sospendere e riattivare

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione annuale. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1 ° febbraio viene sospesa la sottoscrizione. Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Commissione di annullamento|-48,00|1|-48,00

Il 1 ° marzo si riattiva la sottoscrizione. Il 15 marzo il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Ripartizione delle tariffe all'acquisto|41,34|1|41,34

Il prezzo annuo è 48,00, che corrisponde al prezzo giornaliero di 0,13 (48.00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 318 giorni nel periodo di servizio 3/1/2018 – 1/12/2019.

Quindi, prezzo unitario = 41,34 (318x 0.13 x1).
