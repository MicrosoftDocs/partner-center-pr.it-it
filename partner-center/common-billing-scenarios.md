---
title: Scenari di fatturazione comuni | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: fatturazione, pagamenti, ordini, utilizzo, fatturazione basata su licenza, data anniversario, termine, annullamento, rinnovo, formula prezzo, file di riconciliazione, file di ricognizione
ms.localizationpriority: medium
ms.openlocfilehash: a4a152719f20c82ff338e6f577ea83fa9eb5e4f6
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653670"
---
# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-   Fatturazione del programma Cloud Solution Provider

Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze per una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## <a name="in-this-section"></a>Contenuto della sezione

-   [Fatturazione basata sull'utilizzo](#usagebased)

-   [Fatturazione basata su licenza](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione basata sull'utilizzo

Le sottoscrizioni basate sull'utilizzo vengono fatturate mensilmente in via posticipata, nel giorno dell'anniversario della sottoscrizione. Se, ad esempio, la data di ricorrenza della sottoscrizione è la 15, l'addebito verrà addebitato il 15 gennaio per il periodo di servizio del 15 dicembre 14 gennaio. Il 15 febbraio verrà addebitato nuovamente per il periodo di servizio 15 gennaio 14 febbraio e così via. Gli addebiti generati durante il giorno dell'anniversario della sottoscrizione verranno visualizzati nella fattura e nel file di riconciliazione seguenti.

Talvolta si può notare che alcuni costi di utilizzo non sono presenti nella fattura o che l'utilizzo di un mese precedente viene addebitato nella fattura del mese corrente. Non si tratta di un errore. indica semplicemente che il servizio è stato timestamp dopo che i servizi si sono verificati. L'utilizzo riportato entro 24 ore dalla fine del ciclo di fatturazione verrà visualizzato nella fattura del mese successivo. 

Le sottoscrizioni basate sull'utilizzo possono essere sospese in qualsiasi momento. 

Il listino prezzi CSP di Azure viene pubblicato mensilmente e si trova nella pagina Prezzi e offerte di vendita del Centro per i partner. Tieni presente che i prezzi possono cambiare ogni giorno e vengono riportati nella scheda Cronologia modifiche del listino prezzi.

I costi di utilizzo sono basati sui prezzi giornalieri. Se il prezzo cambia durante il periodo di servizio, vedrai una linea di fatturazione per ogni punto di servizio ripartito e il prezzo applicabile.

## <a href="" id="licensebased"></a>Fatturazione basata su licenza

**Fatturazione:** le sottoscrizioni basate su licenza vengono fatturate in anticipo nel giorno dell'anniversario della sottoscrizione.

**Giorno dell'anniversario:** il giorno dell'anniversario è il giorno del mese in cui hai acquistato la sottoscrizione. Ad esempio, se hai acquistato la sottoscrizione il 15 gennaio, il giorno dell'anniversario sarà il giorno 15 di ogni mese.

**Termine:** tutte le sottoscrizioni basate su licenza hanno un termine di pagamento di 12 mesi, che ha inizio il giorno dell'acquisto.

**Annullamento:** le sottoscrizioni sospese il mese 1, verranno accreditate al 100%. Le sottoscrizioni sospese nei mesi 2-12 verranno accreditate proporzionalmente.

**Rinnovo:** tutte le sottoscrizioni basate su licenza si rinnovano automaticamente per 12 mesi dopo l'inizio del termine di pagamento.

## <a href="" id="licensebasedmonthly"></a>Scenari di fatturazione mensili

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tariffa periodica   |4,00       |1        |4,00    

**Scenario 2: modificare la quantità di licenze**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/1/2018        |12/2/2018    |Ripartizione dell'istanza del ciclo   |-4,00       |1        |-4,00    
|13/1/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2,45       |1        |2,45    
|1/2/2018         |12/2/2018    | Ripartizione dell'istanza del ciclo   |1,55       |2        |3,10    
|13/2/2018         |12/3/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    

**Formule prezzo unitario:**

Il prezzo mensile è 4,00 e sono presenti 31 giorni nel periodo di servizio 1/13/2018-2/12/2018. Ciò equivale a un prezzo giornaliero di 0,129 (31/4).

Sono presenti 19 giorni nel periodo Proratio 1/13/2018-1/31/2018.

Prezzo unitario ripartito = 2,451 = 19 x 0,129

Sono presenti 12 giorni nel periodo Proratio 2/1/2018-2/12/2018.

Prezzo unitario ripartito = 1,54 = 12 x 0,129

**Scenario 3: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1 ° febbraio viene sospesa una sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Commissione di annullamento|-4,00|1|-4,00

**Scenario 4: sospendere dopo 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Tariffa periodica|4,00|1|4,00

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/2/2018|12/3/2018|Tariffa periodica|4,00|1|4,00

Il 1° marzo sospendi la sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/3/2018|Commissione di annullamento|-1,72|1|-1,72

**Formule prezzo unitario:**

Il prezzo mensile è 4,00 e il periodo di servizio 2/13/2018-3/12/2018 è di 28 giorni. Ciò equivale a un prezzo giornaliero di 0,143 (28/4).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Il periodo di annullamento 3/1/2018-3/12/2018 è di 12 giorni. 

Pertanto, il prezzo unitario =-1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Scenari di fatturazione annuale

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

**Scenario 2: aggiungere una licenza dopo la data di anniversario della sottoscrizione ma prima della data di fatturazione**

Viene acquistata una nuova sottoscrizione il 11/2/17 con una licenza per $211,20/anno. L'anniversario della sottoscrizione è impostato sull'11 di ogni mese. Il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione: 

-   $211,20 addebito per il periodo 2/11/17-2/10/18. 

Il 12/2/17 è stata acquistata una seconda licenza. La data di fatturazione è 14/2/17. Vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione: 

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione delle tariffe all'acquisto |211,20 |1 | 211,20 |

Nell'anniversario della tua sottoscrizione, 11/3/17, il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione per l'aumento della licenza del 12/2/17: 
-   -$211,20 di credito per il periodo 2/11/17-2/10/18. 
-   $0,58 addebitato in modo prorate per licenza per 1 licenza per il periodo 2/11/17-2/11/17. 
-   $15,62 addebitato in modo prorate per licenza per 2 licenze per il periodo 2/12/17-3/10/2017. 
-   $195,00 addebitato in modo prorate per licenza per 2 licenze per il periodo 3/11/2017-2/10/2018. 

Il 11/2/17 è stata acquistata una sottoscrizione. Il 12/2/17 è stata aggiunta una licenza. La data di fatturazione è 14/2/17. Il 11/2/18 viene rinnovata la sottoscrizione.

La prossima data di fatturazione è il 14/3/17 e vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione: 

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |-211,20 |1 |-211,20 |
|11/2/2017 |11/2/2017 |Ripartizione dell'istanza del ciclo |0,58 |1 |0,58 |
|12/2/2017 |10/3/2017 |Ripartizione dell'istanza del ciclo |15,62 |2 |31,25 |
|11/3/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |195,00 |2 |390,00 |

Il 11/2/18 la sottoscrizione viene rinnovata per un altro periodo di 12 mesi.


**Scenario 3: modificare la quantità di licenze**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/1/2018|12/1/2019|Ripartizione dell'istanza del ciclo|-48,00|1|-48,00
13/1/2018|31/1/2018|Ripartizione dell'istanza del ciclo|2,47|1|2,47
1/2/2018|12/1/2019|Ripartizione dell'istanza del ciclo|44,98|2|89,96

**Formule prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 19 giorni nel periodo di servizio 1/13/2018-1/31/2018. 

Di conseguenza, il prezzo unitario = 2,47 (19x0,13x1)

Sono presenti 346 giorni nel periodo di servizio 2/1/2018-1/12/2019. 

Di conseguenza, il prezzo unitario = 44,98 (346x0,13x2)

**Scenario 4: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

**Scenario 5: sospendere dopo 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basata su licenza non conterrà righe di fatturazione per questa sottoscrizione.
Il 1° marzo sospendi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Commissione di annullamento|-41,34|1|-41,34

**Formule prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 318 giorni nel periodo di servizio 3/1/2018-1/12/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito il prezzo unitario è -41,34.

**Scenario 6: sospendere e riattivare**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

Il 1° marzo riattivi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Ripartizione delle tariffe all'acquisto|41,34|1|41,34

**Formule prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Sono presenti 318 giorni nel periodo di servizio 3/1/2018-1/12/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1).
