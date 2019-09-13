---
title: Panoramica sulla fatturazione | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
Description: Informazioni sugli scenari di fatturazione di base e sulle differenze tra fatturazione basata su licenze e utilizzo
author: LauraBrenner
ms.author: labrenne
keywords: fatturazione, pagamenti, ordini, annullamento, gestione degli ordini, insolvenza, frode, utilizzo improprio, imposta, esenzioni fiscali, file di riconciliazione, file riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e13f3d24e649cf17daa1e3218c3376c8fc6e4faa
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820372"
---
# <a name="billing-overview"></a>Panoramica sulla fatturazione

**Si applica a**

-  Centro per i partner
-  Partner nel programma CSP

A seconda dei prodotti, delle soluzioni e dei servizi acquistati per conto dei clienti, verranno addebitati i costi per questi acquisti in uno o più dei modi seguenti:
-   [Fatturazione basata su licenza](#licensebasedbilling)

    Quando si acquistano prodotti o Servizi online che richiedono licenze, viene addebitata la tariffa per ogni licenza acquistata, non in base all'utilizzo delle licenze. È possibile scegliere se addebitare una fatturazione una volta al mese o una volta all'anno. Se le esigenze aziendali cambiano, è possibile passare da una all'altra e viceversa. 
    
    Per ulteriori informazioni sulla fatturazione mensile rispetto a quella annuale, vedere le [domande frequenti](https://docs.microsoft.com/partner-center/faq-about-new-billing-features)sulla fatturazione.

-   [Fatturazione basata sull'utilizzo](#usagebasedbilling)

    Quando si acquistano Servizi online, ad esempio le sottoscrizioni di Azure, vengono addebitate le tariffe di utilizzo mensili. Solo la fatturazione mensile è disponibile per i prodotti basati sull'utilizzo. I servizi basati sull'utilizzo, ad esempio Azure, vengono fatturati in base alle tariffe a consumo, in base al consumo.

-   [Fatturazione monouso](#onetimebilling)

    Quando si acquistano prenotazioni di Azure o altre sottoscrizioni software, si paga in anticipo per un periodo prestabilito. Poiché stai pagando in anticipo, ti viene addebitata una somma forfettaria. 
    
Se si è scelto di fatturare ogni mese o se sono stati acquistati prodotti basati sull'utilizzo fatturati mensilmente, la data di fatturazione mensile è il giorno del mese selezionato al momento della creazione dell'account CSP nel centro per i partner. Dopo aver creato l'account CSP, Microsoft invierà un messaggio di posta elettronica di conferma che include la data di fatturazione. Una volta creata, la data non può essere modificata. 

## <a name="pricing-and-invoicing"></a>Prezzi e fatturazione
I listini prezzi sono disponibili con un (1) mese di anticipo, dato che vengono aggiornati mensilmente. I prezzi in base alle licenze sono garantiti per l'intera durata della sottoscrizione, in genere 12 mesi dalla data di acquisto. I prezzi in base all'uso possono variare di mese in mese. 

I prezzi per i prodotti, i servizi e le sottoscrizioni software sono garantiti tramite la durata della sottoscrizione, tuttavia i prezzi possono variare quando si rinnova.

Vedrai le rettifiche e i crediti posticipati nella fattura successiva, dopo l'applicazione del credito o della rettifica.

Puoi visualizzare e scaricare le fatture e i file riconciliazione dalla pagina Fatturazione nel Centro per i partner. Nota che le fatture mensili sono disponibili nel Centro per i partner entro quattro (4) giorni dalla data di fatturazione selezionata.

## <a name="payment-terms"></a>Condizioni di pagamento

I termini di pagamento sono netti 60 giorni. Le fatture devono essere pagate in base alla data di scadenza della fattura (60 giorni dopo la data di fatturazione) oppure l'account sarà delinquente, che può influisca sulla registrazione in CSP. È possibile riottenere tutte le funzionalità degli account sospesi quando si paga l'importo dovuto scaduto.

### <a name="tax"></a>Imposta

L'utente viene tassato in base ai dettagli, ovvero non ai clienti, in quanto la relazione di fatturazione tra Microsoft e l'utente. È possibile inviare l'ID fiscale durante il processo di configurazione dell'account o inviando una richiesta di supporto in un secondo momento. Le modifiche saranno riportate nel ciclo di fatturazione successivo.

-   Per la ritenuta e l'esenzione fiscale per le vendite, è necessario inviare la documentazione fiscale tramite una richiesta di supporto. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

-   Per l'esenzione delle imposte IVA, è necessario inviare l'ID IVA (convalidato da Microsoft) tramite una richiesta di servizio. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

È possibile trovare ulteriori dettagli sulle imposte dall'ufficio fiscale locale o da Tax Advisor.

## <a href="" id="licensebasedbilling"></a>Fatturazione basata su licenza

Quando si acquista un prodotto basato su licenza per conto di un cliente, è possibile scegliere di fatturare ogni mese o ogni anno. Se si desidera modificare la frequenza di fatturazione in un secondo momento, attenersi alla procedura riportata di seguito. 

Passare dalla fatturazione mensile alla fatturazione annuale è utile se si dispone di numerose sottoscrizioni fatturate mensilmente e si desidera allinearle a una data di fatturazione comune. Passare dalla fatturazione annuale alla fatturazione mensile è utile per adattare le date di fatturazione a quelle dei singoli clienti. 

Quando si modifica la frequenza di fatturazione, il termine annuale viene aggiornato in modo da riflettere la data in cui è stata modificata la frequenza di fatturazione e viene stabilita una nuova data di rinnovo. 

È possibile modificare la frequenza di fatturazione ogni volta che le esigenze aziendali cambiano. 

### <a name="billing-rules-for-annual-billing"></a>Regole di fatturazione per la fatturazione annuale

-   Le sottoscrizioni sono annuali e rinnovate automaticamente.

-   La fatturazione avviene in 12 rate mensili o con un pagamento annuo per ogni sottoscrizione annuale.

-   La fatturazione avviene in anticipo per il periodo di fatturazione successivo per i servizi in base alle licenze, in base al numero di licenze alla fine del periodo di fatturazione precedente.

-   Eventuali modifiche del numero di licenze verranno addebitate/accreditate posticipatamente (con un calcolo proporzionale basato su licenza/giorni). Per il calcolo proporzionale viene usata la formula seguente: [ARROTONDA((ARROTONDA(Prezzo unitario * Quantità / Numero di giorni nel mese della ripartizione, 2) * Numero di giorni per la ripartizione) / Quantità, 2) * Quantità]

-   I pagamenti vengono fatturati per le licenze vendute (senza provisioning delle licenze).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Per modificare la frequenza di fatturazione di un servizio online

1.  Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente con la sottoscrizione che si desidera modificare. 

2.  Nella pagina sottoscrizioni del cliente selezionare la sottoscrizione che si desidera modificare. 

3.  Nella pagina dettagli, in **frequenza di fatturazione**, selezionare **mensile** o **annuale**. Verrà visualizzata una pagina di conferma con informazioni importanti sulla modifica della frequenza di fatturazione, oltre a un elenco delle sottoscrizioni che stanno per essere modificate. 

4.  Fare clic su **OK** per apportare la modifica oppure su **Annulla** per annullarla. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

Microsoft non addebita i costi di terminazione anticipati per l'annullamento dei servizi basati sulle licenze. 

I crediti per l'annullamento dei servizi in base alle licenze vengono calcolati in modo proporzionale per i giorni inutilizzati nel caso di annullamenti precedenti alla data di scadenza (così come le riduzioni di licenze in base alla formula precedente).

## <a href="" id="usagebasedbilling"></a>Fatturazione basata sull'utilizzo

Alcuni prodotti e servizi Microsoft usano un modello di fatturazione con pagamento in base al consumo, in cui vengono addebitati solo i servizi usati. Ad esempio, Microsoft Azure utilizza questo modello. 

### <a name="billing-rules"></a>Regole per la fatturazione
-   Le sottoscrizioni sono da mese a mese e vengono rinnovate automaticamente alle nuove tariffe per il servizio a consumo. Viene addebitato ogni mese per l'utilizzo del mese precedente.

-   Le tariffe per i servizi a consumo possono variare all'interno del ciclo di fatturazione. 

    -   Aumento prezzo: sono disponibili 30 giorni di preavviso.

    -   Riduzioni del prezzo: attive dal giorno della modifica.

    -   Per le sottoscrizioni esistenti verranno usate le tariffe in vigore all'inizio del ciclo di fatturazione.

    -   Le nuove sottoscrizioni, quando vengono create all'interno dello stesso ciclo di fatturazione, usano la tariffa in vigore alla data di creazione. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

I pagamenti con rettifiche compariranno nella fattura mensile successiva.

Microsoft non addebita i costi di terminazione anticipati per l'annullamento dei servizi basati sull'utilizzo. 

I crediti di qualsiasi tipo, inclusi quelli per il contratto di servizio, compariranno nella fattura mensile successiva.

## <a href="" id="onetimebilling"></a>Fatturazione monouso

È possibile acquistare in anticipo le sottoscrizioni software e le prenotazioni di Azure per un periodo di uno o tre anni. Quando si acquista in anticipo, viene addebitato l'intero costo in una somma forfettaria. Questo tipo di fatturazione è denominato fatturazione monouso.

>[!IMPORTANT]
>Se si acquistano le prenotazioni di Azure e/o le sottoscrizioni software per un cliente in una località con una valuta diversa da quella del cliente, la valuta di fatturazione predefinita è basata sulla posizione del cliente, non sulla località. Se si hanno clienti in più località, si riceveranno fatture separate e file di riconciliazione per ogni valuta che i clienti devono essere fatturati, consentendo di fatturare i clienti nella valuta appropriata. 

### <a name="manage-your-one-time-billing"></a>Gestire la fatturazione una tantum

**Visualizza lo stato di fatturazione corrente, le fatture e i file di ricognizione**

1.  In centro per i partner selezionare **fatturazione** e quindi **una volta** per visualizzare lo stato della fatturazione. 

2.  Seleziona una fattura o un file di riconoscimento per visualizzare informazioni più dettagliate. 

**Visualizzare la cronologia degli ordini di un cliente**

1.  Selezionare **Customers** dal menu centro per i partner.

2.  Nella pagina **Clienti** trova il cliente di cui desideri visualizzare la cronologia ordini e seleziona la freccia giù per espandere il record del cliente. 

3.  Seleziona **Visualizza ordini** per visualizzare la cronologia degli ordini.

**Scarica una nota di credito**

Se devi richiedere un credito o una fatturazione, ti invieremo una nota di credito per annullare la fattura originale. È possibile richiedere un credito o una fatturazione per i motivi seguenti:

-   Correzioni all'ordine di acquisto o all'indirizzo

-   La fattura è stata generata e quindi è stato applicato un rimborso d'imposte. Puoi richiedere un credito/rifatturazione per ottenere il rimborso fiscale a fronte della fattura originale. Ciò vale anche per i rimborsi, in quanto puoi richiedere un credito/rifatturazione della fattura originale e quindi ottenere un rimborso.
