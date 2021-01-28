---
title: 'Fatturazione dei piani di Azure: fattura e file di riconciliazione'
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come accedere e ottieni informazioni sulla struttura dei file di fatturazione e di riconciliazione correlata alla fatturazione per il piano di Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925010"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nuova esperienza commerciale in CSP - Fatturazione di Azure 

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale

Questo articolo illustra come accedere e ottenere informazioni sulla struttura dei file di fatturazione e di riconciliazione correlata alla fatturazione per il piano di Azure. La fatturazione in base al piano di Azure è un'esperienza semplificata che prevede l'uso di una singola data di fatturazione allineata e di un periodo di fatturazione basato sul mese di calendario.

## <a name="summary-of-billing-essentials"></a>Riepilogo dei dati essenziali della fatturazione

- **Data della fattura**: la fattura e il file di riconciliazione saranno disponibili nell'API o nel dashboard Centro per i partner entro il giorno 8 (mezzanotte UTC).

- **Periodo di fatturazione**: il periodo di fatturazione è allineato al mese di calendario, ad esempio 01/10-31/10, 01/11-30/11.

- **Addebiti per i periodi di servizio**: gli addebiti sono allineati al mese di calendario. Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10. La fattura del mese successivo che verrà generata il giorno 08/12 conterrà tutti gli addebiti per il periodo di servizio 01/11-31/11.

- **Termine di pagamento della fattura**: netto a 60 giorni.

- **Valuta fattura**: a partire dal 28 gennaio 2021, i partner dell'area UE/EFTA e del Regno Unito con nuovi clienti e clienti CSP esistenti che acquistano nuove offerte commerciali per la prima volta, i cui tenant sono stati creati prima dell'11 maggio 2020, verranno fatturati per tali acquisti nella valuta della località partner. I partner situati al di fuori dell'area UE/EFTA e del Regno Unito continueranno a essere fatturati in valuta località partner.

- **Incentivi per i partner**: pagamento a 45 giorni dalla fine del mese della fattura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Accedere alle fatture e ai file di riconciliazione

L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione.

Per accedere alla fattura e al file di riconciliazione:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/) Centro per i partner.

2. Dal menu del Centro per i partner seleziona **Fatturazione**.

3. Seleziona la scheda per **Ricorrente** e **Occasionale** e la valuta di tuo interesse.

   :::image type="content" source="images/azure/billing3.png" alt-text="fatturazione":::

4. Seleziona **Fattura** o il file **Reconciliation** (Riconciliazione).  

   Per visualizzare i dati della cronologia relativa alle fatture e ai file di riconciliazione, espandi la riga della cronologia di fatturazione sottostante.

## <a name="understanding-usage-data"></a>Informazioni sui dati di utilizzo 

1. Il piano di Azure è il contenitore radice o di primo livello per l'utilizzo. Tutti gli utilizzi sono associati a un singolo piano di Azure.

2. All'interno di un piano saranno presenti una o più sottoscrizioni di Azure. Si tratta di contenitori usati per la gestione e la distribuzione delle risorse. 

3. All'interno di una sottoscrizione, gruppi di risorse vengono aggiunti a risorse di gruppo. Ogni risorsa viene distribuita a un solo gruppo di risorse. 

4. Esempi di risorse sono le macchine virtuali e gli account di archiviazione. 

5. Le risorse generano contatori, che sono misurazioni del consumo di una risorsa. Una risorsa può generare l'utilizzo di più contatori. I contatori sono identificati da ProductId, SKUId e AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Gerarchia dei gruppi di risorse di sottoscrizione e misurazione

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

4. Gli addebiti sono al netto delle rettifiche (l'importo è al netto del "credito ottenuto dai partner per i servizi gestiti").

5. Per altri dettagli sulla fatturazione, esamina il file di riconciliazione della fattura e il file sull'utilizzo valutato su base giornaliera.

   :::image type="content" source="images/azure/invoice1.png" alt-text="fattura":::

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

   :::image type="content" source="images/azure/pecfinal.png" alt-text="riconciliazione2":::

## <a name="invoice-in-customer-currency"></a>Fattura nella valuta del cliente

I prezzi per i servizi di Azure forniti tramite un piano di Azure verranno addebitati in USD e fatturati in base alla valuta assegnata al paese del cliente. Se la valuta di fatturazione è diversa da USD, il tasso di cambio (FX) usato verrà visualizzato nell'ultima pagina della fattura. I tassi di cambio vengono determinati mensilmente e applicati alla fattura successiva. Per un elenco completo delle valute dei paesi, vedi la [nuova matrice di disponibilità delle offerte commerciali nelle varie aree geografiche e valute dei clienti](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft segue il London Stock Exchange per la conversione. Viene usato il tasso di cambio, che è uguale al tasso di cambio acquisito nell'ultimo secondo dell'ultimo giorno lavorativo del mese per la borsa di Londra. I tassi di cambio verranno aggiornati e saranno disponibili il giorno precedente il primo giorno del mese in cui verranno applicati.

## <a name="azure-reservations"></a>Prenotazioni di Azure


Se si acquistano [prenotazioni di Azure](azure-reservations.md) tramite un piano di Azure, è possibile scegliere una fatturazione singola o mensile.


## <a name="azure-spending"></a>Spese di Azure

L'esperienza di spesa di Azure è stata aggiornata per supportare la nuova fatturazione del piano di Azure nel Centro per i partner. Tale meccanismo consente ai partner di:

- Visualizzare, gestire e ricevere avvisi per il budget impostato a livello di cliente 

- Visualizzare la spesa stimata totale per un piano di Azure (ripartita in base al livello di risorsa e contatore)

Poiché il modello di fatturazione per i servizi di Azure tramite un piano di Azure riguarda un tipo di utilizzo con pagamento posticipato, per evitare di ricevere una fattura di importo maggiore del previsto, i partner possono definire un budget mensile e tenere traccia della percentuale di utilizzo. Un budget può essere applicato a un solo cliente o contemporaneamente a più clienti. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Spese di Azure":::

## <a name="next-steps"></a>Passaggi successivi

- Vedere come viene calcolato il credito ottenuto dai partner. Accedere al [dashboard](https://partner.microsoft.com/dashboard/) del Centro per i partner e individuare l'elenco prezzi disponibile.

- Informazioni sull'[acquisto del piano Azure](purchase-azure-plan.md)

- Vedere il [listino prezzi per la nuova esperienza commerciale di Azure in CSP](azure-plan-price-list.md)
