---
title: "Ottenere l'API del report : Insights dati"
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere tutti gli ID report disponibili in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375602"
---
# <a name="get-report-api"></a>Ottenere l'API del report

Questa API ottiene tutti i report pianificati.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
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
|    reportId     |    stringa    |    No    |    Filtrare per ottenere i dettagli solo dei report con il reportId specificato in questo argomento     |
|    reportName     |    stringa    |    No    |    Filtrare per ottenere i dettagli solo dei report con reportName specificato in questo argomento     |
|    queryId     |    stringa    |    No    |    Filtrare per ottenere i dettagli solo dei report con queryId specificato in questo argomento     |
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
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Glossario**

Questa tabella definisce gli elementi chiave nella risposta:

|    Parametro    |    Descrizione    |
|    ----    |    ----    |
|    ReportId     |    UUID univoco del report creato     |
|    ReportName     |    Nome assegnato al report nel payload della richiesta     |
|    Descrizione     |    Descrizione data al momento della creazione del report     |
|    QueryId     |    ID query passato al momento della creazione del report     |
|    Query     |    Testo della query che verrà eseguito per questo report     |
|    User     |    ID utente usato per creare il report     |
|    CreatedTime     |    Ora di creazione del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ModifiedTime     |    Ora dell'ultima modifica del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    executeNow     |    Flag ExecuteNow impostato al momento della creazione del report    |
|    StartTime     |    Ora di inizio dell'esecuzione. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ReportStatus     |    Stato dell'esecuzione del report. I valori possibili sono Paused, Active e Inactive.     |
|    RecurrenceInterval     |    Intervallo di ricorrenza specificato durante la creazione del report     |
|    RecurrenceCount     |    Numero di ricorrenze specificato durante la creazione del report     |
|    CallbackUrl     |    URL di callback specificato nella richiesta     |
|    CallbackMethod    |    Metodo di callback fornito nella richiesta    |
|    Formato     |    Formato dei file di report     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |