---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389619"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00 |

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tariffa periodica   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Change license quantity

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/1/2018        |12/2/2018    |Ripartizione dell'istanza del ciclo   |-4,00       |1        |-4,00   |
|13/1/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2,45       |1        |2,45    |
|1/2/2018         |12/2/2018    | Ripartizione dell'istanza del ciclo   |1,55       |2        |3,10    |
|13/2/2018         |12/3/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    |

Il prezzo mensile è di 4,00 e sono presenti 31 giorni nel periodo del servizio 13/1/2018-12/2/2018. Ciò equivale a un prezzo giornaliero di 0,129 (31/4).

Ci sono 19 giorni nel periodo di ripartizione proporzionale 13/1/2018 – 31/1/2018.

Prezzo unitario ripartito = 2,451 = 19 x 0,129

Ci sono 12 giorni nel periodo di ripartizione proporzionale 1/2/2018 – 12/2/2018.

Prezzo unitario ripartito = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

On February 1 you suspend a subscription. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Commissione di annullamento|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Tariffa periodica|4,00|1|4,00

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/2/2018|12/3/2018|Tariffa periodica|4,00|1|4,00

Il 1° marzo sospendi la sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/3/2018|Commissione di annullamento|-1,72|1|-1,72

Il prezzo mensile è di 4,00 e sono presenti 28 giorni nel periodo del servizio 13/2/2018-12/3/2018. Ciò equivale a un prezzo giornaliero di 0,143 (28/4).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Il periodo di annullamento ha una durata di 12 giorni 1/3/2018 - 12/3/2018.

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).
