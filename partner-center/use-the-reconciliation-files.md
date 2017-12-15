---
title: Usare i file di riconciliazione | Centro per i partner
description: Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892204ebcdfe1e1318985f2d50df8af2238bd4c1
ms.sourcegitcommit: 2436cb77fbefc41cc9cb3e62e8a616b6326c557f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b8b9a-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="b8b9a-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="b8b9a-104">Applies to</span></span>**

-  <span data-ttu-id="b8b9a-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b8b9a-105">Partner Center</span></span>
-  <span data-ttu-id="b8b9a-106">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="b8b9a-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="b8b9a-107">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="b8b9a-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="b8b9a-108">Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="b8b9a-109">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b8b9a-110">Eseguire la scomposizione dei dati in base al partner</span><span class="sxs-lookup"><span data-stu-id="b8b9a-110">Itemize by partner</span></span>


<span data-ttu-id="b8b9a-111">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b8b9a-112">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b8b9a-112">MPN ID</span></span></th>
<th><span data-ttu-id="b8b9a-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b8b9a-114">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b8b9a-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="b8b9a-115">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-116">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="b8b9a-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b8b9a-117">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b8b9a-118">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b8b9a-119">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b8b9a-120">Per visualizzare o aggiornare il rivenditore, nel menu del Centro per i partner seleziona <strong>Clienti</strong> e quindi scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b8b9a-121">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b8b9a-122">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b8b9a-123">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b8b9a-124">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b8b9a-125">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="b8b9a-126">Campi dei file in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="b8b9a-126">License-based file fields</span></span>


