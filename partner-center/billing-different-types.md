---
title: Informazioni sui tipi di fatturazione nel centro per i Partner | Centro per i partner
ms.topic: article
ms.date: 03/01/2019
Description: Informazioni sui diversi tipi di fatturazione, i periodi di fatturazione e le date di fatturazione
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione e pagamenti, ordini, i file di riconciliazione, file di riconoscimento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 3e664a8a539125bce21d256c6e6d88d1ab22d14d
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343459"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Informazioni sui tipi di fatturazione nel Centro per i partner

**Si applica a**

-  Centro per i partner
-  Partner del programma CSP

A seconda dei tipi di prodotti acquistati per i clienti, potrebbero avere diversi periodi di fatturazione e fatturate in giorni diversi dello stesso mese. Questo articolo illustra le modifiche apportate a partire dal 1 marzo 2019, e come le modifiche possibili conseguenze per te.

## <a name="billing-for-recurring-charges"></a>Fatturazione per addebiti periodici

L'esperienza di fatturazione di addebiti periodici delle sottoscrizioni basate su utilizzo e basati su licenza rimane invariato. Microsoft continuerà a fatturare è il giorno del mese che è stato selezionato come data di fatturazione e il periodo di fatturazione continuerà a essere il mese prima di tale data. Se si seleziona il giorno 15 del mese della data di fatturazione, ti verranno fatturate per tutte le attività dal 15 del mese di calendario al 14 del mese di calendario successivo. Le fatture e i file di riconciliazione sono disponibili a livello generale 2 a 4 giorni, dopo la data di fatturazione.

Come prima, importo verrà addebitato è di questi prodotti nella valuta per il paese/area geografica che in cui ti trovi, indipendentemente dalla posizione del cliente è venduto del prodotto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Fatturazione per una tantum e selezionare addebiti periodici

A partire dal 1 marzo 2019, abbiamo introdotto una nuova esperienza di fatturazione per costi di periodiche e monouso per i prodotti di ISV di terze parti e Microsoft.

Per questi prodotti, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. Si renderà la fattura disponibile su 8 giorni del mese successivo. 

In altre parole, tutte le transazioni che si apportano tra il 1 maggio e il 31 maggio 2019 verranno visualizzati nella fattura giugno 8. Tutte le transazioni che si apportano tra il 1 giugno e il 30 giugno 2019 verranno visualizzati nella fattura 8 luglio. Potrebbe essere fatturati per gli acquisti ricorrenti e monouso nella fattura stesso. 

È anche possibile controllare conto saldo/fattura ogni volta che si desidera (ad esempio, tra il 1 maggio e il 7 giugno) e vedere l'ultima attività di account senza dover attendere la fattura. Si noti che quando viene pubblicata la fattura nell'all'8, includerà le imposte e qualsiasi altro applicabili addebiti e i crediti, in modo che la quantità finale potrebbe essere diverso da quello visualizzato durante il periodo di fatturazione. 

È possibile accedere le fatture l'esattamente che come a questo punto, nel centro per i Partner o dall'API. Questi verranno visualizzati prima di mezzanotte UTC del giorno del mese l'8. 

