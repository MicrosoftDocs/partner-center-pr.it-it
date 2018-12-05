---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Per una visualizzazione di voci delle relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 188f6fe28277cfab624d407bb47157f2dce7e854
ms.sourcegitcommit: d3613d23bd177a53381ebf32b4f1075201f8f7f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/05/2018
ms.locfileid: "8683820"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ba5c9-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-103">Use the reconciliation files</span></span>

**<span data-ttu-id="ba5c9-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="ba5c9-104">Applies to</span></span>**

-  <span data-ttu-id="ba5c9-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ba5c9-105">Partner Center</span></span>
-  <span data-ttu-id="ba5c9-106">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="ba5c9-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ba5c9-107">Per una visualizzazione di voci delle relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="ba5c9-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="ba5c9-109">Eseguire la scomposizione dei dati in base al partner</span><span class="sxs-lookup"><span data-stu-id="ba5c9-109">Itemize by partner</span></span>


<span data-ttu-id="ba5c9-110">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ba5c9-111">ID MPN</span><span class="sxs-lookup"><span data-stu-id="ba5c9-111">MPN ID</span></span></th>
<th><span data-ttu-id="ba5c9-112">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ba5c9-113">ID MPN</span><span class="sxs-lookup"><span data-stu-id="ba5c9-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="ba5c9-114">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-115">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="ba5c9-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ba5c9-116">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ba5c9-117">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ba5c9-118">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ba5c9-119">Per visualizzare o aggiornare il rivenditore, il menu del centro per i Partner seleziona <strong>i clienti</strong>, quindi scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ba5c9-120">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ba5c9-121">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ba5c9-122">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ba5c9-123">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="ba5c9-124">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="ba5c9-125">Campi dei file in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="ba5c9-125">License-based file fields</span></span>


