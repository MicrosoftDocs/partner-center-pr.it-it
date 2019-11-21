---
title: Informazioni sui tipi di fatturazione nel Centro per i partner | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn about different billing types, billing periods, and billing dates you might see in Partner Center.
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione, pagamenti, ordini, file di riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 539d3150e571c33114feee2d316611d7ac324f24
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253198"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Informazioni sui tipi di fatturazione nel Centro per i partner

**Si applica a**

-  Centro per i partner
-  Partner aderenti al programma CSP

A seconda dei tipi di prodotti acquistati per i clienti, potresti avere periodi di fatturazione diversi e addebiti in giorni diversi dello stesso mese. Questo articolo illustra le modifiche apportate a partire dal 1° marzo 2019 e gli effetti prodotti da tali modifiche.

## <a name="billing-for-recurring-charges"></a>Fatturazione per addebiti periodici

L'esperienza di fatturazione per gli addebiti periodici delle sottoscrizioni basate su licenza e sull'utilizzo non cambia. We'll continue to bill you on the day of the month you selected as your billing date, and your billing period will continue to be the month prior to that date. If you selected the 15th day of the month for your billing date, you'll be billed for all activity from the 15th of one calendar month to the 14th of the next calendar month. Le fatture e i file di riconciliazione sono disponibili in genere 2-4 giorni dopo la data di fatturazione.

As before, we'll bill you for these products in the currency for the country/region you're located in, regardless of the location of the customer you sold the product to.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Fatturazione per addebiti occasionali e periodici

A partire dal 1° marzo 2019, è stata introdotta una nuova esperienza di fatturazione per gli addebiti occasionali e periodici per i prodotti ISV Microsoft e di terze parti.

Per questi prodotti, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. We'll make your invoice available on the 8th day of the following month. 

In altre parole, le transazioni effettuate tra il 1° e il 31 maggio 2019 saranno incluse nella fattura dell'8 giugno. Tutte le transazioni effettuate tra il 1° e il 30 giugno 2019 saranno incluse nella fattura dell'8 luglio. È possibile che nella stessa fattura vengano addebitati gli acquisti ricorrenti e occasionali. 

Puoi anche controllare il saldo o la fattura dell'account ogni volta che lo desideri, ad esempio tra il 1° maggio e il 7 giugno, e verificare le ultime attività dell'account senza dover attendere la fattura. Tieni presente che quando l'8 del mese viene pubblicata la fattura, verranno inclusi le imposte e altri eventuali addebiti e crediti applicabili, pertanto l'importo finale potrebbe variare rispetto a quanto visualizzato durante il periodo di fatturazione. 

You'll access your invoices the same way you do now, either in Partner Center or by API. They'll appear before midnight UTC on the 8th day of the month. 

