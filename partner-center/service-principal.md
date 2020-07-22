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
ms.openlocfilehash: 9d0507b684b213e6da5f48a250e6e61f395fd52a
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436430"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="e5732-104">Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="e5732-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="e5732-105">Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="e5732-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="e5732-106">Questa operazione in precedenza veniva eseguita nell'account del portale Cloud Partner (CPP).</span><span class="sxs-lookup"><span data-stu-id="e5732-106">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="e5732-107">Ora che è stata eseguita la migrazione al Centro per i partner, l'account CPP è di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="e5732-107">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="e5732-108">Entità servizio è sinonimo di applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5732-108">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="e5732-109">Aggiungere un'applicazione Azure AD (entità servizio)</span><span class="sxs-lookup"><span data-stu-id="e5732-109">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="e5732-110">Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.</span><span class="sxs-lookup"><span data-stu-id="e5732-110">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="e5732-111">Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="e5732-111">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="e5732-112">Selezionare un'applicazione Azure AD esistente o crearne una nuova.</span><span class="sxs-lookup"><span data-stu-id="e5732-112">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="e5732-113">Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="e5732-113">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="e5732-114">**URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5732-114">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="e5732-115">**URI ID app**: un identificatore logico per l'applicazione Azure AD che viene presentato quando invia una richiesta Single Sign-On ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5732-115">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="e5732-116">**Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5732-116">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
