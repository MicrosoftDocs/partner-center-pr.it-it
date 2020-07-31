---
title: Entità servizio di Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere un'entità servizio al tenant di Azure AD. Si tratta di aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365757"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="96ad4-104">Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="96ad4-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="96ad4-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="96ad4-105">**Applies to**</span></span>

- <span data-ttu-id="96ad4-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="96ad4-106">Partner Center</span></span>

<span data-ttu-id="96ad4-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="96ad4-107">**Appropriate roles**</span></span>

- <span data-ttu-id="96ad4-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="96ad4-108">Global admin</span></span>

<span data-ttu-id="96ad4-109">Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="96ad4-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="96ad4-110">Questa operazione in precedenza veniva eseguita nell'account del portale Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="96ad4-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="96ad4-111">Ora che è stata eseguita la migrazione al Centro per i partner, l'account CPP è di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="96ad4-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="96ad4-112">Entità servizio è sinonimo di applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96ad4-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="96ad4-113">Aggiungere un'applicazione Azure AD (entità servizio)</span><span class="sxs-lookup"><span data-stu-id="96ad4-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="96ad4-114">Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.</span><span class="sxs-lookup"><span data-stu-id="96ad4-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="96ad4-115">Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="96ad4-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="96ad4-116">Selezionare un'applicazione Azure AD esistente o crearne una nuova.</span><span class="sxs-lookup"><span data-stu-id="96ad4-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="96ad4-117">Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="96ad4-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="96ad4-118">**URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96ad4-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="96ad4-119">**URI ID app**: un identificatore logico per l'applicazione Azure AD che viene presentato quando invia una richiesta Single Sign-On ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96ad4-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="96ad4-120">**Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="96ad4-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="96ad4-121">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="96ad4-121">Next steps</span></span>

- [<span data-ttu-id="96ad4-122">Panoramica del marketplace commerciale nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="96ad4-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)