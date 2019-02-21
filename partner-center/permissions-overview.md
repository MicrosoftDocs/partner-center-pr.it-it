---
title: Assegnare ruoli agli utenti e le autorizzazioni | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Tutti i dipendenti che devono lavorare nel centro per i Partner devono essere assegnato un ruolo.
author: labrenne
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086729"
---
# <a name="assign-users-roles-and-permissions"></a>Assegnare autorizzazioni e ruoli utente


Aver configurare il profilo del partner, tra cui nome legale e indirizzo, i dettagli di supporto, le esenzioni fiscali, informazioni bancarie e il contatto principale per la tua azienda. Passaggio successivo: ottenere gli utenti configurato con ruoli e le password in modo che possono iniziare a lavorare con te nel centro per i Partner.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurare i dipendenti di lavorare nel centro per i Partner

Determinare i tipi di accesso che agli utenti dispongono Centro per i Partner per i ruoli e autorizzazioni che assegnare loro. Ruoli sono correlati per i programmi a cui che l'azienda è interessato. Ad esempio, se l'azienda è un'azienda Cloud Solution Provider (CSP), non solo è standard ad Azure AD tenant ruoli di gestione come amministratore globale, ma dovrà ruoli specifici per il programma CSP. Ciascun programma ha ruoli ad esso specifici.

>[!Note]
> Ruoli di tenant Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP. Ruoli di AAD di non includono amministratore MPN, amministratore del profilo di lavoro, amministratore dei riferimenti, amministratore di incentivi e utente degli incentivi. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gestire le transazioni commerciali nel centro per i Partner (Azure AD e ruoli CSP)

|**Ruolo**|**Operazioni consentite**|
|----------------------------------|:---------------------------------|
|Amministratore globale|• Possono accedere a tutti gli account/servizi Microsoft con privilegi completi
|      |• Creazione di ticket di supporto per il centro per i Partner
||• Visualizzazione di contratti, listini prezzi e offerte
||• Visualizzazione, creazione e gestione utenti partner|
|Amministratore utenti   | • Visualizzazione, creazione e gestione di utenti
||• Visualizzare tutti i profili dei partner
||• Visualizzazione, creazione e gestione utenti partner  |
|Utente predefinito|  Visualizza il mio profilo   |
|Agente amministratore | • Dei clienti
||• Aggiungere elenco dei dispositivi per il Center< per i Partner
||• Creare e applicare i profili ai dispositivi
||• Gestione delle sottoscrizioni
||• Servizio integrità e richieste di servizio per i clienti
||• Richiedere i privilegi di amministratore delegato
||• Visualizzazione prezzi e offerte
||• La fatturazione
||• Amministrazione per conto di un cliente
||• Registrazione un valore aggiunto come rivenditore|
|Agente di vendita | • Dei clienti
||• Aggiungere l'elenco dei dispositivi al centro per i Partner
||• Gestione delle sottoscrizioni
||• Visualizzazione ticket di supporto
||• Richiedi una relazione con un cliente
||• La gestione dei lead dei clienti
||• Visualizzazione contratto per il cliente
||• Registrare un rivenditore a valore aggiunto|
|Agente help desk| • La ricerca e visualizzazione di un cliente
||• Modificare i dettagli dei clienti
||• La Guida risolvere i problemi dei clienti con la gestione di fatturazioni o sottoscrizioni
||• Richiesta di supporto per conto dei clienti (Nota: È necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)
||• Gestire le sottoscrizioni e conto dei clienti (Nota: È necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Fornitore Pannello di controllo (CPV). (Ruolo CSP e non AAD)
CPVs sviluppare App per l'uso da parte dei partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con API del centro per i Partner. 

|**Ruolo**   |**Cosa puoi fare**|
|------------------------------|:----------------------------|
|Amministratore globale| Visualizzare e gestire il profilo CPV|
||Visualizzare e gestire uno qualsiasi degli utenti che necessitano dell'accesso a funzionalità CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Gestire l'appartenenza a MPN e la tua azienda (ruoli non AAD)

|**Ruolo** | **Cosa puoi fare**|
|----------------------------|:----------------------------|
|Amministratore MPN|•CAN aggiungere gli utenti non tenant
||• Visualizzazione, creazione e gestione delle richieste di servizio per i partner
||• Visualizzazione legali, l'organizzazione, le aziende e dei profili MPN
||• Visualizzare i dettagli utente e i relativi dati delle competenze
||• Visualizzazione delle competenze
||• Consente di visualizzare e gestire i vantaggi
||Acquisto e la visualizzazione • alle offerte MPN
||• Visualizzazione MPN fatture e cronologia degli ordini di offerte
||• Visualizzare i dati di contributo per i partner
||• Possono utilizzare lo strumento di convalida giustificativo|
|Account amministratore| • Aggiungere gli utenti non tenant
||• Aggiungere o eliminare i percorsi
||-Gestire i profili correlati agli account che sei amministratore 
||• Assegna ruoli per gli utenti nel tenant a ruoli non AAD 
||• Registrare posizioni in programmi

## <a name="manage-referrals-non-aad-roles"></a>Gestire i riferimenti (ruoli non AAD)

|**Ruolo**|**Cosa puoi fare**|
|-----------------------------|:------------------------|
|Amministratore dei riferimenti       |• Visualizzazione, creazione e gestione dei profili aziendali
||• Ricevere e gestivi segnalazioni
||• Visualizzazione, creazione e gestione delle richieste di servizio per i partner|
|Amministratore profilo di lavoro   |•View, creare e gestire profilo di lavoro 
||• Visualizzazione, creazione e gestione delle richieste di servizio per i partner|

## <a name="manage-incentives--non-aad-roles"></a>Gestire gli incentivi (ruoli non AAD)

|**Ruolo** | **Cosa puoi fare**|
|------------------------------|:-------------------------|
|Amministratore di incentivi|• Avvia e gestisce gli incentivi 
||• Può visualizzare e modificare tutti gli aspetti di programmi di incentivi
||• Può visualizzare e modificare i dettagli bancari e fiscali
||• Visualizzazione sconti e utili in collaborazione
||• Supporto per l'accesso
||Pagamenti di incentivi controversie •|
|Utente di incentivi|• Può visualizzare i programmi di incentivi
||• Può visualizzare e avviare attestazioni di incentivi
||• Visualizzazione sconti e utili in collaborazione
||• Visualizzazione sconti e utili in collaborazione
||• Supporto per l'accesso












