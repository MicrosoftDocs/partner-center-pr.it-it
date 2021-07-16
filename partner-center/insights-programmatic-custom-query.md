---
title: Specifica di query personalizzate
description: Informazioni su come creare query personalizzate per l'estrazione di dati dalle tabelle di analisi.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375565"
---
# <a name="custom-query-specification"></a><span data-ttu-id="90e5e-103">Specifica di query personalizzate</span><span class="sxs-lookup"><span data-stu-id="90e5e-103">Custom query specification</span></span>

<span data-ttu-id="90e5e-104">I partner possono usare questa specifica di query per formulare facilmente query personalizzate per l'estrazione dei dati dalle tabelle di analisi.</span><span class="sxs-lookup"><span data-stu-id="90e5e-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="90e5e-105">Le query possono essere usate per selezionare solo le colonne e le metriche desiderate che corrispondono a un determinato criterio.</span><span class="sxs-lookup"><span data-stu-id="90e5e-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="90e5e-106">La base della specifica del linguaggio è la definizione del set di dati in cui è possibile scrivere una query personalizzata.</span><span class="sxs-lookup"><span data-stu-id="90e5e-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="90e5e-107">Set di dati</span><span class="sxs-lookup"><span data-stu-id="90e5e-107">Datasets</span></span>

<span data-ttu-id="90e5e-108">Nello stesso modo in cui alcune query vengono eseguite su un database con tabelle e colonne, una query personalizzata funziona su set di dati con colonne e metriche.</span><span class="sxs-lookup"><span data-stu-id="90e5e-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="90e5e-109">L'elenco completo dei set di dati disponibili per la formulazione di una query può essere ottenuto usando l'API dei set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="90e5e-110">Di seguito è riportato un esempio di set di dati visualizzato come JSON:</span><span class="sxs-lookup"><span data-stu-id="90e5e-110">This is an example of a dataset shown as a JSON:</span></span>

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a><span data-ttu-id="90e5e-111">Parti di un set di dati</span><span class="sxs-lookup"><span data-stu-id="90e5e-111">Parts of a dataset</span></span>

- <span data-ttu-id="90e5e-112">Un nome di set di dati è simile al nome di una tabella di database.</span><span class="sxs-lookup"><span data-stu-id="90e5e-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="90e5e-113">Ad esempio, OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="90e5e-113">For example, OfficeUsage.</span></span> <span data-ttu-id="90e5e-114">Un set di dati include un elenco di colonne che è possibile selezionare, ad esempio CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="90e5e-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="90e5e-115">Un set di dati include anche metriche, che sono simili alle funzioni di aggregazione in un database.</span><span class="sxs-lookup"><span data-stu-id="90e5e-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="90e5e-116">Ad esempio, TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="90e5e-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="90e5e-117">Esistono intervalli di tempo fissi in cui è possibile esportare i dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="90e5e-118">Formulare una query su un set di dati</span><span class="sxs-lookup"><span data-stu-id="90e5e-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="90e5e-119">Di seguito sono riportati alcuni esempi di query che illustrano come estrarre vari tipi di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="90e5e-120">Query</span><span class="sxs-lookup"><span data-stu-id="90e5e-120">Query</span></span>|    <span data-ttu-id="90e5e-121">Descrizione</span><span class="sxs-lookup"><span data-stu-id="90e5e-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="90e5e-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="90e5e-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="90e5e-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="90e5e-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="90e5e-124">Questa query otterrà ogni CusotmerTenantID e il corrispondente PaidAvailableUnits nell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="90e5e-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="90e5e-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="90e5e-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="90e5e-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="90e5e-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="90e5e-127">Questa query otterrà i primi 10 tenant dei clienti in ordine decrescente in base al numero di unità disponibili a pagamento.</span><span class="sxs-lookup"><span data-stu-id="90e5e-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="90e5e-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="90e5e-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="90e5e-129">Questa query otterrà le proprietà PaidAvailableUnits e MonthlyActiveUsers di tutti i clienti con MonthlyActiveUsers maggiori di 100.000.</span><span class="sxs-lookup"><span data-stu-id="90e5e-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="90e5e-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="90e5e-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="90e5e-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="90e5e-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="90e5e-132">Questa query otterrà customerTenantId e gli utenti attivi mensili per ogni mese in base ai due valori CustomerTpId: '2a31c234-1f4e-4c60-909e-76d234f93161' e '80780748-3f9a-11eb-b378-0242ac130002'.</span><span class="sxs-lookup"><span data-stu-id="90e5e-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="90e5e-133">Specifica della query</span><span class="sxs-lookup"><span data-stu-id="90e5e-133">Query specification</span></span>

