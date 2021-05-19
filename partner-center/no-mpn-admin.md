---
title: Cosa fare se l'unico amministratore del programma MPN ha lasciato l'azienda?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come trovare un nuovo amministratore MPN o ottenere assistenza dall'amministratore globale dell'azienda. Informazioni anche su come aggiungere un nuovo amministratore Partner Center globale.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151169"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Cosa fare se l'unico amministratore del programma MPN ha lasciato l'azienda?

**Ruoli appropriati:** amministratore partner MPN | Account admin | Amministratore globale

L'articolo seguente illustra tre scenari tipici relativi alle operazioni da eseguire se l'amministratore MPN ha lasciato l'azienda.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: l'amministratore partner MPN/amministratore dell'account ha lasciato l'azienda, ma nell'account sono ancora presenti amministratori globali

In questo caso, a un'altra persona dell'azienda può essere assegnato il ruolo di amministratore del partner MPN. Per assegnare il ruolo di amministratore partner MPN o amministratore account specifico:

1. Accedere al proprio account Partner Center con l'account aziendale , ad esempio tom@contoso.com .
1. Dalla pagina **Gestione utenti** filtrare l'amministratore globale per verificare chi sono gli amministratori globali dell'azienda. 
1. Contattare uno degli amministratori globali e chiedere loro di assegnare il ruolo specifico mpn necessario. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: l'amministratore partner MPN/amministratore dell'account ha lasciato l'azienda e non sono presenti amministratori globali nell'account 

Se si passa  alla pagina Gestione utenti e si filtra l'opzione Amministratore globale, ma non è presente alcun amministratore globale nell'azienda che possa aiutare a ottenere il ruolo specifico di MPN, seguire questa procedura:

1. Passare a [portal.azure.com](https://ms.portal.azure.com/), accedere con l'account aziendale , ad esempio tom@contoso.com . 
1. Selezionare **l'opzione Guida e** supporto nella barra di spostamento dei menu a sinistra.
1. Nella pagina successiva selezionare **Nuovo** Richiesta di supporto  e tipo di problema tecnico nel menu a discesa, inserire eventuali dettagli aggiuntivi e fare clic su **Avanti: Soluzioni.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Individuare l'amministratore in portale di Azure":::

4. Dopo aver esaminato le soluzioni consigliate nella pagina successiva, selezionare **Avanti: Dettagli** e completare i campi necessari.
1. Esaminare e creare la richiesta di supporto.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: l'amministratore partner MPN,l'amministratore dell'account o l'amministratore globale ha lasciato l'azienda e non sono presenti altri utenti che possono accedere alla rete aziendale Azure AD. Si tratta di una perdita completa di accesso.

Seguire la [procedura di acquisizione amministratore](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) per assumere il controllo di una directory non gestita come Azure Active Directory amministratore.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Se non si è certi che l'azienda abbia già un account aziendale

Se non si è certi che l'azienda abbia un account aziendale, seguire questa procedura per verificare.

1. Accedere al portale [di amministrazione di Azure.](https://ms.portal.azure.com)
2. Selezionare **Azure Active Directory** dal menu a sinistra e quindi selezionare **Nomi di dominio**.
Se hai già un account aziendale, il nome del tuo dominio verrà visualizzato nell'elenco.

>[!Note]
>Se si ha una sottoscrizione attiva a Microsoft Azure o Office 365, si dispone già di un account aziendale e le credenziali di accesso devono essere uguali a quelle usate per accedere a tali servizi.