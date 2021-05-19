---
title: Creare sottoscrizioni dei clienti in Partner Center
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come vendere sottoscrizioni ai clienti per i prodotti pubblicati da Microsoft e i prodotti SaaS pubblicati da ISV di terze parti.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148200"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="d71c9-103">Creare, sospendere o annullare le sottoscrizioni dei clienti</span><span class="sxs-lookup"><span data-stu-id="d71c9-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="d71c9-104">**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d71c9-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d71c9-105">**Ruoli appropriati:** agente di amministrazione | Amministratore fatturazione | Amministratore globale | Agente del supporto | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="d71c9-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="d71c9-106">Dopo aver creato un record del cliente nel Centro per i partner, puoi vendere loro sottoscrizioni per i prodotti nel catalogo.</span><span class="sxs-lookup"><span data-stu-id="d71c9-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="d71c9-107">Sono inclusi i prodotti pubblicati da Microsoft e dai prodotti SaaS (Software as a Service) pubblicati da fornitori di software indipendenti (ISV) di terze parti nel [marketplace commerciale.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="d71c9-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="d71c9-108">Alcune offerte sono limitate a una sottoscrizione per cliente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="d71c9-109">Per vedere l'elenco delle offerte limitate, visita la pagina Prezzi e offerte del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d71c9-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d71c9-110">I partner del programma CSP possono  acquistare sottoscrizioni **SaaS** basate su licenza o a consumo da editori ISV all'interno Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d71c9-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="d71c9-111">Ciò significa che è possibile acquistare **qualsiasi** offerta **SaaS** basata su licenza o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a consumo resa disponibile dall'editore isv, incluse le offerte esclusive a cui si ha accesso.</span><span class="sxs-lookup"><span data-stu-id="d71c9-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="d71c9-112">Per acquistare o gestire altre offerte del marketplace commerciale dagli ISV (ad esempio offerte basate sull'utilizzo che coinvolgono applicazioni di Azure, contenitori o macchine virtuali), è necessario passare al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d71c9-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="d71c9-113">Creare una nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="d71c9-113">Create a new subscription</span></span>

