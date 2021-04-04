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
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132622"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="658dc-104">Migrazione degli abbonamenti Office 365 E4 alle nuove versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="658dc-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="658dc-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="658dc-105">**Appropriate roles**</span></span>

- <span data-ttu-id="658dc-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="658dc-106">Global admin</span></span>
- <span data-ttu-id="658dc-107">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="658dc-107">User management admin</span></span>
- <span data-ttu-id="658dc-108">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="658dc-108">Admin agent</span></span>
- <span data-ttu-id="658dc-109">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="658dc-109">Sales agent</span></span>

<span data-ttu-id="658dc-110">Il piano Office 365 Enterprise E4 è stato ritirato, a partire dal 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="658dc-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="658dc-111">Non è più possibile acquistare nuove sottoscrizioni di Office 365 E4 dopo questa data e le sottoscrizioni E4 esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="658dc-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="658dc-112">Quando le sottoscrizioni E4 sono terminate, verranno annullate.</span><span class="sxs-lookup"><span data-stu-id="658dc-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="658dc-113">Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni E4 in scadenza a un'opzione SKU supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="658dc-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="658dc-114">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="658dc-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="658dc-115">Gli SKU di Office 365 Enterprise E4 Commercial e government sono stati ritirati.</span><span class="sxs-lookup"><span data-stu-id="658dc-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="658dc-116">Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione E4 è stato modificato in "scade in data [DATE]" da "auto renews on [DATE]".</span><span class="sxs-lookup"><span data-stu-id="658dc-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="658dc-117">Se si usa l'API (CREST o centro per i partner), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="658dc-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="658dc-118">Le sottoscrizioni E4 verranno impostate su auto Renew = false nel 7 aprile 2017.</span><span class="sxs-lookup"><span data-stu-id="658dc-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="658dc-119">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="658dc-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="658dc-120">Piani di sostituzione di Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="658dc-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="658dc-121">È possibile scegliere di mantenere la stessa funzionalità con E4 o chiedere ai clienti di sfruttare le funzionalità e le funzionalità più recenti di Office 365 e Skype for business online.</span><span class="sxs-lookup"><span data-stu-id="658dc-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="658dc-122">I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="658dc-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="658dc-123">Secure Product Enterprise E3 o Secure produttiva Enterprise E5 possono essere sostituiti dalle opzioni seguenti per Office 365 Enterprise E3 o Office 365 Enterprise E5 rispettivamente.</span><span class="sxs-lookup"><span data-stu-id="658dc-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="658dc-124">Opzione 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="658dc-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="658dc-125">Opzione 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="658dc-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="658dc-126">Opzione 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (parità prezzo e funzionalità con E4)</span><span class="sxs-lookup"><span data-stu-id="658dc-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="658dc-127">Opzione 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="658dc-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="658dc-128">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="658dc-128">Feature</span></span> | <span data-ttu-id="658dc-129">Opzione 1</span><span class="sxs-lookup"><span data-stu-id="658dc-129">Option 1</span></span> | <span data-ttu-id="658dc-130">Opzione 2</span><span class="sxs-lookup"><span data-stu-id="658dc-130">Option 2</span></span> | <span data-ttu-id="658dc-131">Opzione 3</span><span class="sxs-lookup"><span data-stu-id="658dc-131">Option 3</span></span> | <span data-ttu-id="658dc-132">Opzione 4</span><span class="sxs-lookup"><span data-stu-id="658dc-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="658dc-133">Ottenere tutte le funzionalità incluse in Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="658dc-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="658dc-134">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-134">Yes</span></span> | <span data-ttu-id="658dc-135">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-135">Yes</span></span> | <span data-ttu-id="658dc-136">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-136">Yes</span></span> | <span data-ttu-id="658dc-137">No</span><span class="sxs-lookup"><span data-stu-id="658dc-137">No</span></span> |
| <span data-ttu-id="658dc-138">Numeri di telefono gestiti in Office 365?</span><span class="sxs-lookup"><span data-stu-id="658dc-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="658dc-139">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-139">Yes</span></span> | <span data-ttu-id="658dc-140">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-140">Yes</span></span> | <span data-ttu-id="658dc-141">No</span><span class="sxs-lookup"><span data-stu-id="658dc-141">No</span></span> | <span data-ttu-id="658dc-142">No</span><span class="sxs-lookup"><span data-stu-id="658dc-142">No</span></span> |
| <span data-ttu-id="658dc-143">Numeri di telefono gestiti sia in locale che in Office 365 (distribuzione ibrida)?</span><span class="sxs-lookup"><span data-stu-id="658dc-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="658dc-144">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-144">Yes</span></span> | <span data-ttu-id="658dc-145">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-145">Yes</span></span> | <span data-ttu-id="658dc-146">No</span><span class="sxs-lookup"><span data-stu-id="658dc-146">No</span></span> | <span data-ttu-id="658dc-147">No</span><span class="sxs-lookup"><span data-stu-id="658dc-147">No</span></span> |
| <span data-ttu-id="658dc-148">È possibile aggiungere un piano di chiamata vocale PSTN?</span><span class="sxs-lookup"><span data-stu-id="658dc-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="658dc-149">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-149">Yes</span></span> | <span data-ttu-id="658dc-150">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-150">Yes</span></span> | <span data-ttu-id="658dc-151">No</span><span class="sxs-lookup"><span data-stu-id="658dc-151">No</span></span> | <span data-ttu-id="658dc-152">No</span><span class="sxs-lookup"><span data-stu-id="658dc-152">No</span></span> |
| <span data-ttu-id="658dc-153">Conferenze PSTN?</span><span class="sxs-lookup"><span data-stu-id="658dc-153">PSTN Conferencing?</span></span> | <span data-ttu-id="658dc-154">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-154">Yes</span></span> | <span data-ttu-id="658dc-155">No</span><span class="sxs-lookup"><span data-stu-id="658dc-155">No</span></span> | <span data-ttu-id="658dc-156">No</span><span class="sxs-lookup"><span data-stu-id="658dc-156">No</span></span> | <span data-ttu-id="658dc-157">No</span><span class="sxs-lookup"><span data-stu-id="658dc-157">No</span></span> |
| <span data-ttu-id="658dc-158">Strumenti avanzati per la collaborazione, l'analisi e la sicurezza?</span><span class="sxs-lookup"><span data-stu-id="658dc-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="658dc-159">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-159">Yes</span></span> | <span data-ttu-id="658dc-160">No</span><span class="sxs-lookup"><span data-stu-id="658dc-160">No</span></span> | <span data-ttu-id="658dc-161">No</span><span class="sxs-lookup"><span data-stu-id="658dc-161">No</span></span> | <span data-ttu-id="658dc-162">No</span><span class="sxs-lookup"><span data-stu-id="658dc-162">No</span></span> |
| <span data-ttu-id="658dc-163">Report interattivi, dashboard e visualizzazioni dei dati?</span><span class="sxs-lookup"><span data-stu-id="658dc-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="658dc-164">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-164">Yes</span></span> | <span data-ttu-id="658dc-165">No</span><span class="sxs-lookup"><span data-stu-id="658dc-165">No</span></span> | <span data-ttu-id="658dc-166">No</span><span class="sxs-lookup"><span data-stu-id="658dc-166">No</span></span> | <span data-ttu-id="658dc-167">No</span><span class="sxs-lookup"><span data-stu-id="658dc-167">No</span></span> | 
| <span data-ttu-id="658dc-168">Maggiore controllo sulla sicurezza dei dati e sulla conformità con la privacy incorporata, la trasparenza e i controlli utente perfezionati?</span><span class="sxs-lookup"><span data-stu-id="658dc-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="658dc-169">Sì</span><span class="sxs-lookup"><span data-stu-id="658dc-169">Yes</span></span> | <span data-ttu-id="658dc-170">No</span><span class="sxs-lookup"><span data-stu-id="658dc-170">No</span></span> | <span data-ttu-id="658dc-171">No</span><span class="sxs-lookup"><span data-stu-id="658dc-171">No</span></span> | <span data-ttu-id="658dc-172">No</span><span class="sxs-lookup"><span data-stu-id="658dc-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="658dc-173">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="658dc-173">Transition customers to new product plans</span></span>

