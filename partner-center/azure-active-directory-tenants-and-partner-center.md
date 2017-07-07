---
title: Tenant di Azure Active Directory e Centro per i Partner | Centro per i partner
description: "Per creare un account del Centro per i partner, l'azienda deve disporre di un tenant di Azure Active Directory (Azure AD). Azure AD è un servizio di directory basata su cloud e di gestione dell'identità di Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Tenant di Azure Active Directory e Centro per i Partner  

**Si applica a**

-  Centro per i partner

## <a name="why-you-need-an-azure-ad-tenant"></a>Perché è necessario disporre di un tenant di Azure AD

Dobbiamo collegare il tenant di Azure AD dell'organizzazione al nuovo account del Centro per i Partner, in modo che gli utenti tenant possano accedere al Centro per i partner con i propri nomi utente di Azure AD (account Microsoft) e le password.

Se la propria azienda dispone già di un tenant di Azure AD, puoi collegarlo all'account del Centro per i partner. 

>**Nota**<br> Prima di decidere di usare un tenant di Azure AD esistente, valuta il numero di utenti nel tenant che dovranno lavorare nel Centro per i partner. Se sono presenti utenti nel tenant che non dovranno lavorare nel Centro per i partner, valuta la possibilità di creare un nuovo tenant solo per gli utenti che dovranno lavorare nel Centro per i partner.

Se l'azienda non dispone già di un tenant di Azure AD, puoi crearne uno senza costi aggiuntivi durante il processo di registrazione. Seleziona **Crea nuovo tenant** nella pagina **Accedi ad Azure Active Directory**. 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Non sei sicuro che l'azienda disponga già di un tenant di Azure AD?

Se non sei sicuro che l'azienda disponga di un tenant di Azure AD, attieniti ai seguenti passaggi per controllare. Tieni presente che se disponi di un abbonamento attivo per Microsoft Azure o Office 365, disponi già di un tenant di Azure AD.
1.  Accedi al portale di amministrazione di Azure all'indirizzo https://ms.portal.azure.com
2.  Seleziona Azure Active Directory dal menu, quindi seleziona i nomi di dominio.
3.  Se disponi già di un tenant, il nome di dominio verrà elencato.

### <a name="using-an-existing-tenant"></a>Uso di un tenant esistente?

Se desideri utilizzare un tenant di Azure AD esistente, ma si verificano problemi durante l'accesso, trova lo scenario nel diagramma seguente che meglio corrisponda alla situazione specifica e segui i passaggi consigliati. 

![Disponi di un tenant di Azure AD oppure devi crearne uno?](images/onboardingAADFlow.png)

Per ulteriori informazioni sull'aggiunta di domini in Azure AD, consulta [Aggiungi o associa un dominio in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Informazioni su Microsoft Azure

Microsoft Azure è una piattaforma cloud pubblica che le società possono utilizzare per creare, distribuire e gestire le applicazioni in una rete globale di data center gestiti da Microsoft. Le aziende usano Azure per creare un'infrastruttura IT virtuale con funzioni virtuali o servizi, invece di computer fisici. 

Quando acquisti una sottoscrizione di Azure, essenzialmente stai noleggiando uno spazio dedicato e sicuro in un cloud pubblico di Azure, non è molto diverso dal prendere in affitto un piano in un edificio per ospitare le attività letteralmente fisiche dell'azienda. Per il proprietario dell'edificio, l'azienda è un tenant. 

Un tenant di Azure AD è una rappresentazione virtuale dedicata e isolata della società nel cloud pubblico di Azure, creato quando sottoscrivi un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365. 

Il tenant ospita gli utenti di Azure AD e le informazioni su di essi: password, dati del profilo, autorizzazioni e così via. Il tenant contiene anche gruppi, applicazioni e altre informazioni relative all'azienda e alla sua sicurezza. 

Per ulteriori informazioni su Azure AD, consulta la [Documentazione di Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/). 