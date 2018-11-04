---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Per una visualizzazione di voci delle relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 4b5fbab84c30743e4d91b32bf4cbd2bb8b950992
ms.sourcegitcommit: b433061dff8f667c81b623c33417fb490d8e3b4a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/04/2018
ms.locfileid: "6022244"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b44f8-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-103">Use the reconciliation files</span></span>

**<span data-ttu-id="b44f8-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="b44f8-104">Applies to</span></span>**

-  <span data-ttu-id="b44f8-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b44f8-105">Partner Center</span></span>
-  <span data-ttu-id="b44f8-106">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="b44f8-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="b44f8-107">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="b44f8-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="b44f8-108">Per una visualizzazione di voci delle relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b44f8-109">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="b44f8-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b44f8-110">Eseguire la scomposizione dei dati in base al partner</span><span class="sxs-lookup"><span data-stu-id="b44f8-110">Itemize by partner</span></span>


<span data-ttu-id="b44f8-111">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="b44f8-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b44f8-112">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b44f8-112">MPN ID</span></span></th>
<th><span data-ttu-id="b44f8-113">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b44f8-114">ID MPN</span><span class="sxs-lookup"><span data-stu-id="b44f8-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="b44f8-115">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="b44f8-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-116">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="b44f8-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b44f8-117">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b44f8-118">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b44f8-119">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b44f8-120">Per visualizzare o aggiornare il rivenditore, il menu del centro per i Partner seleziona <strong>i clienti</strong>, quindi scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="b44f8-120">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b44f8-121">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="b44f8-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b44f8-122">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="b44f8-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b44f8-123">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="b44f8-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b44f8-124">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b44f8-125">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="b44f8-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="b44f8-126">Campi dei file in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="b44f8-126">License-based file fields</span></span>


