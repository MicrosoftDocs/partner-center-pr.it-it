---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 07/08/2019
description: Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8fae84790aa84b3c5a006d65a632668a33ac24a7
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820562"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="db23b-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="db23b-103">Use the reconciliation files</span></span>

<span data-ttu-id="db23b-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="db23b-104">**Applies to**</span></span>

-  <span data-ttu-id="db23b-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="db23b-105">Partner Center</span></span>
-  <span data-ttu-id="db23b-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="db23b-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="db23b-107">Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="db23b-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="db23b-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="db23b-109">Problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="db23b-109">Formatting issues</span></span>

<span data-ttu-id="db23b-110">Occasionalmente il file di ricognizione potrebbe avere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="db23b-111">Questo può accadere, ad esempio, se le impostazioni locali EN-US non vengono usate. Per risolvere questi problemi, attenersi alla procedura riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="db23b-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="db23b-112">Aprire il file CSV in Excel e selezionare la prima colonna.</span><span class="sxs-lookup"><span data-stu-id="db23b-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="db23b-113">Sulla barra multifunzione selezionare <strong>dati</strong>, quindi selezionare <strong>testo in colonne</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="db23b-114">Nella procedura guidata Converti testo in colonne selezionare <strong>tipo di file delimitato</strong>e quindi fare clic su <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="db23b-115">Nel campo delimitatori selezionare virgola.</span><span class="sxs-lookup"><span data-stu-id="db23b-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="db23b-116">Se la <strong>scheda</strong> è già selezionata, è possibile lasciarla invariata.</span><span class="sxs-lookup"><span data-stu-id="db23b-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="db23b-117">Selezionare <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="db23b-118">Nel campo formato dati colonna selezionare <strong>Data: MDY</strong>, quindi selezionare <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="db23b-119">Nel campo formato dati colonna selezionare <strong>testo</strong> per tutte le colonne importo, quindi fare clic su <strong>fine</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="db23b-120">Download di un file di ricognizione di grandi dimensioni</span><span class="sxs-lookup"><span data-stu-id="db23b-120">Downloading a large recon file</span></span>

<span data-ttu-id="db23b-121">I file di ricognizione possono avere dimensioni molto elevate e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="db23b-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="db23b-122">Per uno script di PowerShell che consente di scaricare file di ricognizione di grandi dimensioni, vedere [ottenere le voci della fattura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="db23b-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="db23b-123">Descrivere per partner</span><span class="sxs-lookup"><span data-stu-id="db23b-123">Itemize by partner</span></span>


<span data-ttu-id="db23b-124">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="db23b-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="db23b-125">ID MPN</span><span class="sxs-lookup"><span data-stu-id="db23b-125">MPN ID</span></span></th>
<th><span data-ttu-id="db23b-126">Descrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="db23b-127">ID MPN</span><span class="sxs-lookup"><span data-stu-id="db23b-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="db23b-128">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="db23b-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-129">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="db23b-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="db23b-130">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="db23b-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="db23b-131">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="db23b-132">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="db23b-133">eTo visualizzare o aggiornare il rivenditore, dal menu centro per i partner selezionare Customers, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="db23b-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="db23b-134">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="db23b-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="db23b-135">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="db23b-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="db23b-136">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="db23b-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="db23b-137">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="db23b-138">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="db23b-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="db23b-139">Campi di file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="db23b-139">License-based file fields</span></span>


