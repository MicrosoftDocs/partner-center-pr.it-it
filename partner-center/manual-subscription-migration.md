---
title: Eseguire la migrazione di Dynamics 365 e si prevede di Engagement dei clienti da Basic (offerte completo) per le versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement pianificare dalle sottoscrizioni Basic (offre completo) non può essere rinnovato.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offre, rinnovare le offerte, nuovi SKU di Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134401"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="69228-104">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="69228-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="69228-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="69228-105">**Applies to**</span></span>

-  <span data-ttu-id="69228-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="69228-106">Partner Center</span></span>

<span data-ttu-id="69228-107">I clienti il 1 gennaio 2019 efficaci con Dynamics 365 for Sales / Customer Engagement pianificare dalle sottoscrizioni Basic (offre completo) non effettuare il rinnovo non è più queste offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="69228-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="69228-108">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà per "Expires su [date]" da "Rinnova automaticamente in [date]".</span><span class="sxs-lookup"><span data-stu-id="69228-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="69228-109">Per garantire continuità aziendale per i clienti, è necessario eseguire la transizione quelli con le sottoscrizioni in scadenza un'opzione supportata, elencati di seguito.</span><span class="sxs-lookup"><span data-stu-id="69228-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="69228-110">Si consiglia di far passare i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento, al fine di evitare eventuali interruzioni del servizio.</span><span class="sxs-lookup"><span data-stu-id="69228-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="69228-111">Se si usa l'API (CREST o centro per i Partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione con l'automobile vengono rinnovate = False proprietà.</span><span class="sxs-lookup"><span data-stu-id="69228-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="69228-112">Le sottoscrizioni in questione verranno impostate su auto rinnovare = False su 1 gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="69228-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="69228-113">È possibile trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="69228-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="69228-114">Di Dynamics 365 offre in fase di ritiro</span><span class="sxs-lookup"><span data-stu-id="69228-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="69228-115">Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-116">Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="69228-117">Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-118">Dynamics 365 per vendita Enterprise Edition (prezzo per enti pubblici) CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-119">Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-120">Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="69228-121">Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-122">Dynamics 365 per vendita Enterprise Edition (prezzo per enti pubblici) da software Assurance per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-123">Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-124">Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="69228-125">Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-126">Dynamics 365 per il componente aggiuntivo di vendita Enterprise Edition (prezzo per enti pubblici) per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-127">Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-128">Dynamics 365 Customer Engagement piano Enterprise Edition (prezzo per enti pubblici) CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-129">Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-130">Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="69228-131">Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-132">Dynamics 365 Customer Engagement piano Enterprise Edition (prezzo per enti pubblici) da software Assurance per CRM Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-133">Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-134">Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="69228-135">Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-136">Dynamics 365 Customer Engagement Enterprise Edition (prezzo per enti pubblici) componente aggiuntivo del piano Basic CRM (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-137">Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo) per gli studenti</span><span class="sxs-lookup"><span data-stu-id="69228-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="69228-138">Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo) per istituti di istruzione</span><span class="sxs-lookup"><span data-stu-id="69228-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="69228-139">Dynamics 365 for Sales / piani di Customer Engagement piano dalla sostituzione Basic (offre completo)</span><span class="sxs-lookup"><span data-stu-id="69228-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="69228-140">**Offerte ritirate**</span><span class="sxs-lookup"><span data-stu-id="69228-140">**Retired offers**</span></span>   

- <span data-ttu-id="69228-141">Dynamics 365 for Sales da CRM Basic o CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="69228-142">Dynamics 365 Customer Engagement piano da CRM Basic o CRMOL Basic (offerta completo)</span><span class="sxs-lookup"><span data-stu-id="69228-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="69228-143">**Opzioni di sostituzione**</span><span class="sxs-lookup"><span data-stu-id="69228-143">**Replacement options**</span></span>
- <span data-ttu-id="69228-144">Dynamics 365 for Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="69228-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="69228-145">Dynamics 365 for Sales Professional (nuovo)</span><span class="sxs-lookup"><span data-stu-id="69228-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="69228-146">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="69228-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="69228-147">Dynamics 365 Customer Engagement piano o</span><span class="sxs-lookup"><span data-stu-id="69228-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="69228-148">Membri del Team Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="69228-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="69228-149">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="69228-149">Transition customers to new product plans</span></span>

<span data-ttu-id="69228-150">I clienti lo spostamento dal ritirati SKU quelli più recenti richiede i passaggi seguenti nell'ordine indicato:</span><span class="sxs-lookup"><span data-stu-id="69228-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="69228-151">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="69228-151">Purchase the new subscription</span></span>
- <span data-ttu-id="69228-152">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="69228-152">Reassign current user licenses</span></span>
- <span data-ttu-id="69228-153">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="69228-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="69228-154">Il nuovo piano di acquisto per il cliente</span><span class="sxs-lookup"><span data-stu-id="69228-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="69228-155">Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente che si desidera spostare la nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="69228-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="69228-156">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="69228-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="69228-157">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="69228-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="69228-158">Il cliente avrà la sottoscrizione precedente sia quello nuovo.</span><span class="sxs-lookup"><span data-stu-id="69228-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="69228-159">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="69228-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="69228-160">Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.</span><span class="sxs-lookup"><span data-stu-id="69228-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="69228-161">Seleziona **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="69228-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="69228-162">Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **gestire le licenze**.</span><span class="sxs-lookup"><span data-stu-id="69228-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="69228-163">Nel **gestire le licenze** pagina, cancellare il di Dynamics 365 for Sales / piano di Engagement dei clienti da Basic (completi dell'offerta) casella di controllo di licenza e selezionare un nuovo piano di servizio per la sottoscrizione cliente stia passando ad.</span><span class="sxs-lookup"><span data-stu-id="69228-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="69228-164">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="69228-164">Select **Submit**.</span></span> <span data-ttu-id="69228-165">Si eseguirà questa operazione per ogni utente che necessita la nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="69228-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="69228-166">Dopo aver spostato le licenze alla nuova sottoscrizione è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="69228-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="69228-167">Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.</span><span class="sxs-lookup"><span data-stu-id="69228-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="69228-168">Nella pagina di dettagli della sottoscrizione, impostare la sottoscrizione precedente **degli elementi sospesi** e selezionare **Submit**.</span><span class="sxs-lookup"><span data-stu-id="69228-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="69228-169">La sottoscrizione precedente a questo punto viene sospeso e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="69228-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="69228-170">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="69228-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="69228-171">Il cliente non incorrerà costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="69228-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



