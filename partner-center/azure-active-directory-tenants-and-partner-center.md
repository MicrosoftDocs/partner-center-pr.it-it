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
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="1f72e-104">Tenant di Azure Active Directory e Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="1f72e-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="1f72e-105">Si applica a</span><span class="sxs-lookup"><span data-stu-id="1f72e-105">Applies to</span></span>**

-  <span data-ttu-id="1f72e-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1f72e-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="1f72e-107">Perché è necessario disporre di un tenant di Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f72e-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="1f72e-108">Dobbiamo collegare il tenant di Azure AD dell'organizzazione al nuovo account del Centro per i Partner, in modo che gli utenti tenant possano accedere al Centro per i partner con i propri nomi utente di Azure AD (account Microsoft) e le password.</span><span class="sxs-lookup"><span data-stu-id="1f72e-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="1f72e-109">Se la propria azienda dispone già di un tenant di Azure AD, puoi collegarlo all'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1f72e-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="1f72e-110">Nota</span><span class="sxs-lookup"><span data-stu-id="1f72e-110">Note</span></span>**<br> <span data-ttu-id="1f72e-111">Prima di decidere di usare un tenant di Azure AD esistente, valuta il numero di utenti nel tenant che dovranno lavorare nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1f72e-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="1f72e-112">Se sono presenti utenti nel tenant che non dovranno lavorare nel Centro per i partner, valuta la possibilità di creare un nuovo tenant solo per gli utenti che dovranno lavorare nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1f72e-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="1f72e-113">Se l'azienda non dispone già di un tenant di Azure AD, puoi crearne uno senza costi aggiuntivi durante il processo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="1f72e-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="1f72e-114">Seleziona **Crea nuovo tenant** nella pagina **Accedi ad Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="1f72e-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="1f72e-115">Non sei sicuro che l'azienda disponga già di un tenant di Azure AD?</span><span class="sxs-lookup"><span data-stu-id="1f72e-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="1f72e-116">Se non sei sicuro che l'azienda disponga di un tenant di Azure AD, attieniti ai seguenti passaggi per controllare.</span><span class="sxs-lookup"><span data-stu-id="1f72e-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="1f72e-117">Tieni presente che se disponi di un abbonamento attivo per Microsoft Azure o Office 365, disponi già di un tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1f72e-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="1f72e-118">Accedi al portale di amministrazione di Azure all'indirizzo https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="1f72e-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="1f72e-119">Seleziona Azure Active Directory dal menu, quindi seleziona i nomi di dominio.</span><span class="sxs-lookup"><span data-stu-id="1f72e-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="1f72e-120">Se disponi già di un tenant, il nome di dominio verrà elencato.</span><span class="sxs-lookup"><span data-stu-id="1f72e-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="1f72e-121">Uso di un tenant esistente?</span><span class="sxs-lookup"><span data-stu-id="1f72e-121">Using an existing tenant?</span></span>

<span data-ttu-id="1f72e-122">Se desideri utilizzare un tenant di Azure AD esistente, ma si verificano problemi durante l'accesso, trova lo scenario nel diagramma seguente che meglio corrisponda alla situazione specifica e segui i passaggi consigliati.</span><span class="sxs-lookup"><span data-stu-id="1f72e-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![Disponi di un tenant di Azure AD oppure devi crearne uno?](images/onboardingAADFlow.png)

<span data-ttu-id="1f72e-124">Per ulteriori informazioni sull'aggiunta di domini in Azure AD, consulta [Aggiungi o associa un dominio in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="1f72e-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="1f72e-125">Informazioni su Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1f72e-125">About Microsoft Azure</span></span>

<span data-ttu-id="1f72e-126">Microsoft Azure è una piattaforma cloud pubblica che le società possono utilizzare per creare, distribuire e gestire le applicazioni in una rete globale di data center gestiti da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1f72e-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="1f72e-127">Le aziende usano Azure per creare un'infrastruttura IT virtuale con funzioni virtuali o servizi, invece di computer fisici.</span><span class="sxs-lookup"><span data-stu-id="1f72e-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="1f72e-128">Quando acquisti una sottoscrizione di Azure, essenzialmente stai noleggiando uno spazio dedicato e sicuro in un cloud pubblico di Azure, non è molto diverso dal prendere in affitto un piano in un edificio per ospitare le attività letteralmente fisiche dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="1f72e-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="1f72e-129">Per il proprietario dell'edificio, l'azienda è un tenant.</span><span class="sxs-lookup"><span data-stu-id="1f72e-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="1f72e-130">Un tenant di Azure AD è una rappresentazione virtuale dedicata e isolata della società nel cloud pubblico di Azure, creato quando sottoscrivi un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.</span><span class="sxs-lookup"><span data-stu-id="1f72e-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="1f72e-131">Il tenant ospita gli utenti di Azure AD e le informazioni su di essi: password, dati del profilo, autorizzazioni e così via.</span><span class="sxs-lookup"><span data-stu-id="1f72e-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="1f72e-132">Il tenant contiene anche gruppi, applicazioni e altre informazioni relative all'azienda e alla sua sicurezza.</span><span class="sxs-lookup"><span data-stu-id="1f72e-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="1f72e-133">Per ulteriori informazioni su Azure AD, consulta la [Documentazione di Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="1f72e-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 