<span data-ttu-id="90e5e-134">In questa sezione vengono descritte la definizione e la struttura della query.</span><span class="sxs-lookup"><span data-stu-id="90e5e-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="90e5e-135">Informazioni di riferimento sulla grammatica</span><span class="sxs-lookup"><span data-stu-id="90e5e-135">Grammar reference</span></span>

<span data-ttu-id="90e5e-136">Questa tabella descrive i simboli utilizzati nelle query.</span><span class="sxs-lookup"><span data-stu-id="90e5e-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="90e5e-137">Query</span><span class="sxs-lookup"><span data-stu-id="90e5e-137">Query</span></span>    |    <span data-ttu-id="90e5e-138">Descrizione</span><span class="sxs-lookup"><span data-stu-id="90e5e-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="90e5e-139">Facoltativo</span><span class="sxs-lookup"><span data-stu-id="90e5e-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="90e5e-140">Zero o più</span><span class="sxs-lookup"><span data-stu-id="90e5e-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="90e5e-141">Uno o più</span><span class="sxs-lookup"><span data-stu-id="90e5e-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="90e5e-142">Oppure / Uno degli elenchi</span><span class="sxs-lookup"><span data-stu-id="90e5e-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="90e5e-143">Definizione query</span><span class="sxs-lookup"><span data-stu-id="90e5e-143">Query definition</span></span>

<span data-ttu-id="90e5e-144">L'istruzione di query include le clausole seguenti: SelectClause, FromClause, WhereClause, OrderClause, LimitClause e TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="90e5e-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="90e5e-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="90e5e-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="90e5e-146">**ColumOrMetricName:** colonne e metriche definite all'interno del set di dati</span><span class="sxs-lookup"><span data-stu-id="90e5e-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="90e5e-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="90e5e-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="90e5e-148">**DatasetName:** nome del set di dati definito all'interno del set di dati</span><span class="sxs-lookup"><span data-stu-id="90e5e-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="90e5e-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="90e5e-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="90e5e-150">**FilterCondition:** valore dell'operatore ColumOrMetricName</span><span class="sxs-lookup"><span data-stu-id="90e5e-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="90e5e-151">**Operatore**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="90e5e-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="90e5e-152">**Valore**: numero | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="90e5e-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="90e5e-153">**Numero**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="90e5e-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="90e5e-154">**StringLiteral:**`' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="90e5e-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="90e5e-155">**MultiNumberList**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="90e5e-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="90e5e-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="90e5e-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="90e5e-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="90e5e-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="90e5e-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="90e5e-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="90e5e-159">**LimitClause**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="90e5e-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="90e5e-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="90e5e-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="90e5e-161">Struttura della query</span><span class="sxs-lookup"><span data-stu-id="90e5e-161">Query Structure</span></span>

