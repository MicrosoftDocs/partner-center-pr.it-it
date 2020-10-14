---
title: Creare account utente e assegnare ruoli
description: A ogni dipendente deve essere assegnato un ruolo per poter accedere al Centro per i partner. Scopri come creare gli account utente, assegnare ruoli e impostare le autorizzazioni.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006767"
---
# <a name="create-user-accounts"></a>Creare account utente  

**Ruoli appropriati**

- Amministratore degli account
- Amministratore globale
- Amministratore gestione utenti

Crea gli account utente per i dipendenti che hanno bisogno di accedere al Centro per i partner. Questa operazione deve essere eseguita dall'amministratore per la gestione degli utenti, dall'amministratore degli account o dall'amministratore globale. All'utente che esegue queste attività devono essere assegnati anche i ruoli di amministratore degli utenti o amministratore globale di Azure Active Directory (AAD). Per altre informazioni sui ruoli di AAD, vedi [Autorizzazioni dei ruoli di amministratore in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Aggiungere un nuovo utente

1. Dall'icona **Impostazioni** in alto a destra nel Centro per i partner selezionare **Impostazioni account** e quindi **Gestione utenti**.

2. Selezionare **Aggiungi utente**.

3. Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.

4. Seleziona il tipo di agente e/o il tipo di amministratore da assegnare all'utente. L'accesso al Centro per i partner è basato sui ruoli, quindi è possibile assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche.  Se gli utenti vogliono l'assegnazione di un ruolo, possono trovare gli amministratori globali da contattare accedendo a **Gestione utenti** e filtrando in base all'amministratore globale.

5. Selezionare **Aggiungi** per creare l'account utente. Verificare i dettagli dell'utente nella pagina successiva.

> [!IMPORTANT]  
> Prendere nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina. Copiarle e inviarle al nuovo utente perché in seguito non sarà più possibile accedervi. 

L'utente dovrà accedere al Centro per i partner con il nome utente e la password temporanea. Quando l'utente accede al Centro per i partner per la prima volta, gli viene chiesto di modificare la password.

## <a name="assign-user-roles"></a>Assegnare ruoli utente

Per usare il Centro per i partner, devi avere un ruolo assegnato.  I ruoli includono attualmente i ruoli tenant di Azure Active Directory, i ruoli del programma Cloud Solution Provider (CSP) e i ruoli aziendali non AAD. Una singola azienda può avere bisogno di tutti questi ruoli.

>[!Important]
>Per accedere al Centro per i partner, i singoli utenti devono essere elencati nel tenant. Le assegnazioni di ruoli forniscono possibilità di accesso aggiuntive.

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare ruoli utente e autorizzazioni per i dipendenti che devono usare il Centro per i partner](permissions-overview.md)
