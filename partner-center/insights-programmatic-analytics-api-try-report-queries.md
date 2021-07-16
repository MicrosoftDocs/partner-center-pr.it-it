---
title: Provare l'API delle query di report
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per testare la query e convalidare i risultati in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375583"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="cefef-103">Provare l'API delle query di report</span><span class="sxs-lookup"><span data-stu-id="cefef-103">Try report queries API</span></span>

<span data-ttu-id="cefef-104">Questa API esegue un'istruzione di query Report.</span><span class="sxs-lookup"><span data-stu-id="cefef-104">This API executes a Report query statement.</span></span> <span data-ttu-id="cefef-105">L'API restituisce solo 100 record che il partner può usare per verificare se i dati sono come previsto.</span><span class="sxs-lookup"><span data-stu-id="cefef-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cefef-106">Questa API ha un timeout di esecuzione delle query di 100 secondi.</span><span class="sxs-lookup"><span data-stu-id="cefef-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="cefef-107">Se si nota che l'API sta prendendo più di 100 secondi, è molto probabile che la query sia sintatticamente corretta, altrimenti si riceverebbe un codice di errore diverso da 200.</span><span class="sxs-lookup"><span data-stu-id="cefef-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="cefef-108">La generazione di report effettiva verrà superata se la sintassi della query è corretta.</span><span class="sxs-lookup"><span data-stu-id="cefef-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="cefef-109">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="cefef-109">**Request syntax**</span></span>

|    <span data-ttu-id="cefef-110">Metodo</span><span class="sxs-lookup"><span data-stu-id="cefef-110">Method</span></span>    |    <span data-ttu-id="cefef-111">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="cefef-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cefef-112">GET</span><span class="sxs-lookup"><span data-stu-id="cefef-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="cefef-113">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="cefef-113">**Request header**</span></span>

|    <span data-ttu-id="cefef-114">Intestazione</span><span class="sxs-lookup"><span data-stu-id="cefef-114">Header</span></span>    |    <span data-ttu-id="cefef-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefef-115">Type</span></span>    |    <span data-ttu-id="cefef-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="cefef-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="cefef-117">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="cefef-117">Authorization</span></span>    |    <span data-ttu-id="cefef-118">string</span><span class="sxs-lookup"><span data-stu-id="cefef-118">string</span></span>    |    <span data-ttu-id="cefef-119">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="cefef-119">Required.</span></span> <span data-ttu-id="cefef-120">Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="cefef-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="cefef-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cefef-121">Content-Type</span></span>    |    <span data-ttu-id="cefef-122">string</span><span class="sxs-lookup"><span data-stu-id="cefef-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="cefef-123">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="cefef-123">**Path parameter**</span></span>

<span data-ttu-id="cefef-124">Nessuno</span><span class="sxs-lookup"><span data-stu-id="cefef-124">None</span></span>

<span data-ttu-id="cefef-125">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="cefef-125">**Query parameter**</span></span>

|    <span data-ttu-id="cefef-126">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="cefef-126">Parameter Name</span></span>    |    <span data-ttu-id="cefef-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefef-127">Type</span></span>    |    <span data-ttu-id="cefef-128">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="cefef-128">Required</span></span>    |    <span data-ttu-id="cefef-129">Descrizione</span><span class="sxs-lookup"><span data-stu-id="cefef-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="cefef-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="cefef-130">exportQuery</span></span>     |    <span data-ttu-id="cefef-131">stringa</span><span class="sxs-lookup"><span data-stu-id="cefef-131">string</span></span>    |    <span data-ttu-id="cefef-132">No</span><span class="sxs-lookup"><span data-stu-id="cefef-132">No</span></span>    |    <span data-ttu-id="cefef-133">Stringa di query del report che deve essere eseguita</span><span class="sxs-lookup"><span data-stu-id="cefef-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="cefef-134">queryId</span><span class="sxs-lookup"><span data-stu-id="cefef-134">queryId</span></span>     |    <span data-ttu-id="cefef-135">stringa</span><span class="sxs-lookup"><span data-stu-id="cefef-135">string</span></span>    |    <span data-ttu-id="cefef-136">No</span><span class="sxs-lookup"><span data-stu-id="cefef-136">No</span></span>    |    <span data-ttu-id="cefef-137">ID di query esistente valido.</span><span class="sxs-lookup"><span data-stu-id="cefef-137">A valid existing query ID.</span></span> <span data-ttu-id="cefef-138">Si escludono a vicenda con la stringa di query specificata nel parametro exportQuery</span><span class="sxs-lookup"><span data-stu-id="cefef-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="cefef-139">startTime</span><span class="sxs-lookup"><span data-stu-id="cefef-139">startTime</span></span>     |    <span data-ttu-id="cefef-140">stringa</span><span class="sxs-lookup"><span data-stu-id="cefef-140">string</span></span>    |    <span data-ttu-id="cefef-141">No</span><span class="sxs-lookup"><span data-stu-id="cefef-141">No</span></span>    |    <span data-ttu-id="cefef-142">Ora di inizio da cui si vogliono i dati.</span><span class="sxs-lookup"><span data-stu-id="cefef-142">Start time from which we want the data.</span></span> <span data-ttu-id="cefef-143">Esegue l'override dell'intervallo di tempo specificato nella query</span><span class="sxs-lookup"><span data-stu-id="cefef-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="cefef-144">endTime</span><span class="sxs-lookup"><span data-stu-id="cefef-144">endTime</span></span>     |    <span data-ttu-id="cefef-145">stringa</span><span class="sxs-lookup"><span data-stu-id="cefef-145">string</span></span>    |    <span data-ttu-id="cefef-146">No</span><span class="sxs-lookup"><span data-stu-id="cefef-146">No</span></span>    |    <span data-ttu-id="cefef-147">Ora di fine fino alla quale si vogliono i dati.</span><span class="sxs-lookup"><span data-stu-id="cefef-147">End time till which we want the data.</span></span> <span data-ttu-id="cefef-148">Esegue l'override dell'intervallo di tempo specificato nella query</span><span class="sxs-lookup"><span data-stu-id="cefef-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="cefef-149">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="cefef-149">**Request payload**</span></span>

<span data-ttu-id="cefef-150">Nessuno</span><span class="sxs-lookup"><span data-stu-id="cefef-150">None</span></span>

<span data-ttu-id="cefef-151">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="cefef-151">**Glossary**</span></span>

<span data-ttu-id="cefef-152">Nessuno</span><span class="sxs-lookup"><span data-stu-id="cefef-152">None</span></span>

<span data-ttu-id="cefef-153">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="cefef-153">**Response**</span></span>

<span data-ttu-id="cefef-154">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="cefef-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="cefef-155">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="cefef-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="cefef-156">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="cefef-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="cefef-157">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="cefef-157">**Glossary**</span></span>

<span data-ttu-id="cefef-158">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="cefef-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="cefef-159">Parametro</span><span class="sxs-lookup"><span data-stu-id="cefef-159">Parameter</span></span>    |    <span data-ttu-id="cefef-160">Descrizione</span><span class="sxs-lookup"><span data-stu-id="cefef-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cefef-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="cefef-161">TotalCount</span></span>     |    <span data-ttu-id="cefef-162">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="cefef-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="cefef-163">Message</span><span class="sxs-lookup"><span data-stu-id="cefef-163">Message</span></span>     |    <span data-ttu-id="cefef-164">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="cefef-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="cefef-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="cefef-165">StatusCode</span></span>     |    <span data-ttu-id="cefef-166">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="cefef-166">Result Code.</span></span> <span data-ttu-id="cefef-167">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="cefef-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
