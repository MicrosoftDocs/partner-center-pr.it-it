---
title: report Partner Center sottoscrizioni di Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vedere cosa si sta facendo bene e dove è possibile migliorare per quanto riguarda le sottoscrizioni cloud che si vendono o gestiscono per i clienti.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf2663122ca95e8d610c8be792a26682ae1718bf
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276315"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Report Sottoscrizioni prodotto disponibile nel dashboard di Partner Center Insights

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Visualizzatore di report | Visualizzatore di report executive

Il report Sottoscrizioni prodotto presenta l'analisi delle sottoscrizioni cloud vendute o gestite per i clienti. Si tratta di un report specifico del prodotto che include le prestazioni delle sottoscrizioni associate a prodotti cloud come Office 365, Azure, Dynamics e altri.

È possibile visualizzare le sezioni seguenti dal report Sottoscrizioni prodotto.

- Riepilogo
- Distribuzione geografica delle sottoscrizioni
- Tendenza di aggiunta/varianza delle sottoscrizioni
- Distribuzione della sottoscrizione per località partner, canale di vendita, SKU, tipo di collegamento partner, segmento
- Tendenza in base agli stati della sottoscrizione
- Tendenza dei prodotti

 > [!NOTE]
 > Questo report è disponibile nel dashboard di Insights. Per visualizzare questo report, è necessario avere un ruolo specifico in Partner Center, ad esempio Amministratore globale, Amministratore account, Visualizzatore report o Executive Report Viewer. Per altre informazioni, vedere l'amministratore globale dell'azienda. Tipi specifici di dati in questo report possono essere disponibili solo per gli utenti con privilegi Executive Report Viewer.

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot degli indicatori di prestazioni chiave (KPI) correlati alle sottoscrizioni vendute o gestite dall'utente per i clienti.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Riepilogo del report sottoscrizioni.":::

Per altre informazioni su ogni sezione del riepilogo, vedere di seguito:

- Sottoscrizioni:
  - Conteggio corrente delle sottoscrizioni di prodotti cloud vendute o gestite dall'utente.
  - Percentuale di crescita o riduzione delle sottoscrizioni durante l'intervallo di date selezionato.
  - Il grafico Micro presenta una tendenza mensile del conteggio delle sottoscrizioni durante l'intervallo di date selezionato.

- Sottoscrizioni attive:
  - Numero corrente di sottoscrizioni di prodotti cloud con utilizzo attivo misurato in base ai dati di telemetria del prodotto. In questo modo vengono escluse tutte le sottoscrizioni di valutazione nel caso di sottoscrizioni di Azure.
  - Percentuale di crescita o riduzione delle sottoscrizioni attive nel periodo di tempo selezionato.
  - Il grafico Micro presenta una tendenza mensile delle sottoscrizioni attive durante l'intervallo di date selezionato.

- Sottoscrizioni aggiunte:
  - Totale sottoscrizioni dei clienti aggiunte (vendute o gestite) dall'utente durante l'intervallo di date selezionato. Le nuove sottoscrizioni **con stato Attivo** o **Rinnovato** vengono conteggiate come sottoscrizioni aggiunte.
  - Percentuale di crescita o diminuzione delle sottoscrizioni aggiunte nell'ultimo mese completo rispetto al primo mese completo.
  - Il grafico Micro presenta una tendenza mensile delle sottoscrizioni aggiunte durante l'intervallo di date selezionato.

- Sottoscrizioni variate:
  - Totale sottoscrizioni dei clienti variate durante l'intervallo di date selezionato. Le sottoscrizioni con **stato Deprovisioning** o **Sospeso** in tale mese vengono conteggiate come sottoscrizione varianza.  
  - Percentuale di sottoscrizioni variate durante l'intervallo di date selezionato.
  - Il grafico Micro presenta una tendenza mensile delle sottoscrizioni variate rispetto all'intervallo di date selezionato.

- Sottoscrizioni per prodotti: suddivisione del numero di sottoscrizioni corrente per prodotti cloud.

## <a name="geographical-spread-of-subscriptions"></a>Distribuzione geografica delle sottoscrizioni

