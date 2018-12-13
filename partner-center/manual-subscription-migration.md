---
title: Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Enterprise Plan dalle sottoscrizioni di base (offre qualificati) non è più può essere rinnovato.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968271"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="29a4e-103">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="29a4e-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="29a4e-104">Applies to</span></span>**

-  <span data-ttu-id="29a4e-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="29a4e-105">Partner Center</span></span>

<span data-ttu-id="29a4e-106">Effettivi 1 gennaio 2019, i clienti con Dynamics 365 for Sales / Enterprise Plan dalle sottoscrizioni di base (offre qualificati) più possibile rinnovare le offerte legacy; le sottoscrizioni esistenti non verranno rinnovati automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="29a4e-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="29a4e-107">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà a "Data di scadenza [Data]" da "Rinnovo automatico il [Data]".</span><span class="sxs-lookup"><span data-stu-id="29a4e-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="29a4e-108">Per garantire la continuità, è opportuno trasferire quelli con sottoscrizioni in scadenza a delle opzioni supportate elencati di seguito.</span><span class="sxs-lookup"><span data-stu-id="29a4e-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="29a4e-109">Ti consigliamo di far sottoscrivere ai clienti nuove sottoscrizioni prima della data di scadenza annuale della sottoscrizione, al fine di evitare eventuali interruzioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="29a4e-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="29a4e-110">Se si utilizza l'API (CREST o centro per i Partner), puoi trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme automatico = False proprietà.</span><span class="sxs-lookup"><span data-stu-id="29a4e-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="29a4e-111">Le sottoscrizioni in questione verranno impostate su auto renew = False il 1 gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="29a4e-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="29a4e-112">Puoi trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="29a4e-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="29a4e-113">Il Dynamics 365 offre viene ritirato</span><span class="sxs-lookup"><span data-stu-id="29a4e-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="29a4e-114">Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-115">Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29a4e-116">Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (offerta qualificato) per studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-117">Dynamics 365 per la vendita Enterprise Edition (enti pubblici sui prezzi) CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-118">Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-119">Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29a4e-120">Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (offerta qualificato) per studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-121">Dynamics 365 per la vendita Enterprise Edition (enti pubblici sui prezzi) da SA per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-122">Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-123">Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29a4e-124">Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (offerta qualificato) per studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-125">Dynamics 365 per componente aggiuntivo di vendita Enterprise Edition (enti pubblici sui prezzi) per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-126">Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-127">Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-128">Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (offerta qualificato) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-129">Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29a4e-130">Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-131">Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) da SA per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-132">Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (offerta qualificato) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-133">Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="29a4e-134">Dynamics 365 cliente Engagement piano Enterprise Edition un componente aggiuntivo per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-135">Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) un componente aggiuntivo per Basic CRM (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-136">Dynamics 365 Customer coinvolgimento piano Enterprise Edition un componente aggiuntivo per Basic CRM (offerta qualificato) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="29a4e-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="29a4e-137">Dynamics 365 Customer coinvolgimento piano Enterprise Edition un componente aggiuntivo per Basic CRM (offerta qualificato) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="29a4e-138">Dynamics 365 for Sales / Enterprise Plan da sostituzione Basic (offre qualificati) piani</span><span class="sxs-lookup"><span data-stu-id="29a4e-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="29a4e-139">Offerte ritirate</span><span class="sxs-lookup"><span data-stu-id="29a4e-139">Retired offers</span></span>**   

- <span data-ttu-id="29a4e-140">Dynamics 365 for Sales da CRM Basic o CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="29a4e-141">Piano Dynamics 365 Customer Engagement da CRM Basic o CRMOL Basic (qualificato offerta)</span><span class="sxs-lookup"><span data-stu-id="29a4e-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="29a4e-142">Opzioni di sostituzione</span><span class="sxs-lookup"><span data-stu-id="29a4e-142">Replacement options</span></span>**
- <span data-ttu-id="29a4e-143">Dynamics 365 per la vendita Professional (novità)</span><span class="sxs-lookup"><span data-stu-id="29a4e-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="29a4e-144">Dynamics 365 per la vendita Professional (novità)</span><span class="sxs-lookup"><span data-stu-id="29a4e-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="29a4e-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="29a4e-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="29a4e-146">Piano Dynamics 365 Customer Engagement oppure</span><span class="sxs-lookup"><span data-stu-id="29a4e-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="29a4e-147">Membri del Team Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="29a4e-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="29a4e-148">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="29a4e-148">Transition customers to new product plans</span></span>

<span data-ttu-id="29a4e-149">Spostare i clienti da SKU ritirati a quelli più recenti richiede la procedura seguente in questo ordine:</span><span class="sxs-lookup"><span data-stu-id="29a4e-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="29a4e-150">Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="29a4e-150">Purchase the new subscription</span></span>
- <span data-ttu-id="29a4e-151">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="29a4e-151">Reassign current user licenses</span></span>
- <span data-ttu-id="29a4e-152">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="29a4e-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="29a4e-153">Il nuovo piano di acquisto per il cliente</span><span class="sxs-lookup"><span data-stu-id="29a4e-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="29a4e-154">Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente da trasferire alla nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="29a4e-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="29a4e-155">Seleziona **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="29a4e-156">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="29a4e-157">Il cliente verrà ora avere sia la sottoscrizione precedente e quello nuovo.</span><span class="sxs-lookup"><span data-stu-id="29a4e-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="29a4e-158">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="29a4e-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="29a4e-159">Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.</span><span class="sxs-lookup"><span data-stu-id="29a4e-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="29a4e-160">Seleziona **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="29a4e-161">Per riassegnare una licenza a un utente, seleziona l'utente e quindi seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="29a4e-162">Nella pagina **Gestisci licenze** , cancellare il Dynamics 365 for Sales / piano di coinvolgimento dei clienti da Basic (offrire qualificati) casella di controllo della licenza e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente.</span><span class="sxs-lookup"><span data-stu-id="29a4e-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="29a4e-163">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-163">Select **Submit**.</span></span> <span data-ttu-id="29a4e-164">Lo farai per ogni utente che richiede la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="29a4e-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="29a4e-165">Dopo avere spostato le licenze alla nuova sottoscrizione puoi annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="29a4e-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="29a4e-166">Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.</span><span class="sxs-lookup"><span data-stu-id="29a4e-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="29a4e-167">Nella pagina dei dettagli della sottoscrizione imposta la sottoscrizione precedente in **sospeso** e seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="29a4e-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="29a4e-168">La sottoscrizione precedente viene ora sospesa e la nuova sottoscrizione diventa attiva.</span><span class="sxs-lookup"><span data-stu-id="29a4e-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="29a4e-169">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="29a4e-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="29a4e-170">Il cliente non incorrere costi aggiuntivi necessari per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="29a4e-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



