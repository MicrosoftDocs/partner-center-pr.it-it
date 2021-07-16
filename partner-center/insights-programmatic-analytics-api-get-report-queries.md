---
title: Ottenere l'API query di report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere tutte le query disponibili da usare nell'API del report.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375607"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="b0c78-103">API Per ottenere query di report</span><span class="sxs-lookup"><span data-stu-id="b0c78-103">Get report queries API</span></span>

<span data-ttu-id="b0c78-104">L'API Recupera query report ottiene tutte le query disponibili per l'uso nei report.</span><span class="sxs-lookup"><span data-stu-id="b0c78-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="b0c78-105">Ottiene tutte le query di sistema e definite dall'utente per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="b0c78-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="b0c78-106">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="b0c78-106">**Request syntax**</span></span>

|    <span data-ttu-id="b0c78-107">Metodo</span><span class="sxs-lookup"><span data-stu-id="b0c78-107">Method</span></span>    |    <span data-ttu-id="b0c78-108">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="b0c78-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b0c78-109">GET</span><span class="sxs-lookup"><span data-stu-id="b0c78-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="b0c78-110">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="b0c78-110">**Request header**</span></span>

|    <span data-ttu-id="b0c78-111">Intestazione</span><span class="sxs-lookup"><span data-stu-id="b0c78-111">Header</span></span>    |    <span data-ttu-id="b0c78-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c78-112">Type</span></span>    |    <span data-ttu-id="b0c78-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b0c78-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b0c78-114">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="b0c78-114">Authorization</span></span>    |    <span data-ttu-id="b0c78-115">string</span><span class="sxs-lookup"><span data-stu-id="b0c78-115">string</span></span>    |    <span data-ttu-id="b0c78-116">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="b0c78-116">Required.</span></span> <span data-ttu-id="b0c78-117">Token Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b0c78-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b0c78-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0c78-118">Content-Type</span></span>    |    <span data-ttu-id="b0c78-119">string</span><span class="sxs-lookup"><span data-stu-id="b0c78-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b0c78-120">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="b0c78-120">**Path parameter**</span></span>

<span data-ttu-id="b0c78-121">Nessuno</span><span class="sxs-lookup"><span data-stu-id="b0c78-121">None</span></span>

<span data-ttu-id="b0c78-122">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="b0c78-122">**Query parameter**</span></span>

|    <span data-ttu-id="b0c78-123">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="b0c78-123">Parameter Name</span></span>    |    <span data-ttu-id="b0c78-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c78-124">Type</span></span>    |    <span data-ttu-id="b0c78-125">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="b0c78-125">Required</span></span>    |    <span data-ttu-id="b0c78-126">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b0c78-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b0c78-127">queryId</span><span class="sxs-lookup"><span data-stu-id="b0c78-127">queryId</span></span>     |    <span data-ttu-id="b0c78-128">stringa</span><span class="sxs-lookup"><span data-stu-id="b0c78-128">string</span></span>     |    <span data-ttu-id="b0c78-129">No</span><span class="sxs-lookup"><span data-stu-id="b0c78-129">No</span></span>    |    <span data-ttu-id="b0c78-130">Filtrare per ottenere i dettagli solo delle query con l'ID specificato nell'argomento</span><span class="sxs-lookup"><span data-stu-id="b0c78-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="b0c78-131">queryName</span><span class="sxs-lookup"><span data-stu-id="b0c78-131">queryName</span></span>     |    <span data-ttu-id="b0c78-132">stringa</span><span class="sxs-lookup"><span data-stu-id="b0c78-132">string</span></span>     |    <span data-ttu-id="b0c78-133">No</span><span class="sxs-lookup"><span data-stu-id="b0c78-133">No</span></span>    |    <span data-ttu-id="b0c78-134">Filtrare per ottenere i dettagli solo delle query con il nome specificato nell'argomento</span><span class="sxs-lookup"><span data-stu-id="b0c78-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="b0c78-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="b0c78-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="b0c78-136">boolean</span><span class="sxs-lookup"><span data-stu-id="b0c78-136">boolean</span></span>     |    <span data-ttu-id="b0c78-137">No</span><span class="sxs-lookup"><span data-stu-id="b0c78-137">No</span></span>    |    <span data-ttu-id="b0c78-138">Includere query di sistema predefinite nella risposta</span><span class="sxs-lookup"><span data-stu-id="b0c78-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="b0c78-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="b0c78-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="b0c78-140">boolean</span><span class="sxs-lookup"><span data-stu-id="b0c78-140">boolean</span></span>     |    <span data-ttu-id="b0c78-141">No</span><span class="sxs-lookup"><span data-stu-id="b0c78-141">No</span></span>    |    <span data-ttu-id="b0c78-142">Includere solo query di sistema nella risposta</span><span class="sxs-lookup"><span data-stu-id="b0c78-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="b0c78-143">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="b0c78-143">**Request payload**</span></span>

