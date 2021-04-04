---
title: Eseguire la migrazione di sottoscrizioni Dynamics 365 qualificate
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione da sottoscrizioni di base dinamiche 365 qualificate a una nuova sottoscrizione prima della scadenza delle sottoscrizioni esistenti.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132741"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="c844a-103">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="c844a-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="c844a-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="c844a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c844a-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c844a-105">Global admin</span></span>
- <span data-ttu-id="c844a-106">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="c844a-106">User management admin</span></span>
- <span data-ttu-id="c844a-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="c844a-107">Admin agent</span></span>
- <span data-ttu-id="c844a-108">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c844a-108">Sales agent</span></span>

<span data-ttu-id="c844a-109">A partire dal 1 ° gennaio 2019, i clienti con Dynamics 365 per il piano Sales/Customer Engagement dalle sottoscrizioni Basic (offerte qualificate) non possono più rinnovare tali offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="c844a-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="c844a-110">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="c844a-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="c844a-111">Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="c844a-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="c844a-112">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="c844a-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c844a-113">Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="c844a-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="c844a-114">Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="c844a-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="c844a-115">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="c844a-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="c844a-116">Le offerte di Dynamics 365 sono state ritirate</span><span class="sxs-lookup"><span data-stu-id="c844a-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="c844a-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c844a-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-120">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-121">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-122">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c844a-123">Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-124">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-125">Dynamics 365 for Sales Enterprise Edition Add-On per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-126">Dynamics 365 for Sales Enterprise Edition Add-On per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c844a-127">Dynamics 365 for Sales Enterprise Edition Add-On per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-128">Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) Add-On per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c844a-133">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-135">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-136">Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c844a-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) Add-On per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On per CRM Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c844a-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c844a-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On per CRM Basic (offerta qualificata) per i docenti</span><span class="sxs-lookup"><span data-stu-id="c844a-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="c844a-141">Dynamics 365 per Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)</span><span class="sxs-lookup"><span data-stu-id="c844a-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="c844a-142">**Offerte ritirate**</span><span class="sxs-lookup"><span data-stu-id="c844a-142">**Retired offers**</span></span>   

- <span data-ttu-id="c844a-143">Dynamics 365 per le vendite di CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c844a-144">Piano di engagement per i clienti di Dynamics 365 da CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c844a-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="c844a-145">**Opzioni di sostituzione**</span><span class="sxs-lookup"><span data-stu-id="c844a-145">**Replacement options**</span></span>
- <span data-ttu-id="c844a-146">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="c844a-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="c844a-147">Dynamics 365 per Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="c844a-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="c844a-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="c844a-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="c844a-149">Piano di coinvolgimento dei clienti di Dynamics 365 o</span><span class="sxs-lookup"><span data-stu-id="c844a-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="c844a-150">Membri del Team Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c844a-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c844a-151">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="c844a-151">Transition customers to new product plans</span></span>

<span data-ttu-id="c844a-152">Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="c844a-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="c844a-153">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c844a-153">Purchase the new subscription</span></span>
- <span data-ttu-id="c844a-154">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="c844a-154">Reassign current user licenses</span></span>
- <span data-ttu-id="c844a-155">Annulla sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="c844a-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="c844a-156">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="c844a-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="c844a-157">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c844a-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="c844a-158">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="c844a-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="c844a-159">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="c844a-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="c844a-160">Il cliente avrà ora la sottoscrizione precedente e quella nuova.</span><span class="sxs-lookup"><span data-stu-id="c844a-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="c844a-161">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="c844a-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="c844a-162">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="c844a-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c844a-163">Selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="c844a-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="c844a-164">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="c844a-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="c844a-165">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="c844a-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="c844a-166">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="c844a-166">Select **Submit**.</span></span> <span data-ttu-id="c844a-167">Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="c844a-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="c844a-168">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="c844a-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="c844a-169">Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.</span><span class="sxs-lookup"><span data-stu-id="c844a-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c844a-170">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="c844a-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="c844a-171">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="c844a-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="c844a-172">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="c844a-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c844a-173">Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="c844a-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



