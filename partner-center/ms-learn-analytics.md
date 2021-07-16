---
title: Partner Center Insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tenere traccia degli studenti dell'azienda sfruttando i dati su training individuale, moduli completati, percorsi di apprendimento completati e altro ancora.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d9f9ce631fe667030638e1a9167809e3dae69830
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373863"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Usare i Microsoft Learn di analisi dei dati

**Ruoli appropriati:** amministratore globale | Amministratore partner MPN

Il report [Microsoft Learn](/learn/) fornisce informazioni sugli studenti dell'azienda, inclusi i moduli completati e i percorsi di apprendimento in cui sono in esecuzione. Il report visualizza lo stato di ogni singolo apprendimento. Gli amministratori globali e gli amministratori MPN di un'azienda possono visualizzare i dati.

## <a name="how-to-read-the-report"></a>Come leggere il report

### <a name="summary-charts"></a>Grafici di riepilogo

Questi grafici riepilogano le tendenze cumulative mensili e di conteggio per i singoli utenti con training, i completamenti dei moduli e i percorsi di apprendimento.

**Numero di individui con training:** conteggio di tutti gli studenti distinti che hanno completato almeno un modulo durante l'intervallo di date selezionato 

**Mini grafico delle tendenze degli individui con training:** conteggio cumulativo mensile degli studenti attivi 

**Conteggio completamenti modulo:** numero di completamenti del modulo per gli studenti dell'azienda del partner durante l'intervallo di date selezionato.
Ad esempio, se "Modulo 1" viene completato da 15 persone e "Modulo 2" è stato completato dalle stesse 15 persone, il conteggio dei completamenti del modulo sarà 30. La data di completamento del modulo deve rientrare nell'intervallo di date selezionato.

**Grafico di tendenza dei completamenti dei moduli:** conteggio cumulativo mensile dei completamenti dei moduli 

**Learning di completamenti** del percorso: numero di Learning completamenti del percorso da parte degli studenti nell'azienda del partner durante l'intervallo di date selezionato.
Ad esempio, se Learning Path "Path 1" viene completato da 20 persone e il percorso Learning "path 2" è stato completato dalle stesse 20 persone, il conteggio di completamento del percorso Learning sarà 40. La Learning di completamento del percorso deve rientrare nell'intervallo di date selezionato.

**Learning mini grafico di** tendenza dei completamenti del percorso di apprendimento: conteggio cumulativo mensile dei completamenti del percorso di apprendimento 

### <a name="trained-individuals-monthly-trend"></a>Tendenza mensile degli individui con training

Questi dati sono la tendenza degli utenti dell'azienda che hanno completato un modulo per la prima volta nel mese. 

**L'asse X** è il mese per il filtro temporale selezionato. 

**L'asse Y** è il conteggio degli studenti attivi che hanno registrato (la prima volta il completamento di un modulo) durante tale mese. Questa operazione non è cumulativa.

### <a name="module-completions-monthly-trend"></a>Tendenza mensile dei completamenti dei moduli

Questi dati sono la tendenza dei moduli completati da tutti gli utenti dell'azienda durante tale mese. (non cumulativo) 

**L'asse X** è il mese per il filtro temporale selezionato. 

**L'asse Y** è il conteggio dei completamenti del modulo durante tale mese. Questa operazione non è cumulativa.

### <a name="learning-path-completions-monthly-trend"></a>Learning di completamento percorso mensile

Questi dati sono la tendenza dei percorsi di apprendimento completati dagli utenti dell'azienda durante tale mese. (non cumulativo) 

**L'asse X** è il mese per il filtro temporale selezionato. 

**L'asse Y** è il conteggio dei completamenti dei moduli in tale mese. Questa operazione non è cumulativa.

### <a name="learning-path-completion-tabs"></a>Learning di completamento del percorso

#### <a name="module-tab"></a>Scheda Modulo

Questa scheda include la suddivisione dei moduli completati nell'azienda in base ai primi cinque nomi dei moduli. il prodotto a cui è associato il modulo; e il ruolo utente pertinente al modulo.  

- Grafico ad anello dei completamenti dei moduli: suddivisione dei completamenti del modulo (conteggio visualizzato nella sezione di riepilogo) in base ai nomi dei moduli.

Il numero visualizzato al centro del grafico è il totale dei moduli completati

- Completamenti per ruolo: suddivisione dei completamenti del modulo in base al ruolo del modulo. Se un modulo è associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti del modulo.

