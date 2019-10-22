---
title: Piano di Azure - Fatturazione | Centro per i partner
ms.topic: article
ms.date: 10/04/2019
description: Descrive la struttura della fattura e del file di riconciliazione
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171298"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nuova esperienza commerciale in CSP - Fatturazione di Azure 

La fatturazione in base al piano di Azure è un'esperienza di fatturazione semplificata che prevede l'uso di una singola data di fatturazione allineata e di un periodo di fatturazione definito in base al mese di calendario. Per informazioni sulla piattaforma di fatturazione, leggi la [Guida operativa al commercio moderno del Centro per i partner](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).

## <a name="summary-of-billing-essentials"></a>Riepilogo dei dati essenziali della fatturazione

- **Data della fattura**: la fattura e il file di riconciliazione saranno disponibili nell'API o nel dashboard Centro per i partner entro il giorno 8 (mezzanotte UTC).

- **Periodo di fatturazione**: il periodo di fatturazione è allineato al mese di calendario, ad esempio 01/10-31/10, 01/11-30/11.

- **Addebiti per i periodi di servizio**: gli addebiti sono allineati al mese di calendario. Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10. La fattura del mese successivo che verrà generata il giorno 08/12 conterrà tutti gli addebiti per il periodo di servizio 01/11-31/11.

- **Termine di pagamento della fattura**: netto a 60 giorni.

- **Valuta della fattura**: i partner continueranno a ricevere la fattura nella valuta assegnata del paese del cliente. Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.

- **Incentivi per i partner**: pagamento a 45 giorni dalla fine del mese della fattura.

##  <a name="access-your-invoices-and-recon-files"></a>Accedere alle fatture e ai file di riconciliazione

L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione. 

**Per accedere alla fattura e al file di riconciliazione**

1. Accedi al Centro per i partner.

2. Dal menu del Centro per i partner seleziona **Fatturazione**.

3. Seleziona la scheda per il periodo **Calendar-based** (Basato su calendario) e la valuta a cui sei interessato.

![fatturazione](images/azure/billing1.png)

4. Seleziona **Invoice and Recon file** (Fattura e file di riconciliazione).  

Per visualizzare i dati della cronologia relativa alle fatture e ai file di riconciliazione, espandi la riga della cronologia di fatturazione sottostante.

## <a name="read-the-invoice"></a>Leggere la fattura

1. La fattura sarà disponibile entro il giorno 8 di ogni mese.

2. I partner hanno 60 giorni per effettuare il pagamento.

3. Il periodo di fatturazione riguarderà un determinato mese di calendario, ad esempio 01/10-31/10.