<span data-ttu-id="b8b9a-127">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b8b9a-128">Colonna</span><span class="sxs-lookup"><span data-stu-id="b8b9a-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b8b9a-129">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b8b9a-130">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="b8b9a-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b8b9a-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="b8b9a-132">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b8b9a-133">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b8b9a-134">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b8b9a-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b8b9a-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="b8b9a-137">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b8b9a-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b8b9a-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-139">OrderID</span></span></td>
<td><p><span data-ttu-id="b8b9a-140">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b8b9a-141">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b8b9a-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b8b9a-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b8b9a-144">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b8b9a-145">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b8b9a-146">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b8b9a-147">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b8b9a-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b8b9a-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b8b9a-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b8b9a-150">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b8b9a-151">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b8b9a-152">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b8b9a-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b8b9a-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-154">OfferID</span></span></td>
<td><p><span data-ttu-id="b8b9a-155">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-155">Unique offer ID.</span></span> <span data-ttu-id="b8b9a-156">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b8b9a-157"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b8b9a-158">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b8b9a-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b8b9a-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b8b9a-161">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b8b9a-162"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b8b9a-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b8b9a-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-164">OfferName</span></span></td>
<td><p><span data-ttu-id="b8b9a-165">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b8b9a-166">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-168">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b8b9a-169">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b8b9a-170">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b8b9a-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b8b9a-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-173">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b8b9a-174">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b8b9a-175">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b8b9a-176">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b8b9a-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b8b9a-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-179">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b8b9a-180">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b8b9a-181">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b8b9a-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b8b9a-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-184">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="b8b9a-185">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b8b9a-186">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b8b9a-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b8b9a-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b8b9a-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="b8b9a-189">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-189">The type of charge or adjustment.</span></span> <span data-ttu-id="b8b9a-190">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b8b9a-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b8b9a-191">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b8b9a-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b8b9a-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b8b9a-193">Prezzo per postazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-193">Price per seat.</span></span> <span data-ttu-id="b8b9a-194">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b8b9a-195">6.82</span><span class="sxs-lookup"><span data-stu-id="b8b9a-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="b8b9a-196">Quantity</span></span></td>
<td><p><span data-ttu-id="b8b9a-197">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-197">Number of seats.</span></span> <span data-ttu-id="b8b9a-198">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b8b9a-199">2</span><span class="sxs-lookup"><span data-stu-id="b8b9a-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-200">Amount</span><span class="sxs-lookup"><span data-stu-id="b8b9a-200">Amount</span></span></td>
<td><p><span data-ttu-id="b8b9a-201">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-201">Total of price for quantity.</span></span> <span data-ttu-id="b8b9a-202">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b8b9a-203">13.32</span><span class="sxs-lookup"><span data-stu-id="b8b9a-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b8b9a-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b8b9a-205">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b8b9a-206">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b8b9a-207">2.32</span><span class="sxs-lookup"><span data-stu-id="b8b9a-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b8b9a-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="b8b9a-209">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-209">Total before tax.</span></span> <span data-ttu-id="b8b9a-210">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b8b9a-211">11</span><span class="sxs-lookup"><span data-stu-id="b8b9a-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-212">Tax</span><span class="sxs-lookup"><span data-stu-id="b8b9a-212">Tax</span></span></td>
<td><p><span data-ttu-id="b8b9a-213">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b8b9a-214">0</span><span class="sxs-lookup"><span data-stu-id="b8b9a-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b8b9a-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b8b9a-216">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-216">Total after tax.</span></span> <span data-ttu-id="b8b9a-217">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b8b9a-218">11</span><span class="sxs-lookup"><span data-stu-id="b8b9a-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-219">Currency</span><span class="sxs-lookup"><span data-stu-id="b8b9a-219">Currency</span></span></td>
<td><p><span data-ttu-id="b8b9a-220">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-220">Currency type.</span></span> <span data-ttu-id="b8b9a-221">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="b8b9a-222">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b8b9a-223">EUR</span><span class="sxs-lookup"><span data-stu-id="b8b9a-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="b8b9a-225">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b8b9a-226">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b8b9a-227">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="b8b9a-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-228">MPNID</span></span></td>
<td><p><span data-ttu-id="b8b9a-229">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="b8b9a-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b8b9a-230">4390934</span><span class="sxs-lookup"><span data-stu-id="b8b9a-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b8b9a-232">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b8b9a-233">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="b8b9a-234">4390934</span><span class="sxs-lookup"><span data-stu-id="b8b9a-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-235">DomainName</span></span></td>
<td><p><span data-ttu-id="b8b9a-236">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="b8b9a-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b8b9a-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b8b9a-239">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-239">Subscription nickname.</span></span> <span data-ttu-id="b8b9a-240">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b8b9a-241">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="b8b9a-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b8b9a-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b8b9a-243">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b8b9a-244">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b8b9a-245">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="b8b9a-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b8b9a-246">Campi dei file in base all'uso</span><span class="sxs-lookup"><span data-stu-id="b8b9a-246">Usage-based file fields</span></span>


