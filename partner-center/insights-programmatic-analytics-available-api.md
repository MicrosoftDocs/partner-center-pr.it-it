---
title: Elenco di API per l'accesso ai dati delle informazioni dettagliate dei partner
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Elenco di API per l'accesso ai dati delle informazioni dettagliate dei partner.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375571"
---
# <a name="available-apis-for-partner-insights-analytics"></a>API disponibili per l'analisi delle informazioni dettagliate dei partner

Di seguito è riportato l'elenco delle API per l'analisi delle informazioni dettagliate dei partner e le relative funzionalità associate.

## <a name="dataset-pull-apis"></a>API pull del set di dati

***Tabella 1: API pull del set di dati***

| **API** | **Funzionalità** |
| --- | --- |
| [Ottenere tutti i set di dati](insights-programmatic-analytics-api-get-dataset.md) | Ottiene tutti i set di dati disponibili. I set di dati elencano tabelle, colonne, metriche e intervalli di tempo. |
|||

## <a name="query-management-apis"></a>API di gestione delle query

***Tabella 2: API di gestione delle query***

| **API** | **Funzionalità** |
| --- | --- |
| [Creare una query di report](insights-programmatic-access-paradigm.md#create-report-query-api) | Crea query personalizzate che definiscono il set di dati da cui devono essere esportate le colonne e le metriche. |
| [GET Report Query](insights-programmatic-analytics-api-get-report-queries.md) | Ottiene tutte le query disponibili per l'utilizzo nei report. Ottiene tutte le query di sistema e definite dall'utente per impostazione predefinita. |
| [DELETE Report Query](insights-programmatic-analytics-api-delete-report-queries.md) | Elimina le query definite dall'utente. |
|||

## <a name="report-management-apis"></a>API di gestione dei report

***Tabella 3: API di gestione dei report***

| **API** | **Funzionalità** |
| --- | --- |
| [Creazione di report](insights-programmatic-access-paradigm.md#create-report-api) | Pianifica l'esecuzione di una query a intervalli regolari. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Esegue un'istruzione di query Report. Restituisce solo 10 record che un partner può usare per verificare se i dati sono come previsto. |
| [Genera report](insights-programmatic-analytics-api-get-report.md) | Ottenere tutti i report pianificati. |
| [Aggiorna report](insights-programmatic-analytics-api-update-report.md) | Modificare un parametro del report. |
| [Elimina report](insights-programmatic-analytics-api-delete-report.md) | Elimina tutti i record di esecuzione del report e del report. |
| [Sospendere le esecuzioni dei report](insights-programmatic-analytics-api-pause-report-executions.md) | Sospende l'esecuzione pianificata dei report. |
| [Riprendere le esecuzioni dei report](insights-programmatic-analytics-api-resume-report-executions.md) | Riprende l'esecuzione pianificata di un report sospeso. |
|||

## <a name="report-execution-pull-apis"></a>API pull per l'esecuzione di report

***Tabella 4: API pull di esecuzione dei report***

| **API** | **Funzionalità** |
| --- | --- |
| [Ottenere le esecuzioni dei report](insights-programmatic-access-paradigm.md#get-report-execution-api) | Ottiene tutte le esecuzioni che si sono verificato per un determinato report. |
|||

## <a name="next-steps"></a>Passaggi successivi

- È possibile provare le API tramite [l'URL dell'API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).