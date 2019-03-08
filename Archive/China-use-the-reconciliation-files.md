---
title: Usare i file di riconciliazione (centro per i Partner gestito da 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584984"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="372a6-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="372a6-103">Use the reconciliation files</span></span>

<span data-ttu-id="372a6-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="372a6-104">**Applies to**</span></span>

-   <span data-ttu-id="372a6-105">Centro per i partner gestito da 21Vianet</span><span class="sxs-lookup"><span data-stu-id="372a6-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="372a6-106">Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="372a6-107">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="372a6-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="372a6-108">Specificare i dettagli da partner</span><span class="sxs-lookup"><span data-stu-id="372a6-108">Itemize by partner</span></span>


<span data-ttu-id="372a6-109">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="372a6-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="372a6-110">ID MPN</span><span class="sxs-lookup"><span data-stu-id="372a6-110">MPN ID</span></span></th>
<th><span data-ttu-id="372a6-111">Descrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="372a6-112">ID MPN</span><span class="sxs-lookup"><span data-stu-id="372a6-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="372a6-113">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="372a6-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-114">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="372a6-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="372a6-115">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="372a6-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="372a6-116">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="372a6-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="372a6-117">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="372a6-118">Per visualizzare o aggiornare il rivenditore, nel menu del Centro per i partner seleziona <strong>Clienti</strong> e quindi scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="372a6-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="372a6-119">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="372a6-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="372a6-120">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="372a6-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="372a6-121">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="372a6-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="372a6-122">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="372a6-123">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="372a6-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="372a6-124">Campi del file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="372a6-124">License-based file fields</span></span>


<span data-ttu-id="372a6-125">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="372a6-126"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="372a6-127"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="372a6-128"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="372a6-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="372a6-130">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="372a6-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="372a6-131">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="372a6-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="372a6-132">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="372a6-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="372a6-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="372a6-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="372a6-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="372a6-135">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="372a6-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="372a6-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="372a6-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="372a6-137">OrderID</span></span></td>
<td><p><span data-ttu-id="372a6-138">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="372a6-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="372a6-139">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="372a6-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="372a6-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="372a6-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="372a6-142">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="372a6-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="372a6-143">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="372a6-144">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="372a6-145">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="372a6-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="372a6-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="372a6-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="372a6-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="372a6-148">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="372a6-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="372a6-149">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="372a6-150">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="372a6-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="372a6-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="372a6-152">OfferID</span></span></td>
<td><p><span data-ttu-id="372a6-153">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="372a6-153">Unique offer ID.</span></span> <span data-ttu-id="372a6-154">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="372a6-155"><b>Nota</b>: Questo valore non corrisponde ID offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="372a6-156">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="372a6-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="372a6-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="372a6-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="372a6-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="372a6-159">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="372a6-160"><b>Nota</b>: Questo valore corrisponde all'ID dell'offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="372a6-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="372a6-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="372a6-162">OfferName</span></span></td>
<td><p><span data-ttu-id="372a6-163">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="372a6-164">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="372a6-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="372a6-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="372a6-166">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="372a6-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="372a6-167">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="372a6-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="372a6-168">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="372a6-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="372a6-169">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="372a6-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="372a6-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="372a6-171">La data di fine sottoscrizione: 12 mesi + x giorni dopo la data di inizio (in modo da allinearsi partner data di fatturazione) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="372a6-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="372a6-172">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="372a6-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="372a6-173">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="372a6-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="372a6-174">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="372a6-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="372a6-175">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="372a6-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="372a6-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="372a6-177">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="372a6-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="372a6-178">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="372a6-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="372a6-179">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="372a6-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="372a6-180">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="372a6-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="372a6-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="372a6-182">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="372a6-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="372a6-183">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="372a6-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="372a6-184">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="372a6-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="372a6-185">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="372a6-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="372a6-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="372a6-187">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="372a6-187">The type of charge or adjustment.</span></span> <span data-ttu-id="372a6-188">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="372a6-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="372a6-189">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="372a6-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="372a6-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="372a6-191">Prezzo per postazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-191">Price per seat.</span></span> <span data-ttu-id="372a6-192">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="372a6-193">6.82</span><span class="sxs-lookup"><span data-stu-id="372a6-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-194">Quantità</span><span class="sxs-lookup"><span data-stu-id="372a6-194">Quantity</span></span></td>
<td><p><span data-ttu-id="372a6-195">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="372a6-195">Number of seats.</span></span> <span data-ttu-id="372a6-196">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="372a6-197">2</span><span class="sxs-lookup"><span data-stu-id="372a6-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-198">Importo</span><span class="sxs-lookup"><span data-stu-id="372a6-198">Amount</span></span></td>
<td><p><span data-ttu-id="372a6-199">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="372a6-199">Total of price for quantity.</span></span> <span data-ttu-id="372a6-200">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="372a6-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="372a6-201">13.32</span><span class="sxs-lookup"><span data-stu-id="372a6-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="372a6-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="372a6-203">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="372a6-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="372a6-204">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="372a6-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="372a6-205">2.32</span><span class="sxs-lookup"><span data-stu-id="372a6-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-206">Subtotal</span><span class="sxs-lookup"><span data-stu-id="372a6-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="372a6-207">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="372a6-207">Total before tax.</span></span> <span data-ttu-id="372a6-208">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="372a6-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="372a6-209">11</span><span class="sxs-lookup"><span data-stu-id="372a6-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-210">Imposta</span><span class="sxs-lookup"><span data-stu-id="372a6-210">Tax</span></span></td>
<td><p><span data-ttu-id="372a6-211">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="372a6-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="372a6-212">0</span><span class="sxs-lookup"><span data-stu-id="372a6-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="372a6-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="372a6-214">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="372a6-214">Total after tax.</span></span> <span data-ttu-id="372a6-215">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="372a6-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="372a6-216">11</span><span class="sxs-lookup"><span data-stu-id="372a6-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-217">Valuta</span><span class="sxs-lookup"><span data-stu-id="372a6-217">Currency</span></span></td>
<td><p><span data-ttu-id="372a6-218">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="372a6-218">Currency type.</span></span> <span data-ttu-id="372a6-219">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="372a6-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="372a6-220">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="372a6-221">CNY</span><span class="sxs-lookup"><span data-stu-id="372a6-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="372a6-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="372a6-223">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="372a6-224">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="372a6-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="372a6-225">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="372a6-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="372a6-226">MPNID</span></span></td>
<td><p><span data-ttu-id="372a6-227">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="372a6-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="372a6-228">4390934</span><span class="sxs-lookup"><span data-stu-id="372a6-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="372a6-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="372a6-230">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="372a6-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="372a6-231">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="372a6-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="372a6-232">4390934</span><span class="sxs-lookup"><span data-stu-id="372a6-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="372a6-233">DomainName</span></span></td>
<td><p><span data-ttu-id="372a6-234">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="372a6-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="372a6-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="372a6-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="372a6-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="372a6-237">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="372a6-237">Subscription nickname.</span></span> <span data-ttu-id="372a6-238">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="372a6-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="372a6-239">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="372a6-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="372a6-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="372a6-241">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="372a6-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="372a6-242">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="372a6-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="372a6-243">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="372a6-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="372a6-244">Campi del file basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="372a6-244">Usage-based file fields</span></span>


<span data-ttu-id="372a6-245">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="372a6-246">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="372a6-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="372a6-247"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="372a6-248"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="372a6-249"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="372a6-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="372a6-251">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="372a6-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="372a6-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="372a6-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="372a6-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="372a6-254">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="372a6-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="372a6-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="372a6-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="372a6-257">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="372a6-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="372a6-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="372a6-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="372a6-260">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="372a6-261">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="372a6-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="372a6-262">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="372a6-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="372a6-263">MPNID</span></span></td>
<td><p><span data-ttu-id="372a6-264">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="372a6-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="372a6-265">4390934</span><span class="sxs-lookup"><span data-stu-id="372a6-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="372a6-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="372a6-267">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="372a6-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="372a6-268">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="372a6-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="372a6-269">4390934</span><span class="sxs-lookup"><span data-stu-id="372a6-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="372a6-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="372a6-271">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="372a6-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="372a6-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="372a6-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="372a6-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="372a6-274">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="372a6-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="372a6-275">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="372a6-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="372a6-276">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="372a6-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="372a6-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="372a6-278">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="372a6-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="372a6-279">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="372a6-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="372a6-280">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="372a6-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="372a6-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="372a6-282">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="372a6-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="372a6-283">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="372a6-284">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="372a6-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="372a6-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="372a6-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="372a6-287">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="372a6-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="372a6-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="372a6-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="372a6-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="372a6-290">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="372a6-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="372a6-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="372a6-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="372a6-292">OrderID</span></span></td>
<td><p><span data-ttu-id="372a6-293">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="372a6-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="372a6-294">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="372a6-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="372a6-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="372a6-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="372a6-297">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="372a6-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="372a6-298">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="372a6-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="372a6-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="372a6-300">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="372a6-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="372a6-301">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="372a6-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="372a6-302">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="372a6-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="372a6-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="372a6-304">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="372a6-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="372a6-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="372a6-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-306">Resource Name</span><span class="sxs-lookup"><span data-stu-id="372a6-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="372a6-307">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="372a6-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="372a6-308">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="372a6-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="372a6-309">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="372a6-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-310">Region</span><span class="sxs-lookup"><span data-stu-id="372a6-310">Region</span></span></td>
<td><p><span data-ttu-id="372a6-311">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="372a6-311">The region the usage applies to.</span></span> <span data-ttu-id="372a6-312">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="372a6-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="372a6-313">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="372a6-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-314">SKU</span><span class="sxs-lookup"><span data-stu-id="372a6-314">SKU</span></span></td>
<td><p><span data-ttu-id="372a6-315">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="372a6-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="372a6-316">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="372a6-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="372a6-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="372a6-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="372a6-318">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="372a6-319">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="372a6-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="372a6-320">1</span><span class="sxs-lookup"><span data-stu-id="372a6-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="372a6-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="372a6-322">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="372a6-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="372a6-323">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="372a6-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="372a6-324">11</span><span class="sxs-lookup"><span data-stu-id="372a6-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="372a6-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="372a6-326">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="372a6-326">Units included as part of the offer.</span></span> <span data-ttu-id="372a6-327">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="372a6-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="372a6-328">0</span><span class="sxs-lookup"><span data-stu-id="372a6-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="372a6-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="372a6-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="372a6-330">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="372a6-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="372a6-331">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="372a6-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="372a6-332">11</span><span class="sxs-lookup"><span data-stu-id="372a6-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="372a6-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="372a6-334">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="372a6-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="372a6-335">$0.0808</span><span class="sxs-lookup"><span data-stu-id="372a6-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="372a6-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="372a6-337">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="372a6-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="372a6-338">$0.085</span><span class="sxs-lookup"><span data-stu-id="372a6-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="372a6-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="372a6-340">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="372a6-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="372a6-341">$0.08</span><span class="sxs-lookup"><span data-stu-id="372a6-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="372a6-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="372a6-343">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="372a6-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="372a6-344">$0.93</span><span class="sxs-lookup"><span data-stu-id="372a6-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-345">Valuta</span><span class="sxs-lookup"><span data-stu-id="372a6-345">Currency</span></span></td>
<td><p><span data-ttu-id="372a6-346">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="372a6-346">Currency type.</span></span> <span data-ttu-id="372a6-347">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="372a6-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="372a6-348">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="372a6-349">CNY</span><span class="sxs-lookup"><span data-stu-id="372a6-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="372a6-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="372a6-351">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="372a6-351">Pretax price per unit.</span></span> <span data-ttu-id="372a6-352">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="372a6-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="372a6-353">$0.08</span><span class="sxs-lookup"><span data-stu-id="372a6-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="372a6-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="372a6-355">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="372a6-355">Post tax price per unit.</span></span> <span data-ttu-id="372a6-356">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="372a6-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="372a6-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="372a6-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="372a6-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="372a6-359">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="372a6-359">The type of charge or adjustment.</span></span> <span data-ttu-id="372a6-360">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="372a6-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="372a6-361">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="372a6-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="372a6-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="372a6-363">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="372a6-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="372a6-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="372a6-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="372a6-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="372a6-366">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="372a6-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="372a6-367">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="372a6-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="372a6-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="372a6-369">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="372a6-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="372a6-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="372a6-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="372a6-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="372a6-372">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="372a6-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="372a6-373">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="372a6-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="372a6-374">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="372a6-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="372a6-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="372a6-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="372a6-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="372a6-377">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="372a6-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="372a6-378">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="372a6-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-379">Project</span><span class="sxs-lookup"><span data-stu-id="372a6-379">Project</span></span></td>
<td><p><span data-ttu-id="372a6-380">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="372a6-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="372a6-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="372a6-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="372a6-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="372a6-383">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="372a6-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="372a6-384">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="372a6-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="372a6-385">Se disponi di un pacchetto 25 di connessioni del bus di servizio eseguito il provisioning e si fosse utilizzato 1 durante il giorno, l'istruzione di utilizzo giornaliero per quel giorno indicherebbe "25 connessioni / 30 giorni: utilizzato: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="372a6-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="372a6-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="372a6-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="372a6-387">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="372a6-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="372a6-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="372a6-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="372a6-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="372a6-389">DomainName</span></span></td>
<td><p><span data-ttu-id="372a6-390">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="372a6-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="372a6-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="372a6-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="372a6-392">Addebiti di mapping tra una fattura e i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="372a6-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="372a6-393">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="372a6-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="372a6-394">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="372a6-395">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="372a6-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="372a6-396"><strong>Descrizione di addebito della fattura</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-397"><strong>Descrizione di addebito file di riconciliazione (ChargeType colonna)</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-398"><strong>Che cos'è l'addebito?</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-399"><strong>Come è possibile associare queste ChargeTypes nella fattura?</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="372a6-400"><strong>Addebiti periodici</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-401">Istanza di annullamento ripartita proporzionalmente</span><span class="sxs-lookup"><span data-stu-id="372a6-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-402">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="372a6-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="372a6-403">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-404">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="372a6-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-405">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-406">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="372a6-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-407">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="372a6-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-408">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="372a6-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-409">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="372a6-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-410">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="372a6-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-411">Tariffe rateizzate all'acquisto</span><span class="sxs-lookup"><span data-stu-id="372a6-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-412">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="372a6-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-413">Addebito iniziale per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-414">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="372a6-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-415">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-416">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="372a6-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-417">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-418"><strong>Altri prodotti e servizi</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-419">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="372a6-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-420">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="372a6-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-421">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="372a6-422"><strong>Costi di utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-423">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="372a6-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-424">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="372a6-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="372a6-425">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-426">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="372a6-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-427">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="372a6-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-428"><strong>I crediti &amp; regolazioni</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-429">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="372a6-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-430">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="372a6-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-431">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="372a6-432">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="372a6-433"><strong>Altri sconti</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="372a6-434">
<em>(basato su utilizzo)</em></span><span class="sxs-lookup"><span data-stu-id="372a6-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-435">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="372a6-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-436">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="372a6-437">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-438">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="372a6-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-439">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="372a6-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="372a6-440">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="372a6-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-441">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="372a6-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="372a6-442">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="372a6-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-443">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="372a6-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-444"><strong>Altri sconti</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="372a6-445">
<em>(license-based)</em></span><span class="sxs-lookup"><span data-stu-id="372a6-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-446"><em>Può essere applicato a più tipi di costo</em></span><span class="sxs-lookup"><span data-stu-id="372a6-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="372a6-447">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="372a6-448"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-449"><em>Può essere applicato a più tipi di costo</em></span><span class="sxs-lookup"><span data-stu-id="372a6-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="372a6-450"><em>Eccezione: "Una voce di offset" include già le imposte. Vedere i crediti &amp; regolazioni sopra.</em></span><span class="sxs-lookup"><span data-stu-id="372a6-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-451">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="372a6-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="372a6-452">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="372a6-453">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="372a6-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
