---
title: Partner Center insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tenere traccia degli studenti dell'azienda sfruttando i dati su training individuale, moduli completati, percorsi di apprendimento completati e altro ancora.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152631"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Report di analisi di Microsoft Learn che mostra lo stato degli studenti nella società

**Ruoli appropriati:** amministratore globale | Amministratore partner MPN

Il report Microsoft Learn fornisce informazioni sugli studenti dell'azienda, inclusi i moduli completati e i percorsi di apprendimento in cui sono in esecuzione. Il report visualizza lo stato di ogni singolo apprendimento. L'amministratore globale e l'amministratore MPN dell'azienda possono visualizzare i dati.

## <a name="how-to-read-the-report"></a>Come leggere il report

### <a name="summary-charts"></a>Grafici di riepilogo

Questi grafici riepilogano le tendenze cumulative mensili e di conteggio per i singoli utenti con training, i completamenti dei moduli e i percorsi di apprendimento.


**Numero di individui con training:** conteggio di tutti gli studenti distinti che hanno completato almeno un modulo durante l'intervallo di date selezionato 

**Mini grafico delle tendenze degli individui con training:** conteggio cumulativo mensile degli studenti attivi 

**Conteggio completamenti modulo:** numero di completamenti del modulo per gli studenti dell'azienda del partner durante l'intervallo di date selezionato.
Ad esempio, se "Modulo 1" viene completato da 15 persone e il "Modulo 2" è stato completato dalle stesse 15 persone, il conteggio dei completamenti del modulo sarà 30. La data di completamento del modulo deve rientrare nell'intervallo di date selezionato.

**Grafico di tendenza dei completamenti dei moduli:** conteggio cumulativo mensile dei completamenti dei moduli 

**Conteggio dei completamenti del** percorso di apprendimento: numero di completamenti del percorso di apprendimento da parte degli studenti nell'azienda del partner durante l'intervallo di date selezionato.
Ad esempio, se il percorso di apprendimento "Percorso 1" viene completato da 20 persone e il percorso di apprendimento "percorso 2" è stato completato dalle stesse 20 persone, il conteggio di completamento del percorso di apprendimento sarà 40. La data di completamento del percorso di apprendimento deve rientrare nell'intervallo di date selezionato.

**Mini grafico delle tendenze dei completamenti dei** percorsi di apprendimento: conteggio cumulativo mensile dei completamenti del percorso di apprendimento 

### <a name="trained-individuals-monthly-trend"></a>Tendenza mensile degli individui con training

Questi dati sono la tendenza degli utenti dell'azienda che hanno completato un modulo per la prima volta in quel mese. 

**Asse X è** mese per il filtro temporale selezionato. 

**Asse Y è** il conteggio degli studenti attivi che hanno registrato (completamento della prima volta di un modulo) durante il mese. Questa operazione non è cumulativa.

### <a name="module-completions-monthly-trend"></a>Tendenza mensile dei completamenti dei moduli

Questi dati sono la tendenza dei moduli completati da tutti gli utenti dell'azienda durante tale mese. (non cumulativo) 

**Asse X è** mese per il filtro temporale selezionato. 

**Asse Y è** il conteggio dei completamenti del modulo durante tale mese. Questa operazione non è cumulativa.

### <a name="learning-path-completions-monthly-trend"></a>Tendenza mensile dei completamenti dei percorsi di apprendimento

Questi dati sono la tendenza dei percorsi di apprendimento completati dagli utenti dell'azienda durante tale mese. (non cumulativo) 

**Asse X è** mese per il filtro temporale selezionato. 

**Asse Y è** il conteggio dei completamenti del modulo in quel mese. Questa operazione non è cumulativa.

### <a name="learning-path-completion-tabs"></a>Schede di completamento del percorso di apprendimento 

**Scheda Modulo**

Questa scheda include la suddivisione dei moduli completati nell'azienda in base ai primi cinque nomi dei moduli. il prodotto a cui è associato il modulo; e il ruolo utente pertinente al modulo.  

- Grafico ad anello dei completamenti dei moduli: suddivisione dei completamenti del modulo (conteggio visualizzato nella sezione di riepilogo) in base ai nomi dei moduli.

Il numero visualizzato al centro del grafico è il totale dei moduli completati

