---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Per una visualizzazione di voci di ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122278"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="19519-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="19519-103">Use the reconciliation files</span></span>

**<span data-ttu-id="19519-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="19519-104">Applies to</span></span>**

-  <span data-ttu-id="19519-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="19519-105">Partner Center</span></span>
-  <span data-ttu-id="19519-106">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="19519-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="19519-107">Per una visualizzazione di voci di ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="19519-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="19519-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="19519-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="19519-109">Eseguire la scomposizione dei dati in base al partner</span><span class="sxs-lookup"><span data-stu-id="19519-109">Itemize by partner</span></span>


<span data-ttu-id="19519-110">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="19519-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="19519-111">ID MPN</span><span class="sxs-lookup"><span data-stu-id="19519-111">MPN ID</span></span></th>
<th><span data-ttu-id="19519-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="19519-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="19519-113">ID MPN</span><span class="sxs-lookup"><span data-stu-id="19519-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="19519-114">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="19519-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-115">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="19519-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="19519-116">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="19519-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="19519-117">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="19519-118">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="19519-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="19519-119">Per visualizzare o aggiornare il rivenditore, il menu del centro per i Partner seleziona <strong>i clienti</strong>, quindi scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="19519-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="19519-120">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="19519-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="19519-121">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="19519-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="19519-122">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="19519-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="19519-123">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="19519-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="19519-124">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="19519-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="19519-125">Campi dei file in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="19519-125">License-based file fields</span></span>


<span data-ttu-id="19519-126">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="19519-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="19519-127">Colonna</span><span class="sxs-lookup"><span data-stu-id="19519-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="19519-128">Descrizione</span><span class="sxs-lookup"><span data-stu-id="19519-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="19519-129">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="19519-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="19519-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="19519-131">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="19519-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="19519-132">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="19519-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="19519-133">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="19519-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="19519-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="19519-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="19519-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="19519-136">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="19519-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="19519-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="19519-138">OrderID</span></span></td>
<td><p><span data-ttu-id="19519-139">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="19519-140">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="19519-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="19519-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="19519-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="19519-143">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="19519-144">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="19519-145">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="19519-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="19519-146">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="19519-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="19519-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="19519-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="19519-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="19519-149">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="19519-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="19519-150">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="19519-151">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="19519-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="19519-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="19519-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="19519-153">OfferID</span></span></td>
<td><p><span data-ttu-id="19519-154">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="19519-154">Unique offer ID.</span></span> <span data-ttu-id="19519-155">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="19519-156"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="19519-157">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="19519-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="19519-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="19519-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="19519-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="19519-160">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="19519-161"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="19519-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="19519-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="19519-163">OfferName</span></span></td>
<td><p><span data-ttu-id="19519-164">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="19519-165">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="19519-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="19519-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="19519-167">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="19519-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="19519-168">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="19519-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="19519-169">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="19519-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="19519-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="19519-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="19519-172">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="19519-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="19519-173">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="19519-174">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="19519-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="19519-175">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="19519-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="19519-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="19519-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="19519-178">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="19519-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="19519-179">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="19519-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="19519-180">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="19519-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="19519-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="19519-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="19519-183">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="19519-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="19519-184">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="19519-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="19519-185">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="19519-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="19519-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="19519-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="19519-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="19519-188">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="19519-188">The type of charge or adjustment.</span></span> <span data-ttu-id="19519-189">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="19519-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="19519-190">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="19519-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="19519-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="19519-192">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="19519-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="19519-193">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="19519-194">6.82</span><span class="sxs-lookup"><span data-stu-id="19519-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="19519-195">Quantity</span></span></td>
<td><p><span data-ttu-id="19519-196">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="19519-196">Number of seats.</span></span> <span data-ttu-id="19519-197">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="19519-198">2</span><span class="sxs-lookup"><span data-stu-id="19519-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-199">Amount</span><span class="sxs-lookup"><span data-stu-id="19519-199">Amount</span></span></td>
<td><p><span data-ttu-id="19519-200">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="19519-200">Total of price for quantity.</span></span> <span data-ttu-id="19519-201">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="19519-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="19519-202">13.32</span><span class="sxs-lookup"><span data-stu-id="19519-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="19519-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="19519-204">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="19519-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="19519-205">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="19519-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="19519-206">2.32</span><span class="sxs-lookup"><span data-stu-id="19519-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="19519-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="19519-208">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-208">Total before tax.</span></span> <span data-ttu-id="19519-209">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="19519-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="19519-210">11</span><span class="sxs-lookup"><span data-stu-id="19519-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-211">Tax</span><span class="sxs-lookup"><span data-stu-id="19519-211">Tax</span></span></td>
<td><p><span data-ttu-id="19519-212">Importo totale delle imposte, in base alla tua market& #39; regole imposte s e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="19519-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="19519-213">0</span><span class="sxs-lookup"><span data-stu-id="19519-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="19519-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="19519-215">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-215">Total after tax.</span></span> <span data-ttu-id="19519-216">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="19519-217">11</span><span class="sxs-lookup"><span data-stu-id="19519-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-218">Currency</span><span class="sxs-lookup"><span data-stu-id="19519-218">Currency</span></span></td>
<td><p><span data-ttu-id="19519-219">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-219">Currency type.</span></span> <span data-ttu-id="19519-220">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="19519-221">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="19519-222">EUR</span><span class="sxs-lookup"><span data-stu-id="19519-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="19519-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="19519-224">Customer& #39; nome dell'organizzazione s registrato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="19519-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="19519-225">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="19519-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="19519-226">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="19519-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="19519-227">MPNID</span></span></td>
<td><p><span data-ttu-id="19519-228">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="19519-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="19519-229">4390934</span><span class="sxs-lookup"><span data-stu-id="19519-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="19519-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="19519-231">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="19519-232">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="19519-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="19519-233">4390934</span><span class="sxs-lookup"><span data-stu-id="19519-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="19519-234">DomainName</span></span></td>
<td><p><span data-ttu-id="19519-235">Customer& #39; nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="19519-236">Questo non deve essere usato per identificare in modo univoco il cliente, il cliente/partner può aggiornare il dominio di reindirizzamento a microsito/predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="19519-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="19519-237">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="19519-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="19519-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="19519-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="19519-240">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-240">Subscription nickname.</span></span> <span data-ttu-id="19519-241">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="19519-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="19519-242">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="19519-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="19519-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="19519-244">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="19519-245">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="19519-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="19519-246">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="19519-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="19519-247">Campi dei file in base all'uso</span><span class="sxs-lookup"><span data-stu-id="19519-247">Usage-based file fields</span></span>


