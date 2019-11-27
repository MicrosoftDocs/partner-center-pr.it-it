---
title: Scenari di fatturazione mensili comuni | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Scenari comuni nel centro per i partner quando si usa la fatturazione mensile, ad esempio l'aggiunta di nuove sottoscrizioni, la modifica della quantità di licenze e la sospensione delle sottoscrizioni.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: fatturazione, pagamenti, ordini, utilizzo, fatturazione mensile, sottoscrizioni, file di riconciliazione
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389619"
---
# <a name="monthly-billing-scenarios"></a>Scenari di fatturazione mensili

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili se si usa la fatturazione mensile nel centro per i partner.

## <a name="new-monthly-subscription"></a>Nuova sottoscrizione mensile

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00 |

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tariffa periodica   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Modificare la quantità di licenze

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

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1 ° febbraio viene sospesa una sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Commissione di annullamento|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Sospendi dopo 30 giorni

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

Pertanto, il prezzo unitario =-1,716 (12 x 0,143 x (-1)).
