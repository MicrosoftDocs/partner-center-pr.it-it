---
title: Creare sottoscrizioni clienti nel centro per i partner
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come vendere le sottoscrizioni dei clienti ai prodotti pubblicati da Microsoft e ai prodotti SaaS pubblicati da ISV di terze parti.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000525"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="33337-103">Creare, sospendere o annullare le sottoscrizioni dei clienti</span><span class="sxs-lookup"><span data-stu-id="33337-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="33337-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="33337-104">**Applies to**</span></span>

- <span data-ttu-id="33337-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="33337-105">Partner Center</span></span>
- <span data-ttu-id="33337-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="33337-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="33337-107">Partner CSP</span><span class="sxs-lookup"><span data-stu-id="33337-107">CSP partners</span></span>

<span data-ttu-id="33337-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="33337-108">**Appropriate roles**</span></span>

- <span data-ttu-id="33337-109">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="33337-109">Admin agent</span></span>
- <span data-ttu-id="33337-110">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="33337-110">Billing admin</span></span>
- <span data-ttu-id="33337-111">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="33337-111">Global admin</span></span>
- <span data-ttu-id="33337-112">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="33337-112">Helpdesk agent</span></span>
- <span data-ttu-id="33337-113">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="33337-113">Sales agent</span></span>

<span data-ttu-id="33337-114">Dopo aver creato un record del cliente nel Centro per i partner, puoi vendere loro sottoscrizioni per i prodotti nel catalogo.</span><span class="sxs-lookup"><span data-stu-id="33337-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="33337-115">Sono inclusi i prodotti pubblicati da Microsoft, oltre ai prodotti SaaS (software as a Service) pubblicati da fornitori di software indipendenti (ISV) di terze parti nel [Marketplace commerciale](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="33337-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="33337-116">Alcune offerte sono limitate a una sottoscrizione per cliente.</span><span class="sxs-lookup"><span data-stu-id="33337-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="33337-117">Per vedere l'elenco delle offerte limitate, visita la pagina Prezzi e offerte del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="33337-118">Come partner del programma CSP, è possibile acquistare solo sottoscrizioni Saas **basate su licenza** dagli editori ISV all'interno del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="33337-119">Ciò significa che è possibile acquistare qualsiasi offerta SaaS **basata su licenze** che l'editore ISV ha reso disponibile, incluse le [offerte esclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a cui si ha accesso.</span><span class="sxs-lookup"><span data-stu-id="33337-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="33337-120">Per acquistare o gestire altre offerte del Marketplace commerciale dagli ISV, ad esempio offerte basate **sull'utilizzo**, a consumo o a consumo che coinvolgono applicazioni, contenitori o macchine virtuali di Azure, è necessario accedere al portale di [gestione di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="33337-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="33337-121">Per ulteriori informazioni, vedere [acquistare prodotti Marketplace commerciali](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="33337-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="33337-122">Creare una nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="33337-122">Create a new subscription</span></span>

