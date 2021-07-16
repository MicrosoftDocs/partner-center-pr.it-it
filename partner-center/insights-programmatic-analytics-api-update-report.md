---
title: Aggiornare l'API del report
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per aggiornare i parametri del report in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375578"
---
# <a name="update-report-api"></a>Aggiornare l'API del report

Questa API consente di modificare un parametro del report.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Glossario**

Questa tabella elenca le definizioni chiave degli elementi nella risposta.

|    Parametro    |    Obbligatoria    |    Descrizione    |    Valori consentiti    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Sì     |    Nome da assegnare al report     |    Stringa     |
|    Descrizione     |    No     |    Descrizione del report creato     |    Stringa     |
|    StartTime     |    Sì    |    Timestamp dopo il quale inizierà la generazione del report     |    Stringa     |
|    RecurrenceInterval     |    No     |    Frequenza con cui il report deve essere generato in ore. Il valore minimo è 4     |    Intero     |
|    RecurrenceCount     |    No     |    Numero di report da generare. Il valore predefinito è indefinito.     |    Intero     |
|    Formato     |    No    |    Formato di file del file esportato. Il valore predefinito è CSV     |    CSV/TSV     |
|    CallbackURL     |    No     |    URL di callback HTTPS da chiamare per la generazione di report     |    Stringa     |
|    CallbackMethod    |    No    |    Metodo HTTP da usare per il callback    |    GET/POST    |
|        |        |        |        |


**Response**.

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
|    ReportId     |    Identificatore univoco universale (UUID) del report da aggiornare     |
|    ReportName     |    Nome assegnato al report nel payload della richiesta     |
|    Descrizione     |    Descrizione fornita al report nel payload della richiesta     |
|    QueryId     |    ID query passato al momento della creazione del report     |
|    Query     |    Testo della query che verrà eseguito per questo report     |
|    User     |    ID utente usato per creare il report     |
|    CreatedTime     |    Ora di creazione del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ModifiedTime     |    Ora dell'ultima modifica del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    ExecuteNow     |    Flag ExecuteNow impostato al momento della creazione del report    |
|    StartTime     |    Ora di inizio dell'esecuzione del report. Il formato dell'ora è aaaa-MM-ggTHH:mm:ssZ     |
|    Stato report     |    Stato dell'esecuzione del report. I valori possibili sono Paused, Active e Inactive.     |
|    RecurrenceInterval     |    Intervallo di ricorrenza specificato nel payload della richiesta     |
|    RecurrenceCount     |    Numero di ricorrenze specificato nel payload della richiesta     |
|    CallbackUrl     |    URL di callback specificato nella richiesta     |
|    CallbackMethod    |    Metodo di callback fornito nella richiesta    |
|    Formato     |    Formato dei file di report     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |