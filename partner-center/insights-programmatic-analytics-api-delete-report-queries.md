---
title: API Elimina query report - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per eliminare query definite dall'utente in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375378"
---
# <a name="delete-report-queries-api"></a>API Elimina query di report

Questa API elimina le query definite dall'utente.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    DOLETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Intestazione della richiesta**

|    Intestazione    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |
|    Autorizzazione    |    string    |    Obbligatorio. Token Azure Active Directory (AAD) nel formato`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parametro Path**

|    Nome parametro    |    Tipo    |    Obbligatoria    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    stringa     |    No    |    Filtrare per ottenere i dettagli solo delle query con l'ID specificato nell'argomento     |
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
|    QueryId     |    UUID univoco della query eliminata    |
|    Name     |    Nome della query eliminata    |
|    Descrizione     |    Descrizione della query eliminata     |
|    Query     |    Stringa di query del report della query eliminata    |
|    Tipo     |    Impostare su userDefined per le query create dall'utente     |
|    User     |    ID utente che ha creato la query     |
|    CreatedTime     |    Ora di creazione della query     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |
