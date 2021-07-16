---
title: Partner Center Insights - Report cliente
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scoprire i modi per migliorare l'azienda. Visualizzare le tendenze specifiche dei clienti in base all'area geografica, al prodotto e ad altri attributi.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7be488d1002f98e95349046edb72a644e93a47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375661"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Report del dashboard clienti da Partner Center Insights

**Ruoli appropriati:** amministratore globale | Agente di amministrazione | Visualizzatore report | Visualizzatore di report executive

Il dashboard Clienti presenta i dati dei clienti che hanno acquistato prodotti cloud come Office, Azure e Dynamics. tramite l'utente o usato per distribuire e gestire questi prodotti nei tenant. 
 
Il dashboard Clienti include le sezioni seguenti: 

- Riepilogo  
- Distribuzione geografica dei clienti 
- Tendenze di aggiunta/varianza dei clienti 
- Distribuzione dei clienti per località partner, segmenti di clienti, canale di vendita, tipo di attribuzione partner 
- Distribuzione dei clienti per prodotto 
- Tendenze di distribuzione dei clienti per località partner, segmenti di clienti, modello di determinazione prezzi, tipo di attribuzione partner 
- Tendenza clienti attivi 

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot di vari indicatori di prestazioni chiave (KPI) correlati ai clienti, ad esempio clienti, clienti attivi, sottoscrizioni, clienti aggiunti, clienti variati e clienti per ogni prodotto. I filtri a livello di pagina sono applicabili per ogni sezione.

:::image type="content" source="images/insights/customer-product.png" alt-text="Screenshot del dashboard Riepilogo clienti che mostra i grafici a barre e il numero di clienti attivi, aggiunti di recente, persi/sforati o per prodotto specifico.":::

### <a name="customers"></a>Clienti

