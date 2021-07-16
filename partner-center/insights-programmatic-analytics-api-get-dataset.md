---
title: Ottenere tutti i set di dati - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere i dettagli di tutti i set di dati disponibili in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375359"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="049f7-103">Ottenere tutti i set di dati API</span><span class="sxs-lookup"><span data-stu-id="049f7-103">Get all datasets API</span></span>

<span data-ttu-id="049f7-104">L'API Recupera tutti i set di dati ottiene tutti i set di dati disponibili.</span><span class="sxs-lookup"><span data-stu-id="049f7-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="049f7-105">I set di dati elencano tabelle, colonne, metriche e intervalli di tempo.</span><span class="sxs-lookup"><span data-stu-id="049f7-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="049f7-106">**Sintassi della richiesta**</span><span class="sxs-lookup"><span data-stu-id="049f7-106">**Request syntax**</span></span>

|    <span data-ttu-id="049f7-107">Metodo</span><span class="sxs-lookup"><span data-stu-id="049f7-107">Method</span></span>    |    <span data-ttu-id="049f7-108">URI richiesta</span><span class="sxs-lookup"><span data-stu-id="049f7-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="049f7-109">GET</span><span class="sxs-lookup"><span data-stu-id="049f7-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="049f7-110">**Intestazione della richiesta**</span><span class="sxs-lookup"><span data-stu-id="049f7-110">**Request header**</span></span>

|    <span data-ttu-id="049f7-111">Intestazione</span><span class="sxs-lookup"><span data-stu-id="049f7-111">Header</span></span>    |    <span data-ttu-id="049f7-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="049f7-112">Type</span></span>    |    <span data-ttu-id="049f7-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="049f7-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="049f7-114">Autorizzazione</span><span class="sxs-lookup"><span data-stu-id="049f7-114">Authorization</span></span>    |    <span data-ttu-id="049f7-115">string</span><span class="sxs-lookup"><span data-stu-id="049f7-115">string</span></span>    |    <span data-ttu-id="049f7-116">Obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="049f7-116">Required.</span></span> <span data-ttu-id="049f7-117">Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="049f7-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="049f7-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="049f7-118">Content-Type</span></span>    |    <span data-ttu-id="049f7-119">string</span><span class="sxs-lookup"><span data-stu-id="049f7-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="049f7-120">**Parametro Path**</span><span class="sxs-lookup"><span data-stu-id="049f7-120">**Path parameter**</span></span>

<span data-ttu-id="049f7-121">Nessuno</span><span class="sxs-lookup"><span data-stu-id="049f7-121">None</span></span>

<span data-ttu-id="049f7-122">**Query parameter (Parametro di query)**</span><span class="sxs-lookup"><span data-stu-id="049f7-122">**Query parameter**</span></span>

|    <span data-ttu-id="049f7-123">Nome parametro</span><span class="sxs-lookup"><span data-stu-id="049f7-123">Parameter Name</span></span>    |    <span data-ttu-id="049f7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="049f7-124">Type</span></span>    |    <span data-ttu-id="049f7-125">Obbligatoria</span><span class="sxs-lookup"><span data-stu-id="049f7-125">Required</span></span>    |    <span data-ttu-id="049f7-126">Descrizione</span><span class="sxs-lookup"><span data-stu-id="049f7-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="049f7-127">Datasetname</span><span class="sxs-lookup"><span data-stu-id="049f7-127">datasetName</span></span>    |    <span data-ttu-id="049f7-128">stringa</span><span class="sxs-lookup"><span data-stu-id="049f7-128">string</span></span>    |    <span data-ttu-id="049f7-129">No</span><span class="sxs-lookup"><span data-stu-id="049f7-129">No</span></span>    |    <span data-ttu-id="049f7-130">Filtrare per ottenere i dettagli di un solo set di dati</span><span class="sxs-lookup"><span data-stu-id="049f7-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="049f7-131">**Payload della richiesta**</span><span class="sxs-lookup"><span data-stu-id="049f7-131">**Request payload**</span></span>

<span data-ttu-id="049f7-132">Nessuno</span><span class="sxs-lookup"><span data-stu-id="049f7-132">None</span></span>

<span data-ttu-id="049f7-133">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="049f7-133">**Glossary**</span></span>

<span data-ttu-id="049f7-134">Nessuno</span><span class="sxs-lookup"><span data-stu-id="049f7-134">None</span></span>

<span data-ttu-id="049f7-135">**Risposta**</span><span class="sxs-lookup"><span data-stu-id="049f7-135">**Response**</span></span>

<span data-ttu-id="049f7-136">Il payload della risposta è strutturato come segue:</span><span class="sxs-lookup"><span data-stu-id="049f7-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="049f7-137">Codice di risposta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="049f7-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="049f7-138">Esempio di payload della risposta:</span><span class="sxs-lookup"><span data-stu-id="049f7-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="049f7-139">**Glossario**</span><span class="sxs-lookup"><span data-stu-id="049f7-139">**Glossary**</span></span>

<span data-ttu-id="049f7-140">Questa tabella definisce gli elementi chiave nella risposta:</span><span class="sxs-lookup"><span data-stu-id="049f7-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="049f7-141">Parametro</span><span class="sxs-lookup"><span data-stu-id="049f7-141">Parameter</span></span>    |    <span data-ttu-id="049f7-142">Descrizione</span><span class="sxs-lookup"><span data-stu-id="049f7-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="049f7-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="049f7-143">DatasetName</span></span>     |    <span data-ttu-id="049f7-144">Nome del set di dati definito da questo oggetto matrice</span><span class="sxs-lookup"><span data-stu-id="049f7-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="049f7-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="049f7-145">SelectableColumns</span></span>     |    <span data-ttu-id="049f7-146">Colonne non elaborati che possono essere specificate nelle colonne selezionate</span><span class="sxs-lookup"><span data-stu-id="049f7-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="049f7-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="049f7-147">AvailableMetrics</span></span>     |    <span data-ttu-id="049f7-148">Nomi delle colonne di aggregazione/metrica che possono essere specificati nelle colonne selezionate</span><span class="sxs-lookup"><span data-stu-id="049f7-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="049f7-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="049f7-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="049f7-150">Intervallo di date che può essere usato nelle query del report per il set di dati</span><span class="sxs-lookup"><span data-stu-id="049f7-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="049f7-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="049f7-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="049f7-152">Valore minimo dell'intervallo di ricorrenza</span><span class="sxs-lookup"><span data-stu-id="049f7-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="049f7-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="049f7-153">TotalCount</span></span>     |    <span data-ttu-id="049f7-154">Numero di set di dati nella matrice Value</span><span class="sxs-lookup"><span data-stu-id="049f7-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="049f7-155">Message</span><span class="sxs-lookup"><span data-stu-id="049f7-155">Message</span></span>     |    <span data-ttu-id="049f7-156">Messaggio di stato dall'esecuzione dell'API</span><span class="sxs-lookup"><span data-stu-id="049f7-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="049f7-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="049f7-157">StatusCode</span></span>     |    <span data-ttu-id="049f7-158">Codice risultato.</span><span class="sxs-lookup"><span data-stu-id="049f7-158">Result Code.</span></span> <span data-ttu-id="049f7-159">I valori possibili sono 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="049f7-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
