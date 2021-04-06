---
title: Fatturazione per una sola volta & acquisti ricorrenti
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Esempi di fatturazione del centro per i partner per una sola volta e selezionare gli acquisti ricorrenti: quando si acquistano sottoscrizioni, aggiungere altre sottoscrizioni, aggiungere o rimuovere licenze.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 329675e10205755819a19710976073d22f73eb58
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502532"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scenari di fatturazione per il centro per i partner per una sola volta e selezionare gli acquisti ricorrenti

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di supporto tecnico
- Agente di vendita

Si tratta di [scenari di fatturazione comuni](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Acquistare una sottoscrizione e aggiungere una licenza nello stesso giorno

Nello scenario 1 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno acquisti un'altra sottoscrizione dello stesso tipo allo stesso prezzo.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 4 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -4,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 11 giugno. Questo è il periodo in cui si dispone di una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 1 = 4,00.
- Nuova fattura di $ 8,00 ripartita proporzionalmente per periodo di servizio 10 giugno - 9 luglio. Questo è il periodo in cui erano disponibili due licenze. Calcolo = (4/30) x 30 x 2 = 8,00.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |1                 |$ 4            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -4       |addQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Acquistare una sottoscrizione e aggiungere altre sottoscrizioni in un secondo momento

Nello scenario 2 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4 e acquisti un'altra sottoscrizione il 12 giugno per lo stesso prodotto allo stesso prezzo.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 4 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -3,87 ripartita proporzionalmente per periodo di servizio 11 giugno - 12 giugno. Questo è il periodo in cui si disponeva di una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 1 = 3,87.
- Nuova fattura di $ 7,74 ripartita proporzionalmente per periodo di servizio 12 giugno - 9 luglio. Questo è il periodo in cui erano disponibili due licenze. Calcolo = (4/30) x 29 x 2 = 7,74.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (una licenza)     |10/6/2019   |9/7/2019         |$ 4         |1        |$ 4            |Nuova         |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -3,87       |addQuantity           |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Acquistare una sottoscrizione e rimuovere una licenza nello stesso giorno

Nello scenario 3 acquisti due sottoscrizioni per lo stesso prodotto l'11 giugno a un prezzo unitario di $ 4. Successivamente, viene rimossa una delle licenze.  

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 8 per due licenze per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -8,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 11 giugno. Questo è il periodo in cui erano disponibili due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 2 = 8,00.
- Nuova fattura di $ 4,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 9 luglio. Questo è il periodo in cui si disponeva di una licenza. Calcolo = (4/30) x 30 x 1 = 4,00.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |2                 |$ 8            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | -$ 8       |removeQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Acquistare una sottoscrizione e rimuovere le licenze in un secondo momento

Nello scenario 4 si acquistano due sottoscrizioni l'11 giugno a un prezzo unitario di $4 e il 12 giugno si rimuove una delle licenze.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 8 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -7,74 ripartita proporzionalmente per periodo di servizio 11 giugno - 12 giugno. Questo è il periodo in cui erano disponibili due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 2 = 7,74.
- Nuova fattura di $ 3,87 ripartita proporzionalmente per periodo di servizio 12 giugno - 9 luglio. Questo è il periodo in cui si disponeva di una licenza. Calcolo = (4/30) x 29 x 1 = 3,87.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (sono disponibili due licenze)     |10/6/2019   |9/7/2019         |$ 4         |2        |$ 8       |Nuova       |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -7,74       |removeQuantity           |
|6/12/2019 (si dispone di una licenza)    | 10/6/2019    |9/7/2019   |$ 4    |1      |$ 3,87    |removeQuantity |

## <a name="next-steps"></a>Passaggi successivi

- [Scenari di fatturazione mensile di esempio per nuove sottoscrizioni, modifica degli importi di licenze o sospensioni](common-billing-scenarios-monthly.md)