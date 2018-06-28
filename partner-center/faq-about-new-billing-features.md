---
title: Domande frequenti sulle nuove funzionalità di fatturazione | Centro per i partner
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
ms.assetid: ''
author: MaggiePucciEvans
ms.openlocfilehash: 9cb79ba60c06d273bcf2d6435d9146c4920b3ace
ms.sourcegitcommit: f1abc58390563a61a3a2678a7420cd54dfbe2d38
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/01/2018
ms.locfileid: "1936230"
---
# <a name="faq-about-new-billing-features"></a>Domande frequenti sulle nuove funzionalità di fatturazione

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Di seguito sono riportate le domande frequenti su fatturazione annuale del Centro per i partner e funzionalità della versione di valutazione gratuita. 

## <a name="in-this-section"></a>Contenuto della sezione

-   [Domande frequenti sulla fatturazione annuale](#annualbillingfaq)

-   [Domande frequenti sulle versioni di valutazione gratuite](#freetrialsfaq)

-   [Domande frequenti sull'allineamento della fatturazione](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Domande frequenti sulla fatturazione annuale

Sezioni:

[Panoramica dei vantaggi della fatturazione annuale](#overviewandbenefits)

[Effettuare l'ordine e scenari di fatturazione](#placingyourorder)

[Modificare l'abbonamento](#changingyoursubscription)

[Calcolo dei prezzi](#pricingcalculation)

[Creazione di report](#reporting)

[Incentivi](#incentives)


<a href="" id="overviewandbenefits"></a>**Panoramica dei vantaggi della fatturazione annuale**

**D:** Cosa è cambiato?

-   **R:** In risposta alle richieste dei clienti, abbiamo introdotto l'opzione per il pagamento di alcune sottoscrizioni CSP su base annuale o mensile. Questa nuova opzione è diventata disponibile il 17 ottobre 2017.

**D:** Chi può partecipare?

-   **R:** Tutti i partner e i tipi di partner possono avvalersi della fatturazione annuale. La fatturazione annuale è disponibile in tutti i mercati in cui è attualmente disponibile il CSP. 

**D:** Cosa devo prendere in considerazione in relazione alla fatturazione annuale?    

-   **R:** Per prepararti devi considerare come cambia il processo di vendita. Ecco alcuni suggerimenti che ti consentono di utilizzare al meglio la fatturazione annuale. 
    - Aggiorna le API per la funzionalità di fatturazione annuale, se applicabile. 
    - Rivedi le modifiche nel file di fatturazione e riconciliazione basato su licenza.
    - Assicurati che il team sia informato.
    - Aggiorna i processi interni in base alle esigenze.

**D:** Quali sono i vantaggi della fatturazione annuale? 

-   **R:** La fatturazione annuale offre i seguenti vantaggi:

    - Maggiore flessibilità nelle opzioni di pagamento.

    - Migliore allineamento con la fatturazione dei clienti.

    - Impatto ridotto delle fluttuazioni di valuta.

    - Costi operativi di fatturazione ridotti.

**D:** Quali offerte disporranno dell'opzione per la fatturazione annuale?

-   **R:** La maggior parte delle sottoscrizioni basate su licenza ha l'opzione per la fatturazione mensile o annuale. Le sottoscrizioni basate su utilizzo hanno solo l'opzione di fatturazione mensile. La colonna J della matrice dell'offerta identifica le frequenze di fatturazione disponibili per ogni offerta. La matrice dell'offerta è disponibile nella sezione "Vedere offerte e prezzi" nel Centro per i partner. .

**D: ** La fatturazione annuale si intende per sottoscrizione o per licenza?       

-   **R:** La fatturazione mensile e annuale è per sottoscrizione.

**D:** Sono state apportate modifiche alle API per supportare la fatturazione annuale?    

-   **R:** Per utilizzare la fatturazione annuale ci sono alcune modifiche necessarie per le API. Puoi trovare informazioni più dettagliate negli articoli seguenti:

    - https://partnercenter.microsoft.com/en-us/partner/developer

    - https://msdn.microsoft.com/en-us/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Codice di esempio: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Effettuare l'ordine e scenari di fatturazione**

**D:** Ci sarà un'offerta univoca in modo specifico per gli ordini con la fatturazione annuale?   

-   **R:** No. La frequenza di fatturazione, inclusa l'opzione di fatturazione annuale è assegnata all'offerta come attributo. Tuttavia puoi rinominare un'offerta con un nome descrittivo per il cliente per consentire la differenziazione.

**D:** Come si seleziona la fatturazione annuale?

-   **R: ** Quando aggiungi una nuova sottoscrizione ti verrà richiesto di scegliere la frequenza di fatturazione. A questo punto puoi scegliere l'opzione di fatturazione annuale. Dopo aver selezionato la fatturazione annuale, verranno visualizzate tutte le offerte disponibili.

**D:** Come avverrà la fatturazione se si sceglie la fatturazione annuale?    

-   **R:** La fattura verrà emessa alla data di fatturazione successiva. Ad esempio, se la data di fatturazione è il 1° del mese e tu acquisti una sottoscrizione con fatturazione annuale il 29 ottobre 2017, la fattura verrà emessa il 1° novembre 2017. Supponendo che non apporti alcuna modifica alla licenza, la fattura verrà emessa il 1° novembre 2018. Se apporti una modifica alla licenza, riceverai un credito e una nuova fattura alla data di fatturazione successiva. 

**D:** Posso suddividere una sottoscrizione in modo che una parte viene fatturata mensilmente e l'altra annualmente?  

-   **R:** No. L'intera sottoscrizione deve avere la stessa frequenza di fatturazione. L'intera sottoscrizione deve avere la fatturazione mensile o annuale.

**D:** Qual è la data di rinnovo della sottoscrizione con fatturazione annuale?     

-   **R:** La data del rinnovo cade 12 mesi dopo la data di inizio del servizio. Il periodo del servizio inizia il giorno in cui viene creata la sottoscrizione.  Ad esempio, una sottoscrizione creata il 10 gennaio 2018 si rinnova il 10 gennaio 2019.

**D:** Quando verrà emessa la fattura per il rinnovo di una sottoscrizione con fatturazione annuale? 

-   **R:** La fattura verrà emessa alla data di fatturazione successiva alla data di rinnovo della sottoscrizione. Ad esempio, se acquisti una sottoscrizione con fatturazione annuale addebitata il 15 gennaio 2018 e la data di fatturazione è 20 gennaio, la sottoscrizione verrà rinnovata il 15 gennaio 2019. La fattura per il rinnovo verrà addebitata il 20 gennaio 2019.

**D:** Le sottoscrizioni con fatturazione annuale prevedono un periodo gratuito?

-   **R: **No, le sottoscrizioni con fatturazione annuale non prevedono un periodo gratuito. Il termine di pagamento di 12 mesi inizia dalla data di acquisto. Diversamente dalle sottoscrizioni con fatturazione mensile che invece prevedono un periodo gratuito a partire dalla data di acquisto fino alla successiva data di fatturazione.

**D: **Può un cliente avere più sottoscrizioni della stessa offerta con diverse frequenze di fatturazione?    

-   **R:** Dipende dall'offerta. Alcune offerte sono limitate a una sottoscrizione per cliente. Se l'offerta non è limitata, un cliente può avere più sottoscrizioni della stessa offerta con frequenze di fatturazione diverse. Puoi trovare i dettagli di tutti i limiti e le restrizioni delle offerte nella colonna I della matrice dell'offerta. La matrice dell'offerta è disponibile nella sezione "Vedere offerte e prezzi" nel Centro per i partner.

<a href="" id="changingyoursubscription"></a>**Modificare l'abbonamento**

**D:** Posso aggiungere una nuova licenza a una sottoscrizione che ha la fatturazione annuale?    

-   **R:** Sì. Puoi modificare la quantità di licenze per le sottoscrizioni in qualsiasi momento. L'aggiunta di ulteriori licenze non influirà sulla frequenza di fatturazione. 

**D:** Posso aggiungere licenze che hanno la fatturazione mensile a una sottoscrizione che ha la fatturazione annuale? 

-   **R:** Quando acquisti una sottoscrizione con fatturazione annuale, eventuali licenze aggiuntive seguiranno la stessa frequenza di fatturazione. Se quindi devi acquistare licenze con fatturazione mensile, devi acquistare una nuova sottoscrizione.

**D:** Posso cambiare la frequenza di fatturazione per una sottoscrizione da mensile ad annuale e viceversa? 

-   **R:** No. Dopo averla selezionata, non è possibile cambiare una frequenza di fatturazione. 

**D:** La fatturazione annuale è disponibile per le offerte dei componenti aggiuntivi?   

-   **R:** Sì. La sottoscrizione del componente aggiuntivo avrà automaticamente la stessa frequenza di fatturazione della sottoscrizione padre.

**D:** Come funziona la fatturazione annuale quando si aggiungono o rimuovono licenze? 

-   **R:** Puoi aggiungere o rimuovere licenze in qualsiasi momento. Riceverai un credito e una nuova fattura ripartita proporzionalmente alla data di fatturazione successiva dopo aver cambiato il numero di licenze. 

**D:** Cosa succede se annullo una sottoscrizione con fatturazione annuale?    

-   **R:** Il criterio di annullamento è lo stesso per tutte le frequenze di fatturazione. Se la sottoscrizione viene annullata entro 30 giorni dal termine di pagamento di 12 mesi, riceverai un credito del 100% alla data di fatturazione successiva. Se la sottoscrizione viene annullata dopo 30 giorni dal termine di pagamento di 12 mesi, riceverai un credito suddiviso proporzionalmente alla data di fatturazione successiva.

**D:** Può un cliente spostare una sottoscrizione con fatturazione annuale da un partner a un altro?  

-   **R:** No. Le sottoscrizioni non possono essere spostate tra i partner. Il nuovo partner deve acquistare una nuova sottoscrizione per conto del cliente. Questo si applica alle sottoscrizioni fatturate mensilmente e annualmente.

**D:** Posso riattivare una sottoscrizione con la fatturazione annuale?

-   **R:** Sì, puoi riattivare la sottoscrizione entro 90 giorni dalla data di sospensione. Riceverai un addebito ripartito proporzionalmente alla data di fatturazione successiva. La data di rinnovo della sottoscrizione rimane invariata.

<a href="" id="pricingcalculation"></a>**Calcolo dei prezzi**

**D:** Cosa succede se il prezzo di un'offerta cambia parzialmente durante il periodo di 12 mesi di una sottoscrizione annuale fatturata?    

-   **R: **Il prezzo dell'offerta al momento dell'acquisto è garantito per tutto il periodo di validità della sottoscrizione di 12 mesi. 

**D:** Quale sarà il prezzo di una sottoscrizione quando viene rinnovata dopo il periodo di validità della sottoscrizione di 12 mesi?    

-   **R:** Quando una sottoscrizione viene rinnovata, il prezzo viene reimpostato in base al listino prezzi corrente alla data di rinnovo. Il nuovo prezzo è garantito per il successivo periodo di validità della sottoscrizione di 12 mesi.

**D:** Come viene calcolato il credito di una sottoscrizione o una licenza annullata? Viene calcolato al giorno o al mese?   

-   **R:** Il credito di annullamento viene calcolato come segue:

    - Credito per annullamento = ((prezzo mensile*12)/365) * giorni rimanenti del periodo di 12 mesi * numero di licenze annullate.

**D:** Cosa succede se il prezzo di un'offerta scende parzialmente durante il periodo di 12 mesi di una sottoscrizione annuale fatturata? 

-   **R:** Nessun cambiamento. Il prezzo è impostato per il periodo completo di 12 mesi. Lo stesso vale per la fatturazione mensile.


<a href="" id="reporting"></a>**Creazione di report**

**D:** Dove è indicato se un abbonamento è fatturato annualmente o mensilmente?   

-   **R:** Le informazioni sulla frequenza di fatturazione sono indicate nel file di riconciliazione basato su licenza. In particolare, nella colonna AA.

**D:** Quali cambiamenti vedrò nel file di riconciliazione basato su licenza quando un abbonamento con fatturazione annuale viene acquistato o rinnovato?  

-   **R: ** Il primo cambiamento sarà una nuova riga nel file di riconciliazione basato su licenza alla prima data di fatturazione successiva all'acquisto o a una nuova sottoscrizione. Se non vengono apportate modifiche alla sottoscrizione, non verrà visualizzata alcuna riga nei file di riconciliazione per i mesi da due a dodici del periodo di validità della sottoscrizione. Il secondo cambiamento del file di riconciliazione viene visualizzato quando la sottoscrizione viene rinnovata, alla prima data di fatturazione dopo il rinnovo. Se viene apportata una modifica alla sottoscrizione durante il periodo di validità di 12 mesi, verranno visualizzati un credito e una nuova fattura ripartita proporzionalmente nel successivo file di riconciliazione dopo la modifica.

**D:** In che modo l'acquisto, la modifica e l'annullamento di una sottoscrizione annuale vengono visualizzati nella colonna P dei file di utilizzo?

-   **R:** L'addebito di acquisto iniziale viene visualizzato come "Ripartizione delle tariffe all'acquisto". Le modifiche alle licenze che generano crediti e nuove fatture vengono visualizzate come "Ripartizione dell'istanza del ciclo". I crediti per annullamento vengono visualizzati come "Commissione per annullamento".

**D:** Quando viene annullata una sottoscrizione annuale, cosa viene indicato nel file di riconciliazione?   

-   **R: **Il file di riconciliazione conterrà una voce di credito per annullamento. Se l'annullamento avviene entro i primi 30 giorni del periodo di validità di 12 mesi, la sottoscrizione sarà accreditata al 100%. Se l'annullamento si verifica dopo i primi 30 giorni, la sottoscrizione verrà accreditata proporzionalmente.

**D: ** Cosa viene indicato nel file di riconciliazione quando le licenze vengono aggiunte a una sottoscrizione con fatturazione annuale?  

-   **R: **Il file di riconciliazione conterrà un credito e una nuova fattura ripartita proporzionalmente. Lo stesso vale per una sottoscrizione con fatturazione mensile.

**D: ** Cosa viene indicato nel file di riconciliazione quando le licenze vengono rimosse da una sottoscrizione con fatturazione annuale? 

-   **R: **Il file di riconciliazione conterrà un credito e una nuova fattura ripartita proporzionalmente.  Lo stesso vale per una sottoscrizione con fatturazione mensile.

**D:** Il prezzo annuale è indicato nel listino prezzi? 

-   **R:** No. Il prezzo di listino mostra il prezzo mensile. Puoi calcolare il prezzo annuale moltiplicando per dodici il prezzo mensile.

**D:** La matrice dell'offerta presenta voci diverse per le offerte che possono essere fatturate annualmente?   

-   **R:** No. Gli ID offerta sono uguali per tutte le frequenze di fatturazione. Non ci sono ID offerta univoci per la fatturazione annuale.


<a href="" id="incentives"></a>**Incentivi**

**D:** Con quale frequenza vengono calcolati gli incentivi sulle sottoscrizioni annuali? 

-   **R:** Calcoliamo gli incentivi sul ricavo fatturato. I pagamenti degli incentivi realizzati verranno visualizzati in base ai criteri disponibili nelle nostre guide agli incentivi CSP. 

**D:** Come vengono pagati gli incentivi sulle sottoscrizioni fatturate annualmente?  

-   **R:** Attualmente tutti i pagamenti degli incentivi vengono effettuati due volte l'anno. Questi pagamenti vengono effettuati 45 giorni dopo la fine del semestre.

**D:** Quando viene venduta una sottoscrizione fatturata annualmente, come vengono riconosciuti i ricavi della sottoscrizione per il calcolo degli incentivi? Il calcolo sarà basato sui ricavi fatturati o modificati? 

-   **R: **I calcoli degli incentivi si basano sul ricavo fatturato.

**D:** Come vengono calcolati gli utili degli incentivi per una sottoscrizione idonea fatturata annualmente tra le varie tariffe di incentivi CSP (tariffe di incentivi globali, tariffe di acceleratore locale e campagne locali)?

-   **R:** Indipendentemente dalla modalità di fatturazione della sottoscrizione, mensile o annuale, i partner guadagnano gli incentivi per tutte le transazioni idonee. Ciò include la tariffa di incentivi globale che viene applicata al ricavo fatturato per il periodo, l'acceleratore locale per tutte le aree geografiche in cui sono presenti acceleratori locali e qualsiasi campagna globale, ove applicabile.

**D:** Chi posso contattare per chiarimenti sugli incentivi?

-   **R:** È necessario contattare il team di supporto per gli incentivi regionali appropriati:

    - America del Nord: ocina@microsoft.com

    - America latina e Brasile: ocilatam@microsoft.com

    - EMEA: ociemea@microsoft.com

    - APOAC (escluso Giappone): ociapgc@microsoft.com

    - Giappone: ocijp@microsoft.com


**D:** Cosa accade se sospendo la mia sottoscrizione? 

-   **R:** Se sospendi una sottoscrizione nel Centro per i partner o mediante l'API, entro 30 giorni dall'acquisto, riceverai un credito al 100%, indipendentemente dalla frequenza di fatturazione. 

    Con la fatturazione annuale, il calcolo è simile al seguente:

    - Il partner acquista la sottoscrizione il 1 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/1-31/12.
    - Sospende la sottoscrizione il 25 gennaio = la riga di fatturazione accredito viene creata per il periodo di servizio 1/1-31/12.
    - Riattiva la sottoscrizione il 29 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/29-31/12.

    Con la fatturazione mensile, il calcolo è simile al seguente:

    - Il partner acquista la sottoscrizione il 1 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/1-31/1.
    - Sospende la sottoscrizione il 25 gennaio = la riga di fatturazione accredito viene creata per il periodo di servizio 1/1-31/1.
    - Riattiva la sottoscrizione il 29 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/29-31/1.



## <a href="" id="freetrialsfaq"></a>Domande frequenti sulle versioni di valutazione gratuite

**D1:** Cosa sono le versioni di valutazione gratuite?

-   **R:** Puoi offrire ai tuoi clienti una versione di valutazione gratuita di 30 giorni di alcuni prodotti che consente ai clienti di valutare il prodotto prima di acquistarlo. Le versioni di valutazione gratuite sono disponibili per i seguenti prodotti: 

    - Office 365 Business Premium (a partire dal 17 ottobre 2017)
    - Office 365 E3 (a partire dal 17 ottobre 2017)
    - Office 365 E5 con PSTN (a partire dal 17 ottobre 2017)
    - Office 365 E5 senza PSTN (a partire dal 17 ottobre 2017)
    - Enterprise Mobility & Security E5 (a partire dal 17 ottobre 2017)
    - Dynamics 365 Customer Engagement Piano 1 (a partire dal 17 ottobre 2017)
    - Dynamics 365 for Financials (a partire dal 17 ottobre 2017)
    - Microsoft 365 Business (a partire dal 1° marzo 2018)
    
**D2:** La fatturazione annuale e le versioni di valutazione gratuite sono diverse nel cloud di sovranità rispetto al cloud pubblico?

-   **R:** No. Sono uguali. L'unica differenza saranno le SKU della versione di valutazione disponibili al momento del lancio.

**D3:** Chi può partecipare?

-   **R:** Tutti i partner. Tuttavia, questa opzione non è attualmente disponibile in Cina. 

**D4:** Quali azioni devo intraprendere per essere idoneo e utilizzare queste versioni di valutazione gratuite?

-   **R:** Valuta in quale modo la versione di valutazione gratuita può essere incorporata nei movimenti di vendita e l'impatto nei tuoi processi interni. Potresti anche dovere modificare le API che usi per supportare la conversione di una versione di valutazione gratuita in una sottoscrizione a pagamento. Le specifiche tecniche dettagliate di queste modifiche API vengono pubblicate nella visualizzazione Annunci del Centro per i partner.

**D5:** Verrà visualizzata la versione di valutazione gratuita nel file di fattura e riconciliazione?

-   **R:** No, le versioni di valutazione gratuite non sono visualizzate nel file di riconciliazione basato su licenza o fattura. Verrà visualizzata nel file di riconciliazione basato su licenza e fattura dopo aver convertito una versione di valutazione gratuita in una sottoscrizione a pagamento. La sottoscrizione convertita verrà visualizzata nel file di riconciliazione basato su licenza e fattura come qualsiasi altra nuova sottoscrizione.

**D6:** Le versioni di valutazione gratuite hanno impatto sugli incentivi?

-   **R:** No. La versione di valutazione gratuita non ha alcun impatto sugli incentivi.

**D7:** Le versioni di valutazione gratuite saranno disponibili per prodotti Office aggiuntivi in futuro?

-   **R:** Offriamo le versioni di valutazione gratuite per questi prodotti perché sono le offerte aziendali più complete e popolari. È possibile che in futuro vengano aggiunte altre offerte di versioni di valutazione gratuite.

**D8:** Può un cliente avere più di una versione di valutazione gratuita?

-   **R:** Ogni cliente ha diritto a una versione di valutazione gratuita per ogni offerta disponibile.

**D9:** Sono previsti limiti per la versione di valutazione gratuita?

-   **R:** Sì. La versione di valutazione è per un massimo di 25 licenze. Il numero di licenze non può essere modificato durante il periodo di valutazione. Quando la versione di valutazione viene convertita in una sottoscrizione a pagamento, puoi aggiungere altre licenze alla sottoscrizione.

**D10:** La versione di valutazione gratuita viene automaticamente convertita in una sottoscrizione a pagamento?

-   **R:** No. Dovrai effettuare la conversione manuale della sottoscrizione, direttamente nel Centro per i partner o mediante l'API.

**D11:** È possibile utilizzare le versioni di valutazione gratuite per le sottoscrizioni fatturate mensilmente e annualmente?

-   **R:** Sì. Puoi scegliere la frequenza di fatturazione al momento della conversione della versione di valutazione in sottoscrizione a pagamento.

**D12:** La data di inizio della sottoscrizione si basa sulla data di inizio della versione di valutazione gratuita o sulla data di conversione in una sottoscrizione a pagamento? 

-   **R:** La data di inizio si basa sulla data della conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione annuale, la data di rinnovo della sottoscrizione cade 12 mesi dopo la data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione mensile, la data di rinnovo della sottoscrizione cade 12 mesi dopo la data di fatturazione successiva alla data di conversione.

**D13:** Possiamo aggiungere o rimuovere postazioni nella versione di valutazione gratuita?

-   **R:** No. Le versioni di valutazione gratuite avranno una quantità predefinita di 25 licenze e non possono essere aggiornate.

**D14:** Sono disponibili versioni di valutazione per le offerte di componenti aggiuntivi come ATP e PSTN?

-   **R:** Al momento non esistono versioni di valutazione gratuite per le offerte di componenti aggiuntivi.

**D15:** Posso fornire una versione di valutazione gratuita per un'offerta che il cliente già possiede?

-   **R:** No. Se l'offerta è già di proprietà del cliente non può essere utilizzata per una versione di valutazione gratuita.

**D16:** Potrò vedere tutte le offerte di versione di valutazione in sospeso?

-   **R:** Sì. Nella pagina dei clienti sono elencate tutte le sottoscrizioni. Sono incluse le sottoscrizioni delle versioni di valutazione gratuite e le sottoscrizioni a pagamento.

**D17:** L'utente riceverà la notifica di scadenza delle versioni di valutazione gratuite?

-   **R:** No. È possibile tenere traccia delle date di scadenza imminenti utilizzando la visualizzazione dei clienti nel Centro per i partner o eseguendo una query sull'API. È consigliabile monitorare le date di frequente in modo da poter intraprendere le azioni appropriate in relazione alla decisione dei clienti.

**D18:** Se un cliente ha ricevuto una versione di valutazione gratuita per un'offerta, può utilizzare un'altra versione di valutazione per un'offerta diversa? 

-   **R:** Sì. I clienti possono iscriversi a una versione di valutazione per ogni offerta. Ad esempio, possono ottenere una versione di valutazione gratuita per Office 365 Business Premium e una versione di valutazione gratuita per Office 365 E3.

**D19:** Cosa accade quando termina il periodo di valutazione? Io o il mio cliente riceveremo una notifica? Quali notifiche vengono visualizzate quando tento di accedere a una versione di valutazione scaduta?

-   **R:** Se un cliente tenta di accedere a una versione di valutazione scaduta verrà visualizzato un messaggio indicante che la versione di valutazione è scaduta. Non ci saranno notifiche per segnalare che una versione di valutazione sta per scadere, ma i partner possono tenere traccia della validità nella visualizzazione dei clienti o tramite le query all'API.

**D20:** È possibile estendere una versione di valutazione?

-   **R:** No. Dopo 30 giorni la versione di valutazione deve essere convertita o scadrà.

**D21:** Quando una versione di valutazione scade, le informazioni contenute nella versione di valutazione restano accessibili?

-   **R:** Sì. I dati vengono archiviati conformemente agli standard di conservazione dei dati. Dopo aver acquistato una nuova sottoscrizione con gli stessi piani di servizio, i dati del cliente sono accessibili dalla sottoscrizione appena attivata.

**D22:** Sono disponibili versioni di valutazione gratuite per offerte per enti pubblici e istituti di istruzione?

-   **R:** Non sono disponibili versioni di valutazione gratuite per offerte per enti pubblici e istituti di istruzione in questo momento.

**D23:** Le versioni di valutazione gratuite del cliente per il programma Cloud Solution Provider (CSP) possono essere convertite in altri tenant di programma, ad esempio EA, Open o MOSP? 

-   **R:** No. Le sottoscrizioni non possono essere trasferite da CSP a un altro programma.

**D24:** Come posso richiedere supporto per le versioni di valutazione gratuite? 

-   **R:** Invia una richiesta di servizio tramite il Centro per i partner.

## <a href="" id="billingalignmentfaq"></a>Allineamento della fatturazione - fine del periodo gratuito

A partire dal 21 febbraio 2018, il programma Cloud Solution Provider (CSP) inizierà l'implementazione dell'"allineamento della data di fatturazione" per le nuove sottoscrizioni con la frequenza di fatturazione mensile. Questo "allineamento della data di fatturazione" fornirà ai partner maggiore flessibilità e la prevedibilità per le vendite e la fatturazione e per il provisioning e la gestione degli abbonamenti dei clienti. 

**AGGIORNAMENTO DEL 23 FEBBRAIO:** in precedenza avevamo annunciato la data di implementazione del 20 febbraio, ma la nostra implementazione effettiva è stata leggermente ritardata e scaglionata per categoria di prodotto.  Per la data di implementazione per categoria di prodotto, vedere la seguente tabella. 

|**Categoria di prodotti**   |**Giorno di implementazione**   |
|-----------------|:-------------|
|Office  |21 febbraio   |
|Windows, Minecraft   |22 febbraio   |
|Office 365 (Cina)   |23 febbraio   |
|Dynamics/Intune   |23 febbraio   |

Le sottoscrizioni acquistate prima della data di implementazione (vedi la tabella sopra) ottengono un periodo gratuito dalla data di acquisto alla data di fatturazione del partner. Gli abbonamenti acquistati dopo la data di implementazione non riceveranno più il periodo gratuito. Il periodo di 12 mesi a pagamento inizia (viene allineato) alla data di acquisto rispetto alla fatturazione del partner. I partner non vedranno più la "riga di fatturazione a $0" che rappresenta il periodo gratuito nel file di riconciliazione. Non sono state apportate modifiche alle API, alla fatturazione o agli incentivi.  I partner devono informare i team di vendita e contabilità di questa nuova logica di fatturazione e assicurarsi che le operazioni vengano modificate di conseguenza.  

Prima di implementare l'allineamento della data di fatturazione, abbiamo fatturato e addebitato alla data dell'anniversario della fatturazione del partner, ossia la data in cui il partner si è registrato al programma CSP, e non alla data dell'anniversario della sottoscrizione del cliente, ossia la data in cui il cliente ha acquistato la sottoscrizione. Dopo la data di implementazione, i partner riceveranno l'addebito alla data dell'anniversario della sottoscrizione, eliminando questo periodo gratuito.  I partner continueranno a ricevere le fatture alla data dell'anniversario di fatturazione, ma la data di validità della fattura sarà data dell'anniversario della sottoscrizione del cliente. 

Le sottoscrizioni che sono nel periodo gratuito alla data di implementazione, non riceveranno l'addebito tra la data di acquisto e la data di fatturazione del partner. Inoltre, non riceveranno l'addebito per il primo mese del termine di pagamento di 12 mesi. Se usi un file di riconciliazione per la verifica, tieni presente che questo addebito del primo mese non sarà più visibile nel file di riconciliazione.  

**D1:** Cosa cambia per la data di fatturazione?

-   **R:** Le sottoscrizioni basate su licenza non avranno più un periodo gratuito. Attualmente, il periodo gratuito decorre dalla data di acquisto alla data di fatturazione del partner.

**D2:** Quando verrà rimosso il periodo gratuito?

- **R:** A partire dalle date di implementazione elencate nella tabella seguente, le nuove sottoscrizioni non riceveranno un periodo gratuito.

|**Categoria di prodotti**   |**Giorno di implementazione**   |
|-----------------|:-------------|
|Office  |21 febbraio   |
|Windows, Minecraft   |22 febbraio   |
|Office 365 (Cina)   |23 febbraio   |
|Dynamics/Intune   |23 febbraio   |

**D3:** Quale sarà l'impatto sulle sottoscrizioni nel periodo gratuito alla data di implementazione?

- **R:** Le sottoscrizioni che si trovano nel periodo gratuito alla data di implementazione riceveranno comunque un periodo gratuito dalla data di acquisto alla data di fatturazione del partner. Queste licenze riceveranno anche un "periodo gratuito esteso" e non verrà addebitato il primo mese del termine di pagamento di 12 mesi. Il "periodo gratuito esteso" non sarà applicabili alle licenze aggiunte nel primo mese. Se aumenti la quantità di licenze nel primo mese, ti verranno addebitate le licenze aggiunte alla successiva fattura/riconciliazione. Se il file di riconciliazione viene utilizzato per la verifica, tieni presente che l'addebito del primo mese potrebbe non essere presente nel file di riconciliazione. Vedi gli scenari seguenti per una spiegazione più dettagliata.

**D4:** Quando inizierà il periodo a pagamento di 12 mesi per una nuova sottoscrizione?

- **R:** Attualmente, il periodo a pagamento decorre dalla data di fatturazione del partner dopo la data di acquisto. Dalla data di implementazione il periodo a pagamento per le nuove sottoscrizioni inizierà alla data di acquisto.

**D5:** Quando vengono rinnovate automaticamente le sottoscrizioni?

- **R:** Le sottoscrizioni vengono rinnovate automaticamente 12 mesi dopo la prima data di fatturazione. Attualmente, le sottoscrizioni si rinnovano automaticamente 12 mesi dopo la prima data di fatturazione del partner dopo la data di acquisto. Dalla data di implementazione le nuove sottoscrizioni vengono rinnovate automaticamente 12 mesi dopo la data di acquisto.

**D6:** Cosa succede se acquisto la sottoscrizione nei giorni 29, 30 o 31 di un mese?

- **R:** La sottoscrizione sarà disponibile dalla data di acquisto, ma il termine a pagamento di 12 mesi non inizia fino al primo giorno del mese successivo.

**D7:** Quali offerte sono interessate?

- **R:** La rimozione del periodo gratuito si applica a tutte le sottoscrizioni basate su licenza CSP.

**D8:** In che modo è interessato il file di fatturazione e riconciliazione? 

- **R:** Non vedrai più la "riga di fatturazione a $0" nella fattura o nel file di riconciliazione. Attualmente, la riga di fatturazione a 0$ rappresenta il periodo gratuito.

**D9:** La data di fatturazione cambia?

- **R:** No, continuerai a ricevere il file di fatturazione e riconciliazione alla data di fatturazione esistente.

**D10 :** Le date di inizio e fine addebito mensile cambiano per le sottoscrizioni esistenti?

- **R:** No, le date di inizio e fine addebito mensile di una sottoscrizione esistente continueranno a essere allineate alla data di fatturazione. Tuttavia, le nuove sottoscrizioni saranno allineate alla data di acquisto. Vedi l'esempio seguente.

**D11:** Il calcolo degli incentivi cambia?

- **R:** No, non è stata apportata alcuna modifica al calcolo degli incentivi.

**D12:** Le API subiranno cambiamenti?

- **R:** No, non è stata apportata alcuna modifica alle API.

### <a name="common-scenarios"></a>Scenari comuni


|**Scenari**   |**Scenario 1: il periodo di sottoscrizione gratuito termina prima della data di implementazione**   |**Scenario 2: la sottoscrizione si trova nel periodo gratuito alla data di implementazione**  | **Scenario 3: la sottoscrizione è stata acquistata in corrispondenza o dopo la data di implementazione**   |
|----------|:------------|:--------------------|:------------|
|Data di acquisto |1 febbraio 2018    | 1 febbraio 2018    | 1 giugno 2018     |
|Data del provisioning | 1 febbraio 2018   |1 febbraio 2018   |1 giugno 2018   |
|Data di fatturazione   | 15 di ogni mese   |25 di ogni mese   | 15 di ogni mese|
|Periodo gratuito   | 1 febbraio 2018 - 14 febbraio 2018|1 febbraio 2018 - 24 febbraio 2018   |Nessun periodo gratuito|
|Addebito di 1 mese   | 15 febbraio 2018 - 14 marzo 2018 | La quantità di licenze il 24 febbraio 2018 riceverà un periodo gratuito esteso fino al 24 marzo 2018. Le licenze aggiunte dopo 24 febbraio 2018 verranno addebitate. |1 giugno 2018 - 30 giugno 2018   |
|Addebito di 2 mesi   | 15 marzo 2018 - 14 aprile 2018|25 marzo 2018 - 24 aprile 2018   |1 luglio 2018 - 31 luglio 2018|
|Inizia il periodo a pagamento   | 15 febbraio 2018 | 25 febbraio 2018| 1 giugno 2018| 
|Finisce il periodo a pagamento | 14 febbraio 2019   |24 febbraio 2019   | 31 maggio 2019  |
|Data del rinnovo | 15 febbraio 2019 |25 febbraio 2019   |1 giugno 2019|

### <a name="scenario-4---new-purchase"></a>Scenario 4: nuovo acquisto

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. 

Il 15 giugno il file di riconciliazione conterrà solo le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Scenario 5a: sospendere e riattivare prima della data di fatturazione

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 5 giugno 2018, il partner sospende la sottoscrizione. Il 10 giugno 2018, il partner riattiva la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 
- Credito per annullamento -$30 per periodo di servizio 5 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni. 
- Addebito di $30 per periodo di servizio 10 giugno - 30 giugno. L'addebito non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |
|5/6/2018   |30/6/2018   |-$30   |1   |$30   |Commissione di annullamento |
|10/6/2018   |30/6/2018   |$30   |1   |$30   |Commessione di attivazione |

Quando una sottoscrizione viene sospesa e riattivata, la data di rinnovo automatico rimarrà 12 mesi dopo la data di acquisto originale.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scenario 5b: sospendere e riattivare dopo la data di fatturazione ma prima di 30 giorni dalla data di acquisto

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 20 giugno 2018, il partner sospende la sottoscrizione. Il 25 giugno 2018, il partner riattiva la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Credito per annullamento -$30 per periodo di servizio 20 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 25 giugno - 30 giugno. L'addebito non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/6/2018   |30/6/2018   |-$30   |1   |-$30   |Commissione di annullamento |
|25/6/2018   |30/6/2018   |$30   |1   |$30   |Commessione di attivazione |
|1/7/2018   |31/7/2018   |$30   |1   |$30   |Tariffa periodica |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scenario 5c: sospendere e riattivare (differente quantità di licenze) dopo la data di fatturazione ma prima di 30 giorni dalla data di acquisto

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 20 giugno 2018, il partner sospende la sottoscrizione. Il 25 giugno 2018, il partner riattiva la sottoscrizione con due licenze. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Credito per annullamento -$30 per periodo di servizio 20 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 25 giugno - 30 giugno. L'addebito di riattivazione non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni. L'addebito è anche in base alla quantità di licenze originali, ovvero 1.
- Credito -$6 per periodo di servizio 25 giugno - 30 giugno. L'addebito di riattivazione è stato effettuato solo per 1 licenza durante il periodo di servizio 25 giugno - 30 giugno, quando si disponeva di 2 licenze. Il credito di $6 annulla l'addebito non corretto per il servizio di servizio 25 giugno - 30 giugno.
- Nuova fattura di $12 ripartita proporzionalmente per periodo di servizio 25 giugno - 30 giugno. Il partner aveva 2 licenze durante questo periodo di servizio. Il prezzo unitario viene calcolato come (30/30)*6*2 = $12.
- Addebito di $60 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/6/2018   |30/6/2018   |-$30   |1   |-$30   |Commissione di annullamento |
|25/6/2018   |30/6/2018   |$30   |1   |$30   |Commissione di attivazione |
|25/6/2018   |30/6/2018   |-$6   |1   |-$6   |Istanza del ciclo rateizzata |
|25/6/2018   |30/6/2018   |$6   |2   |$12   |Istanza del ciclo rateizzata |
|1/7/2018   |31/7/2018   |$30   |2   |$60   |Tariffa periodica |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Scenario 6: sospendere una sottoscrizione entro 30 giorni dall'acquisto e riattivarla oltre 30 giorni dopo l'acquisto 

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Il 5 giugno, il partner sospende la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno
- Credito per annullamento -$30 per periodo di servizio 5 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto
|5/6/2018   |30/6/2018   |-$30   |1   |-$30   |Commissione di annullamento

Il 10 luglio, il partner riattiva la sottoscrizione. Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito per riattivazione di $21,30 per periodo di servizio 10 luglio - 31 luglio. Le riattivazioni dopo 30 giorni dalla data di acquisto generano un addebito ripartito proporzionalmente. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/7/2018   |31/7/2018   |$21,30   |1   |$21,30   |Commessione di attivazione |

Il 15 agosto il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Addebito di $30 per il periodo di servizio 1 agosto - 31 agosto.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/8/2018   |31/8/2018   |$30   |1   |$30   |Tariffa periodica |

Quando una sottoscrizione viene sospesa e riattivata, la data di rinnovo automatico rimarrà 12 mesi dopo la data di acquisto originale. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Scenario 7: sospendere e riattivare una sottoscrizione dopo 30 giorni dall'acquisto 
La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. 

Il 15 giugno il file di riconciliazione conterrà solo le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il partner sospende la sottoscrizione il 5 luglio, ma la riattiva il 15 luglio. Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio.
- Credito per annullamento -$26,14 per periodo di servizio 5 luglio - 31 luglio. Gli annullamenti dopo 30 giorni dalla data di acquisto generano un credito ripartito proporzionalmente. Calcolo = (prezzo mensile/giorni nel periodo totale di servizio) x giorni nel periodo di servizio ripartito x quantità di licenze x (-1) (30/31) x 27 x 1 x (-1) = -26,14.
- Addebito per riattivazione di $21,30 per periodo di servizio 10 luglio - 31 luglio. Le riattivazioni dopo 30 giorni dalla data di acquisto generano un addebito ripartito proporzionalmente. Calcolo = (30/31) x 22 x 1 = 21,30.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/7/2018   |31/7/2018   |$30  |1   |$30   |Tariffa periodica |
|5/7/2018   |31/7/2018   |   -$26,14   |1   |-$26,14|Commissione di annullamento |
|10/7/2018   |31/7/2018   |-$21,30   |1   |$21,30|Commessione di attivazione |

Il file di riconciliazione del 15 agosto conterrà le seguenti righe:
- Addebito di $30 per il periodo di servizio 1 agosto - 31 agosto.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/8/2018   |31/8/2018   |$30  |1   |$30   |Tariffa periodica |

### <a name="scenario-8-change-of-license-quantity"></a>Scenario 8: modificare la quantità di licenze 

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione per $30 al mese. Il 10 giugno il partner aumenta la quantità di licenze da 1 a 2 licenze. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. Anche se il partner ha aumentato la quantità di licenze prima della data di fatturazione del 15 giugno, la modifica non verrà riconosciuta nel sistema di fatturazione Microsoft fino al giorno dell'anniversario della sottoscrizione del 1 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 1 luglio, giorno dell'anniversario della sottoscrizione, il sistema di fatturazione Microsoft riconoscerà che il 10 giugno la quantità di licenze è stata modificata da 1 a 2. Il sistema di fatturazione genererà un credito e una nuova fattura ripartita proporzionalmente per il periodo di servizio 1 giugno - 9 giugno e 10 giugno - 30 giugno. 

Il file di riconciliazione del 15 luglio conterrà le seguenti righe:

- Credito -$30 per periodo di servizio 1 giugno - 30 giugno.
- Nuova fattura ripartita proporzionalmente $9 per periodo di servizio 1 giugno - 9 giugno. Questo è il periodo quando il cliente aveva 1 licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (30/30) x 9 x 1 = 9.
- Nuova fattura ripartita proporzionalmente $42 per periodo di servizio 10 giugno - 30 giugno. Questo è il periodo quando il cliente aveva 2 licenze. Calcolo = (30/30) x 21 x 2 = 42.
- Addebito di $60 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/6/2018   |-$30   |1   |-$30|Istanza del ciclo rateizzata |
|1/6/2018   |9/6/2018   |$9   |1   |$9|Istanza del ciclo rateizzata |
|10/6/2018   |30/6/2018   |$21   |2   |$42|Istanza del ciclo rateizzata |
|1/7/2018   |31/7/2018   |$30   |2   |$60   |Tariffa periodica |

### <a name="scenario-9-add-on-subscriptions"></a>Scenario 9: sottoscrizioni di componenti aggiuntivi

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Il 10 giugno il partner acquista una nuova sottoscrizione per componente aggiuntivo per $5 al mese. La data di rinnovo della sottoscrizione per componente aggiuntivo si allinea alla data di rinnovo della sottoscrizione di base che è il 1 giugno. 

Il 10 giugno il partner acquista una sottoscrizione per componente aggiuntivo di una licenza per $5 al mese. 

Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. È per la sottoscrizione di base.
- Addebito ripartito proporzionalmente $3,50 per periodo di servizio 10 giugno - 30 giugno. È per la sottoscrizione per componente aggiuntivo. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/6/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |
|10/6/2018   |30/6/2018   |$3,50   |1   |$3,50   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio. È per la sottoscrizione di base.
- Addebito di $5 per periodo di servizio 1 luglio - 31 luglio. È per la sottoscrizione per componente aggiuntivo.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|1/7/2018   |31/7/2018   |$30   |1   |$30   |Tariffa periodica |
|1/7/2018   |31/7/2018   |$5   |1   |$5   |Tariffa periodica |

La data di rinnovo automatico della sottoscrizione per componente aggiuntivo sarà il 1 giugno 2019, allineata alla sottoscrizione di base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Scenario 10: nuovo acquisto il 29, il 30 o il 31 

La data di fatturazione del partner è il 15 del mese. Il 29 maggio il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Le sottoscrizioni acquistate il 29, il 30 o il 31 avranno un periodo gratuito dalla data dell'acquisto fino al 1 del mese successivo. Il giorno di anniversario della sottoscrizione sarà il giorno 1 per impostazione predefinita. In questo scenario, la sottoscrizione riceverà un periodo gratuito dal 29 maggio al 31 maggio e il periodo a pagamento di 12 mesi inizierà il 1 giugno. 

Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantità**   |**Importo**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/05/2018   | 30/06/2018   |$30   |1   |$30  |Rateizza le tariffe all'acquisto |

Il rinnovo automatico della sottoscrizione avverrà il 1 giugno 2019.
