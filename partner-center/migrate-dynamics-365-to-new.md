---
title: Eseguire la migrazione di Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come eseguire la migrazione delle offerte Dynamics 365 Business Edition qualificate a versioni più recenti prima della scadenza.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436830"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="60f08-103">Eseguire la migrazione delle offerte di Dynamics 365 Business Edition a versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="60f08-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="60f08-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="60f08-104">**Applies to**</span></span>

- <span data-ttu-id="60f08-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="60f08-105">Partner Center</span></span>

<span data-ttu-id="60f08-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="60f08-106">**Appropriate roles**</span></span>
- <span data-ttu-id="60f08-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="60f08-107">Global admin</span></span>
- <span data-ttu-id="60f08-108">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="60f08-108">User admin</span></span>
- <span data-ttu-id="60f08-109">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="60f08-109">Admin agent</span></span>
- <span data-ttu-id="60f08-110">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="60f08-110">Sales agent</span></span>

<span data-ttu-id="60f08-111">A partire dal 1 ° gennaio 2019, i clienti con sottoscrizioni Dynamics 365 Business Edition non possono più rinnovarsi nelle offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="60f08-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="60f08-112">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="60f08-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="60f08-113">Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="60f08-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="60f08-114">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="60f08-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="60f08-115">Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="60f08-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="60f08-116">Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="60f08-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="60f08-117">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="60f08-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="60f08-118">Le edizioni di Dynamics 365 business in fase di ritiro</span><span class="sxs-lookup"><span data-stu-id="60f08-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="60f08-119">Dynamics 365 for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="60f08-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="60f08-120">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="60f08-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="60f08-121">Dynamics Business Central: nuove offerte di Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="60f08-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="60f08-122">Grazie alle nuove offerte di Dynamics Business Central, i clienti possono connettere i propri finanziari, le vendite, il servizio e le operazioni per semplificare i processi aziendali, migliorare le interazioni dei clienti e prendere decisioni migliori.</span><span class="sxs-lookup"><span data-stu-id="60f08-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="60f08-123">Dynamics 365 business Central è basato sul cloud e disponibile solo per i partner di programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="60f08-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="60f08-124">I clienti di Dynamics 365 Business Edition sono idonei a ricevere prezzi di transizione scontati per le nuove offerte business Central fino al 30 giugno 2020.</span><span class="sxs-lookup"><span data-stu-id="60f08-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="60f08-125">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="60f08-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="60f08-126">Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="60f08-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="60f08-127">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="60f08-127">Purchase the new subscription</span></span>
- <span data-ttu-id="60f08-128">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="60f08-128">Reassign current user licenses</span></span>
- <span data-ttu-id="60f08-129">Annulla sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="60f08-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="60f08-130">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="60f08-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="60f08-131">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="60f08-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="60f08-132">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="60f08-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="60f08-133">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="60f08-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="60f08-134">Il cliente avrà ora la sottoscrizione precedente e quella nuova.</span><span class="sxs-lookup"><span data-stu-id="60f08-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="60f08-135">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="60f08-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="60f08-136">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="60f08-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="60f08-137">Selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="60f08-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="60f08-138">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="60f08-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="60f08-139">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="60f08-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="60f08-140">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="60f08-140">Select **Submit**.</span></span> <span data-ttu-id="60f08-141">Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="60f08-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="60f08-142">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="60f08-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="60f08-143">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="60f08-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="60f08-144">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="60f08-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="60f08-145">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="60f08-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="60f08-146">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="60f08-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="60f08-147">Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="60f08-147">Your customer will incur no additional costs for the old subscription.</span></span>
