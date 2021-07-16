---
title: dashboard Partner Center Insights panoramica
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vedere uno snapshot delle attività di vendita e distribuzione, crescita dei clienti e crescita dei ricavi con licenze, sottoscrizioni e consumo di Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 46a750749aeb6835c132b971b74bb9f066dc13cc
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375493"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Report del dashboard di panoramica disponibili in Insights del Centro per i partner
 
**Ruoli appropriati:** amministratore globale | Agente di amministrazione | Visualizzatore report | Visualizzatore di report executive

Il dashboard Insights panoramica offre una visualizzazione snapshot degli indicatori di prestazioni chiave (KPI), ad esempio clienti, sottoscrizioni, ricavi a consumo di Azure e licenze. È possibile visualizzare i grafici seguenti nel report Panoramica.

- Riepilogo  
- Distribuzione geografica di clienti, sottoscrizioni e licenze  
- Tendenza di crescita dei clienti 
- Tendenza di crescita delle sottoscrizioni 
- Tendenza di crescita dei ricavi utilizzati da Azure 
- Tendenza di crescita delle licenze 

## <a name="summary"></a>Riepilogo

Il riepilogo include informazioni su clienti, ricavi per l'utilizzo di Azure (ACR), sottoscrizioni vendute, sottoscrizioni attive e licenze distribuite. 

:::image type="content" source="images/insights/summary.png" alt-text="Licenze di riepilogo.":::

Di seguito sono riportate altre informazioni su ogni sezione del riepilogo.

### <a name="customers"></a>Clienti

**L'area Clienti** include:

- Numero corrente di tutti i clienti con almeno una sottoscrizione attiva associata all'azienda tramite tipi di attribuzione diversi e in tutti i prodotti cloud.
- Crescita percentuale dei clienti durante l'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile del numero di clienti nell'intervallo di date selezionato.

### <a name="azure-consumed-revenue-acr"></a>ricavi per l'utilizzo di Azure (ACR)

L ricavi per l'utilizzo di Azure di controllo **di accesso (ACR)** nel riepilogo include:

- Record di controllo di accesso totale (in dollari STATUNITENSI) attribuiti all'utente nell'intervallo di date selezionato.
- Crescita o diminuzione della percentuale di record di controllo di accesso attribuiti (in dollari STATUNITENSI) durante l'intervallo di date selezionato.
- Il micro chart presenta una tendenza mensile di Record di controllo di accesso in dollari statunitensi attribuita all'utente nell'intervallo di date selezionato 

> [!NOTE]
> I dati di Registro Controllo di accesso sono disponibili per gli utenti a cui è stato assegnato il ruolo di visualizzatore di report Executive.
 
### <a name="subscriptions-sold"></a>Sottoscrizioni vendute

**L'area Sottoscrizioni** vendute in Riepilogo include:

- Numero totale corrente di sottoscrizioni di prodotti cloud (attive e inattive) vendute o gestite dall'utente.  
- Crescita o diminuzione percentuale delle sottoscrizioni durante l'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile delle sottoscrizioni totali nell'intervallo di date selezionato.

### <a name="active-subscriptions"></a>Sottoscrizioni attive

**L'area Sottoscrizioni** attive in Riepilogo include:

- Numero corrente di sottoscrizioni di prodotti cloud con utilizzo attivo misurato in base ai dati di telemetria del prodotto. Sono escluse tutte le sottoscrizioni di valutazione di Azure.  
- Crescita percentuale delle sottoscrizioni attive nell'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile delle sottoscrizioni attive nell'intervallo di date selezionato.
 
### <a name="licenses-deployed"></a>Licenze distribuite

**L'area Licenze** distribuite in Riepilogo include:
 
- Numero di tutte le licenze dei prodotti cloud distribuite nelle sottoscrizioni dei clienti nel periodo di tempo selezionato. 
- La percentuale di crescita o diminuzione di queste licenze durante l'intervallo di date selezionato. 
- Il micro chart mostra la tendenza mensile del conteggio delle licenze assegnate nell'intervallo di date selezionato.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Distribuzione geografica di clienti, sottoscrizioni e licenze

Questa visualizzazione è una distribuzione geografica del totale di clienti, sottoscrizioni e licenze per paese del cliente. Selezionare le diverse schede per visualizzare ognuna di queste informazioni dettagliate sulla mappa. È possibile cercare e selezionare un paese nella griglia per fare zoom avanti sulla posizione nella mappa. Ripristinare la visualizzazione originale premendo il pulsante Home sulla mappa. Facendo clic su ogni scheda (ad esempio, Clienti, Sottoscrizioni) vengono visualizzati il valore della metrica per ogni paese e la percentuale di Totale per il paese.  

:::image type="content" source="images/insights/geosummary.png" alt-text="Riepilogo geografico.":::

## <a name="customers-growth-trend"></a>Tendenza di crescita dei clienti

Tendenza mensile dei conteggi totali dei clienti per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero totale di clienti per tale mese. 

:::image type="content" source="images/insights/customer-growth.png" alt-text="tendenza di crescita dei clienti.":::

## <a name="subscriptions-growth-trend"></a>Tendenza di crescita delle sottoscrizioni

Indica la tendenza del numero di sottoscrizioni dei clienti per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di sottoscrizioni del prodotto selezionato. Scorrere il dispositivo di scorrimento nella parte superiore del grafico per ingrandire il grafico in base a un periodo di tempo specifico. 

:::image type="content" source="images/insights/subscription-growth.png" alt-text="Tendenza di crescita delle sottoscrizioni.":::

## <a name="azure-consumed-revenue-growth-trend"></a>ricavi per l'utilizzo di Azure tendenza di crescita

Tendenza mensile dei ricavi consumati da Azure in dollari statunitensi attribuiti all'utente nell'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta i ricavi totali utilizzati da Azure in dollari statunitensi attribuiti all'utente durante il mese.

> [!NOTE]
> Registro Controllo di accesso sarà visibile solo agli utenti a cui è stato assegnato il ruolo di visualizzatore di report Executive. 

:::image type="content" source="images/insights/azure-consumed.png" alt-text="Consumo di Azure.":::

## <a name="licenses-growth-trend"></a>Tendenza di crescita delle licenze
 
Tendenza delle licenze assegnate da tutti i clienti durante l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di licenze del prodotto selezionato. Scorrere il dispositivo di scorrimento nella parte superiore del grafico per ingrandire il grafico in base a un periodo di tempo specifico.  

:::image type="content" source="images/insights/licenses-growth.png" alt-text="Licenze.":::

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights](partner-center-insights.md).
