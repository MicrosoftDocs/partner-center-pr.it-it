---
title: Domande frequenti sulle nuove funzionalità di fatturazione | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
Description: Di seguito sono riportate le domande frequenti su fatturazione annuale del Centro per i partner e funzionalità della versione di valutazione gratuita.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: d595c05adac5ffc57a52d8635abf80cb0b3f375d
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820315"
---
# <a name="faq-about-new-billing-features"></a>Domande frequenti sulle nuove funzionalità di fatturazione

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government


Di seguito sono riportate le domande frequenti su fatturazione annuale del Centro per i partner e funzionalità della versione di valutazione gratuita. 

## <a name="in-this-section"></a>Contenuto della sezione

-   [Domande frequenti sulla fatturazione annuale](#annualbillingfaq)

-   [Domande frequenti sulle versioni di valutazione gratuite](#freetrialsfaq)

-   [Domande frequenti sull'allineamento di fatturazione](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Domande frequenti sulla fatturazione annuale

Sezioni:

[Panoramica e vantaggi della fatturazione annuale](#overviewandbenefits)

[Posizionamento degli scenari di ordine e fatturazione](#placingyourorder)

[Modifica della sottoscrizione](#changingyoursubscription)

[Calcolo dei prezzi](#pricingcalculation)

[Reporting](#reporting)

[Incentivi](#incentives)


<a href="" id="overviewandbenefits"></a>**Panoramica e vantaggi della fatturazione annuale**

**D** Cosa è cambiato?

-   **R:** In risposta alle tue richieste, abbiamo introdotto la possibilità di pagare per alcune sottoscrizioni CSP su base annuale o mensile. Questa nuova opzione è diventata disponibile il 17 ottobre 2017.

**D** Chi può partecipare?

-   **R:** Tutti i partner e i tipi di partner possono avvalersi della fatturazione annuale. La fatturazione annuale è disponibile in tutti i mercati in cui è attualmente disponibile il CSP. 

**D** Cosa è necessario prendere in considerazione quando si pensa alla fatturazione annuale?    

-   **R:** È necessario valutare il modo in cui verrà influenzato il movimento delle vendite. Ecco alcuni suggerimenti che ti consentono di utilizzare al meglio la fatturazione annuale. 
    - Aggiorna le API per la funzionalità di fatturazione annuale, se applicabile. 
    - Rivedi le modifiche nel file di fatturazione e riconciliazione basato su licenza.
    - Assicurati che il team sia informato.
    - Aggiorna i processi interni in base alle esigenze.

**D** Quali sono i vantaggi della fatturazione annuale? 

-   **R:** La fatturazione annuale presenta i vantaggi seguenti:

    - Maggiore flessibilità nelle opzioni di pagamento.

    - Migliore allineamento con la fatturazione dei clienti.

    - Impatto ridotto delle fluttuazioni di valuta.

    - Costi operativi di fatturazione ridotti.

**D** Quali offerte avranno l'opzione per la fatturazione annuale?

-   **R:** Per la maggior parte delle sottoscrizioni basate su licenza è possibile utilizzare l'opzione di fatturazione mensile o annuale. Le sottoscrizioni basate su utilizzo hanno solo l'opzione di fatturazione mensile. La colonna J della matrice dell'offerta identifica le frequenze di fatturazione disponibili per ogni offerta. La matrice dell'offerta è disponibile nella sezione "Vedere offerte e prezzi" nel Centro per i partner. .

**D** Fatturazione annuale per sottoscrizione o licenza?       

-   **R:** La fatturazione annuale e mensile è per sottoscrizione.

**D** Sono necessarie modifiche alle API per supportare la fatturazione annuale?    

-   **R:** Per sfruttare la fatturazione annuale, è necessario apportare alcune modifiche alle API. Puoi trovare informazioni più dettagliate negli articoli seguenti:

    - https://partnercenter.microsoft.com/partner/developer

    - https://msdn.microsoft.com/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Codice di esempio: https://msdn.microsoft.com/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Posizionamento degli scenari di ordine e fatturazione**

**D** Sarà disponibile un'offerta univoca in modo specifico per gli ordini con fatturazione annuale?   

-   **R:** No. La frequenza di fatturazione, inclusa l'opzione di fatturazione annuale è assegnata all'offerta come attributo. Tuttavia puoi rinominare un'offerta con un nome descrittivo per il cliente per consentire la differenziazione.

**D** Ricerca per categorie selezionare fatturazione annuale?

-   **R:** Quando si aggiunge una nuova sottoscrizione, verrà richiesto di scegliere la frequenza di fatturazione. A questo punto puoi scegliere l'opzione di fatturazione annuale. Dopo aver selezionato la fatturazione annuale, verranno visualizzate tutte le offerte disponibili.

**D** Se scelgo la fatturazione annuale quando verrà fatturato?    

-   **R:** Ti verrà addebitato il costo della prossima data di fatturazione. Ad esempio, se la data di fatturazione è il 1° del mese e tu acquisti una sottoscrizione con fatturazione annuale il 29 ottobre 2017, la fattura verrà emessa il 1° novembre 2017. Supponendo che non apporti alcuna modifica alla licenza, la fattura verrà emessa il 1° novembre 2018. Se apporti una modifica alla licenza, riceverai un credito e una nuova fattura alla data di fatturazione successiva. 

**D** È possibile suddividere una sottoscrizione in modo che una parte venga fatturata mensilmente e l'altra venga fatturata annualmente?  

-   **R:** No. L'intera sottoscrizione deve avere la stessa frequenza di fatturazione. L'intera sottoscrizione deve avere la fatturazione mensile o annuale.

**D** Quando il rinnovo per la sottoscrizione al è con fatturazione annuale?     

-   **R:** La data di rinnovo sarà di dodici mesi dopo la data di inizio del servizio. Il periodo del servizio inizia il giorno in cui viene creata la sottoscrizione.  Ad esempio, una sottoscrizione creata il 10 gennaio 2018 si rinnova il 10 gennaio 2019.

**D** Quando verrà addebitato il rinnovo di una sottoscrizione con fatturazione annuale? 

-   **R:** Il costo verrà addebitato alla data di fatturazione successiva dopo la data di rinnovo della sottoscrizione. Ad esempio, se acquisti una sottoscrizione con fatturazione annuale addebitata il 15 gennaio 2018 e la data di fatturazione è 20 gennaio, la sottoscrizione verrà rinnovata il 15 gennaio 2019. La fattura per il rinnovo verrà addebitata il 20 gennaio 2019.

**D** Le sottoscrizioni con fatturazione annuale ricevono un periodo gratuito?

-   **R:** No, le sottoscrizioni con frequenza di fatturazione annuale non ricevono un periodo gratuito. Il termine di pagamento di 12 mesi inizia dalla data di acquisto. Diversamente dalle sottoscrizioni con fatturazione mensile che invece prevedono un periodo gratuito a partire dalla data di acquisto fino alla successiva data di fatturazione.

**D** Un cliente può avere più sottoscrizioni della stessa offerta ognuna con frequenze di fatturazione diverse?    

-   **R:** Dipende dall'offerta. Alcune offerte sono limitate a una sottoscrizione per cliente. Se l'offerta non è limitata, un cliente può avere più sottoscrizioni della stessa offerta con frequenze di fatturazione diverse. Puoi trovare i dettagli di tutti i limiti e le restrizioni delle offerte nella colonna I della matrice dell'offerta. La matrice dell'offerta è disponibile nella sezione "Vedere offerte e prezzi" nel Centro per i partner.

<a href="" id="changingyoursubscription"></a>**Modifica della sottoscrizione**

**D** È possibile aggiungere una nuova licenza a una sottoscrizione esistente con fatturazione annuale?    

-   **R:** Sì. Puoi modificare la quantità di licenze per le sottoscrizioni in qualsiasi momento. L'aggiunta di ulteriori licenze non influirà sulla frequenza di fatturazione. 

**D** È possibile aggiungere licenze con fatturazione mensile a una sottoscrizione esistente con fatturazione annuale? 

-   **R:** Una volta acquistata una sottoscrizione con fatturazione annuale, eventuali licenze aggiuntive seguiranno la stessa frequenza di fatturazione. Se quindi devi acquistare licenze con fatturazione mensile, devi acquistare una nuova sottoscrizione.

**D** È possibile impostare la frequenza di fatturazione per una sottoscrizione da mensile a annuale e viceversa? 

-   **R:** Sì. **Per modificare la frequenza di fatturazione di un servizio online** , vedere Nozioni di [base sulla fatturazione](https://docs.microsoft.com/partner-center/billing-basics).

**D** La fatturazione annuale è disponibile per le offerte per i componenti aggiuntivi?   

-   **R:** Sì. La sottoscrizione del componente aggiuntivo avrà automaticamente la stessa frequenza di fatturazione della sottoscrizione padre.

**D** Come funziona la fatturazione annuale quando si aggiungono o rimuovono le licenze? 

-   **R:** È possibile aggiungere o rimuovere licenze in qualsiasi momento. Riceverai un credito e una nuova fattura ripartita proporzionalmente alla data di fatturazione successiva dopo aver cambiato il numero di licenze. 

**D** Cosa accade se si annulla una sottoscrizione con un lavoro di fatturazione annuale?    

-   **R:** I criteri di annullamento sono gli stessi per tutte le frequenze di fatturazione. Se la sottoscrizione viene annullata entro 30 giorni dal termine di pagamento di 12 mesi, riceverai un credito del 100% alla data di fatturazione successiva. Se la sottoscrizione viene annullata dopo 30 giorni dal termine di pagamento di 12 mesi, riceverai un credito suddiviso proporzionalmente alla data di fatturazione successiva.

**D** Un cliente può spostare una sottoscrizione con una fatturazione annuale da un partner a un altro partner?  

-   **R:** No. Le sottoscrizioni non possono essere spostate tra i partner. Il nuovo partner deve acquistare una nuova sottoscrizione per conto del cliente. Questo si applica alle sottoscrizioni fatturate mensilmente e annualmente.

**D** È possibile riattivare una sottoscrizione con fatturazione annuale?

-   **R:** Sì, è possibile riattivare la sottoscrizione per un massimo di 90 giorni dalla data di sospensione. Riceverai un addebito ripartito proporzionalmente alla data di fatturazione successiva. La data di rinnovo della sottoscrizione rimane invariata.

<a href="" id="pricingcalculation"></a>**Calcolo dei prezzi**

**D** Cosa accade se il prezzo di un'offerta viene modificato nel corso del periodo di 12 mesi di una sottoscrizione fatturata annualmente?    

-   **R:** Il prezzo dell'offerta al momento dell'acquisto è garantito per l'intero periodo di validità della sottoscrizione di 12 mesi. 

**D** Qual è il prezzo di una sottoscrizione al momento del rinnovo automatico dopo un periodo di validità di 12 mesi?    

-   **R:** Quando una sottoscrizione viene rinnovata, il prezzo sarà basato sull'elenco prezzi corrente alla data del rinnovo. Il nuovo prezzo è garantito per il successivo periodo di validità della sottoscrizione di 12 mesi.

**D** Come viene calcolato il credito per una licenza o una sottoscrizione annullata? Viene calcolato al giorno o al mese?   

-   **R:** Il credito di annullamento viene calcolato come segue:

    - Credito per annullamento = ((prezzo mensile*12)/365) * giorni rimanenti del periodo di 12 mesi * numero di licenze annullate.

**D** Cosa accade se il prezzo di un'offerta diminuisce durante il periodo di 12 mesi di una sottoscrizione fatturata annualmente? 

-   **R:** Non sono state apportate modifiche. Il prezzo è impostato per il periodo completo di 12 mesi. Lo stesso vale per la fatturazione mensile.


<a href="" id="reporting"></a>**Reporting**

**D** Dove è possibile sapere se una sottoscrizione viene fatturata annualmente o mensilmente?   

-   **R:** Il file di riconciliazione basato su licenza includerà le informazioni sulla frequenza di fatturazione. In particolare, nella colonna AA.

**D** Quali modifiche vengono visualizzate nel file di riconciliazione basato su licenza quando viene acquistata o rinnovata una sottoscrizione con fatturazione annuale?  

-   **R:** La prima modifica sarà una nuova riga nel file di riconciliazione basato su licenza alla prima data di fatturazione dopo l'acquisto o una nuova sottoscrizione. sottoscrizione. Se non vengono apportate modifiche alla sottoscrizione, non verrà visualizzata alcuna riga nei file di riconciliazione per i mesi da due a dodici del periodo di validità della sottoscrizione. Il secondo cambiamento del file di riconciliazione viene visualizzato quando la sottoscrizione viene rinnovata, alla prima data di fatturazione dopo il rinnovo. Se viene apportata una modifica alla sottoscrizione durante il periodo di validità di 12 mesi, verranno visualizzati un credito e una nuova fattura ripartita proporzionalmente nel successivo file di riconciliazione dopo la modifica.

**D** In che modo l'acquisto, la modifica o l'annullamento di una sottoscrizione annuale viene visualizzato nella colonna P dei file di utilizzo?

-   **R:** L'addebito per l'acquisto iniziale viene visualizzato come "tariffe propagate al momento dell'acquisto". Le modifiche alle licenze che generano crediti e nuove fatture vengono visualizzate come "Ripartizione dell'istanza del ciclo". I crediti per annullamento vengono visualizzati come "Commissione per annullamento".

**D** Quando viene annullata una sottoscrizione annuale, come viene visualizzata nel file di riconciliazione?   

-   **R:** Il file di riconciliazione conterrà una voce per un credito di annullamento. Se l'annullamento avviene entro i primi 30 giorni del periodo di validità di 12 mesi, la sottoscrizione sarà accreditata al 100%. Se l'annullamento si verifica dopo i primi 30 giorni, la sottoscrizione verrà accreditata proporzionalmente.

**D** Come viene visualizzato nel file di riconciliazione se le licenze vengono aggiunte a una sottoscrizione con fatturazione annuale?  

-   **R:** Il file di riconciliazione conterrà un credito e una fatturazione rivalutata. Lo stesso vale per una sottoscrizione con fatturazione mensile.

**D** Come appare Lion il file di riconciliazione se le licenze vengono rimosse da una sottoscrizione con fatturazione annuale? 

-   **R:** Il file di riconciliazione conterrà un credito e una fatturazione rivalutata.  Lo stesso vale per una sottoscrizione con fatturazione mensile.

**D** Il prezzo annuo è indicato nell'elenco prezzi? 

-   **R:** No. Il prezzo di listino mostra il prezzo mensile. Puoi calcolare il prezzo annuale moltiplicando per dodici il prezzo mensile.

**D** La matrice di offerte ha voci diverse per le offerte che possono essere fatturate annualmente.   

-   **R:**  No. Gli ID offerta sono uguali per tutte le frequenze di fatturazione. Non ci sono ID offerta univoci per la fatturazione annuale.


<a href="" id="incentives"></a>**Incentivi**

**D** Con quale frequenza vengono calcolati gli incentivi sulle sottoscrizioni annuali? 

-   **R:** Calcoliamo sui ricavi fatturati. I pagamenti degli incentivi realizzati verranno visualizzati in base ai nostri criteri disponibili nelle nostre guide agli incentivi CSP. 

**D** In che modo vengono pagati gli incentivi per le sottoscrizioni fatturate annualmente?  

-   **R:** Attualmente tutti i pagamenti incentive vengono eseguiti due volte all'anno. Questi pagamenti vengono effettuati 45 giorni dopo la fine del semestre.

**D** Quando viene venduta una sottoscrizione fatturata annualmente, in che modo verranno riconosciuti i ricavi della sottoscrizione per il calcolo degli incentivi. Il calcolo sarà basato sui ricavi fatturati o modificati? 

-   **R:** I calcoli degli incentivi sono basati sui ricavi fatturati.

**D:** Come vengono calcolati gli utili degli incentivi per una sottoscrizione idonea fatturata annualmente tra le varie tariffe di incentivi CSP (tariffe di incentivi globali, tariffe di acceleratore locale e campagne locali)?

-   **R:** Indipendentemente dalla fatturazione di una sottoscrizione, mensile o annuale, i partner ottengono incentivi per tutte le transazioni idonee. Ciò include la tariffa di incentivi globale che viene applicata al ricavo fatturato per il periodo, l'acceleratore locale per tutte le aree geografiche in cui sono presenti acceleratori locali e qualsiasi campagna globale, ove applicabile.

**D** Chi può contattare per eventuali domande sugli incentivi?

- **R:** Contattare il team di supporto tecnico per gli incentivi regionali appropriati:

  - America del Nord: ocina@microsoft.com

  - America latina e Brasile: ocilatam@microsoft.com

  - EMEA: ociemea@microsoft.com

  - APOAC (escluso Giappone): ociapgc@microsoft.com

  - Giappone: ocijp@microsoft.com


**D** Cosa accade se si sospende la sottoscrizione? 

-   **R:** Se si sospende una sottoscrizione, nel centro per i partner o tramite l'API, entro 30 giorni dall'acquisto, si riceverà un credito del 100%, indipendentemente dalla frequenza di fatturazione. 

    Con la fatturazione annuale, il calcolo è simile al seguente:

    - Il partner acquista la sottoscrizione il 1 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/1-31/12.
    - Sospende la sottoscrizione il 25 gennaio = la riga di fatturazione accredito viene creata per il periodo di servizio 1/1-31/12.
    - Riattiva la sottoscrizione il 29 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/29-31/12.

    Con la fatturazione mensile, il calcolo è simile al seguente:

    - Il partner acquista la sottoscrizione il 1 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/1-31/1.
    - Sospende la sottoscrizione il 25 gennaio = la riga di fatturazione accredito viene creata per il periodo di servizio 1/1-31/1.
    - Riattiva la sottoscrizione il 29 gennaio = la riga di fatturazione addebito viene creata per il periodo di servizio 1/29-31/1.



## <a href="" id="freetrialsfaq"></a>Domande frequenti sulle versioni di valutazione gratuite

**Q1** Che cosa sono le versioni di valutazione gratuite?

-   **R:** È possibile offrire ai clienti una versione di valutazione gratuita di 30 giorni di determinati prodotti. In questo modo i clienti possono valutare il prodotto prima di acquistarlo. Le versioni di valutazione gratuite sono disponibili per i seguenti prodotti: 

    - Office 365 Business Premium (a partire dal 17 ottobre 2017)
    - Office 365 E3 (a partire dal 17 ottobre 2017)
    - Office 365 E5 con PSTN (a partire dal 17 ottobre 2017)
    - Office 365 E5 senza PSTN (a partire dal 17 ottobre 2017)
    - Enterprise Mobility & Security E5 (a partire dal 17 ottobre 2017)
    - Dynamics 365 Customer Engagement Piano 1 (a partire dal 17 ottobre 2017)
    - Dynamics 365 for Financials (a partire dal 17 ottobre 2017)
    - Microsoft 365 Business (a partire dal 1° marzo 2018)
    
**Q2** La fatturazione annuale e le versioni di valutazione gratuite sono diverse nel cloud sovrano rispetto al cloud pubblico?

-   **R:** No. Sono uguali. L'unica differenza saranno le SKU della versione di valutazione disponibili al momento del lancio.

**Q3** Chi può partecipare?

-   **R:** Tutti i partner possono partecipare. Tuttavia, questa opzione non è attualmente disponibile in Cina. 

**Q4** Quali azioni è necessario eseguire per sfruttare i vantaggi di queste versioni di valutazione gratuite?

-   **R:** Prendere in considerazione il modo in cui la versione di valutazione gratuita può essere incorporata nel movimento di vendita e l'effetto sui processi interni. Potresti anche dovere modificare le API che usi per supportare la conversione di una versione di valutazione gratuita in una sottoscrizione a pagamento. Le specifiche tecniche dettagliate di queste modifiche API vengono pubblicate nella visualizzazione Annunci del Centro per i partner.

**Q5** La versione di valutazione gratuita viene visualizzata nella fattura e nel file di riconciliazione?

-   **R:** No, le versioni di valutazione gratuite non verranno visualizzate nella fattura o nel file di riconciliazione basato sulle licenze. Verrà visualizzata nel file di riconciliazione basato su licenza e fattura dopo aver convertito una versione di valutazione gratuita in una sottoscrizione a pagamento. La sottoscrizione convertita verrà visualizzata nel file di riconciliazione basato su licenza e fattura come qualsiasi altra nuova sottoscrizione.

**Q6** Le versioni di valutazione gratuite influiscano sugli incentivi?

-   **R:** No. La versione di valutazione gratuita non ha alcun impatto sugli incentivi.

**Q7** Le versioni di valutazione gratuite saranno disponibili per ulteriori prodotti Office in futuro?

-   **R:** Offriamo le versioni di valutazione gratuite per questi prodotti perché sono le offerte aziendali più complete e popolari. È possibile che in futuro vengano aggiunte altre offerte di versioni di valutazione gratuite.

**(DOMANDA 8** Un cliente può avere più di una versione di valutazione gratuita?

-   **R:** Ogni cliente ha diritto a una versione di valutazione gratuita per ogni offerta disponibile.

**Q9** Sono previsti limiti per una versione di valutazione gratuita?

-   **R:** Sì. La versione di valutazione è per un massimo di 25 licenze. Il numero di licenze non può essere modificato durante il periodo di valutazione. Quando la versione di valutazione viene convertita in una sottoscrizione a pagamento, puoi aggiungere altre licenze alla sottoscrizione.

**Q10** Una versione di valutazione gratuita è stata convertita automaticamente in una sottoscrizione a pagamento?

-   **R:** No. Dovrai effettuare la conversione manuale della sottoscrizione, direttamente nel Centro per i partner o mediante l'API.

**Q11** Le versioni di valutazione gratuite possono essere utilizzate sia per le sottoscrizioni mensili che annuali fatturate?

-   **R:** Sì. Puoi scegliere la frequenza di fatturazione al momento della conversione della versione di valutazione in sottoscrizione a pagamento.

**Q12** La data di inizio della sottoscrizione sarà basata sulla data di inizio della versione di valutazione gratuita o sulla data in cui è stata convertita in una sottoscrizione a pagamento? 

-   **R:** La data di inizio è basata sulla data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione annuale, la data di rinnovo della sottoscrizione cade 12 mesi dopo la data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione mensile, la data di rinnovo della sottoscrizione cade 12 mesi dopo la data di fatturazione successiva alla data di conversione.

**Q13** È possibile aggiungere o rimuovere postazioni durante la versione di valutazione gratuita?

-   **R:** No. Le versioni di valutazione gratuite avranno una quantità predefinita di 25 licenze e non possono essere aggiornate.

**Q14** Sono disponibili versioni di valutazione per i componenti aggiuntivi, ad esempio ATP e PSTN?

-   **R:** Al momento non sono disponibili versioni di valutazione gratuite per le offerte per i componenti aggiuntivi.

**Q15** È possibile fornire una versione di valutazione gratuita per un'offerta che un cliente possiede già?

-   **R:** No. Se l'offerta è già di proprietà del cliente non può essere utilizzata per una versione di valutazione gratuita.

**Q16** Potrò vedere tutte le offerte di valutazione in attesa?

-   **R:** Sì. Nella pagina dei clienti sono elencate tutte le sottoscrizioni. Sono incluse le sottoscrizioni delle versioni di valutazione gratuite e le sottoscrizioni a pagamento.

**Q17** Riceverai una notifica per la scadenza delle versioni di valutazione gratuite?

-   **R:** No. È possibile tenere traccia delle date di scadenza imminenti utilizzando la visualizzazione dei clienti nel Centro per i partner o eseguendo una query sull'API. È consigliabile monitorare le date di frequente in modo da poter intraprendere le azioni appropriate in relazione alla decisione dei clienti.

**Q18** Se un cliente dispone di una versione di valutazione gratuita per un'offerta, può utilizzare anche un'altra versione di valutazione per un'offerta diversa? 

-   **R:** Sì. I clienti possono iscriversi a una versione di valutazione per ogni offerta. Ad esempio, possono ottenere una versione di valutazione gratuita per Office 365 Business Premium e una versione di valutazione gratuita per Office 365 E3.

**Q19** Cosa accade quando la versione di valutazione termina? Io o il mio cliente riceveremo una notifica? Quali notifiche vengono visualizzate quando tento di accedere a una versione di valutazione scaduta?

-   **R:** Una volta scaduta la versione di valutazione, un cliente che tenta di accedere a tale versione di valutazione visualizzerà un messaggio che indica che la versione di valutazione è scaduta. Non ci saranno notifiche per segnalare che una versione di valutazione sta per scadere, ma i partner possono tenere traccia della validità nella visualizzazione dei clienti o tramite le query all'API.

**D20** È possibile estendere una versione di valutazione?

-   **R:** No. Dopo 30 giorni la versione di valutazione deve essere convertita o scadrà.

**Q21** Quando una versione di valutazione scade, è possibile accedere alle informazioni della versione di valutazione?

-   **R:** Sì. I dati vengono archiviati conformemente agli standard di conservazione dei dati. Dopo aver acquistato una nuova sottoscrizione con gli stessi piani di servizio, i dati del cliente sono accessibili dalla sottoscrizione appena attivata.

**Q22** Sono disponibili versioni di valutazione gratuite per le offerte governative e scolastiche?

-   **R:** Al momento non sono disponibili versioni di valutazione gratuite per le offerte governative e scolastiche.

**Q23** Le versioni di valutazione gratuite del cliente per il programma Cloud Solution Provider (CSP) possono essere convertite in altri tenant di programma, ad esempio EA, Open o MOSP? 

-   **R:** No. Le sottoscrizioni non possono essere trasferite da CSP a un altro programma.

**Q24** Come è possibile ottenere supporto per le versioni di valutazione gratuite? 

-   **R:** Inviare una richiesta di assistenza tramite il centro per i partner.

## <a href="" id="billingalignmentfaq"></a>Allineamento di fatturazione-fine periodo libero

A partire dal 21 febbraio 2018, il programma Cloud Solution Provider (CSP) inizierà l'implementazione dell'"allineamento della data di fatturazione" per le nuove sottoscrizioni con la frequenza di fatturazione mensile. Questo "allineamento della data di fatturazione" fornirà ai partner maggiore flessibilità e la prevedibilità per le vendite e la fatturazione e per il provisioning e la gestione degli abbonamenti dei clienti. 

**AGGIORNAMENTO del 23 febbraio:**  In precedenza avevamo annunciato la data di implementazione del 20 febbraio, ma la nostra implementazione effettiva è stata leggermente ritardata e scaglionata per categoria di prodotto.  Per la data di implementazione per categoria di prodotto, vedere la seguente tabella. 

|**Categoria prodotto**   |**Giorno di implementazione**   |
|-----------------|:-------------|
|Office  |21 febbraio   |
|Windows, Minecraft   |22 febbraio   |
|Office 365 (Cina)   |23 febbraio   |
|Dynamics/Intune   |23 febbraio   |

Le sottoscrizioni acquistate prima della data di implementazione (vedi la tabella sopra) ottengono un periodo gratuito dalla data di acquisto alla data di fatturazione del partner. Gli abbonamenti acquistati dopo la data di implementazione non riceveranno più il periodo gratuito. Il periodo di 12 mesi a pagamento inizia (viene allineato) alla data di acquisto rispetto alla fatturazione del partner. I partner non vedranno più la "riga di fatturazione a $0" che rappresenta il periodo gratuito nel file di riconciliazione. Non sono state apportate modifiche alle API, alla fatturazione o agli incentivi.  I partner devono informare i team di vendita e contabilità di questa nuova logica di fatturazione e assicurarsi che le operazioni vengano modificate di conseguenza.  

Prima di implementare l'allineamento della data di fatturazione, abbiamo fatturato e addebitato alla data dell'anniversario della fatturazione del partner, ossia la data in cui il partner si è registrato al programma CSP, e non alla data dell'anniversario della sottoscrizione del cliente, ossia la data in cui il cliente ha acquistato la sottoscrizione. Dopo la data di implementazione, i partner riceveranno l'addebito alla data dell'anniversario della sottoscrizione, eliminando questo periodo gratuito.  I partner continueranno a ricevere le fatture alla data dell'anniversario di fatturazione, ma la data di validità della fattura sarà data dell'anniversario della sottoscrizione del cliente. 

Le sottoscrizioni che sono nel periodo gratuito alla data di implementazione, non riceveranno l'addebito tra la data di acquisto e la data di fatturazione del partner. Inoltre, non riceveranno l'addebito per il primo mese del termine di pagamento di 12 mesi. Se usi un file di riconciliazione per la verifica, tieni presente che questo addebito del primo mese non sarà più visibile nel file di riconciliazione.  

**Q1** Cosa sta cambiando con la data di fatturazione?

-   **R:** Le sottoscrizioni basate su licenza non avranno più un periodo gratuito. Attualmente, il periodo gratuito decorre dalla data di acquisto alla data di fatturazione del partner.

**Q2** Quando verrà rimosso il periodo libero?

- **R:** A partire dalla data di implementazione elencata nel grafico seguente, le nuove sottoscrizioni non riceveranno un periodo gratuito.

|**Categoria prodotto**   |**Giorno di implementazione**   |
|-----------------|:-------------|
|Office  |21 febbraio   |
|Windows, Minecraft   |22 febbraio   |
|Office 365 (Cina)   |23 febbraio   |
|Dynamics/Intune   |23 febbraio   |

**Q3** Quale sarà l'effetto sulle sottoscrizioni nel periodo gratuito nella data di implementazione?

- **R:** Le sottoscrizioni che rientrano nel periodo di tempo libero nella data di implementazione riceveranno comunque un periodo di tempo libero dalla data di acquisto alla data di fatturazione del partner. Queste licenze riceveranno anche un "periodo gratuito esteso" e non verrà addebitato il primo mese del termine di pagamento di 12 mesi. Il "periodo gratuito esteso" non sarà applicabili alle licenze aggiunte nel primo mese. Se aumenti la quantità di licenze nel primo mese, ti verranno addebitate le licenze aggiunte alla successiva fattura/riconciliazione. Se il file di riconciliazione viene utilizzato per la verifica, tieni presente che l'addebito del primo mese potrebbe non essere presente nel file di riconciliazione. Vedi gli scenari seguenti per una spiegazione più dettagliata.

**Q4** Quando inizierà il periodo di 12 mesi a pagamento per una nuova sottoscrizione?

- **R:** Attualmente, il periodo a pagamento inizia con la data di fatturazione del partner successiva alla data di acquisto. Dalla data di implementazione il periodo a pagamento per le nuove sottoscrizioni inizierà alla data di acquisto.

**Q5** Quando le sottoscrizioni vengono rinnovate automaticamente?

- **R:** Le sottoscrizioni vengono rinnovate automaticamente 12 mesi dopo la data della prima fatturazione. Attualmente, le sottoscrizioni si rinnovano automaticamente 12 mesi dopo la prima data di fatturazione del partner dopo la data di acquisto. Dalla data di implementazione le nuove sottoscrizioni vengono rinnovate automaticamente 12 mesi dopo la data di acquisto.

**Q6** Cosa accade se si acquista la sottoscrizione il 29, 30 o 31 giorni del mese?

- **R:** La sottoscrizione sarà disponibile a partire dalla data di acquisto, ma il termine a pagamento di 12 mesi non verrà avviato fino al primo giorno del mese successivo.

**Q7** Quali sono le offerte interessate?

- **R:** La rimozione del periodo di tempo libero si applica a tutte le sottoscrizioni basate su licenze CSP.

**(DOMANDA 8** In che modo questo influisca sulla fattura e sul file di riconciliazione? 

- **R:** Non viene più visualizzata la "linea di fatturazione $0" nella fattura o nel file di riconciliazione. Attualmente, la riga di fatturazione a 0$ rappresenta il periodo gratuito.

**Q9** La data di fatturazione cambierà?

- **R:** No, si continuerà a ricevere la fattura e il file di riconciliazione sulla data di fatturazione esistente.

**Q10** Le date mensili di inizio e di fine vengono modificate per le sottoscrizioni esistenti?

- **R:** No, le date di inizio e di fine del costo mensile della sottoscrizione esistente continueranno a essere allineate alla data di fatturazione. Tuttavia, le nuove sottoscrizioni saranno allineate alla data di acquisto. Vedi l'esempio seguente.

**Q11** Per gli incentivi è possibile modificare il calcolo?

- **R:** No, non vengono apportate modifiche ai calcoli degli incentivi.

**Q12** Verranno apportate modifiche alle API?

- **R:** No, non sono state apportate modifiche alle API.

### <a name="common-scenarios"></a>Scenari comuni


|**Scenari**   |**Scenario 1: Il periodo di sottoscrizione gratuito termina prima della data di implementazione**   |**Scenario 2: La sottoscrizione rientra nel periodo di tempo disponibile nella data di implementazione**  | **Scenario 3: Sottoscrizione acquistata il o dopo la data di implementazione**   |
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

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Scenario 5a: Sospendere e riattivare prima della data di fatturazione

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 5 giugno 2018, il partner sospende la sottoscrizione. Il 10 giugno 2018, il partner riattiva la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 
- Credito per annullamento -$30 per periodo di servizio 5 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni. 
- Addebito di $30 per periodo di servizio 10 giugno - 30 giugno. L'addebito non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |
|5/6/2018   |30/06/2018   |-$30   |1   |$30   |Commissione di annullamento |
|10/6/2018   |30/06/2018   |$30   |1   |$30   |Commissione di attivazione |

Quando una sottoscrizione viene sospesa e riattivata, la data di rinnovo automatico rimarrà 12 mesi dopo la data di acquisto originale.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scenario 5b: Sospendere e riattivare dopo la data di fatturazione, ma meno di 30 giorni dalla data di acquisto

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 20 giugno 2018, il partner sospende la sottoscrizione. Il 25 giugno 2018, il partner riattiva la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Credito per annullamento -$30 per periodo di servizio 20 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 25 giugno - 30 giugno. L'addebito non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/6/2018   |30/06/2018   |-$30   |1   |-$30   |Commissione di annullamento |
|25/6/2018   |30/06/2018   |$30   |1   |$30   |Commissione di attivazione |
|1/7/2018   |31/07/2018   |$30   |1   |$30   |Tariffa periodica |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Scenario 5C: Sospendere e riattivare (quantità di licenza diversa) dopo la data di fatturazione, ma meno di 30 giorni dalla data di acquisto

La data di fatturazione del partner è il 15 del mese. Il 1 giugno 2018 il partner acquista una nuova sottoscrizione. La sottoscrizione ha il prezzo di $30 per licenza al mese. Il 20 giugno 2018, il partner sospende la sottoscrizione. Il 25 giugno 2018, il partner riattiva la sottoscrizione con due licenze. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Credito per annullamento -$30 per periodo di servizio 20 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.
- Addebito di $30 per periodo di servizio 25 giugno - 30 giugno. L'addebito di riattivazione non è suddiviso proporzionalmente perché la sottoscrizione è stata riattivata nei primi 30 giorni. L'addebito è anche in base alla quantità di licenze originali, ovvero 1.
- Credito -$6 per periodo di servizio 25 giugno - 30 giugno. L'addebito di riattivazione è stato effettuato solo per 1 licenza durante il periodo di servizio 25 giugno - 30 giugno, quando si disponeva di 2 licenze. Il credito di $6 annulla l'addebito non corretto per il servizio di servizio 25 giugno - 30 giugno.
- Nuova fattura di $12 ripartita proporzionalmente per periodo di servizio 25 giugno - 30 giugno. Il partner aveva 2 licenze durante questo periodo di servizio. Il prezzo unitario viene calcolato come (30/30)*6*2 = $12.
- Addebito di $60 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/6/2018   |30/06/2018   |-$30   |1   |-$30   |Commissione di annullamento |
|25/6/2018   |30/06/2018   |$30   |1   |$30   |Commissione di attivazione |
|25/6/2018   |30/06/2018   |-$6   |1   |-$6   |Istanza del ciclo rateizzata |
|25/6/2018   |30/06/2018   |$6   |2   |$12   |Istanza del ciclo rateizzata |
|1/7/2018   |31/07/2018   |$30   |2   |$60   |Tariffa periodica |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Scenario 6: Sospensione della sottoscrizione inferiore a 30 giorni dopo l'acquisto e riattivazione più di 30 giorni dopo l'acquisto 

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Il 5 giugno, il partner sospende la sottoscrizione. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno
- Credito per annullamento -$30 per periodo di servizio 5 giugno - 30 giugno. Il credito non è suddiviso proporzionalmente perché la sottoscrizione è stata sospesa nei primi 30 giorni.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto
|5/6/2018   |30/06/2018   |-$30   |1   |-$30   |Commissione di annullamento

Il 10 luglio, il partner riattiva la sottoscrizione. Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito per riattivazione di $21,30 per periodo di servizio 10 luglio - 31 luglio. Le riattivazioni dopo 30 giorni dalla data di acquisto generano un addebito ripartito proporzionalmente. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/7/2018   |31/07/2018   |$21,30   |1   |$21,30   |Commissione di attivazione |

Il 15 agosto il file di riconciliazione conterrà le seguenti righe di fatturazione:
- Addebito di $30 per il periodo di servizio 1 agosto - 31 agosto.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/8/2018   |31/08/2018   |$30   |1   |$30   |Tariffa periodica |

Quando una sottoscrizione viene sospesa e riattivata, la data di rinnovo automatico rimarrà 12 mesi dopo la data di acquisto originale. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Scenario 7: sospendere e riattivare una sottoscrizione dopo 30 giorni dall'acquisto 
La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. 

Il 15 giugno il file di riconciliazione conterrà solo le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il partner sospende la sottoscrizione il 5 luglio, ma la riattiva il 15 luglio. Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio.
- Credito per annullamento -$26,14 per periodo di servizio 5 luglio - 31 luglio. Gli annullamenti dopo 30 giorni dalla data di acquisto generano un credito ripartito proporzionalmente. Calcolo = (prezzo mensile/giorni nel periodo totale di servizio) x giorni nel periodo di servizio ripartito x quantità di licenze x (-1) (30/31) x 27 x 1 x (-1) = -26,14.
- $16,45 addebito per riattivazione per il periodo di servizio 15 luglio 31 luglio. Le riattivazioni dopo 30 giorni dalla data di acquisto generano un addebito ripartito proporzionalmente. Calcolo = (30/31) x 17 x 1 = 16,45.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/7/2018   |31/07/2018   |$30  |1   |$30   |Tariffa periodica |
|5/7/2018   |31/07/2018   |   -$26,14   |1   |-$26,14|Commissione di annullamento |
|7/15/2018   |31/07/2018   |-$16,45   |1   |$16,45|Commissione di attivazione |

Il file di riconciliazione del 15 agosto conterrà le seguenti righe:
- Addebito di $30 per il periodo di servizio 1 agosto - 31 agosto.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/8/2018   |31/08/2018   |$30  |1   |$30   |Tariffa periodica |

### <a name="scenario-8-change-of-license-quantity"></a>Scenario 8: Modifica della quantità di licenze 

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione per $30 al mese. Il 10 giugno il partner aumenta la quantità di licenze da 1 a 2 licenze. Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. Anche se il partner ha aumentato la quantità di licenze prima della data di fatturazione del 15 giugno, la modifica non verrà riconosciuta nel sistema di fatturazione Microsoft fino al giorno dell'anniversario della sottoscrizione del 1 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |

Il 1 luglio, giorno dell'anniversario della sottoscrizione, il sistema di fatturazione Microsoft riconoscerà che il 10 giugno la quantità di licenze è stata modificata da 1 a 2. Il sistema di fatturazione genererà un credito e una nuova fattura ripartita proporzionalmente per il periodo di servizio 1 giugno - 9 giugno e 10 giugno - 30 giugno. 

Il file di riconciliazione del 15 luglio conterrà le seguenti righe:

- Credito -$30 per periodo di servizio 1 giugno - 30 giugno.
- Nuova fattura ripartita proporzionalmente $9 per periodo di servizio 1 giugno - 9 giugno. Questo è il periodo quando il cliente aveva 1 licenza. Calcolo = (prezzo mensile/giorni totali nel periodo di servizio) x giorni nel periodo di servizio ripartito x numero di licenze = (30/30) x 9 x 1 = 9.
- Nuova fattura ripartita proporzionalmente $42 per periodo di servizio 10 giugno - 30 giugno. Questo è il periodo quando il cliente aveva 2 licenze. Calcolo = (30/30) x 21 x 2 = 42.
- Addebito di $60 per periodo di servizio 1 luglio - 31 luglio.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/06/2018   |-$30   |1   |-$30|Istanza del ciclo rateizzata |
|1/6/2018   |9/6/2018   |$9   |1   |$9|Istanza del ciclo rateizzata |
|10/6/2018   |30/06/2018   |$21   |2   |$42|Istanza del ciclo rateizzata |
|1/7/2018   |31/07/2018   |$30   |2   |$60   |Tariffa periodica |

### <a name="scenario-9-add-on-subscriptions"></a>Scenario 9: Sottoscrizioni di componenti aggiuntivi

La data di fatturazione del partner è il 15 del mese. Il 1 giugno il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Il 10 giugno il partner acquista una nuova sottoscrizione per componente aggiuntivo per $5 al mese. La data di rinnovo della sottoscrizione per componente aggiuntivo si allinea alla data di rinnovo della sottoscrizione di base che è il 1 giugno. 

Il 10 giugno il partner acquista una sottoscrizione per componente aggiuntivo di una licenza per $5 al mese. 

Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno. È per la sottoscrizione di base.
- Addebito ripartito proporzionalmente $3,50 per periodo di servizio 10 giugno - 30 giugno. È per la sottoscrizione per componente aggiuntivo. 

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|1/6/2018   |30/06/2018   |$30   |1   |$30   |Rateizza le tariffe all'acquisto |
|10/6/2018   |30/06/2018   |$3,50   |1   |$3,50   |Rateizza le tariffe all'acquisto |

Il 15 luglio il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 luglio - 31 luglio. È per la sottoscrizione di base.
- Addebito di $5 per periodo di servizio 1 luglio - 31 luglio. È per la sottoscrizione per componente aggiuntivo.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|1/7/2018   |31/07/2018   |$30   |1   |$30   |Tariffa periodica |
|1/7/2018   |31/07/2018   |$5   |1   |$5   |Tariffa periodica |

La data di rinnovo automatico della sottoscrizione per componente aggiuntivo sarà il 1 giugno 2019, allineata alla sottoscrizione di base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Scenario 10: Nuovo acquisto il 29, 30 o 31 

La data di fatturazione del partner è il 15 del mese. Il 29 maggio il partner acquista una nuova sottoscrizione di una licenza per $30 al mese. Le sottoscrizioni acquistate il 29, il 30 o il 31 avranno un periodo gratuito dalla data dell'acquisto fino al 1 del mese successivo. Il giorno di anniversario della sottoscrizione sarà il giorno 1 per impostazione predefinita. In questo scenario, la sottoscrizione riceverà un periodo gratuito dal 29 maggio al 31 maggio e il periodo a pagamento di 12 mesi inizierà il 1 giugno. 

Il 15 giugno il file di riconciliazione conterrà le seguenti righe di fatturazione:

- Addebito di $30 per periodo di servizio 1 giugno - 30 giugno.

|**Inizio addebito**   |**Fine addebito**   |**Prezzo unitario**   |**Quantity**   |**Quantità**   |**Tipo di addebito** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/05/2018   | 30/06/2018   |$30   |1   |$30  |Rateizza le tariffe all'acquisto |

Il rinnovo automatico della sottoscrizione avverrà il 1 giugno 2019.
