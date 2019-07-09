---
title: Learn Microsoft analitica | Centro per i partner
ms.topic: article
ms.date: 07/05/2019
description: Informazioni su come comprendere l'analitica di apprendimento
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622529"
---
# <a name="microsoft-learn-analytics-report"></a>Report di Microsoft Learn analitica

Il report di Microsoft Learn consente con informazioni sugli strumenti di apprendimento dell'azienda, inclusi i moduli che siano state completate e i percorsi di apprendimento che siano presenti. Il report visualizza lo stato di ogni singolo strumento di apprendimento. L'amministratore globale e l'amministratore MPN per l'azienda può visualizzare i dati.

## <a name="how-to-read-the-report"></a>Come leggere il report

### <a name="summary-charts"></a>Grafici di riepilogo

**Sottoposto a training individui conteggio**: Un conteggio di tutti gli strumenti di apprendimento distinti che hanno completato almeno uno dei moduli durante l'intervallo di date selezionato 

**Mini grafico di tendenza individui sottoposto a training**: Rispetto al conteggio cumulativo del mese degli strumenti di apprendimento attivo 

**Numero di completamenti modulo**: Conteggio del modulo i completamenti per l'apprendimento nella società partner durante l'intervallo di date selezionato.
Ad esempio, se "Modulo 1" è stato completato da 15 utenti e il "modulo 2" è stata completata dalle stesse 15 persone, il numero di completamenti modulo è 30. Data di completamento del modulo deve rientrare nell'intervallo di date selezionato.

**I completamenti di modulo mini grafico di tendenza**: Rispetto al conteggio cumulativo del mese i completamenti di modulo 

**Numero di completamenti di percorso di apprendimento**: Conteggio di Learning percorso i completamenti per l'apprendimento nella società partner durante l'intervallo di date selezionato.
Ad esempio, se il percorso di apprendimento "Percorso 1" è stato completato da 20 singoli e il percorso di apprendimento "percorso 2" è stata completata dalle stesse 20 persone, il conteggio di completamento del percorso di apprendimento è 40. Data di completamento del percorso di apprendimento deve rientrare nell'intervallo di date selezionato.

**Mini grafico di tendenza i completamenti di percorso di apprendimento**: Rispetto al conteggio cumulativo di mese di apprendimento i completamenti di percorso 

### <a name="trained-individuals-monthly-trend"></a>Tendenza mensile degli utenti sottoposti a training

**Asse x** è mese per il filtro temporale selezionato. 

**Asse y** è conteggio degli strumenti di apprendimento attivi che hanno eseguito la registrazione (primo completamento di un modulo) durante il mese. Questo non è cumulativo.

### <a name="module-completions-monthly-trend"></a>Tendenza mensile i completamenti di modulo

**Asse x** è mese per il filtro temporale selezionato. 

**Asse y** è conteggio dei completamenti modulo durante tale mese. Questo non è cumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Tendenza mensile completamenti percorso di apprendimento

**Asse x** è mese per il filtro temporale selezionato. 

**Asse y** è conteggio dei completamenti di modulo in quel mese. Questo non è cumulativo.

### <a name="learning-path-completion-tabs"></a>Le schede di completamento di percorso di apprendimento 

- Scheda modulo

**Grafico ad anello i completamenti modulo**: suddivisione dei completamenti di modulo (conteggio visualizzato nella sezione di riepilogo) per i nomi di modulo.

Numero visualizzato al centro del grafico è i totali moduli completati

**I completamenti dal ruolo**: suddivisione dei completamenti di modulo per il ruolo del modulo. Se un modulo viene associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti di modulo.

Numero visualizzato al centro del grafico ad anello è il numero di ruoli distinti per i completamenti di modulo. 

**I completamenti per prodotto**: suddivisione dei completamenti di modulo in base al prodotto il modulo viene eseguito il mapping a. Se un modulo viene associato a più prodotti, ciascuno dei prodotti viene aggiunto al conteggio dei completamenti di modulo.    

Numero visualizzato al centro del grafico ad anello è il numero di prodotti distinti per i completamenti di modulo.  

- Scheda percorso di apprendimento    

**Grafico ad anello i completamenti di percorsi di apprendimento**: suddivisione dei completamenti di percorsi di apprendimento (conteggio visualizzato nella sezione di riepilogo) in base al nome.

**I completamenti dal ruolo**: suddivisione di learning completamenti percorsi dal ruolo. Se un modulo viene associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti di modulo.

**I completamenti per prodotto**: suddivisione di learning completamenti di percorsi per il prodotto a cui viene eseguito il mapping di percorso di apprendimento. Se un modulo viene associato a più prodotti, ciascuno dei prodotti viene aggiunto al conteggio dei completamenti di modulo.

### <a name="completions-by-learning-individuals"></a>Completamenti per utenti singoli di apprendimento

Learn Microsoft consente di identificare gli strumenti di apprendimento con un ID oggetto utente. Sotto il **scheda moduli**, tutti gli strumenti di apprendimento vengono ordinati in base ai moduli completati. Vengono visualizzati con loro nome utente Learn Microsoft, ID di oggetto e numero di moduli. È possibile eseguire la ricerca usando nome utente.

Per ottenere i dettagli di uno strumento di apprendimento usando l'ID oggetto utente: 

1. Accedere al [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (È necessario essere amministratore globale del tenant di Azure AD della società).

2. Copiare l'ID oggetto utente per il [area evidenziata](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) in Esplora grafico. 

