---
title: Partner Center Insights - Report del cliente
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scoprire i modi per migliorare l'azienda. Visualizzare le tendenze dei clienti specifiche in base all'area geografica, al prodotto e ad altri attributi.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9207e793865bcf7fa2f205fc69b0b5def65b4d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152903"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>Report del dashboard dei clienti Partner Center Insights

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Visualizzatore di report | Visualizzatore di report executive

Il dashboard Clienti presenta i dati dei clienti che hanno acquisito prodotti cloud come Office, Azure, Dynamics e così via tramite l'utente o che hanno usato l'utente per distribuire e gestire questi prodotti nei tenant. 
 
Il dashboard Clienti include le sezioni seguenti: 

- Riepilogo  
- Distribuzione geografica dei clienti 
- I clienti aggiungono/varianza le tendenze 
- Distribuzione dei clienti per località partner, segmenti di clienti, canale di vendita, tipo di attribuzione partner 
- Distribuzione dei clienti per prodotto 
- Tendenze di distribuzione dei clienti per località partner, segmenti di clienti, modello tariffario, tipo di attribuzione partner 
- Tendenza dei clienti attivi 

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot di vari indicatori KPI correlati ai clienti, ad esempio clienti, clienti attivi, sottoscrizioni, clienti aggiunti, clienti variati e clienti per ogni prodotto. I filtri a livello di pagina sono applicabili per ogni sezione.

:::image type="content" source="images/pci/customerproduct.png" alt-text="Screenshot del dashboard Riepilogo clienti che mostra i grafici a barre e il numero di clienti attivi, aggiunti di recente, persi/variati o per prodotto specifico.":::

### <a name="customers"></a>Clienti

- Il numero corrente di tutti i clienti dell'organizzazione è associato tramite diversi tipi di attribuzione in tutti i prodotti cloud, ad esempio Office, Azure, Dynamics e così via. Un cliente viene conteggiato se ha almeno una sottoscrizione con stato Attivo.  
- % di clienti rifiutati durante l'intervallo di date selezionato 
- Il micro chart presenta la tendenza mensile dei clienti che contano sull'intervallo di date selezionato

### <a name="active-customers"></a>Clienti attivi

- Numero corrente di clienti con qualsiasi utilizzo attivo del prodotto, ad esempio l'utilizzo attivo in uno dei prodotti cloud.
- Crescita o diminuzione della % dei clienti attivi durante il periodo di tempo selezionato
- Micro chart presenta una tendenza mensile del numero di clienti attivi nell'intervallo di date selezionato.

### <a name="customers-added"></a>Clienti aggiunti

- Numero di tutti i clienti aggiunti durante il periodo di tempo selezionato.
- Crescita o diminuzione della % dei clienti aggiunti durante l'intervallo di sate selezionato.
- Micro chart presenta la tendenza mensile dei clienti aggiunti nell'intervallo di date selezionato.

### <a name="customers-churned"></a>Clienti che hanno sforato
- Conteggio di tutti i clienti variati ogni mese durante il periodo di tempo selezionato. Un cliente viene considerato perso se non ha una singola sottoscrizione con stato attivo. 
- Percentuale di clienti variati durante l'intervallo di date selezionato 
- Micro chart presenta la tendenza mensile dei clienti che hanno variato nel periodo di tempo selezionato 
 
### <a name="customers-by-products"></a>Clienti per prodotti

- Numero corrente di clienti distribuiti tra i vari prodotti cloud, ad esempio Office 365, Azure, Dynamics e così via.  

## <a name="geographical-spread-of-your-customers"></a>Distribuzione geografica dei clienti

Il conteggio dei clienti correnti, dei clienti attivi correnti e dei clienti appena aggiunti durante l'intervallo di date selezionato viene mappato geograficamente usando il paese del cliente. Le percentuali visualizzate sotto la metrica indicano il contributo percentuale del paese del totale per tale metrica. È possibile passare il mouse sulla mappa per visualizzare i nuovi clienti attivi e totali per quel paese. È possibile cercare e selezionare un paese nella griglia per fare zoom avanti sulla posizione nella mappa. Ripristinare la visualizzazione originale selezionando il **pulsante Home** sulla mappa. Tutte le colonne nella griglia sono ordinabili.  

