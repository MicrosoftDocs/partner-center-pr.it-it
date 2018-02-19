<a name="-head"></a><<<<<<< HEAD
---
titolo: Scenari di fatturazione comuni | Centro per i partner descrizione: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.
ms. AssetID: E4BBD3E7-AFE2-4998-950D-0D27D1178160 autore: MaggiePucciEvans Parole chiave: fatturazione, pagamenti, ordini, utilizzo, fatturazione basata su licenza, data dell'anniversario, periodo gratuito, termine, annullamento, rinnovo, formula di prezzo, file di riconciliazione, file riconciliazione
---

# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze per una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## <a name="in-this-section"></a>Contenuto della sezione

-   [Fatturazione in base all'uso](#usagebased)

-   [Fatturazione in base alle licenze](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione in base all'uso

Vengono fatturati solo i servizi usati nel periodo di fatturazione precedente. Nella fattura comparirà qualsiasi applicazione o servizio di Azure abilitato e usato durante il periodo di fatturazione.

-   Le tariffe per i servizi a consumo possono variare durante il ciclo di fatturazione.
    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni
    -   Le diminuzioni di prezzo sono riportate il giorno in cui vengono rese effettive.
    -   Le sottoscrizioni esistenti vengono fatturate in base alle tariffe in vigore all'inizio del ciclo di fatturazione.
    -   Le nuove sottoscrizioni (quelle create durante il ciclo di fatturazione) vengono fatturate in base alle tariffe in vigore quando sono state aggiunte.
-   Se annulli una sottoscrizione durante il primo ciclo di fatturazione, i costi di utilizzo saranno indicati nel file di riconciliazione per il periodo in cui la sottoscrizione era attiva.

## <a href="" id="licensebased"></a>Fatturazione in base alle licenze

**Fatturazione:** le sottoscrizioni basate su licenza vengono fatturate in anticipo nel giorno dell'anniversario della sottoscrizione.

**Giorno dell'anniversario:** le sottoscrizioni con fatturazione mensile sono allineate alla data di fatturazione del partner e le sottoscrizioni con fatturazione annuale sono allineate alla data di acquisto.

**Periodo gratuito:** alle sottoscrizioni con fatturazione mensile viene assegnato un periodo gratuito a partire dalla data di acquisto fino alla successiva data di fatturazione del partner.

**Termine:** tutte le sottoscrizioni basate su licenza hanno un termine di pagamento di 12 mesi. Il termine di pagamento inizia dalla data di acquisto per le sottoscrizioni con fatturazione annuale e alla data di fatturazione successiva alla data di acquisto per le sottoscrizioni con fatturazione mensile.

**Annullamento:**le sottoscrizioni annullate entro i primi 30 giorni del termine di pagamento verranno accreditate al 100%. Le sottoscrizioni annullate dopo i 30 giorni verranno accreditate proporzionalmente.

**Rinnovo:** tutte le sottoscrizioni basate su licenza si rinnovano automaticamente per 12 mesi dopo l'inizio del termine di pagamento.

## <a href="" id="licensebasedmonthly"></a>Scenari di fatturazione mensile

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         | 14/1/2018   |Tariffa di acquisto   |0,00       |1       |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/2/2018         |14/3/2018    |Tariffa periodica   |4,00       |1        |4,00    
Si continuerà l'addebito il giorno 15 di ogni mese fino a quando la sottoscrizione viene sospesa.

**Scenario 2: modificare la quantità di licenze**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tariffa di acquisto   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/1/2018        |14/2/2018    |Ripartizione dell'istanza del ciclo   |-4,00       |1        |4,00    
|15/1/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2,21       |1        |2,21    
|1/2/2018         |14/2/2018    | Ripartizione dell'istanza del ciclo   |1,82       |2        |3,64    
|15/2/2018         |14/3/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    

**Formule per il prezzo unitario:**

Il prezzo mensile è di 4,00 e sono presenti 31 giorni nel periodo del servizio 15/1/2018-14/2/2018. Ciò equivale a un prezzo giornaliero di 0,13 (31/4).

Ci sono 17 giorni nel periodo di ripartizione proporzionale 15/1/2018 – 31/1/2018.

Prezzo unitario ripartito = 2,21 = 17 x 0,13

Ci sono 14 giorni nel periodo di ripartizione proporzionale 1/2/2018 – 14/2/2018.

Prezzo unitario ripartito = 1,82 = 14 x 0,13

**Scenario 3: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tariffa di acquisto   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1° febbraio sospendi la sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/1/2018|14/2/2018|Commissione di annullamento|-4,00|1|4,00

**Scenario 4: sospendere dopo di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|14/1/2018|Tariffa di acquisto|0,00|1|0,00
15/1/2018|14/2/2018|Tariffa periodica|4,00|1|4,00

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/2/2018|14/3/2018|Tariffa periodica|4,00|1|4,00

Il 1° marzo sospendi la sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|14/3/2018|Commissione di annullamento|-1,96|1|-1,96

**Formule per il prezzo unitario:**

Il prezzo mensile è di 4,00 e sono presenti 28 giorni nel periodo del servizio 15/2/2018-14/3/2018. Ciò equivale a un prezzo giornaliero di 0,14 (28/4).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 14 giorni nel periodo di annullamento 1/3/2018 – 14/3/2018. 

Di conseguenza, il prezzo unitario = -1,96 (14x0,14 x(-1)).

## <a name="annual-billing-scenarios"></a>Scenario di fatturazione annuale

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

**Scenario 2: modificare la quantità di licenze**

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

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 19 giorni nel periodo di servizio 13/1/2018 – 31/1/2018. 

Di conseguenza, il prezzo unitario = 2,47 (19x0,13x1)

Ci sono 346 giorni nel periodo di servizio 1/2/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 44,98 (346x0,13x2)

**Scenario 3: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

**Scenario 4: sospendere dopo di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basata su licenza non conterrà righe di fatturazione per questa sottoscrizione.
Il 1° marzo sospendi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Commissione di annullamento|-41,34|1|-41,34

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito il prezzo unitario è -41,34.

**Scenario 5: sospendere e riattivare**

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

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1).

<a name=""></a>=======
---
titolo: Scenari di fatturazione comuni | Centro per i partner descrizione: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.
ms. AssetID: E4BBD3E7-AFE2-4998-950D-0D27D1178160 autore: MaggiePucciEvans Parole chiave: fatturazione, pagamenti, ordini, utilizzo, fatturazione basata su licenza, data dell'anniversario, periodo gratuito, termine, annullamento, rinnovo, formula di prezzo, file di riconciliazione, file riconciliazione
---

# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze per una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## <a name="in-this-section"></a>Contenuto della sezione

-   [Fatturazione in base all'uso](#usagebased)

-   [Fatturazione in base alle licenze](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione in base all'uso

Vengono fatturati solo i servizi usati nel periodo di fatturazione precedente. Nella fattura comparirà qualsiasi applicazione o servizio di Azure abilitato e usato durante il periodo di fatturazione.

-   Le tariffe per i servizi a consumo possono variare durante il ciclo di fatturazione.
    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni
    -   Le diminuzioni di prezzo sono riportate il giorno in cui vengono rese effettive.
    -   Le sottoscrizioni esistenti vengono fatturate in base alle tariffe in vigore all'inizio del ciclo di fatturazione.
    -   Le nuove sottoscrizioni (quelle create durante il ciclo di fatturazione) vengono fatturate in base alle tariffe in vigore quando sono state aggiunte.
-   Se annulli una sottoscrizione durante il primo ciclo di fatturazione, i costi di utilizzo saranno indicati nel file di riconciliazione per il periodo in cui la sottoscrizione era attiva.

## <a href="" id="licensebased"></a>Fatturazione in base alle licenze

**Fatturazione:** le sottoscrizioni basate su licenza vengono fatturate in anticipo nel giorno dell'anniversario della sottoscrizione.

**Giorno dell'anniversario:** le sottoscrizioni con fatturazione mensile sono allineate alla data di fatturazione del partner e le sottoscrizioni con fatturazione annuale sono allineate alla data di acquisto.

**Periodo gratuito:** alle sottoscrizioni con fatturazione mensile viene assegnato un periodo gratuito a partire dalla data di acquisto fino alla successiva data di fatturazione del partner.

**Termine:** tutte le sottoscrizioni basate su licenza hanno un termine di pagamento di 12 mesi. Il termine di pagamento inizia dalla data di acquisto per le sottoscrizioni con fatturazione annuale e alla data di fatturazione successiva alla data di acquisto per le sottoscrizioni con fatturazione mensile.

**Annullamento:**le sottoscrizioni annullate entro i primi 30 giorni del termine di pagamento verranno accreditate al 100%. Le sottoscrizioni annullate dopo i 30 giorni verranno accreditate proporzionalmente.

**Rinnovo:** tutte le sottoscrizioni basate su licenza si rinnovano automaticamente per 12 mesi dopo l'inizio del termine di pagamento.

## <a href="" id="licensebasedmonthly"></a>Scenari di fatturazione mensile

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         | 14/1/2018   |Tariffa di acquisto   |0,00       |1       |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/2/2018         |14/3/2018    |Tariffa periodica   |4,00       |1        |4,00    
Si continuerà l'addebito il giorno 15 di ogni mese fino a quando la sottoscrizione viene sospesa.

**Scenario 2: modificare la quantità di licenze**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tariffa di acquisto   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1° febbraio aumenti la quantità di licenze da una a due. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/1/2018        |14/2/2018    |Ripartizione dell'istanza del ciclo   |-4,00       |1        |4,00    
|15/1/2018         |31/1/2018    | Ripartizione dell'istanza del ciclo   |2,21       |1        |2,21    
|1/2/2018         |14/2/2018    | Ripartizione dell'istanza del ciclo   |1,82       |2        |3,64    
|15/2/2018         |14/3/2018    | Ripartizione dell'istanza del ciclo   |4,00       |2        |8,00    

**Formule per il prezzo unitario:**

Il prezzo mensile è di 4,00 e sono presenti 31 giorni nel periodo del servizio 15/1/2018-14/2/2018. Ciò equivale a un prezzo giornaliero di 0,13 (31/4).

Ci sono 17 giorni nel periodo di ripartizione proporzionale 15/1/2018 – 31/1/2018.

Prezzo unitario ripartito = 2,21 = 17 x 0,13

Ci sono 14 giorni nel periodo di ripartizione proporzionale 1/2/2018 – 14/2/2018.

Prezzo unitario ripartito = 1,82 = 14 x 0,13

**Scenario 3: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tariffa di acquisto   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tariffa periodica   |4,00       |1        |4,00    

Il 1° febbraio sospendi la sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/1/2018|14/2/2018|Commissione di annullamento|-4,00|1|4,00

**Scenario 4: sospendere dopo di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione mensile. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo le seguenti righe di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|14/1/2018|Tariffa di acquisto|0,00|1|0,00
15/1/2018|14/2/2018|Tariffa periodica|4,00|1|4,00

Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/2/2018|14/3/2018|Tariffa periodica|4,00|1|4,00

Il 1° marzo sospendi la sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|14/3/2018|Commissione di annullamento|-1,96|1|-1,96

**Formule per il prezzo unitario:**

Il prezzo mensile è di 4,00 e sono presenti 28 giorni nel periodo del servizio 15/2/2018-14/3/2018. Ciò equivale a un prezzo giornaliero di 0,14 (28/4).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 14 giorni nel periodo di annullamento 1/3/2018 – 14/3/2018. 

Di conseguenza, il prezzo unitario = -1,96 (14x0,14 x(-1)).

## <a name="annual-billing-scenarios"></a>Scenario di fatturazione annuale

**Scenario 1: nuova sottoscrizione**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

**Scenario 2: Aggiungere una licenza dopo la data dell'anniversario della sottoscrizione, ma prima della data di fatturazione**

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


**Scenario 3: modificare la quantità di licenze**

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

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 19 giorni nel periodo di servizio 13/1/2018 – 31/1/2018. 

Di conseguenza, il prezzo unitario = 2,47 (19x0,13x1)

Ci sono 346 giorni nel periodo di servizio 1/2/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 44,98 (346x0,13x2)

**Scenario 4: sospendere prima di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 1° febbraio sospendi la tua sottoscrizione. Il 15 febbraio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Commissione di annullamento|-48,00|1|-48,00

**Scenario 5: sospendere dopo di 30 giorni**

La data di fatturazione è il 15 di ogni mese. Il 13 gennaio acquisti una nuova sottoscrizione con una licenza per $4 al mese e selezioni la fatturazione annuale. Il 15 gennaio il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Rateizza le tariffe all'acquisto|48,00|1|48,00

Il 15 febbraio il file di riconciliazione basata su licenza non conterrà righe di fatturazione per questa sottoscrizione.
Il 1° marzo sospendi la tua sottoscrizione. Il 15 marzo il file di riconciliazione basata su licenza conterrà solo la seguente riga di fatturazione:
|Data inizio addebito |Data fine addebito |Tipo di addebito |Prezzo unitario |Quantità |Importo |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Commissione di annullamento|-41,34|1|-41,34

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1). Poiché si tratta di un credito il prezzo unitario è -41,34.

**Scenario 6: sospendere e riattivare**

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

**Formule per il prezzo unitario:**

Il prezzo annuale è di 48,00 che equivale al prezzo giornaliero di 0,13 (48,00/365).

Prezzo unitario = giorni nel periodo di servizio x prezzo giornaliero x numero di licenze.

Ci sono 318 giorni nel periodo di servizio 1/3/2018 – 12/1/2019. 

Di conseguenza, il prezzo unitario = 41,34 (318x0,13x1).
>>>>>>> e10d68b8029ab91ddbfc67d278575a79639cf269
