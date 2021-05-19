---
title: Eseguire la migrazione di sottoscrizioni qualificate di Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione da sottoscrizioni dynamics 365 di base qualificate a una nuova sottoscrizione prima della scadenza delle sottoscrizioni esistenti.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151645"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="c59ce-103">Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti</span><span class="sxs-lookup"><span data-stu-id="c59ce-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="c59ce-104">**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c59ce-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="c59ce-105">A partire dal 1° gennaio 2019, i clienti con Dynamics 365 for Sales/Customer Engagement Plan delle sottoscrizioni Basic (Offerte qualificate) non possono più rinnovare queste offerte legacy; Le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="c59ce-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="c59ce-106">Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione verrà modificato in "Scadenza alla [data]" da "Rinnovo automatico il [data]".</span><span class="sxs-lookup"><span data-stu-id="c59ce-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="c59ce-107">Per garantire la continuità per i clienti, è necessario eseguire la transizione di quelli con sottoscrizioni in scadenza a un'opzione supportata, elencata di seguito.</span><span class="sxs-lookup"><span data-stu-id="c59ce-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="c59ce-108">È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="c59ce-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c59ce-109">Se si usa l'API (STEMM o Partner Center), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà rinnovo automatico = False.</span><span class="sxs-lookup"><span data-stu-id="c59ce-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="c59ce-110">Le sottoscrizioni in questione verranno impostate su auto renew=False il 1° gennaio 2019.</span><span class="sxs-lookup"><span data-stu-id="c59ce-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="c59ce-111">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="c59ce-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="c59ce-112">Le offerte dynamics 365 vengono ritirate</span><span class="sxs-lookup"><span data-stu-id="c59ce-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="c59ce-113">Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-114">Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata) per docenti</span><span class="sxs-lookup"><span data-stu-id="c59ce-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c59ce-115">Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c59ce-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-116">Dynamics 365 for Sales edizione Enterprise (government pricing) CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-117">Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-118">Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) for Faculty (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="c59ce-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c59ce-119">Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) for Students (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="c59ce-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-120">Dynamics 365 for Sales edizione Enterprise (prezzi per enti pubblici) Dalla sa per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-121">Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-122">Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="c59ce-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c59ce-123">Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="c59ce-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-124">Dynamics 365 for Sales edizione Enterprise (government pricing) Add-On for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-125">Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-126">Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) CRMOL Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-127">Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata) per studenti</span><span class="sxs-lookup"><span data-stu-id="c59ce-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-128">Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata) per docenti</span><span class="sxs-lookup"><span data-stu-id="c59ce-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c59ce-129">Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-130">Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-131">Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="c59ce-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-132">Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="c59ce-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="c59ce-133">Piano Dynamics 365 Customer Engagement edizione Enterprise Add-On per CRM Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-134">Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) Add-On for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="c59ce-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-135">Dynamics 365 Customer Engagement Plan edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="c59ce-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="c59ce-136">Dynamics 365 Customer Engagement Plan edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="c59ce-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="c59ce-137">Dynamics 365 for Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)</span><span class="sxs-lookup"><span data-stu-id="c59ce-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="c59ce-138">**Offerte ritirate**</span><span class="sxs-lookup"><span data-stu-id="c59ce-138">**Retired offers**</span></span>   

- <span data-ttu-id="c59ce-139">Dynamics 365 for Sales da CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="c59ce-140">Piano Dynamics 365 Customer Engagement di CRM Basic o CRMOL Basic (offerta qualificata)</span><span class="sxs-lookup"><span data-stu-id="c59ce-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="c59ce-141">**Opzioni di sostituzione**</span><span class="sxs-lookup"><span data-stu-id="c59ce-141">**Replacement options**</span></span>
- <span data-ttu-id="c59ce-142">Dynamics 365 for Sales Professional (NUOVO)</span><span class="sxs-lookup"><span data-stu-id="c59ce-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="c59ce-143">Dynamics 365 for Sales Professional (NUOVO)</span><span class="sxs-lookup"><span data-stu-id="c59ce-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="c59ce-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="c59ce-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="c59ce-145">Piano di Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="c59ce-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="c59ce-146">Membri del team di Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="c59ce-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c59ce-147">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="c59ce-147">Transition customers to new product plans</span></span>

<span data-ttu-id="c59ce-148">Per spostare i clienti da SKU ritirati a SKU più recenti, è necessario eseguire i passaggi seguenti in questo ordine:</span><span class="sxs-lookup"><span data-stu-id="c59ce-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="c59ce-149">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c59ce-149">Purchase the new subscription</span></span>
- <span data-ttu-id="c59ce-150">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="c59ce-150">Reassign current user licenses</span></span>
- <span data-ttu-id="c59ce-151">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="c59ce-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="c59ce-152">Acquistare il nuovo piano per il cliente</span><span class="sxs-lookup"><span data-stu-id="c59ce-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="c59ce-153">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente da spostare nella nuova sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c59ce-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="c59ce-154">Selezionare **Aggiungi sottoscrizione.**</span><span class="sxs-lookup"><span data-stu-id="c59ce-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="c59ce-155">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="c59ce-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="c59ce-156">Il cliente avrà ora sia la sottoscrizione precedente che quella nuova.</span><span class="sxs-lookup"><span data-stu-id="c59ce-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="c59ce-157">Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="c59ce-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="c59ce-158">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.</span><span class="sxs-lookup"><span data-stu-id="c59ce-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c59ce-159">Selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="c59ce-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="c59ce-160">Per riassegnare una licenza a un utente, selezionare l'utente e quindi **selezionare Gestisci licenze.**</span><span class="sxs-lookup"><span data-stu-id="c59ce-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="c59ce-161">Nella  pagina Gestisci licenze deselezionare la casella di controllo Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Piano Dynamics 365 for Sales/Customer Engagement dalla licenza Basic - Offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente.</span><span class="sxs-lookup"><span data-stu-id="c59ce-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="c59ce-162">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="c59ce-162">Select **Submit**.</span></span> <span data-ttu-id="c59ce-163">Questa operazione verrà creata per ogni utente che necessita della nuova licenza.</span><span class="sxs-lookup"><span data-stu-id="c59ce-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="c59ce-164">Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="c59ce-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="c59ce-165">Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.</span><span class="sxs-lookup"><span data-stu-id="c59ce-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c59ce-166">Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione precedente su **Sospeso** e selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="c59ce-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="c59ce-167">La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="c59ce-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="c59ce-168">Il provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="c59ce-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c59ce-169">Il cliente non incorrerà in costi aggiuntivi per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="c59ce-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



