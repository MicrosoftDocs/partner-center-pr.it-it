---
title: Risolvere i problemi di configurazione dell'account del centro per i partner o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi relativi alla registrazione nel centro per i partner
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848935"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Risolvere i problemi di configurazione dell'account o di rinnovo MPN

### <a name="applies-to"></a>Si applica a

- Centro per i partner
 
### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore globale
- Amministratore dei partner MPN 
 

Ecco alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell'account del centro per i partner.

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Cosa accade se si esegue la migrazione da partner Membership Center e non è possibile modificare i campi di informazioni aziendali

Questa situazione si verifica nei casi in cui la società dispone già di una presenza nel centro per i partner (ad esempio, l'account CSP). verrà visualizzata una schermata di sola lettura in cui verranno visualizzate tutte le informazioni sull'azienda così come esistono nel centro per i partner.

Non è possibile modificare i dettagli in questa schermata. Si tratta di un errore di progettazione.

Selezionare **Accetto** e **continuare** per procedere.

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Si sta tentando di eseguire la registrazione o di eseguire la migrazione da partner Membership Center e viene visualizzato un messaggio di errore che informa che il reparto IT ha disattivato l' **iscrizione per il centro per i partner**. 

Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o l'iscrizione virale è disabilitata nel tenant del Azure AD. L'amministratore globale dell'account di Azure AD può abilitare le funzionalità necessarie eseguendo il comando PowerShell seguente:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Per altre informazioni, vedere [iscrizione self-service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)

### <a name="you-forgot-your-password"></a>Password dimenticata

Se si dimentica la password, selezionare il collegamento **non è possibile accedere all'account?** nella pagina di accesso per reimpostare la password o chiedere all'amministratore globale di assegnare le nuove credenziali.

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Nella schermata "informazioni sull'azienda" viene visualizzato un errore che indica che si è verificato un problema

Questo problema si verifica in genere se si usano inavvertitamente caratteri speciali, spazi o codici paese nel numero di telefono dell'azienda. Il valore immesso nel campo numero di telefono può contenere un massimo di 10 caratteri.

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Si sta provando a completare l'acquisto tramite carta di credito, ma si riceve un messaggio di errore che informa che l'ordine è stato rifiutato. Verificare le informazioni "

È sempre necessario inserire l'indirizzo corrispondente alla carta di credito e non corrispondente all'entità legale. Verificare inoltre che il codice postale sia corretto e corrisponda all'indirizzo utilizzato.

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Si desidera passare dal pagamento offline al metodo di pagamento online 

È necessario annullare l'ordine originale e riacquistare usando il metodo di pagamento preferito.

Per annullare un ordine:

1. Selezionare la scheda **offerte di appartenenza** nel dashboard.

2. Seleziona **ordine di annullamento**

3. Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.
