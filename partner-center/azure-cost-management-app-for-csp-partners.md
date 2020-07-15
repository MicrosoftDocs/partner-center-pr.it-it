---
title: Gestione dei costi di Azure di Cloudyn per CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come registrare l'app Web Cloudyn e usare una chiave privata per l'app nel centro per i partner, in modo da poter usare l'app per tenere traccia dell'utilizzo e dei costi di Azure per i clienti.
author: aparnagkrishnan
ms.author: aparnag
Keywords: App gestione costi di Azure, Gestisci costi, app Web
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 521501f9a979c0993d299ab30443168408656a44
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390448"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="9a43d-104">Tieni traccia dell'utilizzo e dei costi di Azure per i clienti con l'app gestione costi di Azure per i partner CSP</span><span class="sxs-lookup"><span data-stu-id="9a43d-104">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="9a43d-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="9a43d-105">**Applies to**</span></span>

- <span data-ttu-id="9a43d-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9a43d-106">Partner Center</span></span>
- <span data-ttu-id="9a43d-107">Partner del programma Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="9a43d-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="9a43d-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="9a43d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="9a43d-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9a43d-109">Global admin</span></span>
- <span data-ttu-id="9a43d-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="9a43d-110">Admin agent</span></span>

[<span data-ttu-id="9a43d-111">Ottenere altre informazioni su gestione costi di Azure</span><span class="sxs-lookup"><span data-stu-id="9a43d-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="9a43d-112">Prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="9a43d-112">Before you begin</span></span>
<span data-ttu-id="9a43d-113">Prima di poter usare gestione costi di Azure, assicurarsi di soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="9a43d-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="9a43d-114">Si è partner del programma Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="9a43d-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="9a43d-115">Si ha la possibilità di creare un'app Web per le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9a43d-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="9a43d-116">Panoramica</span><span class="sxs-lookup"><span data-stu-id="9a43d-116">Overview</span></span>

<span data-ttu-id="9a43d-117">Cloudyn è un'app Web che consente di tenere traccia e gestire la quantità di utilizzo di Azure da parte dei clienti e i costi dell'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="9a43d-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="9a43d-118">Viene usato tramite l'API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9a43d-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="9a43d-119">Registrare l'app Web nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9a43d-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="9a43d-120">Quando si registra un'app Web Azure Active Directory nel centro per i partner, si Abilita l'accesso all'API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9a43d-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="9a43d-121">Accedere [al centro per i partner](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando un [account di amministratore globale o di amministratore](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="9a43d-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="9a43d-122">Dal centro per i **partner**selezionare **Impostazioni account** &gt; **[gestione app](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="9a43d-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="9a43d-123">Nella sezione **app Web** fare clic su **Aggiungi nuova app Web**.</span><span class="sxs-lookup"><span data-stu-id="9a43d-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="9a43d-124">**Nota**: se in precedenza è stata creata un'app Web, è possibile ignorare il passaggio 3.</span><span class="sxs-lookup"><span data-stu-id="9a43d-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="9a43d-125">Copiare e salvare il GUID **ID Commerce** e il GUID **ID app** per l'app Web.</span><span class="sxs-lookup"><span data-stu-id="9a43d-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="9a43d-126">Sono necessari entrambi gli ID per usare la versione di valutazione gratuita di 30 giorni dell'app gestione costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="9a43d-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="9a43d-127">Aggiungere una chiave privata all'app</span><span class="sxs-lookup"><span data-stu-id="9a43d-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="9a43d-128">Nell'elenco a discesa accanto al pulsante **Aggiungi chiave** selezionare una durata di 1 o 2 anni.</span><span class="sxs-lookup"><span data-stu-id="9a43d-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="9a43d-129">Fare clic su **Aggiungi chiave**.</span><span class="sxs-lookup"><span data-stu-id="9a43d-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="9a43d-130">Copiare e salvare il valore della chiave privata.</span><span class="sxs-lookup"><span data-stu-id="9a43d-130">Copy and save the secret key value.</span></span> <span data-ttu-id="9a43d-131">Questa operazione sarà necessaria per la versione di valutazione gratuita di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="9a43d-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="9a43d-132">Le chiavi segrete dell'applicazione sono simili alle password con date di scadenza più lunghe.</span><span class="sxs-lookup"><span data-stu-id="9a43d-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="9a43d-133">Salvare il valore della chiave in un percorso sicuro per un uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9a43d-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9a43d-134">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="9a43d-134">Next steps</span></span>
<span data-ttu-id="9a43d-135">Avviare una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="9a43d-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="9a43d-136">Per avviare la versione di valutazione sono necessari i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="9a43d-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="9a43d-137">Credenziali di accesso al centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9a43d-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="9a43d-138">GUID ID Commerce</span><span class="sxs-lookup"><span data-stu-id="9a43d-138">Commerce ID GUID</span></span>
- <span data-ttu-id="9a43d-139">GUID ID app</span><span class="sxs-lookup"><span data-stu-id="9a43d-139">App ID GUID</span></span>
- <span data-ttu-id="9a43d-140">Valore della chiave privata dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="9a43d-140">Application secret key value</span></span>