- Completamenti per ruolo: suddivisione dei completamenti del modulo in base al ruolo del modulo. Se un modulo è associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti del modulo.

Il numero visualizzato al centro del grafico è il numero di ruoli distinti per i completamenti del modulo. 

- Completamenti per prodotto: suddivisione dei completamenti del modulo in base al prodotto a cui è mappato il modulo. Se un modulo è associato a più prodotti, ognuno dei prodotti viene aggiunto al conteggio dei completamenti del modulo.    

Il numero visualizzato al centro del grafico è il numero di prodotti distinti per i completamenti del modulo.  

**Scheda Percorso di apprendimento**   

Questa scheda include una suddivisione dei percorsi di apprendimento completati nell'azienda in base ai primi cinque nomi dei moduli. il prodotto a cui è mappato il percorso di apprendimento; e il ruolo pertinente a questo percorso di apprendimento.  

- Grafico ad anello dei completamenti dei percorsi di apprendimento: suddivisione dei completamenti del percorso di apprendimento (conteggio visualizzato nella sezione di riepilogo) in base al nome.

- Completamenti per ruolo*: suddivisione dei completamenti dei percorsi di apprendimento in base al ruolo. Se un modulo è associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti del modulo.

- Completamenti per prodotto: suddivisione dei completamenti dei percorsi di apprendimento in base al prodotto a cui è mappato il percorso di apprendimento. Se un modulo è associato a più prodotti, ognuno dei prodotti viene aggiunto al conteggio dei completamenti del modulo.

### <a name="completions-by-learning-individuals"></a>Completamenti di singoli utenti

Vengono elencati gli utenti con training nell'azienda e i dettagli dei moduli e dei percorsi di apprendimento completati.

Microsoft Learn identifica gli studenti con un ID oggetto utente. Nella scheda **Moduli tutti** gli studenti vengono ordinati in base ai moduli completati. Vengono visualizzati con il nome Microsoft Learn, l'ID oggetto e il numero di moduli. È possibile eseguire ricerche usando il nome utente. 

Nella scheda **Percorsi di apprendimento tutti** gli studenti ordinati in base ai percorsi di apprendimento completati vengono visualizzati con il nome visualizzato dello learner, l'ID oggetto e il numero di moduli.

Per ottenere i dettagli di uno strumento di apprendimento usando l'ID oggetto utente: 

1. Accedere a [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) È necessario essere l'amministratore globale del tenant Azure AD aziendale.

2. Copiare l'ID oggetto utente [nell'area evidenziata](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) in Graph Explorer. 

## <a name="faq"></a>Domande frequenti

1. Non è possibile visualizzare i dettagli dell'apprendimento dell'azienda.

Questo report è disponibile per i partner che hanno un account in Partner Center. Se si è ancora Partner Membership Center, non sarà possibile visualizzare questo report.

2.  Chi nell'azienda può visualizzare questo report? 

L'amministratore globale e l'amministratore MPN possono visualizzare il report.

3. Come è possibile assicurarsi che tutti gli utenti associano i propri account Microsoft Learn al proprio account Partner Center?

Dopo che l'amministratore globale ha aggiunto un nuovo utente, l'utente deve passare al Mio profilo **per** associare il proprio account Microsoft Learn account.

- Selezionare **l'icona Account** nell'angolo destro del dashboard e quindi selezionare **Mio profilo**. 

-  In **Apprendimento dell'utente** un utente sarà in grado di associare il proprio account Microsoft Learning e connettere il proprio account Microsoft a Partner University.

3. È possibile visualizzare tutti gli utenti dell'azienda che a loro volta a Microsoft Learn con un account msa in questo report?

Attualmente, il modo migliore per eseguire questa operazione è aggiungere questi utenti al tenant di Azure AD e quindi aggiungerli a Partner Center in modo che possano associare il proprio account Microsoft Learn tramite Mio profilo **in** Partner Center. 

Per gli utenti che usano solo l'account msa per il training, nel prossimo futuro il team di Microsoft Learn consentirà loro di associare il proprio indirizzo di posta elettronica aziendale al proprio profilo Microsoft Learn aziendale. 

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report del dashboard Informazioni dettagliate. [Altre informazioni](pci-download-reports.md) 