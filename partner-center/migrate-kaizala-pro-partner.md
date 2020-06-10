---
title: Eseguire la migrazione di sottoscrizioni Kaizala Pro a Microsoft365
description: Informazioni su come eseguire la migrazione di sottoscrizioni Kaizala Pro a Microsoft365 o versioni di Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611237"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="5b99d-103">Eseguire la migrazione di sottoscrizioni Kaizala Pro autonome a Microsoft365 o versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="5b99d-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="5b99d-104">A partire dal 1 ° luglio 2020, Microsoft sta terminando le vendite del servizio Kaizala Pro autonomo.</span><span class="sxs-lookup"><span data-stu-id="5b99d-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="5b99d-105">I clienti non saranno più in grado di acquistare nuove sottoscrizioni Kaizala Pro dopo questa data e le sottoscrizioni Kaizala Pro esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="5b99d-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="5b99d-106">Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni Kaizala Pro autonome in scadenza a un'opzione SKU supportata, elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="5b99d-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="5b99d-107">È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="5b99d-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="5b99d-108">Se si usa l'API (CREST o centro per i partner), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà rinnovo automatico impostata su false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="5b99d-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="5b99d-109">Le sottoscrizioni E4 verranno impostate `auto renew=False` su il 1 ° luglio 2020.</span><span class="sxs-lookup"><span data-stu-id="5b99d-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="5b99d-110">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="5b99d-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="5b99d-111">Piani di sostituzione Kaizala Pro autonomo</span><span class="sxs-lookup"><span data-stu-id="5b99d-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="5b99d-112">Con i nuovi piani, i clienti possono sfruttare le funzionalità e le funzionalità più recenti in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5b99d-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="5b99d-113">I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="5b99d-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="5b99d-114">[**Microsoft 365 per le aziende**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), tra cui:</span><span class="sxs-lookup"><span data-stu-id="5b99d-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="5b99d-115">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="5b99d-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="5b99d-116">Microsoft 365 Business standard</span><span class="sxs-lookup"><span data-stu-id="5b99d-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="5b99d-117">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="5b99d-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="5b99d-118">[**Microsoft 365 per Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), tra cui:</span><span class="sxs-lookup"><span data-stu-id="5b99d-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="5b99d-119">Microsoft 365 F3 (in precedenza Microsoft 365 F1) e Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="5b99d-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="5b99d-120">[**Microsoft 365 per Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), tra cui:</span><span class="sxs-lookup"><span data-stu-id="5b99d-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="5b99d-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="5b99d-121">Office 365 E1</span></span>
   - <span data-ttu-id="5b99d-122">Microsoft 365 E3 e Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="5b99d-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="5b99d-123">Microsoft 365 E5 e Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="5b99d-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="5b99d-124">[**Microsoft 365 per la formazione**](https://www.microsoft.com/education/buy-license/microsoft365), tra cui:</span><span class="sxs-lookup"><span data-stu-id="5b99d-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="5b99d-125">Microsoft 365 a1 e Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="5b99d-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="5b99d-126">Microsoft 365 a3 e Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="5b99d-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="5b99d-127">Microsoft 365 a5 e Office 365 a5</span><span class="sxs-lookup"><span data-stu-id="5b99d-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5b99d-128">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="5b99d-128">Transition customers to new product plans</span></span>

<span data-ttu-id="5b99d-129">Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner.</span><span class="sxs-lookup"><span data-stu-id="5b99d-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="5b99d-130">In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate.</span><span class="sxs-lookup"><span data-stu-id="5b99d-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="5b99d-131">Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="5b99d-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="5b99d-132">A.</span><span class="sxs-lookup"><span data-stu-id="5b99d-132">A.</span></span> <span data-ttu-id="5b99d-133">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="5b99d-133">Purchase the new subscription</span></span>

<span data-ttu-id="5b99d-134">B.</span><span class="sxs-lookup"><span data-stu-id="5b99d-134">B.</span></span> <span data-ttu-id="5b99d-135">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="5b99d-135">Reassign current user licenses</span></span>

<span data-ttu-id="5b99d-136">C.</span><span class="sxs-lookup"><span data-stu-id="5b99d-136">C.</span></span> <span data-ttu-id="5b99d-137">Annulla sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="5b99d-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="5b99d-138">Esegui la migrazione dei clienti ai nuovi piani</span><span class="sxs-lookup"><span data-stu-id="5b99d-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="5b99d-139">A.</span><span class="sxs-lookup"><span data-stu-id="5b99d-139">A.</span></span> <span data-ttu-id="5b99d-140">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="5b99d-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="5b99d-141">Per acquistare la nuova sottoscrizione, scegliere **Customers**dal menu centro per i **partner** , selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="5b99d-142">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).</span><span class="sxs-lookup"><span data-stu-id="5b99d-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="5b99d-143">Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la vecchia sottoscrizione Kaizala Pro autonoma e la nuova sottoscrizione di destinazione, ad esempio, l'opzione 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="5b99d-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="5b99d-144">B.</span><span class="sxs-lookup"><span data-stu-id="5b99d-144">B.</span></span> <span data-ttu-id="5b99d-145">Riassegna licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="5b99d-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="5b99d-146">Per riassegnare le licenze degli utenti del cliente, dal menu **centro** per i partner selezionare **clienti**, selezionare il cliente da trasferire, quindi selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="5b99d-147">Verrà visualizzata la pagina utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="5b99d-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="5b99d-148">Per riassegnare la licenza utente, selezionare l'utente da riassegnare, quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="5b99d-149">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Kaizala Pro standalone License e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta muovendo il cliente.</span><span class="sxs-lookup"><span data-stu-id="5b99d-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="5b99d-150">Selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-150">Select **Submit**.</span></span> <span data-ttu-id="5b99d-151">Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="5b99d-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="5b99d-152">Continuare lo stesso processo per gli altri utenti che necessitano di assegnazioni di licenze.</span><span class="sxs-lookup"><span data-stu-id="5b99d-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="5b99d-153">C.</span><span class="sxs-lookup"><span data-stu-id="5b99d-153">C.</span></span> <span data-ttu-id="5b99d-154">Annulla sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="5b99d-154">Cancel old subscription</span></span>

<span data-ttu-id="5b99d-155">Dopo aver spostato la licenza utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata a livello di cliente.</span><span class="sxs-lookup"><span data-stu-id="5b99d-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="5b99d-156">Scegliere **clienti**dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="5b99d-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="5b99d-157">Selezionare il cliente di cui annullare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="5b99d-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="5b99d-158">Nella pagina Dettagli sottoscrizione impostare la sottoscrizione su **sospesa**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="5b99d-159">Selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="5b99d-159">Select **Submit**.</span></span>

<span data-ttu-id="5b99d-160">La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva.</span><span class="sxs-lookup"><span data-stu-id="5b99d-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="5b99d-161">Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="5b99d-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="5b99d-162">Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="5b99d-162">The customer incurs no additional costs for the old subscription.</span></span>
