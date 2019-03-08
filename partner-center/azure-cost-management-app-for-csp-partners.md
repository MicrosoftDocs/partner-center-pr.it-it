---
title: Azure Cost Management di Cloudyn per i partner CSP | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management di Cloudyn richiede l'accesso tramite provisioning dell'API Centro per i partner.
author: Janet
ms.author: janet
Keywords: App di gestione costi di Azure, gestione dei costi, le app web
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586084"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="0c6d6-104">App Azure Cost Management per i partner CSP Azure</span><span class="sxs-lookup"><span data-stu-id="0c6d6-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="0c6d6-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="0c6d6-105">**Applies to**</span></span>

-  <span data-ttu-id="0c6d6-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0c6d6-106">Partner Center</span></span>

[<span data-ttu-id="0c6d6-107">Ottenere altre informazioni su gestione costi di Azure</span><span class="sxs-lookup"><span data-stu-id="0c6d6-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="0c6d6-108">Prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="0c6d6-108">Before you begin</span></span>
<span data-ttu-id="0c6d6-109">Prima di poter utilizzare Azure Cost Management, assicurati che siano soddisfatti i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="0c6d6-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="0c6d6-110">Essere partner del programma Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="0c6d6-111">Essere in grado di creare un'app Web API di Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="0c6d6-112">Panoramica</span><span class="sxs-lookup"><span data-stu-id="0c6d6-112">Overview</span></span>

<span data-ttu-id="0c6d6-113">Azure Cost Management di Cloudyn è un'app Web che consente di tenere traccia e gestire l'utilizzo di Azure da parte dei clienti e i costi di tale utilizzo.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-113">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="0c6d6-114">Puoi usare l'app tramite l'API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="0c6d6-115">Registra la tua app Web nel Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="0c6d6-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="0c6d6-116">Registrando un'app Web di Azure Active Directory nel Centro per i partner, abiliti l'accesso all'API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="0c6d6-117">Accedi al [Centro per i partner](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) utilizzando un [account di amministratore globale o agente amministratore](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="0c6d6-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="0c6d6-118">Dal **Centro per i Partner**, selezionare **impostazioni Account** &gt;  **[gestione delle App](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="0c6d6-119">Nella sezione **Web App** fai clic su **Add new web app**.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="0c6d6-120">**Nota**: Se è stato creato in precedenza un'app web, è possibile ignorare il passaggio 3.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="0c6d6-121">Copia e salva i GUID **Commerce ID** e **App ID** per la tua app Web.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="0c6d6-122">Entrambi gli ID ti serviranno per utilizzare la versione di valutazione gratuita di 30 giorni dell'app di gestione dei costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="0c6d6-123">Aggiungi una chiave privata alla tua app.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="0c6d6-124">Nell'elenco a discesa accanto al pulsante **Add key** seleziona una durata di 1 o 2 anni.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="0c6d6-125">Fai clic su **Add key**.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="0c6d6-126">Copia e salva il valore della chiave privata.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-126">Copy and save the secret key value.</span></span> <span data-ttu-id="0c6d6-127">Questo valore ti servirà per la versione di valutazione gratuita di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="0c6d6-128">Le chiavi private dell'applicazione sono come le password con date di scadenza più lunghe.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="0c6d6-129">Salva il valore della chiave in un luogo sicuro per l'utilizzo futuro.</span><span class="sxs-lookup"><span data-stu-id="0c6d6-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0c6d6-130">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="0c6d6-130">Next steps</span></span>
<span data-ttu-id="0c6d6-131">Avvia una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="0c6d6-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="0c6d6-132">Per avviare la versione di valutazione ti serve quanto segue:</span><span class="sxs-lookup"><span data-stu-id="0c6d6-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="0c6d6-133">Credenziali di accesso al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0c6d6-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="0c6d6-134">GUID ID commerce</span><span class="sxs-lookup"><span data-stu-id="0c6d6-134">Commerce ID GUID</span></span>
- <span data-ttu-id="0c6d6-135">GUID ID app</span><span class="sxs-lookup"><span data-stu-id="0c6d6-135">App ID GUID</span></span>
- <span data-ttu-id="0c6d6-136">Valore della chiave privata dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="0c6d6-136">Application secret key value</span></span>