<span data-ttu-id="658dc-174">Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner.</span><span class="sxs-lookup"><span data-stu-id="658dc-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="658dc-175">In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate.</span><span class="sxs-lookup"><span data-stu-id="658dc-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="658dc-176">Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="658dc-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="658dc-177">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="658dc-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="658dc-178">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="658dc-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="658dc-179">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="658dc-179">Cancel the old subscription</span></span>

<span data-ttu-id="658dc-180">Seguire questa procedura per eseguire la migrazione della sottoscrizione di Office 365 Enterprise E4 di un cliente a una delle opzioni nella tabella precedente.</span><span class="sxs-lookup"><span data-stu-id="658dc-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="658dc-181">Passaggio 1: acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="658dc-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="658dc-182">Dal menu **centro partner** selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="658dc-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="658dc-183">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="658dc-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="658dc-184">Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione di Office 365 Enterprise E4 precedente e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="658dc-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="658dc-185">Passaggio 2: riassegnare le licenze degli utenti del cliente</span><span class="sxs-lookup"><span data-stu-id="658dc-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="658dc-186">Dal menu **centro** per i partner selezionare **Customers**, selezionare il cliente che si desidera spostare e quindi selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="658dc-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="658dc-187">Verrà visualizzata la pagina utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="658dc-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="658dc-188">Per riassegnare le licenze utente, selezionare l'utente da riassegnare, quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="658dc-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="658dc-189">Nella pagina **Gestisci licenze** deselezionare la casella di controllo licenza di **Office 365 Enterprise E4** e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando.</span><span class="sxs-lookup"><span data-stu-id="658dc-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="658dc-190">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="658dc-190">Select **Submit**.</span></span> <span data-ttu-id="658dc-191">Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="658dc-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="658dc-192">Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.</span><span class="sxs-lookup"><span data-stu-id="658dc-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="658dc-193">Dopo aver spostato le licenze utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata al livello superiore del cliente.</span><span class="sxs-lookup"><span data-stu-id="658dc-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="658dc-194">Passaggio 3: annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="658dc-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="658dc-195">Scegliere **clienti** dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="658dc-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="658dc-196">Selezionare il cliente da spostare e selezionare la sottoscrizione che si vuole annullare.</span><span class="sxs-lookup"><span data-stu-id="658dc-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="658dc-197">Nella pagina Dettagli sottoscrizione impostare lo stato della sottoscrizione su **sospeso**.</span><span class="sxs-lookup"><span data-stu-id="658dc-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="658dc-198">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="658dc-198">Select **Submit**.</span></span>

<span data-ttu-id="658dc-199">La sottoscrizione precedente viene sospesa e la nuova sottoscrizione è attiva.</span><span class="sxs-lookup"><span data-stu-id="658dc-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="658dc-200">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="658dc-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="658dc-201">Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="658dc-201">The customer incurs no additional costs for the old subscription.</span></span>



 



