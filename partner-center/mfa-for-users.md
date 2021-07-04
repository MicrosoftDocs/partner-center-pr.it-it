---
title: Configurare gli utenti con l'autenticazione a più fattori
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come configurare i dipendenti con MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450807"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurare gli utenti con l'autenticazione a più fattori

**Ruoli appropriati:** Amministratore globale

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti nell'ecosistema agiscano e si assicurino che vengano adottate le protezioni di sicurezza appropriate. È consigliabile che tutti i partner abilitino l'autenticazione a più fattori (MFA) per gli utenti nel tenant partner. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Aggiungere l'autenticazione a più fattori per gli utenti

Per completare questa attività, è necessario essere l'amministratore globale della società.

È possibile abilitare l'autenticazione a più fattori per gli utenti con la massima facilità quando tali utenti vengono aggiunti al tenant di Azure AD.

1. Accedere al [portale di Azure](https://portal.azure.com) e quindi passare a **Gestione utenti**.
1. Selezionare **Multi-Factor Authentication**.
1. Selezionare l'utente che si vuole abilitare e quindi selezionare **Abilita**.

Verrà abilitata l'autenticazione a più fattori per l'utente. L'opzione Abilitato indica che all'utente verrà chiesto di impostare la verifica dell'autenticazione a più fattori al primo accesso. Successivamente, al momento dell'accesso, verrà chiesto di fornire un codice ricevuto tramite posta elettronica o SMS, a seconda dell'impostazione fornita.  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Specificare la modalità di verifica.":::

>[!NOTE]
>Per consentire agli utenti di usare l'autenticazione a più fattori, è possibile usare l'opzione **Applica** seguendo la stessa procedura illustrata in precedenza e selezionando **Applica**. Per altre informazioni, vedere [Abilitare Azure Multi-Factor Authentication per singolo utente per proteggere gli eventi di accesso](/azure/active-directory/authentication/howto-mfa-userstates). 

Lo stato iniziale di tutti gli utenti è  **Disabilitato**. Quando si registrano utenti in Azure Active Directory Multi-Factor Authentication, il relativo stato viene modificato in **Abilitato**. Quando gli utenti abilitati eseguono l'accesso e completano il processo di registrazione, il relativo stato viene modificato in  **Applicato**. 

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare ruoli e autorizzazioni agli utenti](permissions-overview.md)