---
title: Report delle sottoscrizioni di partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri cosa puoi fare e dove puoi migliorare le tue sottoscrizioni cloud che Vendi o Gestisci per i tuoi clienti.
ms.assetid: ''
keywords: PCI, prestazioni, misure, successo dei clienti, sottoscrizioni cloud, analisi, report
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d4896fbff07eebc1dd6debf6010dc3970f45a4a
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679318"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Report sulle sottoscrizioni di prodotto disponibile nel dashboard di partner Center Insights

**Ruoli appropriati**
- Amministratore globale
- Agente amministratore
- Visualizzatore report
- Visualizzatore report Executive

Il report sottoscrizioni prodotto presenta analisi sulle sottoscrizioni cloud vendute o gestite per i clienti. Si tratta di un report specifico del prodotto che include le prestazioni delle sottoscrizioni associate ai prodotti cloud, ad esempio Office 365, Azure, Dynamics e così via.

È possibile visualizzare le sezioni seguenti del report sottoscrizioni prodotto.

- Summary
- Distribuzione geografica delle sottoscrizioni
- Tendenza aggiunta/varianza sottoscrizioni
- Distribuzione della sottoscrizione per località partner, canale di vendita, SKU, tipo di connessione partner, segmento
- Tendenza per stati di sottoscrizione
- Tendenza prodotti

 > [!NOTE]
 > Questo report è disponibile nel dashboard di Insights. Per visualizzare questo report, è necessario disporre di un ruolo specifico nel centro per i partner, ad esempio amministratore globale, amministratore account, Visualizzatore report o Visualizzatore report Executive. Per ulteriori informazioni, vedere l'amministratore globale dell'azienda. I tipi specifici di dati in questo report possono essere disponibili solo per gli utenti con privilegi di Visualizzatore di report Executive.

**Riepilogo**

La sezione Riepilogo presenta una visualizzazione snapshot degli indicatori di prestazioni chiave (KPI) correlati alle sottoscrizioni vendute o gestite dall'utente per i clienti.  

- Sottoscrizioni: numero corrente di sottoscrizioni di prodotti cloud vendute o gestite dall'utente.
Percentuale di aumento o diminuzione delle sottoscrizioni durante l'intervallo di date selezionato.

Il grafico micro presenta una tendenza mensile rispetto al numero di sottoscrizioni durante l'intervallo di date selezionato.

- Sottoscrizioni attive: numero corrente di sottoscrizioni di prodotti cloud con utilizzo attivo misurato in base alla telemetria del prodotto. Questa operazione esclude tutte le sottoscrizioni di valutazione nel caso di sottoscrizioni di Azure.
Aumento o riduzione percentuale delle sottoscrizioni attive nel periodo di tempo selezionato.

Il grafico micro presenta una tendenza mensile rispetto al mese delle sottoscrizioni attive durante l'intervallo di date selezionato.

- Sottoscrizioni aggiunte: totale sottoscrizioni cliente aggiunte (vendute o gestite) dall'utente durante l'intervallo di date selezionato. Le nuove sottoscrizioni con stato **attivo** o **rinnovato** vengono conteggiate come sottoscrizioni aggiunte.
Percentuale di aumento o diminuzione delle sottoscrizioni aggiunte nell'ultimo mese intero rispetto al primo mese intero.

Il grafico micro presenta una tendenza mensile delle sottoscrizioni aggiunte durante l'intervallo di date selezionato.

- Sottoscrizioni varianza: numero totale di sottoscrizioni cliente ricorrenti durante l'intervallo di date selezionato. Le sottoscrizioni con stato **deprovisioning** o **sospeso** in tale mese vengono conteggiate come una sottoscrizione di varianza.  
Percentuale di sottoscrizioni varianza durante l'intervallo di date selezionato.

Il grafico micro presenta una tendenza mensile delle sottoscrizioni di varianza nell'intervallo di date selezionato.

- Sottoscrizioni per prodotti: suddivisione del numero di sottoscrizioni correnti per prodotti cloud.

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Riepilogo report sottoscrizioni":::

