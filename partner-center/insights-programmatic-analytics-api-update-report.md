---
title: Aggiornare l'API del report
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per aggiornare i parametri del report in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375578"
---
# <a name="update-report-api"></a><span data-ttu-id="fcbda-103">Aggiornare l'API del report</span><span class="sxs-lookup"><span data-stu-id="fcbda-103">Update report API</span></span>

<span data-ttu-id="fcbda-104">Questa API consente di modificare un parametro del report.</span><span class="sxs-lookup"><span data-stu-id="fcbda-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="fcbda-105">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="fcbda-105">**Request syntax**</span></span>

|    <span data-ttu-id="fcbda-106">Metodo</span><span class="sxs-lookup"><span data-stu-id="fcbda-106">Method</span></span>    |    <span data-ttu-id="fcbda-107">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="fcbda-108">PUT</span><span class="sxs-lookup"><span data-stu-id="fcbda-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="fcbda-109">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="fcbda-109">**Request header**</span></span>

|    <span data-ttu-id="fcbda-110">Intestazione</span><span class="sxs-lookup"><span data-stu-id="fcbda-110">Header</span></span>    |    <span data-ttu-id="fcbda-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcbda-111">Type</span></span>    |    <span data-ttu-id="fcbda-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="fcbda-113">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="fcbda-113">Authorization</span></span>    |    <span data-ttu-id="fcbda-114">string</span><span class="sxs-lookup"><span data-stu-id="fcbda-114">string</span></span>    |    <span data-ttu-id="fcbda-115">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="fcbda-115">Required.</span></span> <span data-ttu-id="fcbda-116">Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="fcbda-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="fcbda-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcbda-117">Content-Type</span></span>    |    <span data-ttu-id="fcbda-118">string</span><span class="sxs-lookup"><span data-stu-id="fcbda-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="fcbda-119">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="fcbda-119">**Path parameter**</span></span>

|    <span data-ttu-id="fcbda-120">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="fcbda-120">Parameter Name</span></span>    |    <span data-ttu-id="fcbda-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcbda-121">Type</span></span>    |    <span data-ttu-id="fcbda-122">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="fcbda-122">Required</span></span>    |    <span data-ttu-id="fcbda-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="fcbda-124">reportId</span><span class="sxs-lookup"><span data-stu-id="fcbda-124">reportId</span></span>     |    <span data-ttu-id="fcbda-125">stringa</span><span class="sxs-lookup"><span data-stu-id="fcbda-125">string</span></span>    |    <span data-ttu-id="fcbda-126">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-126">No</span></span>    |    <span data-ttu-id="fcbda-127">ID del report da modificare</span><span class="sxs-lookup"><span data-stu-id="fcbda-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="fcbda-128">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="fcbda-128">**Query parameter**</span></span>

<span data-ttu-id="fcbda-129">Nessuno</span><span class="sxs-lookup"><span data-stu-id="fcbda-129">None</span></span>

<span data-ttu-id="fcbda-130">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="fcbda-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="fcbda-131">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="fcbda-131">**Glossary**</span></span>

