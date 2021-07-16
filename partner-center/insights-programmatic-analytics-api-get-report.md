---
title: "Ottenere l'API del report : Insights dati"
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere tutti gli ID report disponibili in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375602"
---
# <a name="get-report-api"></a><span data-ttu-id="17d90-103">Ottenere l'API del report</span><span class="sxs-lookup"><span data-stu-id="17d90-103">Get report API</span></span>

<span data-ttu-id="17d90-104">Questa API ottiene tutti i report pianificati.</span><span class="sxs-lookup"><span data-stu-id="17d90-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="17d90-105">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="17d90-105">**Request syntax**</span></span>

|    <span data-ttu-id="17d90-106">Metodo</span><span class="sxs-lookup"><span data-stu-id="17d90-106">Method</span></span>    |    <span data-ttu-id="17d90-107">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="17d90-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="17d90-108">GET</span><span class="sxs-lookup"><span data-stu-id="17d90-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="17d90-109">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="17d90-109">**Request header**</span></span>

|    <span data-ttu-id="17d90-110">Intestazione</span><span class="sxs-lookup"><span data-stu-id="17d90-110">Header</span></span>    |    <span data-ttu-id="17d90-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d90-111">Type</span></span>    |    <span data-ttu-id="17d90-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="17d90-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="17d90-113">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="17d90-113">Authorization</span></span>    |    <span data-ttu-id="17d90-114">string</span><span class="sxs-lookup"><span data-stu-id="17d90-114">string</span></span>    |    <span data-ttu-id="17d90-115">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="17d90-115">Required.</span></span> <span data-ttu-id="17d90-116">Token Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="17d90-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="17d90-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17d90-117">Content-Type</span></span>    |    <span data-ttu-id="17d90-118">string</span><span class="sxs-lookup"><span data-stu-id="17d90-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="17d90-119">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="17d90-119">**Path parameter**</span></span>

<span data-ttu-id="17d90-120">Nessuno</span><span class="sxs-lookup"><span data-stu-id="17d90-120">None</span></span>

<span data-ttu-id="17d90-121">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="17d90-121">**Query parameter**</span></span>

|    <span data-ttu-id="17d90-122">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="17d90-122">Parameter Name</span></span>    |    <span data-ttu-id="17d90-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d90-123">Type</span></span>    |    <span data-ttu-id="17d90-124">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="17d90-124">Required</span></span>    |    <span data-ttu-id="17d90-125">Descrizione</span><span class="sxs-lookup"><span data-stu-id="17d90-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="17d90-126">reportId</span><span class="sxs-lookup"><span data-stu-id="17d90-126">reportId</span></span>     |    <span data-ttu-id="17d90-127">stringa</span><span class="sxs-lookup"><span data-stu-id="17d90-127">string</span></span>    |    <span data-ttu-id="17d90-128">No</span><span class="sxs-lookup"><span data-stu-id="17d90-128">No</span></span>    |    <span data-ttu-id="17d90-129">Filtrare per ottenere i dettagli solo dei report con il reportId specificato in questo argomento</span><span class="sxs-lookup"><span data-stu-id="17d90-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="17d90-130">reportName</span><span class="sxs-lookup"><span data-stu-id="17d90-130">reportName</span></span>     |    <span data-ttu-id="17d90-131">stringa</span><span class="sxs-lookup"><span data-stu-id="17d90-131">string</span></span>    |    <span data-ttu-id="17d90-132">No</span><span class="sxs-lookup"><span data-stu-id="17d90-132">No</span></span>    |    <span data-ttu-id="17d90-133">Filtrare per ottenere i dettagli solo dei report con reportName specificato in questo argomento</span><span class="sxs-lookup"><span data-stu-id="17d90-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="17d90-134">queryId</span><span class="sxs-lookup"><span data-stu-id="17d90-134">queryId</span></span>     |    <span data-ttu-id="17d90-135">stringa</span><span class="sxs-lookup"><span data-stu-id="17d90-135">string</span></span>    |    <span data-ttu-id="17d90-136">No</span><span class="sxs-lookup"><span data-stu-id="17d90-136">No</span></span>    |    <span data-ttu-id="17d90-137">Filtrare per ottenere i dettagli solo dei report con queryId specificato in questo argomento</span><span class="sxs-lookup"><span data-stu-id="17d90-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="17d90-138">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="17d90-138">**Request payload**</span></span>

<span data-ttu-id="17d90-139">Nessuno</span><span class="sxs-lookup"><span data-stu-id="17d90-139">None</span></span>

<span data-ttu-id="17d90-140">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="17d90-140">**Glossary**</span></span>

<span data-ttu-id="17d90-141">Nessuno</span><span class="sxs-lookup"><span data-stu-id="17d90-141">None</span></span>