1. <span data-ttu-id="d71c9-114">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d71c9-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d71c9-115">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d71c9-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d71c9-116">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="d71c9-116">Select **Add subscription**.</span></span> <span data-ttu-id="d71c9-117">La **scheda Online Services** (Servizi online) mostrerà tutte le offerte SaaS del Marketplace disponibili.</span><span class="sxs-lookup"><span data-stu-id="d71c9-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="d71c9-118">Per visualizzare solo determinati tipi di sottoscrizioni, effettua le selezioni nei filtri disponibili:</span><span class="sxs-lookup"><span data-stu-id="d71c9-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="d71c9-119">**Editore:** **scegliere Microsoft** per visualizzare solo le offerte di Microsoft o **Partner per** visualizzare i prodotti del marketplace commerciale pubblicati dagli ISV.</span><span class="sxs-lookup"><span data-stu-id="d71c9-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="d71c9-120">**Tipo di fatturazione:** selezionare il tipo di fatturazione della sottoscrizione da usare: **Licenza** o **Utilizzo.**</span><span class="sxs-lookup"><span data-stu-id="d71c9-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="d71c9-121">Per [informazioni utili per](license-based-billing.md) decidere tra la frequenza di fatturazione mensile e annuale, vedere Fatturazione basata su licenza.</span><span class="sxs-lookup"><span data-stu-id="d71c9-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="d71c9-122">**Categoria:** scegliere **Enterprise,** **Small Business** o **Versione di valutazione.**</span><span class="sxs-lookup"><span data-stu-id="d71c9-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="d71c9-123">Per informazioni sulle sottoscrizioni di versioni di valutazione, vedi [Offrire ai clienti le versioni di valutazione dei prodotti Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="d71c9-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="d71c9-124">Selezionare le sottoscrizioni al prodotto da acquistare per il cliente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="d71c9-125">I prodotti visualizzati dipendono dal tipo di segmento di cliente (istruzione, enti pubblici e così via) e dai filtri applicati.</span><span class="sxs-lookup"><span data-stu-id="d71c9-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="d71c9-126">Alcune offerte visualizzate nel Marketplace potrebbero non essere sempre disponibili per un cliente specifico o per un partner CSP specifico.</span><span class="sxs-lookup"><span data-stu-id="d71c9-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="d71c9-127">Ciò può essere dovuto al seguente:</span><span class="sxs-lookup"><span data-stu-id="d71c9-127">This can be because:</span></span>

   - <span data-ttu-id="d71c9-128">Il cliente ha già una sottoscrizione a tale prodotto e ne è consentito solo uno</span><span class="sxs-lookup"><span data-stu-id="d71c9-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="d71c9-129">La sottoscrizione del cliente potrebbe essere stata sospesa. In questo caso, è possibile riattivare la sottoscrizione anziché acquistarne una nuova.</span><span class="sxs-lookup"><span data-stu-id="d71c9-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="d71c9-130">Per le offerte SaaS ISV, possono esserci alcuni motivi per cui l'offerta non è disponibile per l'acquisto: l'ISV potrebbe non supportare il paese o l'area di fatturazione del cliente; l'ISV potrebbe aver scelto di non rendere disponibile l'offerta tramite il programma CSP; oppure l'ISV potrebbe aver reso l'offerta [esclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo a determinati partner CSP.</span><span class="sxs-lookup"><span data-stu-id="d71c9-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="d71c9-131">L'offerta ISV potrebbe anche non essere transazionabile tramite il Partner Center (ad esempio, contenitori o alcune offerte basate sull'utilizzo).</span><span class="sxs-lookup"><span data-stu-id="d71c9-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="d71c9-132">Per ogni sottoscrizione da aggiungere, immettere il numero di licenze (se necessario) e selezionare **Aggiungi al carrello.**</span><span class="sxs-lookup"><span data-stu-id="d71c9-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="d71c9-133">Al termine dell'aggiunta delle sottoscrizioni, selezionare **Rivedi** ed esamina l'ordine.</span><span class="sxs-lookup"><span data-stu-id="d71c9-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="d71c9-134">Dopo aver esaminato gli ordini e aver pronti per l'acquisto di queste sottoscrizioni, selezionare **Acquista**.</span><span class="sxs-lookup"><span data-stu-id="d71c9-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="d71c9-135">Dopo aver acquistato una sottoscrizione per un cliente, si verificheranno le condizioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d71c9-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="d71c9-136">È possibile esaminare o modificare la sottoscrizione selezionando il nome della sottoscrizione dalla pagina **Sottoscrizioni del** cliente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="d71c9-137">In tale pagina puoi selezionare licenze per componenti aggiuntivi (se disponibili), modificare la quantità di licenze o sospendere la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="d71c9-138">**Per le sottoscrizioni Isv SaaS (basate su licenza e a consumo):**</span><span class="sxs-lookup"><span data-stu-id="d71c9-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="d71c9-139">Si riceverà un collegamento al sito dell'editore ISV.</span><span class="sxs-lookup"><span data-stu-id="d71c9-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="d71c9-140">Questo collegamento consente di completare la distribuzione o la configurazione dell'account della sottoscrizione del cliente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="d71c9-141">Né l'utente né il cliente riceveranno un messaggio di posta elettronica con le istruzioni per completare la configurazione/provisioning dell'account per questo tipo di sottoscrizione ISV.</span><span class="sxs-lookup"><span data-stu-id="d71c9-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="d71c9-142">Se la sottoscrizione include una versione di valutazione gratuita di 30 giorni, il periodo di valutazione gratuita verrà applicato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="d71c9-143">I partner del programma CSP non possono rinunciare al periodo di valutazione gratuito per le offerte acquistate per i clienti.</span><span class="sxs-lookup"><span data-stu-id="d71c9-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="d71c9-144">Al termine del periodo di valutazione gratuita, inizierà il periodo di validità della sottoscrizione e la sottoscrizione verrà convertita in stato a pagamento.</span><span class="sxs-lookup"><span data-stu-id="d71c9-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="d71c9-145">La sottoscrizione verrà quindi rinnovata automaticamente in base alla stessa pianificazione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="d71c9-146">Aggiornare le sottoscrizioni con i componenti aggiuntivi</span><span class="sxs-lookup"><span data-stu-id="d71c9-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="d71c9-147">Per acquistare un componente aggiuntivo, il cliente deve prima avere una sottoscrizione di base attiva.</span><span class="sxs-lookup"><span data-stu-id="d71c9-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="d71c9-148">Non è possibile acquistare i componenti aggiuntivi tramite il catalogo.</span><span class="sxs-lookup"><span data-stu-id="d71c9-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="d71c9-149">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d71c9-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d71c9-150">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d71c9-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d71c9-151">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="d71c9-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d71c9-152">Sotto la **sezione** Stato è riportato un elenco di componenti aggiuntivi disponibili per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="d71c9-153">Aggiornare la quantità di licenze per ogni componente aggiuntivo necessario.</span><span class="sxs-lookup"><span data-stu-id="d71c9-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="d71c9-154">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="d71c9-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="d71c9-155">La possibilità di acquistare componenti aggiuntivi tramite Partner Center è disponibile solo per i provider di fatturazione diretta e indiretti.</span><span class="sxs-lookup"><span data-stu-id="d71c9-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="d71c9-156">Vengono visualizzati solo i componenti aggiuntivi idonei in base ai requisiti di base e alla disponibilità a livello di regione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="d71c9-157">Per altre informazioni sui prezzi e sulle offerte, vedere la matrice di offerte cloud reseller.</span><span class="sxs-lookup"><span data-stu-id="d71c9-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="d71c9-158">La sospensione della sottoscrizione di base comporta anche la sospensione di tutti i componenti aggiuntivi associati.</span><span class="sxs-lookup"><span data-stu-id="d71c9-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="d71c9-159">Le date di inizio per i componenti aggiuntivi sono allineate alla sottoscrizione di base e gli addebiti vengono calcolati dalla data di inizio e dalla data di fine dell'addebito con addebiti proporzionali nella prima fattura.</span><span class="sxs-lookup"><span data-stu-id="d71c9-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="d71c9-160">Per altre informazioni, vedere [Fatturazione basata su licenza](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="d71c9-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="d71c9-161">Sospendere o annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="d71c9-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="d71c9-162">I partner possono sospendere o annullare una sottoscrizione se richiesto dal cliente o in caso di insolvenza o frode.</span><span class="sxs-lookup"><span data-stu-id="d71c9-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="d71c9-163">Sospendere una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="d71c9-163">Suspend a subscription</span></span>

<span data-ttu-id="d71c9-164">Quando cambi lo stato di una sottoscrizione in **Sospesa**, gli utenti non possono accedere alla sottoscrizione o ai servizi.</span><span class="sxs-lookup"><span data-stu-id="d71c9-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="d71c9-165">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d71c9-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d71c9-166">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d71c9-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d71c9-167">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="d71c9-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d71c9-168">Nella sezione **Stato**, scegliere **Sospesa**.</span><span class="sxs-lookup"><span data-stu-id="d71c9-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="d71c9-169">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="d71c9-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d71c9-170">Verranno eliminati tutti i dati, tranne nel caso in cui la sottoscrizione venga riattivata entro 90 giorni o 90 giorni più il numero di giorni tra il momento in cui l'account è stato aperto e il primo periodo di fatturazione (massimo 120 giorni).</span><span class="sxs-lookup"><span data-stu-id="d71c9-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="d71c9-171">Quando sospendi una sottoscrizione, la data visualizzata sotto il pulsante **Sospesa** indica quando la sottoscrizione scadrà automaticamente se non la riattivi.</span><span class="sxs-lookup"><span data-stu-id="d71c9-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="d71c9-172">Le sottoscrizioni CSP non hanno un periodo scaduto (come le sottoscrizioni dirette Web) durante il quale i servizi continuano a funzionare, ma la sottoscrizione non genera alcun addebito per la fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="d71c9-173">Le sottoscrizioni CSP sono attive o sospese (o completamente eliminate).</span><span class="sxs-lookup"><span data-stu-id="d71c9-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="d71c9-174">Annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="d71c9-174">Cancel a subscription</span></span>

<span data-ttu-id="d71c9-175">È possibile annullare sottoscrizioni SaaS basate su licenza da editori ISV di terze parti all'interno Partner Center [marketplace commerciale.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="d71c9-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="d71c9-176">Se si annulla entro il periodo di annullamento, si riceverà un rimborso completo.</span><span class="sxs-lookup"><span data-stu-id="d71c9-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="d71c9-177">Per le offerte ISV fatturate mensilmente:</span><span class="sxs-lookup"><span data-stu-id="d71c9-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="d71c9-178">Se si annulla meno di 24 ore dopo l'ordine, si riceverà un credito completo nella fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="d71c9-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d71c9-179">Se si annulla più di 24 ore dopo l'ordine, l'annullamento verrà pianificato al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="d71c9-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d71c9-180">Per le offerte fatturate annualmente:</span><span class="sxs-lookup"><span data-stu-id="d71c9-180">For offers billed annually:</span></span>

- <span data-ttu-id="d71c9-181">Se si annulla meno di 14 giorni dopo l'ordine, si riceverà un credito completo nella fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="d71c9-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d71c9-182">Se si annulla più di 14 giorni dopo l'esecuzione dell'ordine, l'annullamento verrà pianificato al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="d71c9-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d71c9-183">Al termine di questi periodi, non verrà più visualizzata l'opzione per annullare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="d71c9-184">I servizi ISV di terze parti basati sull'utilizzo e a consumo ,ad esempio che usano macchine virtuali o contenitori, non sono idonei per la restituzione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="d71c9-185">È possibile effettuare il de-provisioning dei servizi basati sull'utilizzo come metodo di annullamento.</span><span class="sxs-lookup"><span data-stu-id="d71c9-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="d71c9-186">Poiché gli addebiti vengono fatturati dopo l'uso, questi servizi non sono idonei per un rimborso.</span><span class="sxs-lookup"><span data-stu-id="d71c9-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="d71c9-187">Per annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="d71c9-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="d71c9-188">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d71c9-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d71c9-189">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d71c9-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d71c9-190">Individuare la sottoscrizione da annullare.</span><span class="sxs-lookup"><span data-stu-id="d71c9-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="d71c9-191">Nella colonna **Stato** selezionare **Annulla.**</span><span class="sxs-lookup"><span data-stu-id="d71c9-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="d71c9-192">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="d71c9-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d71c9-193">Se viene visualizzata una finestra di dialogo, compilare i dettagli pertinenti e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="d71c9-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="d71c9-194">Per confermare l'annullamento, **selezionare Sì, annulla**.</span><span class="sxs-lookup"><span data-stu-id="d71c9-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="d71c9-195">È anche possibile scegliere di annullare una sottoscrizione Azure Marketplace usando le API.</span><span class="sxs-lookup"><span data-stu-id="d71c9-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="d71c9-196">A tale scopo, vedere [Annullare una sottoscrizione Azure Marketplace sottoscrizione.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="d71c9-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="d71c9-197">Scegliere se rinnovare automaticamente una sottoscrizione del Marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="d71c9-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="d71c9-198">Per impostazione predefinita, le sottoscrizioni attive sono impostate in modo da essere rinnovate automaticamente al termine del periodo di sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="d71c9-199">Per [le sottoscrizioni ai prodotti del marketplace commerciale,](csp-commercial-marketplace-overview.md)è possibile scegliere di non rinnovare automaticamente la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d71c9-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="d71c9-200">Per impedire il rinnovo automatico di una sottoscrizione attiva del marketplace commerciale:</span><span class="sxs-lookup"><span data-stu-id="d71c9-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="d71c9-201">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d71c9-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d71c9-202">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d71c9-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d71c9-203">Selezionare **Sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="d71c9-203">Select **Subscriptions**.</span></span> <span data-ttu-id="d71c9-204">Vengono elencate tutte le sottoscrizioni basate su licenza acquistate per il cliente.</span><span class="sxs-lookup"><span data-stu-id="d71c9-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="d71c9-205">Nella **colonna Sottoscrizione** selezionare la sottoscrizione che si vuole modificare.</span><span class="sxs-lookup"><span data-stu-id="d71c9-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="d71c9-206">Nella pagina dei dettagli della sottoscrizione individuare la **sezione Stato** e deselezionare la **casella Rinnovo** automatico.</span><span class="sxs-lookup"><span data-stu-id="d71c9-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="d71c9-207">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="d71c9-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d71c9-208">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d71c9-208">Next steps</span></span>

- [<span data-ttu-id="d71c9-209">Acquistare prodotti del Marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="d71c9-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="d71c9-210">Gestire i prodotti del marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="d71c9-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="d71c9-211">Panoramica del marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="d71c9-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)