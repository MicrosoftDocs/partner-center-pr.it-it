---
title: Analisi Microsoft Learn di partner Center Insights
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tieni traccia degli appresori della tua azienda sfruttando i dati relativi a training individuale, moduli completati, percorsi di apprendimento completati e altro ancora.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b9a0ea8c4eefee1a87b9ccd626b1f2864234521
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132316"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Report di analisi di Microsoft Learn che mostra lo stato degli studenti nella società

**Ruoli appropriati**

- Amministratore globale
- Amministratore dei partner MPN

Il report Microsoft Learn fornisce informazioni sugli appresori dell'azienda, inclusi i moduli completati e i percorsi di apprendimento in cui si trovano. Il report Visualizza lo stato di ogni singolo discente. L'amministratore globale e l'amministratore MPN per l'azienda possono visualizzare i dati.

## <a name="how-to-read-the-report"></a>Come leggere il report

### <a name="summary-charts"></a>Grafici di riepilogo

Questi grafici riepilogano i conteggi e le tendenze cumulative mensili per gli utenti con training, i completamenti dei moduli e i percorsi di apprendimento.


**Numero di utenti** sottoposti a training: numero di tutti gli autori distinti che hanno completato almeno un modulo durante l'intervallo di date selezionato 

**Grafico di tendenza dei singoli utenti con training**: conteggio cumulativo mensile rispetto al mese degli studenti attivi 

**Numero di completamenti dei moduli**: numero di completamenti dei moduli da parte degli studenti nella società del partner durante l'intervallo di date selezionato.
Ad esempio, se "modulo 1" viene completato da 15 utenti e il "modulo 2" è stato completato dalle stesse 15 persone, il conteggio dei completamenti dei moduli sarà 30. La data di completamento del modulo dovrebbe rientrare nell'intervallo di date selezionato.

**Grafico di tendenza dei completamenti del modulo**: conteggio cumulativo mensile rispetto al mese per i completamenti dei moduli 

**Conteggio completamenti percorso di apprendimento**: numero di completamenti percorsi di apprendimento da parte degli studenti nella società del partner durante l'intervallo di date selezionato.
Ad esempio, se il percorso di apprendimento "Path 1" viene completato da 20 utenti e il percorso di apprendimento "Path 2" è stato completato dalle stesse 20 persone, il conteggio di completamento del percorso di apprendimento sarà 40. La data di completamento del percorso di apprendimento deve rientrare nell'intervallo di date selezionato.

**Grafico di tendenza dei completamenti del percorso di apprendimento**: numero cumulativo di mese per mese dei completamenti dei percorsi di apprendimento 

### <a name="trained-individuals-monthly-trend"></a>Tendenza mensile dei singoli utenti sottoposti a training

Questi dati sono la tendenza degli utenti della società che hanno completato un modulo per la prima volta in quel mese. 

L' **asse X** è il mese per il filtro temporale selezionato. 

L' **asse Y** è il numero di Learner attivi che hanno registrato (il primo completamento di un modulo) durante il mese. Questa operazione non è cumulativa.

### <a name="module-completions-monthly-trend"></a>Tendenza mensile completamenti modulo

Questi dati sono la tendenza dei moduli completati da tutti gli utenti della società durante il mese. (non cumulativo) 

L' **asse X** è il mese per il filtro temporale selezionato. 

L' **asse Y** corrisponde al conteggio dei completamenti del modulo durante il mese. Questa operazione non è cumulativa.

### <a name="learning-path-completions-monthly-trend"></a>Tendenza mensile completamenti percorso di apprendimento

Questi dati sono la tendenza dei percorsi di apprendimento completati dagli utenti della società durante il mese. (non cumulativo) 

L' **asse X** è il mese per il filtro temporale selezionato. 

L' **asse Y** corrisponde al numero di completamenti dei moduli in quel mese. Questa operazione non è cumulativa.

### <a name="learning-path-completion-tabs"></a>Schede di completamento percorso di apprendimento 

**Scheda modulo**

Questa scheda include la suddivisione dei moduli completati nell'azienda dai primi cinque nomi di modulo; prodotto a cui è associato il modulo. e il ruolo utente pertinente per il modulo.  

- Grafico ad anello completamenti modulo: suddivisione dei completamenti dei moduli (conteggio visualizzato nella sezione di riepilogo) dai nomi dei moduli.