<span data-ttu-id="db23b-140">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="db23b-141"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="db23b-142"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="db23b-143"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="db23b-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="db23b-145">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="db23b-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="db23b-146">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="db23b-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="db23b-147">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="db23b-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="db23b-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="db23b-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="db23b-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="db23b-150">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="db23b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="db23b-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="db23b-152">OrderID</span></span></td>
<td><p><span data-ttu-id="db23b-153">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db23b-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="db23b-154">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="db23b-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="db23b-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="db23b-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="db23b-157">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db23b-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="db23b-158">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="db23b-159">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="db23b-160">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="db23b-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="db23b-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="db23b-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="db23b-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="db23b-163">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="db23b-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="db23b-164">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="db23b-165">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="db23b-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="db23b-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="db23b-167">OfferID</span></span></td>
<td><p><span data-ttu-id="db23b-168">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="db23b-168">Unique offer ID.</span></span> <span data-ttu-id="db23b-169">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="db23b-170"><b>Nota</b>: Questo valore non corrisponde all'ID offerta nell'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="db23b-171">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="db23b-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="db23b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="db23b-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="db23b-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="db23b-174">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="db23b-175"><b>Nota</b>: Questo valore corrisponde all'ID offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="db23b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="db23b-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="db23b-177">OfferName</span></span></td>
<td><p><span data-ttu-id="db23b-178">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="db23b-179">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="db23b-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="db23b-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="db23b-181">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="db23b-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="db23b-182">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="db23b-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="db23b-183">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="db23b-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="db23b-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="db23b-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="db23b-186">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allinearla alla data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="db23b-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="db23b-187">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="db23b-188">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="db23b-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="db23b-189">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="db23b-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="db23b-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="db23b-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="db23b-192">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="db23b-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="db23b-193">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="db23b-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="db23b-194">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="db23b-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="db23b-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="db23b-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="db23b-197">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="db23b-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="db23b-198">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="db23b-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="db23b-199">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="db23b-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="db23b-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="db23b-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="db23b-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="db23b-202">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="db23b-202">The type of charge or adjustment.</span></span> <span data-ttu-id="db23b-203">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="db23b-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="db23b-204">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="db23b-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="db23b-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="db23b-206">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="db23b-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="db23b-207">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="db23b-208">6.82</span><span class="sxs-lookup"><span data-stu-id="db23b-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-209">Quantità</span><span class="sxs-lookup"><span data-stu-id="db23b-209">Quantity</span></span></td>
<td><p><span data-ttu-id="db23b-210">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="db23b-210">Number of seats.</span></span> <span data-ttu-id="db23b-211">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="db23b-212">2</span><span class="sxs-lookup"><span data-stu-id="db23b-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-213">Importo</span><span class="sxs-lookup"><span data-stu-id="db23b-213">Amount</span></span></td>
<td><p><span data-ttu-id="db23b-214">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="db23b-214">Total of price for quantity.</span></span> <span data-ttu-id="db23b-215">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="db23b-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="db23b-216">13.32</span><span class="sxs-lookup"><span data-stu-id="db23b-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="db23b-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="db23b-218">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="db23b-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="db23b-219">Le licenze dei prodotti incluse con una competenza o mappe o nuove sottoscrizioni idonee per un incentivo conterranno anche un importo di sconto in questo articolo.</span><span class="sxs-lookup"><span data-stu-id="db23b-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="db23b-220">2.32</span><span class="sxs-lookup"><span data-stu-id="db23b-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="db23b-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="db23b-222">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-222">Total before tax.</span></span> <span data-ttu-id="db23b-223">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="db23b-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="db23b-224">11</span><span class="sxs-lookup"><span data-stu-id="db23b-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-225">Imposta</span><span class="sxs-lookup"><span data-stu-id="db23b-225">Tax</span></span></td>
<td><p><span data-ttu-id="db23b-226">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="db23b-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="db23b-227">0</span><span class="sxs-lookup"><span data-stu-id="db23b-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="db23b-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="db23b-229">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-229">Total after tax.</span></span> <span data-ttu-id="db23b-230">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="db23b-231">11</span><span class="sxs-lookup"><span data-stu-id="db23b-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-232">Currency</span><span class="sxs-lookup"><span data-stu-id="db23b-232">Currency</span></span></td>
<td><p><span data-ttu-id="db23b-233">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-233">Currency type.</span></span> <span data-ttu-id="db23b-234">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="db23b-235">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="db23b-236">EUR</span><span class="sxs-lookup"><span data-stu-id="db23b-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="db23b-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="db23b-238">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="db23b-239">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="db23b-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="db23b-240">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="db23b-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-241">MPNID</span></span></td>
<td><p><span data-ttu-id="db23b-242">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="db23b-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="db23b-243">4390934</span><span class="sxs-lookup"><span data-stu-id="db23b-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="db23b-245">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="db23b-246">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="db23b-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="db23b-247">4390934</span><span class="sxs-lookup"><span data-stu-id="db23b-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="db23b-248">DomainName</span></span></td>
<td><p><span data-ttu-id="db23b-249">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="db23b-250">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="db23b-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="db23b-251">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="db23b-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="db23b-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="db23b-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="db23b-254">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-254">Subscription nickname.</span></span> <span data-ttu-id="db23b-255">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="db23b-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="db23b-256">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="db23b-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="db23b-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="db23b-258">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="db23b-259">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="db23b-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="db23b-260">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="db23b-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="db23b-261">Campi di file basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="db23b-261">Usage-based file fields</span></span>


