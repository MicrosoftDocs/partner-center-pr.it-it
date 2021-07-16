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
# <a name="sample-queries-for-partner-center-insights-report"></a>Query di esempio per il report Partner Center insights

Questo articolo fornisce query di esempio per i report Insights partner. È possibile usare queste query chiamando l'endpoint dell'API Di creazione query report. Se necessario, è [possibile modificare la chiamata all'API Create Report Query](insights-programmatic-access-paradigm.md#create-report-query-api) per aggiungere altre colonne, modificare il periodo di calcolo e aggiungere condizioni di filtro.

Per informazioni dettagliate sui nomi, gli attributi e le descrizioni delle colonne, vedere [Definizioni dei dati.](insights-data-definitions.md)

## <a name="customer-details"></a>Dettagli del cliente

Queste query di esempio si applicano al report dei dettagli dei clienti:

### <a name="by-geography"></a>Per area geografica

Elenco di clienti di una specifica area geografica del mese scorso.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Per SKU e ricavi fatturati

L'elenco dei clienti che usano SKU e ricavi fatturati specifici è superiore a 20.000 negli ultimi 6 mesi

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>In base alle postazioni disponibili

Top 10 customers based on Available seats in last month

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Profilo partner

Queste query di esempio si applicano al report del profilo partner:

### <a name="by-geography"></a>Per area geografica

Elenco di partner da una specifica area geografica.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Per partner MPN

Elenco di partner nello stesso partner MPN PGA

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Reseller Performance

Queste query di esempio si applicano al report sulle prestazioni del rivenditore:

### <a name="by-geography"></a>Per area geografica

Elenco di rivenditori di una specifica area geografica del mese scorso.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Per rivenditore

Numero di clienti, numero di sottoscrizioni, totale di postazioni disponibili, totale delle postazioni assegnate, ricavi totali per un rivenditore specifico.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Top 10 by revenue

Primi 10 rivenditori in base ai ricavi totali nell'ultimo mese.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Dettagli sottoscrizione

Queste query di esempio si applicano al report dei dettagli della sottoscrizione:

### <a name="by-renewal-eligibility"></a>In base all'idoneità al rinnovo

Elenco delle sottoscrizioni che non sono idonee per il rinnovo automatico nell'ultimo mese.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Per stato della sottoscrizione

Elenco delle sottoscrizioni con stato Disabilita nell'ultimo mese.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Conteggi per sei mesi

Numero di sottoscrizioni, postazioni vendute totali, numero di clienti per un partner specifico negli ultimi sei mesi.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Utilizzo di Azure

Queste query di esempio si applicano al report sull'utilizzo di Azure:

### <a name="by-meter-category"></a>Per categoria del contatore

Elenco delle sottoscrizioni di utilizzo di Azure con unità di utilizzo e ACR per una categoria di contatori specifica negli ultimi sei mesi.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Per totale ACR

Elenco delle sottoscrizioni di utilizzo di Azure in cui il totale di ACR è maggiore di 20.000 negli ultimi sei mesi

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Passaggi successivi

- [API per l'accesso ai dati analitici delle informazioni dettagliate dei partner](insights-programmatic-analytics-available-api.md)