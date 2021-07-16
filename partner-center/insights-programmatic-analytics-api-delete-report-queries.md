---
title: API Elimina query report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per eliminare query definite dall'utente in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375378"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="d00c9-103">API Elimina query di report</span><span class="sxs-lookup"><span data-stu-id="d00c9-103">Delete report queries API</span></span>

<span data-ttu-id="d00c9-104">Questa API elimina le query definite dall'utente.</span><span class="sxs-lookup"><span data-stu-id="d00c9-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="d00c9-105">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="d00c9-105">**Request syntax**</span></span>

|    <span data-ttu-id="d00c9-106">Metodo</span><span class="sxs-lookup"><span data-stu-id="d00c9-106">Method</span></span>    |    <span data-ttu-id="d00c9-107">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="d00c9-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d00c9-108">DOLETE</span><span class="sxs-lookup"><span data-stu-id="d00c9-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="d00c9-109">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="d00c9-109">**Request header**</span></span>

|    <span data-ttu-id="d00c9-110">Intestazione</span><span class="sxs-lookup"><span data-stu-id="d00c9-110">Header</span></span>    |    <span data-ttu-id="d00c9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d00c9-111">Type</span></span>    |    <span data-ttu-id="d00c9-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="d00c9-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="d00c9-113">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="d00c9-113">Authorization</span></span>    |    <span data-ttu-id="d00c9-114">string</span><span class="sxs-lookup"><span data-stu-id="d00c9-114">string</span></span>    |    <span data-ttu-id="d00c9-115">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="d00c9-115">Required.</span></span> <span data-ttu-id="d00c9-116">Token Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="d00c9-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="d00c9-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d00c9-117">Content-Type</span></span>    |    <span data-ttu-id="d00c9-118">string</span><span class="sxs-lookup"><span data-stu-id="d00c9-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="d00c9-119">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="d00c9-119">**Path parameter**</span></span>

|    <span data-ttu-id="d00c9-120">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="d00c9-120">Parameter Name</span></span>    |    <span data-ttu-id="d00c9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d00c9-121">Type</span></span>    |    <span data-ttu-id="d00c9-122">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="d00c9-122">Required</span></span>    |    <span data-ttu-id="d00c9-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="d00c9-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="d00c9-124">queryId</span><span class="sxs-lookup"><span data-stu-id="d00c9-124">queryId</span></span>     |    <span data-ttu-id="d00c9-125">stringa</span><span class="sxs-lookup"><span data-stu-id="d00c9-125">string</span></span>     |    <span data-ttu-id="d00c9-126">No</span><span class="sxs-lookup"><span data-stu-id="d00c9-126">No</span></span>    |    <span data-ttu-id="d00c9-127">Filtrare per ottenere i dettagli solo delle query con l'ID specificato nell'argomento</span><span class="sxs-lookup"><span data-stu-id="d00c9-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="d00c9-128">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="d00c9-128">**Query parameter**</span></span>

<span data-ttu-id="d00c9-129">Nessuno</span><span class="sxs-lookup"><span data-stu-id="d00c9-129">None</span></span>

<span data-ttu-id="d00c9-130">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="d00c9-130">**Request payload**</span></span>

<span data-ttu-id="d00c9-131">Nessuno</span><span class="sxs-lookup"><span data-stu-id="d00c9-131">None</span></span>

<span data-ttu-id="d00c9-132">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="d00c9-132">**Glossary**</span></span>

<span data-ttu-id="d00c9-133">Nessuno</span><span class="sxs-lookup"><span data-stu-id="d00c9-133">None</span></span>

<span data-ttu-id="d00c9-134">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="d00c9-134">**Response**</span></span>

<span data-ttu-id="d00c9-135">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="d00c9-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="d00c9-136">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="d00c9-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="d00c9-137">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="d00c9-137">Response payload example:</span></span>

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

<span data-ttu-id="d00c9-138">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="d00c9-138">**Glossary**</span></span>

<span data-ttu-id="d00c9-139">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="d00c9-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="d00c9-140">Parametro</span><span class="sxs-lookup"><span data-stu-id="d00c9-140">Parameter</span></span>    |    <span data-ttu-id="d00c9-141">Descrizione</span><span class="sxs-lookup"><span data-stu-id="d00c9-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="d00c9-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="d00c9-142">QueryId</span></span>     |    <span data-ttu-id="d00c9-143">UUID univoco della query eliminata</span><span class="sxs-lookup"><span data-stu-id="d00c9-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="d00c9-144">Name</span><span class="sxs-lookup"><span data-stu-id="d00c9-144">Name</span></span>     |    <span data-ttu-id="d00c9-145">Nome della query eliminata</span><span class="sxs-lookup"><span data-stu-id="d00c9-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="d00c9-146">Descrizione</span><span class="sxs-lookup"><span data-stu-id="d00c9-146">Description</span></span>     |    <span data-ttu-id="d00c9-147">Descrizione della query eliminata</span><span class="sxs-lookup"><span data-stu-id="d00c9-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="d00c9-148">Query</span><span class="sxs-lookup"><span data-stu-id="d00c9-148">Query</span></span>     |    <span data-ttu-id="d00c9-149">Stringa di query del report della query eliminata</span><span class="sxs-lookup"><span data-stu-id="d00c9-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="d00c9-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="d00c9-150">Type</span></span>     |    <span data-ttu-id="d00c9-151">Impostare su userDefined per le query create dall'utente</span><span class="sxs-lookup"><span data-stu-id="d00c9-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="d00c9-152">User</span><span class="sxs-lookup"><span data-stu-id="d00c9-152">User</span></span>     |    <span data-ttu-id="d00c9-153">ID utente che ha creato la query</span><span class="sxs-lookup"><span data-stu-id="d00c9-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="d00c9-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="d00c9-154">CreatedTime</span></span>     |    <span data-ttu-id="d00c9-155">Ora di creazione della query</span><span class="sxs-lookup"><span data-stu-id="d00c9-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="d00c9-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="d00c9-156">TotalCount</span></span>     |    <span data-ttu-id="d00c9-157">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="d00c9-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="d00c9-158">Message</span><span class="sxs-lookup"><span data-stu-id="d00c9-158">Message</span></span>     |    <span data-ttu-id="d00c9-159">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="d00c9-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="d00c9-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="d00c9-160">StatusCode</span></span>     |    <span data-ttu-id="d00c9-161">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="d00c9-161">Result Code.</span></span> <span data-ttu-id="d00c9-162">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="d00c9-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
