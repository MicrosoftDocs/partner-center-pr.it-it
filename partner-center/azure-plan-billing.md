---
title: Piano di Azure - Fatturazione | Centro per i partner
ms.topic: article
ms.date: 11/01/2019
description: Descrive la struttura delle fatture e dei file di riconciliazione per il piano di Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 9b68361f80be0e5c68f707aa578f78cabcdee3e5
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428488"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nuova esperienza commerciale in CSP - Fatturazione di Azure 


La fatturazione in base al piano di Azure è un'esperienza semplificata che prevede l'uso di una singola data di fatturazione allineata e di un periodo di fatturazione basato sul mese di calendario. Per informazioni sulla piattaforma di fatturazione, leggi la [Guida operativa al commercio moderno del Centro per i partner](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).

## <a name="summary-of-billing-essentials"></a>Riepilogo dei dati essenziali della fatturazione

- **Data della fattura**: la fattura e il file di riconciliazione saranno disponibili nell'API o nel dashboard Centro per i partner entro il giorno 8 (mezzanotte UTC).

- **Periodo di fatturazione**: il periodo di fatturazione è allineato al mese di calendario, ad esempio 01/10-31/10, 01/11-30/11.

- **Addebiti per i periodi di servizio**: gli addebiti sono allineati al mese di calendario. Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10. La fattura del mese successivo che verrà generata il giorno 08/12 conterrà tutti gli addebiti per il periodo di servizio 01/11-31/11.

- **Termine di pagamento della fattura**: netto a 60 giorni.

- **Valuta della fattura**: i partner continueranno a ricevere la fattura nella valuta assegnata del paese del cliente. Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.

- **Incentivi per i partner**: pagamento a 45 giorni dalla fine del mese della fattura.

##  <a name="access-your-invoices-and-reconciliation-files"></a>Accedere alle fatture e ai file di riconciliazione

L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione. 

**Per accedere alla fattura e al file di riconciliazione**

