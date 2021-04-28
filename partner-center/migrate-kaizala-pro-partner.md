---
title: Eseguire la migrazione delle sottoscrizioni Kaizala Pro a Microsoft 365
description: Informazioni su come eseguire la migrazione delle sottoscrizioni di Kaizala Pro Microsoft 365 versioni di Office 365. Per altre informazioni sulla transizione dei clienti, vedere questo articolo.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172405"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="ef86b-104">Eseguire la migrazione delle sottoscrizioni autonome di Kaizala Pro Microsoft 365 versioni di Office 365</span><span class="sxs-lookup"><span data-stu-id="ef86b-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="ef86b-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="ef86b-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ef86b-106">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="ef86b-106">Sales agent</span></span>

<span data-ttu-id="ef86b-107">A partire dal 1° luglio 2020, Microsoft termina le vendite del servizio autonomo Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="ef86b-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="ef86b-108">I clienti non potranno più acquistare nuove sottoscrizioni Kaizala Pro dopo questa data e le sottoscrizioni Kaizala Pro esistenti non verranno rinnovate automaticamente alla scadenza.</span><span class="sxs-lookup"><span data-stu-id="ef86b-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ef86b-109">Per garantire la continuità per i clienti, è consigliabile eseguire la transizione dei clienti con sottoscrizioni autonome di Kaizala Pro in scadenza a un'opzione SKU supportata, elencata di seguito.</span><span class="sxs-lookup"><span data-stu-id="ef86b-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ef86b-110">È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.</span><span class="sxs-lookup"><span data-stu-id="ef86b-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ef86b-111">Se si usa l'API (STEMM o Partner Center), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà di rinnovo automatico impostata su false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="ef86b-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="ef86b-112">Le sottoscrizioni E4 verranno impostate su `auto renew=False` il 1° luglio 2020.</span><span class="sxs-lookup"><span data-stu-id="ef86b-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="ef86b-113">È possibile spostare i clienti in un nuovo piano in qualsiasi momento.</span><span class="sxs-lookup"><span data-stu-id="ef86b-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="ef86b-114">Piani di sostituzione autonoma di Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="ef86b-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="ef86b-115">Con i nuovi piani, i clienti possono sfruttare le funzionalità e le funzionalità più nuove in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ef86b-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="ef86b-116">I dettagli dei prezzi sono disponibili nel listino prezzi e nella matrice del listino Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ef86b-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="ef86b-117">[**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)tra cui:</span><span class="sxs-lookup"><span data-stu-id="ef86b-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="ef86b-118">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="ef86b-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="ef86b-119">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="ef86b-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="ef86b-120">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ef86b-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="ef86b-121">[**Microsoft 365 per Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)tra cui:</span><span class="sxs-lookup"><span data-stu-id="ef86b-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="ef86b-122">Microsoft 365 F3 (in precedenza Microsoft 365 F1) e Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="ef86b-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="ef86b-123">[**Microsoft 365 per Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)tra cui:</span><span class="sxs-lookup"><span data-stu-id="ef86b-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="ef86b-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="ef86b-124">Office 365 E1</span></span>
   - <span data-ttu-id="ef86b-125">Microsoft 365 E3 e Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="ef86b-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="ef86b-126">Microsoft 365 E5 e Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="ef86b-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="ef86b-127">[**Microsoft 365 per Education,**](https://www.microsoft.com/education/buy-license/microsoft365)tra cui:</span><span class="sxs-lookup"><span data-stu-id="ef86b-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="ef86b-128">Microsoft 365 A1 e Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="ef86b-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="ef86b-129">Microsoft 365 A3 e Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="ef86b-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="ef86b-130">Microsoft 365 A5 e Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="ef86b-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ef86b-131">Transizione dei clienti ai nuovi piani per i prodotti</span><span class="sxs-lookup"><span data-stu-id="ef86b-131">Transition customers to new product plans</span></span>

<span data-ttu-id="ef86b-132">Microsoft offre continuamente nuovi prodotti e servizi ai partner.</span><span class="sxs-lookup"><span data-stu-id="ef86b-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ef86b-133">In questi casi, potrebbe essere necessario aggiornare i clienti a nuovi servizi o eseguire la migrazione delle sottoscrizioni dagli SKU che verranno arrestati.</span><span class="sxs-lookup"><span data-stu-id="ef86b-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ef86b-134">La migrazione dei clienti da SKU ritirati a SKU più recenti richiede i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="ef86b-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="ef86b-135">A.</span><span class="sxs-lookup"><span data-stu-id="ef86b-135">A.</span></span> <span data-ttu-id="ef86b-136">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ef86b-136">Purchase the new subscription</span></span>

<span data-ttu-id="ef86b-137">B.</span><span class="sxs-lookup"><span data-stu-id="ef86b-137">B.</span></span> <span data-ttu-id="ef86b-138">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="ef86b-138">Reassign current user licenses</span></span>

<span data-ttu-id="ef86b-139">C.</span><span class="sxs-lookup"><span data-stu-id="ef86b-139">C.</span></span> <span data-ttu-id="ef86b-140">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="ef86b-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="ef86b-141">Eseguire la migrazione dei clienti a nuovi piani</span><span class="sxs-lookup"><span data-stu-id="ef86b-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="ef86b-142">A.</span><span class="sxs-lookup"><span data-stu-id="ef86b-142">A.</span></span> <span data-ttu-id="ef86b-143">Acquistare la nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ef86b-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="ef86b-144">Per acquistare la nuova sottoscrizione, dal menu **Partner Center** clienti selezionare **Clienti,** selezionare il cliente che si vuole spostare e quindi selezionare **Aggiungi sottoscrizioni.**</span><span class="sxs-lookup"><span data-stu-id="ef86b-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="ef86b-145">Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="ef86b-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="ef86b-146">Il cliente dovrebbe ora avere sia sottoscrizioni nuove che vecchie, la sottoscrizione kaizala pro autonoma precedente e la nuova sottoscrizione "di destinazione", ad esempio Option 1 - Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="ef86b-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="ef86b-147">B.</span><span class="sxs-lookup"><span data-stu-id="ef86b-147">B.</span></span> <span data-ttu-id="ef86b-148">Riassegnare le licenze utente correnti</span><span class="sxs-lookup"><span data-stu-id="ef86b-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="ef86b-149">Per riassegnare le licenze degli utenti del cliente, dal menu **Partner Center** selezionare **Clienti,** selezionare il cliente che si sta spostando e quindi selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="ef86b-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="ef86b-150">Verrà visualizzata la pagina Utenti e licenze del cliente.</span><span class="sxs-lookup"><span data-stu-id="ef86b-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ef86b-151">Per riassegnare la licenza utente, selezionare l'utente da riassegnare e quindi selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="ef86b-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="ef86b-152">Nella pagina **Gestisci licenze** deselezionare la casella di controllo Licenza autonoma Kaizala Pro e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta passando.</span><span class="sxs-lookup"><span data-stu-id="ef86b-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="ef86b-153">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="ef86b-153">Select **Submit**.</span></span> <span data-ttu-id="ef86b-154">Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.</span><span class="sxs-lookup"><span data-stu-id="ef86b-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="ef86b-155">Continuare lo stesso processo per altri utenti che necessitano di assegnazioni di licenze.</span><span class="sxs-lookup"><span data-stu-id="ef86b-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="ef86b-156">C.</span><span class="sxs-lookup"><span data-stu-id="ef86b-156">C.</span></span> <span data-ttu-id="ef86b-157">Annullare la sottoscrizione precedente</span><span class="sxs-lookup"><span data-stu-id="ef86b-157">Cancel old subscription</span></span>

<span data-ttu-id="ef86b-158">Dopo aver spostata la licenza utente nel nuovo servizio, è possibile annullare in modo sicuro la sottoscrizione ritirata a livello di cliente.</span><span class="sxs-lookup"><span data-stu-id="ef86b-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="ef86b-159">Dal menu **Partner Center** selezionare **Clienti.**</span><span class="sxs-lookup"><span data-stu-id="ef86b-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="ef86b-160">Selezionare il cliente di cui si sta annullando la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ef86b-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="ef86b-161">Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione su **Sospeso.**</span><span class="sxs-lookup"><span data-stu-id="ef86b-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="ef86b-162">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="ef86b-162">Select **Submit**.</span></span>

<span data-ttu-id="ef86b-163">La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva.</span><span class="sxs-lookup"><span data-stu-id="ef86b-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="ef86b-164">Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni.</span><span class="sxs-lookup"><span data-stu-id="ef86b-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ef86b-165">Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.</span><span class="sxs-lookup"><span data-stu-id="ef86b-165">The customer incurs no additional costs for the old subscription.</span></span>
