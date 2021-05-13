---
title: dashboard panoramica di Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vedere uno snapshot delle attività di vendita e distribuzione, crescita dei clienti e crescita dei ricavi con licenze, sottoscrizioni e consumo di Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855200"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Report del dashboard di panoramica disponibili in Insights del Centro per i partner
 
**Ruoli appropriati:** Amministratore globale | Agente amministratore | Visualizzatore di report | Visualizzatore di report executive

Il dashboard Panoramica di Insights offre una visualizzazione snapshot degli indicatori di prestazioni chiave, ad esempio clienti, sottoscrizioni, ricavi a consumo di Azure e licenze. È possibile visualizzare i grafici seguenti nel report Panoramica.

- Riepilogo  
- Distribuzione geografica di clienti, sottoscrizioni e licenze  
- Tendenza di crescita dei clienti 
- Tendenza di crescita delle sottoscrizioni 
- Tendenza di crescita dei ricavi consumati in Azure 
- Tendenza di crescita delle licenze 

## <a name="summary"></a>Riepilogo

Il riepilogo include informazioni su clienti, ricavi per l'utilizzo di Azure (ACR), sottoscrizioni vendute, sottoscrizioni attive e licenze distribuite. 

:::image type="content" source="images/pci/summary.png" alt-text="Licenze di riepilogo":::

Di seguito sono riportate altre informazioni su ogni sezione del riepilogo.

### <a name="customers"></a>Clienti

**L'area Clienti** include:

- Numero corrente di tutti i clienti con almeno una sottoscrizione attiva associata all'azienda tramite tipi di attribuzione diversi e in tutti i prodotti cloud.
- Crescita percentuale dei clienti durante l'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile del numero di clienti all'interno dell'intervallo di date selezionato.

### <a name="azure-consumed-revenue-acr"></a>ricavi per l'utilizzo di Azure (ACR)

**L'area ricavi per l'utilizzo di Azure (ACR)** nel riepilogo include:

- Totale dei ricavi per l'utilizzo di Azure (in US $) attribuiti all'utente nell'intervallo di date selezionato.
- Crescita o diminuzione percentuale nel Record di controllo di accesso con attributi (in US $) durante l'intervallo di date selezionato.
- Il micro chart presenta una tendenza mensile di ACR US$ attribuita all'utente nell'intervallo di date selezionato 

> [!NOTE]
> ricavi per l'utilizzo di Azure (ACR) sono disponibili per gli utenti a cui è stato assegnato il ruolo Executive Report Viewer 
 
### <a name="subscriptions-sold"></a>Sottoscrizioni vendute

**L'area Sottoscrizioni** vendute in Riepilogo include:

- Numero totale corrente di sottoscrizioni di prodotti cloud (attive e inattive) vendute o gestite dall'utente.  
- Crescita o diminuzione percentuale delle sottoscrizioni durante l'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile delle sottoscrizioni totali nell'intervallo di date selezionato.

### <a name="active-subscriptions"></a>Sottoscrizioni attive

**L'area Sottoscrizioni** attive in Riepilogo include:

- Numero corrente di sottoscrizioni di prodotti cloud con utilizzo attivo misurato in base ai dati di telemetria del prodotto. Sono escluse tutte le sottoscrizioni di valutazione nel caso di sottoscrizioni di Azure.  
- Crescita percentuale delle sottoscrizioni attive nell'intervallo di date selezionato.
- Il micro chart presenta la tendenza mensile delle sottoscrizioni attive nell'intervallo di date selezionato.
 
### <a name="licenses-deployed"></a>Licenze distribuite

**L'area Licenze** distribuite in Riepilogo include:
 
- Numero di tutte le licenze dei prodotti cloud distribuite nelle sottoscrizioni dei clienti nel periodo di tempo selezionato. 
- La percentuale di crescita o diminuzione di queste licenze durante l'intervallo di date selezionato. 
- Il micro chart mostra la tendenza mensile del conteggio delle licenze assegnate nell'intervallo di date selezionato.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Distribuzione geografica di clienti, sottoscrizioni e licenze

Questa visualizzazione è una distribuzione geografica del totale di clienti, sottoscrizioni e licenze in base al paese del cliente. Selezionare le diverse schede per visualizzare ognuna di queste informazioni dettagliate sulla mappa. È possibile cercare e selezionare un paese nella griglia per ingrandire la posizione nella mappa. Ripristinare la visualizzazione originale premendo il pulsante Home sulla mappa. Facendo clic su ogni scheda, ad esempio Clienti, Sottoscrizioni, vengono visualizzati il valore della metrica per ogni paese e la percentuale di Totale per il paese.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Riepilogo geografico":::

## <a name="customers-growth-trend"></a>Tendenza di crescita dei clienti

Tendenza mensile dei conteggi dei clienti totali per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero totale di clienti per quel mese. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="tendenza di crescita dei clienti":::

## <a name="subscriptions-growth-trend"></a>Tendenza di crescita delle sottoscrizioni

Indica la tendenza del conteggio delle sottoscrizioni dei clienti per l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di sottoscrizioni del prodotto selezionato. Scorrere il dispositivo di scorrimento nella parte superiore del grafico per eseguire lo zoom del grafico su un periodo di tempo specifico. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Tendenza di crescita delle sottoscrizioni":::

## <a name="azure-consumed-revenue-growth-trend"></a>ricavi per l'utilizzo di Azure tendenza di crescita

Tendenza mensile dei ricavi consumati di Azure US$ attribuiti all'utente nell'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il totale dei ricavi consumati di Azure attribuiti all'utente durante il mese.

> [!NOTE]
> ricavi per l'utilizzo di Azure (ACR) sarà visibile solo agli utenti a cui è stato assegnato il ruolo Executive Report Viewer. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Utilizzo di Azure":::

## <a name="licenses-growth-trend"></a>Tendenza di crescita delle licenze
 
Tendenza delle licenze assegnate da tutti i clienti durante l'intervallo di date selezionato. L'asse X rappresenta i mesi dell'intervallo di date selezionato e l'asse Y rappresenta il numero di licenze del prodotto selezionato. Scorrere il dispositivo di scorrimento nella parte superiore del grafico per ingrandire il grafico in base a un periodo di tempo specifico.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licenze":::

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights.](partner-center-insights.md)
