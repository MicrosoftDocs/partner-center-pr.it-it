---
title: Eseguire la migrazione di sottoscrizioni Dynamics 365 qualificate
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione da sottoscrizioni di base dinamiche 365 qualificate a una nuova sottoscrizione prima della scadenza delle sottoscrizioni esistenti.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 offers, Renew offers, New Dynamics 365 SKU
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795997"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="ad464-104">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="ad464-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="ad464-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="ad464-105">**Applies to**</span></span>

-  <span data-ttu-id="ad464-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ad464-106">Partner Center</span></span>

<span data-ttu-id="ad464-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="ad464-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="ad464-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="ad464-108">Global admin</span></span>
-   <span data-ttu-id="ad464-109">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="ad464-109">User admin</span></span>
-   <span data-ttu-id="ad464-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="ad464-110">Admin agent</span></span>
-   <span data-ttu-id="ad464-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="ad464-111">Sales agent</span></span>

<span data-ttu-id="ad464-112">A partire dal 1 ° gennaio 2019, i clienti con Dynamics 365 per il piano Sales/Customer Engagement dalle sottoscrizioni Basic (offerte qualificate) non possono più rinnovare tali offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="ad464-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="ad464-113">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="ad464-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="ad464-114">Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="ad464-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="ad464-115">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="ad464-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ad464-116">Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="ad464-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="ad464-117">Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="ad464-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="ad464-118">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="ad464-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="ad464-119">Le offerte di Dynamics 365 sono state ritirate</span><span class="sxs-lookup"><span data-stu-id="ad464-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="ad464-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad464-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-123">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-124">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-125">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad464-126">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-127">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-128">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-129">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad464-130">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-131">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad464-136">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-138">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-139">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="ad464-140">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) componente aggiuntivo per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-142">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="ad464-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="ad464-143">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="ad464-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="ad464-144">Dynamics 365 per Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)</span><span class="sxs-lookup"><span data-stu-id="ad464-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="ad464-145">**Offerte ritirate**</span><span class="sxs-lookup"><span data-stu-id="ad464-145">**Retired offers**</span></span>   

- <span data-ttu-id="ad464-146">Dynamics 365 per le vendite di CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="ad464-147">Piano di engagement per i clienti di Dynamics 365 da CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="ad464-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="ad464-148">**Opzioni di sostituzione**</span><span class="sxs-lookup"><span data-stu-id="ad464-148">**Replacement options**</span></span>
- <span data-ttu-id="ad464-149">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="ad464-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ad464-150">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="ad464-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="ad464-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="ad464-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="ad464-152">Piano di coinvolgimento dei clienti di Dynamics 365 o</span><span class="sxs-lookup"><span data-stu-id="ad464-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="ad464-153">Membri del Team Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="ad464-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ad464-154">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="ad464-154">Transition customers to new product plans</span></span>

<span data-ttu-id="ad464-155">Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="ad464-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="ad464-156">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ad464-156">Purchase the new subscription</span></span>
- <span data-ttu-id="ad464-157">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="ad464-157">Reassign current user licenses</span></span>
- <span data-ttu-id="ad464-158">Annulla sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="ad464-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="ad464-159">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="ad464-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="ad464-160">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ad464-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="ad464-161">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="ad464-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="ad464-162">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="ad464-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="ad464-163">Il cliente avrà ora la sottoscrizione precedente e quella nuova.</span><span class="sxs-lookup"><span data-stu-id="ad464-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="ad464-164">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="ad464-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="ad464-165">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="ad464-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ad464-166">Selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="ad464-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="ad464-167">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="ad464-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="ad464-168">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="ad464-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="ad464-169">Selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="ad464-169">Select **Submit**.</span></span> <span data-ttu-id="ad464-170">Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="ad464-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="ad464-171">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="ad464-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="ad464-172">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="ad464-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="ad464-173">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="ad464-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="ad464-174">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="ad464-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="ad464-175">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="ad464-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ad464-176">Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="ad464-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



