---
title: Informazioni sui tipi di fatturazione nel centro per i Partner | Centro per i partner
ms.topic: article
ms.date: 03/01/2019
Description: Informazioni sui diversi tipi di fatturazione, periodi di fatturazione e le date di fatturazione
author: labrenne
ms.author: labrenne
keywords: fatturazione, pagamenti, ordini, i file di riconciliazione, file riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122303"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Informazioni sui tipi di fatturazione nel centro per i Partner

**Si applica a**

-  Centro per i partner
-  Partner nel programma CSP

A seconda dei tipi di prodotti acquistati per i clienti, si potrebbero avere periodi di fatturazione diverse ed emessa diversi giorni dello stesso mese. Questo articolo spiega quali sono i cambiamenti a partire dal 1 marzo 2019, e come puoi influirà sulle modifiche.

## <a name="billing-for-recurring-charges"></a>Fatturazione per addebiti periodici

L'esperienza di fatturazione per addebiti periodici delle sottoscrizioni basate su licenza e basati sull'utilizzo non sta cambiando. Continueremo a addebito il giorno del mese selezionato come la data di fatturazione e il periodo di fatturazione continueranno a essere il mese prima di tale data. Se hai selezionato il 15 del mese per la data di fatturazione, viene fatturata per tutte le attività dal giorno 15 di un mese di calendario al 14 del mese successivo. Le fatture e file di riconciliazione sono in genere disponibili 2-4 giorni dopo la data di fatturazione.

Come prima, ti verranno addebitate puoi per questi prodotti nella valuta del paese/area geografica individuata al, indipendentemente dalla posizione del cliente è venduto il prodotto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Fatturazione per una tantum e selezionare addebiti periodici

A partire dal 1 marzo 2019, abbiamo introdotto una nuova esperienza di fatturazione per costi ricorrenti e una tantum per prodotti di terze parti ISV e Microsoft.

Per questi prodotti, il periodo di fatturazione inizia il primo giorno del mese e termina l'ultimo giorno del mese. La fattura verrà effettuata disponibile dall'8 giorno del mese successivo. 

In altre parole, tutte le transazioni effettuate tra 1 maggio e il 31 maggio 2019 verranno visualizzati nella fattura 8 giugno. Tutte le transazioni effettuate tra il 1 giugno e 30 giugno 2019 verranno visualizzati nella fattura 8 luglio. Potrebbe ottenere la fattura per gli acquisti una tantum e ricorrenti sulla stessa fattura. 

Puoi anche verificare account saldo/fattura ogni volta che si desidera (ad esempio, compreso tra 1 maggio e 7 giugno) e le attività più recenti account senza dover attendere la fattura. Tieni presente che quando si registra la fattura nell'8, includerà le imposte e qualsiasi altri costi applicabili e i crediti, in modo che la quantità finale potrebbero essere diversa da quella visualizzata durante il periodo di fatturazione. 

È possibile accedere le fatture allo stesso modo, che fare ora, nel centro per i Partner o dall'API. Verrà visualizzato prima di mezzanotte UTC il giorno del mese dall'8. 

|**Esperienza di fatturazione**|**Tipi di prodotti**|**Data di fatturazione**|**Periodo di fatturazione**|**Valuta di fatturazione**|**Attività corrente disponibile?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Addebiti periodici per le sottoscrizioni basate su licenza e basati sull'utilizzo |Tutti i prodotti dal [catalogo di servizi online](https://partner.microsoft.com/commerce/preferredoffers/list). Ecco alcuni esempi Office 365, Microsoft 365, Azure Active Directory, Azure (tariffe), Dynamics 365, PowerBI Pro |La data selezionata quando creato l'account del centro per i Partner |Il mese prima della data di fatturazione. |Valuta del paese/area geografica trovano. Ad esempio, se la società si trova nel Regno Unito, ti verranno addebitate puoi nel Regno uniti euro inglese (GBP). Se la società si trova in India, ti verranno addebitate in INR India indiana (con).  |No |
|Costi ricorrenti e una tantum per prodotti di terze parti gli ISV e Microsoft |Tutti i SaaS sottoscrizioni, prenotazioni di Azure e prodotti software (perpetua e basate su sottoscrizione) offerti da Microsoft e gli ISV di terze parti. Vedi i prodotti disponibili [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Gli esempi includono software SUSE Linux (sottoscrizione software), Windows Server 2019 Essentials (definitiva), sottoscrizione di Azure ISV SaaS prodotto. |8 giorni di ogni mese |Dal primo giorno all'ultimo giorno di ogni mese di calendario |Valuta del paese/area geografica cui si trova il cliente. Ciò significa che riceverai fatture separate e file di riconciliazione nella valuta del paese/area geografica ogni cliente che ha venduto nel periodo di fatturazione. |Sì |
