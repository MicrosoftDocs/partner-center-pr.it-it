---
title: Scenari comuni di fatturazione mensile
ms.topic: article
ms.date: 05/13/2020
description: "Scenari comuni nel centro per i partner quando si usa la fatturazione mensile: include l'aggiunta di nuove sottoscrizioni, la modifica della quantità di licenze e la sospensione delle sottoscrizioni."
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 616f706ddb4613f927e0c2830dd794fa3db3944e
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435400"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Scenari di fatturazione mensile di esempio per nuove sottoscrizioni, modifica degli importi di licenze o sospensioni

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di supporto tecnico
- Agente di vendita

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili se si usa la fatturazione mensile nel centro per i partner.

## <a name="new-monthly-subscription"></a>Nuova sottoscrizione mensile

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione mensile. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00 |

Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Tariffa periodica   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Cambia la quantità di licenze

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione mensile. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1 ° febbraio si aumenta la quantità di licenze da uno a due. Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Ripartizione dell'istanza del ciclo   |-4,00       |1        |-4,00   |
|1/13/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2.45       |1        |2.45    |
|2/1/2018         |12/2/2018    | Ripartizione dell'istanza del ciclo   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    |

Il prezzo mensile è 4,00 e sono presenti 31 giorni nel periodo di servizio 1/13/2018 – 2/12/2018. Questo equivale a un prezzo giornaliero di 0,129 (4/31).

Sono presenti 19 giorni nel periodo Proratio 1/13/2018 – 1/31/2018.

Prezzo unitario proporzionale = 2,451 = 19 x 0,129

Sono presenti 12 giorni nel periodo Proratio 2/1/2018 – 2/12/2018.

Prezzo unitario proporzionale = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione mensile. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1 ° febbraio viene sospesa una sottoscrizione. Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Commissione di annullamento|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Sospendi dopo 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $4 al mese e si seleziona la fatturazione mensile. Il 15 gennaio il file di riconciliazione basato sulle licenze conterrà le seguenti righe di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Tariffa del ciclo|4,00|1|4,00

Il 15 febbraio il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Tariffa del ciclo|4,00|1|4,00

Il 1 ° marzo viene sospesa la sottoscrizione. Il 15 marzo il file di riconciliazione basato sulle licenze conterrà la seguente riga di fatturazione:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantità |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Commissione di annullamento|-1,72|1|-1,72

Il prezzo mensile è 4,00 e sono presenti 28 giorni nel periodo di servizio 2/13/2018 – 3/12/2018. Questo equivale a un prezzo giornaliero di 0,143 (4/28).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 12 giorni nel periodo di annullamento 3/1/2018 – 3/12/2018.

Pertanto, il prezzo unitario =-1,716 (12 x 0,143 x (-1)).
