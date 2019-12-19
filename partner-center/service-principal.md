---
title: Entità servizio di Azure AD | Centro per i partner
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aggiungere un'entità servizio al tenant di Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, piano di Azure, entità servizio, applicazione Azure AD
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010382"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="320b0-104">Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="320b0-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="320b0-105">Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nel tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320b0-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="320b0-106">Questa operazione era possibile in precedenza nell'account del portale Cloud Partner, ma dopo la migrazione al Centro per i partner, tale account è diventato di sola lettura. Si noti che entità servizio è sinonimo di applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320b0-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="320b0-107">Aggiungere un'applicazione Azure AD (entità servizio)</span><span class="sxs-lookup"><span data-stu-id="320b0-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="320b0-108">Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.</span><span class="sxs-lookup"><span data-stu-id="320b0-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="320b0-109">Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="320b0-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="320b0-110">Selezionare un'applicazione Azure AD esistente o crearne una nuova.</span><span class="sxs-lookup"><span data-stu-id="320b0-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="320b0-111">Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="320b0-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="320b0-112">  
\*\*Nome\*\*: è simile al campo 'nome descrittivo' del portale Cloud Partner.</span><span class="sxs-lookup"><span data-stu-id="320b0-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="320b0-113">**URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320b0-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="320b0-114">**URI ID app**: Questo è un identificatore logico per l'applicazione Azure AD presentato quando invia una richiesta Single Sign-On ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320b0-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="320b0-115">**Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.</span><span class="sxs-lookup"><span data-stu-id="320b0-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="320b0-116">Quando si seleziona **Salva**, per creare questa applicazione nel Centro per i partner, le informazioni vengono anche sincronizzate nel sistema del portale Cloud Partner.</span><span class="sxs-lookup"><span data-stu-id="320b0-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
