---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430200"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="98c96-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="98c96-103">Use the reconciliation files</span></span>

**<span data-ttu-id="98c96-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="98c96-104">Applies to</span></span>**

-  <span data-ttu-id="98c96-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="98c96-105">Partner Center</span></span>
-  <span data-ttu-id="98c96-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="98c96-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="98c96-107">Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="98c96-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="98c96-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="98c96-109">Problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="98c96-109">Formatting issues</span></span>

<span data-ttu-id="98c96-110">In alcuni casi il file di riconoscimento potrà avere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="98c96-111">(Questa situazione può verificarsi, ad esempio, se non viene utilizzata le impostazioni locali EN-US.) Attenersi alla procedura seguente per risolvere questi problemi.</span><span class="sxs-lookup"><span data-stu-id="98c96-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="98c96-112">Aprire il file con estensione csv in Excel e selezionare la prima colonna.</span><span class="sxs-lookup"><span data-stu-id="98c96-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="98c96-113">Sulla barra multifunzione, selezionare <strong>dati</strong>, quindi selezionare <strong>testo alle colonne</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="98c96-114">La conversione guidata testo in colonne, selezionare <strong>tipo di file delimitati</strong>e quindi selezionare <strong>successivo</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="98c96-115">Nel campo Delimeters, selezionare <strong>virgole</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="98c96-116">Se <strong>scheda</strong> è già selezionata, è possibile lasciarla.</span><span class="sxs-lookup"><span data-stu-id="98c96-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="98c96-117">Selezionare <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="98c96-118">Nel campo formato dei dati di colonna, selezionare <strong>data: MDY</strong>, quindi selezionare <strong>successivo</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="98c96-119">Nel campo formato dei dati di colonna, selezionare <strong>testo</strong> per tutte le colonne e quindi selezionare l'importo <strong>fine</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="98c96-120">Specificare i dettagli da partner</span><span class="sxs-lookup"><span data-stu-id="98c96-120">Itemize by partner</span></span>


<span data-ttu-id="98c96-121">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="98c96-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="98c96-122">ID MPN</span><span class="sxs-lookup"><span data-stu-id="98c96-122">MPN ID</span></span></th>
<th><span data-ttu-id="98c96-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="98c96-124">ID MPN</span><span class="sxs-lookup"><span data-stu-id="98c96-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="98c96-125">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="98c96-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-126">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="98c96-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="98c96-127">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="98c96-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="98c96-128">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="98c96-129">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="98c96-130">eTo visualizzare o aggiornare il rivenditore, dal menu Centro per i Partner, selezionare <strong>clienti</strong>, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="98c96-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="98c96-131">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="98c96-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="98c96-132">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="98c96-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="98c96-133">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="98c96-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="98c96-134">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="98c96-135">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="98c96-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="98c96-136">Campi del file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="98c96-136">License-based file fields</span></span>


