---
title: Impostare un budget di spesa di Azure per i clienti
ms.topic: how-to
ms.date: 03/17/2021
description: Informazioni su come impostare o rimuovere i budget mensili per la spesa di Azure per i clienti e anche per visualizzare i dati di spesa di Azure e impostare le notifiche relative al budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712750"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="51c50-103">Imposta, verifica o Rimuovi i budget mensili per la spesa di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="51c50-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="51c50-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="51c50-104">**Appropriate roles**</span></span>

- <span data-ttu-id="51c50-105">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="51c50-105">Admin agent</span></span>

<span data-ttu-id="51c50-106">È possibile [impostare un budget mensile per la spesa di Azure per i clienti](#set-azure-spending-budget) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="51c50-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="51c50-107">Ciò consente ai clienti di gestire la spesa di Azure.</span><span class="sxs-lookup"><span data-stu-id="51c50-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="51c50-108">Questa opzione consente di confrontare la spesa di Azure da parte dei clienti al budget durante il mese.</span><span class="sxs-lookup"><span data-stu-id="51c50-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="51c50-109">Consente inoltre ai clienti di ottenere un budget per la spesa di Azure in modo che la fattura mensile non sia più elevata del previsto.</span><span class="sxs-lookup"><span data-stu-id="51c50-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="51c50-110">Questa funzionalità non è disponibile negli account sandbox o test negli ambienti di produzione (TIP).</span><span class="sxs-lookup"><span data-stu-id="51c50-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="51c50-111">Dopo aver [impostato un budget di spesa di Azure per i clienti](#set-azure-spending-budget), è anche possibile esaminare l'utilizzo dei clienti nei modi seguenti.</span><span class="sxs-lookup"><span data-stu-id="51c50-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="51c50-112">Queste opzioni possono essere utili per individuare i servizi non configurati correttamente o tendenze insolite che potrebbero suggerire frodi.</span><span class="sxs-lookup"><span data-stu-id="51c50-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="51c50-113">È quindi possibile collaborare con i clienti per identificare la causa principale e gestire i costi.</span><span class="sxs-lookup"><span data-stu-id="51c50-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="51c50-114">Se necessario, è anche possibile [modificare il budget del cliente impostando](#set-azure-spending-budget) un importo superiore.</span><span class="sxs-lookup"><span data-stu-id="51c50-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="51c50-115">Controlla la spesa di Azure corrente</span><span class="sxs-lookup"><span data-stu-id="51c50-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="51c50-116">Attivare le notifiche tramite posta elettronica quando la spesa di un cliente sta per avvicinarsi al limite di budget</span><span class="sxs-lookup"><span data-stu-id="51c50-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="51c50-117">Visualizza i costi in base al servizio per le sottoscrizioni basate sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="51c50-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="51c50-118">È anche possibile [rimuovere un budget di spesa di Azure](#remove-azure-spending-budget) per i clienti in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="51c50-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="51c50-119">Dati della spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="51c50-119">Azure spending data</span></span>

<span data-ttu-id="51c50-120">I dati di spesa di Azure sono una *stima* e gli *importi di fatturazione effettivi possono variare*.</span><span class="sxs-lookup"><span data-stu-id="51c50-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="51c50-121">Il valore dei dati *non riflette* tasse, crediti, rettifiche o altri addebiti che possono essere applicati.</span><span class="sxs-lookup"><span data-stu-id="51c50-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="51c50-122">I dati di spesa vengono *aggiornati una volta al giorno*.</span><span class="sxs-lookup"><span data-stu-id="51c50-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="51c50-123">I clienti possono continuare a usare i servizi e le risorse di Azure, a meno che non si modifichino le impostazioni dell'account nella portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="51c50-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="51c50-124">Imposta budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="51c50-124">Set Azure spending budget</span></span>

<span data-ttu-id="51c50-125">È possibile *impostare un budget mensile per la spesa di Azure* per più clienti nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="51c50-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="51c50-126">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="51c50-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="51c50-127">Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="51c50-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="51c50-128">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti per i quali si desidera impostare un budget.</span><span class="sxs-lookup"><span data-stu-id="51c50-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="51c50-129">Immettere un valore per **budget mensile**.</span><span class="sxs-lookup"><span data-stu-id="51c50-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="51c50-130">Scegliere **applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="51c50-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="51c50-131">È anche possibile *impostare un budget per un singolo cliente* nelle impostazioni della sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="51c50-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="51c50-132">Accedere al dashboard Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="51c50-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="51c50-133">Nel menu a sinistra in **CSP** scegliere **Customers (clienti**).</span><span class="sxs-lookup"><span data-stu-id="51c50-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="51c50-134">Nella pagina **Customers** selezionare il **nome della società** del cliente.</span><span class="sxs-lookup"><span data-stu-id="51c50-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="51c50-135">Nella pagina **sottoscrizioni** del cliente, in **sottoscrizione basata sull'utilizzo**, scegliere **Cambia budget**.</span><span class="sxs-lookup"><span data-stu-id="51c50-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="51c50-136">Immettere un valore per il budget.</span><span class="sxs-lookup"><span data-stu-id="51c50-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="51c50-137">Scegliere **applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="51c50-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="51c50-138">Rimuovi budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="51c50-138">Remove Azure spending budget</span></span>

<span data-ttu-id="51c50-139">È possibile *rimuovere un budget mensile* per la spesa di Azure per i clienti nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="51c50-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="51c50-140">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="51c50-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="51c50-141">Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="51c50-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="51c50-142">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti di cui si desidera rimuovere il budget.</span><span class="sxs-lookup"><span data-stu-id="51c50-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="51c50-143">Scegliere **Rimuovi budget**.</span><span class="sxs-lookup"><span data-stu-id="51c50-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="51c50-144">Controlla la spesa di Azure corrente</span><span class="sxs-lookup"><span data-stu-id="51c50-144">Check current Azure spending</span></span>

<span data-ttu-id="51c50-145">Puoi *tenere traccia delle spese di Azure correnti e dei budget mensili dei clienti* in qualsiasi momento:</span><span class="sxs-lookup"><span data-stu-id="51c50-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="51c50-146">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="51c50-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="51c50-147">Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.</span><span class="sxs-lookup"><span data-stu-id="51c50-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="51c50-148">Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, è possibile visualizzare una panoramica dei budget mensili dei clienti, le stime di spesa correnti e la percentuale del budget usato.</span><span class="sxs-lookup"><span data-stu-id="51c50-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="51c50-149">Notifiche per i limiti del budget</span><span class="sxs-lookup"><span data-stu-id="51c50-149">Notifications for budget limits</span></span>

<span data-ttu-id="51c50-150">È possibile *attivare le notifiche tramite posta elettronica* quando la spesa mensile del cliente si avvicina al limite di budget.</span><span class="sxs-lookup"><span data-stu-id="51c50-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="51c50-151">Quando si attiva questa opzione, si riceverà una notifica quando i clienti usano il 80% o più del budget mensile.</span><span class="sxs-lookup"><span data-stu-id="51c50-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="51c50-152">Questa opzione consente di tenere sotto controllo la fattura di Azure.</span><span class="sxs-lookup"><span data-stu-id="51c50-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="51c50-153">Per configurare le notifiche di posta elettronica:</span><span class="sxs-lookup"><span data-stu-id="51c50-153">To configure email notifications:</span></span>

1. <span data-ttu-id="51c50-154">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="51c50-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="51c50-155">Passare a **Impostazioni**.</span><span class="sxs-lookup"><span data-stu-id="51c50-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="51c50-156">Selezionare **preferenze personali**.</span><span class="sxs-lookup"><span data-stu-id="51c50-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="51c50-157">Se non è possibile, configurare un indirizzo di posta elettronica preferito.</span><span class="sxs-lookup"><span data-stu-id="51c50-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="51c50-158">Configurare la lingua preferita per la notifica.</span><span class="sxs-lookup"><span data-stu-id="51c50-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="51c50-159">Selezionare la scheda **CSP** nella sezione **Preferenze di notifica** .</span><span class="sxs-lookup"><span data-stu-id="51c50-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="51c50-160">Controllare l'opzione di posta elettronica per la notifica di **spesa di Azure** e **salvare**.</span><span class="sxs-lookup"><span data-stu-id="51c50-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="51c50-161">Costi in base al servizio</span><span class="sxs-lookup"><span data-stu-id="51c50-161">Itemized costs by service</span></span>

<span data-ttu-id="51c50-162">È possibile *visualizzare i costi (e l'utilizzo stimato) per servizio per le sottoscrizioni basate sull'utilizzo*:</span><span class="sxs-lookup"><span data-stu-id="51c50-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="51c50-163">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="51c50-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="51c50-164">Nel menu a sinistra in **CSP** scegliere **Customers (clienti**).</span><span class="sxs-lookup"><span data-stu-id="51c50-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="51c50-165">Nella pagina **Customers** selezionare il **nome della società** del cliente.</span><span class="sxs-lookup"><span data-stu-id="51c50-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="51c50-166">Nella pagina **sottoscrizioni** del cliente, in **sottoscrizioni basate sull'utilizzo**, selezionare il nome della **sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="51c50-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="51c50-167">Nella pagina della sottoscrizione è possibile esaminare i **costi** in base al servizio e l' **utilizzo stimato** per il mese corrente.</span><span class="sxs-lookup"><span data-stu-id="51c50-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="51c50-168">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="51c50-168">Next steps</span></span>

- [<span data-ttu-id="51c50-169">Nuova esperienza commerciale in CSP - Fatturazione di Azure</span><span class="sxs-lookup"><span data-stu-id="51c50-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