|**Esperienza di fatturazione**|**Tipi di prodotto**|**Data di fatturazione**|**Periodo di fatturazione**|**Valuta di fatturazione**|**Attività corrente disponibile?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Addebiti periodici per le sottoscrizioni basate su utilizzo e basati su licenza |Tutti i prodotti dal [catalogo di servizi online](https://partner.microsoft.com/commerce/preferredoffers/list). Gli esempi includono Office 365, Microsoft 365, Azure Active Directory, Azure (pagamento a consumo), Dynamics 365, Power BI Pro |La data selezionata durante la creazione dell'account del centro per i Partner |Il mese prima della data di fatturazione. |La valuta del paese/area geografica che in cui ti trovi. Ad esempio, se una società con sede nel Regno Unito, importo verrà addebitato è di British sterline (GBP). Se l'azienda si trova in India, importo verrà addebitato si in India rupia indiana (INR).  |No |
|Addebiti ricorrenti e monouso per prodotti Microsoft e terze parti ISV |Tutti i SaaS sottoscrizioni, le prenotazioni di Azure e i prodotti software (permanenti e basati su abbonamento) offerti da Microsoft e ISV di terze parti. Prodotti disponibili in vedere le [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Gli esempi includono il software SUSE Linux (abbonamento di software), Windows Server 2019 Essentials (software perpetuo), sottoscrizione al prodotto Azure ISV SaaS. |8 giorni del mese |Dal primo giorno all'ultimo giorno di ogni mese di calendario |La valuta del paese/regione del cliente si trova. Ciò significa che riceverai fatture separate e i file di riconciliazione nella valuta del paese/regione ogni cliente che è venduto a nel periodo di fatturazione. |Yes |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Scenari di fatturazione degli acquisti relativi a singole e ricorrenti
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scenario 1: acquistare una sottoscrizione e quindi aggiungere una postazione nella stessa giornata

Nello Scenario 1, si acquista una sottoscrizione l'11 giugno al prezzo unitario pari a $4. In un secondo momento nello stesso giorno si acquista un'altra della stessa sottoscrizione allo stesso prezzo. 

Il file di riconoscimento include quanto segue: 
-   fattura $4 per il periodo del servizio 10 giugno – 9 luglio. 
-   $-4.00 rebill con ripartizione proporzionale per il periodo di assistenza all'11 giugno – 11 giugno. Si tratta del periodo quando era 1 licenza. Calcolo = (mensile totale/prezzo giorni nel periodo del servizio) x giorni nel servizio con ripartizione proporzionale periodo x numero di licenze = (4/30) x 30 x 1 = 4.00.
-   $8.00 applicata la ripartizione proporzionale rebill per periodo servizio 10 giugno – 9 luglio. Si tratta del periodo quando era 2 licenze. Calcolo = (4/30) x 30 x 2 = 8.00.

|**Data di acquisto**   |**Costo iniziale**  |**Fine di addebito**  |**Prezzo unitario**  |**Quantity**  |**Quantità** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Nuova         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Scenario 2 – acquistare una sottoscrizione e quindi aggiungerle più avanti

Nello Scenario 2, si acquista una sottoscrizione l'11 giugno al prezzo unitario pari a $4 e a partire dal 12 giugno si acquista un'altra sottoscrizione per lo stesso prodotto allo stesso prezzo. 

Il file di riconoscimento include quanto segue: 
-   fattura $4 per il periodo del servizio 10 giugno – 9 luglio. 
-   $-3.87 rebill con ripartizione proporzionale per il periodo di assistenza all'11 giugno: 12 giugno. Si tratta del periodo quando era 1 licenza. Calcolo = (mensile totale/prezzo giorni nel periodo del servizio) x giorni nel servizio con ripartizione proporzionale periodo x numero di licenze = x (4/30) 29 x 1 = 3.87.
-   $7.74 applicata la ripartizione proporzionale rebill per periodo del servizio dal 12 giugno – 9 luglio. Si tratta del periodo quando era 2 licenze. Calcolo = x (4/30) 29 x 2 = 7.74.

|**Data di acquisto**   |**Costo iniziale**  |**Fine di addebito**  |**Prezzo unitario**  |**Quantity**  |**Quantità** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (con una licenza)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nuova         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3.87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7.74       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scenario 3: acquistare una sottoscrizione, quindi rimuovere una postazione nella stessa giornata

Nello Scenario 3, acquistare due sottoscrizioni per lo stesso prodotto l'11 giugno al prezzo unitario pari a $4. In un secondo momento nello stesso giorno si rimuovere uno le postazioni.  

Il file di riconoscimento include quanto segue: 
-   fattura a 8 dollari per due licenze per il 10 giugno – 9 luglio periodo del servizio. 
-   $-8.00 rebill con ripartizione proporzionale per il periodo di assistenza all'11 giugno – 11 giugno. Si tratta del periodo quando era 2 licenze. Calcolo = (mensile totale/prezzo giorni nel periodo del servizio) x giorni nel servizio con ripartizione proporzionale periodo x numero di licenze = (4/30) x 30 x 2 = 8.00.
-   $4.00 applicata la ripartizione proporzionale rebill per periodo servizio all'11 giugno – 9 luglio. Si tratta del periodo quando era 1 licenza. Calcolo = (4/30) x 30 x 1 = 4.00.

|**Data di acquisto**   |**Costo iniziale**  |**Fine di addebito**  |**Prezzo unitario**  |**Quantity**  |**Quantità** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nuova         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Scenario 4: acquistare una sottoscrizione, quindi rimuovere postazioni in seguito

Nello Scenario 4 si acquistano 2 sottoscrizioni l'11 giugno al prezzo unitario pari a $4 e a partire dal 12 giugno è rimuovere uno delle postazioni. 

Il file di riconoscimento include quanto segue: 
-   fattura a 8 dollari per il periodo del servizio 10 giugno – 9 luglio. 
-   $-7.74 rebill con ripartizione proporzionale per il periodo di assistenza all'11 giugno: 12 giugno. Si tratta del periodo quando era 2 licenze. Calcolo = (mensile totale/prezzo giorni nel periodo del servizio) x giorni nel servizio con ripartizione proporzionale periodo x numero di licenze = x (4/30) 29 x 2 = 7.74.
-   $3.87 applicata la ripartizione proporzionale rebill per periodo del servizio dal 12 giugno – 9 luglio. Si tratta del periodo quando era 1 licenza. Calcolo = x (4/30) 29 x 1 = 3.87.

|**Data di acquisto**   |**Costo iniziale**  |**Fine di addebito**  |**Prezzo unitario**  |**Quantity**  |**Quantità** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (si dispone di 2 licenze)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Nuova       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7.74       |removeQuantity           |
|6 o 12/2019 (con 1 licenza)    | 6/10/2019    |7/09/2019   |$4    |1      |$3.87    |removeQuantity |
