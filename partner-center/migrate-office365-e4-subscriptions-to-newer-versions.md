---
title: Eseguire la migrazione delle sottoscrizioni di Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 è stato ritirato a partire dal 7 aprile 2017. Informazioni su come eseguire la migrazione delle sottoscrizioni dei clienti a versioni più recenti di Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949050"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="f37fb-104">Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="f37fb-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="f37fb-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="f37fb-105">**Applies to**</span></span>

-  <span data-ttu-id="f37fb-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="f37fb-106">Partner Center</span></span>

<span data-ttu-id="f37fb-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="f37fb-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="f37fb-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="f37fb-108">Global admin</span></span>
-   <span data-ttu-id="f37fb-109">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="f37fb-109">User admin</span></span>
-   <span data-ttu-id="f37fb-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="f37fb-110">Admin agent</span></span>
-   <span data-ttu-id="f37fb-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="f37fb-111">Sales agent</span></span>

<span data-ttu-id="f37fb-112">Il piano Office 365 Enterprise E4 è stato ritirato, a partire dal 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="f37fb-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="f37fb-113">Non è più possibile acquistare nuove sottoscrizioni di Office 365 E4 dopo questa data e le sottoscrizioni E4 esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="f37fb-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="f37fb-114">Quando le sottoscrizioni E4 sono terminate, verranno annullate.</span><span class="sxs-lookup"><span data-stu-id="f37fb-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="f37fb-115">Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni E4 in scadenza a un'opzione SKU supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="f37fb-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="f37fb-116">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="f37fb-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="f37fb-117">Gli SKU di Office 365 Enterprise E4 Commercial e government sono stati ritirati.</span><span class="sxs-lookup"><span data-stu-id="f37fb-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="f37fb-118">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione E4 è stato modificato in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="f37fb-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f37fb-119">Se si usa l'API (CREST o centro per i partner), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="f37fb-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="f37fb-120">Le sottoscrizioni E4 verranno impostate su auto Renew = false nel 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="f37fb-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="f37fb-121">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="f37fb-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="f37fb-122">Piani di sostituzione di Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="f37fb-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="f37fb-123">È possibile scegliere di mantenere la stessa funzionalità con E4 o chiedere ai clienti di sfruttare le funzionalità e le funzionalità più recenti di Office 365 e Skype for business online.</span><span class="sxs-lookup"><span data-stu-id="f37fb-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="f37fb-124">I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f37fb-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="f37fb-125">Secure Product Enterprise E3 o Secure produttiva Enterprise E5 possono essere sostituiti dalle opzioni seguenti per Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.</span><span class="sxs-lookup"><span data-stu-id="f37fb-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="f37fb-126">Opzione 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="f37fb-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="f37fb-127">Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="f37fb-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="f37fb-128">Opzione 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (parità prezzo e funzionalità con E4)</span><span class="sxs-lookup"><span data-stu-id="f37fb-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="f37fb-129">Opzione 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="f37fb-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="f37fb-130">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="f37fb-130">Feature</span></span> | <span data-ttu-id="f37fb-131">Opzione 1</span><span class="sxs-lookup"><span data-stu-id="f37fb-131">Option 1</span></span> | <span data-ttu-id="f37fb-132">Opzione 2</span><span class="sxs-lookup"><span data-stu-id="f37fb-132">Option 2</span></span> | <span data-ttu-id="f37fb-133">Opzione 3</span><span class="sxs-lookup"><span data-stu-id="f37fb-133">Option 3</span></span> | <span data-ttu-id="f37fb-134">Opzione 4</span><span class="sxs-lookup"><span data-stu-id="f37fb-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="f37fb-135">Ottenere tutte le funzionalità incluse in Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="f37fb-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="f37fb-136">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-136">Yes</span></span> | <span data-ttu-id="f37fb-137">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-137">Yes</span></span> | <span data-ttu-id="f37fb-138">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-138">Yes</span></span> | <span data-ttu-id="f37fb-139">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-139">No</span></span> |
| <span data-ttu-id="f37fb-140">Numeri di telefono gestiti in Office 365?</span><span class="sxs-lookup"><span data-stu-id="f37fb-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="f37fb-141">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-141">Yes</span></span> | <span data-ttu-id="f37fb-142">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-142">Yes</span></span> | <span data-ttu-id="f37fb-143">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-143">No</span></span> | <span data-ttu-id="f37fb-144">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-144">No</span></span> |
| <span data-ttu-id="f37fb-145">Numeri di telefono gestiti sia in locale che in Office 365 (distribuzione ibrida)?</span><span class="sxs-lookup"><span data-stu-id="f37fb-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="f37fb-146">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-146">Yes</span></span> | <span data-ttu-id="f37fb-147">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-147">Yes</span></span> | <span data-ttu-id="f37fb-148">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-148">No</span></span> | <span data-ttu-id="f37fb-149">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-149">No</span></span> |
| <span data-ttu-id="f37fb-150">È possibile aggiungere un piano di chiamata vocale PSTN?</span><span class="sxs-lookup"><span data-stu-id="f37fb-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="f37fb-151">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-151">Yes</span></span> | <span data-ttu-id="f37fb-152">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-152">Yes</span></span> | <span data-ttu-id="f37fb-153">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-153">No</span></span> | <span data-ttu-id="f37fb-154">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-154">No</span></span> |
| <span data-ttu-id="f37fb-155">Conferenze PSTN?</span><span class="sxs-lookup"><span data-stu-id="f37fb-155">PSTN Conferencing?</span></span> | <span data-ttu-id="f37fb-156">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-156">Yes</span></span> | <span data-ttu-id="f37fb-157">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-157">No</span></span> | <span data-ttu-id="f37fb-158">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-158">No</span></span> | <span data-ttu-id="f37fb-159">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-159">No</span></span> |
| <span data-ttu-id="f37fb-160">Strumenti avanzati per la collaborazione, l'analisi e la sicurezza?</span><span class="sxs-lookup"><span data-stu-id="f37fb-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="f37fb-161">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-161">Yes</span></span> | <span data-ttu-id="f37fb-162">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-162">No</span></span> | <span data-ttu-id="f37fb-163">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-163">No</span></span> | <span data-ttu-id="f37fb-164">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-164">No</span></span> |
| <span data-ttu-id="f37fb-165">Report interattivi, dashboard e visualizzazioni dei dati?</span><span class="sxs-lookup"><span data-stu-id="f37fb-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="f37fb-166">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-166">Yes</span></span> | <span data-ttu-id="f37fb-167">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-167">No</span></span> | <span data-ttu-id="f37fb-168">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-168">No</span></span> | <span data-ttu-id="f37fb-169">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-169">No</span></span> | 
| <span data-ttu-id="f37fb-170">Maggiore controllo sulla sicurezza dei dati e sulla conformità con la privacy incorporata, la trasparenza e i controlli utente perfezionati?</span><span class="sxs-lookup"><span data-stu-id="f37fb-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="f37fb-171">Sì</span><span class="sxs-lookup"><span data-stu-id="f37fb-171">Yes</span></span> | <span data-ttu-id="f37fb-172">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-172">No</span></span> | <span data-ttu-id="f37fb-173">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-173">No</span></span> | <span data-ttu-id="f37fb-174">No</span><span class="sxs-lookup"><span data-stu-id="f37fb-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f37fb-175">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="f37fb-175">Transition customers to new product plans</span></span>

