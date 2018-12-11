---
title: Panoramica di fatturazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
Description: Information on basic billing scenarios and the differences between license-based and usage-based billing
author: labrenne
ms.author: labrenne
keywords: fatturazione, pagamenti, ordini, annullamento, gestione degli ordini, insolvenza, frode, utilizzo improprio, imposta, esenzioni fiscali, file di riconciliazione, file riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 96a859fda2ba8641c701888c4a865b1a1278c268
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917603"
---
# <a name="billing-overview"></a>Panoramica di fatturazione

**Ambito di applicazione**

-  Centro per i partner
-  Partner nel programma CSP

A seconda di prodotti, soluzioni e servizi che acquistare per conto dei clienti, la fattura verrà per questi acquisti in uno o più dei modi seguenti:
-   [Fatturazione in base alle licenze](#licensebasedbilling)

    Quando si acquista prodotti o servizi online che richiedono licenze, verrà emessa la fattura per ogni licenza che hai acquistato (non in uso licenza). Puoi scegliere se essere fatturate annualmente o una volta al mese. Se la tua azienda deve cambia, puoi passare da uno a altro e nuovamente. 
    
    Per altre informazioni su ogni mese e la fatturazione annuale, vedi le [domande frequenti su](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features)fatturazione.

-   [Fatturazione in base all'uso](#usagebasedbilling)

    Quando si acquistano servizi online, ad esempio sottoscrizioni di Azure, verrà emessa la fattura per i tassi di utilizzo mensile. La fatturazione mensile solo è disponibile per i prodotti basati sull'utilizzo. Servizi basati sull'utilizzo, ad esempio Azure, vengono fatturati in base a tariffe base consumo.

-   [Fatturazione una tantum](#onetimebilling)

    Quando acquisti prenotazioni di Azure o altre sottoscrizioni software, pagare in anticipo per un periodo di validità pre-imposta. Poiché stai pagare in anticipo, verrà emessa la fattura in un'unica soluzione. 
    
Se si è scelto di fatturazione mensile o se hai acquistato prodotti basati sull'utilizzo vengono fatturati mensilmente, alla data di fatturazione mensile è il giorno del mese selezionato quando hai creato l'account CSP nel centro per i Partner. Dopo aver creato correttamente il tuo account CSP, Microsoft invierà un'e-mail di conferma che include la data di fatturazione.

## <a name="pricing-and-invoicing"></a>Prezzi e fatturazione
I listini prezzi sono disponibili con un (1) mese di anticipo, dato che vengono aggiornati mensilmente. I prezzi in base alle licenze sono garantiti per l'intera durata dell'abbonamento, in genere 12 mesi dalla data di acquisto. I prezzi in base all'uso possono variare di mese in mese. 

I prezzi per i prodotti, servizi e le sottoscrizioni software sono garantiti tramite la durata della sottoscrizione, ma prezzi possono subire variazioni al momento del rinnovo.

Vedrai le rettifiche e i crediti posticipati nella fattura successiva, dopo l'applicazione del credito o della rettifica.

Puoi visualizzare e scaricare le fatture e i file riconciliazione dalla pagina Fatturazione nel Centro per i partner. Nota che le fatture mensili sono disponibili nel Centro per i partner entro quattro (4) giorni dalla data di fatturazione selezionata.

## <a name="payment-terms"></a>Condizioni di pagamento

Condizioni di pagamento sono netti 60 giorni. Le fatture devono essere a pagamento per la fattura data di scadenza (60 giorni dopo la data di fatturazione) o il tuo account sarà considerato insolvente, che potrebbero influire negativamente sulla registrazione in CSP. È possibile ricominciare a funzionalità complete per gli account sospesi quando si paga passato importo dovuto.

### <a name="tax"></a>Tax

Vengono tassati in base ai dettagli (non dei tuoi clienti) perché la relazione di fatturazione esiste tra e Microsoft. Puoi inviare il tuo ID fiscale durante il processo di configurazione di account o inviando una richiesta di supporto in un secondo momento. Le modifiche saranno riportate nel ciclo di fatturazione successivo.

-   Per dalla ritenuta alla fonte ed esenzione imposta sulle vendite, devi inviare documentazione fiscale appropriata tramite una richiesta di supporto. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

-   Per l'esenzione IVA (imposta sul valore aggiunto), devi inviare il numero di partita IVA (convalidato da Microsoft) tramite una richiesta di servizio. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

È possibile trovare ulteriori informazioni fiscali all'ufficio imposte locale o consulente fiscale.

## <a href="" id="licensebasedbilling"></a>Fatturazione in base alle licenze

Quando si acquista un prodotto basato su licenza per conto di un cliente, puoi scegliere di fatturazione mensile o annuale. Se vuoi modificare la frequenza di fatturazione in un secondo momento, utilizzare la procedura seguente. 

Il passaggio da fatturazione mensile per la fatturazione annuale è utile se hai numerosi le sottoscrizioni che vengono fatturate mensilmente e si desidera farle a una data di fatturazione comune. Il passaggio dalla fatturazione annuale per la fatturazione mensile è utile per personalizzare le date di fatturazione a quelle di clienti individuali. 

Quando modifichi la frequenza di fatturazione, il termine annuo viene aggiornato per riflettere che la data che è stata modificata la frequenza di fatturazione e una nuova data di rinnovo viene stabilite. 

Ogni volta che l'azienda richiede cambiamento, è possibile modificare la frequenza di fatturazione. 

### <a name="billing-rules-for-annual-billing"></a>Regole per la fatturazione per la fatturazione annuale

-   Le sottoscrizioni sono annuali e rinnovate automaticamente.

-   La fatturazione avviene in 12 rate mensili o un pagamento annuo per ogni sottoscrizione annuale.

-   La fatturazione avviene in anticipo per il periodo di fatturazione successivo per i servizi in base alle licenze, in base al numero di licenze alla fine del periodo di fatturazione precedente.

-   Eventuali modifiche del numero di licenze verranno addebitate/accreditate posticipatamente (con un calcolo proporzionale basato su licenza/giorni). Per il calcolo proporzionale viene usata la formula seguente: [ARROTONDA((ARROTONDA(Prezzo unitario * Quantità / Numero di giorni nel mese della ripartizione, 2) * Numero di giorni per la ripartizione) / Quantità, 2) * Quantità]

-   Sono riferiti alle licenze vendute (non licenze con provisioning).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Per modificare la frequenza di fatturazione di un servizio online

1.  Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente con la sottoscrizione che vuoi modificare. 

2.  Nella pagina delle sottoscrizioni del cliente, seleziona la sottoscrizione che vuoi modificare. 

3.  Nella pagina dei dettagli, in **frequenza di fatturazione**, seleziona **mensile** o **annuale**. Vedrai una pagina di conferma con informazioni importanti sugli modificando la frequenza di fatturazione, nonché un elenco delle sottoscrizioni sta per essere modificato. 

4.  Seleziona **OK** per apportare la modifica o **annullamento** per annullare l'operazione. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

Microsoft non addebiterà alcun costo anticipata previsti costi per annullamento dei servizi basati su licenza. 

I crediti per l'annullamento dei servizi in base alle licenze vengono calcolati in modo proporzionale per i giorni inutilizzati nel caso di annullamenti precedenti alla data di scadenza (così come le riduzioni di licenze in base alla formula precedente).

## <a href="" id="usagebasedbilling"></a>Fatturazione in base all'uso

Alcuni prodotti e servizi Microsoft usano un modello di fatturazione "pay in base all'uso", in cui vengono fatturati solo i servizi usati. Ad esempio, Microsoft Azure utilizza questo modello. 

### <a name="billing-rules"></a>Regole per la fatturazione
-   Le sottoscrizioni sono mese in mese e rinnovo automatico alle nuove tariffe del servizio a consumo. Verrà emessa la fattura ogni mese per l'uso del mese precedente.

-   Le tariffe per i servizi a consumo possono variare all'interno del ciclo di fatturazione. 

    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni

    -   Riduzioni del prezzo: attive dal giorno della modifica.

    -   Per le sottoscrizioni esistenti verranno usate le tariffe in vigore all'inizio del ciclo di fatturazione.

    -   Le nuove sottoscrizioni, quando creata all'interno del ciclo di fatturazione stesso, usano le tariffe in vigore alla data di creazione. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

I pagamenti con rettifiche compariranno nella fattura mensile successiva.

Microsoft non addebiterà alcun costo anticipata previsti costi per annullamento dei servizi basati sull'utilizzo. 

I crediti di qualsiasi tipo, inclusi quelli per il contratto di servizio, compariranno nella fattura mensile successiva.

## <a href="" id="onetimebilling"></a>Fatturazione una tantum

Puoi acquistare prenotazioni di Azure e sottoscrizioni software in anticipo, per i termini di uno o tre anni. Quando acquisti in anticipo, verrà emessa la fattura per il costo intero in un uno attuale. Questo tipo di fatturazione è chiamato fatturazione una tantum.

>[!IMPORTANT]
>Se acquisti prenotazioni di Azure e/o le sottoscrizioni software per un cliente in una posizione con valuta diversa dalla tua, la valuta di fatturazione predefinita si basa sulla posizione del cliente, non sulla tua sede. Se disponi di clienti in più posizioni, riceverai fatture separate e file di riconciliazione per i clienti ogni valuta bisogno di fatturazione, consentendoti di fatturare nella valuta appropriata. 

### <a name="manage-your-one-time-billing"></a>Gestire la fatturazione una tantum

**Visualizzare lo stato della fatturazione corrente, le fatture e i file di riconoscimento**

1.  Nel centro per i Partner, seleziona **la fatturazione** e quindi **una sola volta** per visualizzare lo stato di fatturazione. 

2.  Seleziona una fattura o un file di riconoscimento per visualizzare informazioni più dettagliate. 

**Visualizzare la cronologia degli ordini di un cliente**

1.  Seleziona **clienti** dal menu di Centro per i Partner.

2.  Nella pagina **Clienti** trova il cliente di cui desideri visualizzare la cronologia ordini e seleziona la freccia giù per espandere il record del cliente. 

3.  Seleziona **Visualizza ordini** per visualizzare la cronologia degli ordini.

**Scarica una nota di credito**

Se hai bisogno richiedere un credito o una nuova fattura ripartita, forniremo un accredito per annullare la fattura originale. Si potrebbe richiedere una credito/una nuova fattura ripartita per i motivi seguenti:

-   Correzioni di ordine di acquisto o l'indirizzo

-   Fattura generata e quindi un rimborso fiscale è stato applicato. Puoi richiedere una credito/una nuova fattura ripartita per ottenere la restituzione di imposte trascinata indietro nella fattura originale. Ciò vale anche per i rimborsi, come è possibile richiedere una credito/una nuova fattura ripartita della fattura originale e quindi eseguire il pull in un rimborso.
