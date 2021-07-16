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
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="2fa66-104">Paradigma di accesso a livello di codice</span><span class="sxs-lookup"><span data-stu-id="2fa66-104">Programmatic access paradigm</span></span>

<span data-ttu-id="2fa66-105">Questo diagramma illustra il modello di chiamata API usato per creare un nuovo modello di report, pianificare il report personalizzato e recuperare i dati degli errori.</span><span class="sxs-lookup"><span data-stu-id="2fa66-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flusso di alto livello":::
<span data-ttu-id="2fa66-107">***Figura 1: Flusso di alto livello del modello di chiamata API***</span><span class="sxs-lookup"><span data-stu-id="2fa66-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="2fa66-108">Questo elenco fornisce altri dettagli sulla figura 1.</span><span class="sxs-lookup"><span data-stu-id="2fa66-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="2fa66-109">L'applicazione client può definire lo schema o il modello di report personalizzato chiamando [l'API Crea query report](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="2fa66-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="2fa66-110">In alternativa, è possibile selezionare un modello di report (QueryId) dagli esempi della raccolta di modelli di report [elencati di seguito.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="2fa66-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="2fa66-111">In caso di esito positivo, l'API Crea query report restituisce QueryId.</span><span class="sxs-lookup"><span data-stu-id="2fa66-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="2fa66-112">L'applicazione client deve quindi chiamare [l'API](#create-report-api) Crea report usando QueryId insieme alla data di inizio del report, all'intervallo di ripetizione, alla ricorrenza e a un URI di callback facoltativo.</span><span class="sxs-lookup"><span data-stu-id="2fa66-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="2fa66-113">In caso di esito positivo, [l'API Crea report](#create-report-api) restituisce ReportId.</span><span class="sxs-lookup"><span data-stu-id="2fa66-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="2fa66-114">L'applicazione client riceve una notifica all'URL di callback non appena i dati del report sono pronti per il download.</span><span class="sxs-lookup"><span data-stu-id="2fa66-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="2fa66-115">L'applicazione client usa quindi [l'API Get Report Executions](#get-report-execution-api) per eseguire query sullo stato del report con l'ID report e l'intervallo di date.</span><span class="sxs-lookup"><span data-stu-id="2fa66-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="2fa66-116">In caso di esito positivo, viene restituito il collegamento di download del report e l'applicazione può avviare il download dei dati.</span><span class="sxs-lookup"><span data-stu-id="2fa66-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="2fa66-117">Specifica del linguaggio di query del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-117">Report query language specification</span></span>

<span data-ttu-id="2fa66-118">Anche se vengono fornite [query di sistema](insights-programmatic-system-queries.md) che è possibile usare per creare report, è anche possibile creare query personalizzate in base alle esigenze aziendali.</span><span class="sxs-lookup"><span data-stu-id="2fa66-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="2fa66-119">Per altre informazioni sulle query personalizzate, vedere [Specifica di query personalizzate](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="2fa66-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="2fa66-120">CREARE UN'API di query di report</span><span class="sxs-lookup"><span data-stu-id="2fa66-120">Create report query API</span></span>

<span data-ttu-id="2fa66-121">L'API consente di creare query personalizzate che definiscono il set di dati da cui devono essere esportate le colonne e le metriche.</span><span class="sxs-lookup"><span data-stu-id="2fa66-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="2fa66-122">L'API offre la flessibilità necessaria per creare un nuovo modello di report in base alle esigenze aziendali.</span><span class="sxs-lookup"><span data-stu-id="2fa66-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="2fa66-123">È anche possibile usare le [query di sistema](insights-programmatic-system-queries.md) fornite.</span><span class="sxs-lookup"><span data-stu-id="2fa66-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="2fa66-124">Quando non sono necessari modelli di report personalizzati, è possibile chiamare direttamente [l'API](#create-report-api) Crea report usando gli Id query delle query di sistema fornite.</span><span class="sxs-lookup"><span data-stu-id="2fa66-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="2fa66-125">L'esempio seguente illustra come creare una query personalizzata per ottenere i primi 10 clienti in base ai ricavi dell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="2fa66-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2fa66-126">Sintassi della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-126">Request syntax</span></span>

|    <span data-ttu-id="2fa66-127">Metodo</span><span class="sxs-lookup"><span data-stu-id="2fa66-127">Method</span></span>     |    <span data-ttu-id="2fa66-128">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2fa66-129">POST</span><span class="sxs-lookup"><span data-stu-id="2fa66-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="2fa66-130">Intestazione della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-130">Request header</span></span>

|    <span data-ttu-id="2fa66-131">Intestazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-131">Header</span></span>     |    <span data-ttu-id="2fa66-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-132">Type</span></span>     |    <span data-ttu-id="2fa66-133">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2fa66-134">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-134">Authorization</span></span>     |    <span data-ttu-id="2fa66-135">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-135">string</span></span> |<span data-ttu-id="2fa66-136">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="2fa66-136">Required.</span></span> <span data-ttu-id="2fa66-137">Token di Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2fa66-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2fa66-138">Il formato è  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2fa66-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fa66-139">Content-Type</span></span>     |<span data-ttu-id="2fa66-140">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="2fa66-141">Parametro Path</span><span class="sxs-lookup"><span data-stu-id="2fa66-141">Path parameter</span></span>

<span data-ttu-id="2fa66-142">Nessuno</span><span class="sxs-lookup"><span data-stu-id="2fa66-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="2fa66-143">Query parameter (Parametro di query)</span><span class="sxs-lookup"><span data-stu-id="2fa66-143">Query parameter</span></span>

<span data-ttu-id="2fa66-144">Nessuno</span><span class="sxs-lookup"><span data-stu-id="2fa66-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="2fa66-145">Payload di richiesta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="2fa66-146">Glossario</span><span class="sxs-lookup"><span data-stu-id="2fa66-146">Glossary</span></span>

<span data-ttu-id="2fa66-147">Questa tabella fornisce le definizioni chiave degli elementi nel payload della richiesta.</span><span class="sxs-lookup"><span data-stu-id="2fa66-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="2fa66-148">Parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-148">Parameter</span></span>|    <span data-ttu-id="2fa66-149">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="2fa66-149">Required</span></span>     |    <span data-ttu-id="2fa66-150">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-150">Description</span></span>     |    <span data-ttu-id="2fa66-151">Valori consentiti</span><span class="sxs-lookup"><span data-stu-id="2fa66-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="2fa66-152">Name</span><span class="sxs-lookup"><span data-stu-id="2fa66-152">Name</span></span> |    <span data-ttu-id="2fa66-153">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-153">Yes</span></span>     |    <span data-ttu-id="2fa66-154">Nome descrittivo della query</span><span class="sxs-lookup"><span data-stu-id="2fa66-154">Friendly name of the query</span></span>     |    <span data-ttu-id="2fa66-155">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-155">string</span></span>     |
|    <span data-ttu-id="2fa66-156">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-156">Description</span></span>     |    <span data-ttu-id="2fa66-157">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-157">No</span></span>     |    <span data-ttu-id="2fa66-158">Descrizione degli elementi restituiti dalla query</span><span class="sxs-lookup"><span data-stu-id="2fa66-158">Description of what the query returns</span></span>     |    <span data-ttu-id="2fa66-159">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-159">string</span></span>     |
|    <span data-ttu-id="2fa66-160">Query</span><span class="sxs-lookup"><span data-stu-id="2fa66-160">Query</span></span>     |    <span data-ttu-id="2fa66-161">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-161">Yes</span></span>     |    <span data-ttu-id="2fa66-162">Stringa di query del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-162">Report query string</span></span>     |    <span data-ttu-id="2fa66-163">Tipo di dati: string</span><span class="sxs-lookup"><span data-stu-id="2fa66-163">Data type: string</span></span> <br> <span data-ttu-id="2fa66-164">[Query personalizzata in](insights-programmatic-custom-query.md) base alle esigenze aziendali</span><span class="sxs-lookup"><span data-stu-id="2fa66-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="2fa66-165">Per esempi di query personalizzate, vedere [Esempi di query di esempio.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="2fa66-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="2fa66-166">Risposta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-166">Sample response</span></span>

<span data-ttu-id="2fa66-167">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="2fa66-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="2fa66-168">Codici di risposta: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="2fa66-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="2fa66-169">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="2fa66-169">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2fa66-170">Glossario</span><span class="sxs-lookup"><span data-stu-id="2fa66-170">Glossary</span></span>

<span data-ttu-id="2fa66-171">Questa tabella fornisce le definizioni chiave degli elementi nel payload della richiesta.</span><span class="sxs-lookup"><span data-stu-id="2fa66-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="2fa66-172">Parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-172">Parameter</span></span>     |    <span data-ttu-id="2fa66-173">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="2fa66-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="2fa66-174">QueryId</span></span>     |    <span data-ttu-id="2fa66-175">Identificatore univoco universale (UUID) della query creata</span><span class="sxs-lookup"><span data-stu-id="2fa66-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="2fa66-176">Name</span><span class="sxs-lookup"><span data-stu-id="2fa66-176">Name</span></span>     |    <span data-ttu-id="2fa66-177">Nome descrittivo assegnato alla query nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="2fa66-178">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-178">Description</span></span>     |    <span data-ttu-id="2fa66-179">Descrizione specificata durante la creazione della query</span><span class="sxs-lookup"><span data-stu-id="2fa66-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="2fa66-180">Query</span><span class="sxs-lookup"><span data-stu-id="2fa66-180">Query</span></span>     |    <span data-ttu-id="2fa66-181">Query di report passata come input durante la creazione della query</span><span class="sxs-lookup"><span data-stu-id="2fa66-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="2fa66-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-182">Type</span></span>     |    <span data-ttu-id="2fa66-183">Impostare su `userDefined`</span><span class="sxs-lookup"><span data-stu-id="2fa66-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="2fa66-184">User</span><span class="sxs-lookup"><span data-stu-id="2fa66-184">User</span></span>     |    <span data-ttu-id="2fa66-185">ID utente usato per creare la query</span><span class="sxs-lookup"><span data-stu-id="2fa66-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="2fa66-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-186">CreatedTime</span></span>     |    <span data-ttu-id="2fa66-187">Ora UTC in cui la query è stata creata nel formato seguente: aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2fa66-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-188">TotalCount</span></span>     |    <span data-ttu-id="2fa66-189">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="2fa66-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2fa66-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2fa66-190">StatusCode</span></span>     |    <span data-ttu-id="2fa66-191">Codice risultato</span><span class="sxs-lookup"><span data-stu-id="2fa66-191">Result Code</span></span> <br> <span data-ttu-id="2fa66-192">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="2fa66-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="2fa66-193">message</span><span class="sxs-lookup"><span data-stu-id="2fa66-193">message</span></span>     |    <span data-ttu-id="2fa66-194">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="2fa66-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="2fa66-195">Creare l'API del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-195">Create report API</span></span>

<span data-ttu-id="2fa66-196">Quando si crea correttamente un modello di report [](#create-report-query-api) personalizzato e si riceve QueryID come parte della risposta Crea query report, questa API può essere chiamata per pianificare l'esecuzione di una query a intervalli regolari.</span><span class="sxs-lookup"><span data-stu-id="2fa66-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="2fa66-197">È possibile impostare una frequenza e una pianificazione per il recapito del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="2fa66-198">Per le query di sistema fornite, l'API Crea report può essere chiamata anche con [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="2fa66-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="2fa66-199">Callback URL (URL callback)</span><span class="sxs-lookup"><span data-stu-id="2fa66-199">Callback URL</span></span>

<span data-ttu-id="2fa66-200">L'API di creazione report accetta un URL di callback.</span><span class="sxs-lookup"><span data-stu-id="2fa66-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="2fa66-201">Questo URL verrà chiamato al termine della generazione del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="2fa66-202">L'URL di callback deve essere raggiungibile pubblicamente.</span><span class="sxs-lookup"><span data-stu-id="2fa66-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="2fa66-203">Oltre all'URL, è anche possibile specificare un metodo di callback.</span><span class="sxs-lookup"><span data-stu-id="2fa66-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="2fa66-204">Il metodo di callback può essere solo "GET" o "POST".</span><span class="sxs-lookup"><span data-stu-id="2fa66-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="2fa66-205">Il metodo predefinito se non viene passato alcun valore sarà "POST".</span><span class="sxs-lookup"><span data-stu-id="2fa66-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="2fa66-206">Il reportId che ha completato la generazione verrà sempre passato nuovamente durante il callback.</span><span class="sxs-lookup"><span data-stu-id="2fa66-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="2fa66-207">Callback POST: se l'URL passato è `https://www.contosso.com/callback` , l'URL richiamato sarà `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="2fa66-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="2fa66-208">Callback GET: se l'URL passato è `https://www.contosso.com/callback` , l'URL richiamato sarà `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="2fa66-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="2fa66-209">Report ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2fa66-209">ExecuteNow reports</span></span>

<span data-ttu-id="2fa66-210">È disponibile un provisioning per generare un report senza pianificazione.</span><span class="sxs-lookup"><span data-stu-id="2fa66-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="2fa66-211">Il payload dell'API di creazione report può accettare un parametro , che accoderà il report da generare non appena viene chiamata `ExecuteNow` l'API.</span><span class="sxs-lookup"><span data-stu-id="2fa66-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="2fa66-212">Quando `ExecuteNow` è impostato su true, i campi , , vengono `StartTime` `RecurrenceCount` `RecurrenceInterval` ignorati perché questi report non sono pianificati.</span><span class="sxs-lookup"><span data-stu-id="2fa66-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="2fa66-213">È possibile passare due campi aggiuntivi quando `ExecuteNow` è true e `QueryStartTime` `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="2fa66-214">Questi due campi eseguiranno l'override `TIMESPAN` del campo nella query.</span><span class="sxs-lookup"><span data-stu-id="2fa66-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="2fa66-215">Questi campi non sono applicabili ai report pianificati perché i dati verranno generati continuamente per un periodo di tempo fisso che non cambia.</span><span class="sxs-lookup"><span data-stu-id="2fa66-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2fa66-216">Sintassi della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-216">Request syntax</span></span>

|    <span data-ttu-id="2fa66-217">Metodo</span><span class="sxs-lookup"><span data-stu-id="2fa66-217">Method</span></span>     |    <span data-ttu-id="2fa66-218">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2fa66-219">POST</span><span class="sxs-lookup"><span data-stu-id="2fa66-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="2fa66-220">Intestazione della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-220">Request header</span></span>

|    <span data-ttu-id="2fa66-221">Intestazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-221">Header</span></span>     |    <span data-ttu-id="2fa66-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-222">Type</span></span>     |    <span data-ttu-id="2fa66-223">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2fa66-224">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-224">Authorization</span></span>     |    <span data-ttu-id="2fa66-225">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-225">string</span></span> |<span data-ttu-id="2fa66-226">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="2fa66-226">Required.</span></span> <span data-ttu-id="2fa66-227">Token di Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2fa66-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2fa66-228">Il formato è  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2fa66-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fa66-229">Content-Type</span></span>     |<span data-ttu-id="2fa66-230">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="2fa66-231">Parametro Path</span><span class="sxs-lookup"><span data-stu-id="2fa66-231">Path Parameter</span></span>

<span data-ttu-id="2fa66-232">Nessuno</span><span class="sxs-lookup"><span data-stu-id="2fa66-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="2fa66-233">Parametro della query</span><span class="sxs-lookup"><span data-stu-id="2fa66-233">Query Parameter</span></span>

<span data-ttu-id="2fa66-234">Nessuno</span><span class="sxs-lookup"><span data-stu-id="2fa66-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="2fa66-235">Payload di richiesta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-235">Sample request payload</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2fa66-236">Glossario</span><span class="sxs-lookup"><span data-stu-id="2fa66-236">Glossary</span></span>

<span data-ttu-id="2fa66-237">Le definizioni chiave degli elementi nel payload della richiesta sono articolate di seguito:</span><span class="sxs-lookup"><span data-stu-id="2fa66-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="2fa66-238">Parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-238">Parameter</span></span>     |    <span data-ttu-id="2fa66-239">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="2fa66-239">Required</span></span>     |    <span data-ttu-id="2fa66-240">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-240">Description</span></span>     |    <span data-ttu-id="2fa66-241">Valori consentiti</span><span class="sxs-lookup"><span data-stu-id="2fa66-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2fa66-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="2fa66-242">ReportName</span></span>     |    <span data-ttu-id="2fa66-243">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-243">Yes</span></span>     |    <span data-ttu-id="2fa66-244">Nome da assegnare al report</span><span class="sxs-lookup"><span data-stu-id="2fa66-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="2fa66-245">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-245">string</span></span>     |
|    <span data-ttu-id="2fa66-246">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-246">Description</span></span>     |    <span data-ttu-id="2fa66-247">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-247">No</span></span>     |    <span data-ttu-id="2fa66-248">Descrizione del report creato</span><span class="sxs-lookup"><span data-stu-id="2fa66-248">Description of the created report</span></span>     |    <span data-ttu-id="2fa66-249">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-249">string</span></span>     |
|    <span data-ttu-id="2fa66-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="2fa66-250">QueryId</span></span>     |    <span data-ttu-id="2fa66-251">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-251">Yes</span></span>     |    <span data-ttu-id="2fa66-252">Report query ID</span><span class="sxs-lookup"><span data-stu-id="2fa66-252">Report query ID</span></span>     |    <span data-ttu-id="2fa66-253">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-253">string</span></span>     |
|    <span data-ttu-id="2fa66-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-254">StartTime</span></span>     |    <span data-ttu-id="2fa66-255">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-255">Yes</span></span>     |    <span data-ttu-id="2fa66-256">Timestamp UTC in corrispondenza del quale inizierà la generazione del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="2fa66-257">Il formato deve essere: aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="2fa66-258">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-258">string</span></span>     |
|    <span data-ttu-id="2fa66-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2fa66-259">ExecuteNow</span></span>     |    <span data-ttu-id="2fa66-260">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-260">No</span></span>     |    <span data-ttu-id="2fa66-261">Questo parametro deve essere usato per creare un report che verrà eseguito una sola volta.</span><span class="sxs-lookup"><span data-stu-id="2fa66-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="2fa66-262">`StartTime`e `RecurrenceInterval` `RecurrenceCount` vengono ignorati se è impostato su true.</span><span class="sxs-lookup"><span data-stu-id="2fa66-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="2fa66-263">Il report viene eseguito immediatamente in modo asincrono</span><span class="sxs-lookup"><span data-stu-id="2fa66-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="2fa66-264">true/false</span><span class="sxs-lookup"><span data-stu-id="2fa66-264">true/false</span></span>     |
|    <span data-ttu-id="2fa66-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-265">QueryStartTime</span></span>     |    <span data-ttu-id="2fa66-266">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-266">No</span></span>     |    <span data-ttu-id="2fa66-267">Facoltativamente, specifica l'ora di inizio per la query che estrae i dati.</span><span class="sxs-lookup"><span data-stu-id="2fa66-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="2fa66-268">Questo parametro è applicabile solo per un report di esecuzione una sola volta `ExecuteNow` impostato su true.</span><span class="sxs-lookup"><span data-stu-id="2fa66-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="2fa66-269">L'impostazione di questo parametro `TIMESPAN` sostituisce le impostazioni fornite nella query.</span><span class="sxs-lookup"><span data-stu-id="2fa66-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="2fa66-270">Il formato deve essere aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="2fa66-271">Timestamp come stringa</span><span class="sxs-lookup"><span data-stu-id="2fa66-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="2fa66-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-272">QueryEndTime</span></span>     |    <span data-ttu-id="2fa66-273">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-273">No</span></span>     |    <span data-ttu-id="2fa66-274">Facoltativamente, specifica l'ora di fine per la query che estrae i dati.</span><span class="sxs-lookup"><span data-stu-id="2fa66-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="2fa66-275">Questo parametro è applicabile solo per un report di esecuzione una sola volta `ExecuteNow` impostato su true.</span><span class="sxs-lookup"><span data-stu-id="2fa66-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="2fa66-276">L'impostazione di questo parametro `TIMESPAN` sostituisce le impostazioni fornite nella query.</span><span class="sxs-lookup"><span data-stu-id="2fa66-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="2fa66-277">Il formato deve essere aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="2fa66-278">Timestamp come stringa</span><span class="sxs-lookup"><span data-stu-id="2fa66-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="2fa66-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2fa66-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="2fa66-280">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-280">Yes</span></span>     |    <span data-ttu-id="2fa66-281">Frequenza in ore in cui deve essere generato il report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="2fa66-282">Il valore minimo è 4 e il valore massimo è 2160.</span><span class="sxs-lookup"><span data-stu-id="2fa66-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="2fa66-283">numero intero</span><span class="sxs-lookup"><span data-stu-id="2fa66-283">integer</span></span>     |
|    <span data-ttu-id="2fa66-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-284">RecurrenceCount</span></span>     |    <span data-ttu-id="2fa66-285">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-285">No</span></span>     |    <span data-ttu-id="2fa66-286">Numero di report da generare.</span><span class="sxs-lookup"><span data-stu-id="2fa66-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="2fa66-287">numero intero</span><span class="sxs-lookup"><span data-stu-id="2fa66-287">integer</span></span>     |
|    <span data-ttu-id="2fa66-288">Formato</span><span class="sxs-lookup"><span data-stu-id="2fa66-288">Format</span></span>     |    <span data-ttu-id="2fa66-289">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-289">No</span></span>     |    <span data-ttu-id="2fa66-290">Formato di file del file esportato.</span><span class="sxs-lookup"><span data-stu-id="2fa66-290">File format of the exported file.</span></span> <br> <span data-ttu-id="2fa66-291">Il valore predefinito è CSV.</span><span class="sxs-lookup"><span data-stu-id="2fa66-291">Default is CSV.</span></span>    |    <span data-ttu-id="2fa66-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="2fa66-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="2fa66-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2fa66-293">CallbackUrl</span></span>     |    <span data-ttu-id="2fa66-294">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-294">No</span></span>     |    <span data-ttu-id="2fa66-295">URL raggiungibile pubblicamente che può essere configurato facoltativamente come destinazione di callback</span><span class="sxs-lookup"><span data-stu-id="2fa66-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="2fa66-296">Stringa (URL HTTP)</span><span class="sxs-lookup"><span data-stu-id="2fa66-296">String (http URL)</span></span>     |
|    <span data-ttu-id="2fa66-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2fa66-297">CallbackMethod</span></span>     |    <span data-ttu-id="2fa66-298">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-298">No</span></span>     |    <span data-ttu-id="2fa66-299">Metodo da utilizzare per il callback</span><span class="sxs-lookup"><span data-stu-id="2fa66-299">The method to be used for callback</span></span>     |    <span data-ttu-id="2fa66-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="2fa66-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="2fa66-301">Risposta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-301">Sample response</span></span>

<span data-ttu-id="2fa66-302">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="2fa66-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="2fa66-303">Codici di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2fa66-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2fa66-304">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="2fa66-304">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="2fa66-305">Glossario</span><span class="sxs-lookup"><span data-stu-id="2fa66-305">Glossary</span></span>

<span data-ttu-id="2fa66-306">Le definizioni chiave degli elementi nella risposta sono articolate di seguito:</span><span class="sxs-lookup"><span data-stu-id="2fa66-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="2fa66-307">Parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-307">Parameter</span></span>     |    <span data-ttu-id="2fa66-308">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="2fa66-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="2fa66-309">ReportId</span></span>     |    <span data-ttu-id="2fa66-310">Identificatore univoco universale (UUID) del report creato</span><span class="sxs-lookup"><span data-stu-id="2fa66-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="2fa66-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="2fa66-311">ReportName</span></span>     |    <span data-ttu-id="2fa66-312">Nome assegnato al report nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="2fa66-313">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-313">Description</span></span>     |    <span data-ttu-id="2fa66-314">Descrizione specificata durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="2fa66-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="2fa66-315">QueryId</span></span>     |    <span data-ttu-id="2fa66-316">ID query passato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="2fa66-317">Query</span><span class="sxs-lookup"><span data-stu-id="2fa66-317">Query</span></span>     |    <span data-ttu-id="2fa66-318">Testo della query che verrà eseguito per questo report</span><span class="sxs-lookup"><span data-stu-id="2fa66-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="2fa66-319">User</span><span class="sxs-lookup"><span data-stu-id="2fa66-319">User</span></span>     |    <span data-ttu-id="2fa66-320">ID utente usato per creare il report</span><span class="sxs-lookup"><span data-stu-id="2fa66-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="2fa66-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-321">CreatedTime</span></span>     |    <span data-ttu-id="2fa66-322">Ora UTC in cui il report è stato creato nel formato aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2fa66-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-323">ModifiedTime</span></span>     |    <span data-ttu-id="2fa66-324">Ora UTC dell'ultima modifica del report nel formato: aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2fa66-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2fa66-325">ExecuteNow</span></span>     |    <span data-ttu-id="2fa66-326">`ExecuteNow` flag impostato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="2fa66-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-327">StartTime</span></span>     |    <span data-ttu-id="2fa66-328">ORA UTC L'esecuzione del report inizierà nel formato aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2fa66-329">Stato report</span><span class="sxs-lookup"><span data-stu-id="2fa66-329">ReportStatus</span></span>     |    <span data-ttu-id="2fa66-330">Stato dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-330">Status of the report execution.</span></span> <span data-ttu-id="2fa66-331">I valori possibili sono `Paused` `Active` , e `Inactive`</span><span class="sxs-lookup"><span data-stu-id="2fa66-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="2fa66-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2fa66-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="2fa66-333">Intervallo di ricorrenza specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="2fa66-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-334">RecurrenceCount</span></span>     |    <span data-ttu-id="2fa66-335">Numero di ricorrenze specificato durante la creazione del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="2fa66-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2fa66-336">CallbackUrl</span></span>     |    <span data-ttu-id="2fa66-337">URL di callback specificato nella richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="2fa66-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2fa66-338">CallbackMethod</span></span>     |    <span data-ttu-id="2fa66-339">Metodo di callback fornito nella richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="2fa66-340">Formato</span><span class="sxs-lookup"><span data-stu-id="2fa66-340">Format</span></span>     |    <span data-ttu-id="2fa66-341">Formato dei file di report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-341">Format of the report files.</span></span> <span data-ttu-id="2fa66-342">I valori possibili sono `CSV` o `TSV` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="2fa66-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-343">TotalCount</span></span>     |    <span data-ttu-id="2fa66-344">Numero di record nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="2fa66-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="2fa66-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2fa66-345">StatusCode</span></span>     |    <span data-ttu-id="2fa66-346">Codice risultato</span><span class="sxs-lookup"><span data-stu-id="2fa66-346">Result Code</span></span>     |
|    <span data-ttu-id="2fa66-347">message</span><span class="sxs-lookup"><span data-stu-id="2fa66-347">message</span></span>     |    <span data-ttu-id="2fa66-348">I valori possibili sono 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="2fa66-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="2fa66-349">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="2fa66-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="2fa66-350">Ottenere l'API di esecuzione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-350">Get report execution API</span></span>

<span data-ttu-id="2fa66-351">È possibile usare questo metodo per eseguire una query sullo stato di esecuzione di un report usando l'ID report ricevuto [dall'API Di creazione report](#create-report-api).</span><span class="sxs-lookup"><span data-stu-id="2fa66-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="2fa66-352">Il metodo restituisce il collegamento per il download del report se il report è pronto per il download.</span><span class="sxs-lookup"><span data-stu-id="2fa66-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="2fa66-353">In caso contrario, il metodo restituisce lo stato.</span><span class="sxs-lookup"><span data-stu-id="2fa66-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="2fa66-354">È anche possibile usare questa API per ottenere tutte le esecuzioni che si sono verificato per un determinato report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="2fa66-355">Per questa API sono impostati parametri di query predefiniti `executionStatus=Completed` per e `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="2fa66-356">Di conseguenza, la chiamata all'API prima della prima esecuzione corretta del report restituirà 404.</span><span class="sxs-lookup"><span data-stu-id="2fa66-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="2fa66-357">Le esecuzioni in sospeso possono essere ottenute impostando `executionStatus=Pending` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="2fa66-358">Sintassi della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-358">Request syntax</span></span>

|    <span data-ttu-id="2fa66-359">Metodo</span><span class="sxs-lookup"><span data-stu-id="2fa66-359">Method</span></span>     |    <span data-ttu-id="2fa66-360">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="2fa66-361">GET</span><span class="sxs-lookup"><span data-stu-id="2fa66-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="2fa66-362">Intestazione della richiesta</span><span class="sxs-lookup"><span data-stu-id="2fa66-362">Request header</span></span>

|    <span data-ttu-id="2fa66-363">Intestazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-363">Header</span></span>     |    <span data-ttu-id="2fa66-364">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-364">Type</span></span>     |    <span data-ttu-id="2fa66-365">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="2fa66-366">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="2fa66-366">Authorization</span></span>     |    <span data-ttu-id="2fa66-367">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-367">string</span></span> |<span data-ttu-id="2fa66-368">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="2fa66-368">Required.</span></span> <span data-ttu-id="2fa66-369">Token di Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2fa66-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="2fa66-370">Il formato è  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="2fa66-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fa66-371">Content-Type</span></span>     |<span data-ttu-id="2fa66-372">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="2fa66-373">Parametro Path</span><span class="sxs-lookup"><span data-stu-id="2fa66-373">Path parameter</span></span>

|    <span data-ttu-id="2fa66-374">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-374">Parameter Name</span></span>    |    <span data-ttu-id="2fa66-375">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="2fa66-375">Required</span></span>    |    <span data-ttu-id="2fa66-376">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-376">Type</span></span>    |    <span data-ttu-id="2fa66-377">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2fa66-378">reportId</span><span class="sxs-lookup"><span data-stu-id="2fa66-378">reportId</span></span>    |    <span data-ttu-id="2fa66-379">Sì</span><span class="sxs-lookup"><span data-stu-id="2fa66-379">Yes</span></span>    |    <span data-ttu-id="2fa66-380">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-380">string</span></span>    |    <span data-ttu-id="2fa66-381">Filtrare per ottenere i dettagli di esecuzione solo dei report con il valore reportId specificato in questo argomento.</span><span class="sxs-lookup"><span data-stu-id="2fa66-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="2fa66-382">È possibile specificare più reportId separandoli con un punto e virgola ";".</span><span class="sxs-lookup"><span data-stu-id="2fa66-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="2fa66-383">Query parameter (Parametro di query)</span><span class="sxs-lookup"><span data-stu-id="2fa66-383">Query parameter</span></span>

|    <span data-ttu-id="2fa66-384">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-384">Parameter Name</span></span>    |    <span data-ttu-id="2fa66-385">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="2fa66-385">Required</span></span>    |    <span data-ttu-id="2fa66-386">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fa66-386">Type</span></span>    |    <span data-ttu-id="2fa66-387">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2fa66-388">executionId</span><span class="sxs-lookup"><span data-stu-id="2fa66-388">executionId</span></span>    |    <span data-ttu-id="2fa66-389">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-389">No</span></span>    |    <span data-ttu-id="2fa66-390">string</span><span class="sxs-lookup"><span data-stu-id="2fa66-390">string</span></span>    |    <span data-ttu-id="2fa66-391">Filtrare per ottenere i dettagli solo dei report con il valore executionId specificato in questo argomento.</span><span class="sxs-lookup"><span data-stu-id="2fa66-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="2fa66-392">È possibile specificare più executionId separandoli con un punto e virgola ";".</span><span class="sxs-lookup"><span data-stu-id="2fa66-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="2fa66-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="2fa66-393">executionStatus</span></span>    |    <span data-ttu-id="2fa66-394">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-394">No</span></span>    |    <span data-ttu-id="2fa66-395">String/enum</span><span class="sxs-lookup"><span data-stu-id="2fa66-395">String/enum</span></span>    |    <span data-ttu-id="2fa66-396">Filtrare per ottenere i dettagli solo dei report con executionStatus specificato in questo argomento.</span><span class="sxs-lookup"><span data-stu-id="2fa66-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="2fa66-397">I valori validi sono: `Pending` `Running` , e `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="2fa66-398">Il valore predefinito è `Completed`.</span><span class="sxs-lookup"><span data-stu-id="2fa66-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="2fa66-399">È possibile specificare più stati separandoli con un punto e virgola ";".</span><span class="sxs-lookup"><span data-stu-id="2fa66-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="2fa66-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="2fa66-400">getLatestExecution</span></span>    |    <span data-ttu-id="2fa66-401">No</span><span class="sxs-lookup"><span data-stu-id="2fa66-401">No</span></span>    |    <span data-ttu-id="2fa66-402">boolean</span><span class="sxs-lookup"><span data-stu-id="2fa66-402">boolean</span></span>    |    <span data-ttu-id="2fa66-403">L'API restituirà i dettagli dell'esecuzione più recente.</span><span class="sxs-lookup"><span data-stu-id="2fa66-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="2fa66-404">Per impostazione predefinita, questo parametro è impostato su true.</span><span class="sxs-lookup"><span data-stu-id="2fa66-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="2fa66-405">Se si sceglie di passare il valore di questo parametro come false, l'API restituirà le istanze di esecuzione degli ultimi 90 giorni.</span><span class="sxs-lookup"><span data-stu-id="2fa66-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="2fa66-406">Payload di richiesta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-406">Sample Request Payload</span></span>

<span data-ttu-id="2fa66-407">Nessuno</span><span class="sxs-lookup"><span data-stu-id="2fa66-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="2fa66-408">Risposta di esempio</span><span class="sxs-lookup"><span data-stu-id="2fa66-408">Sample Response</span></span>

<span data-ttu-id="2fa66-409">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="2fa66-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="2fa66-410">Codici di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2fa66-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2fa66-411">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="2fa66-411">Response payload example:</span></span>

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

<span data-ttu-id="2fa66-412">Al termine dell'esecuzione del report, viene visualizzato lo `Completed` stato di esecuzione.</span><span class="sxs-lookup"><span data-stu-id="2fa66-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="2fa66-413">È possibile scaricare il report selezionando l'URL in `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="2fa66-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="2fa66-414">Glossario</span><span class="sxs-lookup"><span data-stu-id="2fa66-414">Glossary</span></span>

<span data-ttu-id="2fa66-415">Definizioni chiave degli elementi nella risposta.</span><span class="sxs-lookup"><span data-stu-id="2fa66-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="2fa66-416">Parametro</span><span class="sxs-lookup"><span data-stu-id="2fa66-416">Parameter</span></span>    |    <span data-ttu-id="2fa66-417">Descrizione</span><span class="sxs-lookup"><span data-stu-id="2fa66-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2fa66-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="2fa66-418">ExecutionId</span></span>    |    <span data-ttu-id="2fa66-419">Identificatore univoco universale (UUID) dell'istanza di esecuzione</span><span class="sxs-lookup"><span data-stu-id="2fa66-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="2fa66-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="2fa66-420">ReportId</span></span>    |    <span data-ttu-id="2fa66-421">ID report associato all'istanza di esecuzione</span><span class="sxs-lookup"><span data-stu-id="2fa66-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="2fa66-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2fa66-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="2fa66-423">Intervallo di ricorrenza specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="2fa66-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-424">RecurrenceCount</span></span>    |    <span data-ttu-id="2fa66-425">Numero di ricorrenze specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="2fa66-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="2fa66-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="2fa66-426">CallbackUrl</span></span>    |    <span data-ttu-id="2fa66-427">URL di callback associato all'istanza di esecuzione</span><span class="sxs-lookup"><span data-stu-id="2fa66-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="2fa66-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="2fa66-428">CallbackMethod</span></span>    |    <span data-ttu-id="2fa66-429">Metodo di callback associato all'istanza di esecuzione</span><span class="sxs-lookup"><span data-stu-id="2fa66-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="2fa66-430">Formato</span><span class="sxs-lookup"><span data-stu-id="2fa66-430">Format</span></span>    |    <span data-ttu-id="2fa66-431">Formato del file generato alla fine dell'esecuzione</span><span class="sxs-lookup"><span data-stu-id="2fa66-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="2fa66-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="2fa66-432">ExecutionStatus</span></span>    |    <span data-ttu-id="2fa66-433">Stato dell'istanza di esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="2fa66-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="2fa66-434">I valori validi sono: `Pending` `Running` , , `Paused` e `Completed`</span><span class="sxs-lookup"><span data-stu-id="2fa66-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="2fa66-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="2fa66-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="2fa66-436">Collegamento tramite il quale è possibile accedere al report in modo sicuro</span><span class="sxs-lookup"><span data-stu-id="2fa66-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="2fa66-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="2fa66-438">Ora UTC dopo la quale il collegamento al report scadrà nel formato seguente: aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="2fa66-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="2fa66-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="2fa66-440">Ora UTC in cui il report è stato generato nel formato seguente: aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="2fa66-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="2fa66-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2fa66-441">TotalCount</span></span>    |    <span data-ttu-id="2fa66-442">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="2fa66-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="2fa66-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2fa66-443">StatusCode</span></span>    |    <span data-ttu-id="2fa66-444">Codice risultato</span><span class="sxs-lookup"><span data-stu-id="2fa66-444">Result Code</span></span> <br> <span data-ttu-id="2fa66-445">I valori possibili sono 200, 400, 401, 403, 404 e 500</span><span class="sxs-lookup"><span data-stu-id="2fa66-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="2fa66-446">message</span><span class="sxs-lookup"><span data-stu-id="2fa66-446">message</span></span>    |    <span data-ttu-id="2fa66-447">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="2fa66-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="2fa66-448">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="2fa66-448">Next steps</span></span>

- <span data-ttu-id="2fa66-449">Provare le API tramite [l'URL dell'API swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="2fa66-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="2fa66-450">Effettuare la prima chiamata API</span><span class="sxs-lookup"><span data-stu-id="2fa66-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)