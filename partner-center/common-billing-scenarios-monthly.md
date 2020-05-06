---
title: Scenari di fatturazione mensili comuni | Centro per i partner
ms.topic: article
ms.date: 11/25/2019
description: Scenari comuni nel centro per i partner quando si usa la fatturazione mensile, ad esempio l'aggiunta di nuove sottoscrizioni, la modifica della quantità di licenze e la sospensione delle sottoscrizioni.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: fatturazione, pagamenti, ordini, utilizzo, fatturazione mensile, sottoscrizioni, file di riconciliazione
ms.localizationpriority: medium
ms.openlocfilehash: e67281a0bf7d5649a68a6a3f3c27c40e3666eb14
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798539"
---
# <a name="monthly-billing-scenarios"></a>Scenari di fatturazione mensili

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