:::image type="content" source="images/pci/customersgeo.png" alt-text="Screenshot del report Partner Center Insights Customer by geography mostra la mappa del mondo e l'elenco dei clienti totali, aggiunti e nuovi in base all'area geografica.":::

## <a name="customer-adds-and-churns"></a>Il cliente aggiunge e varianza

Tendenza dei clienti con suddivisione in nuovi, esistenti e variati per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di clienti. I clienti variati sono rappresentati su scala negativa dell'asse Y. L'istogramma in pila presenta la suddividenza dei clienti nuovi, esistenti e variati per il mese. È possibile ricompilare l'istogramma con elementi dello stack specifici selezionandoli nella legenda. È possibile sfruttare il dispositivo di scorrimento nella parte superiore del grafico per ingrandire un periodo specifico. 

:::image type="content" source="images/pci/customerslost.png" alt-text="Screenshot del Partner Center del cliente di Insights con grafico a barre che mostra il numero di clienti aggiunti e persi o variati in un periodo di tempo specifico.":::

## <a name="customer-distribution"></a>Distribuzione dei clienti

Suddivisione dei clienti correnti in base a località MPN, segmenti di clienti, canale di vendita/modello tariffario di Azure e tipo di attribuzione ,ad esempio DPOR, DAP. Selezionare le rispettive schede sopra il grafico per visualizzare la suddivisione in base a queste categorie. È possibile ricompilare il grafico selezionando/deselezionando dimensioni specifiche selezionando gli elementi della legenda. 

## <a name="customers-by-products"></a>Clienti in base ai prodotti

La suddivisione dei clienti correnti viene conteggiato in base a prodotti e SKU/piani. Selezionare un prodotto nel grafico a torta di interruzione del prodotto per visualizzare la scomposizione in base a SKU/piani nel grafico accanto.

:::image type="content" source="images/pci/customerbyprod.png" alt-text="Screenshot del report Clienti per prodotto che mostra due grafici radiali: uno con scomposizione dei clienti per prodotto, l'altro con scomposizione dei clienti per SKU.":::

## <a name="customer-distribution-trend"></a>Tendenza di distribuzione dei clienti 

Tendenza mensile della distribuzione dei clienti durante l'intervallo di date selezionato per mercati, segmenti, località MPN e prodotti acquisiti. Selezionare le rispettive schede nel grafico per visualizzare la tendenza in base a queste categorie. L'asse X rappresenta i mesi per l'intervallo di date selezionato e l'asse Y include il conteggio dei clienti per la categoria selezionata (selezione della scheda). È possibile passare il mouse sulle colonne del grafico per visualizzare la suddividezione dei valori di ogni stack. È possibile sfruttare il dispositivo di scorrimento nella parte superiore del grafico per fare zoom avanti su un periodo specifico.   

:::image type="content" source="images/pci/customerdistri.png" alt-text="Screenshot del report Tendenza distribuzione clienti che mostra i grafici a barre che è possibile visualizzare per mercato, segmento, località partner o prodotti.":::

## <a name="active-customers"></a>Clienti attivi

Grafico di tendenza mensile che confronta i clienti attivi e totali per l'intervallo di date selezionato. Le colonne rappresentano i conteggi dei clienti attivi ogni mese e la riga rappresenta il totale dei clienti ogni mese. 

:::image type="content" source="images/pci/activecustomer.png" alt-text="Screenshot del report Partner Center Insights Active customers che mostra i grafici a barre nel tempo dei clienti attivi.":::

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights.](partner-center-insights.md)

>[!NOTE]
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report del dashboard Informazioni dettagliate. [Altre informazioni](pci-download-reports.md) 