<span data-ttu-id="b44f8-127">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b44f8-128">Colonna</span><span class="sxs-lookup"><span data-stu-id="b44f8-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b44f8-129">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b44f8-130">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="b44f8-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b44f8-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="b44f8-132">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b44f8-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b44f8-133">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="b44f8-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b44f8-134">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="b44f8-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b44f8-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b44f8-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b44f8-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="b44f8-137">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b44f8-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b44f8-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="b44f8-139">OrderID</span></span></td>
<td><p><span data-ttu-id="b44f8-140">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f8-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b44f8-141">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b44f8-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b44f8-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b44f8-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b44f8-144">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f8-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b44f8-145">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b44f8-146">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b44f8-147">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="b44f8-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b44f8-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b44f8-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b44f8-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b44f8-150">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="b44f8-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b44f8-151">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b44f8-152">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b44f8-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b44f8-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="b44f8-154">OfferID</span></span></td>
<td><p><span data-ttu-id="b44f8-155">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-155">Unique offer ID.</span></span> <span data-ttu-id="b44f8-156">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b44f8-157"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b44f8-158">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="b44f8-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b44f8-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b44f8-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b44f8-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b44f8-161">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b44f8-162"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b44f8-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b44f8-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="b44f8-164">OfferName</span></span></td>
<td><p><span data-ttu-id="b44f8-165">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b44f8-166">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="b44f8-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b44f8-168">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="b44f8-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b44f8-169">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="b44f8-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b44f8-170">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b44f8-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b44f8-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b44f8-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b44f8-173">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="b44f8-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b44f8-174">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b44f8-175">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="b44f8-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b44f8-176">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b44f8-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b44f8-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b44f8-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b44f8-179">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b44f8-180">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="b44f8-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b44f8-181">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b44f8-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b44f8-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b44f8-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b44f8-184">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="b44f8-185">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="b44f8-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b44f8-186">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="b44f8-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b44f8-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b44f8-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b44f8-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="b44f8-189">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="b44f8-189">The type of charge or adjustment.</span></span> <span data-ttu-id="b44f8-190">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b44f8-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b44f8-191">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b44f8-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b44f8-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b44f8-193">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b44f8-194">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b44f8-195">6.82</span><span class="sxs-lookup"><span data-stu-id="b44f8-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="b44f8-196">Quantity</span></span></td>
<td><p><span data-ttu-id="b44f8-197">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="b44f8-197">Number of seats.</span></span> <span data-ttu-id="b44f8-198">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b44f8-199">2</span><span class="sxs-lookup"><span data-stu-id="b44f8-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-200">Amount</span><span class="sxs-lookup"><span data-stu-id="b44f8-200">Amount</span></span></td>
<td><p><span data-ttu-id="b44f8-201">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="b44f8-201">Total of price for quantity.</span></span> <span data-ttu-id="b44f8-202">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b44f8-203">13.32</span><span class="sxs-lookup"><span data-stu-id="b44f8-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b44f8-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b44f8-205">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b44f8-206">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="b44f8-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b44f8-207">2.32</span><span class="sxs-lookup"><span data-stu-id="b44f8-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b44f8-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="b44f8-209">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-209">Total before tax.</span></span> <span data-ttu-id="b44f8-210">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b44f8-211">11</span><span class="sxs-lookup"><span data-stu-id="b44f8-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-212">Tax</span><span class="sxs-lookup"><span data-stu-id="b44f8-212">Tax</span></span></td>
<td><p><span data-ttu-id="b44f8-213">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="b44f8-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b44f8-214">0</span><span class="sxs-lookup"><span data-stu-id="b44f8-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b44f8-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b44f8-216">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-216">Total after tax.</span></span> <span data-ttu-id="b44f8-217">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b44f8-218">11</span><span class="sxs-lookup"><span data-stu-id="b44f8-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-219">Currency</span><span class="sxs-lookup"><span data-stu-id="b44f8-219">Currency</span></span></td>
<td><p><span data-ttu-id="b44f8-220">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-220">Currency type.</span></span> <span data-ttu-id="b44f8-221">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="b44f8-222">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b44f8-223">EUR</span><span class="sxs-lookup"><span data-stu-id="b44f8-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b44f8-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="b44f8-225">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b44f8-226">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="b44f8-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b44f8-227">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="b44f8-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="b44f8-228">MPNID</span></span></td>
<td><p><span data-ttu-id="b44f8-229">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="b44f8-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b44f8-230">4390934</span><span class="sxs-lookup"><span data-stu-id="b44f8-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b44f8-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b44f8-232">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b44f8-233">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="b44f8-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="b44f8-234">4390934</span><span class="sxs-lookup"><span data-stu-id="b44f8-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="b44f8-235">DomainName</span></span></td>
<td><p><span data-ttu-id="b44f8-236">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b44f8-237">Questo non deve essere usato per identificare in modo univoco il cliente quando il cliente/partner può aggiornare il dominio di reindirizzamento a microsito/predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="b44f8-237">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b44f8-238">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-238">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b44f8-239">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b44f8-239">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-240">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b44f8-240">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b44f8-241">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-241">Subscription nickname.</span></span> <span data-ttu-id="b44f8-242">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="b44f8-242">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b44f8-243">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="b44f8-243">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-244">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b44f8-244">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b44f8-245">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-245">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b44f8-246">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-246">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b44f8-247">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="b44f8-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b44f8-248">Campi dei file in base all'uso</span><span class="sxs-lookup"><span data-stu-id="b44f8-248">Usage-based file fields</span></span>


