---
title: Entità servizio di Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere un'entità servizio al tenant di Azure AD. Si tratta di aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028469"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="ad261-104">Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ad261-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="ad261-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="ad261-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ad261-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="ad261-106">Global admin</span></span>

<span data-ttu-id="ad261-107">Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ad261-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="ad261-108">Questa operazione in precedenza veniva eseguita nell'account del portale Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="ad261-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="ad261-109">Ora che è stata eseguita la migrazione al Centro per i partner, l'account CPP è di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="ad261-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="ad261-110">Entità servizio è sinonimo di applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad261-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="ad261-111">Aggiungere un'applicazione Azure AD (entità servizio)</span><span class="sxs-lookup"><span data-stu-id="ad261-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="ad261-112">Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.</span><span class="sxs-lookup"><span data-stu-id="ad261-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="ad261-113">Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="ad261-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="ad261-114">Selezionare un'applicazione Azure AD esistente o crearne una nuova.</span><span class="sxs-lookup"><span data-stu-id="ad261-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="ad261-115">Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="ad261-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="ad261-116">**URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad261-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="ad261-117">**URI ID app**: un identificatore logico per l'applicazione Azure AD che viene presentato quando invia una richiesta Single Sign-On ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad261-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="ad261-118">**Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad261-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="ad261-119">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="ad261-119">Next steps</span></span>

- [<span data-ttu-id="ad261-120">Panoramica del marketplace commerciale nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ad261-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)