<span data-ttu-id="b0c78-144">Nessuno</span><span class="sxs-lookup"><span data-stu-id="b0c78-144">None</span></span>

<span data-ttu-id="b0c78-145">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="b0c78-145">**Glossary**</span></span>

<span data-ttu-id="b0c78-146">Nessuno</span><span class="sxs-lookup"><span data-stu-id="b0c78-146">None</span></span>

<span data-ttu-id="b0c78-147">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="b0c78-147">**Response**</span></span>

<span data-ttu-id="b0c78-148">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="b0c78-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="b0c78-149">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b0c78-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b0c78-150">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="b0c78-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="b0c78-151">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="b0c78-151">**Glossary**</span></span>

<span data-ttu-id="b0c78-152">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="b0c78-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b0c78-153">Parametro</span><span class="sxs-lookup"><span data-stu-id="b0c78-153">Parameter</span></span>    |    <span data-ttu-id="b0c78-154">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b0c78-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b0c78-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="b0c78-155">QueryId</span></span>     |    <span data-ttu-id="b0c78-156">UUID univoco della query</span><span class="sxs-lookup"><span data-stu-id="b0c78-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="b0c78-157">Name</span><span class="sxs-lookup"><span data-stu-id="b0c78-157">Name</span></span>     |    <span data-ttu-id="b0c78-158">Nome assegnato alla query al momento della creazione della query</span><span class="sxs-lookup"><span data-stu-id="b0c78-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="b0c78-159">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b0c78-159">Description</span></span>     |    <span data-ttu-id="b0c78-160">Descrizione specificata durante la creazione della query</span><span class="sxs-lookup"><span data-stu-id="b0c78-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="b0c78-161">Query</span><span class="sxs-lookup"><span data-stu-id="b0c78-161">Query</span></span>     |    <span data-ttu-id="b0c78-162">Stringa di query del report</span><span class="sxs-lookup"><span data-stu-id="b0c78-162">Report query string</span></span>     |
|    <span data-ttu-id="b0c78-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c78-163">Type</span></span>     |    <span data-ttu-id="b0c78-164">Impostare su userDefined per le query create dall'utente e il sistema per le query di sistema predefinite</span><span class="sxs-lookup"><span data-stu-id="b0c78-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="b0c78-165">User</span><span class="sxs-lookup"><span data-stu-id="b0c78-165">User</span></span>     |    <span data-ttu-id="b0c78-166">ID utente che ha creato la query</span><span class="sxs-lookup"><span data-stu-id="b0c78-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="b0c78-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="b0c78-167">CreatedTime</span></span>     |    <span data-ttu-id="b0c78-168">Ora di creazione della query</span><span class="sxs-lookup"><span data-stu-id="b0c78-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="b0c78-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b0c78-169">TotalCount</span></span>     |    <span data-ttu-id="b0c78-170">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="b0c78-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b0c78-171">Message</span><span class="sxs-lookup"><span data-stu-id="b0c78-171">Message</span></span>     |    <span data-ttu-id="b0c78-172">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="b0c78-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b0c78-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="b0c78-173">StatusCode</span></span>     |    <span data-ttu-id="b0c78-174">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="b0c78-174">Result Code.</span></span> <span data-ttu-id="b0c78-175">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="b0c78-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
