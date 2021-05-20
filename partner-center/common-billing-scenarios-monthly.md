---
title: Scenari comuni di fatturazione mensile
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Scenari comuni in Partner Center quando si usa la fatturazione mensile: include l'aggiunta di nuove sottoscrizioni, la modifica della quantità di licenze e la sospensione delle sottoscrizioni."
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148653"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Scenari di fatturazione mensile di esempio per nuove sottoscrizioni, modifica degli importi delle licenze o sospensioni

**Ruoli appropriati:** agente di amministrazione | Amministratore fatturazione | Agente del supporto | Agente di vendita

Questi scenari [di fatturazione comuni di esempio](common-billing-scenarios.md) sono applicabili se si usa la fatturazione mensile in Partner Center.

## <a name="new-monthly-subscription"></a>Nuova sottoscrizione mensile

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione mensile. Il file di riconciliazione basato su licenza del 15 gennaio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00 |

Il file di riconciliazione basato su licenza del 15 febbraio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Tariffa periodica   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Cambia la quantità di licenze

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione mensile. Il file di riconciliazione basato su licenza del 15 gennaio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1° febbraio si aumenta la quantità di licenze da uno a due. Il file di riconciliazione basato su licenza del 15 febbraio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Ripartizione dell'istanza del ciclo   |-4.00       |1        |-4.00   |
|1/13/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2.45       |1        |2.45    |
|2/1/2018         |12/2/2018    | Ripartizione dell'istanza del ciclo   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    |

Il prezzo mensile è 4,00 e sono presenti 31 giorni nel periodo di servizio 13/01/2018 - 12/02/2018. Ciò equivale a un prezzo giornaliero di 0,129 (4/31).

Il periodo di prorazione 13/13/2018 - 31/1/2018 è di 19 giorni.

Prezzo unitario di prorazione = 2,451 = 19 x 0,129

Sono disponibili 12 giorni nel periodo di prorazione 2/1/2018 - 12/02/2018.

Prezzo unitario di prorazione = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Sospendi prima di 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione mensile. Il file di riconciliazione basato su licenza del 15 gennaio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    |

Il 1° febbraio viene sospesa una sottoscrizione. Il file di riconciliazione basato su licenza del 15 febbraio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Commissione di annullamento|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Sospendi dopo 30 giorni

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio si acquista una nuova sottoscrizione con una licenza per $ 4 al mese e si seleziona la fatturazione mensile. Il file di riconciliazione basato su licenza del 15 gennaio conterrà le righe di fatturazione seguenti:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Tariffa ciclo|4,00|1|4,00

Il file di riconciliazione basato su licenza del 15 febbraio conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Tariffa ciclo|4,00|1|4,00

Il 1° marzo si sospende la sottoscrizione. Il file di riconciliazione basato su licenza del 15 marzo conterrà la riga di fatturazione seguente:

|Data di inizio addebito |Data di fine addebito |Tipo di addebito |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Commissione di annullamento|-1.72|1|-1.72

Il prezzo mensile è 4,00 e sono presenti 28 giorni nel periodo di servizio 13/02/2018 - 12/03/2018. Ciò equivale a un prezzo giornaliero di 0,143 (4/28).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 12 giorni nel periodo di annullamento 01/03/2018 - 12/03/2018.

Pertanto, il prezzo unitario = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Passaggi successivi

- [Scenari di fatturazione per acquisti una sola volta e selezione di acquisti ricorrenti](common-billing-scenarios-onetime-recurring.md)