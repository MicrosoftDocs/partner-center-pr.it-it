---
title: Imposta un budget di spesa di Azure per i clienti
ms.topic: article
ms.date: 06/03/2020
description: Informazioni su come impostare o rimuovere i budget mensili per la spesa di Azure per i clienti e anche per visualizzare i dati di spesa di Azure e impostare le notifiche relative al budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17b6186d7e6cddaf598dc663c70841275c0db853
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425990"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="dbb19-103">Imposta, verifica o Rimuovi i budget mensili per la spesa di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dbb19-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="dbb19-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="dbb19-104">Applies to:</span></span>

- <span data-ttu-id="dbb19-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dbb19-105">Partner Center</span></span>
- <span data-ttu-id="dbb19-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="dbb19-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="dbb19-107">È possibile [impostare un budget mensile per la spesa di Azure per i clienti](#set-azure-spending-budget) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="dbb19-108">Ciò consente ai clienti di gestire la spesa di Azure.</span><span class="sxs-lookup"><span data-stu-id="dbb19-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="dbb19-109">Questa opzione consente di confrontare la spesa di Azure da parte dei clienti al budget durante il mese.</span><span class="sxs-lookup"><span data-stu-id="dbb19-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="dbb19-110">Consente inoltre ai clienti di ottenere un budget per la spesa di Azure in modo che la fattura mensile non sia più elevata del previsto.</span><span class="sxs-lookup"><span data-stu-id="dbb19-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="dbb19-111">Questa funzionalità non è disponibile negli account sandbox o test negli ambienti di produzione (TIP).</span><span class="sxs-lookup"><span data-stu-id="dbb19-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="dbb19-112">Dopo aver [impostato un budget di spesa di Azure per i clienti](#set-azure-spending-budget), è anche possibile esaminare l'utilizzo dei clienti nei modi seguenti.</span><span class="sxs-lookup"><span data-stu-id="dbb19-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="dbb19-113">Queste opzioni possono essere utili per individuare i servizi non configurati correttamente o tendenze insolite che potrebbero suggerire frodi.</span><span class="sxs-lookup"><span data-stu-id="dbb19-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="dbb19-114">È quindi possibile collaborare con i clienti per identificare la causa principale e gestire i costi.</span><span class="sxs-lookup"><span data-stu-id="dbb19-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="dbb19-115">Se necessario, è anche possibile [modificare il budget del cliente impostando](#set-azure-spending-budget) un importo superiore.</span><span class="sxs-lookup"><span data-stu-id="dbb19-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="dbb19-116">Controlla la spesa di Azure corrente</span><span class="sxs-lookup"><span data-stu-id="dbb19-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="dbb19-117">Attivare le notifiche tramite posta elettronica quando la spesa di un cliente sta per avvicinarsi al limite di budget</span><span class="sxs-lookup"><span data-stu-id="dbb19-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="dbb19-118">Visualizza i costi in base al servizio per le sottoscrizioni basate sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="dbb19-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="dbb19-119">È anche possibile [rimuovere un budget di spesa di Azure](#remove-azure-spending-budget) per i clienti in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="dbb19-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="dbb19-120">Dati della spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="dbb19-120">Azure spending data</span></span>

<span data-ttu-id="dbb19-121">I dati di spesa di Azure sono una *stima* e gli *importi di fatturazione effettivi possono variare*.</span><span class="sxs-lookup"><span data-stu-id="dbb19-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="dbb19-122">Il valore dei dati *non riflette* tasse, crediti, rettifiche o altri addebiti che possono essere applicati.</span><span class="sxs-lookup"><span data-stu-id="dbb19-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="dbb19-123">I dati di spesa vengono *aggiornati una volta al giorno*.</span><span class="sxs-lookup"><span data-stu-id="dbb19-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="dbb19-124">I clienti possono continuare a usare i servizi e le risorse di Azure, a meno che non si modifichino le impostazioni dell'account nella portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="dbb19-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="dbb19-125">Imposta budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="dbb19-125">Set Azure spending budget</span></span>

<span data-ttu-id="dbb19-126">È possibile *impostare un budget mensile per la spesa di Azure* per più clienti nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="dbb19-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="dbb19-127">Accedere al dashboard del [centro](https://partner.microsoft.com/dashboard/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dbb19-128">Nel menu a sinistra in **CSP**scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dbb19-129">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti per i quali si desidera impostare un budget.</span><span class="sxs-lookup"><span data-stu-id="dbb19-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="dbb19-130">Immettere un valore per **budget mensile**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="dbb19-131">Scegliere **applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="dbb19-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="dbb19-132">È anche possibile *impostare un budget per un singolo cliente* nelle impostazioni della sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="dbb19-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="dbb19-133">Accedi al dashboard Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="dbb19-134">Nel menu a sinistra in **CSP**scegliere **Customers (clienti**).</span><span class="sxs-lookup"><span data-stu-id="dbb19-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dbb19-135">Nella pagina **Customers** selezionare il **nome della società**del cliente.</span><span class="sxs-lookup"><span data-stu-id="dbb19-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dbb19-136">Nella pagina **sottoscrizioni** del cliente, in **sottoscrizione basata sull'utilizzo**, scegliere **Cambia budget**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="dbb19-137">Immettere un valore per il budget.</span><span class="sxs-lookup"><span data-stu-id="dbb19-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="dbb19-138">Scegliere **applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="dbb19-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="dbb19-139">Rimuovi budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="dbb19-139">Remove Azure spending budget</span></span>

<span data-ttu-id="dbb19-140">È possibile *rimuovere un budget mensile* per la spesa di Azure per i clienti nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="dbb19-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="dbb19-141">Accedere al dashboard del [centro](https://partner.microsoft.com/dashboard/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dbb19-142">Nel menu a sinistra in **CSP**scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dbb19-143">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti di cui si desidera rimuovere il budget.</span><span class="sxs-lookup"><span data-stu-id="dbb19-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="dbb19-144">Scegliere **Rimuovi budget**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="dbb19-145">Controlla la spesa di Azure corrente</span><span class="sxs-lookup"><span data-stu-id="dbb19-145">Check current Azure spending</span></span>

<span data-ttu-id="dbb19-146">Puoi *tenere traccia delle spese di Azure correnti e dei budget mensili dei clienti* in qualsiasi momento:</span><span class="sxs-lookup"><span data-stu-id="dbb19-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="dbb19-147">Accedere al dashboard del [centro](https://partner.microsoft.com/dashboard/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="dbb19-148">Nel menu a sinistra in **CSP**scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dbb19-149">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, è possibile visualizzare una panoramica dei budget mensili dei clienti, le stime di spesa correnti e la percentuale del budget usato.</span><span class="sxs-lookup"><span data-stu-id="dbb19-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="dbb19-150">Notifiche per i limiti del budget</span><span class="sxs-lookup"><span data-stu-id="dbb19-150">Notifications for budget limits</span></span>

<span data-ttu-id="dbb19-151">È possibile *attivare le notifiche tramite posta elettronica* quando la spesa mensile del cliente si avvicina al limite di budget.</span><span class="sxs-lookup"><span data-stu-id="dbb19-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="dbb19-152">Quando si attiva questa opzione, si riceverà una notifica quando i clienti usano il 80% o più del budget mensile.</span><span class="sxs-lookup"><span data-stu-id="dbb19-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="dbb19-153">Questa opzione consente di tenere sotto controllo la fattura di Azure.</span><span class="sxs-lookup"><span data-stu-id="dbb19-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="dbb19-154">Per configurare le notifiche di posta elettronica:</span><span class="sxs-lookup"><span data-stu-id="dbb19-154">To configure email notifications:</span></span>

1. <span data-ttu-id="dbb19-155">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dbb19-156">Nel menu a sinistra in **CSP**scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="dbb19-157">Nella pagina **spesa di Azure** , in **notifiche di posta elettronica**, impostare l'opzione **Ottieni messaggi** di posta elettronica **su**attivato.</span><span class="sxs-lookup"><span data-stu-id="dbb19-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="dbb19-158">Scegliere **modifica indirizzo di posta elettronica** per visualizzare l'indirizzo di posta elettronica per le notifiche.</span><span class="sxs-lookup"><span data-stu-id="dbb19-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="dbb19-159">Se l'indirizzo di posta elettronica *non è corretto*, immettere l'indirizzo di posta elettronica corretto e scegliere **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="dbb19-160">Se l'indirizzo di posta elettronica *è corretto*, scegliere **Annulla**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="dbb19-161">Costi in base al servizio</span><span class="sxs-lookup"><span data-stu-id="dbb19-161">Itemized costs by service</span></span>

<span data-ttu-id="dbb19-162">È possibile *visualizzare i costi (e l'utilizzo stimato) per servizio per le sottoscrizioni basate sull'utilizzo*:</span><span class="sxs-lookup"><span data-stu-id="dbb19-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="dbb19-163">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dbb19-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="dbb19-164">Nel menu a sinistra in **CSP**scegliere **Customers (clienti**).</span><span class="sxs-lookup"><span data-stu-id="dbb19-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="dbb19-165">Nella pagina **Customers** selezionare il **nome della società**del cliente.</span><span class="sxs-lookup"><span data-stu-id="dbb19-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="dbb19-166">Nella pagina **sottoscrizioni** del cliente, in **sottoscrizioni basate sull'utilizzo**, selezionare il nome della **sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="dbb19-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="dbb19-167">Nella pagina della sottoscrizione è possibile esaminare i **costi** in base al servizio e l' **utilizzo stimato** per il mese corrente.</span><span class="sxs-lookup"><span data-stu-id="dbb19-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