<span data-ttu-id="98c96-137">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="98c96-138">Column</span><span class="sxs-lookup"><span data-stu-id="98c96-138">Column</span></span></strong></td>
<td><strong><span data-ttu-id="98c96-139">Descrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-139">Description</span></span></strong></td>
<td><strong><span data-ttu-id="98c96-140">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="98c96-140">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="98c96-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="98c96-142">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="98c96-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="98c96-143">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="98c96-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="98c96-144">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="98c96-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="98c96-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="98c96-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="98c96-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="98c96-147">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="98c96-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="98c96-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="98c96-149">OrderID</span></span></td>
<td><p><span data-ttu-id="98c96-150">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="98c96-151">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="98c96-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="98c96-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="98c96-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="98c96-154">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="98c96-155">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="98c96-156">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="98c96-157">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="98c96-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="98c96-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="98c96-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="98c96-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="98c96-160">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="98c96-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="98c96-161">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="98c96-162">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="98c96-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="98c96-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="98c96-164">OfferID</span></span></td>
<td><p><span data-ttu-id="98c96-165">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="98c96-165">Unique offer ID.</span></span> <span data-ttu-id="98c96-166">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="98c96-167"><b>Nota</b>: Questo valore non corrisponde ID offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="98c96-168">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="98c96-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="98c96-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="98c96-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="98c96-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="98c96-171">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="98c96-172"><b>Nota</b>: Questo valore corrisponde all'ID dell'offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="98c96-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="98c96-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="98c96-174">OfferName</span></span></td>
<td><p><span data-ttu-id="98c96-175">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="98c96-176">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="98c96-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="98c96-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="98c96-178">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="98c96-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="98c96-179">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="98c96-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="98c96-180">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="98c96-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="98c96-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="98c96-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="98c96-183">La data di fine sottoscrizione: 12 mesi + x giorni dopo la data di inizio (in modo da allinearsi partner data di fatturazione) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="98c96-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="98c96-184">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="98c96-185">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="98c96-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="98c96-186">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="98c96-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="98c96-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="98c96-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="98c96-189">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="98c96-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="98c96-190">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="98c96-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="98c96-191">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="98c96-192">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="98c96-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="98c96-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="98c96-194">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="98c96-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="98c96-195">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="98c96-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="98c96-196">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="98c96-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="98c96-197">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="98c96-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="98c96-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="98c96-199">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="98c96-199">The type of charge or adjustment.</span></span> <span data-ttu-id="98c96-200">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="98c96-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="98c96-201">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="98c96-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="98c96-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="98c96-203">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="98c96-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="98c96-204">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="98c96-205">6.82</span><span class="sxs-lookup"><span data-stu-id="98c96-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-206">Quantità</span><span class="sxs-lookup"><span data-stu-id="98c96-206">Quantity</span></span></td>
<td><p><span data-ttu-id="98c96-207">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="98c96-207">Number of seats.</span></span> <span data-ttu-id="98c96-208">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="98c96-209">2</span><span class="sxs-lookup"><span data-stu-id="98c96-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-210">Importo</span><span class="sxs-lookup"><span data-stu-id="98c96-210">Amount</span></span></td>
<td><p><span data-ttu-id="98c96-211">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="98c96-211">Total of price for quantity.</span></span> <span data-ttu-id="98c96-212">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="98c96-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="98c96-213">13.32</span><span class="sxs-lookup"><span data-stu-id="98c96-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="98c96-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="98c96-215">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="98c96-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="98c96-216">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="98c96-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="98c96-217">2.32</span><span class="sxs-lookup"><span data-stu-id="98c96-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="98c96-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="98c96-219">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-219">Total before tax.</span></span> <span data-ttu-id="98c96-220">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="98c96-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="98c96-221">11</span><span class="sxs-lookup"><span data-stu-id="98c96-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-222">Imposta</span><span class="sxs-lookup"><span data-stu-id="98c96-222">Tax</span></span></td>
<td><p><span data-ttu-id="98c96-223">Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="98c96-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="98c96-224">0</span><span class="sxs-lookup"><span data-stu-id="98c96-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="98c96-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="98c96-226">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-226">Total after tax.</span></span> <span data-ttu-id="98c96-227">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="98c96-228">11</span><span class="sxs-lookup"><span data-stu-id="98c96-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-229">Valuta</span><span class="sxs-lookup"><span data-stu-id="98c96-229">Currency</span></span></td>
<td><p><span data-ttu-id="98c96-230">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-230">Currency type.</span></span> <span data-ttu-id="98c96-231">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="98c96-232">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="98c96-233">EUR</span><span class="sxs-lookup"><span data-stu-id="98c96-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="98c96-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="98c96-235">Cliente&#39;nome organizzazione s come riportato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="98c96-236">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="98c96-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="98c96-237">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="98c96-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-238">MPNID</span></span></td>
<td><p><span data-ttu-id="98c96-239">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="98c96-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="98c96-240">4390934</span><span class="sxs-lookup"><span data-stu-id="98c96-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="98c96-242">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="98c96-243">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="98c96-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="98c96-244">4390934</span><span class="sxs-lookup"><span data-stu-id="98c96-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="98c96-245">DomainName</span></span></td>
<td><p><span data-ttu-id="98c96-246">Cliente&#39;nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="98c96-247">Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="98c96-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="98c96-248">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="98c96-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="98c96-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="98c96-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="98c96-251">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-251">Subscription nickname.</span></span> <span data-ttu-id="98c96-252">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="98c96-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="98c96-253">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="98c96-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="98c96-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="98c96-255">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="98c96-256">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="98c96-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="98c96-257">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="98c96-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="98c96-258">Campi del file basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="98c96-258">Usage-based file fields</span></span>


