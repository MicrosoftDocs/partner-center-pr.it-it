---
title: Elenco di API per l'accesso ai dati delle informazioni dettagliate dei partner
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Elenco di API per l'accesso ai dati delle informazioni dettagliate dei partner.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375571"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="bde7b-103">API disponibili per l'analisi delle informazioni dettagliate dei partner</span><span class="sxs-lookup"><span data-stu-id="bde7b-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="bde7b-104">Di seguito è riportato l'elenco delle API per l'analisi delle informazioni dettagliate dei partner e le relative funzionalità associate.</span><span class="sxs-lookup"><span data-stu-id="bde7b-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="bde7b-105">API pull del set di dati</span><span class="sxs-lookup"><span data-stu-id="bde7b-105">Dataset pull APIs</span></span>

<span data-ttu-id="bde7b-106">***Tabella 1: API pull del set di dati***</span><span class="sxs-lookup"><span data-stu-id="bde7b-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="bde7b-107">**API**</span><span class="sxs-lookup"><span data-stu-id="bde7b-107">**API**</span></span> | <span data-ttu-id="bde7b-108">**Funzionalità**</span><span class="sxs-lookup"><span data-stu-id="bde7b-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="bde7b-109">Ottenere tutti i set di dati</span><span class="sxs-lookup"><span data-stu-id="bde7b-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="bde7b-110">Ottiene tutti i set di dati disponibili.</span><span class="sxs-lookup"><span data-stu-id="bde7b-110">Gets all the available datasets.</span></span> <span data-ttu-id="bde7b-111">I set di dati elencano tabelle, colonne, metriche e intervalli di tempo.</span><span class="sxs-lookup"><span data-stu-id="bde7b-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="bde7b-112">API di gestione delle query</span><span class="sxs-lookup"><span data-stu-id="bde7b-112">Query management APIs</span></span>

<span data-ttu-id="bde7b-113">***Tabella 2: API di gestione delle query***</span><span class="sxs-lookup"><span data-stu-id="bde7b-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="bde7b-114">**API**</span><span class="sxs-lookup"><span data-stu-id="bde7b-114">**API**</span></span> | <span data-ttu-id="bde7b-115">**Funzionalità**</span><span class="sxs-lookup"><span data-stu-id="bde7b-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="bde7b-116">Creare una query di report</span><span class="sxs-lookup"><span data-stu-id="bde7b-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="bde7b-117">Crea query personalizzate che definiscono il set di dati da cui devono essere esportate le colonne e le metriche.</span><span class="sxs-lookup"><span data-stu-id="bde7b-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="bde7b-118">GET Report Query</span><span class="sxs-lookup"><span data-stu-id="bde7b-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="bde7b-119">Ottiene tutte le query disponibili per l'utilizzo nei report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="bde7b-120">Ottiene tutte le query di sistema e definite dall'utente per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="bde7b-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="bde7b-121">DELETE Report Query</span><span class="sxs-lookup"><span data-stu-id="bde7b-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="bde7b-122">Elimina le query definite dall'utente.</span><span class="sxs-lookup"><span data-stu-id="bde7b-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="bde7b-123">API di gestione dei report</span><span class="sxs-lookup"><span data-stu-id="bde7b-123">Report management APIs</span></span>

<span data-ttu-id="bde7b-124">***Tabella 3: API di gestione dei report***</span><span class="sxs-lookup"><span data-stu-id="bde7b-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="bde7b-125">**API**</span><span class="sxs-lookup"><span data-stu-id="bde7b-125">**API**</span></span> | <span data-ttu-id="bde7b-126">**Funzionalità**</span><span class="sxs-lookup"><span data-stu-id="bde7b-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="bde7b-127">Creazione di report</span><span class="sxs-lookup"><span data-stu-id="bde7b-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="bde7b-128">Pianifica l'esecuzione di una query a intervalli regolari.</span><span class="sxs-lookup"><span data-stu-id="bde7b-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="bde7b-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="bde7b-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="bde7b-130">Esegue un'istruzione di query Report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-130">Executes a Report query statement.</span></span> <span data-ttu-id="bde7b-131">Restituisce solo 10 record che un partner può usare per verificare se i dati sono come previsto.</span><span class="sxs-lookup"><span data-stu-id="bde7b-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="bde7b-132">Genera report</span><span class="sxs-lookup"><span data-stu-id="bde7b-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="bde7b-133">Ottenere tutti i report pianificati.</span><span class="sxs-lookup"><span data-stu-id="bde7b-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="bde7b-134">Aggiorna report</span><span class="sxs-lookup"><span data-stu-id="bde7b-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="bde7b-135">Modificare un parametro del report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="bde7b-136">Elimina report</span><span class="sxs-lookup"><span data-stu-id="bde7b-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="bde7b-137">Elimina tutti i record di esecuzione del report e del report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="bde7b-138">Sospendere le esecuzioni dei report</span><span class="sxs-lookup"><span data-stu-id="bde7b-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="bde7b-139">Sospende l'esecuzione pianificata dei report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="bde7b-140">Riprendere le esecuzioni dei report</span><span class="sxs-lookup"><span data-stu-id="bde7b-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="bde7b-141">Riprende l'esecuzione pianificata di un report sospeso.</span><span class="sxs-lookup"><span data-stu-id="bde7b-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="bde7b-142">API pull per l'esecuzione di report</span><span class="sxs-lookup"><span data-stu-id="bde7b-142">Report execution pull APIs</span></span>

<span data-ttu-id="bde7b-143">***Tabella 4: API pull di esecuzione dei report***</span><span class="sxs-lookup"><span data-stu-id="bde7b-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="bde7b-144">**API**</span><span class="sxs-lookup"><span data-stu-id="bde7b-144">**API**</span></span> | <span data-ttu-id="bde7b-145">**Funzionalità**</span><span class="sxs-lookup"><span data-stu-id="bde7b-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="bde7b-146">Ottenere le esecuzioni dei report</span><span class="sxs-lookup"><span data-stu-id="bde7b-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="bde7b-147">Ottiene tutte le esecuzioni che si sono verificato per un determinato report.</span><span class="sxs-lookup"><span data-stu-id="bde7b-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="bde7b-148">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="bde7b-148">Next steps</span></span>

- <span data-ttu-id="bde7b-149">È possibile provare le API tramite [l'URL dell'API Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="bde7b-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>