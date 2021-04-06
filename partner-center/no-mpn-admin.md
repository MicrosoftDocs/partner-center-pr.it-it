---
title: Cosa fare se l'unico amministratore del programma MPN ha lasciato la società?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle operazioni da eseguire per trovare un nuovo amministratore MPN o ottenere assistenza dall'amministratore globale dell'azienda. Inoltre, informazioni su come aggiungere un nuovo amministratore globale del centro per i partner.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3702ebd5a9421036a053a9a142a2f40d3e488137
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106442000"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Cosa fare se l'unico amministratore del programma MPN ha lasciato la società?

**Ruoli appropriati**

- Amministratore dei partner MPN
- Amministratore degli account
- Amministratore globale

L'articolo seguente illustra tre scenari tipici relativi alle operazioni da eseguire se l'amministratore MPN ha lasciato l'azienda.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: l'amministratore del partner MPN o l'amministratore dell'account ha lasciato la società, ma sono ancora presenti amministratori globali nell'account

In questo caso, è possibile assegnare un altro utente della società al ruolo di amministratore partner MPN. Per essere assegnato il ruolo di amministratore dell'account/amministratore del partner MPN specifico:

1. Accedere all'account del centro per i partner con l'account aziendale, ad esempio tom@contoso.com .
1. Dal filtro della pagina **Gestione utenti** su amministratore globale per vedere chi sono gli amministratori globali dell'azienda. 
1. Contattare uno degli amministratori globali e chiedere di assegnare il ruolo specifico di MPN necessario. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: l'amministratore dell'account o l'amministratore del partner MPN ha lasciato la società e non sono presenti amministratori globali nell'account 

Se si passa alla pagina di **gestione degli utenti** e si filtra l'amministratore globale, ma si scopre che nell'azienda non è presente alcun amministratore globale che può aiutare a ottenere il ruolo specifico di MPN, attenersi alla procedura seguente:

1. Passare a [Portal.Azure.com](https://ms.portal.azure.com/), accedere con l'account aziendale (ad esempio, tom@contoso.com ). 
1. Selezionare l'opzione **Guida e supporto** nella barra di navigazione del menu a sinistra.
1. Nella pagina successiva selezionare **nuovo richiesta di supporto** e tipo di **problema tecnico** nel menu a discesa, inserire eventuali dettagli aggiuntivi e fare clic su **Avanti: soluzioni.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Individuare l'amministratore in portale di Azure":::

4. Dopo aver esaminato le soluzioni consigliate nella pagina successiva, selezionare **Avanti: dettagli** e completare i campi necessari.
1. Esaminare e creare la richiesta di supporto.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: l'amministratore del partner MPN/amministratore dell'account/amministratore globale ha lasciato la società e non sono presenti altri utenti che possono accedere alla Azure AD della società. Si tratta di una perdita completa di accesso.

Attenersi alla procedura di [acquisizione dell'amministratore](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) per acquisire la proprietà di una directory non gestita come amministratore Azure Active Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Se non si è certi che l'azienda abbia già un account aziendale

Se non si è certi che la società disponga di un account di lavoro, attenersi alla procedura seguente per verificare.

1. Accedere al portale di [amministrazione di Azure](https://ms.portal.azure.com).
2. Selezionare **Azure Active Directory** dal menu a sinistra e quindi selezionare **nomi di dominio**.
Se hai già un account aziendale, il nome del tuo dominio verrà visualizzato nell'elenco.

>[!Note]
>Se si dispone di una sottoscrizione attiva per Microsoft Azure o Office 365, si dispone già di un account aziendale e le credenziali di accesso devono essere identiche a quelle usate per accedere a tali servizi.