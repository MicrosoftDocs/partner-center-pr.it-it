---
title: Scenari di fatturazione comuni per una sola volta e selezionare gli acquisti ricorrenti | Centro per i partner
ms.topic: article
ms.date: 11/25/2019
description: 'Vedere gli esempi di fatturazione per il centro per i partner per una sola volta e selezionare gli acquisti ricorrenti: quando si acquistano sottoscrizioni, aggiungere altre sottoscrizioni, aggiungere o rimuovere postazioni.'
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: fatturazione, pagamenti, acquisto monouso, acquisto ricorrente, sottoscrizioni, postazioni
ms.localizationpriority: medium
ms.openlocfilehash: 9f1a96bfeee667f998d163416b96c281803f7107
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390120"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>Scenari di fatturazione monouso e selezionati per gli acquisti ricorrenti

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente help desk
- Agente di vendita

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio si applicano a [una sola volta e selezionano costi ricorrenti](one-time-and-recurring-billing.md) nel centro per i partner.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Acquistare una sottoscrizione e aggiungere una postazione nello stesso giorno

Nello scenario 1 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno acquisti un'altra sottoscrizione dello stesso tipo allo stesso prezzo.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 4 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -4,00 ripartita proporzionalmente per periodo di servizio 11 giugno - 11 giugno. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 1 = 4,00.
- Nuova fattura di $ 8,00 ripartita proporzionalmente per periodo di servizio 10 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 30 x 2 = 8,00.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
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

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
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

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |2                 |$ 8            |Nuovo         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -8       |removeQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Acquistare una sottoscrizione e rimuovere le postazioni in un secondo momento

Nello scenario 4 acquisti due sottoscrizioni l'11 giugno a un prezzo unitario di $ 4 e rimuovi una delle postazioni il 12 giugno.

Il file di riconciliazione includerà quanto segue:

- Fattura di $ 8 per periodo di servizio 10 giugno - 9 luglio.
- Nuova fattura di $ -7,74 ripartita proporzionalmente per periodo di servizio 11 giugno - 12 giugno. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 2 = 7,74.
- Nuova fattura di $ 3,87 ripartita proporzionalmente per periodo di servizio 12 giugno - 9 luglio. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 29 x 1 = 3,87.

|**Data di acquisto**   |**Inizio addebito** |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (due licenze)     |10/6/2019   |9/7/2019         |$ 4         |2        |$ 8       |Nuovo       |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -7,74       |removeQuantity           |
|12/6/2019 (una licenza)    | 10/6/2019    |9/7/2019   |$ 4    |1      |$ 3,87    |removeQuantity |
