---
title: Problemi di associazione dei clienti agli incentivi
description: Informazioni su come risolvere i problemi che si verificano quando si lavora con le associazioni Partner of Record richieste (CPOR).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152172"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemi relativi alle associazioni Partner of Record richieste di assistenza (CPOR)

**Ruoli appropriati:** Amministratore fatturazione | Amministratore globale | Amministratore incentivi

Il contenuto seguente consente di risolvere i problemi che possono verificarsi quando si lavora con le associazioni dei clienti.

## <a name="domain-tenant-mismatch"></a>Mancata corrispondenza tra tenant di dominio

Nel flusso di richiesta di Partner of Record richiesta di associazione (CPOR) verrà richiesto di specificare l'ID tenant del cliente e il sottodominio. Se viene visualizzato un errore che indica che non corrispondono, contattare il cliente per assicurarsi di avere i dettagli corretti.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Errori di sottoscrizione nel flusso di attestazioni di associazione CPOR

Nel flusso di richiesta di associazione CPOR potrebbe essere richiesto di fornire una sottoscrizione per un prodotto che si sta tentando di richiedere tramite Business Applications (Dynamics 365). La sottoscrizione viene richiesta perché viene verificata in modo dinamico che il prodotto e la sottoscrizione appartengano al tenant richiesto. Viene anche verificato che lo stato della sottoscrizione sia attivo/in stato di tolleranza.

Se viene visualizzato l'errore, l'errore potrebbe essere per diversi motivi:

- Il prodotto selezionato non esiste nel tenant del cliente
- La sottoscrizione fornita non è per Dynamics
- La sottoscrizione specificata è per CSP
- Il cliente non ha ancora attivato/effettuato il provisioning dei prodotti per la sottoscrizione
- La sottoscrizione è già stata richiesta
- L'identificatore specificato non è un ID sottoscrizione

In caso di domande sull'accuratezza della sottoscrizione, collaborare con il cliente per assicurarsi che la sottoscrizione sia corretta e che si sta usando l'ID tenant corretto.

Se la route non ha risolto il problema, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Quando le sottoscrizioni saranno disponibili per l'attestazione

Quando si effettua la richiesta di una sottoscrizione, si riceverà un errore se non è ancora stato effettuato il provisioning della sottoscrizione. Il cliente deve eseguire diversi passaggi perché la sottoscrizione diventi disponibile per la piattaforma CPOR per prelevarla e renderla disponibile per l'attestazione. Se si riceve un errore durante il tentativo di richiedere una sottoscrizione, contattare il cliente per assicurarsi che sia stato effettuato il provisioning e che la sottoscrizione richiesta sia corretta. Se questa route è già stata intrapresa, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Quale attività è possibile scegliere?

La piattaforma di attestazione CPOR consente le attestazioni di associazione CPOR correlate alle Business Applications e Microsoft 365 soluzioni. Le attività applicabili a ogni area della soluzione sono riportate di seguito. Selezionare l'attività corretta in base alle descrizioni per evitare di dover recuperare in futuro. La richiesta di un'attività non corretta può comportare mancati requisiti di idoneità e incentivi.


| Area soluzione | Attività | Applicabile per |
| ------ | ----------- | ----------- |
| Applicazioni aziendali      | Prevendita   | Selezionare se è stato influenzato l'acquisto di un prodotto idoneo e si vuole richiedere incentivi per la pre-vendita. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite contratto multilicenza o Web-Direct. |
|    |  Utilizzo  | Selezionare questa opzione se si intende adottare e usare un carico di lavoro idoneo e si vuole applicare gli incentivi per l'utilizzo. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite contratto multilicenza o Web-Direct. |
|    | Associazione di ricavi   | Selezionare se è stata influenzata la selezione di un prodotto idoneo come Fattori di influenza aziendale. Questa opzione è valida solo per l'associazione di ricavi, non per i pagamenti di incentivi. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite contratto multilicenza o Web-Direct.   |
| Microsoft 365   | Utilizzo   | Selezionare questa opzione se si intende adottare e usare un carico di lavoro idoneo e si vuole applicare gli incentivi per l'utilizzo. |

## <a name="which-mpn-do-i-choose"></a>Quale MPN si sceglie?

Nel flusso di attestazione dell'associazione CPOR verrà chiesto di scegliere un MPN aziendale che deve essere associato al lavoro per il cliente finale. L'azienda può avere molte reti MPN, alcune delle quali possono essere registrate in programmi di incentivi e altre associate a un tipo di partner, ad esempio FRP FastTrack. Il flusso di richiesta di associazione CPOR identificherà quali MPN sono registrate in un programma di incentivi, ma non ti dirà se si tratta di un tipo di partner specifico MPN. È importante selezionare il mpn corretto, per evitare di dover recuperare in futuro. La richiesta di un MPN non corretto può comportare la mancata idoneità e gli utili di incentivi.

Se non si sa quale MPN usare, contattare l'amministratore globale.

Se il file MPN che si vuole usare non è registrato, è possibile gestirvi nella scheda [Panoramica](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) degli incentivi (è necessario l'accesso).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Scelta di un prodotto o immissione di una sottoscrizione

Quando un prodotto Dynamics viene richiesto e approvato, il partner può visualizzare l'ID sottoscrizione nell'attestazione di associazione CPOR stessa. Quando questa sottoscrizione viene richiesta, è attiva o in stato di tolleranza, ma potrebbe esserci un momento in cui la sottoscrizione termina e le nuove sottoscrizioni dovranno essere dichiarate in un'attestazione di associazione CPOR separata.

## <a name="competing-claims"></a>Attestazioni concorrenti

Se si sta creando una richiesta di associazione CPOR per un cliente e i relativi prodotti già associati a un altro partner, la richiesta verrà arbitrata:

1. Dopo aver creato una nuova associazione del cliente, Microsoft verificherà i dettagli dell'associazione e la prova di esecuzione indicata per garantirne l'accuratezza.

2. Se l'utente e un altro partner dichiarano lo stesso cliente e lo stesso prodotto/carico di lavoro, Microsoft esamina la documentazione della prova di esecuzione di ogni partner per determinare quale partner approvare.

3. Potrebbero essere richieste informazioni aggiuntive a entrambi i partner, che potrebbero causare ritardi nell'elaborazione della richiesta di associazione.

4. L'attestazione di associazione CPOR verrà comunque esaminata entro cinque giorni lavorativi, anche se il suo stato può rimanere In revisione _per_ un periodo di tempo più lungo. Questo scenario può verificarsi quando Microsoft collabora con il partner attualmente proprietario del prodotto o del carico di lavoro. In tal caso, si riceverà una notifica nella sezione dei commenti dell'attestazione. 

>[!IMPORTANT]
>Se sono necessarie informazioni aggiuntive per verificare la prova di esecuzione (PoE) dell'associazione CPOR, l'utente verrà contattato tramite la sezione commenti sulle attestazioni di associazione CPOR.

## <a name="next-steps"></a>Passaggi successivi

- [Introduzione agli incentivi](incentives-get-started-intro.md)
