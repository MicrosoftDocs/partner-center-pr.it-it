---
title: Assegnare ruoli e autorizzazioni agli utenti
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri quali sono i ruoli più adatti per gli utenti della tua azienda che gestiscono transazioni commerciali, segnalazioni, incentivi o adesioni MPN nel Centro per i partner.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565084"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner

**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Amministratore partner MPN

Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda. Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurare i dipendenti in modo che possano lavorare nel Centro per i partner

Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici. I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda. Ad esempio, se l'azienda è un'azienda Cloud Solution Provider (CSP), non solo si avranno i ruoli di gestione tenant standard Azure Active Directory (Azure AD), ad esempio l'amministratore globale, ma saranno necessari ruoli specifici per il programma CSP. Ogni programma prevede ruoli specifici.

>[!Note]
> Azure AD ruoli del tenant includono amministratore globale, amministratore utenti e ruoli CSP. I ruoli non Azure AD sono i ruoli che non gestiscono il tenant e includono l'amministratore partner MPN (Microsoft Partner Network), l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente incentivo. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)

|**Ruolo**|**Operazioni consentite**|**Altre informazioni**|
|----------------------------------|---|:---------------------------------|
|Amministratore globale|*    Accesso a tutti gli account/servizi Microsoft con privilegi completi|[Gestire l'account per il Centro per i partner](partner-center-account-setup.md)
|      |*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati
||*    Visualizzazione di contratti, listini prezzi e offerte
||*    Visualizzazione, creazione e gestione di utenti partner|
||  Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione
|Amministratore gestione utenti   | *    Visualizzazione, creazione e gestione di utenti|[Gestire i vantaggi derivanti dall'appartenenza a Microsoft Partner Network nel Centro per i partner](manage-your-partner-network-benefits.md)
||*    Visualizzazione di tutti i profili dei partner
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati
|Amministratore fatturazione | - Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione|[Leggere la fattura](billing.md)
||*    Visualizzazione dei prezzi
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati
|Utente predefinito|  Visualizzazione del profilo personale   |[Reimpostare la password](reset-my-pasword.md)
|Agente amministratore | *    Gestione dei clienti|[Entrare in contatto con i clienti](connect-with-your-customers.md)
||*    Aggiunta dell'elenco dei dispositivi al Centro per i partner
||*    Creazione e applicazione di profili ai dispositivi
||*    Gestione degli abbonamenti
||*    Integrità del servizio e richieste di servizio per i clienti
||*    Richiesta dei privilegi di amministratore con delega
||*    Visualizzazione di prezzi e offerte
||*    Fatturazione
||*    Amministrazione per conto di un cliente
||*    Registrazione di un rivenditore a valore aggiunto
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati|
|Agente di vendita | *    Gestione dei clienti|[Fornire ai clienti supporto per la fatturazione e rispondere alle domande sulla fatturazione](provide-billing-support.md)
||*    Aggiunta dell'elenco dei dispositivi al Centro per i partner
||*    Gestione degli abbonamenti
||*    Visualizzazione dei ticket di supporto
||*    Richiesta di una relazione con un cliente
||*    Visualizzazione di prezzi e offerte
||*    Gestione dei clienti potenziali
||*    Visualizzazione del contratto per il cliente
||*    Registrazione di un rivenditore a valore aggiunto
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati|
|Agente di supporto tecnico| *    Ricerca e visualizzazione di un cliente|[Riassegnare i problemi a Microsoft e imparare a conoscere i problemi più adatti per la riassegnazione a Microsoft](escalate-problems-to-microsoft.md)
||*    Modifica dei dettagli dei clienti
||*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti
||*    Richiesta di supporto per conto dei clienti 
||*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Fornitore del pannello di controllo (CPV) (ruolo CSP e ruolo non Azure Active Directory)

I CSP sviluppano app per l'uso da parte dei partner CSP per consentire loro di integrare i propri sistemi con Partner Center API. 

|**Ruolo**   |**Operazioni consentite**|**Altre informazioni**|
|------------------------------|:----------------------------|----|
|Amministratore globale| Visualizzare e gestire il profilo Pannello di controllo vendor (CPV)|[Iscriversi come fornitore del pannello di controllo per integrare i sistemi di partner CSP con le API del Centro per i partner](enroll-as-cpv.md)
||Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Utente guest (deve essere aggiunto al tenant Azure AD)

|**Utente guest**   | **Ruoli**|
|---------------------------|:--------------------|
||Amministratore dei partner MPN|
||Amministratore del profilo di business|
||Amministratore delle segnalazioni|


## <a name="manage-mpn-membership-and-your-company"></a>Gestione dell'appartenenza a MPN e dell'azienda 

Questi ruoli non sono Azure AD ruoli. Questi ruoli gestiscono l'attività aziendale anziché il tenant.

|**Ruolo** | **Operazioni consentite**|**Altre informazioni**|
|----------------------------|:----------------------------|-----|
|Amministratore dei partner MPN|*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner|[Acquistare o rinnovare un abbonamento a Microsoft Action Pack oppure competenze Silver o Gold](mpn-get-action-pack.md)
||*    Visualizzazione di profili legali, aziendali, commerciali e MPN
||*    Visualizzazione dei dettagli dell'utente e dei relativi dati delle competenze
||*    Visualizzazione delle competenze
||*    Visualizzazione e gestione dei vantaggi
||*    Visualizzazione e acquisto di offerte MPN
||*    Visualizzazione di fatture e cronologia degli ordini di offerte MPN
||*    Visualizzazione dei dati degli indicatori di contributi dei partner
||*    Uso dello strumento di convalida dei giustificativi|
||*    Visualizzazione dell'analisi dei dati dei clienti
||*    Visualizzazione di altri ruoli utente all'interno dell'azienda, senza la possibilità di assegnare ruoli
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati
|Amministratore degli account| Aggiunta di posizioni|[Gestire le sedi](manage-locations.md)
|| Gestione di profili relativi agli account amministrati 
||* Assegnare ruoli per gli utenti nel tenant a ruoli non Azure-AD 
||*    Registrazione di posizioni nei programmi
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati

## <a name="manage-referrals"></a>Gestione delle segnalazioni

|**Ruolo** | **Operazioni consentite**|**Altre informazioni**
|------------------------------|:-------------------------|---|
|Amministratore delle segnalazioni|Attività di creazione e gestione nella scheda Segnalazioni del Centro per i partner|[Gestire le opportunità di co-selling](manage-co-sell-opportunities.md)
||    Visualizzazione e modifica di tutte le opportunità e tutti i lead di co-selling
||    Assegnazione di membri del team per una trattativa
||    Visualizzazione e modifica dei profili di business
||    Visualizzazione e registrazione delle trattative per le opportunità contrassegnate come vinte e idonee per la registrazione della trattativa
||    Creazione e visualizzazione dei ticket di supporto
|Utente delle segnalazioni|Creazione e gestione delle opportunità di co-selling solo se l'utente è membro del team |[Gestire le opportunità di co-selling](manage-co-sell-opportunities.md)
||    Creazione di opportunità di co-selling per le sedi in cui l'utente dispone del ruolo
||    Visualizzazione e registrazione delle trattative per le opportunità contrassegnate come vinte e idonee per la registrazione della trattativa se l'utente è membro del team
||    Creazione e visualizzazione dei ticket di supporto
|Amministratore del profilo di business|Creazione e gestione dei profili di business | [Gestire i profili di business](create-a-marketing-profile.md)
||    Creazione e visualizzazione dei ticket di supporto

Insieme al nuovo ruolo utente Segnalazioni, viene introdotto anche l'ambito della sede per le trattative. La tabella seguente illustra l'accesso alle trattative in base alla sede.

|**Scope** | **Operazioni consentite** |
|------------------------------|:-------------------------|
|Intera azienda | Sia gli amministratori che gli utenti possono accedere per creare trattative per qualsiasi sede dell'azienda|
|| L'amministratore delle segnalazioni può accedere per visualizzare e modificare tutte le trattative |
|| Gli utenti delle segnalazioni possono accedere per visualizzare e modificare tutte le trattative solo se sono membri del team |
|Una o più sedi | Sia gli amministratori che gli utenti possono accedere per creare trattative per la sede assegnata nell'azienda|
|| L'amministratore delle segnalazioni può accedere per visualizzare e modificare tutte le trattative appartenenti alle sedi assegnate|
|| Gli utenti delle segnalazioni possono accedere per visualizzare e modificare tutte le trattative appartenenti alle sedi assegnate se sono membri del team|

## <a name="manage-incentives"></a>Gestione degli incentivi

|**Ruolo** | **Operazioni consentite**|**Altre informazioni**
|------------------------------|:-------------------------|---|
|Amministratore degli incentivi|*    Avvio e gestione di incentivi |[Risorse utili per iniziare a usare gli incentivi](incentives-get-started-intro.md)
||*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi
||*    Visualizzazione e modifica dei dettagli bancari e fiscali
||*    Visualizzazione di sconti e utili in collaborazione
||*    Accesso al supporto
||*    Controversie sui pagamenti di incentivi|
|Utente di incentivi|*    Visualizzazione di programmi di incentivi
||*    Visualizzazione e avvio di attestazioni di incentivi
||*    Visualizzazione di sconti e utili in collaborazione
||*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione dei ticket di supporto per i partner creati

## <a name="view-partner-center-insights-data"></a>Visualizzare i dati di Insights del Centro per i partner

|**Ruolo** | **Operazioni consentite**|**Altre informazioni**|
|------------------------------|:-------------------------|---|
|Visualizzatore di report esecutivi|Accesso a tutti i set di dati di reporting, creazione di ticket di supporto per i partner, visualizzazione dei ticket di supporto per i partner creati|[Report del dashboard di panoramica disponibili in Insights del Centro per i partner](pci-overview-report.md)
|Visualizzatore di report|Accesso ai report di dati tranne quelli relativi ai ricavi e ai dati personali di clienti e dipendenti, creazione di ticket di supporto per i partner, visualizzazione dei ticket di supporto per i partner creati|

## <a name="next-steps"></a>Passaggi successivi

- [Creare account utente e assegnare ruoli e autorizzazioni](create-user-accounts-and-set-permissions.md)
- [Verificare le informazioni sull'account quando si effettua l'iscrizione a un nuovo programma del Centro per i partner](verification-responses.md)
