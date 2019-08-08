---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 3/5/2019
description: A tutti i dipendenti che devono lavorare nel centro per i partner deve essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708861"
---
# <a name="assign-users-roles-and-permissions"></a>Assegnare autorizzazioni e ruoli utente


Il profilo partner è stato configurato, inclusi nome e indirizzo validi, informazioni di supporto, esenzioni fiscali per i file, informazioni bancarie e il contatto principale per l'azienda. Passaggio successivo: configurare gli utenti con password e ruoli in modo che possano iniziare a lavorare nel centro per i partner.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurare i dipendenti per lavorare nel centro per i partner

Si determinano i tipi di accesso che gli utenti devono avere al centro per i partner mediante i ruoli e le autorizzazioni che si forniscono. I ruoli sono correlati ai programmi interessati dall'azienda. Se, ad esempio, l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo i ruoli di gestione dei tenant di Azure AD standard, ad esempio l'amministratore globale, ma dovranno avere ruoli specifici per il programma CSP. Ogni programma dispone di ruoli specifici.

>[!Note]
> I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, amministratore utente e ruoli CSP. I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore del riferimento, l'amministratore di incentivi e l'utente di incentivi. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Gestire le transazioni commerciali nel centro per i partner (ruoli Azure AD e CSP)

|**Ruolo**|**Cosa è possibile fare**|
|----------------------------------|:---------------------------------|
|Amministratore globale|• Può accedere a tutti i account Microsoft/servizi con privilegi completi
|      |• Creare ticket di supporto per il centro per i partner
||• Visualizzare contratti, elenchi prezzi e offerte
||• Visualizzare, creare e gestire gli utenti partner|
||  Visualizzare, creare e gestire la fatturazione, le fatture e i file di ricognizione
|Amministratore gestione utenti   | • Visualizzare, creare e gestire gli utenti
||• Visualizza tutti i profili partner
||• Visualizzare, creare e gestire gli utenti partner  |
|Amministratore fatturazione | -Visualizzare, creare e gestire la fatturazione, le fatture e i file di ricognizione|
|Utente predefinito|  Visualizza profilo personale   |
|Agente amministratore | • Gestione clienti
||• Aggiungere un elenco di dispositivi al centro per i partner
||• Creare e applicare profili ai dispositivi
||• Gestione delle sottoscrizioni
||• Richieste di assistenza e integrità dei servizi per i clienti
||• Richiedere privilegi di amministratore delegato
||• Visualizza prezzi e offerte
||• Fatturazione
||• Amministrazione per conto di un cliente
||• Registrare un valore aggiunto rivenditore|
|Agente di vendita | • Gestione clienti
||• Aggiungere un elenco di dispositivi al centro per i partner
||• Gestione delle sottoscrizioni
||• Visualizza elenchi prezzi e offerte
||• Visualizzare i ticket di supporto
||• Richiedere una relazione con un cliente
||• Gestisci lead cliente
||• Visualizzare il contratto del cliente
||• Registrare un rivenditore con valore aggiunto|
|Agente help desk| • Cercare e visualizzare un cliente
||• Modificare i dettagli del cliente
||• Risolvere i problemi del cliente con la fatturazione o la gestione delle sottoscrizioni
||• Richiedere supporto per conto dei clienti (Nota: Per completare questa attività per le sottoscrizioni di Office 365, è necessario essere un agente di amministrazione
||• Gestire le sottoscrizioni e i problemi di fatturazione per conto dei clienti (Nota: Per completare questa attività per le sottoscrizioni di Office 365, è necessario essere un agente di amministrazione|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Pannello di controllo Fornitore (CPV). (Ruolo CSP e ruolo non AAD)
CPVs sviluppa le app per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con le API del centro per i partner. 

|**Ruolo**   |**Operazioni possibili**|
|------------------------------|:----------------------------|
|Amministratore globale| Visualizzare e gestire il profilo CPV|
||Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Utente Guest (deve essere aggiunto al tenant di AAD)

|**Utente Guest**   | **Ruoli**|
|---------------------------|:--------------------|
||Amministratore dei partner MPN|
||Amministratore degli account|
||Amministratore di incentivi|
||Amministratore profilo di lavoro|
||Amministratore riferimenti|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Gestire l'appartenenza a MPN e la società (ruoli non AAD: questi ruoli gestiscono l'azienda anziché il tenant)

|**Ruolo** | **Operazioni possibili**|
|----------------------------|:----------------------------|
|Amministratore dei partner MPN|• Visualizzare, creare e gestire le richieste di servizio partner||
||• Visualizzare profili legali, aziendali, aziendali e MPN
||• Visualizzare i dettagli dell'utente e i relativi dati di competenze
||• Visualizzare le competenze
||• Visualizzare e gestire i vantaggi
||• Visualizzare e acquistare offerte MPN
||• View MPN offre la cronologia degli ordini e le fatture
||• Visualizzare i dati degli indicatori di contributo partner
||• È possibile usare lo strumento di convalida del voucher|
||-Visualizzare analisi dei dati del cliente
|| Visualizza altri ruoli utente all'interno della società, ma non può assegnare ruoli
|Amministratore account| Aggiungi percorsi
|| Gestire i profili correlati agli account per i quali si è amministratori 
||• Assegnare i ruoli per gli utenti nel tenant ai ruoli non AAD 
||• Registrare i percorsi nei programmi


## <a name="manage-referrals"></a>Gestisci riferimenti 

|**Ruolo**|**Operazioni possibili**|
|-----------------------------|:------------------------|
|Amministratore riferimenti       |• Visualizzare, creare e gestire i profili di business
||• Ricevere e gestire i riferimenti
||• Visualizzare, creare e gestire i riferimenti di co-selling|
||• Visualizzare, creare e gestire le richieste di servizio partner
|Amministratore profilo di lavoro   |• Visualizzare, creare e gestire il profilo di business 
||• Visualizzare, creare e gestire le richieste di servizio partner|

## <a name="manage-incentives"></a>Gestisci incentivi 

|**Ruolo** | **Operazioni possibili**|
|------------------------------|:-------------------------|
|Amministratore di incentivi|• Avvia e gestisce gli incentivi 
||• Consente di visualizzare e modificare tutti gli aspetti dei programmi per gli incentivi
||• Consente di visualizzare e modificare le informazioni fiscali e bancarie
||• Visualizzare i guadagni di sconto e co-op
||• Supporto per l'accesso
||• Pagamenti di incentivi per controversie|
|Utente di incentivi|• Può visualizzare i programmi per gli incentivi
||• Può visualizzare e avviare attestazioni per gli incentivi
||• Visualizzare i guadagni di sconto e co-op
||• Supporto per l'accesso












