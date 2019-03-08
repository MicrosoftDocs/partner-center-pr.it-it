---
title: Panoramica della fatturazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
Description: Informazioni su scenari di fatturazione di base e le differenze tra la fatturazione basati su licenza e basata sull'utilizzo
author: LauraBrenner
ms.author: labrenne
keywords: fatturazione, pagamenti, ordini, annullamento, gestione degli ordini, insolvenza, frode, utilizzo improprio, imposta, esenzioni fiscali, file di riconciliazione, file riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 917b04e9aba40aaf8dbfa27960e7baed7f39819d
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584674"
---
# <a name="billing-overview"></a>Panoramica della fatturazione

**Si applica a**

-  Centro per i partner
-  Partner del programma CSP

A seconda di prodotti, soluzioni e servizi che acquista per conto dei clienti, ti verranno fatturate per tali acquisti in uno o più dei modi seguenti:
-   [Fatturazione basati su licenza](#licensebasedbilling)

    Quando si acquistano prodotti o servizi online che richiedono licenze, vengono addebitati per ogni licenza acquistato (non sull'utilizzo delle licenze). È possibile scegliere se per la fatturazione mensile oppure una volta all'anno. Se variare delle esigenze aziendali, è possibile passare da uno a altro e viceversa. 
    
    Per altre informazioni sulla frequenza mensile e la fatturazione annua, vedere la fatturazione [domande frequenti su](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features).

-   [Fatturazione basata sull'utilizzo](#usagebasedbilling)

    Quando si acquistano servizi online, ad esempio le sottoscrizioni di Azure, la fatturazione per le tariffe di utilizzo mensili. La fatturazione solo mensile è disponibile per i prodotti basati sull'utilizzo. I servizi basati sull'utilizzo, ad esempio Azure, vengono fatturati in base alle tariffe a consumo, in base al consumo.

-   [Fatturazione singola](#onetimebilling)

    Quando si acquistano prenotazioni di Azure o altre sottoscrizioni di software, si paga in anticipo per un termine preimpostato. Poiché sta effettuando il pagamento in anticipo, vengono addebitati in un'unica soluzione. 
    
Se si è scelto di fatturati ogni mese o se si sono acquistato prodotti basati sull'utilizzo fatturati mensilmente, la data di fatturazione mensile è il giorno del mese selezionato al momento della creazione dell'account CSP nel centro per i Partner. Dopo aver creato l'account CSP, Microsoft invierà un messaggio di posta elettronica di conferma che include la data di fatturazione. Una volta creato, questa data non può essere modificata. 

## <a name="pricing-and-invoicing"></a>Prezzi e fatturazione
I listini prezzi sono disponibili con un (1) mese di anticipo, dato che vengono aggiornati mensilmente. I prezzi in base alle licenze sono garantiti per l'intera durata della sottoscrizione, in genere 12 mesi dalla data di acquisto. I prezzi in base all'uso possono variare di mese in mese. 

I prezzi per i prodotti, servizi e sottoscrizioni del software sono invece garantiti la durata della sottoscrizione, ma i prezzi vengano modificati al momento del rinnovo.

Vedrai le rettifiche e i crediti posticipati nella fattura successiva, dopo l'applicazione del credito o della rettifica.

Puoi visualizzare e scaricare le fatture e i file riconciliazione dalla pagina Fatturazione nel Centro per i partner. Nota che le fatture mensili sono disponibili nel Centro per i partner entro quattro (4) giorni dalla data di fatturazione selezionata.

## <a name="payment-terms"></a>Condizioni di pagamento

Le condizioni di pagamento sono net 60 giorni. Devono essere pagate le fatture tramite fattura data di scadenza (60 giorni dopo la data di fatturazione) o l'account sarà insoluta, che può rallentare la registrazione nel provider CSP. È possibile ripristinare le funzionalità complete degli account sospeso quando si effettuano pagamenti passato dovuti quantità.

### <a name="tax"></a>Imposta

Sono comprensivi di imposte in base sui dettagli (non dei clienti) perché la relazione di fatturazione è tra Microsoft e gli utenti. È possibile inviare l'ID imposta durante il processo di configurazione di account o inviando una richiesta di supporto in un secondo momento. Le modifiche saranno riportate nel ciclo di fatturazione successivo.

-   Per trattenere ed esenzione IVA, è necessario inviare documentazione tax tramite una richiesta di supporto. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

-   Per valore aggiunto esenzione IVA, è necessario inviare il numero di partita IVA (convalidati da Microsoft) tramite una richiesta di servizio. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

È possibile trovare ulteriori dettagli fiscali dal consulente fiscale o l'ufficio locale imposte.

## <a href="" id="licensebasedbilling"></a>Fatturazione basati su licenza

Quando si acquista un prodotto basato su licenza per conto di un cliente, è possibile scegliere per la fatturazione mensile o annuale. Se si desidera modificare la frequenza di fatturazione in un secondo momento, usare la procedura riportata di seguito. 

Il passaggio dalla fatturazione mensile per la fatturazione annua è utile se si dispone di numerose sottoscrizioni fatturate ogni mese e si vuole allinearli a una data di fatturazione comune. Il passaggio dalla fatturazione annuale di fatturazione mensile è utile in adattando le date di fatturazione a quelle dei singoli clienti. 

Quando si modifica la frequenza di fatturazione, la scadenza annuale viene aggiornato per riflettere che la data che è stata modificata la frequenza di fatturazione e una nuova data di rinnovo viene stabilite. 

Ogni volta che variare delle esigenze aziendali, è possibile modificare la frequenza di fatturazione. 

### <a name="billing-rules-for-annual-billing"></a>Regole di fatturazione per la fatturazione annua

-   Le sottoscrizioni sono annuali e rinnovate automaticamente.

-   La fatturazione avviene in 12 rate mensili o con un pagamento annuo per ogni sottoscrizione annuale.

-   La fatturazione avviene in anticipo per il periodo di fatturazione successivo per i servizi in base alle licenze, in base al numero di licenze alla fine del periodo di fatturazione precedente.

-   Eventuali modifiche del numero di licenze verranno addebitate/accreditate posticipatamente (con un calcolo proporzionale basato su licenza/giorni). Per il calcolo proporzionale viene usata la formula seguente: [ARROTONDA((ARROTONDA(Prezzo unitario * Quantità / Numero di giorni nel mese della ripartizione, 2) * Numero di giorni per la ripartizione) / Quantità, 2) * Quantità]

-   I pagamenti sono fatturati per licenze vendute (non il provisioning in licenze).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>Per modificare la frequenza di fatturazione di un servizio online

1.  Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente con la sottoscrizione da modificare. 

2.  Nella pagina di sottoscrizione del cliente, selezionare la sottoscrizione che si desidera modificare. 

3.  Nella pagina dei dettagli, sotto **frequenza di fatturazione**, selezionare **mensile** oppure **annuale**. Verrà visualizzata una pagina di conferma con informazioni importanti su come modificare la frequenza di fatturazione, nonché un elenco delle sottoscrizioni per essere modificato. 

4.  Selezionare **OK** apportare la modifica, o **Annulla** per annullare l'operazione. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

Microsoft non prevede un addebito tariffe per la terminazione anticipata di annullamento dei servizi basati su licenza. 

I crediti per l'annullamento dei servizi in base alle licenze vengono calcolati in modo proporzionale per i giorni inutilizzati nel caso di annullamenti precedenti alla data di scadenza (così come le riduzioni di licenze in base alla formula precedente).

## <a href="" id="usagebasedbilling"></a>Fatturazione basata sull'utilizzo

Alcuni prodotti e servizi Microsoft usano un modello di fatturazione "pagamento a consumo", in cui vengono fatturati solo i servizi usati. Ad esempio, Microsoft Azure Usa questo modello. 

### <a name="billing-rules"></a>Regole per la fatturazione
-   Le sottoscrizioni sono mese per mese e rinnova automaticamente alle nuove tariffe a consumo del servizio. Vengono addebitati ogni mese per l'utilizzo del mese precedente.

-   Le tariffe per i servizi a consumo possono variare all'interno del ciclo di fatturazione. 

    -   Aumento dei prezzi: preavviso di 30 giorni è disponibile.

    -   Riduzioni del prezzo: attive dal giorno della modifica.

    -   Per le sottoscrizioni esistenti verranno usate le tariffe in vigore all'inizio del ciclo di fatturazione.

    -   Le nuove sottoscrizioni, quando creato all'interno del ciclo di fatturazione stesso, usano la frequenza in vigore alla data di che creazione. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

I pagamenti con rettifiche compariranno nella fattura mensile successiva.

Microsoft non prevede un addebito tariffe per la terminazione anticipata di annullamento dei servizi basati sull'utilizzo. 

I crediti di qualsiasi tipo, inclusi quelli per il contratto di servizio, compariranno nella fattura mensile successiva.

## <a href="" id="onetimebilling"></a>Fatturazione singola

È possibile acquistare le sottoscrizioni di software e le prenotazioni di Azure in anticipo, per i termini di uno o tre anni. Quando si acquista in anticipo, sarà addebitato l'intero costo nella somma forfettaria di uno. Questo tipo di fatturazione è detto fatturazione monouso.

>[!IMPORTANT]
>Se si acquistano prenotazioni di Azure e/o le sottoscrizioni di software per un cliente in un percorso con una valuta diversa da quelle in uso, l'impostazione predefinita valuta di fatturazione è basata sulla posizione del cliente, non il percorso. Se i clienti si trovano in località diverse, si riceveranno fatture separate e i file di riconciliazione per ogni cliente di valuta devono applicata una fatturazione, consentendo la fatturazione della valuta appropriata. 

### <a name="manage-your-one-time-billing"></a>Gestire la fatturazione una tantum

**Visualizzare il stato di fatturazione corrente, fatture e i file di riconoscimento**

1.  Nel centro per i Partner, selezionare **fatturazione** e quindi **una volta** per visualizzare il tuo stato di fatturazione. 

2.  Seleziona una fattura o un file di riconoscimento per visualizzare informazioni più dettagliate. 

**Visualizzare la cronologia degli ordini del cliente**

1.  Selezionare **clienti** dal menu di scelta Centro per i Partner.

2.  Nella pagina **Clienti** trova il cliente di cui desideri visualizzare la cronologia ordini e seleziona la freccia giù per espandere il record del cliente. 

3.  Seleziona **Visualizza ordini** per visualizzare la cronologia degli ordini.

**Scaricare una nota di credito**

Se è necessario richiedere un credito o rebill, forniremo una nota di credito per annullare la fattura originale. È possibile richiedere una carta di credito/rebill per i motivi seguenti:

-   Correzioni all'ordine di acquisto o all'indirizzo

-   La fattura è stata generata e quindi è stato applicato un rimborso d'imposte. Puoi richiedere un credito/rifatturazione per ottenere il rimborso fiscale a fronte della fattura originale. Ciò vale anche per i rimborsi, in quanto puoi richiedere un credito/rifatturazione della fattura originale e quindi ottenere un rimborso.