<span data-ttu-id="fcbda-132">Questa tabella elenca le definizioni chiave degli elementi nella risposta.</span><span class="sxs-lookup"><span data-stu-id="fcbda-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="fcbda-133">Parametro</span><span class="sxs-lookup"><span data-stu-id="fcbda-133">Parameter</span></span>    |    <span data-ttu-id="fcbda-134">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="fcbda-134">Required</span></span>    |    <span data-ttu-id="fcbda-135">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-135">Description</span></span>    |    <span data-ttu-id="fcbda-136">Valori consentiti</span><span class="sxs-lookup"><span data-stu-id="fcbda-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="fcbda-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="fcbda-137">ReportName</span></span>     |    <span data-ttu-id="fcbda-138">Sì</span><span class="sxs-lookup"><span data-stu-id="fcbda-138">Yes</span></span>     |    <span data-ttu-id="fcbda-139">Nome da assegnare al report</span><span class="sxs-lookup"><span data-stu-id="fcbda-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="fcbda-140">Stringa</span><span class="sxs-lookup"><span data-stu-id="fcbda-140">String</span></span>     |
|    <span data-ttu-id="fcbda-141">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-141">Description</span></span>     |    <span data-ttu-id="fcbda-142">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-142">No</span></span>     |    <span data-ttu-id="fcbda-143">Descrizione del report creato</span><span class="sxs-lookup"><span data-stu-id="fcbda-143">Description of the created report</span></span>     |    <span data-ttu-id="fcbda-144">Stringa</span><span class="sxs-lookup"><span data-stu-id="fcbda-144">String</span></span>     |
|    <span data-ttu-id="fcbda-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="fcbda-145">StartTime</span></span>     |    <span data-ttu-id="fcbda-146">Sì</span><span class="sxs-lookup"><span data-stu-id="fcbda-146">Yes</span></span>    |    <span data-ttu-id="fcbda-147">Timestamp dopo il quale inizierà la generazione del report</span><span class="sxs-lookup"><span data-stu-id="fcbda-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="fcbda-148">Stringa</span><span class="sxs-lookup"><span data-stu-id="fcbda-148">String</span></span>     |
|    <span data-ttu-id="fcbda-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="fcbda-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="fcbda-150">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-150">No</span></span>     |    <span data-ttu-id="fcbda-151">Frequenza con cui il report deve essere generato in ore.</span><span class="sxs-lookup"><span data-stu-id="fcbda-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="fcbda-152">Il valore minimo è 4</span><span class="sxs-lookup"><span data-stu-id="fcbda-152">Minimum value is 4</span></span>     |    <span data-ttu-id="fcbda-153">Intero</span><span class="sxs-lookup"><span data-stu-id="fcbda-153">Integer</span></span>     |
|    <span data-ttu-id="fcbda-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="fcbda-154">RecurrenceCount</span></span>     |    <span data-ttu-id="fcbda-155">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-155">No</span></span>     |    <span data-ttu-id="fcbda-156">Numero di report da generare.</span><span class="sxs-lookup"><span data-stu-id="fcbda-156">Numbers of report to be generated.</span></span> <span data-ttu-id="fcbda-157">Il valore predefinito è indefinito.</span><span class="sxs-lookup"><span data-stu-id="fcbda-157">Default is indefinite.</span></span>     |    <span data-ttu-id="fcbda-158">Intero</span><span class="sxs-lookup"><span data-stu-id="fcbda-158">Integer</span></span>     |
|    <span data-ttu-id="fcbda-159">Formato</span><span class="sxs-lookup"><span data-stu-id="fcbda-159">Format</span></span>     |    <span data-ttu-id="fcbda-160">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-160">No</span></span>    |    <span data-ttu-id="fcbda-161">Formato di file del file esportato.</span><span class="sxs-lookup"><span data-stu-id="fcbda-161">File format of the exported file.</span></span> <span data-ttu-id="fcbda-162">Il valore predefinito è CSV</span><span class="sxs-lookup"><span data-stu-id="fcbda-162">Default is CSV</span></span>     |    <span data-ttu-id="fcbda-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="fcbda-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="fcbda-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="fcbda-164">CallbackURL</span></span>     |    <span data-ttu-id="fcbda-165">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-165">No</span></span>     |    <span data-ttu-id="fcbda-166">URL di callback HTTPS da chiamare per la generazione di report</span><span class="sxs-lookup"><span data-stu-id="fcbda-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="fcbda-167">Stringa</span><span class="sxs-lookup"><span data-stu-id="fcbda-167">String</span></span>     |
|    <span data-ttu-id="fcbda-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="fcbda-168">CallbackMethod</span></span>    |    <span data-ttu-id="fcbda-169">No</span><span class="sxs-lookup"><span data-stu-id="fcbda-169">No</span></span>    |    <span data-ttu-id="fcbda-170">Metodo HTTP da usare per il callback</span><span class="sxs-lookup"><span data-stu-id="fcbda-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="fcbda-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="fcbda-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="fcbda-172">**Response**.</span><span class="sxs-lookup"><span data-stu-id="fcbda-172">**Response**</span></span>

<span data-ttu-id="fcbda-173">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="fcbda-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="fcbda-174">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="fcbda-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="fcbda-175">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="fcbda-175">Response payload example:</span></span>

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

<span data-ttu-id="fcbda-176">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="fcbda-176">**Glossary**</span></span>

