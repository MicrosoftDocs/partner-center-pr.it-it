---
title: Eliminare l'API del report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per eliminare qualsiasi report in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375614"
---
# <a name="delete-report-api"></a><span data-ttu-id="5eafa-103">ELIMINARE L'API del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-103">Delete report API</span></span>

<span data-ttu-id="5eafa-104">Durante l'esecuzione, questa API elimina tutti i record di esecuzione del report e del report.</span><span class="sxs-lookup"><span data-stu-id="5eafa-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="5eafa-105">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="5eafa-105">**Request syntax**</span></span>

|    <span data-ttu-id="5eafa-106">Metodo</span><span class="sxs-lookup"><span data-stu-id="5eafa-106">Method</span></span>    |    <span data-ttu-id="5eafa-107">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="5eafa-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5eafa-108">DOLETE</span><span class="sxs-lookup"><span data-stu-id="5eafa-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="5eafa-109">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="5eafa-109">**Request header**</span></span>

|    <span data-ttu-id="5eafa-110">Intestazione</span><span class="sxs-lookup"><span data-stu-id="5eafa-110">Header</span></span>    |    <span data-ttu-id="5eafa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5eafa-111">Type</span></span>    |    <span data-ttu-id="5eafa-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5eafa-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="5eafa-113">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="5eafa-113">Authorization</span></span>    |    <span data-ttu-id="5eafa-114">string</span><span class="sxs-lookup"><span data-stu-id="5eafa-114">string</span></span>    |    <span data-ttu-id="5eafa-115">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="5eafa-115">Required.</span></span> <span data-ttu-id="5eafa-116">Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="5eafa-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="5eafa-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5eafa-117">Content-Type</span></span>    |    <span data-ttu-id="5eafa-118">string</span><span class="sxs-lookup"><span data-stu-id="5eafa-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="5eafa-119">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="5eafa-119">**Path parameter**</span></span>

|    <span data-ttu-id="5eafa-120">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="5eafa-120">Parameter Name</span></span>    |    <span data-ttu-id="5eafa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5eafa-121">Type</span></span>    |    <span data-ttu-id="5eafa-122">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="5eafa-122">Required</span></span>    |    <span data-ttu-id="5eafa-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5eafa-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="5eafa-124">reportId</span><span class="sxs-lookup"><span data-stu-id="5eafa-124">reportId</span></span>     |    <span data-ttu-id="5eafa-125">stringa</span><span class="sxs-lookup"><span data-stu-id="5eafa-125">string</span></span>    |    <span data-ttu-id="5eafa-126">No</span><span class="sxs-lookup"><span data-stu-id="5eafa-126">No</span></span>    |    <span data-ttu-id="5eafa-127">ID del report da eliminare</span><span class="sxs-lookup"><span data-stu-id="5eafa-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="5eafa-128">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="5eafa-128">**Query parameter**</span></span>

<span data-ttu-id="5eafa-129">Nessuno</span><span class="sxs-lookup"><span data-stu-id="5eafa-129">None</span></span>

<span data-ttu-id="5eafa-130">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="5eafa-130">**Request payload**</span></span>

<span data-ttu-id="5eafa-131">Nessuno</span><span class="sxs-lookup"><span data-stu-id="5eafa-131">None</span></span>

<span data-ttu-id="5eafa-132">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="5eafa-132">**Glossary**</span></span>

<span data-ttu-id="5eafa-133">Nessuno</span><span class="sxs-lookup"><span data-stu-id="5eafa-133">None</span></span>

<span data-ttu-id="5eafa-134">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="5eafa-134">**Response**</span></span>

<span data-ttu-id="5eafa-135">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="5eafa-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="5eafa-136">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="5eafa-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="5eafa-137">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="5eafa-137">Response payload example:</span></span>

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

<span data-ttu-id="5eafa-138">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="5eafa-138">**Glossary**</span></span>

