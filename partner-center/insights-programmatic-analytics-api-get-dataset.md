---
title: Ottenere tutti i set di dati - Insights dati
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare questa API per ottenere i dettagli di tutti i set di dati disponibili in Partner Center dettagliate.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375359"
---
# <a name="get-all-datasets-api"></a>Ottenere tutti i set di dati API

L'API Recupera tutti i set di dati ottiene tutti i set di dati disponibili. I set di dati elencano tabelle, colonne, metriche e intervalli di tempo.

**Sintassi della richiesta**

|    Metodo    |    URI richiesta    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    Datasetname    |    stringa    |    No    |    Filtrare per ottenere i dettagli di un solo set di dati    |
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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Glossario**

Questa tabella definisce gli elementi chiave nella risposta:

|    Parametro    |    Descrizione    |
|    ----    |    ----    |
|    DatasetName     |    Nome del set di dati definito da questo oggetto matrice     |
|    SelectableColumns     |    Colonne non elaborati che possono essere specificate nelle colonne selezionate     |
|    AvailableMetrics     |    Nomi delle colonne di aggregazione/metrica che possono essere specificati nelle colonne selezionate     |
|    AvailableDateRanges     |    Intervallo di date che può essere usato nelle query del report per il set di dati     |
|    minimumRecurrenceInterval     |    Valore minimo dell'intervallo di ricorrenza     |
|    TotalCount     |    Numero di set di dati nella matrice Value     |
|    Message     |    Messaggio di stato dall'esecuzione dell'API     |
|    StatusCode     |    Codice risultato. I valori possibili sono 200, 400, 401, 403, 500     |
|        |        |
