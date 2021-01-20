---
title: Configurare gli utenti con l'autenticazione a più fattori
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come impostare i dipendenti con l'autenticazione a più fattori
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182376"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurare gli utenti con l'autenticazione a più fattori

**Ruoli appropriati**

- Amministratore globale

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti nell'ecosistema agiscano e si assicurino che vengano adottate le protezioni di sicurezza appropriate. È consigliabile che tutti i partner abilitino l'autenticazione a più fattori (MFA) per gli utenti nel tenant partner. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Aggiungere l'autenticazione a più fattori per gli utenti

Per completare questa attività, è necessario essere l'amministratore globale della società.

È possibile abilitare l'autenticazione a più fattori per gli utenti con la massima facilità quando tali utenti vengono aggiunti al tenant di Azure AD.

1. Accedere al [portale di Azure](https://portal.azure.com) e quindi passare a **Gestione utenti**.
1. Selezionare **Multi-Factor Authentication**.
1. Selezionare l'utente che si vuole abilitare e quindi selezionare **Abilita**.

Verrà abilitata l'autenticazione a più fattori per l'utente. L'opzione Abilitato indica che all'utente verrà chiesto di impostare la verifica dell'autenticazione a più fattori al primo accesso. Successivamente, al momento dell'accesso, verrà chiesto di fornire un codice ricevuto tramite posta elettronica o SMS, a seconda dell'impostazione fornita.  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Specificare i dati per la verifica":::

>[!NOTE]
>Per consentire agli utenti di usare l'autenticazione a più fattori, è possibile usare l'opzione **Applica** seguendo la stessa procedura illustrata in precedenza e selezionando **Applica**. Per altre informazioni, vedere [Abilitare Azure Multi-Factor Authentication per singolo utente per proteggere gli eventi di accesso](/azure/active-directory/authentication/howto-mfa-userstates). 

Lo stato iniziale di tutti gli utenti è  **Disabilitato**. Quando gli utenti vengono registrati per Azure Multi-Factor Authentication per singolo utente, il relativo stato viene modificato in  **Abilitato**. Quando gli utenti abilitati eseguono l'accesso e completano il processo di registrazione, il relativo stato viene modificato in  **Applicato**. 

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare ruoli e autorizzazioni agli utenti](permissions-overview.md)