---
title: Sospendere l'API di esecuzione del report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per sospendere l'esecuzione di qualsiasi report in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375601"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="f41b5-103">Sospendi l'API esecuzioni di report</span><span class="sxs-lookup"><span data-stu-id="f41b5-103">Pause report executions API</span></span>

<span data-ttu-id="f41b5-104">In caso di esecuzione, questa API sospende l'esecuzione pianificata dei report.</span><span class="sxs-lookup"><span data-stu-id="f41b5-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="f41b5-105">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="f41b5-105">**Request syntax**</span></span>

|    <span data-ttu-id="f41b5-106">Metodo</span><span class="sxs-lookup"><span data-stu-id="f41b5-106">Method</span></span>    |    <span data-ttu-id="f41b5-107">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="f41b5-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f41b5-108">PUT</span><span class="sxs-lookup"><span data-stu-id="f41b5-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="f41b5-109">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="f41b5-109">**Request header**</span></span>

|    <span data-ttu-id="f41b5-110">Intestazione</span><span class="sxs-lookup"><span data-stu-id="f41b5-110">Header</span></span>    |    <span data-ttu-id="f41b5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f41b5-111">Type</span></span>    |    <span data-ttu-id="f41b5-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f41b5-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="f41b5-113">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="f41b5-113">Authorization</span></span>    |    <span data-ttu-id="f41b5-114">string</span><span class="sxs-lookup"><span data-stu-id="f41b5-114">string</span></span>    |    <span data-ttu-id="f41b5-115">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="f41b5-115">Required.</span></span> <span data-ttu-id="f41b5-116">Token Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="f41b5-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="f41b5-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f41b5-117">Content-Type</span></span>    |    <span data-ttu-id="f41b5-118">string</span><span class="sxs-lookup"><span data-stu-id="f41b5-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="f41b5-119">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="f41b5-119">**Path parameter**</span></span>

|    <span data-ttu-id="f41b5-120">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="f41b5-120">Parameter Name</span></span>    |    <span data-ttu-id="f41b5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f41b5-121">Type</span></span>    |    <span data-ttu-id="f41b5-122">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="f41b5-122">Required</span></span>    |    <span data-ttu-id="f41b5-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f41b5-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="f41b5-124">reportId</span><span class="sxs-lookup"><span data-stu-id="f41b5-124">reportId</span></span>     |    <span data-ttu-id="f41b5-125">stringa</span><span class="sxs-lookup"><span data-stu-id="f41b5-125">string</span></span>    |    <span data-ttu-id="f41b5-126">No</span><span class="sxs-lookup"><span data-stu-id="f41b5-126">No</span></span>    |    <span data-ttu-id="f41b5-127">ID del report da modificare</span><span class="sxs-lookup"><span data-stu-id="f41b5-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="f41b5-128">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="f41b5-128">**Query parameter**</span></span>

<span data-ttu-id="f41b5-129">Nessuno</span><span class="sxs-lookup"><span data-stu-id="f41b5-129">None</span></span>

<span data-ttu-id="f41b5-130">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="f41b5-130">**Request payload**</span></span>

<span data-ttu-id="f41b5-131">Nessuno</span><span class="sxs-lookup"><span data-stu-id="f41b5-131">None</span></span>

<span data-ttu-id="f41b5-132">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="f41b5-132">**Glossary**</span></span>

<span data-ttu-id="f41b5-133">Nessuno</span><span class="sxs-lookup"><span data-stu-id="f41b5-133">None</span></span>

<span data-ttu-id="f41b5-134">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="f41b5-134">**Response**</span></span>

<span data-ttu-id="f41b5-135">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="f41b5-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="f41b5-136">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="f41b5-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="f41b5-137">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="f41b5-137">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="f41b5-138">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="f41b5-138">**Glossary**</span></span>

