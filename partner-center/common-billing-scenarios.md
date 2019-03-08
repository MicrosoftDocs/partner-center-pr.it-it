---
title: Scenari di fatturazione comuni | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: la fatturazione, pagamenti, ordini, utilizzo, fatturazione basati su licenza, la data di ricorrenza, termine, l'annullamento, rinnovo, formula del price, file di riconciliazione, riconoscimento file
ms.localizationpriority: medium
ms.openlocfilehash: 5f7820219110bfdbe153d8467da91e1d66d82341
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57585704"
---
# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-   Fatturazione di cloud Solution Provider program

Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze per una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## <a name="in-this-section"></a>Contenuto della sezione

-   [Fatturazione basata sull'utilizzo](#usagebased)

-   [Fatturazione basati su licenza](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione basata sull'utilizzo

Le sottoscrizioni basate sull'utilizzo vengono fatturate mensilmente in via posticipata, nel giorno dell'anniversario della sottoscrizione. Ad esempio, se la data dell'anniversario della sottoscrizione è di 15 del mese, riceverai l'addebito il 15 gennaio per il periodo di servizio 15 dicembre-14 gennaio. Verranno addebitati anche in questo caso il 15 febbraio per il periodo del servizio il 15 gennaio-14 febbraio e così via. I costi che vengono generati nel giorno anniversario sottoscrizione verranno visualizzato nel file di riconciliazione e fatturazione seguente.

È talvolta possibile notare che alcuni addebiti non sono presenti la fattura, o che l'utilizzo di un mese precedente verrà addebitato nella fattura del mese corrente. Non si tratta di un errore. significa semplicemente che il servizio è con timestamp dopo l'esecuzione dei servizi. Utilizzo segnalato entro 24 ore di fine del ciclo di fatturazione verrà visualizzati nella fattura del mese successivo. 

Le sottoscrizioni basate sull'utilizzo possono essere sospeso in qualsiasi momento. 

Il listino prezzi CSP di Azure viene pubblicato mensilmente e si trova nella pagina Prezzi e offerte di vendita del Centro per i partner. Tieni presente che i prezzi possono cambiare ogni giorno e vengono riportati nella scheda Cronologia modifiche del listino prezzi.

I costi di utilizzo sono basati sui prezzi giornalieri. Se il prezzo cambia durante il periodo di servizio, vedrai una linea di fatturazione per ogni punto di servizio ripartito e il prezzo applicabile.

## <a href="" id="licensebased"></a>Fatturazione basati su licenza

**Fatturazione:** Le sottoscrizioni basate su licenza vengono fatturate in anticipo il giorno dell'anniversario di sottoscrizione.

**Giorno di ricorrenza annuale:** Il giorno dell'anniversario è il giorno del mese che è stata acquistata la sottoscrizione. Ad esempio, se hai acquistato la sottoscrizione il 15 gennaio, il giorno dell'anniversario sarà il giorno 15 di ogni mese.

**Periodo di validità:** Tutte le sottoscrizioni basati su licenza contengono un termine a pagamento di 12 mesi, che inizia alla data di acquisto.

**Annullamento:** Le sottoscrizioni sospese nel mese 1 sarà accreditato 100%. Le sottoscrizioni sospese nei mesi 2-12 verranno accreditate proporzionalmente.

**Rinnovo:** Tutte le sottoscrizioni basati su licenza di rinnovo automatico per 12 mesi dopo il termine a pagamento ha inizio.

## <a href="" id="licensebasedmonthly"></a>Scenari di fatturazione mensili

**Scenario 1: Nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tariffa periodica   |4,00       |1        |4,00    

**Scenario 2: Modificare la quantità di licenze**

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

**Unit Price formule:**

Il prezzo mensile è di 4,00 e sono presenti 31 giorni nel periodo del servizio 13/1/2018-12/2/2018. Ciò equivale a un prezzo giornaliero di 0,129 (31/4).

Ci sono 19 giorni nel periodo di ripartizione proporzionale 13/1/2018 – 31/1/2018.

Prezzo unitario ripartito = 2,451 = 19 x 0,129

Ci sono 12 giorni nel periodo di ripartizione proporzionale 1/2/2018 – 12/2/2018.

Prezzo unitario ripartito = 1,54 = 12 x 0,129

**Scenario 3: Sospensione prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1 ° febbraio si sospende una sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Commissione di annullamento|-4,00|1|-4,00

**Scenario 4: Sospensione dopo 30 giorni**

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

**Unit Price formule:**

Il prezzo mensile è di 4,00 e sono presenti 28 giorni nel periodo del servizio 13/2/2018-12/3/2018. Ciò equivale a un prezzo giornaliero di 0,143 (28/4).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Il periodo di annullamento ha una durata di 12 giorni 1/3/2018 - 12/3/2018. 

Pertanto, il prezzo unitario =-1.716 (12 x 0.143 x (-1)).

## <a name="annual-billing-scenarios"></a>Scenari di fatturazione annuale

**Scenario 1: Nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

**Scenario 2: Aggiungere licenze dopo la data di ricorrenza annuale della sottoscrizione, ma prima della data di fatturazione**

Viene acquistata una nuova sottoscrizione il 11/2/17 con una licenza per $211,20/anno. L'anniversario della sottoscrizione è impostato sull'11 di ogni mese. Il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione: 

-   Addebito di $211,20 per il periodo 2/11/17 - 10/2/18. 

Il 12/2/17 è stata acquistata una seconda licenza. La data di fatturazione è 14/2/17. Vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione: 

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione delle tariffe all'acquisto |211,20 |1 | 211,20 |

Nell'anniversario della tua sottoscrizione, 11/3/17, il sistema di fatturazione Microsoft crea le seguenti righe di fatturazione per l'aumento della licenza del 12/2/17: 
-   Credito di -$211,20 per il periodo 2/11/17 - 2/10/18. 
-   Addebito di $0,58 ripartito per licenza per 1 licenza per il periodo 11/2/17 - 11/2/17. 
-   Addebito di $15,62 ripartito per licenza per 2 licenze per il periodo 12/2/17 - 10/3/2017. 
-   Addebito di $195,00 ripartito per licenza per 2 licenze per il periodo 11/3/2017 - 10/2/2018. 

Il 11/2/17 è stata acquistata una sottoscrizione. Il 12/2/17 è stata aggiunta una licenza. La data di fatturazione è 14/2/17. Il 11/2/18 viene rinnovata la sottoscrizione.

La prossima data di fatturazione è il 14/3/17 e vengono generati i file di riconciliazione e di fatturazione. Il file di riconciliazione conterrà le seguenti righe di fatturazione: 

|Data inizio addebito  |Data fine addebito  |Tipo di addebito  |Prezzo unitario |Quantità | Importo |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/2/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |-211,20 |1 |-211,20 |
|11/2/2017 |11/2/2017 |Ripartizione dell'istanza del ciclo |0,58 |1 |0,58 |
|12/2/2017 |10/3/2017 |Ripartizione dell'istanza del ciclo |15,62 |2 |31,25 |
|11/3/2017 |10/2/2018 |Ripartizione dell'istanza del ciclo |195,00 |2 |390,00 |

Il 11/2/18 la sottoscrizione viene rinnovata per un altro periodo di 12 mesi.


**Scenario 3: Modificare la quantità di licenze**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/1/2018|12/1/2019|Ripartizione dell'istanza del ciclo|-48,00|1|-48,00
13/1/2018|31/1/2018|Ripartizione dell'istanza del ciclo|2,47|1|2,47
1/2/2018|12/1/2019|Ripartizione dell'istanza del ciclo|44,98|2|89,96

**Unit Price formule:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 19 giorni nel periodo di servizio 13/1/2018 – 31/1/2018. 

Di conseguenza, il prezzo unitario = 2,47 (19x0,13x1)

Ci sono 346 giorni nel periodo di servizio 1/2/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 44,98 (346x0,13x2)

**Scenario 4: Sospensione prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

**Scenario 5: Sospensione dopo 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basata su licenza non conterrà righe di fatturazione per questa sottoscrizione.
Il 1° marzo sospendi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Commissione di annullamento|-41,34|1|-41,34

**Unit Price formule:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito il prezzo unitario è -41,34.

**Scenario 6: Sospendere e riattivare**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

Il 1° marzo riattivi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:

|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Rateizza le tariffe all'acquisto|41,34|1|41,34

**Unit Price formule:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1).