<span data-ttu-id="ba5c9-126">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="ba5c9-127">Colonna</span><span class="sxs-lookup"><span data-stu-id="ba5c9-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="ba5c9-128">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="ba5c9-129">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="ba5c9-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="ba5c9-131">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ba5c9-132">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ba5c9-133">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ba5c9-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ba5c9-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="ba5c9-136">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ba5c9-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ba5c9-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-138">OrderID</span></span></td>
<td><p><span data-ttu-id="ba5c9-139">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ba5c9-140">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ba5c9-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ba5c9-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ba5c9-143">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ba5c9-144">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ba5c9-145">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ba5c9-146">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ba5c9-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ba5c9-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="ba5c9-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ba5c9-149">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ba5c9-150">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ba5c9-151">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ba5c9-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ba5c9-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-153">OfferID</span></span></td>
<td><p><span data-ttu-id="ba5c9-154">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-154">Unique offer ID.</span></span> <span data-ttu-id="ba5c9-155">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ba5c9-156"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ba5c9-157">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ba5c9-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ba5c9-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ba5c9-160">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ba5c9-161"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ba5c9-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ba5c9-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-163">OfferName</span></span></td>
<td><p><span data-ttu-id="ba5c9-164">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ba5c9-165">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="ba5c9-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-167">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ba5c9-168">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ba5c9-169">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ba5c9-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ba5c9-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-172">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ba5c9-173">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ba5c9-174">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ba5c9-175">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ba5c9-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ba5c9-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-178">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ba5c9-179">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ba5c9-180">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ba5c9-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ba5c9-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-183">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="ba5c9-184">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ba5c9-185">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ba5c9-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ba5c9-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ba5c9-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="ba5c9-188">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-188">The type of charge or adjustment.</span></span> <span data-ttu-id="ba5c9-189">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ba5c9-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ba5c9-190">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ba5c9-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ba5c9-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ba5c9-192">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ba5c9-193">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ba5c9-194">6.82</span><span class="sxs-lookup"><span data-stu-id="ba5c9-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="ba5c9-195">Quantity</span></span></td>
<td><p><span data-ttu-id="ba5c9-196">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-196">Number of seats.</span></span> <span data-ttu-id="ba5c9-197">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ba5c9-198">2</span><span class="sxs-lookup"><span data-stu-id="ba5c9-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-199">Amount</span><span class="sxs-lookup"><span data-stu-id="ba5c9-199">Amount</span></span></td>
<td><p><span data-ttu-id="ba5c9-200">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-200">Total of price for quantity.</span></span> <span data-ttu-id="ba5c9-201">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ba5c9-202">13.32</span><span class="sxs-lookup"><span data-stu-id="ba5c9-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ba5c9-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ba5c9-204">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ba5c9-205">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ba5c9-206">2.32</span><span class="sxs-lookup"><span data-stu-id="ba5c9-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="ba5c9-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="ba5c9-208">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-208">Total before tax.</span></span> <span data-ttu-id="ba5c9-209">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ba5c9-210">11</span><span class="sxs-lookup"><span data-stu-id="ba5c9-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-211">Tax</span><span class="sxs-lookup"><span data-stu-id="ba5c9-211">Tax</span></span></td>
<td><p><span data-ttu-id="ba5c9-212">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ba5c9-213">0</span><span class="sxs-lookup"><span data-stu-id="ba5c9-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ba5c9-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ba5c9-215">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-215">Total after tax.</span></span> <span data-ttu-id="ba5c9-216">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ba5c9-217">11</span><span class="sxs-lookup"><span data-stu-id="ba5c9-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-218">Currency</span><span class="sxs-lookup"><span data-stu-id="ba5c9-218">Currency</span></span></td>
<td><p><span data-ttu-id="ba5c9-219">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-219">Currency type.</span></span> <span data-ttu-id="ba5c9-220">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="ba5c9-221">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ba5c9-222">EUR</span><span class="sxs-lookup"><span data-stu-id="ba5c9-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="ba5c9-224">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ba5c9-225">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ba5c9-226">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="ba5c9-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-227">MPNID</span></span></td>
<td><p><span data-ttu-id="ba5c9-228">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="ba5c9-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ba5c9-229">4390934</span><span class="sxs-lookup"><span data-stu-id="ba5c9-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ba5c9-231">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ba5c9-232">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="ba5c9-233">4390934</span><span class="sxs-lookup"><span data-stu-id="ba5c9-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-234">DomainName</span></span></td>
<td><p><span data-ttu-id="ba5c9-235">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ba5c9-236">Questo non deve essere usato per identificare in modo univoco il cliente quando il cliente/partner può aggiornare il dominio di reindirizzamento a microsito/predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ba5c9-237">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ba5c9-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ba5c9-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ba5c9-240">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-240">Subscription nickname.</span></span> <span data-ttu-id="ba5c9-241">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ba5c9-242">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="ba5c9-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ba5c9-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ba5c9-244">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ba5c9-245">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ba5c9-246">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="ba5c9-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="ba5c9-247">Campi dei file in base all'uso</span><span class="sxs-lookup"><span data-stu-id="ba5c9-247">Usage-based file fields</span></span>