<span data-ttu-id="db23b-262">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="db23b-263">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="db23b-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="db23b-264"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="db23b-265"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="db23b-266"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="db23b-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="db23b-268">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="db23b-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="db23b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="db23b-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="db23b-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="db23b-271">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="db23b-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="db23b-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="db23b-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="db23b-274">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="db23b-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="db23b-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="db23b-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="db23b-277">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="db23b-278">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="db23b-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="db23b-279">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="db23b-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-280">MPNID</span></span></td>
<td><p><span data-ttu-id="db23b-281">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="db23b-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="db23b-282">4390934</span><span class="sxs-lookup"><span data-stu-id="db23b-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="db23b-284">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="db23b-285">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="db23b-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="db23b-286">4390934</span><span class="sxs-lookup"><span data-stu-id="db23b-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="db23b-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="db23b-288">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="db23b-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="db23b-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="db23b-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="db23b-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="db23b-291">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="db23b-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="db23b-292">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="db23b-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="db23b-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="db23b-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="db23b-295">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="db23b-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="db23b-296">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="db23b-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="db23b-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="db23b-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="db23b-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="db23b-299">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db23b-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="db23b-300">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="db23b-301">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="db23b-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="db23b-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="db23b-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="db23b-304">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="db23b-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="db23b-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="db23b-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="db23b-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="db23b-307">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="db23b-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="db23b-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="db23b-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="db23b-309">OrderID</span></span></td>
<td><p><span data-ttu-id="db23b-310">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db23b-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="db23b-311">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="db23b-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="db23b-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="db23b-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="db23b-314">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="db23b-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="db23b-315">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="db23b-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="db23b-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="db23b-317">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="db23b-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="db23b-318">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="db23b-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="db23b-319">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="db23b-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="db23b-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="db23b-321">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="db23b-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="db23b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="db23b-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-323">Nome risorsa</span><span class="sxs-lookup"><span data-stu-id="db23b-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="db23b-324">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="db23b-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="db23b-325">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="db23b-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="db23b-326">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="db23b-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-327">Region</span><span class="sxs-lookup"><span data-stu-id="db23b-327">Region</span></span></td>
<td><p><span data-ttu-id="db23b-328">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="db23b-328">The region the usage applies to.</span></span> <span data-ttu-id="db23b-329">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="db23b-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="db23b-330">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="db23b-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-331">SKU</span><span class="sxs-lookup"><span data-stu-id="db23b-331">SKU</span></span></td>
<td><p><span data-ttu-id="db23b-332">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="db23b-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="db23b-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="db23b-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="db23b-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="db23b-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="db23b-335">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="db23b-336">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="db23b-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="db23b-337">1</span><span class="sxs-lookup"><span data-stu-id="db23b-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="db23b-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="db23b-339">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="db23b-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="db23b-340">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="db23b-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="db23b-341">11</span><span class="sxs-lookup"><span data-stu-id="db23b-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="db23b-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="db23b-343">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="db23b-343">Units included as part of the offer.</span></span> <span data-ttu-id="db23b-344">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="db23b-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="db23b-345">0</span><span class="sxs-lookup"><span data-stu-id="db23b-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="db23b-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="db23b-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="db23b-347">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="db23b-348">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="db23b-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="db23b-349">11</span><span class="sxs-lookup"><span data-stu-id="db23b-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="db23b-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="db23b-351">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="db23b-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="db23b-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="db23b-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="db23b-354">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="db23b-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="db23b-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="db23b-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="db23b-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="db23b-357">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="db23b-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="db23b-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="db23b-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="db23b-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="db23b-360">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="db23b-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="db23b-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="db23b-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-362">Currency</span><span class="sxs-lookup"><span data-stu-id="db23b-362">Currency</span></span></td>
<td><p><span data-ttu-id="db23b-363">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-363">Currency type.</span></span> <span data-ttu-id="db23b-364">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="db23b-365">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="db23b-366">EUR</span><span class="sxs-lookup"><span data-stu-id="db23b-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="db23b-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="db23b-368">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-368">Pretax price per unit.</span></span> <span data-ttu-id="db23b-369">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="db23b-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="db23b-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="db23b-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="db23b-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="db23b-372">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-372">Post tax price per unit.</span></span> <span data-ttu-id="db23b-373">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="db23b-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="db23b-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="db23b-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="db23b-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="db23b-376">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="db23b-376">The type of charge or adjustment.</span></span> <span data-ttu-id="db23b-377">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="db23b-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="db23b-378">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="db23b-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="db23b-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="db23b-380">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="db23b-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="db23b-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="db23b-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="db23b-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="db23b-383">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="db23b-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="db23b-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="db23b-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="db23b-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="db23b-386">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="db23b-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="db23b-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="db23b-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="db23b-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="db23b-389">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="db23b-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="db23b-390">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="db23b-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="db23b-391">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="db23b-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="db23b-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="db23b-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="db23b-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="db23b-394">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="db23b-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="db23b-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="db23b-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-396">Progetto</span><span class="sxs-lookup"><span data-stu-id="db23b-396">Project</span></span></td>
<td><p><span data-ttu-id="db23b-397">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="db23b-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="db23b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="db23b-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="db23b-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="db23b-400">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="db23b-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="db23b-401">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="db23b-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="db23b-402">Se è stato eseguito il provisioning di 25 pacchetti di bus di bus e si è usato 1 durante tale giorno, l'istruzione di utilizzo giornaliero per quel giorno indicherà "25 connessioni/30 giorni – usato: 1,000000 ".</span><span class="sxs-lookup"><span data-stu-id="db23b-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="db23b-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="db23b-404">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="db23b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="db23b-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="db23b-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="db23b-406">DomainName</span></span></td>
<td><p><span data-ttu-id="db23b-407">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="db23b-408">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="db23b-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="db23b-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="db23b-410">Unità</span><span class="sxs-lookup"><span data-stu-id="db23b-410">Unit</span></span></td>
<td><p><span data-ttu-id="db23b-411">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="db23b-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="db23b-412">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="db23b-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="db23b-413">Campi di file una sola volta e ricorrenti</span><span class="sxs-lookup"><span data-stu-id="db23b-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="db23b-414">Colonna</span><span class="sxs-lookup"><span data-stu-id="db23b-414">Column</span></span></th>
<th><span data-ttu-id="db23b-415">Descrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="db23b-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="db23b-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="db23b-417">Identificatore univoco del tenant Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="db23b-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="db23b-418">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="db23b-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="db23b-419">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="db23b-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-420">ID cliente</span><span class="sxs-lookup"><span data-stu-id="db23b-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="db23b-421">Univoco Microsoft Azure Active Directory ID tenant, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-422">Nome del cliente</span><span class="sxs-lookup"><span data-stu-id="db23b-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="db23b-423">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="db23b-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="db23b-425">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="db23b-426">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="db23b-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="db23b-427">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-428">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="db23b-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="db23b-429">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-430">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="db23b-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="db23b-431">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="db23b-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="db23b-432">MpnId</span></span></td>
<td><p><span data-ttu-id="db23b-433">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="db23b-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-434">Rivenditore MpnId</span><span class="sxs-lookup"><span data-stu-id="db23b-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="db23b-435">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-436">ID ordine</span><span class="sxs-lookup"><span data-stu-id="db23b-436">Order ID</span></span></td>
<td><p><span data-ttu-id="db23b-437">Identificatore univoco per un ordine in Microsoft Commerce platform.</span><span class="sxs-lookup"><span data-stu-id="db23b-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="db23b-438">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-439">Data ordine</span><span class="sxs-lookup"><span data-stu-id="db23b-439">Order date</span></span></td>
<td><p><span data-ttu-id="db23b-440">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="db23b-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="db23b-441">ProductId</span></span></td>
<td><p><span data-ttu-id="db23b-442">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="db23b-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="db23b-443">SkuId</span></span></td>
<td><p><span data-ttu-id="db23b-444">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="db23b-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="db23b-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="db23b-446">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="db23b-446">The ID for a particular Availability.</span></span> <span data-ttu-id="db23b-447">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="db23b-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-448">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="db23b-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="db23b-449">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="db23b-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-450">Nome prodotto</span><span class="sxs-lookup"><span data-stu-id="db23b-450">Product name</span></span></td>
<td><p><span data-ttu-id="db23b-451">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="db23b-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="db23b-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="db23b-453">Nome del server di pubblicazione del prodotto.</span><span class="sxs-lookup"><span data-stu-id="db23b-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="db23b-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="db23b-455">ID univoco per questo server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-456">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="db23b-457">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-458">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="db23b-459">Identificatore univoco per una sottoscrizione nella piattaforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="db23b-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="db23b-460">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="db23b-461">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="db23b-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="db23b-463">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="db23b-463">Start day of the charges.</span></span> <span data-ttu-id="db23b-464">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="db23b-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="db23b-466">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="db23b-466">End day of the charges.</span></span> <span data-ttu-id="db23b-467">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="db23b-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-468">Termini e billingcycle</span><span class="sxs-lookup"><span data-stu-id="db23b-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="db23b-469">Durata e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="db23b-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="db23b-470">Ad esempio, "1 anno, mensile".</span><span class="sxs-lookup"><span data-stu-id="db23b-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-471">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="db23b-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="db23b-472">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="db23b-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-473">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="db23b-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="db23b-474">Prezzo pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="db23b-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="db23b-475">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-476">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="db23b-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="db23b-477">Prezzo unitario dopo le rettifiche apportate.</span><span class="sxs-lookup"><span data-stu-id="db23b-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-478">Quantità</span><span class="sxs-lookup"><span data-stu-id="db23b-478">Quantity</span></span></td>
<td><p><span data-ttu-id="db23b-479">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="db23b-479">Number of units.</span></span> <span data-ttu-id="db23b-480">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-481">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="db23b-481">Unit type</span></span></td>
<td><p><span data-ttu-id="db23b-482">Tipo di unità da acquistare.</span><span class="sxs-lookup"><span data-stu-id="db23b-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="db23b-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="db23b-484">Spiegazione di qualsiasi sconto applicabile.</span><span class="sxs-lookup"><span data-stu-id="db23b-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-485">Totale parziale</span><span class="sxs-lookup"><span data-stu-id="db23b-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="db23b-486">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-486">Total before tax.</span></span> <span data-ttu-id="db23b-487">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="db23b-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-488">Imposta totale</span><span class="sxs-lookup"><span data-stu-id="db23b-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="db23b-489">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="db23b-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-490">Totale</span><span class="sxs-lookup"><span data-stu-id="db23b-490">Total</span></span></td>
<td><p><span data-ttu-id="db23b-491">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-491">Total after tax.</span></span> <span data-ttu-id="db23b-492">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-493">Currency</span><span class="sxs-lookup"><span data-stu-id="db23b-493">Currency</span></span></td>
<td><p><span data-ttu-id="db23b-494">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-494">Currency type.</span></span> <span data-ttu-id="db23b-495">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="db23b-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="db23b-496">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="db23b-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="db23b-498">Identificatore alternativo a un ID dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="db23b-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="db23b-499">Campi del file di utilizzo con classificazione giornaliera</span><span class="sxs-lookup"><span data-stu-id="db23b-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="db23b-500">Colonna</span><span class="sxs-lookup"><span data-stu-id="db23b-500">Column</span></span></th>
<th><span data-ttu-id="db23b-501">Descrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="db23b-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="db23b-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="db23b-503">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="db23b-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="db23b-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="db23b-505">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="db23b-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="db23b-507">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="db23b-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="db23b-509">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="db23b-510">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="db23b-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="db23b-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="db23b-512">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-512">The customer’s domain name.</span></span> <span data-ttu-id="db23b-513">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-514">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="db23b-514">Customer country</span></span></td>
<td><p><span data-ttu-id="db23b-515">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="db23b-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-516">MPNID</span></span></td>
<td><p><span data-ttu-id="db23b-517">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="db23b-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-518">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="db23b-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="db23b-519">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="db23b-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="db23b-520">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="db23b-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="db23b-522">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="db23b-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="db23b-523">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="db23b-524">ProductId</span></span></td>
<td><p><span data-ttu-id="db23b-525">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="db23b-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="db23b-526">SkuId</span></span></td>
<td><p><span data-ttu-id="db23b-527">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="db23b-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="db23b-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="db23b-529">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="db23b-529">The ID for a particular Availability.</span></span> <span data-ttu-id="db23b-530">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="db23b-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-531">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="db23b-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="db23b-532">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="db23b-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="db23b-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="db23b-534">Nome del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="db23b-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="db23b-536">ID del server di pubblicazione in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="db23b-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="db23b-537">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="db23b-538">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="db23b-539">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="db23b-540">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="db23b-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-541">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="db23b-542">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db23b-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="db23b-543">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="db23b-544">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="db23b-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="db23b-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="db23b-546">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="db23b-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="db23b-547">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="db23b-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="db23b-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="db23b-549">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="db23b-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="db23b-550">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="db23b-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-551">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="db23b-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="db23b-552">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="db23b-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-553">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="db23b-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="db23b-554">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="db23b-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-555">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="db23b-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="db23b-556">Servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="db23b-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-557">ID contatore</span><span class="sxs-lookup"><span data-stu-id="db23b-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="db23b-558">ID del contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="db23b-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-559">Sottocategoria contatore</span><span class="sxs-lookup"><span data-stu-id="db23b-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="db23b-560">Tipo di servizio di Azure che può influire sulla frequenza.</span><span class="sxs-lookup"><span data-stu-id="db23b-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-561">Nome contatore</span><span class="sxs-lookup"><span data-stu-id="db23b-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="db23b-562">Unità di misura per il contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="db23b-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-563">Area del contatore</span><span class="sxs-lookup"><span data-stu-id="db23b-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="db23b-564">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="db23b-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-565">Unità</span><span class="sxs-lookup"><span data-stu-id="db23b-565">Unit</span></span></td>
<td><p><span data-ttu-id="db23b-566">Unità del nome della risorsa.</span><span class="sxs-lookup"><span data-stu-id="db23b-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-567">Quantità utilizzata</span><span class="sxs-lookup"><span data-stu-id="db23b-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="db23b-568">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="db23b-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="db23b-569">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="db23b-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-570">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="db23b-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="db23b-571">Data Center in cui è in esecuzione il contatore.</span><span class="sxs-lookup"><span data-stu-id="db23b-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-572">Servizio utilizzato</span><span class="sxs-lookup"><span data-stu-id="db23b-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="db23b-573">Il servizio della piattaforma Azure usato.</span><span class="sxs-lookup"><span data-stu-id="db23b-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="db23b-574">URI della risorsa</span><span class="sxs-lookup"><span data-stu-id="db23b-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="db23b-575">URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="db23b-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-576">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="db23b-576">Charge type</span></span></td>
<td><p><span data-ttu-id="db23b-577">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="db23b-577">The type of charge or adjustment.</span></span> <span data-ttu-id="db23b-578">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-579">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="db23b-579">Unit price</span></span></td>
<td><p><span data-ttu-id="db23b-580">Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="db23b-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="db23b-581">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-582">Quantità</span><span class="sxs-lookup"><span data-stu-id="db23b-582">Quantity</span></span></td>
<td><p><span data-ttu-id="db23b-583">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="db23b-583">Number of licenses.</span></span> <span data-ttu-id="db23b-584">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-585">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="db23b-585">Unit type</span></span></td>
<td><p><span data-ttu-id="db23b-586">Tipo di unità in cui viene addebitato il contatore.</span><span class="sxs-lookup"><span data-stu-id="db23b-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="db23b-587">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="db23b-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-588">Pre-imposta fatturazione</span><span class="sxs-lookup"><span data-stu-id="db23b-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="db23b-589">Importo totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-590">Valuta fatturazione</span><span class="sxs-lookup"><span data-stu-id="db23b-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="db23b-591">Valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="db23b-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-592">Prezzi pretassazione totali</span><span class="sxs-lookup"><span data-stu-id="db23b-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="db23b-593">I prezzi prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="db23b-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-594">Valuta prezzi</span><span class="sxs-lookup"><span data-stu-id="db23b-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="db23b-595">Valuta nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="db23b-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="db23b-596">Informazioni servizio 1</span><span class="sxs-lookup"><span data-stu-id="db23b-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="db23b-597">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="db23b-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-598">Informazioni servizio 2</span><span class="sxs-lookup"><span data-stu-id="db23b-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="db23b-599">Campo legacy che acquisisce i metadati facoltativi specifici del servizio.</span><span class="sxs-lookup"><span data-stu-id="db23b-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="db23b-600">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="db23b-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="db23b-601">Eventuali informazioni aggiuntive non incluse in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="db23b-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="db23b-602">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="db23b-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="db23b-603">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="db23b-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="db23b-604">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="db23b-605">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="db23b-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="db23b-606">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="db23b-607">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="db23b-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="db23b-608"><strong>Descrizione addebito fattura</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-609"><strong>Descrizione addebito file di riconciliazione (colonna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-610"><strong>Qual è il costo?</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-611"><strong>Ricerca per categorie mappare questi ChargeTypes alla fattura?</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="db23b-612"><strong>Addebiti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-613">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="db23b-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-614">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="db23b-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="db23b-615">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-616">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="db23b-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-617">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="db23b-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-618">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="db23b-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-619">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-620">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="db23b-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-621">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="db23b-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-622">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="db23b-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-623">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="db23b-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-624">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="db23b-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-625">Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale</span><span class="sxs-lookup"><span data-stu-id="db23b-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-626">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="db23b-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-627">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="db23b-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-628">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="db23b-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-629">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="db23b-630">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="db23b-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-631">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-632">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="db23b-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-633">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="db23b-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="db23b-634"><strong>Addebiti monouso</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="db23b-635">Nuova</span><span class="sxs-lookup"><span data-stu-id="db23b-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-636">Utilizzato quando viene creato un nuovo acquisto</span><span class="sxs-lookup"><span data-stu-id="db23b-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="db23b-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-638">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo l'aumento</span><span class="sxs-lookup"><span data-stu-id="db23b-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="db23b-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-640">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo la riduzione</span><span class="sxs-lookup"><span data-stu-id="db23b-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-641">Annulla</span><span class="sxs-lookup"><span data-stu-id="db23b-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-642">Utilizzato quando viene annullata una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-643">Convertire</span><span class="sxs-lookup"><span data-stu-id="db23b-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-644">Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato</span><span class="sxs-lookup"><span data-stu-id="db23b-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="db23b-645"><strong>Addebiti per l'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-646">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="db23b-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-647">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="db23b-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="db23b-648">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-649">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="db23b-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-650">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="db23b-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="db23b-651"><strong>Crediti</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-652">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="db23b-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-653">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="db23b-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-654">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="db23b-655">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="db23b-656"><strong>Sconti basati sull'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-657">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="db23b-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-658">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="db23b-659">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-660">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="db23b-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-661">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="db23b-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-662">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="db23b-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-663">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="db23b-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-664">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="db23b-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-665">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="db23b-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="db23b-666"><strong>Sconti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-667"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="db23b-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="db23b-668">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="db23b-669"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-670"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="db23b-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="db23b-671"><em>Eccezione: &quot;Offset una voce&quot; include già le imposte. Vedere crediti, sopra.</em></span><span class="sxs-lookup"><span data-stu-id="db23b-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-672">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="db23b-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="db23b-673">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="db23b-674">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="db23b-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
