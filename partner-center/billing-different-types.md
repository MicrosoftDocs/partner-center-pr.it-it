---
title: Informazioni sui tipi di fatturazione nel Centro per i partner | Centro per i partner
ms.topic: article
ms.date: 10/04/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni sui diversi tipi di fatturazione, sui periodi di fatturazione e sulle date di fatturazione
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione, pagamenti, ordini, file di riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b5991e5134d56684fb1ef43db5785d904fc9c15a
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653742"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Informazioni sui tipi di fatturazione nel Centro per i partner

**Si applica a**

-  Centro per i partner
-  Partner aderenti al programma CSP

A seconda dei tipi di prodotti acquistati per i clienti, potresti avere periodi di fatturazione diversi e addebiti in giorni diversi dello stesso mese. Questo articolo illustra le modifiche apportate a partire dal 1° marzo 2019 e gli effetti prodotti da tali modifiche.

## <a name="billing-for-recurring-charges"></a>Fatturazione per addebiti periodici

L'esperienza di fatturazione per gli addebiti periodici delle sottoscrizioni basate su licenza e sull'utilizzo non cambia. Si continuerà a fatturare il giorno del mese selezionato come data di fatturazione e il periodo di fatturazione continuerà a essere il mese precedente a tale data. Se è stato selezionato il quindicesimo giorno del mese per la data di fatturazione, verranno addebitate tutte le attività dal 15 ° di un mese di calendario al 14 del mese di calendario successivo. Le fatture e i file di riconciliazione sono disponibili in genere 2-4 giorni dopo la data di fatturazione.

Come prima, verranno addebitati i prodotti nella valuta per il paese/area geografica in cui si trovano, indipendentemente dalla posizione del cliente a cui si è venduto il prodotto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Fatturazione per addebiti occasionali e periodici

A partire dal 1° marzo 2019, è stata introdotta una nuova esperienza di fatturazione per gli addebiti occasionali e periodici per i prodotti ISV Microsoft e di terze parti.

Per questi prodotti, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. La fattura sarà disponibile l'ottavo giorno del mese successivo. 

In altre parole, le transazioni effettuate tra il 1° e il 31 maggio 2019 saranno incluse nella fattura dell'8 giugno. Tutte le transazioni effettuate tra il 1° e il 30 giugno 2019 saranno incluse nella fattura dell'8 luglio. È possibile che nella stessa fattura vengano addebitati gli acquisti ricorrenti e occasionali. 

Puoi anche controllare il saldo o la fattura dell'account ogni volta che lo desideri, ad esempio tra il 1° maggio e il 7 giugno, e verificare le ultime attività dell'account senza dover attendere la fattura. Tieni presente che quando l'8 del mese viene pubblicata la fattura, verranno inclusi le imposte e altri eventuali addebiti e crediti applicabili, pertanto l'importo finale potrebbe variare rispetto a quanto visualizzato durante il periodo di fatturazione. 

Potrai accedere alle tue fatture nello stesso modo che fai adesso, in centro per i partner o tramite API. Verranno visualizzati prima della mezzanotte UTC dell'ottavo giorno del mese. 

