---
title: Creare sottoscrizioni dei clienti in Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come vendere sottoscrizioni ai clienti per prodotti pubblicati da Microsoft e prodotti SaaS pubblicati da ISV di terze parti.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201409"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="c84ac-103">Creare, sospendere o annullare le sottoscrizioni dei clienti</span><span class="sxs-lookup"><span data-stu-id="c84ac-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="c84ac-104">**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c84ac-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c84ac-105">**Ruoli appropriati:** Agente di amministrazione | Amministratore della fatturazione | Amministratore globale | Supporto per l'agente | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c84ac-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="c84ac-106">Dopo aver creato un record del cliente nel Centro per i partner, puoi vendere loro sottoscrizioni per i prodotti nel catalogo.</span><span class="sxs-lookup"><span data-stu-id="c84ac-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="c84ac-107">Sono inclusi i prodotti pubblicati da Microsoft e prodotti SaaS (Software as a Service) pubblicati da fornitori di software indipendenti (ISV) di terze parti nel [marketplace commerciale.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="c84ac-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="c84ac-108">Alcune offerte sono limitate a una sottoscrizione per cliente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="c84ac-109">Per vedere l'elenco delle offerte limitate, visita la pagina Prezzi e offerte del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c84ac-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="c84ac-110">I partner del programma CSP possono  acquistare sottoscrizioni **SaaS** basate su licenza o a consumo da editori ISV all'interno Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c84ac-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="c84ac-111">Ciò significa che  è possibile acquistare qualsiasi offerta **SaaS** basata su licenza o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a consumo resa disponibile dall'editore ISV, incluse le offerte esclusive a cui si ha accesso.</span><span class="sxs-lookup"><span data-stu-id="c84ac-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="c84ac-112">Per acquistare o gestire altre offerte del marketplace commerciale dagli ISV (ad esempio offerte basate sull'utilizzo che coinvolgono applicazioni di Azure, contenitori o macchine virtuali), è necessario passare al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c84ac-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="c84ac-113">Tutte le date e le ore Partner Center sono specificate nello standard dell'ora UTC (Universal Time Coordinated).</span><span class="sxs-lookup"><span data-stu-id="c84ac-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="c84ac-114">Può variare fino a 24 ore rispetto all'ora locale.</span><span class="sxs-lookup"><span data-stu-id="c84ac-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="c84ac-115">Creare una nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c84ac-115">Create a new subscription</span></span>

1. <span data-ttu-id="c84ac-116">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c84ac-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c84ac-117">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c84ac-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c84ac-118">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="c84ac-118">Select **Add subscription**.</span></span> <span data-ttu-id="c84ac-119">Nella **scheda Servizi online** verranno mostrate tutte le offerte SaaS del Marketplace disponibili.</span><span class="sxs-lookup"><span data-stu-id="c84ac-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="c84ac-120">Per visualizzare solo determinati tipi di sottoscrizioni, effettua le selezioni nei filtri disponibili:</span><span class="sxs-lookup"><span data-stu-id="c84ac-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="c84ac-121">**Editore:** scegliere **Microsoft** per visualizzare solo le offerte di Microsoft o **partner** per visualizzare i prodotti del marketplace commerciale pubblicati dagli ISV.</span><span class="sxs-lookup"><span data-stu-id="c84ac-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="c84ac-122">**Tipo di fatturazione:** selezionare il tipo di fatturazione della sottoscrizione da usare: **Licenza** o **Utilizzo.**</span><span class="sxs-lookup"><span data-stu-id="c84ac-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="c84ac-123">Vedere [Fatturazione basata su licenza](license-based-billing.md) per informazioni che consentono di decidere tra la frequenza di fatturazione mensile e annuale.</span><span class="sxs-lookup"><span data-stu-id="c84ac-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="c84ac-124">**Categoria:** scegliere **Enterprise,** **Small Business** o **Trial.**</span><span class="sxs-lookup"><span data-stu-id="c84ac-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="c84ac-125">Per informazioni sulle sottoscrizioni di versioni di valutazione, vedi [Offrire ai clienti le versioni di valutazione dei prodotti Microsoft](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="c84ac-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="c84ac-126">Selezionare le sottoscrizioni al prodotto da acquistare per il cliente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="c84ac-127">I prodotti visualizzati dipendono dal tipo di segmento di cliente (istruzione, enti pubblici e così via) e dai filtri applicati.</span><span class="sxs-lookup"><span data-stu-id="c84ac-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="c84ac-128">Alcune offerte visualizzate nel Marketplace potrebbero non essere sempre disponibili per un cliente specifico o per un partner CSP specifico.</span><span class="sxs-lookup"><span data-stu-id="c84ac-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="c84ac-129">Ciò può essere dovuto al seguente:</span><span class="sxs-lookup"><span data-stu-id="c84ac-129">This can be because:</span></span>

   - <span data-ttu-id="c84ac-130">Il cliente ha già una sottoscrizione a tale prodotto e ne è consentita solo una</span><span class="sxs-lookup"><span data-stu-id="c84ac-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="c84ac-131">La sottoscrizione del cliente potrebbe essere stata sospesa. In questo caso, è possibile riattivare la sottoscrizione anziché acquistarne una nuova.</span><span class="sxs-lookup"><span data-stu-id="c84ac-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="c84ac-132">Per le offerte SaaS ISV, possono esserci alcuni motivi per cui l'offerta non è disponibile per l'acquisto: l'ISV potrebbe non supportare il paese o l'area di fatturazione del cliente; l'ISV potrebbe aver scelto di non rendere disponibile l'offerta tramite il programma CSP; oppure l'ISV potrebbe aver reso l'offerta [esclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo a determinati partner CSP.</span><span class="sxs-lookup"><span data-stu-id="c84ac-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="c84ac-133">L'offerta ISV potrebbe anche non essere transazionabile tramite il Partner Center (ad esempio, contenitori o alcune offerte basate sull'utilizzo).</span><span class="sxs-lookup"><span data-stu-id="c84ac-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="c84ac-134">Per ogni sottoscrizione da aggiungere, immettere il numero di licenze (se necessario) e selezionare **Aggiungi al carrello.**</span><span class="sxs-lookup"><span data-stu-id="c84ac-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="c84ac-135">Al termine dell'aggiunta delle sottoscrizioni, selezionare **Rivedi** ed esamina l'ordine.</span><span class="sxs-lookup"><span data-stu-id="c84ac-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="c84ac-136">Dopo aver esaminato gli ordini e aver pronti per l'acquisto di queste sottoscrizioni, selezionare **Acquista**.</span><span class="sxs-lookup"><span data-stu-id="c84ac-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="c84ac-137">Dopo aver acquistato una sottoscrizione per un cliente, si verificheranno le condizioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c84ac-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="c84ac-138">È possibile esaminare o modificare la sottoscrizione selezionando il nome della sottoscrizione dalla pagina **Sottoscrizioni del** cliente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="c84ac-139">In tale pagina puoi selezionare licenze per componenti aggiuntivi (se disponibili), modificare la quantità di licenze o sospendere la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="c84ac-140">**Per le sottoscrizioni Isv SaaS (basate su licenza e a consumo):**</span><span class="sxs-lookup"><span data-stu-id="c84ac-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="c84ac-141">Si riceverà un collegamento al sito dell'editore ISV.</span><span class="sxs-lookup"><span data-stu-id="c84ac-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="c84ac-142">Questo collegamento consente di completare la distribuzione o la configurazione dell'account della sottoscrizione del cliente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="c84ac-143">Né l'utente né il cliente riceveranno un messaggio di posta elettronica con le istruzioni per completare la configurazione/provisioning dell'account per questo tipo di sottoscrizione ISV.</span><span class="sxs-lookup"><span data-stu-id="c84ac-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="c84ac-144">Se la sottoscrizione include una versione di valutazione gratuita di 30 giorni, il periodo di valutazione gratuita verrà applicato automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="c84ac-145">I partner del programma CSP non possono rinunciare al periodo di valutazione gratuito per le offerte acquistate per i clienti.</span><span class="sxs-lookup"><span data-stu-id="c84ac-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="c84ac-146">Al termine del periodo di valutazione gratuita, il periodo di sottoscrizione inizierà e la sottoscrizione verrà convertita in stato a pagamento.</span><span class="sxs-lookup"><span data-stu-id="c84ac-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="c84ac-147">La sottoscrizione verrà quindi rinnovata automaticamente in base alla stessa pianificazione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="c84ac-148">Aggiornare le sottoscrizioni con i componenti aggiuntivi</span><span class="sxs-lookup"><span data-stu-id="c84ac-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="c84ac-149">Per acquistare un componente aggiuntivo, il cliente deve prima avere una sottoscrizione di base attiva.</span><span class="sxs-lookup"><span data-stu-id="c84ac-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="c84ac-150">Non è possibile acquistare i componenti aggiuntivi tramite il catalogo.</span><span class="sxs-lookup"><span data-stu-id="c84ac-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="c84ac-151">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c84ac-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c84ac-152">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c84ac-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c84ac-153">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="c84ac-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c84ac-154">Sotto la **sezione** Stato è riportato un elenco di componenti aggiuntivi disponibili per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="c84ac-155">Aggiornare la quantità di licenze per ogni componente aggiuntivo necessario.</span><span class="sxs-lookup"><span data-stu-id="c84ac-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="c84ac-156">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="c84ac-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="c84ac-157">La possibilità di acquistare componenti aggiuntivi tramite Partner Center è disponibile solo per i provider di fatturazione diretta e indiretti.</span><span class="sxs-lookup"><span data-stu-id="c84ac-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="c84ac-158">Vengono visualizzati solo i componenti aggiuntivi idonei in base ai requisiti di base e alla disponibilità a livello di regione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="c84ac-159">Per altre informazioni sui prezzi e sulle offerte, vedere la matrice di offerte cloud reseller.</span><span class="sxs-lookup"><span data-stu-id="c84ac-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="c84ac-160">La sospensione della sottoscrizione di base comporta anche la sospensione di tutti i componenti aggiuntivi associati.</span><span class="sxs-lookup"><span data-stu-id="c84ac-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="c84ac-161">Le date di inizio per i componenti aggiuntivi sono allineate alla sottoscrizione di base e gli addebiti vengono calcolati dalla data di inizio e dalla data di fine dell'addebito con addebiti proporzionali nella prima fattura.</span><span class="sxs-lookup"><span data-stu-id="c84ac-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="c84ac-162">Per altre informazioni, vedere [Fatturazione basata su licenza.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="c84ac-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="c84ac-163">Sospendere o annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c84ac-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="c84ac-164">I partner possono sospendere o annullare una sottoscrizione se richiesto dal cliente o in caso di insolvenza o frode.</span><span class="sxs-lookup"><span data-stu-id="c84ac-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="c84ac-165">Sospendere una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c84ac-165">Suspend a subscription</span></span>

<span data-ttu-id="c84ac-166">Quando cambi lo stato di una sottoscrizione in **Sospesa**, gli utenti non possono accedere alla sottoscrizione o ai servizi.</span><span class="sxs-lookup"><span data-stu-id="c84ac-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="c84ac-167">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c84ac-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c84ac-168">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c84ac-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c84ac-169">Scegli la sottoscrizione che vuoi gestire.</span><span class="sxs-lookup"><span data-stu-id="c84ac-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="c84ac-170">Nella sezione **Stato**, scegliere **Sospesa**.</span><span class="sxs-lookup"><span data-stu-id="c84ac-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="c84ac-171">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="c84ac-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c84ac-172">Verranno eliminati tutti i dati, tranne nel caso in cui la sottoscrizione venga riattivata entro 90 giorni o 90 giorni più il numero di giorni tra il momento in cui l'account è stato aperto e il primo periodo di fatturazione (massimo 120 giorni).</span><span class="sxs-lookup"><span data-stu-id="c84ac-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="c84ac-173">Quando sospendi una sottoscrizione, la data visualizzata sotto il pulsante **Sospesa** indica quando la sottoscrizione scadrà automaticamente se non la riattivi.</span><span class="sxs-lookup"><span data-stu-id="c84ac-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="c84ac-174">Le sottoscrizioni CSP non hanno un periodo scaduto (come le sottoscrizioni dirette Web) durante il quale i servizi continuano a funzionare, ma la sottoscrizione non genera alcun addebito per la fatturazione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="c84ac-175">Le sottoscrizioni CSP sono attive o sospese (o completamente eliminate).</span><span class="sxs-lookup"><span data-stu-id="c84ac-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="c84ac-176">Annullare una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="c84ac-176">Cancel a subscription</span></span>

<span data-ttu-id="c84ac-177">È possibile annullare sottoscrizioni SaaS basate su licenza da editori ISV di terze parti all'interno Partner Center [marketplace commerciale.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="c84ac-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="c84ac-178">Se si annulla entro il periodo di annullamento, si riceverà un rimborso completo.</span><span class="sxs-lookup"><span data-stu-id="c84ac-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="c84ac-179">Per le offerte ISV fatturate mensilmente:</span><span class="sxs-lookup"><span data-stu-id="c84ac-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="c84ac-180">Se si annulla meno di 24 ore dopo l'ordine, si riceverà un credito completo nella fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="c84ac-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c84ac-181">Se si annulla più di 24 ore dopo l'ordine, l'annullamento verrà pianificato al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="c84ac-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c84ac-182">Per le offerte fatturate annualmente:</span><span class="sxs-lookup"><span data-stu-id="c84ac-182">For offers billed annually:</span></span>

- <span data-ttu-id="c84ac-183">Se si annulla meno di 14 giorni dopo l'ordine, si riceverà un credito completo nella fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="c84ac-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="c84ac-184">Se si annulla più di 14 giorni dopo l'esecuzione dell'ordine, l'annullamento verrà pianificato al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="c84ac-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="c84ac-185">Al termine di questi periodi, non verrà più visualizzata l'opzione per annullare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="c84ac-186">I servizi ISV di terze parti basati sull'utilizzo e a consumo (ad esempio, che usano macchine virtuali o contenitori) non sono idonei per la restituzione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="c84ac-187">È possibile effettuare il de-provisioning dei servizi basati sull'utilizzo come metodo di annullamento.</span><span class="sxs-lookup"><span data-stu-id="c84ac-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="c84ac-188">Poiché gli addebiti vengono fatturati dopo l'uso, questi servizi non sono idonei per un rimborso.</span><span class="sxs-lookup"><span data-stu-id="c84ac-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="c84ac-189">Per annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="c84ac-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="c84ac-190">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c84ac-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c84ac-191">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c84ac-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c84ac-192">Individuare la sottoscrizione da annullare.</span><span class="sxs-lookup"><span data-stu-id="c84ac-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="c84ac-193">Nella colonna **Stato** selezionare **Annulla.**</span><span class="sxs-lookup"><span data-stu-id="c84ac-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="c84ac-194">**Inviare** quindi le modifiche.</span><span class="sxs-lookup"><span data-stu-id="c84ac-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="c84ac-195">Se viene visualizzata una finestra di dialogo, immettere i dettagli pertinenti e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="c84ac-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="c84ac-196">Per confermare l'annullamento, **selezionare Sì, annulla**.</span><span class="sxs-lookup"><span data-stu-id="c84ac-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="c84ac-197">È anche possibile scegliere di annullare una sottoscrizione Azure Marketplace usando le API.</span><span class="sxs-lookup"><span data-stu-id="c84ac-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="c84ac-198">A tale scopo, vedere [Annullare una sottoscrizione Azure Marketplace sottoscrizione.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="c84ac-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="c84ac-199">Scegliere se rinnovare automaticamente una sottoscrizione del Marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="c84ac-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="c84ac-200">Per impostazione predefinita, le sottoscrizioni attive sono impostate in modo da essere rinnovate automaticamente al termine del periodo di sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="c84ac-201">Per [le sottoscrizioni ai prodotti del marketplace commerciale,](csp-commercial-marketplace-overview.md)è possibile scegliere di non rinnovare automaticamente la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c84ac-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="c84ac-202">Per impedire il rinnovo automatico di una sottoscrizione attiva del marketplace commerciale:</span><span class="sxs-lookup"><span data-stu-id="c84ac-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="c84ac-203">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c84ac-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="c84ac-204">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c84ac-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="c84ac-205">Selezionare **Sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="c84ac-205">Select **Subscriptions**.</span></span> <span data-ttu-id="c84ac-206">Vengono elencate tutte le sottoscrizioni basate su licenza acquistate per il cliente.</span><span class="sxs-lookup"><span data-stu-id="c84ac-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="c84ac-207">Nella **colonna Sottoscrizione** selezionare la sottoscrizione che si vuole modificare.</span><span class="sxs-lookup"><span data-stu-id="c84ac-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="c84ac-208">Nella pagina dei dettagli della sottoscrizione individuare la **sezione Stato** e deselezionare la **casella Rinnovo** automatico.</span><span class="sxs-lookup"><span data-stu-id="c84ac-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="c84ac-209">Selezionare **Submit** (Invia).</span><span class="sxs-lookup"><span data-stu-id="c84ac-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c84ac-210">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c84ac-210">Next steps</span></span>

- [<span data-ttu-id="c84ac-211">Acquistare prodotti del Marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="c84ac-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="c84ac-212">Gestire i prodotti del marketplace commerciale per i clienti</span><span class="sxs-lookup"><span data-stu-id="c84ac-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="c84ac-213">Panoramica del marketplace commerciale</span><span class="sxs-lookup"><span data-stu-id="c84ac-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)