- Il numero corrente di tutti i clienti dell'organizzazione è associato tramite diversi tipi di attribuzione in tutti i prodotti cloud, ad esempio Office, Azure e Dynamics. Un cliente viene conteggiato se ha almeno una sottoscrizione con stato Attivo.  
- % di clienti rifiutati durante l'intervallo di date selezionato 
- Micro chart presents month over month trend of customers count over the selected date range (Micro chart presenta la tendenza mensile dei clienti nell'intervallo di date selezionato)

### <a name="active-customers"></a>Clienti attivi

- Numero corrente di clienti con qualsiasi utilizzo attivo del prodotto, ad esempio l'utilizzo attivo in uno dei prodotti cloud.
- Crescita o diminuzione della % dei clienti attivi durante il periodo di tempo selezionato
- Micro chart presenta una tendenza mensile del numero di clienti attivi nell'intervallo di date selezionato.

### <a name="customers-added"></a>Clienti aggiunti

- Numero di tutti i clienti aggiunti durante il periodo di tempo selezionato.
- Crescita o diminuzione della % dei clienti aggiunti durante l'intervallo di sate selezionato.
- Micro chart presenta la tendenza mensile dei clienti aggiunti nell'intervallo di date selezionato.

### <a name="customers-churned"></a>Clienti che hanno sforato
- Conteggio di tutti i clienti variati ogni mese durante il periodo di tempo selezionato. Un cliente viene considerato perso se non ha una sola sottoscrizione con stato attivo. 
- Percentuale di clienti che hanno variato durante l'intervallo di date selezionato 
- Micro chart presenta la tendenza mensile dei clienti che hanno variato nel periodo di tempo selezionato 
 
### <a name="customers-by-products"></a>Clienti per prodotti

- Numero corrente di clienti distribuiti tra i vari prodotti cloud, ad esempio Office 365, Azure e Dynamics.  

## <a name="geographical-spread-of-your-customers"></a>Distribuzione geografica dei clienti

Il conteggio dei clienti correnti, dei clienti attivi correnti e dei clienti appena aggiunti durante l'intervallo di date selezionato viene mappato geograficamente usando il paese del cliente. Le percentuali visualizzate sotto la metrica indicano il contributo percentuale del paese del totale per tale metrica. È possibile passare il mouse sulla mappa per visualizzare i nuovi clienti attivi e totali per quel paese. È possibile cercare e selezionare un paese nella griglia per fare zoom avanti sulla posizione nella mappa. Ripristinare la visualizzazione originale selezionando il **pulsante Home** sulla mappa. Tutte le colonne nella griglia sono ordinabili.  

:::image type="content" source="images/insights/customer-geography.png" alt-text="Screenshot del report Partner Center Insights cliente per area geografica che mostra la mappa del mondo e l'elenco dei clienti totali, aggiunti e nuovi in base all'area.":::

## <a name="customer-adds-and-churns"></a>Aggiunte e varianza dei clienti

Tendenza dei clienti con suddivisione in nuovi, esistenti e variati per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di clienti. I clienti variati sono rappresentati su una scala negativa dell'asse Y. L'istogramma a colonne in pila presenta la scomposizione dei clienti nuovi, esistenti e variati per il mese. È possibile ricompilare l'istogramma con elementi dello stack specifici, selezionandoli nella legenda. È possibile sfruttare il dispositivo di scorrimento nella parte superiore del grafico per fare zoom avanti su un periodo specifico. 

:::image type="content" source="images/insights/customer-lost.png" alt-text="Screenshot del Partner Center Insights del cliente con grafico a barre che mostra il numero di clienti aggiunti e persi o sforati in un periodo di tempo specifico.":::

## <a name="customer-distribution"></a>Distribuzione dei clienti

Scomposizione dei clienti correnti per località Microsoft Partner Network (MPN), segmenti di clienti, canale di vendita/modello tariffario di Azure e tipo di attribuzione. Selezionare le rispettive schede sopra il grafico per visualizzare la suddivisione in base a queste categorie. È possibile ricompilare il grafico selezionando o deselezionando dimensioni specifiche selezionando gli elementi della legenda. 

## <a name="customers-by-products"></a>Clienti per prodotti

La suddivisione dei clienti correnti viene conteggiato per prodotti e SKU/piani. Selezionare un prodotto nel grafico a torta di scomparti del prodotto per visualizzare la scomposizione in base a SKU/piani nel grafico accanto.

:::image type="content" source="images/insights/customer-by-product.png" alt-text="Screenshot del report Clienti per prodotto che mostra due grafici radiali: uno con scomposizione dei clienti per prodotto, l'altro con scomposizione dei clienti per SKU.":::

## <a name="customer-distribution-trend"></a>Tendenza di distribuzione dei clienti 

Tendenza mensile della distribuzione dei clienti durante l'intervallo di date selezionato per mercati, segmenti, località MPN e prodotti acquisiti. Selezionare le rispettive schede nel grafico per visualizzare la tendenza in base a queste categorie. L'asse X rappresenta i mesi per l'intervallo di date selezionato e l'asse Y include il conteggio dei clienti per la categoria selezionata (selezione della scheda). È possibile passare il mouse sulle colonne del grafico per visualizzare la suddividezione dei valori di ogni stack. È possibile sfruttare il dispositivo di scorrimento nella parte superiore del grafico per fare zoom avanti su un periodo specifico.   

:::image type="content" source="images/insights/customer-by-distribution.png" alt-text="Screenshot del report Delle tendenze di distribuzione dei clienti che mostra i grafici a barre che è possibile visualizzare per mercato, segmento, località partner o prodotti.":::

## <a name="active-customers"></a>Clienti attivi

Grafico di tendenza mensile che confronta i clienti attivi e totali per l'intervallo di date selezionato. Le colonne rappresentano i conteggi dei clienti attivi ogni mese e la riga rappresenta il totale dei clienti ogni mese. 

:::image type="content" source="images/insights/active-customer.png" alt-text="Screenshot del report Partner Center Insights Active customers (Clienti attivi) che mostra i grafici a barre nel tempo dei clienti attivi.":::

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights](partner-center-insights.md).

>[!NOTE]
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report nel dashboard Insights dati. [Altre informazioni](insights-download-reports.md) 