Il numero visualizzato al centro del grafico è il numero di ruoli distinti per i completamenti del modulo. 

- Completamenti per prodotto: suddivisione dei completamenti del modulo in base al prodotto a cui è mappato il modulo. Se un modulo è associato a più prodotti, ognuno dei prodotti viene aggiunto al conteggio dei completamenti del modulo.    

Il numero visualizzato al centro del grafico è il numero di prodotti distinti per i completamenti del modulo.  

#### <a name="learning-path-tab"></a>Learning percorso

Questa scheda include una suddivisione dei percorsi di apprendimento completati nell'azienda in base ai primi cinque nomi dei moduli. il prodotto a cui è mappato il percorso di apprendimento; e il ruolo pertinente a questo percorso di apprendimento.  

- Learning grafico ad anello dei percorsi di completamento dei percorsi: suddivisione dei completamenti del percorso Learning(conteggio visualizzato nella sezione di riepilogo) in base al nome.

- Completamenti per ruolo: suddivisione dei completamenti dei percorsi di apprendimento in base al ruolo. Se un modulo è associato a più ruoli, ognuno dei ruoli viene aggiunto al conteggio dei completamenti del modulo.

- Completamenti per prodotto: suddivisione dei completamenti dei percorsi di apprendimento in base al prodotto a cui è mappato il percorso di apprendimento. Se un modulo è associato a più prodotti, ognuno dei prodotti viene aggiunto al conteggio dei completamenti del modulo.

### <a name="completions-by-learning-individuals"></a>Completamenti di singoli utenti

Vengono elencati gli utenti con training nell'azienda e i dettagli dei moduli e dei percorsi di apprendimento completati.

Microsoft Learn identifica gli studenti con un ID oggetto utente. Nella scheda **Moduli tutti** gli studenti vengono ordinati in base ai moduli completati. Vengono visualizzati con il nome Microsoft Learn, l'ID oggetto e il numero di moduli. È possibile eseguire ricerche usando il nome utente. 

Nella scheda **Learning** di apprendimento tutti gli studenti ordinati in base ai percorsi di apprendimento completati vengono visualizzati con il nome visualizzato, l'ID oggetto e il numero di moduli.

Per ottenere i dettagli di uno strumento di apprendimento usando l'ID oggetto utente: 

1. Accedere a [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) È necessario essere l'amministratore globale del tenant Azure AD aziendale.

2. Copiare l'ID oggetto utente [nell'area evidenziata](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Domande frequenti

1. Non è possibile visualizzare i dettagli di Learn dell'azienda.

   Questo report è disponibile per i partner che hanno un account in Partner Center. Se si è ancora Partner Membership Center, non sarà possibile visualizzare questo report.

2. Who dell'azienda può visualizzare questo report? 

   L'amministratore globale e l'amministratore MPN possono visualizzare il report.

3. Come è possibile assicurarsi che tutti gli utenti associano i propri account Microsoft Learn al proprio account Partner Center?

   *Dopo che* l'amministratore globale ha aggiunto un nuovo [utente,](/learn/) tale utente deve passare a Microsoft Learn per collegare l'account aziendale o l'account aziendale di Azure Active Directory (AD) al proprio account Learn. In questo modo la Insights Learning mostra i corsi e le competenze giuste.
   
   L'utente deve:
   
   1. Accedere [Microsoft Learn](/learn/).
   2. Selezionare l'immagine del profilo, quindi **selezionare Mio profilo**.
   3. Selezionare **Impostazioni**.
   4. In **Gestione account** aggiungere il proprio account aziendale in Account **collegati.**

4. È possibile visualizzare tutti gli utenti dell'azienda che a loro volta a Microsoft Learn con un account msa in questo report?

   Attualmente, il modo migliore per eseguire questa operazione è aggiungere questi utenti al tenant di Azure AD e quindi aggiungerli a Partner Center in modo che possano associare il proprio account Microsoft Learn tramite Mio profilo **in** Partner Center. 

   Per gli utenti che usano solo l'account msa per il training, nel prossimo futuro il team di Microsoft Learn consentirà loro di associare la posta elettronica aziendale al proprio profilo Microsoft Learn aziendale. 

## <a name="next-steps"></a>Passaggi successivi

Per altri report, vedere [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report nel dashboard Insights dati. [Altre informazioni](insights-download-reports.md) 
