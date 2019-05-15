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
ms.openlocfilehash: 4b2b42c0d9bbb2654bbd486f987e3d5da9c562a2
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135381"
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
|Addebiti ricorrenti e monouso per prodotti Microsoft e terze parti ISV |Tutti i SaaS sottoscrizioni, le prenotazioni di Azure e i prodotti software (permanenti e basati su abbonamento) offerti da Microsoft e ISV di terze parti. Prodotti disponibili in vedere le [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Gli esempi includono il software SUSE Linux (abbonamento di software), Windows Server 2019 Essentials (software perpetuo), sottoscrizione al prodotto Azure ISV SaaS. |8 giorni del mese |Dal primo giorno all'ultimo giorno di ogni mese di calendario |La valuta del paese/regione del cliente si trova. Ciò significa che riceverai fatture separate e i file di riconciliazione nella valuta del paese/dell'area geografica ogni cliente che è venduto a nel periodo di fatturazione. |Yes |