<span data-ttu-id="98c96-259">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="98c96-260">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="98c96-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="98c96-261">Column</span><span class="sxs-lookup"><span data-stu-id="98c96-261">Column</span></span></strong></td>
<td><strong><span data-ttu-id="98c96-262">Descrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-262">Description</span></span></strong></td>
<td><strong><span data-ttu-id="98c96-263">Valore di esempio</span><span class="sxs-lookup"><span data-stu-id="98c96-263">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="98c96-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="98c96-265">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="98c96-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="98c96-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="98c96-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="98c96-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="98c96-268">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="98c96-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="98c96-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="98c96-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="98c96-271">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="98c96-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="98c96-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="98c96-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="98c96-274">Cliente&#39;nome organizzazione s come riportato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="98c96-275">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="98c96-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="98c96-276">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="98c96-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-277">MPNID</span></span></td>
<td><p><span data-ttu-id="98c96-278">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="98c96-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="98c96-279">4390934</span><span class="sxs-lookup"><span data-stu-id="98c96-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="98c96-281">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="98c96-282">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="98c96-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="98c96-283">4390934</span><span class="sxs-lookup"><span data-stu-id="98c96-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="98c96-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="98c96-285">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="98c96-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="98c96-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="98c96-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="98c96-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="98c96-288">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="98c96-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="98c96-289">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="98c96-290">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="98c96-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="98c96-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="98c96-292">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="98c96-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="98c96-293">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="98c96-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="98c96-294">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="98c96-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="98c96-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="98c96-296">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="98c96-297">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="98c96-298">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="98c96-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="98c96-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="98c96-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="98c96-301">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="98c96-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="98c96-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="98c96-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="98c96-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="98c96-304">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="98c96-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="98c96-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="98c96-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="98c96-306">OrderID</span></span></td>
<td><p><span data-ttu-id="98c96-307">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="98c96-308">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="98c96-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="98c96-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="98c96-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="98c96-311">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="98c96-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="98c96-312">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="98c96-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="98c96-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="98c96-314">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="98c96-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="98c96-315">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="98c96-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="98c96-316">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="98c96-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="98c96-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="98c96-318">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="98c96-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="98c96-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="98c96-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-320">Resource Name</span><span class="sxs-lookup"><span data-stu-id="98c96-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="98c96-321">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="98c96-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="98c96-322">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="98c96-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="98c96-323">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="98c96-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-324">Region</span><span class="sxs-lookup"><span data-stu-id="98c96-324">Region</span></span></td>
<td><p><span data-ttu-id="98c96-325">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="98c96-325">The region the usage applies to.</span></span> <span data-ttu-id="98c96-326">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="98c96-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="98c96-327">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="98c96-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-328">SKU</span><span class="sxs-lookup"><span data-stu-id="98c96-328">SKU</span></span></td>
<td><p><span data-ttu-id="98c96-329">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="98c96-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="98c96-330">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="98c96-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="98c96-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="98c96-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="98c96-332">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="98c96-333">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="98c96-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="98c96-334">1</span><span class="sxs-lookup"><span data-stu-id="98c96-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="98c96-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="98c96-336">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="98c96-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="98c96-337">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="98c96-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="98c96-338">11</span><span class="sxs-lookup"><span data-stu-id="98c96-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="98c96-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="98c96-340">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="98c96-340">Units included as part of the offer.</span></span> <span data-ttu-id="98c96-341">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="98c96-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="98c96-342">0</span><span class="sxs-lookup"><span data-stu-id="98c96-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="98c96-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="98c96-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="98c96-344">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="98c96-345">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="98c96-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="98c96-346">11</span><span class="sxs-lookup"><span data-stu-id="98c96-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="98c96-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="98c96-348">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="98c96-349">$0.0808</span><span class="sxs-lookup"><span data-stu-id="98c96-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="98c96-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="98c96-351">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="98c96-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="98c96-352">$0.085</span><span class="sxs-lookup"><span data-stu-id="98c96-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="98c96-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="98c96-354">Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="98c96-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="98c96-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="98c96-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="98c96-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="98c96-357">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="98c96-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="98c96-358">$0.93</span><span class="sxs-lookup"><span data-stu-id="98c96-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-359">Valuta</span><span class="sxs-lookup"><span data-stu-id="98c96-359">Currency</span></span></td>
<td><p><span data-ttu-id="98c96-360">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-360">Currency type.</span></span> <span data-ttu-id="98c96-361">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="98c96-362">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="98c96-363">EUR</span><span class="sxs-lookup"><span data-stu-id="98c96-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="98c96-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="98c96-365">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-365">Pretax price per unit.</span></span> <span data-ttu-id="98c96-366">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="98c96-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="98c96-367">$0.08</span><span class="sxs-lookup"><span data-stu-id="98c96-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="98c96-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="98c96-369">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-369">Post tax price per unit.</span></span> <span data-ttu-id="98c96-370">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="98c96-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="98c96-371">$0.08</span><span class="sxs-lookup"><span data-stu-id="98c96-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="98c96-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="98c96-373">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="98c96-373">The type of charge or adjustment.</span></span> <span data-ttu-id="98c96-374">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="98c96-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="98c96-375">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="98c96-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="98c96-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="98c96-377">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="98c96-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="98c96-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="98c96-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="98c96-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="98c96-380">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="98c96-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="98c96-381">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="98c96-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="98c96-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="98c96-383">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="98c96-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="98c96-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="98c96-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="98c96-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="98c96-386">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="98c96-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="98c96-387">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="98c96-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="98c96-388">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="98c96-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="98c96-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="98c96-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="98c96-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="98c96-391">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="98c96-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="98c96-392">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="98c96-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-393">Project</span><span class="sxs-lookup"><span data-stu-id="98c96-393">Project</span></span></td>
<td><p><span data-ttu-id="98c96-394">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="98c96-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="98c96-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="98c96-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="98c96-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="98c96-397">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="98c96-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="98c96-398">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="98c96-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="98c96-399">Se disponi di un pacchetto 25 di connessioni del bus di servizio eseguito il provisioning e si fosse utilizzato 1 durante il giorno, l'istruzione di utilizzo giornaliero per quel giorno indicherebbe "25 connessioni / 30 giorni: utilizzato: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="98c96-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="98c96-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="98c96-401">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="98c96-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="98c96-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="98c96-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="98c96-403">DomainName</span></span></td>
<td><p><span data-ttu-id="98c96-404">Cliente&#39;nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="98c96-405">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="98c96-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="98c96-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="98c96-407">Unità</span><span class="sxs-lookup"><span data-stu-id="98c96-407">Unit</span></span></td>
<td><p><span data-ttu-id="98c96-408">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="98c96-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="98c96-409">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="98c96-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="98c96-410">Campi del file sia monouso che ricorrenti</span><span class="sxs-lookup"><span data-stu-id="98c96-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="98c96-411">Column</span><span class="sxs-lookup"><span data-stu-id="98c96-411">Column</span></span></th>
<th><span data-ttu-id="98c96-412">Descrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="98c96-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="98c96-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="98c96-414">Identificatore univoco tenant di Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="98c96-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="98c96-415">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="98c96-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="98c96-416">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="98c96-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-417">Id cliente</span><span class="sxs-lookup"><span data-stu-id="98c96-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="98c96-418">Microsoft Azure Active Directory tenant ID univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-419">Nome cliente</span><span class="sxs-lookup"><span data-stu-id="98c96-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="98c96-420">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="98c96-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="98c96-422">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="98c96-423">Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="98c96-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="98c96-424">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-425">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="98c96-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="98c96-426">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-427">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="98c96-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="98c96-428">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="98c96-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="98c96-429">MpnId</span></span></td>
<td><p><span data-ttu-id="98c96-430">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="98c96-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-431">MpnId rivenditore</span><span class="sxs-lookup"><span data-stu-id="98c96-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="98c96-432">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-433">ID ordine</span><span class="sxs-lookup"><span data-stu-id="98c96-433">Order ID</span></span></td>
<td><p><span data-ttu-id="98c96-434">Identificatore univoco per un ordine in cui la piattaforma di e-commerce di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="98c96-435">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-436">Data ordine</span><span class="sxs-lookup"><span data-stu-id="98c96-436">Order date</span></span></td>
<td><p><span data-ttu-id="98c96-437">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="98c96-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="98c96-438">ProductId</span></span></td>
<td><p><span data-ttu-id="98c96-439">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="98c96-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="98c96-440">SkuId</span></span></td>
<td><p><span data-ttu-id="98c96-441">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="98c96-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="98c96-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="98c96-443">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="98c96-443">The ID for a particular Availability.</span></span> <span data-ttu-id="98c96-444">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="98c96-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-445">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="98c96-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="98c96-446">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="98c96-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-447">Nome prodotto</span><span class="sxs-lookup"><span data-stu-id="98c96-447">Product name</span></span></td>
<td><p><span data-ttu-id="98c96-448">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="98c96-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="98c96-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="98c96-450">Il nome del server di pubblicazione del prodotto.</span><span class="sxs-lookup"><span data-stu-id="98c96-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="98c96-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="98c96-452">ID univoco per questo server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-453">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="98c96-454">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-455">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="98c96-456">Identificatore univoco per una sottoscrizione nella piattaforma Microsoft e-commerce.</span><span class="sxs-lookup"><span data-stu-id="98c96-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="98c96-457">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="98c96-458">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="98c96-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="98c96-460">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="98c96-460">Start day of the charges.</span></span> <span data-ttu-id="98c96-461">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="98c96-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="98c96-463">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="98c96-463">End day of the charges.</span></span> <span data-ttu-id="98c96-464">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="98c96-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-465">Periodo di validità e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="98c96-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="98c96-466">La durata del periodo e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="98c96-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="98c96-467">Ad esempio, "1 anno, mese."</span><span class="sxs-lookup"><span data-stu-id="98c96-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-468">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="98c96-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="98c96-469">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="98c96-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-470">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="98c96-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="98c96-471">Il prezzo come pubblicato nel listino prezzi dei contratti al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="98c96-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="98c96-472">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-473">Prezzo unitario efficace</span><span class="sxs-lookup"><span data-stu-id="98c96-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="98c96-474">Il prezzo unitario dopo che sono state apportate modifiche.</span><span class="sxs-lookup"><span data-stu-id="98c96-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-475">Quantità</span><span class="sxs-lookup"><span data-stu-id="98c96-475">Quantity</span></span></td>
<td><p><span data-ttu-id="98c96-476">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="98c96-476">Number of units.</span></span> <span data-ttu-id="98c96-477">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-478">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="98c96-478">Unit type</span></span></td>
<td><p><span data-ttu-id="98c96-479">Il tipo di unità acquistate.</span><span class="sxs-lookup"><span data-stu-id="98c96-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="98c96-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="98c96-481">Spiegazione di eventuali sconti.</span><span class="sxs-lookup"><span data-stu-id="98c96-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-482">Subtotale</span><span class="sxs-lookup"><span data-stu-id="98c96-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="98c96-483">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-483">Total before tax.</span></span> <span data-ttu-id="98c96-484">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="98c96-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-485">Totale imposte</span><span class="sxs-lookup"><span data-stu-id="98c96-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="98c96-486">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="98c96-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-487">Totale</span><span class="sxs-lookup"><span data-stu-id="98c96-487">Total</span></span></td>
<td><p><span data-ttu-id="98c96-488">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-488">Total after tax.</span></span> <span data-ttu-id="98c96-489">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-490">Valuta</span><span class="sxs-lookup"><span data-stu-id="98c96-490">Currency</span></span></td>
<td><p><span data-ttu-id="98c96-491">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-491">Currency type.</span></span> <span data-ttu-id="98c96-492">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="98c96-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="98c96-493">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="98c96-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="98c96-495">Un identificatore alternativo per un ID dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="98c96-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="98c96-496">Campi del file classificati giornaliera dell'utilizzo</span><span class="sxs-lookup"><span data-stu-id="98c96-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="98c96-497">Column</span><span class="sxs-lookup"><span data-stu-id="98c96-497">Column</span></span></th>
<th><span data-ttu-id="98c96-498">Descrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="98c96-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="98c96-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="98c96-500">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="98c96-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="98c96-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="98c96-502">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="98c96-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="98c96-504">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="98c96-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="98c96-506">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="98c96-507">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="98c96-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="98c96-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="98c96-509">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-509">The customer’s domain name.</span></span> <span data-ttu-id="98c96-510">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-511">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="98c96-511">Customer country</span></span></td>
<td><p><span data-ttu-id="98c96-512">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="98c96-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-513">MPNID</span></span></td>
<td><p><span data-ttu-id="98c96-514">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="98c96-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-515">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="98c96-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="98c96-516">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="98c96-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="98c96-517">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="98c96-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="98c96-519">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="98c96-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="98c96-520">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="98c96-521">ProductId</span></span></td>
<td><p><span data-ttu-id="98c96-522">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="98c96-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="98c96-523">SkuId</span></span></td>
<td><p><span data-ttu-id="98c96-524">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="98c96-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="98c96-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="98c96-526">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="98c96-526">The ID for a particular Availability.</span></span> <span data-ttu-id="98c96-527">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="98c96-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-528">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="98c96-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="98c96-529">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="98c96-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="98c96-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="98c96-531">Il nome del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="98c96-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="98c96-533">L'ID del server di pubblicazione, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="98c96-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="98c96-534">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="98c96-535">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="98c96-536">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="98c96-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="98c96-537">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="98c96-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-538">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="98c96-539">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98c96-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="98c96-540">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="98c96-541">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="98c96-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="98c96-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="98c96-543">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="98c96-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="98c96-544">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="98c96-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="98c96-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="98c96-546">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="98c96-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="98c96-547">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="98c96-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-548">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="98c96-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="98c96-549">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="98c96-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-550">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="98c96-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="98c96-551">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="98c96-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-552">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="98c96-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="98c96-553">Il servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="98c96-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-554">Id contatore</span><span class="sxs-lookup"><span data-stu-id="98c96-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="98c96-555">L'ID del contatore in uso.</span><span class="sxs-lookup"><span data-stu-id="98c96-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-556">Sottocategoria contatore</span><span class="sxs-lookup"><span data-stu-id="98c96-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="98c96-557">Tipo di servizio di Azure che possa influire sulla tariffa.</span><span class="sxs-lookup"><span data-stu-id="98c96-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-558">Nome contatore</span><span class="sxs-lookup"><span data-stu-id="98c96-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="98c96-559">L'unità di misura per il contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="98c96-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-560">Area contatore</span><span class="sxs-lookup"><span data-stu-id="98c96-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="98c96-561">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="98c96-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-562">Unità</span><span class="sxs-lookup"><span data-stu-id="98c96-562">Unit</span></span></td>
<td><p><span data-ttu-id="98c96-563">Unità di risorsa del nome.</span><span class="sxs-lookup"><span data-stu-id="98c96-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-564">Quantità utilizzata</span><span class="sxs-lookup"><span data-stu-id="98c96-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="98c96-565">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="98c96-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="98c96-566">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="98c96-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-567">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="98c96-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="98c96-568">Il Data Center in cui il contatore è in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="98c96-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-569">Servizio utilizzato</span><span class="sxs-lookup"><span data-stu-id="98c96-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="98c96-570">Il servizio della piattaforma Azure che è stato usato.</span><span class="sxs-lookup"><span data-stu-id="98c96-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-571">Gruppo di risorse</span><span class="sxs-lookup"><span data-stu-id="98c96-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="98c96-572">Il gruppo di risorse in cui è in esecuzione il contatore distribuito.</span><span class="sxs-lookup"><span data-stu-id="98c96-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-573">URI della risorsa</span><span class="sxs-lookup"><span data-stu-id="98c96-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="98c96-574">L'URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="98c96-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-575">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="98c96-575">Charge type</span></span></td>
<td><p><span data-ttu-id="98c96-576">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="98c96-576">The type of charge or adjustment.</span></span> <span data-ttu-id="98c96-577">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-578">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="98c96-578">Unit price</span></span></td>
<td><p><span data-ttu-id="98c96-579">Prezzo per ciascuna licenza, come pubblicato nel listino prezzi dei contratti al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="98c96-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="98c96-580">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-581">Quantità</span><span class="sxs-lookup"><span data-stu-id="98c96-581">Quantity</span></span></td>
<td><p><span data-ttu-id="98c96-582">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="98c96-582">Number of licenses.</span></span> <span data-ttu-id="98c96-583">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-584">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="98c96-584">Unit type</span></span></td>
<td><p><span data-ttu-id="98c96-585">Il tipo di unità che in cui viene addebitato il contatore.</span><span class="sxs-lookup"><span data-stu-id="98c96-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="98c96-586">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="98c96-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-587">La fatturazione pre fiscali</span><span class="sxs-lookup"><span data-stu-id="98c96-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="98c96-588">Quantità totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-589">Valuta di fatturazione</span><span class="sxs-lookup"><span data-stu-id="98c96-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="98c96-590">La valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="98c96-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-591">Prezzo totale al lordo di imposte</span><span class="sxs-lookup"><span data-stu-id="98c96-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="98c96-592">Il piano tariffario prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-593">Prezzi di valuta</span><span class="sxs-lookup"><span data-stu-id="98c96-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="98c96-594">La valuta nel prezzo di listino.</span><span class="sxs-lookup"><span data-stu-id="98c96-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-595">Informazioni servizio 1</span><span class="sxs-lookup"><span data-stu-id="98c96-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="98c96-596">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="98c96-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-597">Informazioni servizio 2</span><span class="sxs-lookup"><span data-stu-id="98c96-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="98c96-598">Campo legacy che acquisisce i metadati specifici del servizio facoltativo.</span><span class="sxs-lookup"><span data-stu-id="98c96-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="98c96-599">Tag</span><span class="sxs-lookup"><span data-stu-id="98c96-599">Tags</span></span></td>
<td><p><span data-ttu-id="98c96-600">Tag che è assegnare a misuratore in ordine per raggruppare i record di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="98c96-601">Ad esempio, è possibile usare tag per distribuire i costi in base al reparto che utilizza il contatore.</span><span class="sxs-lookup"><span data-stu-id="98c96-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="98c96-602">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="98c96-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="98c96-603">Eventuali informazioni aggiuntive non incluse in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="98c96-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="98c96-604">Addebiti di mapping tra una fattura e i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="98c96-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="98c96-605">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="98c96-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="98c96-606">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="98c96-607">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="98c96-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="98c96-608">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="98c96-609">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="98c96-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="98c96-610">Descrizione dell'addebito in fattura</span><span class="sxs-lookup"><span data-stu-id="98c96-610">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="98c96-611">Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="98c96-611">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="98c96-612">Descrizione dell'addebito</span><span class="sxs-lookup"><span data-stu-id="98c96-612">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="98c96-613">Come posso eseguire il mapping di questi tipi di addebito alla fattura?</span><span class="sxs-lookup"><span data-stu-id="98c96-613">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="98c96-614">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="98c96-614">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="98c96-615">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="98c96-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-616">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="98c96-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="98c96-617">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-618">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="98c96-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-619">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="98c96-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-620">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="98c96-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-621">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-622">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="98c96-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-623">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="98c96-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-624">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="98c96-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-625">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="98c96-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-626">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="98c96-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-627">Il tipo di addebito per una sottoscrizione quando si usa la fatturazione annua</span><span class="sxs-lookup"><span data-stu-id="98c96-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-628">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="98c96-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-629">Il tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="98c96-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-630">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="98c96-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-631">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="98c96-632">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="98c96-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-633">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-634">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="98c96-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-635">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="98c96-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="98c96-636">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="98c96-636">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="98c96-637">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="98c96-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-638">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="98c96-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="98c96-639">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-640">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="98c96-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-641">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="98c96-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="98c96-642">Crediti</span><span class="sxs-lookup"><span data-stu-id="98c96-642">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="98c96-643">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="98c96-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-644">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="98c96-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-645">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="98c96-646">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="98c96-647">Sconti in base all'uso</span><span class="sxs-lookup"><span data-stu-id="98c96-647">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="98c96-648">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="98c96-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-649">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="98c96-650">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-651">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="98c96-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-652">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="98c96-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-653">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="98c96-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-654">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="98c96-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-655">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="98c96-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-656">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="98c96-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="98c96-657">Sconti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="98c96-657">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="98c96-658">Possono essere applicati a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="98c96-658">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="98c96-659">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="98c96-660"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="98c96-661">Possono essere applicati a più tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="98c96-661">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="98c96-662">Eccezione: &quot;Offset di una voce&quot; include già le imposte.</span><span class="sxs-lookup"><span data-stu-id="98c96-662">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="98c96-663">Vedere Crediti qui sopra.</span><span class="sxs-lookup"><span data-stu-id="98c96-663">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="98c96-664">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="98c96-664">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="98c96-665">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-665">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="98c96-666">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="98c96-666">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
