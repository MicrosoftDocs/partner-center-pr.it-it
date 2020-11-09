---
title: Risolvere i problemi di configurazione dell'account del centro per i partner o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi durante il tentativo di registrazione nel centro per i partner. Le risposte rispondono a problemi con i metodi di pagamento, dimenticando le password e altro ancora.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381410"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Risolvere i problemi di configurazione dell'account o di rinnovo MPN

**Si applica a**

- Centro per i partner
 
**Ruoli appropriati**

- Amministratore globale
- Amministratore dei partner MPN 
 
Ecco alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell'account del centro per i partner.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Cosa accade se si esegue la migrazione da partner Membership Center e non è possibile modificare i campi di informazioni aziendali

Nei casi in cui la società dispone già di una presenza nel centro per i partner (ad indicare un account CSP), verrà visualizzata una schermata di sola lettura. In questa schermata vengono visualizzate tutte le informazioni sull'azienda così come esistono nel centro per i partner.

Non è possibile modificare i dettagli in questa schermata. Si tratta di un errore di progettazione.

Selezionare **Accetto** e **continuare** per procedere.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Se il reparto IT ha disattivato l' **iscrizione per il centro per i partner**.

Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o perché l'iscrizione virale è disabilitata nel tenant Azure AD. L'amministratore globale dell'account di Azure AD può abilitare le funzionalità necessarie eseguendo il comando PowerShell seguente:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Per altre informazioni, vedere [iscrizione self-service](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Password dimenticata

Se si dimentica la password, selezionare il collegamento **non è possibile accedere all'account?** nella pagina di accesso. Questa opzione consente di reimpostare la password o di richiedere all'amministratore globale di assegnare le nuove credenziali.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Nella schermata "informazioni sull'azienda" viene visualizzato un errore che indica che si è verificato un problema

Questo messaggio di errore viene in genere visualizzato se si usano inavvertitamente caratteri speciali, spazi o codice paese nel numero di telefono dell'azienda. Il valore immesso nel campo numero di telefono può contenere un massimo di 10 caratteri.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>L'acquisto della carta di credito riceve un messaggio di errore che informa che l'ordine è stato rifiutato. Verificare le informazioni "


Usare sempre l'indirizzo corrispondente alla carta di credito invece che all'entità legale. Verificare inoltre che il codice postale sia corretto e corrisponda all'indirizzo utilizzato.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Si desidera passare dal pagamento offline al metodo di pagamento online 

È necessario annullare l'ordine originale e riacquistare usando il metodo di pagamento preferito.

Per annullare un ordine:

1. Selezionare la scheda **offerte di appartenenza** nel dashboard.

2. Seleziona **ordine di annullamento**

3. Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire l'account per il Centro per i partner](partner-center-account-setup.md)
- [Come leggere il file di fatturazione e di ricognizione](read-your-bill.md)
