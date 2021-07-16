---
title: Provare l'API delle query di report
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per testare la query e convalidare i risultati in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375583"
---
# <a name="try-report-queries-api"></a>Provare l'API delle query di report

Questa API esegue un'istruzione di query Report. L'API restituisce solo 100 record che il partner può usare per verificare se i dati sono come previsto.

> [!IMPORTANT]
> Questa API ha un timeout di esecuzione delle query di 100 secondi. Se si nota che l'API sta prendendo più di 100 secondi, è molto probabile che la query sia sintatticamente corretta, altrimenti si riceverebbe un codice di errore diverso da 200. La generazione di report effettiva verrà superata se la sintassi della query è corretta.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Intestazione della richiesta**

|    Intestazione    |    Tipo    |    Descrizione    |
|    ----    |    ----    |    ----    |
|    Autorizzazione    |    string    |    Obbligatorio. Token Azure Active Directory di accesso di Azure Active Directory (AAD) nel formato`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parametro Path**

Nessuno

**Query parameter (Parametro di query)**

|    Nome parametro    |    Tipo    |    Obbligatoria    |    Descrizione    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    stringa    |    No    |    Stringa di query del report che deve essere eseguita     |
|    queryId     |    stringa    |    No    |    ID di query esistente valido. Si escludono a vicenda con la stringa di query specificata nel parametro exportQuery    |
|    startTime     |    stringa    |    No    |    Ora di inizio da cui si vogliono i dati. Esegue l'override dell'intervallo di tempo specificato nella query    |
|    endTime     |    stringa    |    No    |    Ora di fine fino alla quale si vogliono i dati. Esegue l'override dell'intervallo di tempo specificato nella query    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |
