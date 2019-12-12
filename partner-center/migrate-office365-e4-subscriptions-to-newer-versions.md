---
title: Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365 | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'edizione Microsoft Office 365 Enterprise E4 è stata ritirata il 7 aprile 2017. Scopri come eseguire la migrazione degli abbonamenti del cliente alle nuove versioni di Office 365.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 314711a3f640ad6a228a437e35fe0d8a543e4da5
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004565"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="b362b-104">Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="b362b-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="b362b-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="b362b-105">**Applies to**</span></span>

-  <span data-ttu-id="b362b-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b362b-106">Partner Center</span></span>

<span data-ttu-id="b362b-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="b362b-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="b362b-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="b362b-108">Global admin</span></span>
-   <span data-ttu-id="b362b-109">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="b362b-109">User admin</span></span>
-   <span data-ttu-id="b362b-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="b362b-110">Admin agent</span></span>
-   <span data-ttu-id="b362b-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="b362b-111">Sales agent</span></span>

<span data-ttu-id="b362b-112">Il piano Office 365 Enterprise E4 è stato ritirato il 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="b362b-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="b362b-113">Dopo tale data, non sarà possibile acquistare nuovi abbonamenti a Office 365 E4 e gli abbonamenti E4 esistenti non verranno rinnovati automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="b362b-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="b362b-114">Gli abbonamenti E4 verranno annullati alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="b362b-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="b362b-115">Per garantire la continuità, è opportuno trasferire i clienti con abbonamenti E4 in scadenza a una delle opzioni SKU supportate indicate di seguito.</span><span class="sxs-lookup"><span data-stu-id="b362b-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="b362b-116">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="b362b-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="b362b-117">Gli SKU di Office 365 Enterprise E4 Commercial e government sono stati ritirati.</span><span class="sxs-lookup"><span data-stu-id="b362b-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="b362b-118">Nella pagina dei dettagli dell'abbonamento, lo stato dell'abbonamento E4 è passato a "Data di scadenza [data]" da "Rinnovo automatico il [data]".</span><span class="sxs-lookup"><span data-stu-id="b362b-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="b362b-119">Se usi l'API (CREST o Centro per i partner), puoi individuare gli abbonamenti in scadenza valutando la data di scadenza dell'abbonamento insieme alla proprietà auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="b362b-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="b362b-120">Gli abbonamenti E4 verranno impostati su auto renew=False il 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="b362b-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="b362b-121">È possibile trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="b362b-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="b362b-122">Piani di sostituzione dell'edizione Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="b362b-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="b362b-123">Puoi scegliere di mantenere le stesse funzionalità di E4 oppure proporre ai clienti di trarre vantaggio dalle nuove funzionalità di Office 365 e Skype for Business Online.</span><span class="sxs-lookup"><span data-stu-id="b362b-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="b362b-124">I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice dell'elenco di offerte nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b362b-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="b362b-125">È possibile sostituire Secure Product Enterprise E3 o Secure Productive Enterprise E5 nelle opzioni seguenti di Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.</span><span class="sxs-lookup"><span data-stu-id="b362b-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="b362b-126">Opzione 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="b362b-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="b362b-127">Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="b362b-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="b362b-128">Opzione 3: Office 365 Enterprise E3 + Skype for Business più CAL (a parità di prezzo e funzionalità con E4)</span><span class="sxs-lookup"><span data-stu-id="b362b-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="b362b-129">Opzione 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b362b-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="b362b-130">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="b362b-130">Feature</span></span> | <span data-ttu-id="b362b-131">Opzione 1</span><span class="sxs-lookup"><span data-stu-id="b362b-131">Option 1</span></span> | <span data-ttu-id="b362b-132">Opzione 2</span><span class="sxs-lookup"><span data-stu-id="b362b-132">Option 2</span></span> | <span data-ttu-id="b362b-133">Opzione 3</span><span class="sxs-lookup"><span data-stu-id="b362b-133">Option 3</span></span> | <span data-ttu-id="b362b-134">Opzione 4</span><span class="sxs-lookup"><span data-stu-id="b362b-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="b362b-135">Offre tutte le funzionalità incluse in Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="b362b-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="b362b-136">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-136">Yes</span></span> | <span data-ttu-id="b362b-137">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-137">Yes</span></span> | <span data-ttu-id="b362b-138">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-138">Yes</span></span> | <span data-ttu-id="b362b-139">No</span><span class="sxs-lookup"><span data-stu-id="b362b-139">No</span></span> |
| <span data-ttu-id="b362b-140">Numeri di telefono gestiti in Office 365?</span><span class="sxs-lookup"><span data-stu-id="b362b-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="b362b-141">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-141">Yes</span></span> | <span data-ttu-id="b362b-142">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-142">Yes</span></span> | <span data-ttu-id="b362b-143">No</span><span class="sxs-lookup"><span data-stu-id="b362b-143">No</span></span> | <span data-ttu-id="b362b-144">No</span><span class="sxs-lookup"><span data-stu-id="b362b-144">No</span></span> |
| <span data-ttu-id="b362b-145">Numeri di telefono gestiti in locale e in Office 365 (distribuzione ibrida)?</span><span class="sxs-lookup"><span data-stu-id="b362b-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="b362b-146">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-146">Yes</span></span> | <span data-ttu-id="b362b-147">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-147">Yes</span></span> | <span data-ttu-id="b362b-148">No</span><span class="sxs-lookup"><span data-stu-id="b362b-148">No</span></span> | <span data-ttu-id="b362b-149">No</span><span class="sxs-lookup"><span data-stu-id="b362b-149">No</span></span> |
| <span data-ttu-id="b362b-150">Opzione per aggiungere un piano per le chiamate vocali PSTN?</span><span class="sxs-lookup"><span data-stu-id="b362b-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="b362b-151">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-151">Yes</span></span> | <span data-ttu-id="b362b-152">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-152">Yes</span></span> | <span data-ttu-id="b362b-153">No</span><span class="sxs-lookup"><span data-stu-id="b362b-153">No</span></span> | <span data-ttu-id="b362b-154">No</span><span class="sxs-lookup"><span data-stu-id="b362b-154">No</span></span> |
| <span data-ttu-id="b362b-155">Servizi di conferenza PSTN?</span><span class="sxs-lookup"><span data-stu-id="b362b-155">PSTN Conferencing?</span></span> | <span data-ttu-id="b362b-156">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-156">Yes</span></span> | <span data-ttu-id="b362b-157">No</span><span class="sxs-lookup"><span data-stu-id="b362b-157">No</span></span> | <span data-ttu-id="b362b-158">No</span><span class="sxs-lookup"><span data-stu-id="b362b-158">No</span></span> | <span data-ttu-id="b362b-159">No</span><span class="sxs-lookup"><span data-stu-id="b362b-159">No</span></span> |
| <span data-ttu-id="b362b-160">Strumenti avanzati per collaborazione, analisi e sicurezza?</span><span class="sxs-lookup"><span data-stu-id="b362b-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="b362b-161">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-161">Yes</span></span> | <span data-ttu-id="b362b-162">No</span><span class="sxs-lookup"><span data-stu-id="b362b-162">No</span></span> | <span data-ttu-id="b362b-163">No</span><span class="sxs-lookup"><span data-stu-id="b362b-163">No</span></span> | <span data-ttu-id="b362b-164">No</span><span class="sxs-lookup"><span data-stu-id="b362b-164">No</span></span> |
| <span data-ttu-id="b362b-165">Report interattivi, dashboard ed effetti di visualizzazione dei dati?</span><span class="sxs-lookup"><span data-stu-id="b362b-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="b362b-166">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-166">Yes</span></span> | <span data-ttu-id="b362b-167">No</span><span class="sxs-lookup"><span data-stu-id="b362b-167">No</span></span> | <span data-ttu-id="b362b-168">No</span><span class="sxs-lookup"><span data-stu-id="b362b-168">No</span></span> | <span data-ttu-id="b362b-169">No</span><span class="sxs-lookup"><span data-stu-id="b362b-169">No</span></span> | 
| <span data-ttu-id="b362b-170">Maggiore controllo sulla sicurezza e sulla conformità dei dati con controlli avanzati integrati per la privacy, la trasparenza e gli utenti?</span><span class="sxs-lookup"><span data-stu-id="b362b-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="b362b-171">Sì</span><span class="sxs-lookup"><span data-stu-id="b362b-171">Yes</span></span> | <span data-ttu-id="b362b-172">No</span><span class="sxs-lookup"><span data-stu-id="b362b-172">No</span></span> | <span data-ttu-id="b362b-173">No</span><span class="sxs-lookup"><span data-stu-id="b362b-173">No</span></span> | <span data-ttu-id="b362b-174">No</span><span class="sxs-lookup"><span data-stu-id="b362b-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b362b-175">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="b362b-175">Transition customers to new product plans</span></span>

