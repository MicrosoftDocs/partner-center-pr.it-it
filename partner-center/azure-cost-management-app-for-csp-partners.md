---
title: Azure Cost Management di Cloudyn per i partner CSP | Centro per i partner
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come registrare l'app Web Cloudyn e usare una chiave privata per l'app nel centro per i partner, in modo da poter usare l'app per tenere traccia dell'utilizzo e dei costi di Azure per i clienti.
author: Janet
ms.author: janet
Keywords: App gestione costi di Azure, Gestisci costi, app Web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253300"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="ba77d-104">App Azure Cost Management per i partner CSP Azure</span><span class="sxs-lookup"><span data-stu-id="ba77d-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="ba77d-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="ba77d-105">**Applies to**</span></span>

- <span data-ttu-id="ba77d-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ba77d-106">Partner Center</span></span>
- <span data-ttu-id="ba77d-107">Partner del programma Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="ba77d-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="ba77d-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="ba77d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="ba77d-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="ba77d-109">Global admin</span></span>
- <span data-ttu-id="ba77d-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="ba77d-110">Admin agent</span></span>

[<span data-ttu-id="ba77d-111">Ottenere altre informazioni su gestione costi di Azure</span><span class="sxs-lookup"><span data-stu-id="ba77d-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="ba77d-112">Prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="ba77d-112">Before you begin</span></span>
<span data-ttu-id="ba77d-113">Prima di poter utilizzare Azure Cost Management, assicurati che siano soddisfatti i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="ba77d-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="ba77d-114">Essere partner del programma Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="ba77d-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="ba77d-115">Essere in grado di creare un'app Web API di Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba77d-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="ba77d-116">Panoramica</span><span class="sxs-lookup"><span data-stu-id="ba77d-116">Overview</span></span>

<span data-ttu-id="ba77d-117">Cloudyn è un'app Web che consente di tenere traccia e gestire la quantità di utilizzo di Azure da parte dei clienti e i costi dell'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="ba77d-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="ba77d-118">Puoi usare l'app tramite l'API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba77d-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="ba77d-119">Registra la tua app Web nel Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="ba77d-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="ba77d-120">Registrando un'app Web di Azure Active Directory nel Centro per i partner, abiliti l'accesso all'API di Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ba77d-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="ba77d-121">Accedi al [Centro per i partner](https://partnercenter.microsoft.com/pcv/dashboard/overview) utilizzando un [account di amministratore globale o agente amministratore](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="ba77d-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="ba77d-122">Dal centro per i **partner**selezionare **Impostazioni account** &gt; **[gestione app](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="ba77d-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="ba77d-123">Nella sezione **Web App** fai clic su **Add new web app**.</span><span class="sxs-lookup"><span data-stu-id="ba77d-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="ba77d-124">**Nota**: se in precedenza hai creato un'app Web, puoi ignorare il passaggio 3.</span><span class="sxs-lookup"><span data-stu-id="ba77d-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="ba77d-125">Copia e salva i GUID **Commerce ID** e **App ID** per la tua app Web.</span><span class="sxs-lookup"><span data-stu-id="ba77d-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="ba77d-126">Entrambi gli ID ti serviranno per utilizzare la versione di valutazione gratuita di 30 giorni dell'app di gestione dei costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="ba77d-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="ba77d-127">Aggiungi una chiave privata alla tua app.</span><span class="sxs-lookup"><span data-stu-id="ba77d-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="ba77d-128">Nell'elenco a discesa accanto al pulsante **Add key** seleziona una durata di 1 o 2 anni.</span><span class="sxs-lookup"><span data-stu-id="ba77d-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="ba77d-129">Fai clic su **Add key**.</span><span class="sxs-lookup"><span data-stu-id="ba77d-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="ba77d-130">Copia e salva il valore della chiave privata.</span><span class="sxs-lookup"><span data-stu-id="ba77d-130">Copy and save the secret key value.</span></span> <span data-ttu-id="ba77d-131">Questo valore ti servirà per la versione di valutazione gratuita di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="ba77d-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="ba77d-132">Le chiavi segrete dell'applicazione sono simili alle password con date di scadenza più lunghe.</span><span class="sxs-lookup"><span data-stu-id="ba77d-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="ba77d-133">Salva il valore della chiave in un luogo sicuro per l'utilizzo futuro.</span><span class="sxs-lookup"><span data-stu-id="ba77d-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba77d-134">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="ba77d-134">Next steps</span></span>
<span data-ttu-id="ba77d-135">Avvia una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="ba77d-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="ba77d-136">Per avviare la versione di valutazione ti serve quanto segue:</span><span class="sxs-lookup"><span data-stu-id="ba77d-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="ba77d-137">Credenziali di accesso al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ba77d-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="ba77d-138">GUID ID commerce</span><span class="sxs-lookup"><span data-stu-id="ba77d-138">Commerce ID GUID</span></span>
- <span data-ttu-id="ba77d-139">GUID ID app</span><span class="sxs-lookup"><span data-stu-id="ba77d-139">App ID GUID</span></span>
- <span data-ttu-id="ba77d-140">Valore della chiave privata dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="ba77d-140">Application secret key value</span></span>