<span data-ttu-id="f41b5-139">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="f41b5-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="f41b5-140">Parametro</span><span class="sxs-lookup"><span data-stu-id="f41b5-140">Parameter</span></span>    |    <span data-ttu-id="f41b5-141">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f41b5-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="f41b5-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="f41b5-142">ReportId</span></span>     |    <span data-ttu-id="f41b5-143">Identificatore univoco universale (UUID) del report sospeso</span><span class="sxs-lookup"><span data-stu-id="f41b5-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="f41b5-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="f41b5-144">ReportName</span></span>     |    <span data-ttu-id="f41b5-145">Nome assegnato al report durante la creazione</span><span class="sxs-lookup"><span data-stu-id="f41b5-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="f41b5-146">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f41b5-146">Description</span></span>     |    <span data-ttu-id="f41b5-147">Descrizione fornita durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="f41b5-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="f41b5-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="f41b5-148">QueryId</span></span>     |    <span data-ttu-id="f41b5-149">ID query passato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="f41b5-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="f41b5-150">Query</span><span class="sxs-lookup"><span data-stu-id="f41b5-150">Query</span></span>     |    <span data-ttu-id="f41b5-151">Testo della query che verrà eseguito per questo report</span><span class="sxs-lookup"><span data-stu-id="f41b5-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="f41b5-152">User</span><span class="sxs-lookup"><span data-stu-id="f41b5-152">User</span></span>     |    <span data-ttu-id="f41b5-153">ID utente usato per creare il report</span><span class="sxs-lookup"><span data-stu-id="f41b5-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="f41b5-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="f41b5-154">CreatedTime</span></span>     |    <span data-ttu-id="f41b5-155">Ora di creazione del report.</span><span class="sxs-lookup"><span data-stu-id="f41b5-155">Time the report was created.</span></span> <span data-ttu-id="f41b5-156">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f41b5-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f41b5-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="f41b5-157">ModifiedTime</span></span>     |    <span data-ttu-id="f41b5-158">Ora dell'ultima modifica del report.</span><span class="sxs-lookup"><span data-stu-id="f41b5-158">Time the report was last modified.</span></span> <span data-ttu-id="f41b5-159">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f41b5-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f41b5-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="f41b5-160">ExecuteNow</span></span>     |    <span data-ttu-id="f41b5-161">Flag ExecuteNow impostato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="f41b5-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="f41b5-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="f41b5-162">StartTime</span></span>     |    <span data-ttu-id="f41b5-163">Ora di inizio dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="f41b5-163">Time the report execution will begin.</span></span> <span data-ttu-id="f41b5-164">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="f41b5-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="f41b5-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="f41b5-165">ReportStatus</span></span>     |    <span data-ttu-id="f41b5-166">Stato dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="f41b5-166">Status of the report execution.</span></span> <span data-ttu-id="f41b5-167">I valori possibili sono Paused, Active e Inactive.</span><span class="sxs-lookup"><span data-stu-id="f41b5-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="f41b5-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="f41b5-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="f41b5-169">Intervallo di ricorrenza specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="f41b5-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="f41b5-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="f41b5-170">RecurrenceCount</span></span>     |    <span data-ttu-id="f41b5-171">Numero di ricorrenze specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="f41b5-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="f41b5-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="f41b5-172">CallbackUrl</span></span>     |    <span data-ttu-id="f41b5-173">URL di callback specificato nella richiesta</span><span class="sxs-lookup"><span data-stu-id="f41b5-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="f41b5-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="f41b5-174">CallbackMethod</span></span>    |    <span data-ttu-id="f41b5-175">Metodo di callback fornito nella richiesta</span><span class="sxs-lookup"><span data-stu-id="f41b5-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="f41b5-176">Formato</span><span class="sxs-lookup"><span data-stu-id="f41b5-176">Format</span></span>     |    <span data-ttu-id="f41b5-177">Formato dei file di report</span><span class="sxs-lookup"><span data-stu-id="f41b5-177">Format of the report files</span></span>     |
|    <span data-ttu-id="f41b5-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="f41b5-178">TotalCount</span></span>     |    <span data-ttu-id="f41b5-179">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="f41b5-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="f41b5-180">Message</span><span class="sxs-lookup"><span data-stu-id="f41b5-180">Message</span></span>     |    <span data-ttu-id="f41b5-181">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="f41b5-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="f41b5-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="f41b5-182">StatusCode</span></span>     |    <span data-ttu-id="f41b5-183">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="f41b5-183">Result Code.</span></span> <span data-ttu-id="f41b5-184">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="f41b5-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