<span data-ttu-id="f37fb-176">Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner.</span><span class="sxs-lookup"><span data-stu-id="f37fb-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="f37fb-177">In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate.</span><span class="sxs-lookup"><span data-stu-id="f37fb-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="f37fb-178">Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="f37fb-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="f37fb-179">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f37fb-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="f37fb-180">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="f37fb-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="f37fb-181">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="f37fb-181">Cancel the old subscription</span></span>

<span data-ttu-id="f37fb-182">Seguire questa procedura per eseguire la migrazione della sottoscrizione di Office 365 Enterprise E4 di un cliente a una delle opzioni nella tabella precedente.</span><span class="sxs-lookup"><span data-stu-id="f37fb-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="f37fb-183">Passaggio 1: acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f37fb-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="f37fb-184">Dal menu **centro partner** selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="f37fb-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="f37fb-185">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="f37fb-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="f37fb-186">Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="f37fb-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="f37fb-187">Passaggio 2: riassegnare le licenze degli utenti del cliente</span><span class="sxs-lookup"><span data-stu-id="f37fb-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="f37fb-188">Dal menu **centro** per i partner selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="f37fb-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="f37fb-189">Verrà visualizzata la pagina utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="f37fb-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="f37fb-190">Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="f37fb-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="f37fb-191">Nella pagina **Gestisci licenze** deselezionare la casella di controllo licenza di **Office 365 Enterprise E4** e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="f37fb-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="f37fb-192">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="f37fb-192">Select **Submit**.</span></span> <span data-ttu-id="f37fb-193">Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="f37fb-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="f37fb-194">Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.</span><span class="sxs-lookup"><span data-stu-id="f37fb-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="f37fb-195">Dopo aver spostato le licenze utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata al livello superiore del cliente.</span><span class="sxs-lookup"><span data-stu-id="f37fb-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="f37fb-196">Passaggio 3: annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="f37fb-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="f37fb-197">Scegliere **clienti**dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="f37fb-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="f37fb-198">Selezionare il cliente da spostare e selezionare la sottoscrizione che si vuole annullare.</span><span class="sxs-lookup"><span data-stu-id="f37fb-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="f37fb-199">Nella pagina Dettagli sottoscrizione impostare lo stato della sottoscrizione su **sospeso**.</span><span class="sxs-lookup"><span data-stu-id="f37fb-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="f37fb-200">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="f37fb-200">Select **Submit**.</span></span>

<span data-ttu-id="f37fb-201">La sottoscrizione precedente viene sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="f37fb-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="f37fb-202">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="f37fb-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f37fb-203">Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="f37fb-203">The customer incurs no additional costs for the old subscription.</span></span>



 



