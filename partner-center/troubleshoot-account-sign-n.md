---
title: Risolvere i problemi di configurazione dell'account Partner Center o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi durante il tentativo di registrazione in Partner Center. Le risposte consentono di risolvere i problemi relativi ai metodi di pagamento, all'eliminazione delle password e altro ancora.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686263"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Risolvere i problemi di configurazione dell'account o di rinnovo MPN


**Ruoli appropriati**

- Amministratore globale
- Amministratore dei partner MPN
 
Di seguito sono riportati alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell Partner Center account.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Cosa accade se si esegue la migrazione da Partner Membership Center e non è possibile modificare i campi di informazioni aziendali

Nei casi in cui l'azienda ha già una presenza in Partner Center (ad esempio, un account CSP), verrà visualizzata una schermata di sola lettura. Questa schermata visualizza tutte le informazioni sull'azienda così come esiste Partner Center.

Non è possibile modificare i dettagli in questa schermata. Si tratta di un errore di progettazione e non di un errore.

Selezionare **Accetta** e **continua** per continuare.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Se il reparto IT ha disattivato **l'iscrizione per l'Partner Center**

Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o perché l'iscrizione virale è disabilitata Azure AD tenant. L'amministratore globale per l'account Azure AD può abilitare le funzionalità necessarie eseguendo il comando di PowerShell seguente:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Per altre informazioni, vedere [Iscrizione self-service.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>La password è stata dimenticata

Se la password è stata dimenticata, selezionare il collegamento Non è possibile **accedere all'account?** nella pagina di accesso. Questa opzione consente di reimpostare la password o chiedere all'amministratore globale di assegnare nuove credenziali.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Nella schermata "Informazioni sull'azienda" viene visualizzato un errore "Si è verificato un errore"

Questo messaggio di errore viene in genere visualizzato se si usano inavvertitamente caratteri speciali, spazi o codice paese nel numero di telefono dell'azienda. Il valore immesso nel campo Numero di telefono può contenere solo un massimo di 10 caratteri.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>L'acquisto con carta di credito riceve un messaggio di errore che indica che l'ordine è stato rifiutato. Verificare le informazioni"


Usare sempre l'indirizzo corrispondente alla carta di credito anziché la persona legale. Assicurarsi inoltre che il codice postale sia corretto e corrisponda all'indirizzo in uso.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Si vuole passare dal pagamento offline al metodo di pagamento online 

Sarà necessario annullare l'ordine originale e riacquisirlo usando il metodo di pagamento preferito.

Per annullare un ordine:

1. Selezionare **la scheda Offerte** di appartenenza nel dashboard.

2. Selezionare **Annulla ordine**

3. Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire l'account per il Centro per i partner](partner-center-account-setup.md)
- [Come leggere la fattura e il file di ricognizione](read-your-bill.md)
