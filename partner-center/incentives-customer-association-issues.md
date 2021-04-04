---
title: Problemi di associazione dei clienti agli incentivi
description: Informazioni su come risolvere i problemi che si verificano quando si lavora con le associazioni clienti di CPOR (partner di record).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 30639725c0a852046251e83c3791f56d788931c1
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179212"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemi con le associazioni clienti di CPOR (partner di record) rivendicate

**Ruoli appropriati**

- Amministratore fatturazione
- Amministratore globale
- Amministratore degli incentivi

Il contenuto seguente consente di risolvere i problemi che possono verificarsi quando si lavora con le associazioni dei clienti.

## <a name="domain-tenant-mismatch"></a>Dominio-tenant non corrispondente

Nel flusso di attestazioni dell'associazione partner del record (CPOR) richiesto verrà richiesto di fornire l'ID del tenant e il sottodominio del cliente. Se viene visualizzato un messaggio di errore che informa che non corrispondono, contattare il cliente per assicurarsi di avere i dettagli corretti.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Errori di sottoscrizione nel flusso di attestazioni di associazione CPOR

Nel flusso di attestazioni di associazione CPOR, potrebbe essere richiesto di fornire una sottoscrizione per un prodotto che si sta tentando di rivendicare tramite Business Applications (Dynamics 365). Viene richiesta la sottoscrizione perché viene verificata in modo dinamico che il prodotto e la sottoscrizione appartengano al tenant richiesto per. Si sta anche verificando che la sottoscrizione sia attiva/in stato di tolleranza.

Se si riceve l'errore, è possibile che si verifichino diversi motivi:

- Il prodotto selezionato non esiste nel tenant del cliente
- La sottoscrizione specificata non è per Dynamics
- La sottoscrizione specificata è per CSP
- Il cliente non ha ancora attivato/effettuato il provisioning dei prodotti per tale sottoscrizione
- La sottoscrizione è già stata richiesta
- L'identificatore specificato non è un ID sottoscrizione

In caso di domande sull'accuratezza della sottoscrizione, collaborare con il cliente per assicurarsi che la sottoscrizione sia corretta e che si stia usando l'ID tenant corretto.

Se la route non ha risolto il problema, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Quando le sottoscrizioni saranno disponibili per l'attestazione

Quando si richiede una sottoscrizione, verrà visualizzato un errore se non è ancora stato eseguito il provisioning della sottoscrizione. Ci sono diversi passaggi che il cliente deve eseguire affinché la sottoscrizione diventi disponibile per la piattaforma CPOR e la renda disponibile per l'attestazione. Se si riceve un errore quando si prova a richiedere una sottoscrizione, contattare il cliente per assicurarsi che sia stato effettuato il provisioning e che la sottoscrizione che si sta reclamando sia corretta. Se questa route è già stata eseguita, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Quale attività è possibile scegliere?

La piattaforma di attestazione CPOR consente le attestazioni di associazione CPOR relative a Business Applications e Microsoft 365 aree della soluzione. Di seguito sono riportate le attività applicabili a ogni area della soluzione. Selezionare l'attività corretta in base alle descrizioni per evitare di dover recuperare in futuro. La richiesta di un'attività non corretta può comportare la mancata idoneità e i guadagni degli incentivi.


| Area soluzione | Attività | Applicabile per |
| ------ | ----------- | ----------- |
| Applicazioni aziendali      | Prevendite   | Selezionare se è stato influenzato l'acquisto di un prodotto idoneo e si desidera applicare gli incentivi per le vendite preliminari. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite il contratto multilicenza o il Web-Direct. |
|    |  Utilizzo  | Selezionare se si intende adottare l'adozione e l'utilizzo di un carico di lavoro idoneo e si desidera applicare gli incentivi per l'utilizzo. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite il contratto multilicenza o il Web-Direct. |
|    | Associazione dei ricavi   | Selezionare se è stato influenzato la selezione di un prodotto idoneo come influencer aziendale. Questa opzione è solo per l'associazione di ricavi, non per i pagamenti di incentivi. Questa opzione è applicabile solo se il cliente ha acquistato questi prodotti tramite il contratto multilicenza o il Web-Direct.   |
| Microsoft 365   | Utilizzo   | Selezionare se si intende adottare l'adozione e l'utilizzo di un carico di lavoro idoneo e si desidera applicare gli incentivi per l'utilizzo. |

## <a name="which-mpn-do-i-choose"></a>Quale MPN scegliere?

Nel flusso di attestazioni di associazione CPOR verrà richiesto di scegliere un MPN aziendale che deve essere associato al lavoro che si sta reclamando al cliente finale. L'azienda potrebbe avere molti MPNs, alcuni dei quali possono essere iscritti a programmi incentive e altri associati a un tipo di partner, ad esempio FRP FastTrack. Il flusso di attestazioni dell'associazione CPOR identifica i MPNs registrati in un programma di incentivazione, ma non indica se si tratta di un tipo di partner specifico MPN. È importante selezionare il MPN corretto, per evitare di dover recuperare in futuro. La richiesta di un MPN errato può comportare la mancata idoneità e i guadagni degli incentivi.

Se non si conosce il MPN da usare, contattare l'amministratore globale.

Se il MPN che si vuole usare non è registrato, è possibile gestirlo nella [scheda Panoramica incentivi](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (accesso richiesto).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Scelta di un prodotto rispetto all'immissione di una sottoscrizione

Quando un prodotto Dynamics viene richiesto e approvato, il partner può visualizzare l'ID sottoscrizione nell'attestazione di associazione CPOR stessa. Quando la sottoscrizione viene richiesta, è in stato attivo o in stato di tolleranza, ma è possibile che si verifichi un momento in cui la sottoscrizione termina e le nuove sottoscrizioni dovranno essere richieste in un'attestazione di associazione CPOR separata.

## <a name="competing-claims"></a>Attestazioni in competizione

Se si sta creando un'attestazione di associazione CPOR per un cliente e i relativi prodotti già associati a un altro partner, l'attestazione passerà attraverso l'arbitraggio:

1. Dopo aver creato una nuova associazione del cliente, Microsoft verificherà i dettagli dell'associazione e la prova di esecuzione indicata per garantirne l'accuratezza.

2. Se l'utente e un altro partner reclamano lo stesso cliente e prodotto/carico di lavoro, Microsoft esaminerà la documentazione di prova dell'esecuzione di ogni partner per determinare quale partner approverà.

3. È possibile che vengano richieste informazioni aggiuntive da entrambi i partner, che potrebbero causare ritardi nell'elaborazione della richiesta di associazione.

4. L'attestazione di associazione CPOR verrà comunque esaminata entro cinque giorni lavorativi, sebbene il relativo stato possa rimanere come sottoposto a _Verifica_ per un periodo di tempo più lungo. Questo scenario può verificarsi quando Microsoft collabora con il partner che attualmente possiede il prodotto o il carico di lavoro. In tal caso, si riceverà una notifica nella sezione dei commenti dell'attestazione. 

>[!IMPORTANT]
>Se sono necessarie ulteriori informazioni per verificare la CPOR Association Proof of Execution (PoE), si verrà contattati tramite la sezione CPOR Association Claim comments.

## <a name="next-steps"></a>Passaggi successivi

- [Introduzione agli incentivi](incentives-get-started-intro.md)
