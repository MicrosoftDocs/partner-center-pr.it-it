---
title: Eseguire la migrazione delle offerte di Dynamics 365 Business Edition alle versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione delle offerte di Dynamics 365 Business Edition a versioni più recenti prima della scadenza.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, Renew offers, New Dynamics 365 SKU
ms.openlocfilehash: d4efd051b4d237eac5b766ed1aedc432e8b93ecc
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005120"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="34873-104">Eseguire la migrazione edizione di Dynamics 365 Business offre alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="34873-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span> 

<span data-ttu-id="34873-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="34873-105">**Applies to**</span></span>

- <span data-ttu-id="34873-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="34873-106">Partner Center</span></span>

<span data-ttu-id="34873-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="34873-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="34873-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="34873-108">Global admin</span></span>
-   <span data-ttu-id="34873-109">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="34873-109">User admin</span></span>
-   <span data-ttu-id="34873-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="34873-110">Admin agent</span></span>
-   <span data-ttu-id="34873-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="34873-111">Sales agent</span></span>

<span data-ttu-id="34873-112">A partire dal 1 ° gennaio 2019, i clienti con sottoscrizioni Dynamics 365 Business Edition non possono più rinnovarsi nelle offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="34873-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="34873-113">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="34873-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="34873-114">Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="34873-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="34873-115">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="34873-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="34873-116">Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="34873-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="34873-117">Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="34873-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="34873-118">È possibile trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="34873-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="34873-119">Le edizioni di Dynamics 365 business in fase di ritiro</span><span class="sxs-lookup"><span data-stu-id="34873-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="34873-120">Dynamics 365 for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="34873-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="34873-121">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="34873-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="34873-122">Dynamics Business Central: nuove offerte di Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="34873-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="34873-123">Grazie alle nuove offerte di Dynamics Business Central, i clienti possono connettere i propri finanziari, le vendite, il servizio e le operazioni per semplificare i processi aziendali, migliorare le interazioni dei clienti e prendere decisioni migliori.</span><span class="sxs-lookup"><span data-stu-id="34873-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="34873-124">Dynamics 365 business Central è basato sul cloud e disponibile solo per i partner di programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="34873-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="34873-125">I clienti di Dynamics 365 Business Edition sono idonei a ricevere prezzi di transizione scontati per le nuove offerte business Central fino al 30 giugno 2020.</span><span class="sxs-lookup"><span data-stu-id="34873-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="34873-126">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="34873-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="34873-127">Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="34873-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="34873-128">Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="34873-128">Purchase the new subscription</span></span>
- <span data-ttu-id="34873-129">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="34873-129">Reassign current user licenses</span></span>
- <span data-ttu-id="34873-130">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="34873-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="34873-131">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="34873-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="34873-132">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="34873-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="34873-133">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="34873-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="34873-134">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="34873-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="34873-135">Il cliente avrà ora la sottoscrizione precedente e quella nuova.</span><span class="sxs-lookup"><span data-stu-id="34873-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="34873-136">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="34873-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="34873-137">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="34873-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="34873-138">Seleziona **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="34873-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="34873-139">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="34873-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="34873-140">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="34873-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="34873-141">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="34873-141">Select **Submit**.</span></span> <span data-ttu-id="34873-142">Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="34873-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="34873-143">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="34873-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="34873-144">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="34873-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="34873-145">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="34873-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="34873-146">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="34873-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="34873-147">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="34873-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="34873-148">Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="34873-148">Your customer will incur no additional costs for the old subscription.</span></span>