Il numero visualizzato al centro del grafico è il totale dei moduli completati

- Completamenti per ruolo: suddivisione dei completamenti del modulo in base al ruolo del modulo. Se un modulo è associato a più ruoli, ogni ruolo viene aggiunto al conteggio dei completamenti del modulo.

Il numero visualizzato al centro del grafico è il numero di ruoli distinti per i completamenti del modulo. 

- Completamenti per prodotto: suddivisione dei completamenti del modulo dal prodotto a cui è stato eseguito il mapping del modulo. Se un modulo è associato a più prodotti, ogni prodotto viene aggiunto al conteggio dei completamenti del modulo.    

Il numero visualizzato al centro del grafico è il numero di prodotti distinti per i completamenti dei moduli.  

**Scheda percorso di apprendimento**   

Questa scheda include una suddivisione dei percorsi di apprendimento completati nell'azienda dai primi cinque nomi di modulo; prodotto a cui è stato eseguito il mapping del percorso di apprendimento. e il ruolo pertinente per questo percorso di apprendimento.  

- Grafici ad anello completamenti dei percorsi di apprendimento: suddivisione dei completamenti del percorso di apprendimento (conteggio visualizzato nella sezione di riepilogo) in base al nome.

- Completamenti per ruolo *: suddivisione dei percorsi di apprendimento completati dal ruolo. Se un modulo è associato a più ruoli, ogni ruolo viene aggiunto al conteggio dei completamenti del modulo.

- Completamenti per prodotto: suddivisione dei percorsi di apprendimento completati dal prodotto a cui viene eseguito il mapping del percorso di apprendimento. Se un modulo è associato a più prodotti, ogni prodotto viene aggiunto al conteggio dei completamenti del modulo.

### <a name="completions-by-learning-individuals"></a>Completamenti per apprendimento di singoli utenti

Verranno elencati gli utenti con training nell'azienda e i dettagli relativi ai moduli e ai percorsi di apprendimento completati.

Microsoft Learn identifica gli Learner con un ID oggetto utente. Nella **scheda moduli** tutti gli learners sono ordinati in base ai moduli completati. Vengono visualizzati con il nome utente Microsoft Learn, l'ID oggetto e il numero di moduli. È possibile eseguire la ricerca usando username. 

Nella **scheda percorsi di apprendimento** tutti gli apprendimento ordinati per percorsi di apprendimento completati vengono visualizzati con il nome visualizzato, l'ID oggetto e il numero di moduli dello Learner.

Per ottenere i dettagli di un discente usando l'ID oggetto utente: 

1. Accedere a [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). È necessario essere l'amministratore globale del tenant Azure AD della società.

2. Copiare l'ID oggetto utente nell' [area evidenziata](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) in Graph Explorer. 

## <a name="faq"></a>Domande frequenti

1. Non riesco a visualizzare i dettagli di formazione della mia azienda.

Questo report è disponibile per i partner che hanno un account nel centro per i partner. Se si è ancora in centro di appartenenza ai partner, non sarà possibile visualizzare questo report.

2.  Chi nell'azienda può visualizzare questo report? 

L'amministratore globale e l'amministratore MPN possono visualizzare il report.

3. Come è possibile verificare che tutti gli utenti associno gli account di Microsoft Learn al proprio account del centro per i partner?

Dopo che l'amministratore globale ha aggiunto un nuovo utente, l'utente deve passare al proprio **profilo personale** per associare l'account Microsoft Learn.

- Selezionare l'icona dell' **account** nell'angolo destro del dashboard e quindi selezionare **profilo personale**. 

-  In base alla **formazione** , un utente potrà associare il proprio account Microsoft Learning e connettere il proprio account Microsoft all'Università partner.

3. È possibile visualizzare tutti gli utenti della società che accedono a Microsoft Learn con un account MSA in questo report?

Attualmente, il modo migliore per eseguire questa operazione consiste nell'aggiungere questi utenti al tenant di Azure AD e quindi aggiungerli al centro per i partner, in modo che possano associare il proprio account di Microsoft Learn tramite il **profilo personale** nel centro per i partner. 

Per gli utenti che usano solo il proprio account MSA per il training, nel prossimo futuro il team di Microsoft Learn consentirà di associare il proprio indirizzo di posta elettronica aziendale al proprio profilo di Microsoft Learn. 

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione download dei report nel dashboard di Insights. [Altre informazioni](pci-download-reports.md) 