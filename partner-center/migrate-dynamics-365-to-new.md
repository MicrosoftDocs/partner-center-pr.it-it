---
title: Eseguire la migrazione di Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione di offerte Dynamics 365 Business Edition qualificate a versioni più recenti prima della scadenza.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151526"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="fac7b-103">Eseguire la migrazione delle offerte di Dynamics 365 Business Edition a versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="fac7b-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="fac7b-104">**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente di amministrazione | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="fac7b-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="fac7b-105">A partire dal 1° gennaio 2019, i clienti con sottoscrizioni a Dynamics 365 Business Edition non possono più rinnovare queste offerte legacy; Le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="fac7b-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="fac7b-106">Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione verrà modificato in "Scadenza [data]" da "Rinnovo automatico il [data]".</span><span class="sxs-lookup"><span data-stu-id="fac7b-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="fac7b-107">Per garantire la continuità per i clienti, è consigliabile eseguire la transizione di quelli con sottoscrizioni in scadenza a un'opzione supportata, elencata di seguito.</span><span class="sxs-lookup"><span data-stu-id="fac7b-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="fac7b-108">È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="fac7b-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="fac7b-109">Se si usa l'API (EITHER o Partner Center), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="fac7b-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="fac7b-110">Le sottoscrizioni in questione verranno impostate su auto renew=False il 1° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="fac7b-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="fac7b-111">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="fac7b-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="fac7b-112">Le edizioni di Dynamics 365 Business in fase di ritiro</span><span class="sxs-lookup"><span data-stu-id="fac7b-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="fac7b-113">Dynamics 365 for Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="fac7b-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="fac7b-114">Dynamics 365 for Team Members, Business Edition</span><span class="sxs-lookup"><span data-stu-id="fac7b-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="fac7b-115">Dynamics Business Central : nuove offerte di Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="fac7b-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="fac7b-116">Con le nuove offerte di Dynamics Business Central, i clienti possono connettere i dati finanziari, le vendite, il servizio e le operazioni per semplificare i processi aziendali, migliorare le interazioni dei clienti e prendere decisioni migliori.</span><span class="sxs-lookup"><span data-stu-id="fac7b-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="fac7b-117">Dynamics 365 Business Central è basato sul cloud e disponibile solo tramite Cloud Solution Provider partner del programma CSP.)</span><span class="sxs-lookup"><span data-stu-id="fac7b-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="fac7b-118">I clienti di Dynamics 365 Business Edition sono idonei a ricevere prezzi di transizione scontati per le nuove offerte business central fino al 30 giugno 2020.</span><span class="sxs-lookup"><span data-stu-id="fac7b-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="fac7b-119">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="fac7b-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="fac7b-120">Per spostare i clienti da SKU ritirati a SKU più recenti, è necessario eseguire i passaggi seguenti in questo ordine:</span><span class="sxs-lookup"><span data-stu-id="fac7b-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="fac7b-121">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="fac7b-121">Purchase the new subscription</span></span>
- <span data-ttu-id="fac7b-122">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="fac7b-122">Reassign current user licenses</span></span>
- <span data-ttu-id="fac7b-123">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="fac7b-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="fac7b-124">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="fac7b-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="fac7b-125">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente da spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="fac7b-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="fac7b-126">Selezionare **Aggiungi sottoscrizione.**</span><span class="sxs-lookup"><span data-stu-id="fac7b-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="fac7b-127">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="fac7b-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="fac7b-128">Il cliente avrà ora sia la sottoscrizione precedente che quella nuova.</span><span class="sxs-lookup"><span data-stu-id="fac7b-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="fac7b-129">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="fac7b-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="fac7b-130">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.</span><span class="sxs-lookup"><span data-stu-id="fac7b-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fac7b-131">Selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="fac7b-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="fac7b-132">Per riassegnare una licenza a un utente, selezionare l'utente e quindi **selezionare Gestisci licenze.**</span><span class="sxs-lookup"><span data-stu-id="fac7b-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="fac7b-133">Nella **pagina** Gestisci licenze deselezionare la casella di controllo Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Piano Dynamics 365 for Sales/Customer Engagement dalla licenza Basic - Offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente.</span><span class="sxs-lookup"><span data-stu-id="fac7b-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="fac7b-134">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="fac7b-134">Select **Submit**.</span></span> <span data-ttu-id="fac7b-135">Questa operazione verrà creata per ogni utente che necessita della nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="fac7b-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="fac7b-136">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="fac7b-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="fac7b-137">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.</span><span class="sxs-lookup"><span data-stu-id="fac7b-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fac7b-138">Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione precedente su **Sospeso e** selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="fac7b-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="fac7b-139">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="fac7b-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="fac7b-140">Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="fac7b-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="fac7b-141">Il cliente non incorrerà in costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="fac7b-141">Your customer will incur no additional costs for the old subscription.</span></span>