La **visualizzazione Sottoscrizioni per area geografica** mostra la distribuzione geografica delle sottoscrizioni totali in base ai mercati dei clienti. L'importo totale della sottoscrizione include sia le sottoscrizioni vendute che le sottoscrizioni attive.

La **tabella Number of countries/region** (Numero di paesi/aree geografiche) presenta il totale dei paesi/aree geografiche in cui si hanno sottoscrizioni e l'importo per paese delle sottoscrizioni totali e attive.

È possibile cercare e selezionare un paese nella griglia per ingrandire la posizione nella mappa. Premere **l'opzione** Home sulla mappa per ripristinare la visualizzazione originale. Passare il mouse sulla mappa per visualizzare tutte le sottoscrizioni e le sottoscrizioni attive in base al paese. Entrambi i campi nella griglia sono ordinabili.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="sottoscrizioni in base all'area geografica.":::

## <a name="subscription-addschurns"></a>Aggiunta/varianza della sottoscrizione

Questa visualizzazione presenta una tendenza di sottoscrizioni. Queste sono suddivise in categorie diverse (Nuovo, Esistente, Varianza) per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato. L'asse Y rappresenta il numero di sottoscrizioni. Le sottoscrizioni variate sono rappresentate sulla scala negativa dell'asse Y. 

L'istogramma in pila presenta una suddivisione delle sottoscrizioni nuove, esistenti e variate per il mese. È possibile ricompilare l'istogramma, suddiviso con elementi dello stack specifici. A tale scopo, selezionare gli elementi specifici nella legenda. È anche possibile usare il dispositivo di scorrimento nella parte superiore del grafico per ingrandire un periodo specifico.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="la sottoscrizione aggiunge e varianza.":::

## <a name="subscription-distribution"></a>Distribuzione della sottoscrizione

Questa visualizzazione presenta una suddivisione delle sottoscrizioni correnti in base a località MPN, segmenti di clienti, canale di vendita/modello tariffario di Azure e al tipo di attribuzione ,ad esempio DPOR, DAP e altri. Selezionare le rispettive schede per visualizzare la suddivisione in base a queste categorie. Per creare il grafico a torta con una suddivisione di categorie di elementi specifiche, selezionare tali categorie di elementi nella legenda.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuzione della sottoscrizione.":::

## <a name="subscription-state-distribution"></a>Distribuzione dello stato della sottoscrizione

Questa visualizzazione mostra la distribuzione delle sottoscrizioni dei clienti correnti in base allo stato o allo stato della sottoscrizione. Sono inclusi gli stati di sottoscrizione seguenti: **Attivo,** **Disabilitato,** **Deprovisioning,** **Apri,** **InGracePeriod,** **Chiuso** e **Altri.**

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuzione dello stato della sottoscrizione.":::

## <a name="products-trend"></a>Tendenza dei prodotti

Questa visualizzazione mostra un grafico a barre e due grafici a torta. Il grafico a barre presenta una tendenza mensile delle sottoscrizioni suddivise per prodotti commerciali, ad esempio Azure, Office, Dynamics e così via.

I due grafici a torta mostrano una suddivisione delle sottoscrizioni dei clienti correnti. Il primo grafico a torta suddivide le sottoscrizioni in base ai prodotti. Il secondo grafico a torta suddivide le sottoscrizioni in base a SKU o piani. Quando si seleziona un  prodotto nel grafico a torta scomposizione per prodotti, il grafico a torta adiacente mostra una suddivisione delle sottoscrizioni del prodotto in base a SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendenza dei prodotti.":::

> [!NOTE]
 > Il conteggio delle sottoscrizioni suddiviso in base a SKU potrebbe non corrispondere sempre al numero totale di sottoscrizioni per il prodotto. Questo problema può verificarsi se un cliente ha acquistato più SKU nella stessa sottoscrizione del prodotto.

## <a name="next-steps"></a>Passaggi successivi

- Per altri report, vedere Partner Center [Insights](partner-center-insights.md).

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report nel dashboard di Insights. [Altre informazioni](pci-download-reports.md) 