<span data-ttu-id="5eafa-139">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="5eafa-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="5eafa-140">Parametro</span><span class="sxs-lookup"><span data-stu-id="5eafa-140">Parameter</span></span>    |    <span data-ttu-id="5eafa-141">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5eafa-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5eafa-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="5eafa-142">ReportId</span></span>     |    <span data-ttu-id="5eafa-143">Identificatore univoco universale (UUID) del report eliminato</span><span class="sxs-lookup"><span data-stu-id="5eafa-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="5eafa-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="5eafa-144">ReportName</span></span>     |    <span data-ttu-id="5eafa-145">Nome assegnato al report durante la creazione</span><span class="sxs-lookup"><span data-stu-id="5eafa-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="5eafa-146">Descrizione</span><span class="sxs-lookup"><span data-stu-id="5eafa-146">Description</span></span>     |    <span data-ttu-id="5eafa-147">Descrizione specificata durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="5eafa-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="5eafa-148">QueryId</span></span>     |    <span data-ttu-id="5eafa-149">ID query passato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="5eafa-150">Query</span><span class="sxs-lookup"><span data-stu-id="5eafa-150">Query</span></span>     |    <span data-ttu-id="5eafa-151">Testo della query che verrà eseguito per questo report</span><span class="sxs-lookup"><span data-stu-id="5eafa-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="5eafa-152">User</span><span class="sxs-lookup"><span data-stu-id="5eafa-152">User</span></span>     |    <span data-ttu-id="5eafa-153">ID utente usato per creare il report</span><span class="sxs-lookup"><span data-stu-id="5eafa-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="5eafa-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="5eafa-154">CreatedTime</span></span>     |    <span data-ttu-id="5eafa-155">Ora di creazione del report.</span><span class="sxs-lookup"><span data-stu-id="5eafa-155">Time the report was created.</span></span> <span data-ttu-id="5eafa-156">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="5eafa-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5eafa-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="5eafa-157">ModifiedTime</span></span>     |    <span data-ttu-id="5eafa-158">Ora dell'ultima modifica del report.</span><span class="sxs-lookup"><span data-stu-id="5eafa-158">Time the report was last modified.</span></span> <span data-ttu-id="5eafa-159">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="5eafa-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5eafa-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="5eafa-160">ExecuteNow</span></span>     |    <span data-ttu-id="5eafa-161">Flag ExecuteNow impostato al momento della creazione del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="5eafa-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="5eafa-162">StartTime</span></span>     |    <span data-ttu-id="5eafa-163">Ora di inizio dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="5eafa-163">Time the report execution will begin.</span></span> <span data-ttu-id="5eafa-164">Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="5eafa-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="5eafa-165">Stato report</span><span class="sxs-lookup"><span data-stu-id="5eafa-165">ReportStatus</span></span>     |    <span data-ttu-id="5eafa-166">Stato dell'esecuzione del report.</span><span class="sxs-lookup"><span data-stu-id="5eafa-166">Status of the report execution.</span></span> <span data-ttu-id="5eafa-167">I valori possibili sono Paused, Active e Inactive.</span><span class="sxs-lookup"><span data-stu-id="5eafa-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="5eafa-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="5eafa-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="5eafa-169">Intervallo di ricorrenza specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="5eafa-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="5eafa-170">RecurrenceCount</span></span>     |    <span data-ttu-id="5eafa-171">Numero di ricorrenze specificato durante la creazione del report</span><span class="sxs-lookup"><span data-stu-id="5eafa-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="5eafa-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="5eafa-172">CallbackUrl</span></span>     |    <span data-ttu-id="5eafa-173">URL di callback specificato nella richiesta</span><span class="sxs-lookup"><span data-stu-id="5eafa-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="5eafa-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="5eafa-174">CallbackMethod</span></span>    |    <span data-ttu-id="5eafa-175">Metodo di callback fornito nella richiesta</span><span class="sxs-lookup"><span data-stu-id="5eafa-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="5eafa-176">Formato</span><span class="sxs-lookup"><span data-stu-id="5eafa-176">Format</span></span>     |    <span data-ttu-id="5eafa-177">Formato dei file di report</span><span class="sxs-lookup"><span data-stu-id="5eafa-177">Format of the report files</span></span>     |
|    <span data-ttu-id="5eafa-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5eafa-178">TotalCount</span></span>     |    <span data-ttu-id="5eafa-179">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="5eafa-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="5eafa-180">Message</span><span class="sxs-lookup"><span data-stu-id="5eafa-180">Message</span></span>     |    <span data-ttu-id="5eafa-181">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="5eafa-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="5eafa-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="5eafa-182">StatusCode</span></span>     |    <span data-ttu-id="5eafa-183">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="5eafa-183">Result Code.</span></span> <span data-ttu-id="5eafa-184">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="5eafa-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
