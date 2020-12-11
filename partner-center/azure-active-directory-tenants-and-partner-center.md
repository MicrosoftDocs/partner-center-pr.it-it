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
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="58a50-104">Creare un account aziendale per collegare l'azienda al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="58a50-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="58a50-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="58a50-105">**Appropriate roles**</span></span>

- <span data-ttu-id="58a50-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="58a50-106">Global admin</span></span>
- <span data-ttu-id="58a50-107">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="58a50-107">User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="58a50-108">Perché è necessario un account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-108">Why you need a work account</span></span>

<span data-ttu-id="58a50-109">Microsoft richiede di collegare il proprio account aziendale al nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="58a50-109">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="58a50-110">Il collegamento consente agli utenti dell'account di accedere al Centro per i partner con i nomi utente e le password dell'account aziendale.</span><span class="sxs-lookup"><span data-stu-id="58a50-110">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="58a50-111">Indirizzo e-mail dell'account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-111">The work account email address</span></span>

<span data-ttu-id="58a50-112">L'indirizzo e-mail aziendale o quello dell'account aziendale è l'indirizzo e-mail che ti è stato fornito dall'azienda.</span><span class="sxs-lookup"><span data-stu-id="58a50-112">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="58a50-113">L'indirizzo e-mail di un account aziendale è in genere nel formato `you@yourcompany.com`.</span><span class="sxs-lookup"><span data-stu-id="58a50-113">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="58a50-114">Gli indirizzi e-mail personali, ad esempio Hotmail, Gmail o Yahoo, non sono di tipo aziendale e non possono essere usati per l'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="58a50-114">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="58a50-115">Se hai più indirizzi e-mail aziendali validi, usa quello associato alla sede centrale dell'azienda anziché al reparto regionale, ad esempio usa `contoso.com` anziché `contoso.uk`.</span><span class="sxs-lookup"><span data-stu-id="58a50-115">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="58a50-116">Prima di decidere di usare un account aziendale esistente, valuta il numero di utenti dell'account che dovranno usare il Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="58a50-116">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="58a50-117">Se nell'account sono presenti utenti che non dovranno lavorare nel Centro per i partner, valuta la possibilità di creare un nuovo account solo per gli utenti che dovranno usare il Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="58a50-117">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="58a50-118">Se non si è certi che l'azienda abbia già un account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-118">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="58a50-119">Se non sei certo che l'azienda abbia un account aziendale, verifica questo aspetto attenendoti alla procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="58a50-119">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="58a50-120">Se hai una sottoscrizione attiva a Microsoft Azure o Office 365, hai già un account aziendale.</span><span class="sxs-lookup"><span data-stu-id="58a50-120">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="58a50-121">Accedi al [portale di Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="58a50-121">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="58a50-122">Seleziona Azure Active Directory dal menu e quindi seleziona Nomi di dominio.</span><span class="sxs-lookup"><span data-stu-id="58a50-122">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="58a50-123">Se hai già un account aziendale, il nome del tuo dominio verrà visualizzato nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="58a50-123">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="58a50-124">Se la tua azienda non ha ancora un account aziendale, puoi crearne uno durante il processo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="58a50-124">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="58a50-125">Il diagramma seguente illustra i passaggi da eseguire per alcuni scenari tipici:</span><span class="sxs-lookup"><span data-stu-id="58a50-125">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="58a50-126">stabilisci se hai un account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-126">determine if you have a work account</span></span>
- <span data-ttu-id="58a50-127">determina come accedere all'account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-127">determine how to sign into your work account</span></span>
- <span data-ttu-id="58a50-128">stabilisci se devi creare un nuovo account aziendale</span><span class="sxs-lookup"><span data-stu-id="58a50-128">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Hai un account aziendale o devi crearne uno?":::

<span data-ttu-id="58a50-130">Per altre informazioni sull'aggiunta di domini in Azure AD, vedi [Aggiungere o associare un dominio in Azure AD](/azure/active-directory/active-directory-add-domain).</span><span class="sxs-lookup"><span data-stu-id="58a50-130">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="58a50-131">Informazioni su Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="58a50-131">About Microsoft Azure</span></span>

<span data-ttu-id="58a50-132">Microsoft Azure è una piattaforma cloud pubblica che consente alle aziende di creare, distribuire e gestire le applicazioni in una rete globale di data center gestiti da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58a50-132">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="58a50-133">Le aziende usano Azure per creare un'infrastruttura IT virtuale con funzioni virtuali, o servizi, invece di computer fisici.</span><span class="sxs-lookup"><span data-stu-id="58a50-133">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="58a50-134">Quando acquisti una sottoscrizione di Azure, stai fondamentalmente affittando uno spazio dedicato e sicuro nel cloud pubblico di Azure, non molto diverso dall'affitto di un piano in un edificio direzionale per ospitare le attività fisiche della tua azienda.</span><span class="sxs-lookup"><span data-stu-id="58a50-134">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="58a50-135">Per il proprietario dell'edificio direzionale, la tua azienda è un tenant.</span><span class="sxs-lookup"><span data-stu-id="58a50-135">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="58a50-136">Un account aziendale Azure è una rappresentazione virtuale, dedicata e isolata, della tua azienda nel cloud pubblico di Azure che viene creata al momento della sottoscrizione di un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.</span><span class="sxs-lookup"><span data-stu-id="58a50-136">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="58a50-137">Il tuo account aziendale ospita gli utenti di Azure AD e le informazioni correlate: password, dati del profilo, autorizzazioni e così via.</span><span class="sxs-lookup"><span data-stu-id="58a50-137">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="58a50-138">L'account aziendale contiene anche gruppi, applicazioni e altre informazioni relative a una società e alla sua sicurezza.</span><span class="sxs-lookup"><span data-stu-id="58a50-138">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="58a50-139">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="58a50-139">Next steps</span></span>

- [<span data-ttu-id="58a50-140">Gestire l'account per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="58a50-140">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="58a50-141">Stato di verifica della tracciabilità</span><span class="sxs-lookup"><span data-stu-id="58a50-141">Track verification status</span></span>](verification-responses.md)