<span data-ttu-id="b362b-176">Microsoft offre continuamente nuovi prodotti e servizi ai suoi partner.</span><span class="sxs-lookup"><span data-stu-id="b362b-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="b362b-177">In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione dei loro abbonamenti da SKU destinati a essere ritirati.</span><span class="sxs-lookup"><span data-stu-id="b362b-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="b362b-178">La migrazione dei clienti da SKU ritirati a quelli più recenti richiede la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="b362b-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="b362b-179">Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="b362b-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="b362b-180">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="b362b-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="b362b-181">Annullare l'abbonamento precedente</span><span class="sxs-lookup"><span data-stu-id="b362b-181">Cancel the old subscription</span></span>

<span data-ttu-id="b362b-182">Attieniti a questa procedura per eseguire la migrazione dell'abbonamento a Office 365 Enterprise E4 di un cliente a una delle opzioni incluse nella tabella precedente.</span><span class="sxs-lookup"><span data-stu-id="b362b-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="b362b-183">Passaggio 1: Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="b362b-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="b362b-184">Dal menu **centro partner** selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="b362b-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="b362b-185">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="b362b-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="b362b-186">Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b362b-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="b362b-187">Passaggio 2: Riassegnare le licenze utente del cliente</span><span class="sxs-lookup"><span data-stu-id="b362b-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="b362b-188">Dal menu **centro** per i partner selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="b362b-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="b362b-189">Verrà visualizzata la pagina utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="b362b-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="b362b-190">Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="b362b-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="b362b-191">Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza di **Office 365 Enterprise E4** e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente.</span><span class="sxs-lookup"><span data-stu-id="b362b-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="b362b-192">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="b362b-192">Select **Submit**.</span></span> <span data-ttu-id="b362b-193">Le nuove cessioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="b362b-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="b362b-194">Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.</span><span class="sxs-lookup"><span data-stu-id="b362b-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="b362b-195">Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare l'abbonamento ritirato al livello principale del cliente.</span><span class="sxs-lookup"><span data-stu-id="b362b-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="b362b-196">Passaggio 3: Annullare l'abbonamento precedente</span><span class="sxs-lookup"><span data-stu-id="b362b-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="b362b-197">Scegliere **clienti**dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="b362b-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b362b-198">Seleziona il cliente da trasferire e l'abbonamento da annullare.</span><span class="sxs-lookup"><span data-stu-id="b362b-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="b362b-199">Nella pagina dei dettagli sull'abbonamento imposta lo stato su **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="b362b-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="b362b-200">Seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="b362b-200">Select **Submit**.</span></span>

<span data-ttu-id="b362b-201">L'abbonamento precedente viene sospeso e quello nuovo diventa attivo.</span><span class="sxs-lookup"><span data-stu-id="b362b-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="b362b-202">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="b362b-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b362b-203">Il cliente non dovrà sostenere alcun costo aggiuntivo per l'abbonamento precedente.</span><span class="sxs-lookup"><span data-stu-id="b362b-203">The customer incurs no additional costs for the old subscription.</span></span>



 