<span data-ttu-id="17d90-142">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="17d90-142">**Response**</span></span>

<span data-ttu-id="17d90-143">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="17d90-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="17d90-144">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="17d90-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="17d90-145">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="17d90-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="17d90-146">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="17d90-146">**Glossary**</span></span>

<span data-ttu-id="17d90-147">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="17d90-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="17d90-148">Parametro</span><span class="sxs-lookup"><span data-stu-id="17d90-148">Parameter</span></span>    |    <span data-ttu-id="17d90-149">Descrizione</span><span class="sxs-lookup"><span data-stu-id="17d90-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="17d90-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="17d90-150">ReportId</span></span>     |    <span data-ttu-id="17d90-151">UUID univoco del report creato</span><span class="sxs-lookup"><span data-stu-id="17d90-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="17d90-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="17d90-152">ReportName</span></span>     |    <span data-ttu-id="17d90-153">Nome assegnato al report nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="17d90-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="17d90-154">Descrizione</span><span class="sxs-lookup"><span data-stu-id="17d90-154">Description</span></span>     |    <span data-ttu-id="17d90-155">Descrizione data al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="17d90-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="17d90-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="17d90-156">QueryId</span></span>     |    <span data-ttu-id="17d90-157">ID query passato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="17d90-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="17d90-158">Query</span><span class="sxs-lookup"><span data-stu-id="17d90-158">Query</span></span>     |    <span data-ttu-id="17d90-159">Testo della query che verrà eseguito per questo report</span><span class="sxs-lookup"><span data-stu-id="17d90-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="17d90-160">User</span><span class="sxs-lookup"><span data-stu-id="17d90-160">User</span></span>     |    <span data-ttu-id="17d90-161">ID utente usato per creare il report</span><span class="sxs-lookup"><span data-stu-id="17d90-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="17d90-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="17d90-162">CreatedTime</span></span>     |    <span data-ttu-id="17d90-163">Ora di creazione del report.</span><span class="sxs-lookup"><span data-stu-id="17d90-163">Time the report was created.</span></span> <span data-ttu-id="17d90-164">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="17d90-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="17d90-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="17d90-165">ModifiedTime</span></span>     |    <span data-ttu-id="17d90-166">Ora dell'ultima modifica del report.</span><span class="sxs-lookup"><span data-stu-id="17d90-166">Time the report was last modified.</span></span> <span data-ttu-id="17d90-167">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="17d90-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="17d90-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="17d90-168">executeNow</span></span>     |    <span data-ttu-id="17d90-169">Flag ExecuteNow impostato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="17d90-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="17d90-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="17d90-170">StartTime</span></span>     |    <span data-ttu-id="17d90-171">Ora di inizio dell'esecuzione.</span><span class="sxs-lookup"><span data-stu-id="17d90-171">Time execution will begin.</span></span> <span data-ttu-id="17d90-172">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="17d90-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="17d90-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="17d90-173">ReportStatus</span></span>     |    <span data-ttu-id="17d90-174">Stato dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="17d90-174">Status of the report execution.</span></span> <span data-ttu-id="17d90-175">I valori possibili sono Paused, Active e Inactive.</span><span class="sxs-lookup"><span data-stu-id="17d90-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="17d90-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="17d90-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="17d90-177">Intervallo di ricorrenza specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="17d90-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="17d90-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="17d90-178">RecurrenceCount</span></span>     |    <span data-ttu-id="17d90-179">Numero di ricorrenze specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="17d90-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="17d90-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="17d90-180">CallbackUrl</span></span>     |    <span data-ttu-id="17d90-181">URL di callback specificato nella richiesta</span><span class="sxs-lookup"><span data-stu-id="17d90-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="17d90-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="17d90-182">CallbackMethod</span></span>    |    <span data-ttu-id="17d90-183">Metodo di callback fornito nella richiesta</span><span class="sxs-lookup"><span data-stu-id="17d90-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="17d90-184">Formato</span><span class="sxs-lookup"><span data-stu-id="17d90-184">Format</span></span>     |    <span data-ttu-id="17d90-185">Formato dei file di report</span><span class="sxs-lookup"><span data-stu-id="17d90-185">Format of the report files</span></span>     |
|    <span data-ttu-id="17d90-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="17d90-186">TotalCount</span></span>     |    <span data-ttu-id="17d90-187">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="17d90-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="17d90-188">Message</span><span class="sxs-lookup"><span data-stu-id="17d90-188">Message</span></span>     |    <span data-ttu-id="17d90-189">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="17d90-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="17d90-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="17d90-190">StatusCode</span></span>     |    <span data-ttu-id="17d90-191">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="17d90-191">Result Code.</span></span> <span data-ttu-id="17d90-192">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="17d90-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |