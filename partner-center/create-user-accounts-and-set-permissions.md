---
title: Creare account utente e impostare le autorizzazioni | Centro partner
ms.topic: article
ms.date: 02/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come creare account utente e assegnare ruoli nel Centro per i partner per ciascun dipendente che necessita dell'accesso. Gli utenti con privilegi di amministratore diversi possono eseguire questa operazione.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.author: evansma
Keywords: ruoli, autorizzazioni, aggiungi utente, assegna ruolo, amministratore, agente,
ms.localizationpriority: high
ms.openlocfilehash: 6bbae5b8bcd2882c7ba32a8b660fc256dec4e49a
ms.sourcegitcommit: 717ef04f5c0040611af3ba9e5a324ab67e99ba14
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2020
ms.locfileid: "78240208"
---
# <a name="create-user-accounts-and-assign-permissions"></a>Creare account utente e assegnare autorizzazioni

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

> [!NOTE]  
>  Se l'amministratore globale ha lasciato l'organizzazione o ha assunto un altro ruolo ed è necessario aggiungere un nuovo amministratore globale, devi registrare una richiesta di servizio nel [portale MPN](https://partner.microsoft.com/support). Se il richiedente è in grado di fornire le informazioni di identità personale richieste e altre informazioni sull'organizzazione, l'agente del supporto può richiedere l'elevazione dei privilegi di un utente ad amministratore globale.

### <a name="find-your-global-admin"></a>Trovare l'amministratore globale

A volte può essere necessario modificare il ruolo di un utente oppure un nuovo utente può desiderare un'assegnazione di ruolo specifica.  
Per trovare un amministratore globale che può apportare modifiche ai ruoli o assegnare ruoli a un nuovo utente, dall'**icona Impostazioni** in alto a destra nel Centro per i partner seleziona **Gestione utenti** e filtra in base all'amministratore globale. 

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