<span data-ttu-id="90e5e-162">Una query report è costituito da più parti:</span><span class="sxs-lookup"><span data-stu-id="90e5e-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="90e5e-163">Ogni parte è descritta di seguito.</span><span class="sxs-lookup"><span data-stu-id="90e5e-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="90e5e-164">Questa parte della query specifica le colonne che verranno esportate.</span><span class="sxs-lookup"><span data-stu-id="90e5e-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="90e5e-165">Le colonne che è possibile selezionare sono i campi elencati nelle *sezioni selectableColumns* e *availableMetrics* di un set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="90e5e-166">Facoltativamente, `DISTINCT` è possibile specificare la parola chiave dopo `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="90e5e-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="90e5e-167">Se `DISTINCT` viene specificato , le righe esportate finali conterranno sempre valori distinti delle colonne selezionate.</span><span class="sxs-lookup"><span data-stu-id="90e5e-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="90e5e-168">Le metriche verranno calcolate per ogni combinazione distinta delle colonne selezionate, pertanto la parola chiave non è obbligatoria quando una colonna della metrica viene `DISTINCT` inclusa nell'elenco di selezione delle colonne.</span><span class="sxs-lookup"><span data-stu-id="90e5e-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="90e5e-169">**Esempio:**</span><span class="sxs-lookup"><span data-stu-id="90e5e-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="90e5e-170">Questa parte della query indica il set di dati da cui devono essere esportati i dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="90e5e-171">Il nome del set di dati qui specificato deve essere un nome di set di dati valido restituito dall'API dei set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="90e5e-172">**Esempio:**</span><span class="sxs-lookup"><span data-stu-id="90e5e-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="90e5e-173">Questa parte della query viene usata per specificare le condizioni di filtro per il set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="90e5e-174">Solo le righe corrispondenti a tutte le condizioni elencate in questa clausola saranno presenti nel file esportato finale.</span><span class="sxs-lookup"><span data-stu-id="90e5e-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="90e5e-175">La condizione di filtro può essere in una qualsiasi delle colonne elencate in *selectableColumns* e *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="90e5e-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="90e5e-176">I valori specificati nella condizione di filtro possono essere un elenco di numeri o un elenco di stringhe solo quando l'operatore è `IN` o `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="90e5e-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="90e5e-177">I valori possono sempre essere specificati come stringa letterale e verranno convertiti nei tipi nativi di colonne.</span><span class="sxs-lookup"><span data-stu-id="90e5e-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="90e5e-178">Più condizioni di filtro devono essere separate con un'operazione AND.</span><span class="sxs-lookup"><span data-stu-id="90e5e-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="90e5e-179">**Esempio:**</span><span class="sxs-lookup"><span data-stu-id="90e5e-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="90e5e-180">Questa parte della query specifica i criteri di ordinamento per le righe esportate.</span><span class="sxs-lookup"><span data-stu-id="90e5e-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="90e5e-181">Le colonne in cui è possibile definire l'ordinamento devono essere da *selectableColumns* e *availableMetrics* del set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="90e5e-182">Se non è specificata alcuna direzione di ordinamento, per impostazione predefinita verrà impostata su DESC nella colonna.</span><span class="sxs-lookup"><span data-stu-id="90e5e-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="90e5e-183">L'ordinamento può essere definito in più colonne separando i criteri con una virgola.</span><span class="sxs-lookup"><span data-stu-id="90e5e-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="90e5e-184">**Esempio:**</span><span class="sxs-lookup"><span data-stu-id="90e5e-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="90e5e-185">Questa parte della query specifica il numero di righe che verranno esportate.</span><span class="sxs-lookup"><span data-stu-id="90e5e-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="90e5e-186">Il numero specificato deve essere un numero intero positivo diverso da zero.</span><span class="sxs-lookup"><span data-stu-id="90e5e-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="90e5e-187">Questa parte della query specifica la durata dell'esportazione dei dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="90e5e-188">I valori possibili devono essere del campo *availableDateRanges* nella definizione del set di dati.</span><span class="sxs-lookup"><span data-stu-id="90e5e-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="90e5e-189">Distinzione tra maiuscole e minuscole nella specifica della query</span><span class="sxs-lookup"><span data-stu-id="90e5e-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="90e5e-190">La specifica non fa distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="90e5e-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="90e5e-191">È possibile specificare parole chiave, nomi di colonna e valori predefiniti usando lettere maiuscole o minuscole.</span><span class="sxs-lookup"><span data-stu-id="90e5e-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="90e5e-192">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="90e5e-192">Next steps</span></span>

- [<span data-ttu-id="90e5e-193">Elenco di query di sistema</span><span class="sxs-lookup"><span data-stu-id="90e5e-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="90e5e-194">Elenco di query di esempio</span><span class="sxs-lookup"><span data-stu-id="90e5e-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)