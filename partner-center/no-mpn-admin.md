---
title: Cosa fare se l'unico amministratore del programma MPN ha lasciato l'azienda?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come trovare un nuovo amministratore MPN o ottenere assistenza dall'amministratore globale dell'azienda. Scopri anche come aggiungere un nuovo amministratore Partner Center globale.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277675"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Cosa fare se l'unico amministratore del programma MPN ha lasciato l'azienda?

**Ruoli appropriati:** amministratore partner MPN | Account admin | Amministratore globale

L'articolo seguente illustra tre scenari tipici relativi alle operazioni da eseguire se l'amministratore MPN ha lasciato l'azienda.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: l'amministratore partner o l'amministratore dell'account MPN ha lasciato l'azienda, ma nell'account sono ancora presenti amministratori globali

In questo caso, a un'altra persona dell'azienda può essere assegnato il ruolo di amministratore partner MPN. Per assegnare il ruolo di amministratore partner MPN/amministratore account specifico:

1. Accedere all'account Partner Center con l'account aziendale , ad esempio tom@contoso.com .
1. Nella pagina **Gestione utenti filtrare** in Amministratore globale per vedere chi sono gli amministratori globali dell'azienda. 
1. Contattare uno degli amministratori globali e chiedere di assegnare all'utente il ruolo specifico di MPN necessario. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: l'amministratore partner o l'amministratore dell'account MPN ha lasciato l'azienda e non sono presenti amministratori globali nell'account 

Se si passa alla pagina **User Management** (Gestione utenti) e si filtra l'opzione Global admin (Amministratore globale), ma non è presente alcun amministratore globale nell'azienda che possa aiutare a ottenere il ruolo specifico di MPN, seguire questa procedura:

1. Passare a [portal.azure.com](https://ms.portal.azure.com/), accedere con l'account aziendale , ad esempio tom@contoso.com . 
1. Selezionare **l'opzione Guida e** supporto nella barra di spostamento del menu a sinistra.
1. Nella pagina successiva selezionare New **Richiesta di supporto** and **Technical Issue** type (Nuovo tipo di problema e problema tecnico) nel menu a discesa, inserire eventuali dettagli aggiuntivi e fare clic su **Next: Solutions (Avanti: Soluzioni).**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Individuare admin in portale di Azure.":::

4. Dopo aver esaminato le soluzioni consigliate nella pagina successiva, selezionare **Avanti: Dettagli** e completare i campi necessari.
1. Esaminare e creare la richiesta di supporto.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: l'amministratore partner MPN,l'amministratore dell'account o l'amministratore globale ha lasciato l'azienda e non sono presenti altri utenti che possono accedere alle risorse Azure AD. Si tratta di una perdita completa di accesso.

Seguire la [procedura di acquisizione della proprietà](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) dell'amministratore per assumere la proprietà di una directory non gestita Azure Active Directory amministratore.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Se non si è certi che l'azienda abbia già un account aziendale

Se non si è certi che l'azienda abbia un account aziendale, seguire questa procedura per verificare.

1. Accedere al portale [di amministrazione di Azure.](https://ms.portal.azure.com)
2. Selezionare **Azure Active Directory** dal menu a sinistra e quindi selezionare **Nomi di dominio.**
Se hai già un account aziendale, il nome del tuo dominio verrà visualizzato nell'elenco.

>[!Note]
>Se si ha una sottoscrizione attiva a Microsoft Azure o Office 365, si ha già un account aziendale e le credenziali di accesso devono essere le stesse usate per accedere a tali servizi.