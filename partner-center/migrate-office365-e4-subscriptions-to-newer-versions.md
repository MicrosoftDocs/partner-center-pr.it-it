---
title: Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365 | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'edizione Microsoft Office 365 Enterprise E4 è stata ritirata il 7 aprile 2017. Scopri come eseguire la migrazione degli abbonamenti del cliente alle nuove versioni di Office 365.
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390880"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="58a4d-104">Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="58a4d-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="58a4d-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="58a4d-105">**Applies to**</span></span>

-  <span data-ttu-id="58a4d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="58a4d-106">Partner Center</span></span>

<span data-ttu-id="58a4d-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="58a4d-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="58a4d-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="58a4d-108">Global admin</span></span>
-   <span data-ttu-id="58a4d-109">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="58a4d-109">User admin</span></span>
-   <span data-ttu-id="58a4d-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="58a4d-110">Admin agent</span></span>
-   <span data-ttu-id="58a4d-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="58a4d-111">Sales agent</span></span>

<span data-ttu-id="58a4d-112">Il piano Office 365 Enterprise E4 è stato ritirato il 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="58a4d-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="58a4d-113">Dopo tale data, non sarà possibile acquistare nuovi abbonamenti a Office 365 E4 e gli abbonamenti E4 esistenti non verranno rinnovati automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="58a4d-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="58a4d-114">Gli abbonamenti E4 verranno annullati alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="58a4d-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="58a4d-115">Per garantire la continuità, è opportuno trasferire i clienti con abbonamenti E4 in scadenza a una delle opzioni SKU supportate indicate di seguito.</span><span class="sxs-lookup"><span data-stu-id="58a4d-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="58a4d-116">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="58a4d-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="58a4d-117">Gli SKU di Office 365 Enterprise E4 Commercial e government sono stati ritirati.</span><span class="sxs-lookup"><span data-stu-id="58a4d-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="58a4d-118">Nella pagina dei dettagli dell'abbonamento, lo stato dell'abbonamento E4 è passato a "Data di scadenza [data]" da "Rinnovo automatico il [data]".</span><span class="sxs-lookup"><span data-stu-id="58a4d-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="58a4d-119">Se usi l'API (CREST o Centro per i partner), puoi individuare gli abbonamenti in scadenza valutando la data di scadenza dell'abbonamento insieme alla proprietà auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="58a4d-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="58a4d-120">Gli abbonamenti E4 verranno impostati su auto renew=False il 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="58a4d-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="58a4d-121">È possibile trasferire i clienti a un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="58a4d-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="58a4d-122">Piani di sostituzione dell'edizione Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="58a4d-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="58a4d-123">Puoi scegliere di mantenere le stesse funzionalità di E4 oppure proporre ai clienti di trarre vantaggio dalle nuove funzionalità di Office 365 e Skype for Business Online.</span><span class="sxs-lookup"><span data-stu-id="58a4d-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="58a4d-124">I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice dell'elenco di offerte nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="58a4d-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="58a4d-125">È possibile sostituire Secure Product Enterprise E3 o Secure Productive Enterprise E5 nelle opzioni seguenti di Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="58a4d-126">Opzione 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="58a4d-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="58a4d-127">Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="58a4d-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="58a4d-128">Opzione 3: Office 365 Enterprise E3 + Skype for Business più CAL (a parità di prezzo e funzionalità con E4)</span><span class="sxs-lookup"><span data-stu-id="58a4d-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="58a4d-129">Opzione 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="58a4d-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="58a4d-130">Caratteristica</span><span class="sxs-lookup"><span data-stu-id="58a4d-130">Feature</span></span> | <span data-ttu-id="58a4d-131">Opzione 1</span><span class="sxs-lookup"><span data-stu-id="58a4d-131">Option 1</span></span> | <span data-ttu-id="58a4d-132">Opzione 2</span><span class="sxs-lookup"><span data-stu-id="58a4d-132">Option 2</span></span> | <span data-ttu-id="58a4d-133">Opzione 3</span><span class="sxs-lookup"><span data-stu-id="58a4d-133">Option 3</span></span> | <span data-ttu-id="58a4d-134">Opzione 4</span><span class="sxs-lookup"><span data-stu-id="58a4d-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="58a4d-135">Offre tutte le funzionalità incluse in Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="58a4d-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="58a4d-136">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-136">Yes</span></span> | <span data-ttu-id="58a4d-137">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-137">Yes</span></span> | <span data-ttu-id="58a4d-138">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-138">Yes</span></span> | <span data-ttu-id="58a4d-139">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-139">No</span></span> |
| <span data-ttu-id="58a4d-140">Numeri di telefono gestiti in Office 365?</span><span class="sxs-lookup"><span data-stu-id="58a4d-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="58a4d-141">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-141">Yes</span></span> | <span data-ttu-id="58a4d-142">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-142">Yes</span></span> | <span data-ttu-id="58a4d-143">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-143">No</span></span> | <span data-ttu-id="58a4d-144">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-144">No</span></span> |
| <span data-ttu-id="58a4d-145">Numeri di telefono gestiti in locale e in Office 365 (distribuzione ibrida)?</span><span class="sxs-lookup"><span data-stu-id="58a4d-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="58a4d-146">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-146">Yes</span></span> | <span data-ttu-id="58a4d-147">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-147">Yes</span></span> | <span data-ttu-id="58a4d-148">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-148">No</span></span> | <span data-ttu-id="58a4d-149">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-149">No</span></span> |
| <span data-ttu-id="58a4d-150">Opzione per aggiungere un piano per le chiamate vocali PSTN?</span><span class="sxs-lookup"><span data-stu-id="58a4d-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="58a4d-151">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-151">Yes</span></span> | <span data-ttu-id="58a4d-152">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-152">Yes</span></span> | <span data-ttu-id="58a4d-153">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-153">No</span></span> | <span data-ttu-id="58a4d-154">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-154">No</span></span> |
| <span data-ttu-id="58a4d-155">Servizi di conferenza PSTN?</span><span class="sxs-lookup"><span data-stu-id="58a4d-155">PSTN Conferencing?</span></span> | <span data-ttu-id="58a4d-156">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-156">Yes</span></span> | <span data-ttu-id="58a4d-157">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-157">No</span></span> | <span data-ttu-id="58a4d-158">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-158">No</span></span> | <span data-ttu-id="58a4d-159">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-159">No</span></span> |
| <span data-ttu-id="58a4d-160">Strumenti avanzati per collaborazione, analisi e sicurezza?</span><span class="sxs-lookup"><span data-stu-id="58a4d-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="58a4d-161">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-161">Yes</span></span> | <span data-ttu-id="58a4d-162">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-162">No</span></span> | <span data-ttu-id="58a4d-163">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-163">No</span></span> | <span data-ttu-id="58a4d-164">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-164">No</span></span> |
| <span data-ttu-id="58a4d-165">Report interattivi, dashboard ed effetti di visualizzazione dei dati?</span><span class="sxs-lookup"><span data-stu-id="58a4d-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="58a4d-166">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-166">Yes</span></span> | <span data-ttu-id="58a4d-167">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-167">No</span></span> | <span data-ttu-id="58a4d-168">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-168">No</span></span> | <span data-ttu-id="58a4d-169">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-169">No</span></span> | 
| <span data-ttu-id="58a4d-170">Maggiore controllo sulla sicurezza e sulla conformità dei dati con controlli avanzati integrati per la privacy, la trasparenza e gli utenti?</span><span class="sxs-lookup"><span data-stu-id="58a4d-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="58a4d-171">Sì</span><span class="sxs-lookup"><span data-stu-id="58a4d-171">Yes</span></span> | <span data-ttu-id="58a4d-172">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-172">No</span></span> | <span data-ttu-id="58a4d-173">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-173">No</span></span> | <span data-ttu-id="58a4d-174">No</span><span class="sxs-lookup"><span data-stu-id="58a4d-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="58a4d-175">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="58a4d-175">Transition customers to new product plans</span></span>

