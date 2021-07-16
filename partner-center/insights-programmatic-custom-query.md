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
# <a name="custom-query-specification"></a>Specifica di query personalizzate

I partner possono usare questa specifica di query per formulare facilmente query personalizzate per l'estrazione dei dati dalle tabelle di analisi. Le query possono essere usate per selezionare solo le colonne e le metriche desiderate che corrispondono a un determinato criterio. La base della specifica del linguaggio è la definizione del set di dati in cui è possibile scrivere una query personalizzata.

## <a name="datasets"></a>Set di dati

Nello stesso modo in cui alcune query vengono eseguite su un database con tabelle e colonne, una query personalizzata funziona su set di dati con colonne e metriche. L'elenco completo dei set di dati disponibili per la formulazione di una query può essere ottenuto usando l'API dei set di dati.

Di seguito è riportato un esempio di set di dati visualizzato come JSON:

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

## <a name="parts-of-a-dataset"></a>Parti di un set di dati

- Un nome di set di dati è simile al nome di una tabella di database. Ad esempio, OfficeUsage. Un set di dati include un elenco di colonne che è possibile selezionare, ad esempio CustomerTenantId.
- Un set di dati include anche metriche, che sono simili alle funzioni di aggregazione in un database. Ad esempio, TotalMonthlyActiveUsers.
- Esistono intervalli di tempo fissi in cui è possibile esportare i dati.

## <a name="formulating-a-query-on-a-dataset"></a>Formulare una query su un set di dati

Di seguito sono riportati alcuni esempi di query che illustrano come estrarre vari tipi di dati.

|Query|    Descrizione    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Questa query otterrà ogni CusotmerTenantID e il corrispondente PaidAvailableUnits nell'ultimo mese.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Questa query otterrà i primi 10 tenant dei clienti in ordine decrescente in base al numero di unità disponibili a pagamento.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Questa query otterrà le proprietà PaidAvailableUnits e MonthlyActiveUsers di tutti i clienti con MonthlyActiveUsers maggiori di 100.000.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Questa query otterrà customerTenantId e gli utenti attivi mensili per ogni mese in base ai due valori CustomerTpId: '2a31c234-1f4e-4c60-909e-76d234f93161' e '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Specifica della query

In questa sezione vengono descritte la definizione e la struttura della query.

## <a name="grammar-reference"></a>Informazioni di riferimento sulla grammatica

Questa tabella descrive i simboli utilizzati nelle query.

|    Query    |    Descrizione    |
|    ----    |    ----    |
|    `?`    |    Facoltativo    |
|    `*`    |    Zero o più    |
|    `+`    |    Uno o più    |
|    `\|`    |    Oppure / Uno degli elenchi    |
|        |        |

## <a name="query-definition"></a>Definizione query

L'istruzione di query include le clausole seguenti: SelectClause, FromClause, WhereClause, OrderClause, LimitClause e TimeSpan.

- **SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** colonne e metriche definite all'interno del set di dati
- **FromClause**: `FROM DatasetName`
    - **DatasetName:** nome del set di dati definito all'interno del set di dati
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** valore dell'operatore ColumOrMetricName
        - **Operatore**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Valore**: numero | StringLiteral | MultiNumberList | MultiStringList
            - **Numero**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral:**`' [a-zA-Z0-9_]*'`
            - **MultiNumberList**: `(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition**: `ColumOrMetricName (ASC | DESC)*`
- **LimitClause**: `LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Struttura della query

Una query report è costituito da più parti:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Ogni parte è descritta di seguito.

### `SELECT`

Questa parte della query specifica le colonne che verranno esportate. Le colonne che è possibile selezionare sono i campi elencati nelle *sezioni selectableColumns* e *availableMetrics* di un set di dati.

Facoltativamente, `DISTINCT` è possibile specificare la parola chiave dopo `SELECT` . Se `DISTINCT` viene specificato , le righe esportate finali conterranno sempre valori distinti delle colonne selezionate. Le metriche verranno calcolate per ogni combinazione distinta delle colonne selezionate, pertanto la parola chiave non è obbligatoria quando una colonna della metrica viene `DISTINCT` inclusa nell'elenco di selezione delle colonne.

**Esempio:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Questa parte della query indica il set di dati da cui devono essere esportati i dati. Il nome del set di dati qui specificato deve essere un nome di set di dati valido restituito dall'API dei set di dati.

**Esempio:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Questa parte della query viene usata per specificare le condizioni di filtro per il set di dati. Solo le righe corrispondenti a tutte le condizioni elencate in questa clausola saranno presenti nel file esportato finale. La condizione di filtro può essere in una qualsiasi delle colonne elencate in *selectableColumns* e *availableMetrics*. I valori specificati nella condizione di filtro possono essere un elenco di numeri o un elenco di stringhe solo quando l'operatore è `IN` o `NOT IN` . I valori possono sempre essere specificati come stringa letterale e verranno convertiti nei tipi nativi di colonne. Più condizioni di filtro devono essere separate con un'operazione AND.

**Esempio:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Questa parte della query specifica i criteri di ordinamento per le righe esportate. Le colonne in cui è possibile definire l'ordinamento devono essere da *selectableColumns* e *availableMetrics* del set di dati. Se non è specificata alcuna direzione di ordinamento, per impostazione predefinita verrà impostata su DESC nella colonna. L'ordinamento può essere definito in più colonne separando i criteri con una virgola.

**Esempio:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Questa parte della query specifica il numero di righe che verranno esportate. Il numero specificato deve essere un numero intero positivo diverso da zero.

### `TIMESPAN`

Questa parte della query specifica la durata dell'esportazione dei dati. I valori possibili devono essere del campo *availableDateRanges* nella definizione del set di dati.

### <a name="case-sensitivity-in-query-specification"></a>Distinzione tra maiuscole e minuscole nella specifica della query

La specifica non fa distinzione tra maiuscole e minuscole. È possibile specificare parole chiave, nomi di colonna e valori predefiniti usando lettere maiuscole o minuscole.

## <a name="next-steps"></a>Passaggi successivi

- [Elenco di query di sistema](insights-programmatic-system-queries.md)
- [Elenco di query di esempio](insights-programmatic-sample-queries.md)