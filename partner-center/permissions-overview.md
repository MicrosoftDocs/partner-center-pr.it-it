---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Tutti i dipendenti che hanno necessità di lavorare in Partner Center devono essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587744"
---
# <a name="assign-users-roles-and-permissions"></a>Assegnare autorizzazioni e ruoli utente


È stata configurare il profilo di partner inclusi ragione sociale e indirizzi, i dettagli sul supporto, esenzione di file, informazioni bancarie e il contatto principale per l'azienda. Passaggio successivo: gli utenti configurati con le password e i ruoli in modo che possano iniziare a lavorare nel centro per i Partner con l'utente.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurare i dipendenti di lavorare in Centro per i Partner

Determinare i tipi di accesso che al centro per i Partner gli utenti dispongono per i ruoli e autorizzazioni che finti. I ruoli sono correlati per le applicazioni che è interessata dalla propria azienda. Ad esempio, se l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo è il standard di Azure AD i ruoli di gestione, ad esempio amministratore globale del tenant, ma sarà necessario ruoli specifici per il programma CSP. Ogni programma svolge ruoli specifici a esso.

>[!Note]
> I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP. Ruoli AAD-non includono MPN amministratore, amministratore profilo business, amministrazione di referral, admin incentivi e incentivi utente. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gestire le transazioni commerciali nel centro per i Partner (Azure AD e i ruoli CSP)

|**Ruolo**|**Le operazioni possibili**|
|----------------------------------|:---------------------------------|
|Amministratore globale|• Possono accedere a tutti i Microsoft account/servizi con privilegi completi
|      |• Creare ticket di supporto per il centro per i Partner
||• Visualizzare gli accordi sui listini prezzi e offerte
||• Visualizzare, creare e gestire gli utenti partner|
|Amministratore utenti   | • Visualizzare, creare e gestire gli utenti
||• Visualizzare tutti i profili partner
||• Visualizzare, creare e gestire gli utenti partner  |
|Utente predefinito|  Visualizza profilo personale   |
|Agente amministratore | • Gestione con i clienti
||• Aggiungere l'elenco dei dispositivi al centro per i Partner <
||• Creare e applicare i profili nei dispositivi
||• Gestione delle sottoscrizioni
||• Servizio integrità e soddisfare richieste per i clienti
||• Richiesta delegati i privilegi di amministratore
||• Visualizza i prezzi e offerte
||• La fatturazione
||• Amministra per conto di un cliente
||• Registra un valore aggiunto rivenditore|
|Agente di vendita | • Gestione con i clienti
||• Aggiungere l'elenco dei dispositivi al centro per i Partner
||• Gestione delle sottoscrizioni
||Ticket di supporto di visualizzazione •
||• Richiesta una relazione con un cliente
||• Gestire i lead dei clienti
||• Visualizzare il contratto del cliente
||• Registro un rivenditore a valore aggiunto|
|Agente help desk| • Cercare e visualizzare un cliente
||• Modificare i dettagli cliente
||• Guida risolvere cliente i problemi con la gestione di fatturazione o alla sottoscrizione
||• Richiedere il supporto per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)
||• Gestire le sottoscrizioni e fatturazione problemi per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornitore del Pannello di controllo (CPV). (Non-AAD ruolo e ruolo CSP)
CPVs lo sviluppo di App per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con Partner Center API. 

|**Ruolo**   |**Operazioni possibili**|
|------------------------------|:----------------------------|
|Amministratore globale| Visualizzare e gestire il profilo CPV|
||Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Gestire l'appartenenza MPN e la propria azienda (ruoli non-AAD)

|**Ruolo** | **Operazioni possibili**|
|----------------------------|:----------------------------|
|Amministratore dei partner MPN|•CAN aggiungere gli utenti non tenant
||• Visualizzare, creare e gestire le richieste di servizio partner
||• Vista legale, l'organizzazione, business e i profili MPN
||• Visualizzare i dettagli di utente e i relativi dati di competenze
||• Visualizza competenze
||• Visualizzare e gestire i vantaggi
||Acquisto e la visualizzazione • ottenuta MPN
||• Visualizzare MPN offre le fatture e cronologia degli ordini
||• Visualizza dati contributi di partner
||• Possono utilizzare lo strumento di convalida Voucher|
||-Visualizzare analitica dei dati dei clienti
|Amministratore account| • È possibile aggiungere gli utenti non tenant
||• Aggiunta o eliminazione di percorsi
||-Gestire i profili relativi agli account di per che amministratore 
||• Assegnare ruoli per gli utenti nel tenant per i ruoli AAD non 
||• Percorsi nei programmi di registrazione

## <a name="manage-referrals-non-aad-roles"></a>Gestire i riferimenti (ruoli non-AAD)

|**Ruolo**|**Operazioni possibili**|
|-----------------------------|:------------------------|
|Amministratore dei riferimenti       |• Visualizzare, creare e gestire i profili di business
||• Ricevere e gestire i riferimenti
||• Visualizzare, creare e gestire le richieste di servizio partner|
|Amministratore profilo di lavoro   |• Visualizzare, creare e gestire il profilo di business 
||• Visualizzare, creare e gestire le richieste di servizio partner|

## <a name="manage-incentives--non-aad-roles"></a>Gestire gli incentivi (ruoli non-AAD)

|**Ruolo** | **Operazioni possibili**|
|------------------------------|:-------------------------|
|Amministratore di incentivi|• Avvia e gestisce gli incentivi 
||• È possibile visualizzare e modificare tutti gli aspetti dei programmi di incentivi
||• È possibile visualizzare e modificare i dettagli fiscali e bancarie
||Utili sugli sconti e cooperativa visualizzazione •
||• Supporto dell'accesso
||Pagamenti di incentivi controversia •|
|Utente di incentivi|• Consente di visualizzare i programmi di incentivi
||• È possibile visualizzare e avviare le attestazioni di incentivi
||Utili sugli sconti e cooperativa visualizzazione •
||Utili sugli sconti e cooperativa visualizzazione •
||• Supporto dell'accesso