<span data-ttu-id="b8b9a-247">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b8b9a-248">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b8b9a-249">Colonna</span><span class="sxs-lookup"><span data-stu-id="b8b9a-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b8b9a-250">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b8b9a-251">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="b8b9a-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="b8b9a-253">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b8b9a-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b8b9a-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="b8b9a-256">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b8b9a-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b8b9a-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b8b9a-259">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b8b9a-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="b8b9a-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="b8b9a-262">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b8b9a-263">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b8b9a-264">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="b8b9a-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-265">MPNID</span></span></td>
<td><p><span data-ttu-id="b8b9a-266">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b8b9a-267">4390934</span><span class="sxs-lookup"><span data-stu-id="b8b9a-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b8b9a-269">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b8b9a-270">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="b8b9a-271">4390934</span><span class="sxs-lookup"><span data-stu-id="b8b9a-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b8b9a-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b8b9a-273">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b8b9a-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b8b9a-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-276">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b8b9a-277">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b8b9a-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b8b9a-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-280">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b8b9a-281">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b8b9a-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b8b9a-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b8b9a-284">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b8b9a-285">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b8b9a-286">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b8b9a-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b8b9a-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b8b9a-289">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b8b9a-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b8b9a-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b8b9a-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b8b9a-292">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="b8b9a-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b8b9a-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b8b9a-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-294">OrderID</span></span></td>
<td><p><span data-ttu-id="b8b9a-295">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b8b9a-296">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b8b9a-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b8b9a-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="b8b9a-299">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b8b9a-300">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="b8b9a-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b8b9a-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="b8b9a-302">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b8b9a-303">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="b8b9a-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b8b9a-304">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="b8b9a-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b8b9a-306">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b8b9a-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b8b9a-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-308">Resource Name</span><span class="sxs-lookup"><span data-stu-id="b8b9a-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="b8b9a-309">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b8b9a-310">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b8b9a-311">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-312">Region</span><span class="sxs-lookup"><span data-stu-id="b8b9a-312">Region</span></span></td>
<td><p><span data-ttu-id="b8b9a-313">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-313">The region the usage applies to.</span></span> <span data-ttu-id="b8b9a-314">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b8b9a-315">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="b8b9a-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-316">SKU</span><span class="sxs-lookup"><span data-stu-id="b8b9a-316">SKU</span></span></td>
<td><p><span data-ttu-id="b8b9a-317">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="b8b9a-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b8b9a-318">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="b8b9a-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b8b9a-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b8b9a-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b8b9a-320">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b8b9a-321">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b8b9a-322">1</span><span class="sxs-lookup"><span data-stu-id="b8b9a-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b8b9a-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b8b9a-324">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b8b9a-325">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b8b9a-326">11</span><span class="sxs-lookup"><span data-stu-id="b8b9a-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b8b9a-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b8b9a-328">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-328">Units included as part of the offer.</span></span> <span data-ttu-id="b8b9a-329">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b8b9a-330">0</span><span class="sxs-lookup"><span data-stu-id="b8b9a-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b8b9a-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b8b9a-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b8b9a-332">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b8b9a-333">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b8b9a-334">11</span><span class="sxs-lookup"><span data-stu-id="b8b9a-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b8b9a-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="b8b9a-336">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b8b9a-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="b8b9a-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b8b9a-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b8b9a-339">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b8b9a-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="b8b9a-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b8b9a-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b8b9a-342">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b8b9a-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="b8b9a-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b8b9a-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b8b9a-345">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b8b9a-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="b8b9a-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-347">Currency</span><span class="sxs-lookup"><span data-stu-id="b8b9a-347">Currency</span></span></td>
<td><p><span data-ttu-id="b8b9a-348">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-348">Currency type.</span></span> <span data-ttu-id="b8b9a-349">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="b8b9a-350">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b8b9a-351">EUR</span><span class="sxs-lookup"><span data-stu-id="b8b9a-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b8b9a-353">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-353">Pretax price per unit.</span></span> <span data-ttu-id="b8b9a-354">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b8b9a-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="b8b9a-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b8b9a-357">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-357">Post tax price per unit.</span></span> <span data-ttu-id="b8b9a-358">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b8b9a-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="b8b9a-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b8b9a-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="b8b9a-361">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-361">The type of charge or adjustment.</span></span> <span data-ttu-id="b8b9a-362">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b8b9a-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b8b9a-363">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b8b9a-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b8b9a-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b8b9a-365">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b8b9a-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="b8b9a-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="b8b9a-368">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b8b9a-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b8b9a-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b8b9a-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b8b9a-371">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b8b9a-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="b8b9a-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b8b9a-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="b8b9a-374">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b8b9a-375">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b8b9a-376">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b8b9a-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="b8b9a-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b8b9a-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b8b9a-379">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b8b9a-380">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="b8b9a-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-381">Project</span><span class="sxs-lookup"><span data-stu-id="b8b9a-381">Project</span></span></td>
<td><p><span data-ttu-id="b8b9a-382">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="b8b9a-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b8b9a-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b8b9a-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b8b9a-385">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b8b9a-386">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="b8b9a-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b8b9a-387">Se hai un pacchetto da 25 connessioni ServiceBus e ne hai utilizzata 1 per quel giorno, l'uso giornaliero registrato sarà "25 Connections / 30 Days – Used: 1.000000".</span><span class="sxs-lookup"><span data-stu-id="b8b9a-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b8b9a-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="b8b9a-389">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b8b9a-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b8b9a-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b8b9a-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="b8b9a-391">DomainName</span></span></td>
<td><p><span data-ttu-id="b8b9a-392">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="b8b9a-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b8b9a-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b8b9a-394">Unità</span><span class="sxs-lookup"><span data-stu-id="b8b9a-394">Unit</span></span></td>
<td><p><span data-ttu-id="b8b9a-395">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="b8b9a-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b8b9a-396">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="b8b9a-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="b8b9a-397">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b8b9a-398">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b8b9a-399">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b8b9a-400">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="b8b9a-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b8b9a-401">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b8b9a-402">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="b8b9a-403">Descrizione dell'addebito in fattura</span><span class="sxs-lookup"><span data-stu-id="b8b9a-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b8b9a-404">Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b8b9a-405">Descrizione dell'addebito</span><span class="sxs-lookup"><span data-stu-id="b8b9a-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b8b9a-406">Modalità di mapping di questi tipi di addebito alla fattura</span><span class="sxs-lookup"><span data-stu-id="b8b9a-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="b8b9a-407">Addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="b8b9a-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-408">Istanza di annullamento rateizzata</span><span class="sxs-lookup"><span data-stu-id="b8b9a-408">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-409">Addebiti rateizzati rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-409">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="b8b9a-410">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-411">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="b8b9a-411">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-412">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-412">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-413">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="b8b9a-413">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-414">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="b8b9a-414">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-415">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="b8b9a-415">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-416">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="b8b9a-416">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-417">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="b8b9a-417">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-418">Tariffe rateizzate all'acquisto</span><span class="sxs-lookup"><span data-stu-id="b8b9a-418">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-419">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="b8b9a-419">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-420">Addebito iniziale per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-420">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-421">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-421">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-422">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-422">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-423">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-423">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-424">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-424">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b8b9a-425">Altri prodotti e servizi</span><span class="sxs-lookup"><span data-stu-id="b8b9a-425">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-426">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-426">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-427">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-427">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-428">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-428">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="b8b9a-429">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-429">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-430">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="b8b9a-430">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-431">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="b8b9a-431">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b8b9a-432">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-432">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-433">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="b8b9a-433">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-434">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="b8b9a-434">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b8b9a-435">Crediti e rettifiche</span><span class="sxs-lookup"><span data-stu-id="b8b9a-435">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-436">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="b8b9a-436">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-437">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="b8b9a-437">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-438">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-438">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b8b9a-439">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-439">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="b8b9a-440">Altri sconti</span><span class="sxs-lookup"><span data-stu-id="b8b9a-440">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="b8b9a-441">(in base all'uso)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-441">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-442">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-442">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-443">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-443">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="b8b9a-444">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-444">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-445">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-445">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-446">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="b8b9a-446">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="b8b9a-447">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="b8b9a-447">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-448">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b8b9a-448">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="b8b9a-449">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="b8b9a-449">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-450">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="b8b9a-450">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b8b9a-451">Altri sconti</span><span class="sxs-lookup"><span data-stu-id="b8b9a-451">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="b8b9a-452">(in base alle licenze)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-452">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="b8b9a-453">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="b8b9a-453">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="b8b9a-454">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-454">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b8b9a-455"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-455"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="b8b9a-456">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="b8b9a-456">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="b8b9a-457">Eccezione: "Compensa una voce" include già le imposte.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-457">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="b8b9a-458">Vedi Crediti e rettifiche, sopra.</span><span class="sxs-lookup"><span data-stu-id="b8b9a-458">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-459">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="b8b9a-459">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b8b9a-460">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-460">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b8b9a-461">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="b8b9a-461">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