1. Accedi al [dashboard](https://partner.microsoft.com/en-us/dashboard/) Centro per i partner.

2. Dal menu del Centro per i partner seleziona **Fatturazione**.

3. Seleziona la scheda per **Ricorrente** e **Occasionale** e la valuta di tuo interesse.

![fatturazione](images/azure/billing1.png)

4. Seleziona **Fattura** o il file **Reconciliation** (Riconciliazione).  

Per visualizzare i dati della cronologia relativa alle fatture e ai file di riconciliazione, espandi la riga della cronologia di fatturazione sottostante.


## <a name="understanding-usage-data"></a>Informazioni sui dati di utilizzo 

1. Il piano di Azure è il contenitore radice o di primo livello per l'utilizzo. Tutti gli utilizzi sono associati a un singolo piano di Azure. 

2. All'interno di un piano saranno presenti una o più sottoscrizioni di Azure. Si tratta di contenitori usati per la gestione e la distribuzione delle risorse. 

3. All'interno di una sottoscrizione, gruppi di risorse vengono aggiunti a risorse di gruppo. Ogni risorsa viene distribuita a un solo gruppo di risorse. 

4. Esempi di risorse sono le macchine virtuali e gli account di archiviazione. 

5. Le risorse generano contatori, che sono misurazioni del consumo di una risorsa. Una risorsa può generare l'utilizzo di più contatori. I contatori sono identificati da ProductId, SKUId e AvailabilityId. 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a>Gerarchia della misurazione e dei gruppi di risorse di sottoscrizione

**Account di Azure (tenant)**

- Sottoscrizione A
    - ResourceGroup 1
        - Macchina virtuale (risorsa)
            - Contatore di calcolo
        - Rete virtuale (risorsa)
            - Nessun contatore di fatturazione

    - ResourceGroup 2
        - Macchina virtuale (risorsa)
            - Contatore di calcolo
        - Disco gestito SSD Premium (risorsa)
            - Contatore della capacità di archiviazione
            - Contatore delle operazioni di archiviazione

- Sottoscrizione B   -ResourceGroup 1       - Azure SQL (risorsa)           - Contatore DTU       - Gateway VPN (risorsa)           - Contatore gateway VPN

    - ResourceGroup 2
        - Interfaccia di rete virtuale (risorsa)
            - Nessun contatore di fatturazione

## <a name="read-the-invoice"></a>Leggere la fattura

1. La fattura sarà disponibile entro il giorno 8 di ogni mese.

2. I partner hanno 60 giorni per effettuare il pagamento.

3. Il periodo di fatturazione riguarderà un determinato mese di calendario, ad esempio 01/10-31/10.

4. Gli addebiti sono al netto delle rettifiche (l'importo è al netto del "Credito ottenuto dai partner per i servizi gestiti").

5. Per altri dettagli sulla fatturazione, esamina il file di riconciliazione della fattura e il file sull'utilizzo valutato su base giornaliera.

![fattura](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a>Leggere il file di riconciliazione della fattura

1. Per ogni combinazione di piano di Azure e contatore possono essere presenti al massimo due righe di fatturazione nel file di riconciliazione.

2. Se il contatore è idoneo a un qualsiasi tipo di sconto o credito (ad esempio, agli sconti in base al livello o al credito ottenuto dai partner per i servizi gestiti) durante l'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione. La colonna **PriceAdjusmentDescription** farà riferimento allo sconto o al credito ottenuto.

3. Se non sono presenti risorse per un determinato contatore idoneo allo sconto o al credito ottenuto dai partner, il file di riconciliazione conterrà una sola riga di fatturazione e il prezzo unitario effettivo sarà il prezzo al dettaglio, ovvero il prezzo unitario.

4. Se il contatore, o qualsiasi risorsa che genera tale contatore, è idoneo al **credito ottenuto dai partner per i servizi gestiti** per una parte del mese, il file di riconciliazione conterrà due righe di fatturazione. Una riga rappresenterà i giorni per i quali il contatore è idoneo e la seconda rappresenterà i giorni per i quali non lo è. 

## <a name="read-the-daily-usage-file"></a>Leggere il file sull'utilizzo giornaliero

- I contatori delle sottoscrizioni in un piano di Azure vengono valutati e cumulati su base giornaliera. 

- Il **credito ottenuto dai partner per i servizi gestiti** viene determinato e applicato su base giornaliera.

- Ogni contatore della sottoscrizione avrà una riga per ogni giorno del mese di utilizzo.

- Nell'esempio seguente:

  - Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 01/07-03/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.

   - Il contatore non è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 04/07-07/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio.

    - Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 08/07-31/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.

![riconciliazione2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a>Fattura nella valuta del cliente 

I prezzi per i servizi di Azure forniti tramite un piano di Azure verranno addebitati in USD e fatturati in base alla valuta assegnata al paese del cliente. Se la valuta di fatturazione è diversa da USD, il tasso di cambio (FX) usato verrà visualizzato nell'ultima pagina della fattura. I tassi di cambio vengono determinati mensilmente e applicati alla fattura successiva. Per l'elenco completo delle valute dei paesi, vedi la [nuova matrice di disponibilità delle offerte commerciali nelle varie aree geografiche e valute dei clienti](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V). 

Microsoft userà [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) per determinare i tassi di cambio usati per la conversione della valuta dei prezzi nella valuta di fatturazione. I tassi di cambio verranno aggiornati e saranno disponibili il giorno precedente il primo giorno del mese in cui verranno applicati.

**Esempio**:  gli addebiti relativi all'utilizzo per il periodo di servizio compreso tra il 1° e il 31 agosto verranno fatturati in base al tasso di cambio pubblicato il 31 luglio. Questi addebiti verranno riportati nella fattura di settembre e il tasso di cambio sarà indicato nell'ultima pagina della fattura. 

 
## <a name="azure-reservations"></a>Prenotazioni di Azure 

Se vengono acquistate [prenotazioni di Azure](https://docs.microsoft.com/partner-center/azure-reservations) tramite un piano di Azure, inizialmente nel Centro per i partner sarà possibile scegliere solo la fatturazione una tantum. La fatturazione mensile è disponibile nel portale di Azure. Nel Centro per i partner sarà disponibile in una data successiva. 

## <a name="azure-spending"></a>Spese di Azure 

L'esperienza di spesa di Azure è stata aggiornata per supportare la nuova fatturazione del piano di Azure nel Centro per i partner. Tale meccanismo consente ai partner di:

- Visualizzare, gestire e ricevere avvisi per il budget impostato a livello di cliente 

- Visualizzare la spesa stimata totale per un piano di Azure (ripartita in base al livello di risorsa e contatore)

Poiché il modello di fatturazione per i servizi di Azure tramite un piano di Azure riguarda un tipo di utilizzo con pagamento posticipato, per evitare di ricevere una fattura di importo maggiore del previsto, i partner possono definire un budget mensile e tenere traccia della percentuale di utilizzo. Un budget può essere applicato a un solo cliente o contemporaneamente a più clienti. 

![Spese di Azure](images/azure/azurespend.png)

**Per altre informazioni**

-  La modalità di calcolo del credito ottenuto dal partner (PEC) è indicata nel listino prezzi disponibile tramite il [dashboard](https://partner.microsoft.com/en-us/dashboard/) Centro per i partner (è richiesto l'accesso). 
   
-  [Acquistare il piano di Azure](purchase-azure-plan.md)

-  [Listino prezzi per la nuova esperienza commerciale di Azure in CSP](azure-plan-price-list.md)