|**Esperienza di fatturazione**|**Tipi di prodotto**|**Data di fatturazione**|**Periodo di fatturazione**|**Valuta di fatturazione**|**Disponibilità attività corrente**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Addebiti periodici per le sottoscrizioni basate su licenza e sull'utilizzo |Tutti i prodotti del [catalogo dei servizi online](https://partner.microsoft.com/commerce/preferredoffers/list). Gli esempi includono Office 365, Microsoft 365, Azure Active Directory, Azure (con pagamento in base al consumo), Dynamics 365, Power bi Pro |Data selezionata al momento della creazione dell'account del Centro per i partner |Mese che precede la data di fatturazione. |The currency of the country/region you're located in. For example, if your company is located in the United Kingdom, we'll bill you in British pounds sterling (GBP). If your company is located in India, we'll bill you in India Rupees (INR).  |No |
|Addebiti periodici e occasionali per prodotti ISV Microsoft e di terze parti |Tutte le sottoscrizioni SaaS, le prenotazioni di Azure e i prodotti software (perpetui e basati sulle sottoscrizioni) offerti da ISV Microsoft e di terze parti. Vedi i prodotti disponibili nel [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Gli esempi includono il software SUSE Linux (sottoscrizione software), Windows Server 2019 Essentials (software perpetuo) e la sottoscrizione di prodotti SaaS ISV di Azure. |8 di ogni mese |Dal primo all'ultimo giorno di ogni mese di calendario |Valuta del paese o dell'area geografica in cui si trova il tuo cliente. This means you'll receive separate invoices and reconciliation files in the currency of the country/region each customer you sold to in the billing period. |Sì |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Scenari di fatturazione per acquisti occasionali e periodici
### <a name="scenario-1---purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Scenario 1 - Purchase a subscription and then add a seat on the same day

Nello scenario 1 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno acquisti un'altra sottoscrizione dello stesso tipo allo stesso prezzo. 

Il file di riconciliazione includerà quanto segue: 
-   $4 bill for service period June 10 - July 9. 
-   $-4.00 prorated rebill for service period June 11 - June 11. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 1 = 4,00.
-   $8.00 prorated rebill for service period June 10 - July 9. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 30 x 2 = 8,00.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |1                 |$ 4            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -4       |addQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 8         |addQuantity           |

### <a name="scenario-2---purchase-a-subscription-and-then-add-more-later"></a>Scenario 2 - Purchase a subscription and then add more later

Nello scenario 2 acquisti una sottoscrizione l'11 giugno a un prezzo unitario di $ 4 e acquisti un'altra sottoscrizione il 12 giugno per lo stesso prodotto allo stesso prezzo. 

Il file di riconciliazione includerà quanto segue: 
-   $4 bill for service period June 10 - July 9. 
-   $-3.87 prorated rebill for service period June 11 - June 12. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 1 = 3,87.
-   $7.74 prorated rebill for service period June 12 - July 9. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (4/30) x 29 x 2 = 7,74.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (una licenza)     |10/6/2019   |9/7/2019         |$ 4         |1        |$ 4            |Nuova         |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |1        | $ -3,87       |addQuantity           |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 2      |$ 7,74       |addQuantity           |

### <a name="scenario-3---purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Scenario 3 - Purchase a subscription and then remove a seat on the same day

Nello scenario 3 acquisti due sottoscrizioni per lo stesso prodotto l'11 giugno a un prezzo unitario di $ 4. Successivamente lo stesso giorno rimuovi una delle postazioni.  

Il file di riconciliazione includerà quanto segue: 
-   $8 bill for two licenses for service period June 10 - July 9. 
-   $-8.00 prorated rebill for service period June 11 - June 11. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 30 x 2 = 8,00.
-   $4.00 prorated rebill for service period June 11 - July 9. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 30 x 1 = 4,00.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |9/7/2019         |$ 4                |2                 |$ 8            |Nuova         |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -8       |removeQuantity           |
|11/6/2019     | 10/6/2019    |9/7/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

### <a name="scenario-4---purchase-a-subscription-and-then-remove-seats-later"></a>Scenario 4 - Purchase a subscription and then remove seats later

Nello scenario 4 acquisti due sottoscrizioni l'11 giugno a un prezzo unitario di $ 4 e rimuovi una delle postazioni il 12 giugno. 

Il file di riconciliazione includerà quanto segue: 
-   $8 bill for service period June 10 - July 9. 
-   $-7.74 prorated rebill for service period June 11 - June 12. Questo è l'intervallo di tempo in cui hai avuto due licenze. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (4/30) x 29 x 2 = 7,74.
-   $3.87 prorated rebill for service period June 12 - July 9. Questo è l'intervallo di tempo in cui hai avuto una licenza. Calcolo = (4/30) x 29 x 1 = 3,87.

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (due licenze)     |10/6/2019   |9/7/2019         |$ 4         |2        |$ 8       |Nuova       |
|12/6/2019     | 10/6/2019    |9/7/2019        |$ 4        |2        | $ -7,74       |removeQuantity           |
|12/6/2019 (una licenza)    | 10/6/2019    |9/7/2019   |$ 4    |1      |$ 3,87    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Scenari di fatturazione per transazioni SaaS basate su licenza per versione di valutazione gratuita
### <a name="scenario-5---renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Scenario 5 - Renew a license-based free trial SaaS subscription to a paid subscription at the end of the free trial period

In questo scenario acquisti una sottoscrizione SaaS (software come un servizio) di una versione di valutazione gratuita basata su licenza il 10 giugno che si rinnova automaticamente come sottoscrizione a pagamento al termine del periodo di valutazione gratuita. 

I file di riconciliazione includeranno quanto segue: 
- $0 bill for service period June 10 - July 9 
- $2 bill for service period July 10 - August 9

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (una licenza)      |10/6/2019   |9/7/2019         |$ 0                |1                 |$ 0            |Nuova         |
|10/7/2019 (una licenza)     | 10/7/2019    |9/8/2019        |$ 2        |1        | $ 2       |renew           |

### <a name="scenario-6---cancel-a-license-based-free-trial-saas-subscription"></a>Scenario 6 - Cancel a license-based free trial SaaS subscription

Puoi annullare una sottoscrizione SaaS (software come un servizio) di una versione di valutazione gratuita basata su licenza in qualsiasi momento, anche durante il periodo di valutazione gratuita. 

In questo scenario acquisti una sottoscrizione SaaS di una versione di valutazione gratuita basata su licenza il 1° luglio e quindi la annulli immediatamente nel Centro per i partner. 

Il file di riconciliazione includerà quanto segue: 
- $0 bill for service period June 10th  - July 9th  for the new purchase
- $0 bill for service period July 10th  - July 9th for the cancelation

|**Data di acquisto**   |**Inizio addebito**  |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (11 licenze)      |10/6/2019   |9/7/2019         |$ 0                |11                |$ 0            |Nuova         |
|10/6/2019 (0 licenze)     | 10/6/2019    |9/7/2019        |$ 0        |11       | $ 0       |annulla           |

### <a name="scenario-7---convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Scenario 7 - Convert a custom meter SaaS subscription from one SKU to another for the same product on the same day

In questo scenario acquisti uno SKU (Silver) in un prodotto e lo converti in un altro SKU disponibile (Bronze) in questo prodotto nello stesso giorno. 

Il file di riconciliazione includerà quanto segue: 
- $20 bill of Silver for service period June 10th, 2019 - July 9th, 2020
- $20 prorated rebill for Silver for service period June 10th, 2019 - July 9th, 2020
- $10 bill of Bronze for service period June 10th, 2019 - July 9th, 2020

|**Data di acquisto**   |**SKU**   |**Inizio addebito**   |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (una licenza) |Silver     |10/6/2019   |10/6/2019         |$ 20        |1         |$ 20            |Nuova      |
|10/6/2019 (una licenza) |Silver    | 10/6/2019    |10/6/2019        |$ 20        |1       | $ -20       |Convertire           |
|10/6/2019 (una licenza) |Bronze    | 10/6/2019    |10/6/2019        |$ 10        |1       | $ 10       |Convertire           |

### <a name="scenario-8---purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Scenario 8 - Purchase and cancel a custom meter SaaS subscription from the Azure portal on the same day 

In questo scenario acquisti nel portale di Azure una sottoscrizione SaaS a consumo personalizzata e quindi la annulli nello stesso giorno. 

|**Data di acquisto**   |**SKU**   |**Inizio addebito**   |**Fine addebito**  |**Prezzo unitario**  |**Quantità**  |**Importo** |**Tipo di addebito** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (una licenza) |Bronze     |10/6/2019   |10/6/2019         |$ 10        |1         |$ 10            |Nuova      |
|6/10/2019 (0 licenze) |Bronze    | 10/6/2019    |10/6/2019        |$ 10        |1       | $ -10       |CancelImmediate  |

## <a name="billing-under-the-azure-plan"></a>Billing under the Azure plan

- **Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).

- **Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1 - 10/31, 11/1 - 11/30).

- **Charge service periods**: Charges will align to the calendar month. Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10. The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.

- **Invoice payment term**: Net 60 days.

- **Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency. Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.

- **Partner incentives**: Paid 45 days from the end of the invoice month.

For information on the Azure plan see:

- [Azure plan - overview](azure-plan-get-started.md)

- [Azure plan - billing](azure-plan-billing.md)