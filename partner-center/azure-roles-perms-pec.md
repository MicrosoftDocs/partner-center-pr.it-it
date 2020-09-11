---
title: Ruoli, autorizzazioni per il credito guadagnato dal partner
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui ruoli e sulle autorizzazioni per i partner per poter guadagnare i crediti guadagnati dal partner (PEC). Questi sono diversi dai ruoli per lavorare nel centro per i partner.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011741"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Ruoli e autorizzazioni idonei per ottenere il credito guadagnato dal partner

I ruoli seguenti sono mappati ai livelli di autorizzazione che determinano se un partner è idoneo per i crediti ottenuti dal partner.

>[!Important]
>Questi ruoli e autorizzazioni non sono uguali ai ruoli e alle autorizzazioni che un utente deve usare nel centro per i partner.

|**Ruolo**   |**Descrizione**   |**Idoneo per PEC**   |
|-----------------|:------------------|:--------------|
|Proprietario  |Si gestiscono tutti gli elementi, incluso l'accesso alle risorse.|Sì|
|Autore di contributi |Si gestiscono tutti gli elementi, ad eccezione della concessione dell'accesso alle risorse.|Sì|
|Reader|È possibile visualizzare tutti gli elementi, ma non apportare modifiche|No|
|ACRDelete|acr delete|Sì|
|ACRImageSigner|firmatario immagine acr|Sì|
|ACRPull|acr pull|Sì|
|AcrPush|acr push|Sì|
|AcrQuarantineReader|lettore di dati di quarantena acr|No|
|AcrQuarantineWriter| writer di dati di quarantena acr|Sì|
|Collaboratore servizio Gestione API|Può gestire il servizio e le API.|Sì|
|Ruolo operatore del servizio Gestione API|Può gestire il servizio ma non le API.|Sì|
|Ruolo lettura del servizio Gestione API|Consente l'accesso di sola lettura al servizio e alle API.|No|
|Collaboratore componente di Application Insights|Gestisce i componenti di Application Insights|Sì|
|Debugger di snapshot di Application Insights|Concede l'autorizzazione utente per visualizzare e scaricare gli snapshot di debug raccolti con Application Insights Snapshot Debugger. Si noti che queste autorizzazioni non sono incluse nei ruoli Proprietario e Collaboratore.|Sì|
Operatore processo di automazione | Consente di creare e gestire i processi tramite i runbook di Automazione. | Sì | 
Operatore di automazione | Gli operatori di automazione possono avviare, arrestare, sospendere e riprendere processi. | Sì | 
Operatore runbook di automazione | Consente di leggere le proprietà del runbook per permettere di creare processi del runbook. | Sì | 
Collaboratore per Avere | Può creare e gestire un cluster Avere vFXT. | Sì | 
Operatore di Avere | Usato dal cluster Avere vFXT per gestire il cluster | Sì | 
Proprietario dei dati di Hub eventi di Azure | Consente l'accesso completo alle risorse di Hub eventi di Azure. | Sì | 
Ricevitore dei dati di Hub eventi di Azure | Consente l'accesso per la ricezione alle risorse dell'Hub eventi di Azure. | Sì | 
Mittente dei dati di Hub eventi di Azure | Consente l'accesso per l'invio alle risorse dell'Hub eventi di Azure. | Sì | 
Ruolo di amministratore del cluster del servizio Azure Kubernetes | Elencare l'azione delle credenziali di amministratore del cluster. | Sì | 
Ruolo di utente del cluster del servizio Azure Kubernetes | Elencare l'azione delle credenziali di utente del cluster. | Sì | 
Lettore di dati per Mappe di Azure (anteprima) | Concede l'accesso per la lettura dei dati correlati alle mappe da un account Mappe di Azure. | No | 
Proprietario dei dati del bus di servizio di Azure | Consente l'accesso completo alle risorse del bus di servizio di Azure. | Sì | 
Ricevitore dei dati del bus di servizio di Azure | Consente l'accesso per la ricezione alle risorse del bus di servizio di Azure. | Sì | 
Mittente dei dati del bus di servizio di Azure | Consente l'accesso per l'invio alle risorse del bus di servizio di Azure. | Sì | 
Proprietario della registrazione di Azure Stack | Consente di gestire le registrazioni di Azure Stack. | Sì | 
Collaboratore di backup | Consente di gestire il servizio di backup, ma non di creare insiemi di credenziali e concedere l'accesso ad altri utenti | Sì | 
Operatore di backup | Consente di gestire i servizi di backup, ma non di rimuovere il backup, creare insiemi di credenziali e concedere l'accesso ad altri utenti. | Sì | 
Lettore di backup | Può visualizzare i servizi di backup, ma non può apportare modifiche. | No | 
Lettore per la fatturazione | Consente l'accesso in lettura ai dati di fatturazione. | No | 
Collaboratore BizTalk | Consente di gestire i servizi BizTalk, ma non di accedervi. | Sì | 
Accesso ai nodi di tipo membro della blockchain (anteprima) | Consente l'accesso ai nodi di tipo membro della blockchain | Sì | 
Collaboratore di progetto | Può gestire le definizioni di progetto, ma non assegnarle. | Sì | 
Operatore di progetto | Può assegnare i progetti pubblicati esistenti, ma non creare nuovi progetti. Nota: questa operazione funziona solo se l'assegnazione viene eseguita con un'identità gestita assegnata dall'utente. | Sì | 
Collaboratore endpoint rete CDN | Può gestire gli endpoint della rete CDN, ma non può concedere l'accesso ad altri utenti. | Sì | 
Lettore endpoint rete CDN | Può visualizzare gli endpoint della rete CDN, ma non può apportare modifiche. | No | 
Collaboratore profilo rete CDN | Può gestire i profili e i rispettivi endpoint della rete CDN, ma non può concedere l'accesso ad altri utenti. | Sì | 
Lettore profilo rete CDN | Può visualizzare i profili e i rispettivi endpoint della rete CDN, ma non può apportare modifiche. | No | 
Collaboratore reti virtuali classiche | Consente di gestire le reti classiche, ma non di accedervi. | Sì | 
Collaboratore account di archiviazione classico | Consente di gestire gli account di archiviazione classici, ma non di accedervi. | Sì | 
Ruolo del servizio dell'operatore della chiave dell'account di archiviazione classico | Gli operatori della chiave dell'account di archiviazione classico sono autorizzati a elencare e rigenerare le chiavi negli account di archiviazione classici | Sì | 
Collaboratore macchine virtuali classiche | Consente di gestire le macchine virtuali classiche, ma non di accedervi né di gestire la rete virtuale o l'account di archiviazione a cui sono connesse. | Sì | 
Collaboratore Servizi cognitivi | Consente di creare, leggere, aggiornare, eliminare e gestire le chiavi di Servizi cognitivi. | Sì | 
Ruolo con autorizzazioni di lettura per i dati di Servizi cognitivi (anteprima) | Consente di leggere i dati di Servizi cognitivi. | No | 
Utente Servizi cognitivi | Consente di leggere ed elencare le chiavi di Servizi cognitivi. | No | 
Ruolo Lettore dell'account Cosmos DB | Può leggere i dati degli account Azure Cosmos DB. Vedere Collaboratore account DocumentDB per la gestione degli account Azure Cosmos DB. | No | 
Operatore di Cosmos DB | Consente di gestire gli account Azure Cosmos DB, ma non di accedere ai dati contenuti negli stessi. Impedisce l'accesso a chiavi dell'account e stringhe di connessione. | Sì | 
CosmosBackupOperator | Può inviare una richiesta di ripristino per un database di Cosmos DB o un contenitore per un account | Sì | 
Collaboratore Gestione costi | Può visualizzare i costi e gestire la configurazione dei costi, ad esempio budget ed esportazioni | Sì | 
Lettore Gestione costi | Può visualizzare la configurazione e i dati dei costi, ad esempio budget ed esportazioni | No | 
Collaboratore Data Box | Consente di gestire tutto il servizio Data Box, ad eccezione della concessione dell'accesso ad altri utenti. | Sì | 
Lettore Data Box | Consente di gestire il servizio Data Box, ad eccezione della creazione di ordini, della modifica dei dettagli dell'ordine e della concessione dell'accesso ad altri utenti. | No | 
Collaboratore Data Factory | Consente di creare e gestire data factory, oltre alle risorse figlio in esse contenute. | Sì | 
Sviluppatore di Data Lake Analytics | Consente di inviare, monitorare e gestire i propri processi, ma non di creare o eliminare account Data Lake Analytics. | Sì | 
Pulizia dati | Può eliminare i dati di analisi | Sì | 
Utente DevTest Labs | Consente di connettere, avviare, riavviare e arrestare le macchine virtuali in Azure DevTest Labs. | Sì | 
Collaboratore zona DNS | Consente di gestire le zone DNS e i set di record in DNS di Azure, ma non di controllare chi è autorizzato ad accedervi. | Sì | 
Collaboratore account DocumentDB | È in grado di gestire account Azure Cosmos DB. Azure Cosmos DB era precedentemente noto come DocumentDB. | Sì | 
Collaboratore per sottoscrizioni di eventi di Griglia di eventi | Consente di gestire le operazioni di sottoscrizione di eventi EventGrid. | Sì | 
Ruolo con autorizzazioni di lettura per sottoscrizioni di eventi di Griglia di eventi | Consente di leggere le sottoscrizioni di eventi EventGrid. | No | 
Operatore di cluster HDInsight | Consente di leggere e modificare le configurazioni dei cluster HDInsight. | Sì | 
Collaboratore Servizi di dominio HDInsight | Può leggere, creare, modificare ed eliminare operazioni correlate ai Servizi di dominio necessarie per HDInsight Enterprise Security Package | Sì | 
Collaboratore account Intelligent Systems | Consente di gestire gli account Sistemi intelligenti, ma non di accedervi. | Sì | 
Collaboratore di Key Vault | Consente di gestire gli insiemi di credenziali delle chiavi, ma non di accedervi. | Sì | 
Lab Creator (Creatore di lab) | Consente di creare, gestire ed eliminare i lab gestiti con gli account di Azure Lab. | Sì | 
Collaboratore di Log Analytics | Il ruolo Collaboratore di Log Analytics può leggere tutti i dati di monitoraggio e modificare le impostazioni di monitoraggio. La modifica delle impostazioni di monitoraggio include l'aggiunta di estensioni delle VM alle VM, la lettura delle chiavi dell'account di archiviazione per potere configurare la raccolta di log dall'Archiviazione di Azure, la creazione e la configurazione degli account di Automazione, l'aggiunta di soluzioni e la configurazione di Diagnostica di Azure in tutte le risorse di Azure. | Sì | 
Lettore di Log Analytics | Il ruolo Lettore di Log Analytics può visualizzare ed eseguire ricerche in tutti i dati di monitoraggio e può visualizzare le impostazioni di monitoraggio, inclusa la visualizzazione della configurazione di Diagnostica di Azure in tutte le risorse di Azure. | No | 
Collaboratore alle app per la logica | Consente di gestire le app per la logica, ma non di modificarne l'accesso. | Sì | 
Operatore delle app per la logica | Consente di leggere, abilitare e disabilitare le app per la logica, ma non di modificarle o aggiornarle. | Sì | 
Ruolo di Operatore applicazione gestita | Consente di leggere ed eseguire azioni sulle risorse dell'applicazione gestita | Sì | 
Lettore applicazioni gestite | Consente di leggere le risorse in un accesso di app gestita e JIT richiesta. | No | 
Managed Identity Contributor (Collaboratore per identità gestita) | Crea, legge, aggiorna ed elimina l'identità assegnata all'utente | Sì | 
Managed Identity Operator (Operatore per identità gestita) | Legge e assegna l'identità assegnata all'utente | Sì | 
Collaboratore gruppo di gestione | Ruolo Collaboratore gruppo di gestione | Sì | 
Lettore gruppo di gestione | Ruolo Lettore gruppo di gestione | No | 
Collaboratore al monitoraggio | Può leggere tutti i dati del monitoraggio e modificare le impostazioni di monitoraggio. Vedere anche Introduzione a ruoli, autorizzazioni e sicurezza con il monitoraggio di Azure. | Sì | 
Autore delle metriche di monitoraggio | Abilitare la pubblicazione di metriche nelle risorse di Azure | Sì | 
Lettore di monitoraggio | Può leggere tutti i dati del monitoraggio (metriche, log e così via). Vedere anche Introduzione a ruoli, autorizzazioni e sicurezza con il monitoraggio di Azure. | No | 
Collaboratore di rete | Consente di gestire le reti, ma non di accedervi. | Sì | 
Collaboratore account New Relic APM | Consente di gestire gli account e le applicazioni di APR New Relic, ma non di accedervi. | Sì | 
Lettore e accesso ai dati | Consente di visualizzare tutti gli elementi ma non consente di eliminare o creare un account di archiviazione o una risorsa contenuta. Consente anche l'accesso in lettura/scrittura a tutti i dati contenuti in un account di archiviazione tramite l'accesso alle chiavi dell'account di archiviazione. | Sì | 
Collaboratore cache Redis | Consente di gestire le cache Redis, ma non di accedervi. | Sì | 
Collaboratore ai criteri delle risorse (anteprima) | (Anteprima) Utenti di cui sono state recuperate informazioni da EA, con diritti per la creazione/modifica di criteri delle risorse, la creazione di ticket di supporto e la lettura di risorse/gerarchia. | Sì | 
Collaboratore raccolte di processi dell'unità di pianificazione | Consente di gestire le raccolte di processi dell'utilità di pianificazione, ma non di accedervi. | Sì | 
Collaboratore servizi di ricerca | Consente di gestire i servizi di Ricerca, ma non di accedervi. | Sì | 
Amministrazione della protezione | Solo in Centro sicurezza: è possibile visualizzare i criteri di sicurezza e gli stati di sicurezza, modificare i criteri di sicurezza, visualizzare gli avvisi e le raccomandazioni, ignorare gli avvisi e le raccomandazioni | Sì | 
Gestore sicurezza (legacy) | Questo è un ruolo legacy. Usare invece Amministratore della protezione | Sì | 
Ruolo con autorizzazioni di lettura per la sicurezza | Solo in Centro sicurezza: è possibile visualizzare raccomandazioni, avvisi, criteri di sicurezza e stati di sicurezza, ma non è possibile apportare modifiche | No | 
Collaboratore al ripristino sito | Consente di gestire il servizio Site Recovery ad eccezione della creazione dell'insieme di credenziali e dell'assegnazione di ruolo. | Sì | 
Operatore del ripristino sito | Consente di eseguire il failover e il failback ma non di eseguire altre operazioni di gestione di Site Recovery. | Sì | 
Reader di ripristino sito | Consente di visualizzare lo stato di Site Recovery ma non di eseguire altre operazioni di gestione. | No | 
Collaboratore per l'account per gli ancoraggi spaziali | Consente di gestire gli ancoraggi nello spazio nell'account, ma non di eliminarli | Sì | 
Proprietario dell'account per gli ancoraggi spaziali | Consente di gestire gli ancoraggi nello spazio nell'account, incluse le operazioni di eliminazione | Sì | 
Ruolo Lettore dell'account per gli ancoraggi spaziali | Consente di individuare e leggere le proprietà degli ancoraggi nello spazio nell'account | No | 
Collaboratore database SQL | Consente di gestire i database SQL, ma non di accedervi né di gestirne i criteri relativi alla sicurezza o i rispettivi server SQL padre. | Sì | 
Collaboratore per Istanza gestita di SQL | Consente di gestire le istanze gestite di SQL e la configurazione di rete richiesta, ma non di concedere l'accesso ad altri utenti. | Sì | 
Gestione della sicurezza SQL | Consente di gestire i criteri relativi alla sicurezza di server e database SQL, ma non di accedervi. | Sì | 
Collaboratore SQL Server | Consente di gestire i server e i database SQL, ma non di accedervi né di gestirne i criteri relativi alla sicurezza. | Sì | 
Collaboratore account di archiviazione | Consente di gestire gli account di archiviazione. Consente di accedere alla chiave dell'account, che può essere usata per accedere ai dati usando l'autorizzazione con chiave condivisa. | Sì | 
Ruolo del servizio dell'operatore della chiave dell'account di archiviazione | Consente di elencare e rigenerare le chiavi di accesso dell'account di archiviazione. | Sì | 
Collaboratore ai dati del BLOB di archiviazione | Consente di leggere, scrivere ed eliminare i contenitori e i BLOB di archiviazione di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | Sì | 
Proprietario dei dati del BLOB di archiviazione | Concede l'accesso completo ai contenitori e ai dati dei BLOB di Archiviazione di Azure, inclusa l'assegnazione del controllo di accesso POSIX. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | Sì | 
Lettore dei dati del BLOB di archiviazione | Consente di leggere ed elencare i contenitori e i BLOB di archiviazione di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | No | 
Delegante di BLOB di archiviazione | Ottiene una chiave di delega utente, che può quindi essere usata per creare una firma di accesso condiviso per un contenitore o un BLOB firmato con credenziali di Azure AD. Per altre informazioni, vedere Creare una firma di accesso condiviso di delega utente. | Sì | 
Collaboratore per la condivisione SMB di dati per file di archiviazione | Consente l'accesso in lettura, scrittura ed eliminazione nelle condivisioni file di archiviazione di Azure tramite SMB | Sì | 
Collaboratore con privilegi elevati per la condivisione SMB di dati per file di archiviazione | Consente l'accesso in lettura, scrittura, eliminazione e modifica delle autorizzazioni NTFS nelle condivisioni file di archiviazione di Azure tramite SMB | Sì | 
Ruolo con autorizzazioni di lettura per la condivisione SMB di dati per file di archiviazione | Consente l'accesso in lettura alla condivisione file di Azure tramite SMB | No | 
Collaboratore ai dati della coda di archiviazione | Lettura, scrittura ed eliminazione delle code e dei messaggi delle code di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | Sì | 
Ruolo con autorizzazioni di elaborazione per i messaggi sui dati della coda di archiviazione | Visualizzazione in anteprima, recupero ed eliminazione di un messaggio da una coda di Archiviazione di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | Sì | 
Mittente dei messaggi sui dati della coda di archiviazione | Consente di aggiungere messaggi a una coda di Archiviazione di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | Sì | 
Ruolo con autorizzazioni di lettura per i dati della coda di archiviazione | Consente di leggere ed elencare le code e i messaggi delle code di Azure. Per informazioni sulle azioni necessarie per una determinata operazione sui dati, vedere le autorizzazioni per la chiamata di operazioni sui dati BLOB e della coda. | No | 
Collaboratore alla richiesta di supporto | Consente di creare e gestire le richieste di supporto. | Sì | 
Collaboratore Gestione traffico | Consente di gestire i profili di Gestione traffico, ma non di controllare chi è autorizzato ad accedervi. | Sì | 
Amministratore accessi utente | Consente di gestire gli accessi utente alle risorse di Azure. | Sì | 
Virtual Machine Administrator Login (Accesso amministratore macchina virtuale) | Consente di visualizzare le macchine virtuali nel portale e di accedere come amministratore | Sì | 
Collaboratore macchine virtuali | Consente di gestire le macchine virtuali, ma non di accedervi né di gestire la rete virtuale o l'account di archiviazione a cui sono connesse. | Sì | 
Virtual Machine User Login (Accesso utente macchina virtuale) | Consente di visualizzare le macchine virtuali nel portale e di accedere come utente normale. | Sì | 
Collaboratore piani Web | Consente di gestire i piani Web per i siti Web, ma non di accedervi. | Sì | 
Collaboratore siti Web | Consente di gestire i siti Web (non i piani Web), ma non di accedervi | Sì |
