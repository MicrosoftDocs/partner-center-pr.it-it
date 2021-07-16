---
title: Paradigma di accesso a livello di codice per Insights dati
description: Informazioni sul flusso di alto livello del modello di chiamata API per l'analisi a livello di codice. Vengono trattate anche le API per l'accesso ai report di analisi delle informazioni dettagliate dei partner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375383"
---
# <a name="programmatic-access-paradigm"></a>Paradigma di accesso a livello di codice

Questo diagramma illustra il modello di chiamata API usato per creare un nuovo modello di report, pianificare il report personalizzato e recuperare i dati degli errori.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flusso di alto livello":::
***Figura 1: Flusso di alto livello del modello di chiamata API***

Questo elenco fornisce altri dettagli sulla figura 1.

1. L'applicazione client può definire lo schema o il modello di report personalizzato chiamando [l'API Crea query report](#create-report-query-api). In alternativa, è possibile selezionare un modello di report (QueryId) dagli esempi della raccolta di modelli di report [elencati di seguito.](insights-programmatic-system-queries.md)
2. In caso di esito positivo, l'API Crea query report restituisce QueryId.
3. L'applicazione client deve quindi chiamare [l'API](#create-report-api) Crea report usando QueryId insieme alla data di inizio del report, all'intervallo di ripetizione, alla ricorrenza e a un URI di callback facoltativo.
4. In caso di esito positivo, [l'API Crea report](#create-report-api) restituisce ReportId.
5. L'applicazione client riceve una notifica all'URL di callback non appena i dati del report sono pronti per il download.
6. L'applicazione client usa quindi [l'API Get Report Executions](#get-report-execution-api) per eseguire query sullo stato del report con l'ID report e l'intervallo di date.
7. In caso di esito positivo, viene restituito il collegamento di download del report e l'applicazione può avviare il download dei dati.

## <a name="report-query-language-specification"></a>Specifica del linguaggio di query del report

Anche se vengono fornite [query di sistema](insights-programmatic-system-queries.md) che è possibile usare per creare report, è anche possibile creare query personalizzate in base alle esigenze aziendali. Per altre informazioni sulle query personalizzate, vedere [Specifica di query personalizzate](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>CREARE UN'API di query di report

L'API consente di creare query personalizzate che definiscono il set di dati da cui devono essere esportate le colonne e le metriche. L'API offre la flessibilità necessaria per creare un nuovo modello di report in base alle esigenze aziendali.  

È anche possibile usare le [query di sistema](insights-programmatic-system-queries.md) fornite. Quando non sono necessari modelli di report personalizzati, è possibile chiamare direttamente [l'API](#create-report-api) Crea report usando gli Id query delle query di sistema fornite.  

L'esempio seguente illustra come creare una query personalizzata per ottenere i primi 10 clienti in base ai ricavi dell'ultimo mese.

### <a name="request-syntax"></a>Sintassi della richiesta

|    Metodo     |    URI richiesta     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Intestazione della richiesta

|    Intestazione     |    Tipo     |    Descrizione     |
|-------|-----|------|
|    Autorizzazione     |    string |Obbligatorio. Token di Azure Active Directory (Azure AD). Il formato è  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parametro Path

Nessuno

### <a name="query-parameter"></a>Query parameter (Parametro di query)

Nessuno

### <a name="sample-request-payload"></a>Payload di richiesta di esempio

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glossario

Questa tabella fornisce le definizioni chiave degli elementi nel payload della richiesta.

|Parametro|    Obbligatoria     |    Descrizione     |    Valori consentiti     |
|-----|    -----    |    -----    |    -----    |
|Name |    Sì     |    Nome descrittivo della query     |    string     |
|    Descrizione     |    No     |    Descrizione degli elementi restituiti dalla query     |    string     |
|    Query     |    Sì     |    Stringa di query del report     |    Tipo di dati: string <br> [Query personalizzata in](insights-programmatic-custom-query.md) base alle esigenze aziendali |
|        |        |        |        |

> [!Note]
> Per esempi di query personalizzate, vedere [Esempi di query di esempio.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Risposta di esempio

Il payload della risposta è strutturato come segue:

Codici di risposta: 200, 400, 401, 403, 500

Esempio di payload della risposta:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Glossario

Questa tabella fornisce le definizioni chiave degli elementi nel payload della richiesta.

|    Parametro     |    Descrizione     |
|    ----    |    ----    |
|    QueryId     |    Identificatore univoco universale (UUID) della query creata     |
|    Name     |    Nome descrittivo assegnato alla query nel payload della richiesta     |
|    Descrizione     |    Descrizione specificata durante la creazione della query     |
|    Query     |    Query di report passata come input durante la creazione della query     |
|    Tipo     |    Impostare su `userDefined`     |
|    User     |    ID utente usato per creare la query     |
|    CreatedTime     |    Ora UTC in cui la query è stata creata nel formato seguente: aaaa-MM-ggTHH:mm:ssZ     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    StatusCode     |    Codice risultato <br> I valori possibili sono 200, 400, 401, 403, 500     |
|    message     |    Messaggio di stato dall'esecuzione dell'API     |
|        |        |

## <a name="create-report-api"></a>Creare l'API del report

Quando si crea correttamente un modello di report [](#create-report-query-api) personalizzato e si riceve QueryID come parte della risposta Crea query report, questa API può essere chiamata per pianificare l'esecuzione di una query a intervalli regolari. È possibile impostare una frequenza e una pianificazione per il recapito del report.
Per le query di sistema fornite, l'API Crea report può essere chiamata anche con [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>Callback URL (URL callback)

L'API di creazione report accetta un URL di callback. Questo URL verrà chiamato al termine della generazione del report. L'URL di callback deve essere raggiungibile pubblicamente. Oltre all'URL, è anche possibile specificare un metodo di callback. Il metodo di callback può essere solo "GET" o "POST". Il metodo predefinito se non viene passato alcun valore sarà "POST". Il reportId che ha completato la generazione verrà sempre passato nuovamente durante il callback.

Callback POST: se l'URL passato è `https://www.contosso.com/callback` , l'URL richiamato sarà `https://www.contosso.com/callback/<reportID>` 

Callback GET: se l'URL passato è `https://www.contosso.com/callback` , l'URL richiamato sarà `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Report ExecuteNow

È disponibile un provisioning per generare un report senza pianificazione. Il payload dell'API di creazione report può accettare un parametro , che accoderà il report da generare non appena viene chiamata `ExecuteNow` l'API. Quando `ExecuteNow` è impostato su true, i campi , , vengono `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorati perché questi report non sono pianificati.

È possibile passare due campi aggiuntivi quando `ExecuteNow` è true e `QueryStartTime` `QueryEndTime` . Questi due campi eseguiranno l'override `TIMESPAN` del campo nella query. Questi campi non sono applicabili ai report pianificati perché i dati verranno generati continuamente per un periodo di tempo fisso che non cambia.

### <a name="request-syntax"></a>Sintassi della richiesta

|    Metodo     |    URI richiesta     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Intestazione della richiesta

|    Intestazione     |    Tipo     |    Descrizione     |
|-------|-----|------|
|    Autorizzazione     |    string |Obbligatorio. Token di Azure Active Directory (Azure AD). Il formato è  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parametro Path

Nessuno

### <a name="query-parameter"></a>Parametro della query

Nessuno

### <a name="sample-request-payload"></a>Payload di richiesta di esempio

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Glossario

Le definizioni chiave degli elementi nel payload della richiesta sono articolate di seguito:

|    Parametro     |    Obbligatoria     |    Descrizione     |    Valori consentiti     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Sì     |    Nome da assegnare al report     |    string     |
|    Descrizione     |    No     |    Descrizione del report creato     |    string     |
|    QueryId     |    Sì     |    Report query ID     |    string     |
|    StartTime     |    Sì     |    Timestamp UTC in corrispondenza del quale inizierà la generazione del report. <br> Il formato deve essere: aaaa-MM-ggTHH:mm:ssZ       |    string     |
|    ExecuteNow     |    No     |    Questo parametro deve essere usato per creare un report che verrà eseguito una sola volta. `StartTime`e `RecurrenceInterval` `RecurrenceCount` vengono ignorati se è impostato su true. Il report viene eseguito immediatamente in modo asincrono     |    true/false     |
|    QueryStartTime     |    No     |    Facoltativamente, specifica l'ora di inizio per la query che estrae i dati. Questo parametro è applicabile solo per un report di esecuzione una sola volta `ExecuteNow` impostato su true. L'impostazione di questo parametro `TIMESPAN` sostituisce le impostazioni fornite nella query. Il formato deve essere aaaa-MM-ggTHH:mm:ssZ     |    Timestamp come stringa     |
|    QueryEndTime     |    No     |    Facoltativamente, specifica l'ora di fine per la query che estrae i dati. Questo parametro è applicabile solo per un report di esecuzione una sola volta `ExecuteNow` impostato su true. L'impostazione di questo parametro `TIMESPAN` sostituisce le impostazioni fornite nella query. Il formato deve essere aaaa-MM-ggTHH:mm:ssZ     |    Timestamp come stringa     |
|    RecurrenceInterval     |    Sì     |    Frequenza in ore in cui deve essere generato il report. <br> Il valore minimo è 4 e il valore massimo è 2160.      |    numero intero     |
|    RecurrenceCount     |    No     |    Numero di report da generare.     |    numero intero     |
|    Formato     |    No     |    Formato di file del file esportato. <br> Il valore predefinito è CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    URL raggiungibile pubblicamente che può essere configurato facoltativamente come destinazione di callback     |    Stringa (URL HTTP)     |
|    CallbackMethod     |    No     |    Metodo da utilizzare per il callback     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Risposta di esempio

Il payload della risposta è strutturato come segue:

Codici di risposta: 200, 400, 401, 403, 404, 500

Esempio di payload della risposta:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Glossario

Le definizioni chiave degli elementi nella risposta sono articolate di seguito:

|    Parametro     |    Descrizione     |
|    ----    |    ----    |
|    ReportId     |    Identificatore univoco universale (UUID) del report creato     |
|    ReportName     |    Nome assegnato al report nel payload della richiesta     |
|    Descrizione     |    Descrizione specificata durante la creazione del report     |
|    QueryId     |    ID query passato al momento della creazione del report     |
|    Query     |    Testo della query che verrà eseguito per questo report     |
|    User     |    ID utente usato per creare il report     |
|    CreatedTime     |    Ora UTC in cui il report è stato creato nel formato aaaa-MM-ggTHH:mm:ssZ     |
|    ModifiedTime     |    Ora UTC dell'ultima modifica del report nel formato: aaaa-MM-ggTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` flag impostato al momento della creazione del report     |
|    StartTime     |    ORA UTC L'esecuzione del report inizierà nel formato aaaa-MM-ggTHH:mm:ssZ     |
|    Stato report     |    Stato dell'esecuzione del report. I valori possibili sono `Paused` `Active` , e `Inactive`     |
|    RecurrenceInterval     |    Intervallo di ricorrenza specificato durante la creazione del report     |
|    RecurrenceCount     |    Numero di ricorrenze specificato durante la creazione del report.      |
|    CallbackUrl     |    URL di callback specificato nella richiesta     |
|    CallbackMethod     |    Metodo di callback fornito nella richiesta     |
|    Formato     |    Formato dei file di report. I valori possibili sono `CSV` o `TSV` .     |
|    TotalCount     |    Numero di record nella matrice Value     |
|    StatusCode     |    Codice risultato     |
|    message     |    I valori possibili sono 200, 400, 401, 403, 500. Messaggio di stato dall'esecuzione dell'API     |
|        |        |

## <a name="get-report-execution-api"></a>Ottenere l'API di esecuzione del report

È possibile usare questo metodo per eseguire una query sullo stato di esecuzione di un report usando l'ID report ricevuto [dall'API Di creazione report](#create-report-api). Il metodo restituisce il collegamento per il download del report se il report è pronto per il download. In caso contrario, il metodo restituisce lo stato. È anche possibile usare questa API per ottenere tutte le esecuzioni che si sono verificato per un determinato report.  

>[!IMPORTANT]
>Per questa API sono impostati parametri di query predefiniti `executionStatus=Completed` per e `getLatestExecution=true` . Di conseguenza, la chiamata all'API prima della prima esecuzione corretta del report restituirà 404. Le esecuzioni in sospeso possono essere ottenute impostando `executionStatus=Pending` .

### <a name="request-syntax"></a>Sintassi della richiesta

|    Metodo     |    URI richiesta     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Intestazione della richiesta

|    Intestazione     |    Tipo     |    Descrizione     |
|-------|-----|------|
|    Autorizzazione     |    string |Obbligatorio. Token di Azure Active Directory (Azure AD). Il formato è  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parametro Path

|    Nome parametro    |    Obbligatoria    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Sì    |    string    |    Filtrare per ottenere i dettagli di esecuzione solo dei report con il valore reportId specificato in questo argomento. È possibile specificare più reportId separandoli con un punto e virgola ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Query parameter (Parametro di query)

|    Nome parametro    |    Obbligatoria    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    No    |    string    |    Filtrare per ottenere i dettagli solo dei report con il valore executionId specificato in questo argomento. È possibile specificare più executionId separandoli con un punto e virgola ";".    |
|    executionStatus    |    No    |    String/enum    |    Filtrare per ottenere i dettagli solo dei report con executionStatus specificato in questo argomento. <br> I valori validi sono: `Pending` `Running` , e `Paused` `Completed` . <br> Il valore predefinito è `Completed`. <br> È possibile specificare più stati separandoli con un punto e virgola ";".    |
|    getLatestExecution    |    No    |    boolean    |    L'API restituirà i dettagli dell'esecuzione più recente. Per impostazione predefinita, questo parametro è impostato su true.<br> Se si sceglie di passare il valore di questo parametro come false, l'API restituirà le istanze di esecuzione degli ultimi 90 giorni.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Payload di richiesta di esempio

Nessuno

### <a name="sample-response"></a>Risposta di esempio

Il payload della risposta è strutturato come segue:

Codici di risposta: 200, 400, 401, 403, 404, 500

Esempio di payload della risposta:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Al termine dell'esecuzione del report, viene visualizzato lo `Completed` stato di esecuzione. È possibile scaricare il report selezionando l'URL in `reportAccessSecureLink` .

### <a name="glossary"></a>Glossario

Definizioni chiave degli elementi nella risposta.

|    Parametro    |    Descrizione    |
|    ----    |    ----    |
|    ExecutionId    |    Identificatore univoco universale (UUID) dell'istanza di esecuzione    |
|    ReportId    |    ID report associato all'istanza di esecuzione    |
|    RecurrenceInterval    |    Intervallo di ricorrenza specificato durante la creazione del report    |
|    RecurrenceCount    |    Numero di ricorrenze specificato durante la creazione del report    |
|    CallbackUrl    |    URL di callback associato all'istanza di esecuzione    |
|    CallbackMethod    |    Metodo di callback associato all'istanza di esecuzione    |
|    Formato    |    Formato del file generato alla fine dell'esecuzione    |
|    ExecutionStatus    |    Stato dell'istanza di esecuzione del report. <br> I valori validi sono: `Pending` `Running` , , `Paused` e `Completed`    |
|    ReportAccessSecureLink    |Collegamento tramite il quale è possibile accedere al report in modo sicuro        |
|    ReportExpiryTime    |    Ora UTC dopo la quale il collegamento al report scadrà nel formato seguente: aaaa-MM-ggTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Ora UTC in cui il report è stato generato nel formato seguente: aaaa-MM-ggTHH:mm:ssZ    |
|    TotalCount    |    Numero di set di dati nella matrice Value    |
|    StatusCode    |    Codice risultato <br> I valori possibili sono 200, 400, 401, 403, 404 e 500    |
|    message    |    Messaggio di stato dall'esecuzione dell'API    |
|        |        |

## <a name="next-steps"></a>Passaggi successivi

- Provare le API tramite [l'URL dell'API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Effettuare la prima chiamata API](insights-programmatic-first-api-call.md)