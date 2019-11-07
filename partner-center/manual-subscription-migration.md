---
title: Eseguire la migrazione di Dynamics 365 e del piano Customer Engagement da Basic (offerte qualificate) a versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Non è più possibile rinnovare il piano Dynamics 365 per Sales/Customer Engagement da sottoscrizioni di base (offerte qualificate).
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, Renew offers, New Dynamics 365 SKU
ms.openlocfilehash: 354846973227fd292514454dd6f648934e5156ef
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653303"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="d593f-104">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="d593f-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="d593f-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="d593f-105">**Applies to**</span></span>

-  <span data-ttu-id="d593f-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d593f-106">Partner Center</span></span>

<span data-ttu-id="d593f-107">A partire dal 1 ° gennaio 2019, i clienti con Dynamics 365 per il piano Sales/Customer Engagement dalle sottoscrizioni Basic (offerte qualificate) non possono più rinnovare tali offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="d593f-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="d593f-108">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="d593f-108">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="d593f-109">Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="d593f-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="d593f-110">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="d593f-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d593f-111">Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="d593f-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="d593f-112">Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="d593f-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="d593f-113">È possibile trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="d593f-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="d593f-114">Le offerte di Dynamics 365 sono state ritirate</span><span class="sxs-lookup"><span data-stu-id="d593f-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="d593f-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d593f-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-118">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-119">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-120">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d593f-121">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-122">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-123">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-124">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d593f-125">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-126">Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d593f-131">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-133">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-134">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d593f-135">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) componente aggiuntivo per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-137">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="d593f-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d593f-138">Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="d593f-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="d593f-139">Dynamics 365 per Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)</span><span class="sxs-lookup"><span data-stu-id="d593f-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="d593f-140">**Offerte ritirate**</span><span class="sxs-lookup"><span data-stu-id="d593f-140">**Retired offers**</span></span>   

- <span data-ttu-id="d593f-141">Dynamics 365 per le vendite di CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d593f-142">Piano di engagement per i clienti di Dynamics 365 da CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="d593f-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="d593f-143">**Opzioni di sostituzione**</span><span class="sxs-lookup"><span data-stu-id="d593f-143">**Replacement options**</span></span>
- <span data-ttu-id="d593f-144">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="d593f-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d593f-145">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="d593f-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d593f-146">Dynamics 365 per il servizio clienti</span><span class="sxs-lookup"><span data-stu-id="d593f-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="d593f-147">Piano di coinvolgimento dei clienti di Dynamics 365 o</span><span class="sxs-lookup"><span data-stu-id="d593f-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="d593f-148">Membri del Team Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d593f-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d593f-149">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="d593f-149">Transition customers to new product plans</span></span>

<span data-ttu-id="d593f-150">Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="d593f-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="d593f-151">Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="d593f-151">Purchase the new subscription</span></span>
- <span data-ttu-id="d593f-152">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="d593f-152">Reassign current user licenses</span></span>
- <span data-ttu-id="d593f-153">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="d593f-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="d593f-154">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="d593f-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="d593f-155">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d593f-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="d593f-156">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="d593f-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="d593f-157">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="d593f-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="d593f-158">Il cliente avrà ora la sottoscrizione precedente e quella nuova.</span><span class="sxs-lookup"><span data-stu-id="d593f-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="d593f-159">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="d593f-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="d593f-160">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="d593f-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d593f-161">Seleziona **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="d593f-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="d593f-162">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="d593f-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="d593f-163">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="d593f-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="d593f-164">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="d593f-164">Select **Submit**.</span></span> <span data-ttu-id="d593f-165">Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="d593f-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="d593f-166">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="d593f-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="d593f-167">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="d593f-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d593f-168">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="d593f-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="d593f-169">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="d593f-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="d593f-170">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="d593f-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d593f-171">Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="d593f-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



