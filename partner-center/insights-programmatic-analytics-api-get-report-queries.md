---
title: Ottenere l'API query di report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere tutte le query disponibili da usare nell'API del report.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375607"
---
# <a name="get-report-queries-api"></a>API Per ottenere query di report

L'API Recupera query report ottiene tutte le query disponibili per l'uso nei report. Ottiene tutte le query di sistema e definite dall'utente per impostazione predefinita.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Intestazione della richiesta**

|    Intestazione    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |
|    Autorizzazione    |    string    |    Obbligatorio. Token Azure Active Directory (AAD) nel formato`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parametro Path**

Nessuno

**Query parameter (Parametro di query)**

|    Nome parametro    |    Tipo    |    Obbligatoria    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    stringa     |    No    |    Filtrare per ottenere i dettagli solo delle query con l'ID specificato nell'argomento     |
|    queryName     |    stringa     |    No    |    Filtrare per ottenere i dettagli solo delle query con il nome specificato nell'argomento     |
|    IncludeSystemQueries     |    boolean     |    No    |    Includere query di sistema predefinite nella risposta     |
|    IncludeOnlySystemQueries     |    boolean     |    No    |    Includere solo query di sistema nella risposta     |
|        |        |        |        |


**Payload della richiesta**

Nessuno

**Glossario**

Nessuno

**Risposta**

Il payload della risposta è strutturato come segue:

Codice di risposta: 200, 400, 401, 403, 404, 500

Esempio di payload della risposta:

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

**Glossario**

Questa tabella definisce gli elementi chiave nella risposta:

|    Parametro    |    Descrizione    |
|    ----    |    ----    |
|    QueryId     |    UUID univoco della query     |
|    Name     |    Nome assegnato alla query al momento della creazione della query     |
|    Descrizione     |    Descrizione specificata durante la creazione della query     |
|    Query     |    Stringa di query del report     |
|    Tipo     |    Impostare su userDefined per le query create dall'utente e il sistema per le query di sistema predefinite     |
|    User     |    ID utente che ha creato la query     |
|    CreatedTime     |    Ora di creazione della query     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |
