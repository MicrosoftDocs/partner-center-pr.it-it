---
title: Elenco di query di esempio
description: Usare le query di esempio per accedere a livello di codice ai dati analitici delle informazioni dettagliate dei partner.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375340"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="e2fb9-103">Query di esempio per il report Partner Center insights</span><span class="sxs-lookup"><span data-stu-id="e2fb9-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="e2fb9-104">Questo articolo fornisce query di esempio per i report Insights partner.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="e2fb9-105">È possibile usare queste query chiamando l'endpoint dell'API Di creazione query report.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="e2fb9-106">Se necessario, è [possibile modificare la chiamata all'API Create Report Query](insights-programmatic-access-paradigm.md#create-report-query-api) per aggiungere altre colonne, modificare il periodo di calcolo e aggiungere condizioni di filtro.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="e2fb9-107">Per informazioni dettagliate sui nomi, gli attributi e le descrizioni delle colonne, vedere [Definizioni dei dati.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="e2fb9-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="e2fb9-108">Dettagli del cliente</span><span class="sxs-lookup"><span data-stu-id="e2fb9-108">Customer details</span></span>

<span data-ttu-id="e2fb9-109">Queste query di esempio si applicano al report dei dettagli dei clienti:</span><span class="sxs-lookup"><span data-stu-id="e2fb9-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="e2fb9-110">Per area geografica</span><span class="sxs-lookup"><span data-stu-id="e2fb9-110">By geography</span></span>

<span data-ttu-id="e2fb9-111">Elenco di clienti di una specifica area geografica del mese scorso.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="e2fb9-112">Per SKU e ricavi fatturati</span><span class="sxs-lookup"><span data-stu-id="e2fb9-112">By SKU and billed revenue</span></span>

<span data-ttu-id="e2fb9-113">L'elenco dei clienti che usano SKU e ricavi fatturati specifici è superiore a 20.000 negli ultimi 6 mesi</span><span class="sxs-lookup"><span data-stu-id="e2fb9-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="e2fb9-114">In base alle postazioni disponibili</span><span class="sxs-lookup"><span data-stu-id="e2fb9-114">By available seats</span></span>

<span data-ttu-id="e2fb9-115">Top 10 customers based on Available seats in last month</span><span class="sxs-lookup"><span data-stu-id="e2fb9-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="e2fb9-116">Profilo partner</span><span class="sxs-lookup"><span data-stu-id="e2fb9-116">Partner Profile</span></span>

<span data-ttu-id="e2fb9-117">Queste query di esempio si applicano al report del profilo partner:</span><span class="sxs-lookup"><span data-stu-id="e2fb9-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="e2fb9-118">Per area geografica</span><span class="sxs-lookup"><span data-stu-id="e2fb9-118">By geography</span></span>

<span data-ttu-id="e2fb9-119">Elenco di partner da una specifica area geografica.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="e2fb9-120">Per partner MPN</span><span class="sxs-lookup"><span data-stu-id="e2fb9-120">By MPN partner</span></span>

<span data-ttu-id="e2fb9-121">Elenco di partner nello stesso partner MPN PGA</span><span class="sxs-lookup"><span data-stu-id="e2fb9-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="e2fb9-122">Reseller Performance</span><span class="sxs-lookup"><span data-stu-id="e2fb9-122">Reseller Performance</span></span>

<span data-ttu-id="e2fb9-123">Queste query di esempio si applicano al report sulle prestazioni del rivenditore:</span><span class="sxs-lookup"><span data-stu-id="e2fb9-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="e2fb9-124">Per area geografica</span><span class="sxs-lookup"><span data-stu-id="e2fb9-124">By geography</span></span>

<span data-ttu-id="e2fb9-125">Elenco di rivenditori di una specifica area geografica del mese scorso.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="e2fb9-126">Per rivenditore</span><span class="sxs-lookup"><span data-stu-id="e2fb9-126">By reseller</span></span>

<span data-ttu-id="e2fb9-127">Numero di clienti, numero di sottoscrizioni, totale di postazioni disponibili, totale delle postazioni assegnate, ricavi totali per un rivenditore specifico.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="e2fb9-128">Top 10 by revenue</span><span class="sxs-lookup"><span data-stu-id="e2fb9-128">Top 10 by revenue</span></span>

<span data-ttu-id="e2fb9-129">Primi 10 rivenditori in base ai ricavi totali nell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="e2fb9-130">Dettagli sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="e2fb9-130">Subscription Details</span></span>

<span data-ttu-id="e2fb9-131">Queste query di esempio si applicano al report dei dettagli della sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="e2fb9-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="e2fb9-132">In base all'idoneità al rinnovo</span><span class="sxs-lookup"><span data-stu-id="e2fb9-132">By renewal eligibility</span></span>

<span data-ttu-id="e2fb9-133">Elenco delle sottoscrizioni che non sono idonee per il rinnovo automatico nell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="e2fb9-134">Per stato della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="e2fb9-134">By subscription state</span></span>

<span data-ttu-id="e2fb9-135">Elenco delle sottoscrizioni con stato Disabilita nell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="e2fb9-136">Conteggi per sei mesi</span><span class="sxs-lookup"><span data-stu-id="e2fb9-136">Counts for six months</span></span>

<span data-ttu-id="e2fb9-137">Numero di sottoscrizioni, postazioni vendute totali, numero di clienti per un partner specifico negli ultimi sei mesi.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="e2fb9-138">Utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="e2fb9-138">Azure Usage</span></span>

<span data-ttu-id="e2fb9-139">Queste query di esempio si applicano al report sull'utilizzo di Azure:</span><span class="sxs-lookup"><span data-stu-id="e2fb9-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="e2fb9-140">Per categoria del contatore</span><span class="sxs-lookup"><span data-stu-id="e2fb9-140">By meter category</span></span>

<span data-ttu-id="e2fb9-141">Elenco delle sottoscrizioni di utilizzo di Azure con unità di utilizzo e ACR per una categoria di contatori specifica negli ultimi sei mesi.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="e2fb9-142">Per totale ACR</span><span class="sxs-lookup"><span data-stu-id="e2fb9-142">By total ACR</span></span>

<span data-ttu-id="e2fb9-143">Elenco delle sottoscrizioni di utilizzo di Azure in cui il totale di ACR è maggiore di 20.000 negli ultimi sei mesi</span><span class="sxs-lookup"><span data-stu-id="e2fb9-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="e2fb9-144">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="e2fb9-144">Next steps</span></span>

- [<span data-ttu-id="e2fb9-145">API per l'accesso ai dati analitici delle informazioni dettagliate dei partner</span><span class="sxs-lookup"><span data-stu-id="e2fb9-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)