**Distribuzione geografica delle sottoscrizioni**

La vista **sottoscrizioni in base alla geografia** Mostra la distribuzione geografica delle sottoscrizioni totali per i mercati dei clienti. L'importo totale delle sottoscrizioni include sia le sottoscrizioni vendute sia le sottoscrizioni attive.

Il **numero di paesi/area geografica** presenta il totale dei paesi/aree geografiche in cui sono presenti sottoscrizioni e la quantità per ogni paese di sottoscrizioni totali e attive.

È possibile cercare e selezionare un paese nella griglia per ingrandire la posizione della mappa. Premere l'opzione **Home** sulla mappa per ripristinare la visualizzazione originale. Passare il puntatore del mouse sulla mappa per visualizzare tutte le sottoscrizioni e le sottoscrizioni attive per paese. Entrambi i campi sulla griglia sono ordinabili.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="sottoscrizioni per geografia":::

**Aggiunta/varianza della sottoscrizione**

Questa vista presenta una tendenza delle sottoscrizioni. Questi sono suddivisi in categorie diverse (nuove, esistenti, in varianza) per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato. L'asse Y rappresenta il conteggio delle sottoscrizioni. Le sottoscrizioni con varianza sono rappresentate sulla scala negativa dell'asse Y. 

L'istogramma a colonne in pila presenta una suddivisione delle sottoscrizioni nuove, esistenti e a varianza per il mese. È possibile ricompilare l'istogramma, suddiviso con elementi dello stack specifici. A tale scopo, selezionare gli elementi specifici nella legenda. È inoltre possibile utilizzare il dispositivo di scorrimento nella parte superiore del grafico per ingrandire un periodo specifico.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="Aggiunta e varianza della sottoscrizione":::

**Distribuzione della sottoscrizione**

Questa visualizzazione presenta una suddivisione delle sottoscrizioni correnti in base alle località MPN, ai segmenti dei clienti, al modello di prezzo di canale di vendita/Azure e al tipo di attribuzione, ad esempio DPOR, DAP e così via. Fare clic sulle rispettive schede per visualizzare la suddivisione in base a queste categorie. Per compilare il grafico a torta con una suddivisione delle categorie di elementi specifiche, selezionare le categorie di elementi nella legenda.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuzione della sottoscrizione":::

**Distribuzione dello stato della sottoscrizione**

Questa visualizzazione Mostra la distribuzione delle sottoscrizioni dei clienti correnti in base allo stato o allo stato della sottoscrizione. Sono inclusi gli Stati di sottoscrizione seguenti: **attivo**, **disabilitato**, sottoposta a **deprovisioning**, **aperto**, **InGracePeriod**, **chiuso**e **altro**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuzione dello stato della sottoscrizione":::

**Tendenza prodotti**

Questa vista mostra un grafico a barre e due grafici a torta. Il grafico a barre presenta una tendenza mensile delle sottoscrizioni suddivise da prodotti commerciali, ad esempio Azure, Office, Dynamics e così via.

I due grafici a torta mostrano una suddivisione delle sottoscrizioni dei clienti correnti. Il primo grafico a torta suddivide le sottoscrizioni in base ai prodotti. Il secondo grafico a torta suddivide le sottoscrizioni in base a SKU o piani. Quando si seleziona un prodotto nel grafico a torta suddivisione **per prodotti** , nel grafico a torta adiacente viene visualizzata una suddivisione delle sottoscrizioni di tale prodotto per SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendenza prodotti":::

> [!NOTE]
 > Il numero di sottoscrizioni suddivise in base agli SKU potrebbe non corrispondere sempre al numero totale di sottoscrizioni per quel prodotto. Questo problema può verificarsi se un cliente ha acquistato più SKU con la stessa sottoscrizione al prodotto.

## <a name="next-steps"></a>Passaggi successivi

- Per altri report, vedere [Partner Center Insights](partner-center-insights.md).
