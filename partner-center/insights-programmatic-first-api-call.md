---
title: Effettuare la prima chiamata API per accedere ai dati di analisi delle informazioni dettagliate dei partner
description: Esempi per imparare a usare l'API per accedere ai dati analitici delle informazioni dettagliate dei partner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375355"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Effettuare la prima chiamata API per accedere ai dati di analisi delle informazioni dettagliate dei partner

Per un elenco delle API per l'accesso ai dati analitici delle informazioni dettagliate dei partner, vedere API per l'accesso ai dati analitici [delle informazioni dettagliate dei partner.](insights-programmatic-analytics-available-api.md) Prima di effettuare la prima chiamata API, [](insights-programmatic-prerequisites.md) assicurarsi di aver soddisfatto i prerequisiti per accedere a livello di codice ai dati di analisi Insights partner.

## <a name="token-generation"></a>Generazione di token

Prima di chiamare uno dei metodi, è necessario ottenere un token di accesso Azure Active Directory (AAD). È necessario passare il token Azure AD di accesso all'intestazione Authorization di ogni metodo nell'API. Dopo aver ottenuto un token di accesso, è necessario usarlo per 60 minuti prima della scadenza. Dopo la scadenza del token, è possibile aggiornare il token e continuare a usarlo per altre chiamate all'API.

Fare riferimento a una richiesta di esempio riportata di seguito per la generazione di un token. I tre valori necessari per generare il token sono `clientId` `clientSecret` , e `tenantId` . Il parametro della risorsa deve essere impostato su `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Esempio di richiesta

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Per altre informazioni su come ottenere un token di Azure AD per l'applicazione, vedere Accedere ai dati di analisi usando i [servizi dello Store.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Chiamata API a livello di codice

Dopo aver ottenuto il token AAD come descritto nella sezione precedente, seguire questa procedura per creare il primo report di accesso a livello di codice.

I dati possono essere scaricati dai set di dati seguenti (datasetName):

- CustomersAndTenants
- PostazioniSottoscrizioniAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profilo
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetenzaPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

Nella sezione seguente verranno illustrati esempi di come accedere a livello di codice dal set `SubscriptionId` di dati DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Passaggio 1: Effettuare una chiamata REST usando l'API get datasets

La risposta dell'API fornisce il nome del set di dati da cui è possibile scaricare il report. Per il set di dati specifico, la risposta dell'API fornisce anche l'elenco delle colonne selezionabili che possono essere usate per il modello di report personalizzato. È anche possibile fare riferimento alle [definizioni dei dati](insights-data-definitions.md) per ottenere i nomi delle colonne.

#### <a name="request-example"></a>Esempio di richiesta

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Passaggio 2: Creare la query personalizzata

In questo passaggio si userà SubscriptionId del set di dati DynamicsUsage per creare una query personalizzata per il report desiderato. L'intervallo di tempo predefinito se non specificato nella query è 6 mesi.

#### <a name="request-example"></a>Esempio di richiesta

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Al termine dell'esecuzione della query, viene generato un oggetto che `queryId` deve essere utilizzato per generare il report.

### <a name="step-3-execute-test-query-api"></a>Passaggio 3: Eseguire l'API di query di test

In questo passaggio si userà l'API di query di test per ottenere le prime 100 righe per la query creata.

#### <a name="request-example"></a>Esempio di richiesta

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Passaggio 4: Creare il report

In questo passaggio si userà il Valore QueryId generato in precedenza per creare il report.

#### <a name="request-example"></a>Esempio di richiesta

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
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

Al termine dell'esecuzione, `reportId` viene generato un oggetto che deve essere utilizzato per pianificare un download del report.

### <a name="step-5-execute-report-executions-api"></a>Passaggio 5: Eseguire l'API di esecuzione dei report

In questo passaggio si userà l'API Esecuzioni report per ottenere la posizione sicura (URL) del report.

#### <a name="request-example"></a>Esempio di richiesta

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Esempio di risposta

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Passaggi successivi

- Provare le API tramite [l'URL dell'API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)