<span data-ttu-id="b44f8-249">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-249">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b44f8-250">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="b44f8-250">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b44f8-251">Colonna</span><span class="sxs-lookup"><span data-stu-id="b44f8-251">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b44f8-252">Descrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-252">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b44f8-253">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="b44f8-253">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-254">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b44f8-254">PartnerID</span></span></td>
<td><p><span data-ttu-id="b44f8-255">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b44f8-255">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b44f8-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b44f8-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-257">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b44f8-257">PartnerName</span></span></td>
<td><p><span data-ttu-id="b44f8-258">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-258">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b44f8-259">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b44f8-259">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-260">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b44f8-260">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b44f8-261">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-261">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b44f8-262">1010578050</span><span class="sxs-lookup"><span data-stu-id="b44f8-262">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-263">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b44f8-263">CustomerName</span></span></td>
<td><p><span data-ttu-id="b44f8-264">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-264">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b44f8-265">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="b44f8-265">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b44f8-266">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="b44f8-266">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-267">MPNID</span><span class="sxs-lookup"><span data-stu-id="b44f8-267">MPNID</span></span></td>
<td><p><span data-ttu-id="b44f8-268">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="b44f8-268">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b44f8-269">4390934</span><span class="sxs-lookup"><span data-stu-id="b44f8-269">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-270">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b44f8-270">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b44f8-271">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-271">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b44f8-272">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="b44f8-272">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="b44f8-273">4390934</span><span class="sxs-lookup"><span data-stu-id="b44f8-273">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-274">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b44f8-274">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b44f8-275">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="b44f8-275">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b44f8-276">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b44f8-276">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-277">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-277">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b44f8-278">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="b44f8-278">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b44f8-279">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="b44f8-279">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b44f8-280">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b44f8-280">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-281">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-281">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b44f8-282">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="b44f8-282">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b44f8-283">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="b44f8-283">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b44f8-284">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b44f8-284">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-285">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b44f8-285">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b44f8-286">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f8-286">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b44f8-287">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-287">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b44f8-288">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-288">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b44f8-289">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b44f8-289">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-290">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b44f8-290">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b44f8-291">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="b44f8-291">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b44f8-292">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b44f8-292">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-293">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b44f8-293">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b44f8-294">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="b44f8-294">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b44f8-295">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b44f8-295">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-296">OrderID</span><span class="sxs-lookup"><span data-stu-id="b44f8-296">OrderID</span></span></td>
<td><p><span data-ttu-id="b44f8-297">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f8-297">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b44f8-298">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-298">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b44f8-299">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b44f8-299">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-300">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b44f8-300">ServiceName</span></span></td>
<td><p><span data-ttu-id="b44f8-301">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-301">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b44f8-302">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="b44f8-302">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-303">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b44f8-303">ServiceType</span></span></td>
<td><p><span data-ttu-id="b44f8-304">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="b44f8-304">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b44f8-305">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="b44f8-305">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b44f8-306">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="b44f8-306">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-307">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b44f8-307">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b44f8-308">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="b44f8-308">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b44f8-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b44f8-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-310">Resource Name</span><span class="sxs-lookup"><span data-stu-id="b44f8-310">Resource Name</span></span></td>
<td><p><span data-ttu-id="b44f8-311">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="b44f8-311">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b44f8-312">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="b44f8-312">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b44f8-313">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="b44f8-313">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-314">Region</span><span class="sxs-lookup"><span data-stu-id="b44f8-314">Region</span></span></td>
<td><p><span data-ttu-id="b44f8-315">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="b44f8-315">The region the usage applies to.</span></span> <span data-ttu-id="b44f8-316">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="b44f8-316">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b44f8-317">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="b44f8-317">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-318">SKU</span><span class="sxs-lookup"><span data-stu-id="b44f8-318">SKU</span></span></td>
<td><p><span data-ttu-id="b44f8-319">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="b44f8-319">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b44f8-320">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="b44f8-320">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b44f8-321">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b44f8-321">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b44f8-322">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-322">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b44f8-323">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="b44f8-323">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b44f8-324">1</span><span class="sxs-lookup"><span data-stu-id="b44f8-324">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-325">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b44f8-325">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b44f8-326">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="b44f8-326">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b44f8-327">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-327">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b44f8-328">11</span><span class="sxs-lookup"><span data-stu-id="b44f8-328">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-329">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b44f8-329">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b44f8-330">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-330">Units included as part of the offer.</span></span> <span data-ttu-id="b44f8-331">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="b44f8-331">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b44f8-332">0</span><span class="sxs-lookup"><span data-stu-id="b44f8-332">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b44f8-333">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b44f8-333">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b44f8-334">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-334">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b44f8-335">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="b44f8-335">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b44f8-336">11</span><span class="sxs-lookup"><span data-stu-id="b44f8-336">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-337">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b44f8-337">ListPrice</span></span></td>
<td><p><span data-ttu-id="b44f8-338">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-338">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b44f8-339">$0.0808</span><span class="sxs-lookup"><span data-stu-id="b44f8-339">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-340">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b44f8-340">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b44f8-341">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="b44f8-341">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b44f8-342">$0.085</span><span class="sxs-lookup"><span data-stu-id="b44f8-342">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-343">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b44f8-343">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b44f8-344">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="b44f8-344">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b44f8-345">$0.08</span><span class="sxs-lookup"><span data-stu-id="b44f8-345">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-346">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b44f8-346">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b44f8-347">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="b44f8-347">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b44f8-348">$0.93</span><span class="sxs-lookup"><span data-stu-id="b44f8-348">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-349">Currency</span><span class="sxs-lookup"><span data-stu-id="b44f8-349">Currency</span></span></td>
<td><p><span data-ttu-id="b44f8-350">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-350">Currency type.</span></span> <span data-ttu-id="b44f8-351">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-351">Each billing entity has only one currency.</span></span> <span data-ttu-id="b44f8-352">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-352">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b44f8-353">EUR</span><span class="sxs-lookup"><span data-stu-id="b44f8-353">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-354">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b44f8-354">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b44f8-355">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-355">Pretax price per unit.</span></span> <span data-ttu-id="b44f8-356">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="b44f8-356">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b44f8-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="b44f8-357">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-358">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b44f8-358">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b44f8-359">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-359">Post tax price per unit.</span></span> <span data-ttu-id="b44f8-360">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="b44f8-360">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b44f8-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="b44f8-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-362">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b44f8-362">ChargeType</span></span></td>
<td><p><span data-ttu-id="b44f8-363">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="b44f8-363">The type of charge or adjustment.</span></span> <span data-ttu-id="b44f8-364">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b44f8-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b44f8-365">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="b44f8-365">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-366">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b44f8-366">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b44f8-367">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="b44f8-367">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b44f8-368">1280018095</span><span class="sxs-lookup"><span data-stu-id="b44f8-368">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-369">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-369">UsageDate</span></span></td>
<td><p><span data-ttu-id="b44f8-370">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="b44f8-370">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b44f8-371">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b44f8-371">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-372">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b44f8-372">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b44f8-373">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="b44f8-373">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b44f8-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="b44f8-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-375">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b44f8-375">MeteredService</span></span></td>
<td><p><span data-ttu-id="b44f8-376">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b44f8-376">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b44f8-377">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b44f8-377">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b44f8-378">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="b44f8-378">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b44f8-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="b44f8-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-380">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b44f8-380">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b44f8-381">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="b44f8-381">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b44f8-382">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="b44f8-382">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-383">Project</span><span class="sxs-lookup"><span data-stu-id="b44f8-383">Project</span></span></td>
<td><p><span data-ttu-id="b44f8-384">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="b44f8-384">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b44f8-385">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b44f8-385">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-386">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b44f8-386">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b44f8-387">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="b44f8-387">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b44f8-388">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="b44f8-388">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b44f8-389">Se hai un pacchetto da 25 connessioni ServiceBus e ne hai utilizzata 1 per quel giorno, l'uso giornaliero registrato sarà "25 Connections / 30 Days – Used: 1.000000".</span><span class="sxs-lookup"><span data-stu-id="b44f8-389">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-390">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b44f8-390">CustomerID</span></span></td>
<td><p><span data-ttu-id="b44f8-391">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-391">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b44f8-392">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b44f8-392">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b44f8-393">DomainName</span><span class="sxs-lookup"><span data-stu-id="b44f8-393">DomainName</span></span></td>
<td><p><span data-ttu-id="b44f8-394">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-394">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b44f8-395">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-395">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b44f8-396">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b44f8-396">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b44f8-397">Unità</span><span class="sxs-lookup"><span data-stu-id="b44f8-397">Unit</span></span></td>
<td><p><span data-ttu-id="b44f8-398">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="b44f8-398">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b44f8-399">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="b44f8-399">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="b44f8-400">Campi dei file acquisto una tantum</span><span class="sxs-lookup"><span data-stu-id="b44f8-400">One-time purchase file fields</span></span>

