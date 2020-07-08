---
title: Assegnare ruoli e autorizzazioni agli utenti
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri quali sono i ruoli più adatti per gli utenti della tua azienda che gestiscono transazioni commerciali, segnalazioni, incentivi o adesioni MPN nel Centro per i partner.
author: hemas
ms.author: hemas
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f4ec3a1a14e6845f7b6079e286876d9bb1f3dd5
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948592"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Amministratore dei partner MPN

Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda. Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurare i dipendenti in modo che possano lavorare nel Centro per i partner

Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici. I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda. Ad esempio, se si tratta di un'azienda CSP (Cloud Solution Provider), non solo avrai i ruoli di gestione del tenant di Azure AD standard (tra cui il ruolo di amministratore globale), ma avrai bisogno anche di ruoli specifici del programma CSP. Ogni programma prevede ruoli specifici.

>[!Note]
> I ruoli relativi al tenant di Azure Active Directory (AAD) includono l'amministratore globale, l'amministratore utenti e i ruoli CSP. I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente di incentivi. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)

|**Ruolo**|**Operazioni consentite**|
|----------------------------------|:---------------------------------|
|Amministratore globale|*    Accesso a tutti gli account/servizi Microsoft con privilegi completi
|      |*    Creazione di ticket di supporto per il Centro per i partner
||*    Visualizzazione di contratti, listini prezzi e offerte
||*    Visualizzazione, creazione e gestione di utenti partner|
||  Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione
|Amministratore gestione utenti   | *    Visualizzazione, creazione e gestione di utenti
||*    Visualizzazione di tutti i profili dei partner
||*    Visualizzazione, creazione e gestione di utenti partner  |
|Amministratore fatturazione | - Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione|
|Utente predefinito|  Visualizzazione del profilo personale   |
|Agente amministratore | *    Gestione dei clienti
||*    Aggiunta dell'elenco dei dispositivi al Centro per i partner
||*    Creazione e applicazione di profili ai dispositivi
||*    Gestione degli abbonamenti
||*    Integrità del servizio e richieste di servizio per i clienti
||*    Richiesta dei privilegi di amministratore con delega
||*    Visualizzazione di prezzi e offerte
||*    Fatturazione
||*    Amministrazione per conto di un cliente
||*    Registrazione di un rivenditore a valore aggiunto|
|Agente di vendita | *    Gestione dei clienti
||*    Aggiunta dell'elenco dei dispositivi al Centro per i partner
||*    Gestione degli abbonamenti
||*    Visualizzazione dei ticket di supporto
||*    Richiesta di una relazione con un cliente
||*    Gestione dei clienti potenziali
||*    Visualizzazione del contratto per il cliente
||*    Registrazione di un rivenditore a valore aggiunto|
|Agente di supporto tecnico| *    Ricerca e visualizzazione di un cliente
||*    Modifica dei dettagli dei clienti
||*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti
||*    Richiesta di supporto per conto dei clienti 
||*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornitore del pannello di controllo (CPV) (ruolo CSP e ruolo non AAD)
I CPV sviluppano app destinate ai partner CSP (Cloud Solution Provider) affinché possano integrare i loro sistemi con le API del Centro per i partner. 

|**Ruolo**   |**Operazioni consentite**|
|------------------------------|:----------------------------|
|Amministratore globale| Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo|
||Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Utente guest (deve essere aggiunto al tenant di AAD)

|**Utente guest**   | **Ruoli**|
|---------------------------|:--------------------|
||Amministratore dei partner MPN|
||Amministratore degli account|
||Amministratore degli incentivi|
||Amministratore del profilo di business|
||Amministratore delle segnalazioni|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gestione dell'appartenenza a MPN e dell'azienda (ruoli non AAD: questi ruoli gestiscono l'attività dell'azienda anziché il tenant)

|**Ruolo** | **Operazioni consentite**|
|----------------------------|:----------------------------|
|Amministratore dei partner MPN|*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner||
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
|Amministratore degli account| Aggiunta di posizioni
|| Gestione di profili relativi agli account amministrati 
||*    Assegnazione di ruoli per gli utenti nel tenant a ruoli non AAD 
||*    Registrazione di posizioni nei programmi


## <a name="manage-referrals"></a>Gestione delle segnalazioni 

|**Ruolo**|**Operazioni consentite**|
|-----------------------------|:------------------------|
|Amministratore delle segnalazioni       |*    Visualizzazione, creazione e gestione dei profili di business
||*    Ricezione e gestione delle segnalazioni
||*    Visualizzazione, creazione e gestione delle segnalazioni di co-selling|
||*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner
|Amministratore del profilo di business   |*    Visualizzazione, creazione e gestione del profilo di business 
||*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner|

## <a name="manage-incentives"></a>Gestione degli incentivi 

|**Ruolo** | **Operazioni consentite**|
|------------------------------|:-------------------------|
|Amministratore degli incentivi|*    Avvio e gestione di incentivi 
||*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi
||*    Visualizzazione e modifica dei dettagli bancari e fiscali
||*    Visualizzazione di sconti e utili in collaborazione
||*    Accesso al supporto
||*    Controversie sui pagamenti di incentivi|
|Utente di incentivi|*    Visualizzazione di programmi di incentivi
||*    Visualizzazione e avvio di attestazioni di incentivi
||*    Visualizzazione di sconti e utili in collaborazione
||*    Accesso al supporto

## <a name="view-partner-center-insights-data"></a>Visualizzare i dati di Insights del Centro per i partner

|**Ruolo** | **Operazioni consentite**|
|------------------------------|:-------------------------|
|Visualizzatore di report esecutivi|Accedere a tutti i set di dati di reporting|
|Visualizzatore di report|Accedere ai report di dati, ad eccezione dei ricavi e dei dati personali di clienti e dipendenti|












                                    