---
title: Collegare l'account aziendale per accedere al Centro per i partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Crea un account aziendale per collegare l'azienda al Centro per i partner. In questo modo i dipendenti dell'azienda potranno accedere al Centro per i partner.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: bc837db5a9dbcf92fbfead54b552695a218ae675
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534795"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Creare un account aziendale per collegare l'azienda al Centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore gestione utenti

## <a name="why-you-need-a-work-account"></a>Perché è necessario un account aziendale

Microsoft richiede di collegare il proprio account aziendale al nuovo account del Centro per i partner. Il collegamento consente agli utenti dell'account di accedere al Centro per i partner con i nomi utente e le password dell'account aziendale.

## <a name="the-work-account-email-address"></a>Indirizzo e-mail dell'account aziendale

L'indirizzo e-mail aziendale o quello dell'account aziendale è l'indirizzo e-mail che ti è stato fornito dall'azienda. L'indirizzo e-mail di un account aziendale è in genere nel formato `you@yourcompany.com`. Gli indirizzi e-mail personali, ad esempio Hotmail, Gmail o Yahoo, non sono di tipo aziendale e non possono essere usati per l'account del Centro per i partner.

Se hai più indirizzi e-mail aziendali validi, usa quello associato alla sede centrale dell'azienda anziché al reparto regionale, ad esempio usa `contoso.com` anziché `contoso.uk`.

> [!NOTE]  
> Prima di decidere di usare un account aziendale esistente, valuta il numero di utenti dell'account che dovranno usare il Centro per i partner. Se nell'account sono presenti utenti che non dovranno lavorare nel Centro per i partner, valuta la possibilità di creare un nuovo account solo per gli utenti che dovranno usare il Centro per i partner.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Se non si è certi che l'azienda abbia già un account aziendale

Se non sei certo che l'azienda abbia un account aziendale, verifica questo aspetto attenendoti alla procedura seguente. Se hai una sottoscrizione attiva a Microsoft Azure o Office 365, hai già un account aziendale.

1. Accedi al [portale di Azure](https://portal.azure.com).

2. Seleziona Azure Active Directory dal menu e quindi seleziona Nomi di dominio.

3. Se hai già un account aziendale, il nome del tuo dominio verrà visualizzato nell'elenco.

Se la tua azienda non ha ancora un account aziendale, puoi crearne uno durante il processo di registrazione.

Il diagramma seguente illustra i passaggi da eseguire per alcuni scenari tipici:

- stabilisci se hai un account aziendale
- determina come accedere all'account aziendale
- stabilisci se devi creare un nuovo account aziendale

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Hai un account aziendale o devi crearne uno?":::

Per altre informazioni sull'aggiunta di domini in Azure AD, vedi [Aggiungere o associare un dominio in Azure AD](/azure/active-directory/active-directory-add-domain).

## <a name="about-microsoft-azure"></a>Informazioni su Microsoft Azure

Microsoft Azure è una piattaforma cloud pubblica che consente alle aziende di creare, distribuire e gestire le applicazioni in una rete globale di data center gestiti da Microsoft. Le aziende usano Azure per creare un'infrastruttura IT virtuale con funzioni virtuali, o servizi, invece di computer fisici.

Quando acquisti una sottoscrizione di Azure, stai fondamentalmente affittando uno spazio dedicato e sicuro nel cloud pubblico di Azure, non molto diverso dall'affitto di un piano in un edificio direzionale per ospitare le attività fisiche della tua azienda. Per il proprietario dell'edificio direzionale, la tua azienda è un tenant.

Un account aziendale Azure è una rappresentazione virtuale, dedicata e isolata, della tua azienda nel cloud pubblico di Azure che viene creata al momento della sottoscrizione di un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.

Il tuo account aziendale ospita gli utenti di Azure AD e le informazioni correlate: password, dati del profilo, autorizzazioni e così via. L'account aziendale contiene anche gruppi, applicazioni e altre informazioni relative a una società e alla sua sicurezza.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire l'account per il Centro per i partner](partner-center-account-setup.md)
- [Stato di verifica della tracciabilità](verification-responses.md)