4. Gli addebiti sono al netto delle rettifiche (l'importo è al netto del "Credito ottenuto dai partner per i servizi gestiti").

5. Per altri dettagli sulla fatturazione, esamina il file di riconciliazione della fattura e il file sull'utilizzo valutato su base giornaliera.

![fattura](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>Leggere il file di riconciliazione

1. Ogni contatore della sottoscrizione di Azure può avere al massimo due righe di fatturazione nel file di riconciliazione.

2. Se il contatore è idoneo a un tipo di sconto o di credito (ad esempio, gli sconti di livello 1 o il credito ottenuto dai partner per i servizi gestiti) durante l'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione. La colonna **PriceAdjustmentDescription** farà riferimento allo sconto o al credito ottenuto. Il prezzo unitario effettivo sarà il prezzo al dettaglio meno il credito ottenuto dai partner o eventuali altri sconti.

3. Se il contatore non è idoneo al credito ottenuto dai partner per i servizi gestiti nell'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione e il prezzo unitario effettivo sarà il prezzo al dettaglio, ovvero il prezzo unitario.

4. Se il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** per una parte del mese, il file di riconciliazione conterrà due righe di fatturazione. Una riga rappresenterà i giorni per i quali il contatore è idoneo e la seconda rappresenterà i giorni per i quali non lo è. 

## <a name="read-the-daily-usage-file"></a>Leggere il file sull'utilizzo giornaliero

- I contatori delle sottoscrizioni in un piano di Azure vengono valutati e cumulati su base giornaliera. 

- Il **credito ottenuto dai partner per i servizi gestiti** viene determinato e applicato su base giornaliera.

- Ogni contatore della sottoscrizione avrà una riga per ogni giorno del mese di utilizzo.

- Nell'esempio seguente:

  - Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 01/07-03/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.

   - Il contatore non è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 04/07-07/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio.

    - Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 08/07-31/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.

![riconciliazione2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>Fattura nella valuta del cliente 

I prezzi per i servizi di Azure forniti tramite un piano di Azure verranno addebitati in USD e fatturati in base alla valuta assegnata al paese del cliente. Se la valuta di fatturazione è diversa da USD, il tasso di cambio usato verrà visualizzato nell'ultima pagina della fattura. I tassi di cambio vengono determinati mensilmente e applicati alla fattura successiva. Per l'elenco completo delle valute dei paesi, vedi la [nuova matrice di disponibilità delle offerte commerciali nelle varie aree geografiche e valute dei clienti](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V). 

Microsoft userà [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) per determinare il tasso di cambio usato per la conversione della valuta dei prezzi nella valuta della fattura. Il tasso di cambio verrà aggiornato e sarà disponibile il giorno precedente il primo giorno del mese in cui verrà applicato.

**Esempio**:  gli addebiti relativi all'utilizzo per il periodo di servizio compreso tra il 1° agosto e il 31 agosto verranno fatturati in base al tasso di cambio pubblicato il 1° agosto. Questi addebiti verranno riportati nella fattura di settembre e il tasso di cambio sarà indicato nell'ultima pagina della fattura. 

Gli utenti del tenant del partner continueranno a visualizzare le informazioni correlate specifiche dei ruoli riguardanti tutti i clienti e tutti gli ordini, indipendentemente dalla valuta di fatturazione. Inoltre, l'utente potrà visualizzare tutte le fatture in tutte le valute.  
 
## <a name="azure-reservations"></a>Prenotazioni di Azure 

Se vengono acquistate [prenotazioni di Azure](https://docs.microsoft.com/partner-center/azure-reservations) tramite un piano di Azure, inizialmente nel Centro per i partner sarà possibile scegliere solo la fatturazione una tantum. La fatturazione mensile è disponibile nel portale di Azure. Nel Centro per i partner sarà disponibile in una data successiva. 

## <a name="azure-cost-management"></a>Gestione costi di Azure 

Gli strumenti di Gestione costi di Azure consentono alle organizzazioni di visualizzare, gestire e ottimizzare i costi in Microsoft Azure. Questa funzionalità sarà disponibile nel portale di Azure. I partner avranno a disposizione una soluzione sempre attiva, a bassa latenza, con le seguenti funzionalità: 

- Analisi avanzata e avvisi relativi al budget 
- API e connettori di Power BI 
- Visualizzazione di più clienti 
- Gestione gratuita dei costi di Azure 
- Espansione di ruoli/utenti 

Visita la pagina [Gestione dei costi e fatturazione di Azure](https://azure.microsoft.com/services/cost-management) per altre informazioni su questa funzionalità, disponibile per i contratti Enterprise Agreement dal mese di febbraio 2019. La funzionalità è disponibile solo con i servizi di Azure acquistati nell'ambito di questa nuova esperienza commerciale di Azure in CSP. 
 
## <a name="azure-spending"></a>Spese di Azure 

Nel Centro per i partner sarà disponibile uno strumento di calcolo delle spese di Azure per la nuova esperienza commerciale in CSP. Quando applicata, questa funzionalità consentirà ai partner di visualizzare i dati seguenti:  

- Budget totale per un cliente 
- Spese stimate totali per un piano di Azure esistente 
- Percentuale di utilizzo dei clienti in ogni periodo di fatturazione 

Poiché il modello di fatturazione per i servizi di Azure tramite un piano di Azure riguarda un tipo di utilizzo con pagamento posticipato, per evitare di ricevere una fattura di importo maggiore del previsto, i partner possono definire un budget mensile e tenere traccia della percentuale di utilizzo. Un budget può essere applicato a un solo cliente o contemporaneamente a più clienti. 

![Spese di Azure](images/azure/azurespend.png)

**Per altre informazioni**

-  La modalità di calcolo del credito guadagnato dal partner (PEC) è indicata nel listino prezzi disponibile tramite il dashboard Centro per i partner. 
   
-  [Acquistare il piano di Azure](purchase-azure-plan.md)

-  [Listino prezzi per la nuova esperienza commerciale di Azure in CSP](azure-plan-price-list.md)
