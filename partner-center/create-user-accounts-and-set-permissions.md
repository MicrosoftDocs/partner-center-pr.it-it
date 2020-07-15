---
title: Creare account utente e assegnare ruoli
description: A ogni dipendente deve essere assegnato un ruolo per poter accedere al Centro per i partner. Scopri come creare gli account utente, assegnare ruoli e impostare le autorizzazioni.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
Keywords: ruoli, autorizzazioni, aggiungi utente, assegna ruolo, amministratore, agente,
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 9ec8e98f77d49e34b6747b0f580502e9df25a950
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265198"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a>Creare account utente e assegnare ruoli e autorizzazioni

**Ruoli appropriati**

- Amministratore degli account
- Amministratore globale
- Amministratore gestione utenti

Crea gli account utente per i dipendenti che hanno bisogno di accedere al Centro per i partner. Questa operazione deve essere eseguita dall'amministratore per la gestione degli utenti, dall'amministratore degli account o dall'amministratore globale. All'utente che esegue queste attività devono essere assegnati anche i ruoli di amministratore degli utenti o amministratore globale di Azure Active Directory (AAD). Per altre informazioni sui ruoli di AAD, vedi [Autorizzazioni dei ruoli di amministratore in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Aggiungere un nuovo utente

1. Dall'icona **Impostazioni** in alto a destra nel Centro per i partner seleziona **Gestione utenti**.

2. Selezionare **Aggiungi utente**.

3. Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.

4. Seleziona il tipo di agente e/o il tipo di amministratore da assegnare all'utente. L'accesso al Centro per i partner è basato sui ruoli, quindi è possibile assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche.  Se gli utenti vogliono l'assegnazione di un ruolo, possono trovare gli amministratori globali da contattare accedendo a **Gestione utenti** e filtrando in base all'amministratore globale.

5. Selezionare **Aggiungi** per creare l'account utente. Verificare i dettagli dell'utente nella pagina successiva.

> [!IMPORTANT]  
> Prendere nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina. Copiarle e inviarle al nuovo utente perché in seguito non sarà più possibile accedervi. 


L'utente dovrà accedere al Centro per i partner con il nome utente e la password temporanea. Quando l'utente accede al Centro per i partner per la prima volta, gli viene chiesto di modificare la password. 


### <a name="find-your-global-admin"></a>Trovare l'amministratore globale

A volte può essere necessario modificare il ruolo di un utente oppure un nuovo utente può desiderare un'assegnazione di ruolo specifica.  
Per trovare un amministratore globale che può apportare modifiche ai ruoli o assegnare ruoli a un nuovo utente, dall'**icona Impostazioni** in alto a destra nel Centro per i partner seleziona **Gestione utenti** e filtra in base all'amministratore globale. 


### <a name="new-global-admin"></a>Nuovo amministratore globale

Se l'amministratore globale lascia l'organizzazione ed è necessario che un altro utente ricopra questo ruolo, puoi inviare un ticket al team di Azure o di Office 365. Per informazioni su come eseguire questa operazione, seleziona una delle opzioni riportate di seguito.

[Nuovo amministratore globale per Azure](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Nuovo amministratore globale per Office 365](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>Assegnare ruoli utente

Per usare il Centro per i partner, devi avere un ruolo assegnato.  I ruoli includono attualmente i ruoli tenant di Azure Active Directory, i ruoli del programma Cloud Solution Provider (CSP) e i ruoli aziendali non AAD. Una singola azienda può avere bisogno di tutti questi ruoli.

>[!Important]
>Per accedere al Centro per i partner, i singoli utenti devono essere elencati nel tenant. Le assegnazioni di ruoli forniscono possibilità di accesso aggiuntive.


**I ruoli tenant di AAD includono**:
- Amministratore globale
- Amministratore utenti

**I ruoli CSP includono**:
- Agente amministratore
- Amministratore fatturazione
- Agente di vendita
- Agente di supporto tecnico

**Ruoli che gestiscono l'appartenenza a MPN e la società (non AAD)**
- Amministratore dei partner MPN
- Amministratore degli account
- Amministratore delle segnalazioni
- Amministratore del profilo di business
- Utente e amministratore degli incentivi

**Produttore del pannello di controllo è un ruolo CSP e non AAD**.
- Amministratore globale

L'**utente guest** deve essere incluso nel tenant AAD e può avere qualsiasi ruolo non AAD.

Per informazioni specifiche sui ruoli e sulle operazioni possibili con ciascun ruolo, vedi [Assegnare le autorizzazioni utente](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Associare l'account Microsoft Learn di un utente nel Centro per i partner

Per consentire di visualizzare i percorsi di formazione e apprendimento seguiti per l'acquisizione delle competenze, gli utenti devono associare il proprio ID MCP al corrispondente account del Centro per i partner. Come amministratore globale, quando aggiungi nuovi utenti ricorda loro di associare l'ID MCP al relativo account. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Come associare l'ID MCP all'account del Centro per i partner

1. Dal dashboard del Centro per i partner seleziona l'icona **Il tuo account** nell'angolo destro del dashboard e quindi **Profilo personale**.

2. In **Your learning** (La tua formazione) potrai associare il tuo account Microsoft Learning e connettere anche il tuo account Microsoft a Partner University.