<span data-ttu-id="58a4d-176">Microsoft offre continuamente nuovi prodotti e servizi ai suoi partner.</span><span class="sxs-lookup"><span data-stu-id="58a4d-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="58a4d-177">In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione dei loro abbonamenti da SKU destinati a essere ritirati.</span><span class="sxs-lookup"><span data-stu-id="58a4d-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="58a4d-178">La migrazione dei clienti da SKU ritirati a quelli più recenti richiede la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="58a4d-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="58a4d-179">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="58a4d-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="58a4d-180">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="58a4d-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="58a4d-181">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="58a4d-181">Cancel the old subscription</span></span>

<span data-ttu-id="58a4d-182">Attieniti a questa procedura per eseguire la migrazione dell'abbonamento a Office 365 Enterprise E4 di un cliente a una delle opzioni incluse nella tabella precedente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="58a4d-183">Passaggio 1: Acquistare il nuovo abbonamento</span><span class="sxs-lookup"><span data-stu-id="58a4d-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="58a4d-184">Dal menu **centro partner** selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="58a4d-185">Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="58a4d-186">Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="58a4d-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="58a4d-187">Passaggio 2: Riassegnare le licenze utente del cliente</span><span class="sxs-lookup"><span data-stu-id="58a4d-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="58a4d-188">Dal menu **centro** per i partner selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="58a4d-189">Verrà visualizzata la pagina utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="58a4d-190">Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="58a4d-191">Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza di **Office 365 Enterprise E4** e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="58a4d-192">Selezionare **Submit**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-192">Select **Submit**.</span></span> <span data-ttu-id="58a4d-193">Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="58a4d-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="58a4d-194">Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.</span><span class="sxs-lookup"><span data-stu-id="58a4d-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="58a4d-195">Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare l'abbonamento ritirato al livello principale del cliente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="58a4d-196">Passaggio 3: Annullare l'abbonamento precedente</span><span class="sxs-lookup"><span data-stu-id="58a4d-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="58a4d-197">Scegliere **clienti**dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="58a4d-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="58a4d-198">Seleziona il cliente da trasferire e l'abbonamento da annullare.</span><span class="sxs-lookup"><span data-stu-id="58a4d-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="58a4d-199">Nella pagina dei dettagli sull'abbonamento imposta lo stato su **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="58a4d-200">Selezionare **Submit**.</span><span class="sxs-lookup"><span data-stu-id="58a4d-200">Select **Submit**.</span></span>

<span data-ttu-id="58a4d-201">L'abbonamento precedente viene sospeso e quello nuovo diventa attivo.</span><span class="sxs-lookup"><span data-stu-id="58a4d-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="58a4d-202">Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="58a4d-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="58a4d-203">Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="58a4d-203">The customer incurs no additional costs for the old subscription.</span></span>



 