|**<span data-ttu-id="b44f8-401">Campo</span><span class="sxs-lookup"><span data-stu-id="b44f8-401">Field</span></span>** |**<span data-ttu-id="b44f8-402">Definizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-402">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="b44f8-403">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b44f8-403">PartnerId</span></span> |<span data-ttu-id="b44f8-404">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b44f8-404">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="b44f8-405">CustomerId</span><span class="sxs-lookup"><span data-stu-id="b44f8-405">CustomerId</span></span> |<span data-ttu-id="b44f8-406">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-406">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="b44f8-407">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b44f8-407">CustomerName</span></span> |<span data-ttu-id="b44f8-408">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-408">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b44f8-409">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="b44f8-409">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="b44f8-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b44f8-410">CustomerDomainName</span></span> |<span data-ttu-id="b44f8-411">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-411">The customer’s domain name.</span></span> |
|<span data-ttu-id="b44f8-412">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="b44f8-412">CustomerCountry</span></span> |<span data-ttu-id="b44f8-413">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="b44f8-413">The country in which the customer is located.</span></span> |
|<span data-ttu-id="b44f8-414">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b44f8-414">InvoiceNumber</span></span> |<span data-ttu-id="b44f8-415">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="b44f8-415">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="b44f8-416">MpnId</span><span class="sxs-lookup"><span data-stu-id="b44f8-416">MpnId</span></span> |<span data-ttu-id="b44f8-417">ID MPN del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="b44f8-417">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="b44f8-418">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="b44f8-418">Reseller MPN ID</span></span> |<span data-ttu-id="b44f8-419">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-419">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="b44f8-420">ID MPN del rivenditore nel record per la prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-420">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="b44f8-421">Corrisponde all'ID rivenditore elencato per la prenotazione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-421">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="b44f8-422">Se un partner CSP ha venduto la prenotazione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="b44f8-422">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="b44f8-423">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="b44f8-423">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="b44f8-424">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="b44f8-424">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="b44f8-425">OrderId</span><span class="sxs-lookup"><span data-stu-id="b44f8-425">OrderId</span></span> |<span data-ttu-id="b44f8-426">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f8-426">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b44f8-427">Può essere utile per identificare la prenotazione di Azure quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-427">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="b44f8-428">OrderDate</span><span class="sxs-lookup"><span data-stu-id="b44f8-428">OrderDate</span></span> |<span data-ttu-id="b44f8-429">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="b44f8-429">The date the order was placed.</span></span> |
|<span data-ttu-id="b44f8-430">ProductId</span><span class="sxs-lookup"><span data-stu-id="b44f8-430">ProductId</span></span> |<span data-ttu-id="b44f8-431">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-431">The ID for the product.</span></span> |
|<span data-ttu-id="b44f8-432">SkuId</span><span class="sxs-lookup"><span data-stu-id="b44f8-432">SkuId</span></span>  |<span data-ttu-id="b44f8-433">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="b44f8-433">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="b44f8-434">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b44f8-434">AvailabilityId</span></span> |<span data-ttu-id="b44f8-435">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="b44f8-435">The ID for a particular Availability.</span></span> <span data-ttu-id="b44f8-436">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="b44f8-436">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="b44f8-437">SkuName</span><span class="sxs-lookup"><span data-stu-id="b44f8-437">SkuName</span></span>  |<span data-ttu-id="b44f8-438">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="b44f8-438">The title for a particular SKU.</span></span> |
|<span data-ttu-id="b44f8-439">ProductName</span><span class="sxs-lookup"><span data-stu-id="b44f8-439">ProductName</span></span> |<span data-ttu-id="b44f8-440">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-440">The name of the product.</span></span> |
|<span data-ttu-id="b44f8-441">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b44f8-441">ChargeType</span></span> |<span data-ttu-id="b44f8-442">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="b44f8-442">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="b44f8-443">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b44f8-443">UnitPrice</span></span> |<span data-ttu-id="b44f8-444">Prezzo per prodotto ordinato.</span><span class="sxs-lookup"><span data-stu-id="b44f8-444">Price per product ordered.</span></span> |
|<span data-ttu-id="b44f8-445">Quantity</span><span class="sxs-lookup"><span data-stu-id="b44f8-445">Quantity</span></span> |<span data-ttu-id="b44f8-446">Numero di prodotti ordinati.</span><span class="sxs-lookup"><span data-stu-id="b44f8-446">Number of products ordered.</span></span> |
|<span data-ttu-id="b44f8-447">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b44f8-447">Subtotal</span></span> |<span data-ttu-id="b44f8-448">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-448">Total before tax.</span></span> <span data-ttu-id="b44f8-449">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-449">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="b44f8-450">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="b44f8-450">TaxTotal</span></span> |<span data-ttu-id="b44f8-451">Totale di tutte le imposte applicabili.</span><span class="sxs-lookup"><span data-stu-id="b44f8-451">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="b44f8-452">Total</span><span class="sxs-lookup"><span data-stu-id="b44f8-452">Total</span></span> |<span data-ttu-id="b44f8-453">Importo totale di questo acquisto.</span><span class="sxs-lookup"><span data-stu-id="b44f8-453">The total amount of this purchase.</span></span> |
|<span data-ttu-id="b44f8-454">Currency</span><span class="sxs-lookup"><span data-stu-id="b44f8-454">Currency</span></span> |<span data-ttu-id="b44f8-455">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-455">Currency type.</span></span> <span data-ttu-id="b44f8-456">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="b44f8-456">Each billing entity has only one currency.</span></span> <span data-ttu-id="b44f8-457">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-457">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="b44f8-458">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="b44f8-458">DiscountDetails</span></span> |<span data-ttu-id="b44f8-459">Elenco dettagliato di eventuali sconti pertinenti.</span><span class="sxs-lookup"><span data-stu-id="b44f8-459">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="b44f8-460">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-460">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b44f8-461">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="b44f8-461">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b44f8-462">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-462">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b44f8-463">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="b44f8-463">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b44f8-464">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-464">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b44f8-465">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="b44f8-465">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="b44f8-466">Descrizione dell'addebito in fattura</span><span class="sxs-lookup"><span data-stu-id="b44f8-466">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b44f8-467">Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="b44f8-467">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b44f8-468">Descrizione dell'addebito</span><span class="sxs-lookup"><span data-stu-id="b44f8-468">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b44f8-469">Modalità di mapping di questi tipi di addebito alla fattura</span><span class="sxs-lookup"><span data-stu-id="b44f8-469">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="b44f8-470">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="b44f8-470">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b44f8-471">Commessione di attivazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-471">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-472">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="b44f8-472">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b44f8-473">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-473">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-474">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="b44f8-474">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-475">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="b44f8-475">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-476">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="b44f8-476">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-477">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-477">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-478">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="b44f8-478">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-479">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="b44f8-479">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-480">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="b44f8-480">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-481">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="b44f8-481">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-482">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="b44f8-482">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-483">Tariffe rateizzate all'acquisto</span><span class="sxs-lookup"><span data-stu-id="b44f8-483">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-484">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="b44f8-484">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-485">Addebito iniziale per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-485">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-486">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="b44f8-486">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-487">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-487">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b44f8-488">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="b44f8-488">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-489">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-489">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-490">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-491">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="b44f8-492">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="b44f8-492">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b44f8-493">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="b44f8-493">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-494">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="b44f8-494">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b44f8-495">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-495">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-496">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="b44f8-496">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-497">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="b44f8-497">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b44f8-498">Crediti</span><span class="sxs-lookup"><span data-stu-id="b44f8-498">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b44f8-499">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="b44f8-499">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-500">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="b44f8-500">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-501">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-501">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b44f8-502">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-502">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="b44f8-503">Sconti basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="b44f8-503">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b44f8-504">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="b44f8-504">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-505">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-505">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b44f8-506">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-506">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-507">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="b44f8-507">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-508">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="b44f8-508">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-509">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="b44f8-509">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-510">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="b44f8-510">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-511">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="b44f8-511">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-512">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="b44f8-512">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="b44f8-513">Basato su licenza sconti</span><span class="sxs-lookup"><span data-stu-id="b44f8-513">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="b44f8-514">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="b44f8-514">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b44f8-515">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-515">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b44f8-516"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-516"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="b44f8-517">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="b44f8-517">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="b44f8-518">Eccezione: "Compensa una voce" include già le imposte.</span><span class="sxs-lookup"><span data-stu-id="b44f8-518">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="b44f8-519">Vedi crediti, sopra.</span><span class="sxs-lookup"><span data-stu-id="b44f8-519">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="b44f8-520">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="b44f8-520">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b44f8-521">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-521">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b44f8-522">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="b44f8-522">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