1. <span data-ttu-id="33337-123">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="33337-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="33337-124">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="33337-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="33337-125">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="33337-125">Select **Add subscription**.</span></span> <span data-ttu-id="33337-126">La scheda **Online Services** mostrerà tutte le offerte SaaS del Marketplace disponibili.</span><span class="sxs-lookup"><span data-stu-id="33337-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="33337-127">Per visualizzare solo determinati tipi di sottoscrizioni, effettua le selezioni nei filtri disponibili:</span><span class="sxs-lookup"><span data-stu-id="33337-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="33337-128">**Autore**: scegliere **Microsoft** per visualizzare solo le offerte di Microsoft o il **partner** per vedere i prodotti commerciali del Marketplace pubblicati dagli ISV.</span><span class="sxs-lookup"><span data-stu-id="33337-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="33337-129">**Tipo di fatturazione**: selezionare il tipo di fatturazione per la sottoscrizione che si vuole usare: **licenza** o **utilizzo**.</span><span class="sxs-lookup"><span data-stu-id="33337-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="33337-130">Per informazioni che consentano di decidere tra la frequenza di fatturazione mensile e annuale, vedere [fatturazione basata sulle licenze](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="33337-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="33337-131">**Categoria**: scegliere **Enterprise**, **Small Business**o **Trial**.</span><span class="sxs-lookup"><span data-stu-id="33337-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="33337-132">Per informazioni sulle sottoscrizioni di versioni di valutazione, vedi [Offrire ai clienti le versioni di valutazione dei prodotti Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="33337-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="33337-133">Selezionare le sottoscrizioni di prodotto che si desidera acquistare per il cliente.</span><span class="sxs-lookup"><span data-stu-id="33337-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="33337-134">I prodotti visualizzati dipendono dal tipo di segmento dei clienti (Education, Government e così via) e dai filtri applicati.</span><span class="sxs-lookup"><span data-stu-id="33337-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="33337-135">Alcune offerte visualizzate sul Marketplace potrebbero non essere sempre disponibili per un cliente specifico o per un partner CSP specifico.</span><span class="sxs-lookup"><span data-stu-id="33337-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="33337-136">Il motivo può essere il seguente:</span><span class="sxs-lookup"><span data-stu-id="33337-136">This can be because:</span></span>

   - <span data-ttu-id="33337-137">Il cliente dispone già di una sottoscrizione a tale prodotto e ne è consentito solo uno</span><span class="sxs-lookup"><span data-stu-id="33337-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="33337-138">La sottoscrizione del cliente potrebbe essere stata sospesa. in questo caso, è possibile riattivare la sottoscrizione anziché acquistarne una nuova.</span><span class="sxs-lookup"><span data-stu-id="33337-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="33337-139">Per le offerte SaaS ISV, potrebbero esserci alcuni motivi per cui l'offerta non è disponibile per l'acquisto: l'ISV potrebbe non supportare il paese o l'area di fatturazione del cliente; l'ISV potrebbe aver scelto di non rendere disponibile l'offerta tramite il programma CSP; in alternativa, l'ISV potrebbe avere reso l'offerta [esclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo per determinati partner CSP.</span><span class="sxs-lookup"><span data-stu-id="33337-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="33337-140">L'offerta ISV potrebbe anche non essere transazionale tramite il centro per i partner, ad esempio i contenitori o alcune offerte basate sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="33337-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="33337-141">Per ogni sottoscrizione che si vuole aggiungere, immettere il numero di licenze (se necessario) e selezionare **Aggiungi al carrello**.</span><span class="sxs-lookup"><span data-stu-id="33337-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="33337-142">Al termine dell'aggiunta delle sottoscrizioni, selezionare **Revisione** ed esaminare l'ordine.</span><span class="sxs-lookup"><span data-stu-id="33337-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="33337-143">Dopo aver esaminato gli ordini ed è possibile acquistare tali sottoscrizioni, selezionare **Acquista**.</span><span class="sxs-lookup"><span data-stu-id="33337-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="33337-144">Dopo aver acquistato una sottoscrizione per un cliente, si verificherà quanto segue:</span><span class="sxs-lookup"><span data-stu-id="33337-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="33337-145">È possibile esaminare o modificare la sottoscrizione selezionando il nome della sottoscrizione dalla pagina **sottoscrizioni** del cliente.</span><span class="sxs-lookup"><span data-stu-id="33337-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="33337-146">In tale pagina puoi selezionare licenze per componenti aggiuntivi (se disponibili), modificare la quantità di licenze o sospendere la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="33337-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="33337-147">**Per le sottoscrizioni SaaS (basate su licenza) ISV:**</span><span class="sxs-lookup"><span data-stu-id="33337-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="33337-148">Si riceverà un collegamento al sito dell'editore ISV.</span><span class="sxs-lookup"><span data-stu-id="33337-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="33337-149">Questo collegamento dovrebbe aiutare a completare la distribuzione o la configurazione dell'account della sottoscrizione del cliente.</span><span class="sxs-lookup"><span data-stu-id="33337-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="33337-150">Né l'utente né il cliente riceveranno un messaggio di posta elettronica con le istruzioni per completare la configurazione e il provisioning dell'account per questo tipo di sottoscrizione ISV.</span><span class="sxs-lookup"><span data-stu-id="33337-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="33337-151">Se la sottoscrizione viene fornita con una versione di valutazione gratuita di 30 giorni, il periodo di valutazione gratuito verrà applicato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="33337-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="33337-152">I partner del programma CSP non possono rinunciare al periodo di valutazione gratuito sulle offerte acquistate per i clienti.</span><span class="sxs-lookup"><span data-stu-id="33337-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="33337-153">Una volta terminato il periodo di valutazione gratuita, viene avviato il periodo di validità della sottoscrizione e la sottoscrizione viene convertita in stato a pagamento.</span><span class="sxs-lookup"><span data-stu-id="33337-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="33337-154">La sottoscrizione verrà quindi rinnovata automaticamente in base alla stessa pianificazione.</span><span class="sxs-lookup"><span data-stu-id="33337-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="33337-155">Aggiornare le sottoscrizioni con i componenti aggiuntivi</span><span class="sxs-lookup"><span data-stu-id="33337-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="33337-156">Per acquistare un componente aggiuntivo, il cliente deve avere prima una sottoscrizione di base attiva.</span><span class="sxs-lookup"><span data-stu-id="33337-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="33337-157">Non è possibile acquistare i componenti aggiuntivi tramite il catalogo.</span><span class="sxs-lookup"><span data-stu-id="33337-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="33337-158">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="33337-159">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="33337-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="33337-160">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="33337-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="33337-161">Sotto la sezione **stato** , sono elencati i componenti aggiuntivi disponibili per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="33337-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="33337-162">Aggiornare la quantità di licenze per ogni componente aggiuntivo richiesto.</span><span class="sxs-lookup"><span data-stu-id="33337-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="33337-163">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="33337-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="33337-164">La possibilità di acquistare componenti aggiuntivi tramite il centro per i partner è disponibile solo per la fatturazione diretta e i provider indiretti.</span><span class="sxs-lookup"><span data-stu-id="33337-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="33337-165">Vengono visualizzati solo i componenti aggiuntivi idonei in base ai requisiti di base e alla disponibilità a livello di area.</span><span class="sxs-lookup"><span data-stu-id="33337-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="33337-166">Per altre informazioni su prezzi e offerte, fare riferimento alla matrice di offerte del rivenditore cloud.</span><span class="sxs-lookup"><span data-stu-id="33337-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="33337-167">La sospensione della sottoscrizione di base comporta anche la sospensione di tutti i componenti aggiuntivi associati.</span><span class="sxs-lookup"><span data-stu-id="33337-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="33337-168">Le date di inizio per i componenti aggiuntivi sono allineate alla sottoscrizione di base e gli addebiti vengono calcolati dalla data di inizio e dalla data di fine dell'addebito con addebiti proporzionali nella prima fattura.</span><span class="sxs-lookup"><span data-stu-id="33337-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="33337-169">Per ulteriori informazioni, vedere [fatturazione basata su licenze](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="33337-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="33337-170">Sospendere o annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="33337-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="33337-171">I partner possono sospendere o annullare una sottoscrizione se richiesto dal cliente o in caso di insolvenza o frode.</span><span class="sxs-lookup"><span data-stu-id="33337-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="33337-172">Sospendere una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="33337-172">Suspend a subscription</span></span>

<span data-ttu-id="33337-173">Quando cambi lo stato di una sottoscrizione in **Sospesa**, gli utenti non possono accedere alla sottoscrizione o ai servizi.</span><span class="sxs-lookup"><span data-stu-id="33337-173">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="33337-174">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="33337-175">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="33337-175">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="33337-176">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="33337-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="33337-177">Nella sezione **Stato**, scegliere **Sospesa**.</span><span class="sxs-lookup"><span data-stu-id="33337-177">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="33337-178">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="33337-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="33337-179">Verranno eliminati tutti i dati, tranne nel caso in cui la sottoscrizione venga riattivata entro 90 giorni o 90 giorni più il numero di giorni tra il momento in cui l'account è stato aperto e il primo periodo di fatturazione (massimo 120 giorni).</span><span class="sxs-lookup"><span data-stu-id="33337-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="33337-180">Quando sospendi una sottoscrizione, la data visualizzata sotto il pulsante **Sospesa** indica quando la sottoscrizione scadrà automaticamente se non la riattivi.</span><span class="sxs-lookup"><span data-stu-id="33337-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="33337-181">Annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="33337-181">Cancel a subscription</span></span>

<span data-ttu-id="33337-182">È possibile scegliere di annullare le sottoscrizioni SaaS basate su licenza da autori ISV di terze parti all'interno del [Marketplace commerciale](csp-commercial-marketplace-overview.md)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="33337-183">Fino a quando l'annullamento viene annullato entro il periodo di annullamento, si riceverà un rimborso completo.</span><span class="sxs-lookup"><span data-stu-id="33337-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="33337-184">Per le offerte ISV fatturate mensilmente:</span><span class="sxs-lookup"><span data-stu-id="33337-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="33337-185">Se si annulla meno di 24 ore dopo aver effettuato l'ordine, si riceverà un credito completo per la fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="33337-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="33337-186">Se si annulla l'annullamento in seguito a 24 ore dopo l'esecuzione dell'ordine, l'annullamento verrà pianificato per il rinnovo.</span><span class="sxs-lookup"><span data-stu-id="33337-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="33337-187">Per le offerte fatturate annualmente:</span><span class="sxs-lookup"><span data-stu-id="33337-187">For offers billed annually:</span></span>

- <span data-ttu-id="33337-188">Se si annulla meno di 14 giorni dopo aver effettuato l'ordine, si riceverà un credito completo per la fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="33337-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="33337-189">Se si annulla dopo 14 giorni dopo aver inserito l'ordine, l'annullamento verrà pianificato per il rinnovo.</span><span class="sxs-lookup"><span data-stu-id="33337-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="33337-190">Al termine di questi periodi, non verrà più visualizzata l'opzione per annullare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="33337-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="33337-191">I servizi ISV di terze parti basati sull'utilizzo e a consumo (che usano macchine virtuali o contenitori, ad esempio) non sono idonei per la restituzione.</span><span class="sxs-lookup"><span data-stu-id="33337-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="33337-192">Il deprovisioning dei servizi basati sull'utilizzo può essere effettuato come un metodo di annullamento.</span><span class="sxs-lookup"><span data-stu-id="33337-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="33337-193">Poiché i costi vengono addebitati dopo l'utilizzo, questi servizi non sono idonei per un rimborso.</span><span class="sxs-lookup"><span data-stu-id="33337-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="33337-194">Per annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="33337-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="33337-195">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="33337-196">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="33337-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="33337-197">Individuare la sottoscrizione che si vuole annullare.</span><span class="sxs-lookup"><span data-stu-id="33337-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="33337-198">Nella colonna **stato** selezionare **Annulla**.</span><span class="sxs-lookup"><span data-stu-id="33337-198">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="33337-199">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="33337-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="33337-200">Se viene visualizzata una finestra di dialogo, compilare eventuali dettagli rilevanti, quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="33337-200">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="33337-201">Per confermare l'annullamento, selezionare **Sì, Annulla**.</span><span class="sxs-lookup"><span data-stu-id="33337-201">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="33337-202">È anche possibile scegliere di annullare una sottoscrizione di Azure Marketplace usando le API.</span><span class="sxs-lookup"><span data-stu-id="33337-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="33337-203">A tale scopo, vedere [annullare una sottoscrizione di Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="33337-203">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="33337-204">Scegliere se rinnovare automaticamente una sottoscrizione del Marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="33337-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="33337-205">Per impostazione predefinita, le sottoscrizioni attive sono impostate in modo da essere rinnovate automaticamente al termine del periodo di sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="33337-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="33337-206">Per le [sottoscrizioni ai prodotti Marketplace commerciali](csp-commercial-marketplace-overview.md), è possibile scegliere di non rinnovare automaticamente la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="33337-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="33337-207">Per arrestare una sottoscrizione del Marketplace commerciale attiva dal rinnovo automatico:</span><span class="sxs-lookup"><span data-stu-id="33337-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="33337-208">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="33337-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="33337-209">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="33337-209">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="33337-210">Selezionare **Sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="33337-210">Select **Subscriptions**.</span></span> <span data-ttu-id="33337-211">Verranno elencate tutte le sottoscrizioni basate sulle licenze acquistate per il cliente.</span><span class="sxs-lookup"><span data-stu-id="33337-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="33337-212">Nella colonna **sottoscrizione** selezionare la sottoscrizione che si desidera modificare.</span><span class="sxs-lookup"><span data-stu-id="33337-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="33337-213">Nella pagina Dettagli sottoscrizione individuare la sezione **stato** e deselezionare la casella **rinnovo automatico** .</span><span class="sxs-lookup"><span data-stu-id="33337-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="33337-214">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="33337-214">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="33337-215">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="33337-215">Next steps</span></span>

- [<span data-ttu-id="33337-216">Acquistare prodotti del Marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="33337-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="33337-217">Gestione dei prodotti del Marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="33337-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="33337-218">Panoramica del marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="33337-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)