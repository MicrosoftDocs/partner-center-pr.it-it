---
title: Fatturazione per una sola volta & acquisti ricorrenti
ms.topic: article
ms.date: 05/05/2020
description: 'Vedere gli esempi di fatturazione per il centro per i partner per una sola volta e selezionare gli acquisti ricorrenti: quando si acquistano sottoscrizioni, aggiungere altre sottoscrizioni, aggiungere o rimuovere postazioni.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 06ecd9463f7b9bcb5d370de8f3cd011973cb3607
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435390"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Scenari di fatturazione per il centro per i partner per una sola volta e selezionare gli acquisti ricorrenti

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di supporto tecnico
- Agente di vendita

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio si applicano a [una sola volta e selezionano costi ricorrenti](one-time-and-recurring-billing.md) nel centro per i partner.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Acquistare una sottoscrizione e aggiungere una postazione nello stesso giorno

Nello scenario 1 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno acquisti un'altra sottoscrizione dello stesso tipo allo stesso prezzo.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 4 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -4,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 11 giugno. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 1 = 4,00.
- Nuova fattura di $ 8,00 ripartita proporzionalmente per periodo di servizio 10 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 30 x 2 = 8,00.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |1                 |$ 4            |Nuovo         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -4       |addQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Acquistare una sottoscrizione e aggiungere altre sottoscrizioni in un secondo momento

Nello scenario 2 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4 e acquisti un'altra sottoscrizione il 12 giugno per lo stesso prodotto allo stesso prezzo.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 4 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -3,87 ripartita proporzionalmente per periodo di servizio 11 giugno - 12 giugno. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 1 = 3,87.
- Nuova fattura di $ 7,74 ripartita proporzionalmente per periodo di servizio 12 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 29 x 2 = 7,74.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (una licenza)     |10/6/2019   |9/7/2019         |$ 4         |1        |$ 4            |Nuovo         |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -3,87       |addQuantity           |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Acquistare una sottoscrizione e rimuovere una postazione nello stesso giorno

Nello scenario 3 acquisti due sottoscrizioni per lo stesso prodotto l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno rimuovi una delle postazioni.  

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 8 per due licenze per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -8,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 11 giugno. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 2 = 8,00.
- Nuova fattura di $ 4,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 30 x 1 = 4,00.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |2                 |$ 8            |Nuovo         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | -$ 8       |removeQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Acquistare una sottoscrizione e rimuovere le postazioni in un secondo momento

Nello scenario 4 acquisti due sottoscrizioni l'11 giugno a un prezzo unitario di $ 4 e rimuovi una delle postazioni il 12 giugno.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 8 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -7,74 ripartita proporzionalmente per periodo di servizio 11 giugno - 12 giugno. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 2 = 7,74.
- Nuova fattura di $ 3,87 ripartita proporzionalmente per periodo di servizio 12 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 29 x 1 = 3,87.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Amount** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (due licenze)     |10/6/2019   |9/7/2019         |$ 4         |2        |$ 8       |Nuovo       |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -7,74       |removeQuantity           |
|12/6/2019 (una licenza)    | 10/6/2019    |9/7/2019   |$ 4    |1      |$ 3,87    |removeQuantity |