|**Esperienza di fatturazione**|**Tipi di prodotto**|**Data di fatturazione**|**Periodo di fatturazione**|**Valuta di fatturazione**|**Disponibilità attività corrente**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Addebiti periodici per le sottoscrizioni basate su licenza e sull'utilizzo |Tutti i prodotti del [catalogo dei servizi online](https://partner.microsoft.com/commerce/preferredoffers/list). Gli esempi includono Office 365, Microsoft 365, Azure Active Directory, Azure (con pagamento in base al consumo), Dynamics 365, Power bi Pro |Data selezionata al momento della creazione dell'account del Centro per i partner |Mese che precede la data di fatturazione. |Valuta del paese in cui si trova l'area geografica. Se, ad esempio, la società si trova nel Regno Unito, la fatturazione verrà fatturata in sterline britanniche (GBP). Se la società si trova in India, verrà fatturata in India rupie (INR).  |No |
|Addebiti periodici e occasionali per prodotti ISV Microsoft e di terze parti |Tutte le sottoscrizioni SaaS, le prenotazioni di Azure e i prodotti software (perpetui e basati sulle sottoscrizioni) offerti da ISV Microsoft e di terze parti. Vedi i prodotti disponibili nel [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Gli esempi includono il software SUSE Linux (sottoscrizione software), Windows Server 2019 Essentials (software perpetuo) e la sottoscrizione di prodotti SaaS ISV di Azure. |8 di ogni mese |Dal primo all'ultimo giorno di ogni mese di calendario |Valuta del paese o dell'area geografica in cui si trova il tuo cliente. Ciò significa che si riceveranno fatture separate e file di riconciliazione nella valuta del paese/area geografica di ogni cliente venduto nel periodo di fatturazione. |Sì |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Scenari di fatturazione per acquisti occasionali e periodici
### <a name="scenario-1---purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scenario 1: acquistare una sottoscrizione e quindi aggiungere una postazione nello stesso giorno

Nello scenario 1 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno acquisti un'altra sottoscrizione dello stesso tipo allo stesso prezzo. 

Il file di riconciliazione includerà quanto segue: 
-   $4 fattura per il periodo di servizio dal 10 giugno al 9 luglio. 
-   $-4,00 rifatturare rifatturato per il periodo di servizio 11 giugno 11 giugno. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 1 = 4,00.
-   $8,00 rifatturazione rivalutata per il periodo di servizio 10 giugno 9. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 30 x 2 = 8,00.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |1                 |$ 4            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -4       |addQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 8         |addQuantity           |

### <a name="scenario-2---purchase-a-subscription-and-then-add-more-later"></a>Scenario 2: acquistare una sottoscrizione e quindi aggiungerla più tardi

Nello scenario 2 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4 e acquisti un'altra sottoscrizione il 12 giugno per lo stesso prodotto allo stesso prezzo. 

Il file di riconciliazione includerà quanto segue: 
-   $4 fattura per il periodo di servizio dal 10 giugno al 9 luglio. 
-   $-3,87 rifatturazione rivalutata per il periodo di servizio 11 giugno 12 giugno. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 1 = 3,87.
-   $7,74 rifatturazione rivalutata per il periodo di servizio 12 giugno-9 luglio 9. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 29 x 2 = 7,74.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (una licenza)     |10/6/2019   |9/7/2019         |$ 4         |1        |$ 4            |Nuova         |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -3,87       |addQuantity           |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 7,74       |addQuantity           |

### <a name="scenario-3---purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scenario 3: acquistare una sottoscrizione e quindi rimuovere una postazione nello stesso giorno

Nello scenario 3 acquisti due sottoscrizioni per lo stesso prodotto l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno rimuovi una delle postazioni.  

Il file di riconciliazione includerà quanto segue: 
-   $8 fattura per due licenze per il periodo di servizio dal 10 giugno al 9 luglio. 
-   $-8,00 rifatturare rifatturato per il periodo di servizio 11 giugno 11 giugno. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 2 = 8,00.
-   $4,00 rifatturazione rivalutata per il periodo di servizio 11 giugno-9 luglio. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 30 x 1 = 4,00.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |2                 |$ 8            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -8       |removeQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

### <a name="scenario-4---purchase-a-subscription-and-then-remove-seats-later"></a>Scenario 4: acquistare una sottoscrizione e quindi rimuovere le postazioni in un secondo momento

Nello scenario 4 acquisti due sottoscrizioni l'11 giugno a un prezzo unitario di $ 4 e rimuovi una delle postazioni il 12 giugno. 

Il file di riconciliazione includerà quanto segue: 
-   $8 fattura per il periodo di servizio dal 10 giugno al 9 luglio. 
-   $-7,74 rifatturazione rivalutata per il periodo di servizio 11 giugno 12 giugno. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 2 = 7,74.
-   $3,87 rifatturazione rivalutata per il periodo di servizio 12 giugno-9 luglio 9. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 29 x 1 = 3,87.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (due licenze)     |10/6/2019   |9/7/2019         |$ 4         |2        |$ 8       |Nuova       |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -7,74       |removeQuantity           |
|12/6/2019 (una licenza)    | 10/6/2019    |9/7/2019   |$ 4    |1      |$ 3,87    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Scenari di fatturazione per transazioni SaaS basate su licenza per versione di valutazione gratuita
### <a name="scenario-5---renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Scenario 5: rinnovare una sottoscrizione SaaS di valutazione gratuita basata su licenza a una sottoscrizione a pagamento al termine del periodo di valutazione gratuita

In questo scenario acquisti una sottoscrizione SaaS (software come un servizio) di una versione di valutazione gratuita basata su licenza il 10 giugno che si rinnova automaticamente come sottoscrizione a pagamento al termine del periodo di valutazione gratuita. 

I file di riconciliazione includeranno quanto segue: 
- $0 fattura per il periodo di servizio 10 giugno-9 luglio 
- $2 fattura per il periodo di servizio 10 luglio-9 agosto

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (una licenza)      |10/6/2019   |9/7/2019         |$ 0                |1                 |$ 0            |Nuova         |
|10/7/2019 (una licenza)     | 10/7/2019    |9/8/2019        |$ 2        |1        | $ 2       |renew           |

### <a name="scenario-6---cancel-a-license-based-free-trial-saas-subscription"></a>Scenario 6: annullare una sottoscrizione SaaS della versione di valutazione gratuita basata su licenza

Puoi annullare una sottoscrizione SaaS (software come un servizio) di una versione di valutazione gratuita basata su licenza in qualsiasi momento, anche durante il periodo di valutazione gratuita. 

In questo scenario acquisti una sottoscrizione SaaS di una versione di valutazione gratuita basata su licenza il 1° luglio e quindi la annulli immediatamente nel Centro per i partner. 

Il file di riconciliazione includerà quanto segue: 
- $0 fattura per il periodo di servizio dal 10 giugno al 9 luglio per il nuovo acquisto
- $0 fattura per il periodo di servizio dal 10 luglio al 9 luglio per l'annullamento

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (11 licenze)      |10/6/2019   |9/7/2019         |$ 0                |11                |$ 0            |Nuova         |
|10/6/2019 (0 licenze)     | 10/6/2019    |9/7/2019        |$ 0        |11       | $ 0       |annulla           |

### <a name="scenario-7---convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Scenario 7: convertire una sottoscrizione SaaS di misurazione personalizzata da uno SKU a un altro per lo stesso prodotto nello stesso giorno

In questo scenario acquisti uno SKU (Silver) in un prodotto e lo converti in un altro SKU disponibile (Bronze) in questo prodotto nello stesso giorno. 

Il file di riconciliazione includerà quanto segue: 
- $20 fattura di Silver per il periodo di servizio 10 giugno, 2019-9 luglio 2020
- $20 rifatturato in modo prorata per Silver per il periodo di servizio 10 giugno, 2019-9 luglio, 2020
- $10 fattura di bronzo per il periodo di servizio del 10 giugno, 2019-9 luglio 2020

|**Data di acquisto**   |**SKU**   |**Inizio addebito**   |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (una licenza) |Silver     |10/6/2019   |10/6/2019         |$ 20        |1         |$ 20            |Nuova      |
|10/6/2019 (una licenza) |Silver    | 10/6/2019    |10/6/2019        |$ 20        |1       | $ -20       |Convertire           |
|10/6/2019 (una licenza) |Bronze    | 10/6/2019    |10/6/2019        |$ 10        |1       | $ 10       |Convertire           |

### <a name="scenario-8---purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Scenario 8: acquistare e annullare una sottoscrizione SaaS del contatore personalizzato dalla portale di Azure nello stesso giorno 

In questo scenario acquisti nel portale di Azure una sottoscrizione SaaS a consumo personalizzata e quindi la annulli nello stesso giorno. 

|**Data di acquisto**   |**SKU**   |**Inizio addebito**   |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (una licenza) |Bronze     |10/6/2019   |10/6/2019         |$ 10        |1         |$ 10            |Nuova      |
|6/10/2019 (0 licenze) |Bronze    | 10/6/2019    |10/6/2019        |$ 10        |1       | $ -10       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Fatturazione in base al piano di Azure

- **Data di fatturazione**: la fattura e il file di riconciliazione saranno disponibili nel dashboard/API del centro per i partner per l'ottava (mezzanotte UTC).

- **Periodo di fatturazione fattura**: il periodo di fatturazione della fattura è allineato al mese di calendario, ad esempio 10/1-10/31, 11/1-11/30.

- **Periodi di servizio di addebito**: i costi si allineano al mese di calendario. Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10. La fattura del mese successivo che verrà generata il 12/8 contiene tutti gli addebiti per il periodo di servizio 11/1-11/31.

- **Termine pagamento fattura**: NET 60 giorni.

- **Valuta fattura**: i partner continueranno a essere fatturati nella valuta assegnata country's del cliente. Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.

- **Incentivi**per i Partner: 45 giorni a pagamento a partire dalla fine del mese di fatturazione.

Per informazioni sul piano Azure, vedere:

- [Piano di Azure-Panoramica](azure-plan-get-started.md)

- [Piano di Azure-fatturazione](azure-plan-billing.md)