<span data-ttu-id="ba5c9-248">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ba5c9-249">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="ba5c9-250">Colonna</span><span class="sxs-lookup"><span data-stu-id="ba5c9-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="ba5c9-251">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="ba5c9-252">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="ba5c9-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="ba5c9-254">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ba5c9-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ba5c9-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="ba5c9-257">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ba5c9-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ba5c9-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ba5c9-260">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ba5c9-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="ba5c9-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="ba5c9-263">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ba5c9-264">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ba5c9-265">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="ba5c9-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-266">MPNID</span></span></td>
<td><p><span data-ttu-id="ba5c9-267">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ba5c9-268">4390934</span><span class="sxs-lookup"><span data-stu-id="ba5c9-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ba5c9-270">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ba5c9-271">Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="ba5c9-272">4390934</span><span class="sxs-lookup"><span data-stu-id="ba5c9-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ba5c9-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ba5c9-274">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ba5c9-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ba5c9-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-277">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ba5c9-278">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ba5c9-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ba5c9-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-281">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ba5c9-282">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ba5c9-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ba5c9-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ba5c9-285">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ba5c9-286">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ba5c9-287">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ba5c9-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ba5c9-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ba5c9-290">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ba5c9-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ba5c9-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ba5c9-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ba5c9-293">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="ba5c9-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ba5c9-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ba5c9-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-295">OrderID</span></span></td>
<td><p><span data-ttu-id="ba5c9-296">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ba5c9-297">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ba5c9-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ba5c9-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="ba5c9-300">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ba5c9-301">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="ba5c9-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ba5c9-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="ba5c9-303">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ba5c9-304">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="ba5c9-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="ba5c9-305">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="ba5c9-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ba5c9-307">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ba5c9-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ba5c9-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-309">Resource Name</span><span class="sxs-lookup"><span data-stu-id="ba5c9-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="ba5c9-310">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ba5c9-311">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="ba5c9-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ba5c9-312">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="ba5c9-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-313">Region</span><span class="sxs-lookup"><span data-stu-id="ba5c9-313">Region</span></span></td>
<td><p><span data-ttu-id="ba5c9-314">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-314">The region the usage applies to.</span></span> <span data-ttu-id="ba5c9-315">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ba5c9-316">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="ba5c9-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-317">SKU</span><span class="sxs-lookup"><span data-stu-id="ba5c9-317">SKU</span></span></td>
<td><p><span data-ttu-id="ba5c9-318">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="ba5c9-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ba5c9-319">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ba5c9-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ba5c9-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ba5c9-321">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ba5c9-322">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ba5c9-323">1</span><span class="sxs-lookup"><span data-stu-id="ba5c9-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ba5c9-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ba5c9-325">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ba5c9-326">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ba5c9-327">11</span><span class="sxs-lookup"><span data-stu-id="ba5c9-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ba5c9-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ba5c9-329">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-329">Units included as part of the offer.</span></span> <span data-ttu-id="ba5c9-330">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ba5c9-331">0</span><span class="sxs-lookup"><span data-stu-id="ba5c9-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ba5c9-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ba5c9-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ba5c9-333">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ba5c9-334">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ba5c9-335">11</span><span class="sxs-lookup"><span data-stu-id="ba5c9-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ba5c9-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="ba5c9-337">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ba5c9-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="ba5c9-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ba5c9-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ba5c9-340">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ba5c9-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="ba5c9-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ba5c9-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ba5c9-343">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ba5c9-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="ba5c9-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ba5c9-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ba5c9-346">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ba5c9-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="ba5c9-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-348">Currency</span><span class="sxs-lookup"><span data-stu-id="ba5c9-348">Currency</span></span></td>
<td><p><span data-ttu-id="ba5c9-349">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-349">Currency type.</span></span> <span data-ttu-id="ba5c9-350">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="ba5c9-351">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ba5c9-352">EUR</span><span class="sxs-lookup"><span data-stu-id="ba5c9-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ba5c9-354">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-354">Pretax price per unit.</span></span> <span data-ttu-id="ba5c9-355">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ba5c9-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="ba5c9-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ba5c9-358">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-358">Post tax price per unit.</span></span> <span data-ttu-id="ba5c9-359">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ba5c9-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="ba5c9-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ba5c9-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="ba5c9-362">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-362">The type of charge or adjustment.</span></span> <span data-ttu-id="ba5c9-363">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ba5c9-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ba5c9-364">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ba5c9-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ba5c9-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ba5c9-366">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ba5c9-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="ba5c9-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="ba5c9-369">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ba5c9-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ba5c9-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ba5c9-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ba5c9-372">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ba5c9-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="ba5c9-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="ba5c9-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="ba5c9-375">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ba5c9-376">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ba5c9-377">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ba5c9-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="ba5c9-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ba5c9-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ba5c9-380">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ba5c9-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="ba5c9-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-382">Project</span><span class="sxs-lookup"><span data-stu-id="ba5c9-382">Project</span></span></td>
<td><p><span data-ttu-id="ba5c9-383">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="ba5c9-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ba5c9-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ba5c9-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ba5c9-386">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ba5c9-387">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="ba5c9-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="ba5c9-388">Se hai un pacchetto da 25 connessioni ServiceBus e ne hai utilizzata 1 per quel giorno, l'uso giornaliero registrato sarà "25 Connections / 30 Days – Used: 1.000000".</span><span class="sxs-lookup"><span data-stu-id="ba5c9-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ba5c9-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="ba5c9-390">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ba5c9-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ba5c9-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ba5c9-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-392">DomainName</span></span></td>
<td><p><span data-ttu-id="ba5c9-393">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ba5c9-394">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ba5c9-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ba5c9-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ba5c9-396">Unità</span><span class="sxs-lookup"><span data-stu-id="ba5c9-396">Unit</span></span></td>
<td><p><span data-ttu-id="ba5c9-397">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="ba5c9-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ba5c9-398">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="ba5c9-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="ba5c9-399">Campi dei file acquisto una tantum</span><span class="sxs-lookup"><span data-stu-id="ba5c9-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="ba5c9-400">Campo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-400">Field</span></span>** |**<span data-ttu-id="ba5c9-401">Definizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="ba5c9-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-402">PartnerId</span></span> |<span data-ttu-id="ba5c9-403">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="ba5c9-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-404">CustomerId</span></span> |<span data-ttu-id="ba5c9-405">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="ba5c9-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-406">CustomerName</span></span> |<span data-ttu-id="ba5c9-407">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ba5c9-408">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="ba5c9-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-409">CustomerDomainName</span></span> |<span data-ttu-id="ba5c9-410">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="ba5c9-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="ba5c9-411">CustomerCountry</span></span> |<span data-ttu-id="ba5c9-412">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="ba5c9-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ba5c9-413">InvoiceNumber</span></span> |<span data-ttu-id="ba5c9-414">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="ba5c9-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-415">MpnId</span></span> |<span data-ttu-id="ba5c9-416">ID MPN del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="ba5c9-417">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="ba5c9-417">Reseller MPN ID</span></span> |<span data-ttu-id="ba5c9-418">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="ba5c9-419">ID MPN del rivenditore nel record per la prenotazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="ba5c9-420">Corrisponde all'ID rivenditore elencato per la prenotazione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="ba5c9-421">Se un partner CSP ha venduto la prenotazione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="ba5c9-422">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="ba5c9-423">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="ba5c9-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-424">OrderId</span></span> |<span data-ttu-id="ba5c9-425">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ba5c9-426">Può essere utile per identificare la prenotazione di Azure quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="ba5c9-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-427">OrderDate</span></span> |<span data-ttu-id="ba5c9-428">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-428">The date the order was placed.</span></span> |
|<span data-ttu-id="ba5c9-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-429">ProductId</span></span> |<span data-ttu-id="ba5c9-430">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-430">The ID for the product.</span></span> |
|<span data-ttu-id="ba5c9-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-431">SkuId</span></span>  |<span data-ttu-id="ba5c9-432">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="ba5c9-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ba5c9-433">AvailabilityId</span></span> |<span data-ttu-id="ba5c9-434">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-434">The ID for a particular Availability.</span></span> <span data-ttu-id="ba5c9-435">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="ba5c9-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-436">SkuName</span></span>  |<span data-ttu-id="ba5c9-437">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="ba5c9-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="ba5c9-438">ProductName</span></span> |<span data-ttu-id="ba5c9-439">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-439">The name of the product.</span></span> |
|<span data-ttu-id="ba5c9-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ba5c9-440">ChargeType</span></span> |<span data-ttu-id="ba5c9-441">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="ba5c9-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ba5c9-442">UnitPrice</span></span> |<span data-ttu-id="ba5c9-443">Prezzo per prodotto ordinato.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-443">Price per product ordered.</span></span> |
|<span data-ttu-id="ba5c9-444">Quantity</span><span class="sxs-lookup"><span data-stu-id="ba5c9-444">Quantity</span></span> |<span data-ttu-id="ba5c9-445">Numero di prodotti ordinati.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-445">Number of products ordered.</span></span> |
|<span data-ttu-id="ba5c9-446">Subtotal</span><span class="sxs-lookup"><span data-stu-id="ba5c9-446">Subtotal</span></span> |<span data-ttu-id="ba5c9-447">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-447">Total before tax.</span></span> <span data-ttu-id="ba5c9-448">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="ba5c9-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="ba5c9-449">TaxTotal</span></span> |<span data-ttu-id="ba5c9-450">Totale di tutte le imposte applicabili.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="ba5c9-451">Total</span><span class="sxs-lookup"><span data-stu-id="ba5c9-451">Total</span></span> |<span data-ttu-id="ba5c9-452">Importo totale di questo acquisto.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="ba5c9-453">Currency</span><span class="sxs-lookup"><span data-stu-id="ba5c9-453">Currency</span></span> |<span data-ttu-id="ba5c9-454">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-454">Currency type.</span></span> <span data-ttu-id="ba5c9-455">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="ba5c9-456">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="ba5c9-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="ba5c9-457">DiscountDetails</span></span> |<span data-ttu-id="ba5c9-458">Elenco dettagliato di eventuali sconti pertinenti.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="ba5c9-459">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ba5c9-460">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ba5c9-461">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ba5c9-462">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="ba5c9-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="ba5c9-463">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="ba5c9-464">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="ba5c9-465">Descrizione dell'addebito in fattura</span><span class="sxs-lookup"><span data-stu-id="ba5c9-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ba5c9-466">Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="ba5c9-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ba5c9-467">Descrizione dell'addebito</span><span class="sxs-lookup"><span data-stu-id="ba5c9-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="ba5c9-468">Modalità di mapping di questi tipi di addebito alla fattura</span><span class="sxs-lookup"><span data-stu-id="ba5c9-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="ba5c9-469">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="ba5c9-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-470">Commessione di attivazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-471">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="ba5c9-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="ba5c9-472">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-473">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="ba5c9-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-474">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-475">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="ba5c9-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-476">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-477">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="ba5c9-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-478">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="ba5c9-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-479">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="ba5c9-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-480">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="ba5c9-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-481">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="ba5c9-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-482">Tariffe rateizzate all'acquisto</span><span class="sxs-lookup"><span data-stu-id="ba5c9-482">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-483">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="ba5c9-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-484">Addebito iniziale per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-484">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-485">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-486">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="ba5c9-487">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-488">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-489">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-490">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="ba5c9-491">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-492">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="ba5c9-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-493">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="ba5c9-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ba5c9-494">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-495">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="ba5c9-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-496">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="ba5c9-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="ba5c9-497">Crediti</span><span class="sxs-lookup"><span data-stu-id="ba5c9-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-498">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="ba5c9-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-499">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="ba5c9-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-500">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ba5c9-501">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="ba5c9-502">Sconti basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-503">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-504">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="ba5c9-505">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-506">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-507">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="ba5c9-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-508">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="ba5c9-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-509">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ba5c9-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-510">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="ba5c9-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-511">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="ba5c9-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="ba5c9-512">Basato su licenza sconti</span><span class="sxs-lookup"><span data-stu-id="ba5c9-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="ba5c9-513">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="ba5c9-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-514">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ba5c9-515"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="ba5c9-516">Possono essere applicate a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="ba5c9-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="ba5c9-517">Eccezione: "Compensa una voce" include già le imposte.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="ba5c9-518">Vedi crediti, sopra.</span><span class="sxs-lookup"><span data-stu-id="ba5c9-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-519">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="ba5c9-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ba5c9-520">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ba5c9-521">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="ba5c9-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
