---
title: Imposizione del limite di credito
ms.topic: how-to
ms.date: 05/11/2021
description: Informazioni sul limite di credito e su come viene calcolato. Include domande frequenti.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148109"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="704fd-104">Imposizione del limite di credito (CLE)</span><span class="sxs-lookup"><span data-stu-id="704fd-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="704fd-105">**Ruoli appropriati:** amministratore della fatturazione</span><span class="sxs-lookup"><span data-stu-id="704fd-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="704fd-106">Limite di credito e funzionamento</span><span class="sxs-lookup"><span data-stu-id="704fd-106">Your credit limit and how it works</span></span>

<span data-ttu-id="704fd-107">Il limite di credito è l'importo massimo (in dollari STATUNITENSI) che il partner può spendere per acquistare prodotti o sottoscrizioni in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="704fd-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="704fd-108">Se si supera il limite di credito, non sarà possibile effettuare nuovi acquisti fino a quando non viene effettuato un pagamento sufficiente.</span><span class="sxs-lookup"><span data-stu-id="704fd-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="704fd-109">Le sottoscrizioni esistenti continueranno senza interruzioni.</span><span class="sxs-lookup"><span data-stu-id="704fd-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="704fd-110">I limiti di credito si applicano alle offerte nei prodotti Piano di Azure, Prenotazioni di Azure, Software, Marketplace, Azure 145 P, Office e Dynamics.</span><span class="sxs-lookup"><span data-stu-id="704fd-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="704fd-111">I limiti di credito non si applicano ai rinnovi e al consumo in corso.</span><span class="sxs-lookup"><span data-stu-id="704fd-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="704fd-112">Il limite di credito viene assegnato a livello di tenant durante il periodo di onboarding.</span><span class="sxs-lookup"><span data-stu-id="704fd-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="704fd-113">Si basa sui ricavi previsti, sulle prodeghe di acquisto e sulla cronologia dei pagamenti.</span><span class="sxs-lookup"><span data-stu-id="704fd-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="704fd-114">Viene quindi utilizzata la formula seguente per calcolare il saldo disponibile:</span><span class="sxs-lookup"><span data-stu-id="704fd-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="704fd-115">**[Limite di credito : (Acquisto in entrata + Fatture non pagate in sospeso + Addebiti non fatturati - Eccedenza pagamento)]**</span><span class="sxs-lookup"><span data-stu-id="704fd-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="704fd-116">Domande frequenti</span><span class="sxs-lookup"><span data-stu-id="704fd-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="704fd-117">Il limite di credito è impostato a livello tenant o globale?</span><span class="sxs-lookup"><span data-stu-id="704fd-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="704fd-118">Livello del tenant.</span><span class="sxs-lookup"><span data-stu-id="704fd-118">The tenant level.</span></span> <span data-ttu-id="704fd-119">Si supponga, ad esempio, di operare da Stati Uniti, Canada e Giappone.</span><span class="sxs-lookup"><span data-stu-id="704fd-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="704fd-120">Se il tenant canadese raggiunge il limite di credito, il tenant riceverà una notifica quando tenterà di effettuare un acquisto Partner Center.</span><span class="sxs-lookup"><span data-stu-id="704fd-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="704fd-121">Gli altri tenant non saranno interessati.</span><span class="sxs-lookup"><span data-stu-id="704fd-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="704fd-122">Se si supera il limite di credito, è possibile continuare a usare i clienti e le sottoscrizioni esistenti con accesso completo?</span><span class="sxs-lookup"><span data-stu-id="704fd-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="704fd-123">Sì.</span><span class="sxs-lookup"><span data-stu-id="704fd-123">Yes.</span></span> <span data-ttu-id="704fd-124">Le sottoscrizioni esistenti dei clienti continueranno senza interruzioni.</span><span class="sxs-lookup"><span data-stu-id="704fd-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="704fd-125">Non è tuttavia possibile acquistare nuove sottoscrizioni per i clienti.</span><span class="sxs-lookup"><span data-stu-id="704fd-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="704fd-126">CLE si applica sia ai partner con fatturazione diretta che ai provider indiretti?</span><span class="sxs-lookup"><span data-stu-id="704fd-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="704fd-127">Sì, si applica a entrambi.</span><span class="sxs-lookup"><span data-stu-id="704fd-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="704fd-128">Dopo aver inviato il pagamento per ripristinare l'account, quando è possibile acquistare altre sottoscrizioni?</span><span class="sxs-lookup"><span data-stu-id="704fd-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="704fd-129">Dovrebbe essere possibile riprendere l'acquisto entro 24 ore dal pagamento, presupponendo che Microsoft abbia ricevuto tutti i requisiti per procedere con il processo di verifica del credito.</span><span class="sxs-lookup"><span data-stu-id="704fd-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="704fd-130">Come è possibile controllare il limite di credito?</span><span class="sxs-lookup"><span data-stu-id="704fd-130">How can I check my credit limit?</span></span>

<span data-ttu-id="704fd-131">Contattare [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) per visualizzare il limite di credito e ottenere informazioni sugli acquisti recenti.</span><span class="sxs-lookup"><span data-stu-id="704fd-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="704fd-132">Le fatture in conflitto vengono conteggiata rispetto al limite di credito?</span><span class="sxs-lookup"><span data-stu-id="704fd-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="704fd-133">Sì.</span><span class="sxs-lookup"><span data-stu-id="704fd-133">Yes.</span></span> <span data-ttu-id="704fd-134">È tuttavia possibile contattare Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) all'indirizzo per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="704fd-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="704fd-135">Quanto tempo verrà visualizzato se si scrive in ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="704fd-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="704fd-136">Si dovrebbe avere una risposta in meno di 24 ore.</span><span class="sxs-lookup"><span data-stu-id="704fd-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="704fd-137">Quali criteri vengono utilizzati da Microsoft per impostare il limite di credito di un partner?</span><span class="sxs-lookup"><span data-stu-id="704fd-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="704fd-138">Il limite di credito viene determinato in base ai ricavi previsti, alle prodeghe di acquisto e alla cronologia dei pagamenti.</span><span class="sxs-lookup"><span data-stu-id="704fd-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="704fd-139">Il limite di credito è attualmente applicato alla nuova esperienza commerciale?</span><span class="sxs-lookup"><span data-stu-id="704fd-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="704fd-140">Sì.</span><span class="sxs-lookup"><span data-stu-id="704fd-140">Yes.</span></span> <span data-ttu-id="704fd-141">I limiti di credito si applicano a tutti i programmi e prodotti CSP in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="704fd-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="704fd-142">Chi riceverà la notifica quando l'organizzazione sta per essere prossima al limite di credito?</span><span class="sxs-lookup"><span data-stu-id="704fd-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="704fd-143">La notifica deve essere ricevuta dal contatto finance account payable dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="704fd-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="704fd-144">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="704fd-144">Next steps</span></span>

[<span data-ttu-id="704fd-145">Nozioni di base sulla fatturazione</span><span class="sxs-lookup"><span data-stu-id="704fd-145">Billing basics</span></span>](./billing-basics.md)