<span data-ttu-id="fcbda-177">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="fcbda-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="fcbda-178">Parametro</span><span class="sxs-lookup"><span data-stu-id="fcbda-178">Parameter</span></span>    |    <span data-ttu-id="fcbda-179">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="fcbda-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="fcbda-180">ReportId</span></span>     |    <span data-ttu-id="fcbda-181">Identificatore univoco universale (UUID) del report da aggiornare</span><span class="sxs-lookup"><span data-stu-id="fcbda-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="fcbda-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="fcbda-182">ReportName</span></span>     |    <span data-ttu-id="fcbda-183">Nome assegnato al report nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="fcbda-184">Descrizione</span><span class="sxs-lookup"><span data-stu-id="fcbda-184">Description</span></span>     |    <span data-ttu-id="fcbda-185">Descrizione fornita al report nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="fcbda-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="fcbda-186">QueryId</span></span>     |    <span data-ttu-id="fcbda-187">ID query passato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="fcbda-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="fcbda-188">Query</span><span class="sxs-lookup"><span data-stu-id="fcbda-188">Query</span></span>     |    <span data-ttu-id="fcbda-189">Testo della query che verrà eseguito per questo report</span><span class="sxs-lookup"><span data-stu-id="fcbda-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="fcbda-190">User</span><span class="sxs-lookup"><span data-stu-id="fcbda-190">User</span></span>     |    <span data-ttu-id="fcbda-191">ID utente usato per creare il report</span><span class="sxs-lookup"><span data-stu-id="fcbda-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="fcbda-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="fcbda-192">CreatedTime</span></span>     |    <span data-ttu-id="fcbda-193">Ora di creazione del report.</span><span class="sxs-lookup"><span data-stu-id="fcbda-193">Time the report was created.</span></span> <span data-ttu-id="fcbda-194">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="fcbda-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="fcbda-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="fcbda-195">ModifiedTime</span></span>     |    <span data-ttu-id="fcbda-196">Ora dell'ultima modifica del report.</span><span class="sxs-lookup"><span data-stu-id="fcbda-196">Time the report was last modified.</span></span> <span data-ttu-id="fcbda-197">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="fcbda-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="fcbda-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="fcbda-198">ExecuteNow</span></span>     |    <span data-ttu-id="fcbda-199">Flag ExecuteNow impostato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="fcbda-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="fcbda-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="fcbda-200">StartTime</span></span>     |    <span data-ttu-id="fcbda-201">Ora di inizio dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="fcbda-201">Time the report execution will begin.</span></span> <span data-ttu-id="fcbda-202">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="fcbda-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="fcbda-203">Stato report</span><span class="sxs-lookup"><span data-stu-id="fcbda-203">ReportStatus</span></span>     |    <span data-ttu-id="fcbda-204">Stato dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="fcbda-204">Status of the report execution.</span></span> <span data-ttu-id="fcbda-205">I valori possibili sono Paused, Active e Inactive.</span><span class="sxs-lookup"><span data-stu-id="fcbda-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="fcbda-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="fcbda-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="fcbda-207">Intervallo di ricorrenza specificato nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="fcbda-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="fcbda-208">RecurrenceCount</span></span>     |    <span data-ttu-id="fcbda-209">Numero di ricorrenze specificato nel payload della richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="fcbda-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="fcbda-210">CallbackUrl</span></span>     |    <span data-ttu-id="fcbda-211">URL di callback specificato nella richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="fcbda-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="fcbda-212">CallbackMethod</span></span>    |    <span data-ttu-id="fcbda-213">Metodo di callback fornito nella richiesta</span><span class="sxs-lookup"><span data-stu-id="fcbda-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="fcbda-214">Formato</span><span class="sxs-lookup"><span data-stu-id="fcbda-214">Format</span></span>     |    <span data-ttu-id="fcbda-215">Formato dei file di report</span><span class="sxs-lookup"><span data-stu-id="fcbda-215">Format of the report files</span></span>     |
|    <span data-ttu-id="fcbda-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="fcbda-216">TotalCount</span></span>     |    <span data-ttu-id="fcbda-217">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="fcbda-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="fcbda-218">Message</span><span class="sxs-lookup"><span data-stu-id="fcbda-218">Message</span></span>     |    <span data-ttu-id="fcbda-219">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="fcbda-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="fcbda-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="fcbda-220">StatusCode</span></span>     |    <span data-ttu-id="fcbda-221">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="fcbda-221">Result Code.</span></span> <span data-ttu-id="fcbda-222">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="fcbda-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |