---
title: Riprendere l'esecuzione del report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per riprendere l'esecuzione di qualsiasi report sospeso in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375595"
---
# <a name="resume-report-executions-api"></a>Riprendere l'API di esecuzione dei report

In fase di esecuzione, questa API riprende l'esecuzione pianificata di un report sospeso.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

**Intestazione della richiesta**

|    Intestazione    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |
|    Autorizzazione    |    string    |    Obbligatorio. Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parametro Path**

|    Nome parametro    |    Tipo    |    Obbligatoria    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    stringa    |    No    |    ID del report da modificare     |
|        |        |        |        |

**Query parameter (Parametro di query)**

Nessuno

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

**Glossario**

Questa tabella definisce gli elementi chiave nella risposta:

|    Parametro    |    Descrizione    |
|    ----    |    ----    |
|    ReportId     |    Identificatore univoco universale (UUID) del report ripreso     |
|    ReportName     |    Nome assegnato al report durante la creazione     |
|    Descrizione     |    Descrizione specificata durante la creazione del report     |
|    QueryId     |    ID query passato al momento della creazione del report     |
|    Query     |    Testo della query che verrà eseguito per questo report     |
|    User     |    ID utente usato per creare il report     |
|    CreatedTime     |    Ora di creazione del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ModifiedTime     |    Ora dell'ultima modifica del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ExecuteNow     |    Flag ExecuteNow impostato al momento della creazione del report    |
|    StartTime     |    Ora di inizio dell'esecuzione del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    Stato report     |    Stato dell'esecuzione del report. I valori possibili sono Paused, Active e Inactive.     |
|    RecurrenceInterval     |    Intervallo di ricorrenza specificato durante la creazione del report     |
|    RecurrenceCount     |    Numero di ricorrenze specificato durante la creazione del report     |
|    CallbackUrl     |    URL di callback specificato nella richiesta     |
|    CallbackMethod    |    Metodo di callback fornito nella richiesta    |
|    Formato     |    Formato dei file di report     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |
