---
title: Impostare un budget di spesa di Azure per i clienti
ms.topic: how-to
ms.date: 03/17/2021
description: Informazioni su come impostare o rimuovere budget mensili di spesa di Azure per i clienti, visualizzare i dati di spesa di Azure e impostare notifiche correlate al budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855353"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="04cce-103">Impostare, controllare o rimuovere i budget di spesa mensili di Azure per i clienti in Partner Center</span><span class="sxs-lookup"><span data-stu-id="04cce-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="04cce-104">**Ruoli appropriati:** Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="04cce-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="04cce-105">È possibile [impostare un budget di spesa mensile di Azure per i clienti](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="04cce-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="04cce-106">Ciò consente ai clienti di gestire la spesa di Azure.</span><span class="sxs-lookup"><span data-stu-id="04cce-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="04cce-107">Questa opzione consente di confrontare la spesa di Azure dei clienti con il budget durante il mese.</span><span class="sxs-lookup"><span data-stu-id="04cce-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="04cce-108">Consente inoltre ai clienti di bilanciare la spesa di Azure in modo che la fattura mensile non sia superiore a quanto previsto.</span><span class="sxs-lookup"><span data-stu-id="04cce-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="04cce-109">Questa funzionalità non è disponibile negli account sandbox o Test in produzione (TIP).</span><span class="sxs-lookup"><span data-stu-id="04cce-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="04cce-110">Dopo aver [impostato un budget di spesa di Azure per](#set-azure-spending-budget)i clienti, è anche possibile esaminare l'utilizzo dei clienti nei modi seguenti.</span><span class="sxs-lookup"><span data-stu-id="04cce-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="04cce-111">Queste opzioni consentono di individuare servizi non configurati correttamente o tendenze insolite che potrebbero suggerire frodi.</span><span class="sxs-lookup"><span data-stu-id="04cce-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="04cce-112">È quindi possibile collaborare con i clienti per identificare la causa radice e gestire i costi.</span><span class="sxs-lookup"><span data-stu-id="04cce-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="04cce-113">Se necessario, è anche possibile [modificare il budget del cliente](#set-azure-spending-budget) in un importo superiore.</span><span class="sxs-lookup"><span data-stu-id="04cce-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="04cce-114">Controllare la spesa corrente di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="04cce-115">Attivare le notifiche di posta elettronica per quando la spesa di un cliente sta per essere vicina al limite di budget</span><span class="sxs-lookup"><span data-stu-id="04cce-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="04cce-116">Visualizzare i costi in base al servizio per le sottoscrizioni basate sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="04cce-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="04cce-117">È anche possibile [rimuovere un budget di spesa di Azure](#remove-azure-spending-budget) per i clienti in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="04cce-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="04cce-118">Dati di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-118">Azure spending data</span></span>

<span data-ttu-id="04cce-119">I dati di spesa di Azure sono una *stima e* gli importi di fatturazione effettivi *possono variare.*</span><span class="sxs-lookup"><span data-stu-id="04cce-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="04cce-120">Il valore dei dati *non riflette* le imposte, i crediti, le rettifiche o altri addebiti applicabili.</span><span class="sxs-lookup"><span data-stu-id="04cce-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="04cce-121">I dati di spesa *vengono aggiornati una volta al giorno.*</span><span class="sxs-lookup"><span data-stu-id="04cce-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="04cce-122">I clienti possono continuare a usare (e addebitare) i servizi e le risorse di Azure, a meno che non si cambino le impostazioni dell'account nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="04cce-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="04cce-123">Impostare il budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-123">Set Azure spending budget</span></span>

<span data-ttu-id="04cce-124">È possibile *impostare un budget di spesa mensile di Azure* per più clienti in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="04cce-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="04cce-125">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="04cce-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="04cce-126">Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**</span><span class="sxs-lookup"><span data-stu-id="04cce-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="04cce-127">Nella pagina Di spesa di **Azure,** in Clienti **con Microsoft Azure sottoscrizioni**, selezionare i clienti per cui si vuole impostare un budget.</span><span class="sxs-lookup"><span data-stu-id="04cce-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="04cce-128">Immettere un valore per **Budget mensile.**</span><span class="sxs-lookup"><span data-stu-id="04cce-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="04cce-129">Scegliere **Applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="04cce-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="04cce-130">È anche possibile *impostare un budget per un singolo cliente nelle* impostazioni di sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="04cce-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="04cce-131">Accedere al dashboard Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="04cce-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="04cce-132">Nel menu a sinistra in **CSP** scegliere **Clienti.**</span><span class="sxs-lookup"><span data-stu-id="04cce-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="04cce-133">Nella pagina **Clienti** selezionare il nome società **del cliente.**</span><span class="sxs-lookup"><span data-stu-id="04cce-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="04cce-134">Nella pagina Sottoscrizioni **del** cliente, in **Sottoscrizione basata sull'utilizzo** scegliere **Modifica budget.**</span><span class="sxs-lookup"><span data-stu-id="04cce-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="04cce-135">Immettere un valore per il budget.</span><span class="sxs-lookup"><span data-stu-id="04cce-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="04cce-136">Scegliere **Applica** per salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="04cce-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="04cce-137">Rimuovere il budget di spesa di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-137">Remove Azure spending budget</span></span>

<span data-ttu-id="04cce-138">È possibile *rimuovere un budget di spesa mensile* di Azure per i clienti in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="04cce-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="04cce-139">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="04cce-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="04cce-140">Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**</span><span class="sxs-lookup"><span data-stu-id="04cce-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="04cce-141">Nella pagina Di spesa di **Azure,** in Clienti con Microsoft Azure **sottoscrizioni**, selezionare i clienti di cui si vuole rimuovere il budget.</span><span class="sxs-lookup"><span data-stu-id="04cce-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="04cce-142">Scegliere **Rimuovi budget.**</span><span class="sxs-lookup"><span data-stu-id="04cce-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="04cce-143">Controllare la spesa corrente di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-143">Check current Azure spending</span></span>

<span data-ttu-id="04cce-144">È possibile *tenere traccia delle spese correnti di Azure e dei budget mensili* dei clienti in qualsiasi momento:</span><span class="sxs-lookup"><span data-stu-id="04cce-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="04cce-145">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="04cce-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="04cce-146">Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**</span><span class="sxs-lookup"><span data-stu-id="04cce-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="04cce-147">Nella pagina **Di spesa di Azure,** **in** Clienti con sottoscrizioni Microsoft Azure , è possibile visualizzare una panoramica dei budget mensili dei clienti, delle stime di spesa correnti e della percentuale del budget usato.</span><span class="sxs-lookup"><span data-stu-id="04cce-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="04cce-148">Notifiche per i limiti del budget</span><span class="sxs-lookup"><span data-stu-id="04cce-148">Notifications for budget limits</span></span>

<span data-ttu-id="04cce-149">È possibile *attivare le notifiche tramite posta elettronica* per quando la spesa mensile del cliente sta per essere vicina al limite di budget.</span><span class="sxs-lookup"><span data-stu-id="04cce-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="04cce-150">Quando si attiva questa opzione, si riceve una notifica quando i clienti usano l'80% o più del budget mensile.</span><span class="sxs-lookup"><span data-stu-id="04cce-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="04cce-151">Questa opzione consente di tenere d'occhio la fattura di Azure.</span><span class="sxs-lookup"><span data-stu-id="04cce-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="04cce-152">Per configurare le notifiche tramite posta elettronica:</span><span class="sxs-lookup"><span data-stu-id="04cce-152">To configure email notifications:</span></span>

1. <span data-ttu-id="04cce-153">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="04cce-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="04cce-154">Passare a **Impostazioni**.</span><span class="sxs-lookup"><span data-stu-id="04cce-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="04cce-155">Selezionare **Preferenze personali**.</span><span class="sxs-lookup"><span data-stu-id="04cce-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="04cce-156">Se non è stato fatto, configurare un indirizzo di posta elettronica preferito.</span><span class="sxs-lookup"><span data-stu-id="04cce-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="04cce-157">Configurare la lingua preferita per la notifica.</span><span class="sxs-lookup"><span data-stu-id="04cce-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="04cce-158">Selezionare **la scheda CSP** nella **sezione Preferenze di** notifica.</span><span class="sxs-lookup"><span data-stu-id="04cce-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="04cce-159">Selezionare l'opzione Posta elettronica per **Notifica di spesa** di Azure e **Salva**.</span><span class="sxs-lookup"><span data-stu-id="04cce-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="04cce-160">Costi in base al servizio</span><span class="sxs-lookup"><span data-stu-id="04cce-160">Itemized costs by service</span></span>

<span data-ttu-id="04cce-161">È possibile *visualizzare i costi (e l'utilizzo stimato) in base al servizio per le sottoscrizioni basate sull'utilizzo:*</span><span class="sxs-lookup"><span data-stu-id="04cce-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="04cce-162">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="04cce-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="04cce-163">Nel menu a sinistra in **CSP** scegliere **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="04cce-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="04cce-164">Nella pagina **Clienti** selezionare il nome della società **del cliente.**</span><span class="sxs-lookup"><span data-stu-id="04cce-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="04cce-165">Nella pagina Sottoscrizioni **del** cliente, in **Sottoscrizioni basate sull'utilizzo,** selezionare il nome della **sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="04cce-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="04cce-166">Nella pagina della sottoscrizione è possibile esaminare i **costi** in base al servizio e l'utilizzo **stimato** per il mese corrente.</span><span class="sxs-lookup"><span data-stu-id="04cce-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="04cce-167">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="04cce-167">Next steps</span></span>

- [<span data-ttu-id="04cce-168">Nuova esperienza commerciale in CSP - Fatturazione di Azure</span><span class="sxs-lookup"><span data-stu-id="04cce-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
