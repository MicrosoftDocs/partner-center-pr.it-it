---
title: Domande comuni sull'accesso a livello di codice per informazioni dettagliate sui partner
description: Risposte alle domande frequenti sull'accesso ai dati delle informazioni dettagliate dei partner tramite l'API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375554"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Domande comuni sull'accesso a livello di codice ai dati di analisi

Questo articolo risolve le domande frequenti su come accedere a livello di codice ai dati di informazioni dettagliate dei partner Partner Center.

## <a name="api-responses"></a>Risposte dell'API

Quali sono i diversi scenari in cui è possibile ricevere una risposta API diversa da 200 (operazione riuscita)?

Questa tabella descrive le risposte dell'API e cosa fare se vengono ricevute.

|    Descrizione errore     |    Codice di errore     |    Risolvere problemi     |
|    ----    |    ----    |    ----    |
|    Non autorizzata     |    401     |    Si tratta di un'eccezione di autenticazione. Verificare la correttezza del token Azure Active Directory (AAD). Il token AAD è valido per 60 minuti, dopo il quale sarà necessario rigenerare il token AAD.     |
|    Nome di tabella non valido     |    400     |    Il nome del set di dati non è corretto. Controllare nuovamente il nome del set di dati chiamando l'API "Get All Datasets".     |
|    Nome di colonna non corretto     |    400     |    Il nome della colonna nella query non è corretto. Controllare di nuovo il nome della colonna chiamando l'API "Get All Datasets" (Ottieni tutti i set di dati) o fare riferimento ai nomi di colonna nelle definizioni dei dati    |
|    Valore Null o mancante     |    400     |    È possibile che non siano presenti parametri obbligatori come parte del payload della richiesta dell'API.     |
|    Parametri del report non validi     |    400     |    Assicurarsi che i parametri del report siano corretti. Ad esempio, è possibile che venga fornito un valore minore di 4 per il parametro RecurrenceInterval.     |
|    L'intervallo di ricorrenza deve essere compreso tra 4 e 2160     |    400     |    Assicurarsi che il valore del parametro di richiesta RecurrenceInterval sia compreso tra 4 e 2160.     |
|    QueryId non valido     |    400     |    Controllare di nuovo l'oggetto QueryId generato.     |
|    Parametri del report non validi per la creazione: l'ora di inizio del report deve essere almeno 4 ore dall'ora UTC corrente     |    400     |    Il parametro Ora di inizio come parte del payload della richiesta non deve essere nel passato. L'ora di inizio del report deve essere di almeno 4 ore dall'ora UTC corrente.     |
|    Il valore richiesto 'string' non è stato trovato     |    400     |    Controllare se i parametri o il formato della `callbackurl` richiesta sono stati aggiornati.     |
|    Nessun elemento trovato con i filtri specifici.     |    404     |    Controllare il parametro reportID usato nell'API Get Report Executions .     |
|    Non sono state verificate esecuzioni per le condizioni di filtro specificate. Controllare il valore di reportId o executionId e ripetere l'API dopo il tempo di esecuzione pianificato del report     |    404     |    Assicurarsi che reportId sia corretto. Ripetere l'API dopo il tempo di esecuzione pianificato del report, come specificato nel payload della richiesta.     |
|    Errore interno durante la creazione del report. ID di correlazione <>     |    500     |    Assicurarsi che il formato della data per i campi *StartTime*, *QueryStartTime* e *QueryEndTime* sia corretto.     |
|    Servizio non disponibile    |    500     |    Se si riceve continuamente un servizio non disponibile (errore 5xx), aprire un ticket di supporto.    |
|        |        |        |

## <a name="no-records"></a>Nessun record

Si riceve la risposta API 200 quando si scarica il report dal percorso sicuro. Perché non si riceve alcun record?
Controllare se la stringa nella query include uno dei valori consentiti per l'intestazione di colonna. Ad esempio, questa query restituirà zero risultati:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

In questo esempio i valori consentiti per `IsDuplicateRowForPGA` sono 0 o 1. Fare riferimento alle [definizioni dei dati](insights-data-definitions.md) per tutti i valori possibili per le varie colonne.