<span data-ttu-id="19519-248">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="19519-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="19519-249">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="19519-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="19519-250">Colonna</span><span class="sxs-lookup"><span data-stu-id="19519-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="19519-251">Descrizione</span><span class="sxs-lookup"><span data-stu-id="19519-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="19519-252">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="19519-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="19519-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="19519-254">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="19519-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="19519-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="19519-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="19519-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="19519-257">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="19519-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="19519-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="19519-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="19519-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="19519-260">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="19519-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="19519-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="19519-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="19519-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="19519-263">Customer& #39; nome dell'organizzazione s registrato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="19519-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="19519-264">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="19519-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="19519-265">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="19519-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="19519-266">MPNID</span></span></td>
<td><p><span data-ttu-id="19519-267">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="19519-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="19519-268">4390934</span><span class="sxs-lookup"><span data-stu-id="19519-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="19519-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="19519-270">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="19519-271">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="19519-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="19519-272">4390934</span><span class="sxs-lookup"><span data-stu-id="19519-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="19519-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="19519-274">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="19519-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="19519-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="19519-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="19519-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="19519-277">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="19519-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="19519-278">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="19519-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="19519-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="19519-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="19519-281">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="19519-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="19519-282">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="19519-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="19519-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="19519-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="19519-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="19519-285">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="19519-286">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="19519-287">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="19519-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="19519-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="19519-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="19519-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="19519-290">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="19519-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="19519-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="19519-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="19519-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="19519-293">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="19519-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="19519-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="19519-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="19519-295">OrderID</span></span></td>
<td><p><span data-ttu-id="19519-296">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="19519-297">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="19519-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="19519-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="19519-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="19519-300">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="19519-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="19519-301">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="19519-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="19519-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="19519-303">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="19519-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="19519-304">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="19519-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="19519-305">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="19519-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="19519-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="19519-307">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="19519-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="19519-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="19519-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="19519-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="19519-310">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="19519-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="19519-311">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="19519-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="19519-312">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="19519-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-313">Region</span><span class="sxs-lookup"><span data-stu-id="19519-313">Region</span></span></td>
<td><p><span data-ttu-id="19519-314">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="19519-314">The region the usage applies to.</span></span> <span data-ttu-id="19519-315">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="19519-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="19519-316">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="19519-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-317">SKU</span><span class="sxs-lookup"><span data-stu-id="19519-317">SKU</span></span></td>
<td><p><span data-ttu-id="19519-318">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="19519-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="19519-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="19519-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="19519-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="19519-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="19519-321">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="19519-322">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="19519-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="19519-323">1</span><span class="sxs-lookup"><span data-stu-id="19519-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="19519-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="19519-325">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="19519-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="19519-326">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="19519-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="19519-327">11</span><span class="sxs-lookup"><span data-stu-id="19519-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="19519-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="19519-329">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="19519-329">Units included as part of the offer.</span></span> <span data-ttu-id="19519-330">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="19519-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="19519-331">0</span><span class="sxs-lookup"><span data-stu-id="19519-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="19519-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="19519-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="19519-333">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="19519-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="19519-334">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="19519-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="19519-335">11</span><span class="sxs-lookup"><span data-stu-id="19519-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="19519-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="19519-337">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="19519-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="19519-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="19519-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="19519-340">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="19519-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="19519-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="19519-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="19519-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="19519-343">Importo totale delle imposte, in base alla tua market& #39; regole imposte s e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="19519-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="19519-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="19519-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="19519-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="19519-346">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="19519-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="19519-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="19519-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-348">Currency</span><span class="sxs-lookup"><span data-stu-id="19519-348">Currency</span></span></td>
<td><p><span data-ttu-id="19519-349">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-349">Currency type.</span></span> <span data-ttu-id="19519-350">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="19519-351">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="19519-352">EUR</span><span class="sxs-lookup"><span data-stu-id="19519-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="19519-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="19519-354">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-354">Pretax price per unit.</span></span> <span data-ttu-id="19519-355">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="19519-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="19519-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="19519-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="19519-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="19519-358">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-358">Post tax price per unit.</span></span> <span data-ttu-id="19519-359">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="19519-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="19519-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="19519-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="19519-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="19519-362">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="19519-362">The type of charge or adjustment.</span></span> <span data-ttu-id="19519-363">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="19519-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="19519-364">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="19519-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="19519-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="19519-366">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="19519-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="19519-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="19519-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="19519-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="19519-369">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="19519-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="19519-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="19519-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="19519-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="19519-372">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="19519-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="19519-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="19519-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="19519-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="19519-375">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="19519-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="19519-376">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="19519-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="19519-377">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="19519-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="19519-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="19519-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="19519-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="19519-380">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="19519-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="19519-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="19519-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-382">Project</span><span class="sxs-lookup"><span data-stu-id="19519-382">Project</span></span></td>
<td><p><span data-ttu-id="19519-383">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="19519-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="19519-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="19519-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="19519-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="19519-386">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="19519-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="19519-387">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="19519-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="19519-388">Se hai un pacchetto da 25 connessioni ServiceBus e ne hai utilizzata 1 per quel giorno, l'uso giornaliero registrato sarà "25 Connections / 30 Days – Used: 1.000000".</span><span class="sxs-lookup"><span data-stu-id="19519-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="19519-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="19519-390">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="19519-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="19519-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="19519-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="19519-392">DomainName</span></span></td>
<td><p><span data-ttu-id="19519-393">Customer& #39; nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="19519-394">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="19519-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="19519-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="19519-396">Unità</span><span class="sxs-lookup"><span data-stu-id="19519-396">Unit</span></span></td>
<td><p><span data-ttu-id="19519-397">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="19519-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="19519-398">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="19519-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="19519-399">Campi dei file temporanei e ricorrenti</span><span class="sxs-lookup"><span data-stu-id="19519-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="19519-400">Colonna</span><span class="sxs-lookup"><span data-stu-id="19519-400">Column</span></span></th>
<th><span data-ttu-id="19519-401">Descrizione</span><span class="sxs-lookup"><span data-stu-id="19519-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="19519-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="19519-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="19519-403">Identificatore univoco tenant di Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="19519-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="19519-404">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="19519-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="19519-405">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="19519-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-406">Id del cliente</span><span class="sxs-lookup"><span data-stu-id="19519-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="19519-407">Microsoft Azure Active Directory tenant ID univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-408">Nome cliente</span><span class="sxs-lookup"><span data-stu-id="19519-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="19519-409">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="19519-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="19519-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="19519-411">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="19519-412">Questo non deve essere usato per identificare in modo univoco il cliente, il cliente/partner può aggiornare il dominio di reindirizzamento a microsito/predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="19519-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="19519-413">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-414">Paese cliente</span><span class="sxs-lookup"><span data-stu-id="19519-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="19519-415">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-416">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="19519-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="19519-417">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="19519-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="19519-418">MpnId</span></span></td>
<td><p><span data-ttu-id="19519-419">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="19519-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-420">MpnId rivenditore</span><span class="sxs-lookup"><span data-stu-id="19519-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="19519-421">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-422">ID ordine</span><span class="sxs-lookup"><span data-stu-id="19519-422">Order ID</span></span></td>
<td><p><span data-ttu-id="19519-423">Identificatore univoco di un ordine nella piattaforma di e-commerce di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="19519-424">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-425">Data ordine</span><span class="sxs-lookup"><span data-stu-id="19519-425">Order date</span></span></td>
<td><p><span data-ttu-id="19519-426">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="19519-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="19519-427">ProductId</span></span></td>
<td><p><span data-ttu-id="19519-428">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="19519-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="19519-429">SkuId</span></span></td>
<td><p><span data-ttu-id="19519-430">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="19519-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="19519-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="19519-432">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="19519-432">The ID for a particular Availability.</span></span> <span data-ttu-id="19519-433">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="19519-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-434">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="19519-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="19519-435">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="19519-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-436">Nome prodotto</span><span class="sxs-lookup"><span data-stu-id="19519-436">Product name</span></span></td>
<td><p><span data-ttu-id="19519-437">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="19519-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="19519-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="19519-439">Nome dell'autore del prodotto.</span><span class="sxs-lookup"><span data-stu-id="19519-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="19519-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="19519-441">ID univoco per il server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="19519-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-442">Descrizione di sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="19519-443">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-444">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="19519-445">Identificatore univoco per una sottoscrizione nella piattaforma di e-commerce di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="19519-446">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="19519-447">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="19519-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="19519-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="19519-449">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="19519-449">Start day of the charges.</span></span> <span data-ttu-id="19519-450">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="19519-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="19519-452">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="19519-452">End day of the charges.</span></span> <span data-ttu-id="19519-453">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="19519-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-454">Termine e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="19519-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="19519-455">La lunghezza del termine e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="19519-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="19519-456">Ad esempio, "1 anno, mensilmente."</span><span class="sxs-lookup"><span data-stu-id="19519-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-457">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="19519-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="19519-458">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="19519-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-459">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="19519-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="19519-460">Il prezzo come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="19519-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="19519-461">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-462">Prezzo unitario effettivi</span><span class="sxs-lookup"><span data-stu-id="19519-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="19519-463">Il prezzo unitario dopo che sono state apportate modifiche.</span><span class="sxs-lookup"><span data-stu-id="19519-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-464">Quantità</span><span class="sxs-lookup"><span data-stu-id="19519-464">Quantity</span></span></td>
<td><p><span data-ttu-id="19519-465">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="19519-465">Number of units.</span></span> <span data-ttu-id="19519-466">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-467">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="19519-467">Unit type</span></span></td>
<td><p><span data-ttu-id="19519-468">Il tipo di unità da acquistare.</span><span class="sxs-lookup"><span data-stu-id="19519-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="19519-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="19519-470">Una spiegazione di eventuali sconti.</span><span class="sxs-lookup"><span data-stu-id="19519-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-471">Totale parziale</span><span class="sxs-lookup"><span data-stu-id="19519-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="19519-472">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-472">Total before tax.</span></span> <span data-ttu-id="19519-473">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="19519-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-474">Totale delle imposte</span><span class="sxs-lookup"><span data-stu-id="19519-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="19519-475">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="19519-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-476">Total</span><span class="sxs-lookup"><span data-stu-id="19519-476">Total</span></span></td>
<td><p><span data-ttu-id="19519-477">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-477">Total after tax.</span></span> <span data-ttu-id="19519-478">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-479">Currency</span><span class="sxs-lookup"><span data-stu-id="19519-479">Currency</span></span></td>
<td><p><span data-ttu-id="19519-480">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-480">Currency type.</span></span> <span data-ttu-id="19519-481">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="19519-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="19519-482">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="19519-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="19519-484">Un identificatore alternativo a un ID.</span><span class="sxs-lookup"><span data-stu-id="19519-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="19519-485">Campi dei file di utilizzo in modo proporzionale giornaliera</span><span class="sxs-lookup"><span data-stu-id="19519-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="19519-486">Colonna</span><span class="sxs-lookup"><span data-stu-id="19519-486">Column</span></span></th>
<th><span data-ttu-id="19519-487">Descrizione</span><span class="sxs-lookup"><span data-stu-id="19519-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="19519-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="19519-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="19519-489">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="19519-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="19519-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="19519-491">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="19519-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="19519-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="19519-493">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="19519-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="19519-495">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="19519-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="19519-496">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="19519-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="19519-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="19519-498">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-498">The customer’s domain name.</span></span> <span data-ttu-id="19519-499">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-500">Paese cliente</span><span class="sxs-lookup"><span data-stu-id="19519-500">Customer country</span></span></td>
<td><p><span data-ttu-id="19519-501">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="19519-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="19519-502">MPNID</span></span></td>
<td><p><span data-ttu-id="19519-503">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="19519-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-504">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="19519-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="19519-505">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="19519-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="19519-506">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="19519-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="19519-508">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="19519-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="19519-509">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="19519-510">ProductId</span></span></td>
<td><p><span data-ttu-id="19519-511">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="19519-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="19519-512">SkuId</span></span></td>
<td><p><span data-ttu-id="19519-513">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="19519-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="19519-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="19519-515">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="19519-515">The ID for a particular Availability.</span></span> <span data-ttu-id="19519-516">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="19519-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-517">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="19519-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="19519-518">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="19519-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="19519-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="19519-520">Il nome dell'autore.</span><span class="sxs-lookup"><span data-stu-id="19519-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="19519-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="19519-522">ID dell'editore, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="19519-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="19519-523">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="19519-524">Descrizione di sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="19519-525">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="19519-526">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="19519-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-527">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="19519-528">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="19519-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="19519-529">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="19519-530">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="19519-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="19519-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="19519-532">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="19519-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="19519-533">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="19519-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="19519-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="19519-535">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="19519-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="19519-536">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="19519-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-537">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="19519-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="19519-538">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="19519-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-539">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="19519-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="19519-540">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="19519-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-541">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="19519-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="19519-542">Il servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="19519-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-543">Id misuratore</span><span class="sxs-lookup"><span data-stu-id="19519-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="19519-544">L'ID per il misuratore in uso.</span><span class="sxs-lookup"><span data-stu-id="19519-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-545">Misuratore sottocategoria</span><span class="sxs-lookup"><span data-stu-id="19519-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="19519-546">Tipo di servizio di Azure che possa influenzare il tasso di.</span><span class="sxs-lookup"><span data-stu-id="19519-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-547">Nome misuratore</span><span class="sxs-lookup"><span data-stu-id="19519-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="19519-548">L'unità di misura per il misuratore consumato.</span><span class="sxs-lookup"><span data-stu-id="19519-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-549">Area geografica misuratore</span><span class="sxs-lookup"><span data-stu-id="19519-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="19519-550">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="19519-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-551">Unit</span><span class="sxs-lookup"><span data-stu-id="19519-551">Unit</span></span></td>
<td><p><span data-ttu-id="19519-552">L'unità della risorsa di nome.</span><span class="sxs-lookup"><span data-stu-id="19519-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-553">Quantità consumata</span><span class="sxs-lookup"><span data-stu-id="19519-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="19519-554">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="19519-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="19519-555">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="19519-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-556">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="19519-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="19519-557">La Data Center in cui è in esecuzione il misuratore.</span><span class="sxs-lookup"><span data-stu-id="19519-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-558">Servizio consumato</span><span class="sxs-lookup"><span data-stu-id="19519-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="19519-559">Il servizio di piattaforma Azure che hai usato.</span><span class="sxs-lookup"><span data-stu-id="19519-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-560">Gruppo di risorse</span><span class="sxs-lookup"><span data-stu-id="19519-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="19519-561">Il gruppo di risorse in cui è in esecuzione il misuratore distribuito.</span><span class="sxs-lookup"><span data-stu-id="19519-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-562">URI di risorsa</span><span class="sxs-lookup"><span data-stu-id="19519-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="19519-563">L'URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="19519-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-564">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="19519-564">Charge type</span></span></td>
<td><p><span data-ttu-id="19519-565">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="19519-565">The type of charge or adjustment.</span></span> <span data-ttu-id="19519-566">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-567">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="19519-567">Unit price</span></span></td>
<td><p><span data-ttu-id="19519-568">Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="19519-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="19519-569">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-570">Quantità</span><span class="sxs-lookup"><span data-stu-id="19519-570">Quantity</span></span></td>
<td><p><span data-ttu-id="19519-571">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="19519-571">Number of licenses.</span></span> <span data-ttu-id="19519-572">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-573">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="19519-573">Unit type</span></span></td>
<td><p><span data-ttu-id="19519-574">Il tipo di unità il misuratore viene addebitato.</span><span class="sxs-lookup"><span data-stu-id="19519-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="19519-575">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="19519-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-576">Fatturazione mettono fiscali</span><span class="sxs-lookup"><span data-stu-id="19519-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="19519-577">Importo totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-578">Valuta di fatturazione</span><span class="sxs-lookup"><span data-stu-id="19519-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="19519-579">Valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="19519-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-580">Prezzo totale al lordo di imposte</span><span class="sxs-lookup"><span data-stu-id="19519-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="19519-581">Il prezzo prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-582">Valuta i prezzi</span><span class="sxs-lookup"><span data-stu-id="19519-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="19519-583">Valuta nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="19519-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-584">Informazioni di servizio 1</span><span class="sxs-lookup"><span data-stu-id="19519-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="19519-585">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="19519-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-586">Servizio Info 2</span><span class="sxs-lookup"><span data-stu-id="19519-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="19519-587">Un campo legacy che acquisisce metadati specifici del servizio facoltativi.</span><span class="sxs-lookup"><span data-stu-id="19519-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="19519-588">Tag</span><span class="sxs-lookup"><span data-stu-id="19519-588">Tags</span></span></td>
<td><p><span data-ttu-id="19519-589">Tag che assegnare al misuratore nell'ordine per raggruppare i record di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="19519-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="19519-590">Ad esempio, è possibile utilizzare i tag per distribuire i costi dal reparto che usa il misuratore.</span><span class="sxs-lookup"><span data-stu-id="19519-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="19519-591">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="19519-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="19519-592">Informazioni aggiuntive non trattate in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="19519-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="19519-593">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="19519-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="19519-594">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="19519-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="19519-595">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="19519-596">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="19519-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="19519-597">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="19519-598">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="19519-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="19519-599">Descrizione dell'addebito in fattura</span><span class="sxs-lookup"><span data-stu-id="19519-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="19519-600">Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="19519-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="19519-601">Descrizione dell'addebito</span><span class="sxs-lookup"><span data-stu-id="19519-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="19519-602">Modalità di mapping di questi tipi di addebito alla fattura</span><span class="sxs-lookup"><span data-stu-id="19519-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="19519-603">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="19519-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="19519-604">Commessione di attivazione</span><span class="sxs-lookup"><span data-stu-id="19519-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-605">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="19519-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="19519-606">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="19519-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-607">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="19519-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-608">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="19519-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-609">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="19519-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-610">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-611">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="19519-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-612">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="19519-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-613">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="19519-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-614">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="19519-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-615">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="19519-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-616">Il tipo di addebito per una sottoscrizione quando si utilizza la fatturazione annuale</span><span class="sxs-lookup"><span data-stu-id="19519-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-617">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="19519-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-618">Il tipo di addebito per una sottoscrizione quando si utilizza la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="19519-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-619">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="19519-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-620">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="19519-621">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="19519-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-622">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-623">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="19519-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-624">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="19519-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="19519-625">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="19519-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="19519-626">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="19519-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-627">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="19519-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="19519-628">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="19519-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-629">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="19519-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-630">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="19519-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="19519-631">Crediti</span><span class="sxs-lookup"><span data-stu-id="19519-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="19519-632">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="19519-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-633">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="19519-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-634">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="19519-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="19519-635">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="19519-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="19519-636">Sconti basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="19519-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="19519-637">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="19519-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-638">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="19519-639">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="19519-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-640">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="19519-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-641">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="19519-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-642">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="19519-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-643">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="19519-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-644">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="19519-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-645">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="19519-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="19519-646">Basato su licenza sconti</span><span class="sxs-lookup"><span data-stu-id="19519-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="19519-647">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="19519-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="19519-648">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="19519-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="19519-649"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="19519-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="19519-650">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="19519-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="19519-651">Eccezione: &quot;compensa una voce&quot; include già le imposte.</span><span class="sxs-lookup"><span data-stu-id="19519-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="19519-652">Vedi crediti, sopra.</span><span class="sxs-lookup"><span data-stu-id="19519-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="19519-653">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="19519-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="19519-654">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="19519-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="19519-655">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="19519-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
