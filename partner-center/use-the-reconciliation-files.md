---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
description: Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 2d5792ad8f1a01c94336b208c825b10a269ae054
ms.sourcegitcommit: 47a91bb6d961630f154fde738075b73ff84a829e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/18/2019
ms.locfileid: "67193418"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="ea9e7-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-103">Use the reconciliation files</span></span>

<span data-ttu-id="ea9e7-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="ea9e7-104">**Applies to**</span></span>

-  <span data-ttu-id="ea9e7-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ea9e7-105">Partner Center</span></span>
-  <span data-ttu-id="ea9e7-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ea9e7-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ea9e7-107">Per una visualizzazione dettagliata voce ogni gratuitamente in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="ea9e7-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="ea9e7-109">Problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-109">Formatting issues</span></span>

<span data-ttu-id="ea9e7-110">In alcuni casi il file di riconoscimento potrà avere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="ea9e7-111">(Questa situazione può verificarsi, ad esempio, se non viene utilizzata le impostazioni locali EN-US.) Attenersi alla procedura seguente per risolvere questi problemi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="ea9e7-112">Aprire il file con estensione csv in Excel e selezionare la prima colonna.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="ea9e7-113">Sulla barra multifunzione, selezionare <strong>dati</strong>, quindi selezionare <strong>testo alle colonne</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="ea9e7-114">La conversione guidata testo in colonne, selezionare <strong>tipo di file delimitati</strong>e quindi selezionare <strong>successivo</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ea9e7-115">Nel campo Delimeters, selezionare <strong>virgole</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="ea9e7-116">Se <strong>scheda</strong> è già selezionata, è possibile lasciarla.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="ea9e7-117">Selezionare <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="ea9e7-118">Nel campo formato dei dati di colonna, selezionare <strong>data: MDY</strong>, quindi selezionare <strong>successivo</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="ea9e7-119">Nel campo formato dei dati di colonna, selezionare <strong>testo</strong> per tutte le colonne e quindi selezionare l'importo <strong>fine</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="ea9e7-120">Download di un file di riconoscimento di grandi dimensioni</span><span class="sxs-lookup"><span data-stu-id="ea9e7-120">Downloading a large recon file</span></span>

<span data-ttu-id="ea9e7-121">File di riconoscimento possono raggiungere dimensioni molto grandi e sono talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="ea9e7-122">Per uno script di PowerShell scaricare i file di grandi dimensioni riconoscimento, vedere [voci della fattura Get](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="ea9e7-123">Specificare i dettagli da partner</span><span class="sxs-lookup"><span data-stu-id="ea9e7-123">Itemize by partner</span></span>


<span data-ttu-id="ea9e7-124">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ea9e7-125">ID MPN</span><span class="sxs-lookup"><span data-stu-id="ea9e7-125">MPN ID</span></span></th>
<th><span data-ttu-id="ea9e7-126">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ea9e7-127">ID MPN</span><span class="sxs-lookup"><span data-stu-id="ea9e7-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="ea9e7-128">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-129">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="ea9e7-130">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="ea9e7-131">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ea9e7-132">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="ea9e7-133">eTo visualizzare o aggiornare il rivenditore, dal menu Centro per i Partner, selezionare <strong>clienti</strong>, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="ea9e7-134">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="ea9e7-135">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="ea9e7-136">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="ea9e7-137">Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="ea9e7-138">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="ea9e7-139">Campi del file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="ea9e7-139">License-based file fields</span></span>


<span data-ttu-id="ea9e7-140">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ea9e7-141"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ea9e7-142"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ea9e7-143"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="ea9e7-145">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ea9e7-146">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ea9e7-147">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="ea9e7-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="ea9e7-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="ea9e7-150">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ea9e7-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="ea9e7-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-152">OrderID</span></span></td>
<td><p><span data-ttu-id="ea9e7-153">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ea9e7-154">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ea9e7-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ea9e7-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ea9e7-157">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ea9e7-158">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ea9e7-159">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="ea9e7-160">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="ea9e7-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ea9e7-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="ea9e7-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="ea9e7-163">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="ea9e7-164">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="ea9e7-165">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ea9e7-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="ea9e7-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-167">OfferID</span></span></td>
<td><p><span data-ttu-id="ea9e7-168">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-168">Unique offer ID.</span></span> <span data-ttu-id="ea9e7-169">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="ea9e7-170"><b>Nota</b>: Questo valore non corrisponde ID offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="ea9e7-171">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="ea9e7-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="ea9e7-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="ea9e7-174">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="ea9e7-175"><b>Nota</b>: Questo valore corrisponde all'ID dell'offerta dall'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="ea9e7-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="ea9e7-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-177">OfferName</span></span></td>
<td><p><span data-ttu-id="ea9e7-178">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="ea9e7-179">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="ea9e7-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-181">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="ea9e7-182">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="ea9e7-183">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ea9e7-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ea9e7-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-186">La data di fine sottoscrizione: 12 mesi + x giorni dopo la data di inizio (in modo da allinearsi partner data di fatturazione) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="ea9e7-187">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="ea9e7-188">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="ea9e7-189">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ea9e7-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ea9e7-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-192">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="ea9e7-193">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ea9e7-194">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ea9e7-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="ea9e7-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-197">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="ea9e7-198">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="ea9e7-199">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ea9e7-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="ea9e7-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ea9e7-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="ea9e7-202">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-202">The type of charge or adjustment.</span></span> <span data-ttu-id="ea9e7-203">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ea9e7-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ea9e7-204">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ea9e7-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="ea9e7-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="ea9e7-206">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ea9e7-207">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ea9e7-208">6.82</span><span class="sxs-lookup"><span data-stu-id="ea9e7-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-209">Quantità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-209">Quantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-210">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-210">Number of seats.</span></span> <span data-ttu-id="ea9e7-211">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="ea9e7-212">2</span><span class="sxs-lookup"><span data-stu-id="ea9e7-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-213">Importo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-213">Amount</span></span></td>
<td><p><span data-ttu-id="ea9e7-214">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-214">Total of price for quantity.</span></span> <span data-ttu-id="ea9e7-215">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="ea9e7-216">13.32</span><span class="sxs-lookup"><span data-stu-id="ea9e7-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="ea9e7-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="ea9e7-218">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="ea9e7-219">IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="ea9e7-220">2.32</span><span class="sxs-lookup"><span data-stu-id="ea9e7-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="ea9e7-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="ea9e7-222">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-222">Total before tax.</span></span> <span data-ttu-id="ea9e7-223">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="ea9e7-224">11</span><span class="sxs-lookup"><span data-stu-id="ea9e7-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-225">Imposta</span><span class="sxs-lookup"><span data-stu-id="ea9e7-225">Tax</span></span></td>
<td><p><span data-ttu-id="ea9e7-226">Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ea9e7-227">0</span><span class="sxs-lookup"><span data-stu-id="ea9e7-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="ea9e7-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="ea9e7-229">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-229">Total after tax.</span></span> <span data-ttu-id="ea9e7-230">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="ea9e7-231">11</span><span class="sxs-lookup"><span data-stu-id="ea9e7-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-232">Currency</span><span class="sxs-lookup"><span data-stu-id="ea9e7-232">Currency</span></span></td>
<td><p><span data-ttu-id="ea9e7-233">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-233">Currency type.</span></span> <span data-ttu-id="ea9e7-234">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="ea9e7-235">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ea9e7-236">EUR</span><span class="sxs-lookup"><span data-stu-id="ea9e7-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="ea9e7-238">Cliente&#39;nome organizzazione s come riportato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ea9e7-239">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ea9e7-240">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="ea9e7-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-241">MPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-242">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="ea9e7-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="ea9e7-243">4390934</span><span class="sxs-lookup"><span data-stu-id="ea9e7-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-245">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ea9e7-246">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ea9e7-247">4390934</span><span class="sxs-lookup"><span data-stu-id="ea9e7-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-248">DomainName</span></span></td>
<td><p><span data-ttu-id="ea9e7-249">Cliente&#39;nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ea9e7-250">Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ea9e7-251">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ea9e7-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ea9e7-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ea9e7-254">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-254">Subscription nickname.</span></span> <span data-ttu-id="ea9e7-255">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="ea9e7-256">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="ea9e7-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ea9e7-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ea9e7-258">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ea9e7-259">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="ea9e7-260">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="ea9e7-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="ea9e7-261">Campi del file basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-261">Usage-based file fields</span></span>


<span data-ttu-id="ea9e7-262">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="ea9e7-263">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ea9e7-264"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="ea9e7-265"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="ea9e7-266"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="ea9e7-268">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="ea9e7-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ea9e7-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="ea9e7-271">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="ea9e7-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="ea9e7-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="ea9e7-274">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="ea9e7-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="ea9e7-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="ea9e7-277">Cliente&#39;nome organizzazione s come riportato nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="ea9e7-278">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="ea9e7-279">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="ea9e7-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-280">MPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-281">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="ea9e7-282">4390934</span><span class="sxs-lookup"><span data-stu-id="ea9e7-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-284">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ea9e7-285">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="ea9e7-286">4390934</span><span class="sxs-lookup"><span data-stu-id="ea9e7-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ea9e7-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ea9e7-288">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="ea9e7-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="ea9e7-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-291">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ea9e7-292">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="ea9e7-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ea9e7-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-295">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="ea9e7-296">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="ea9e7-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="ea9e7-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="ea9e7-299">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ea9e7-300">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="ea9e7-301">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="ea9e7-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="ea9e7-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="ea9e7-304">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="ea9e7-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ea9e7-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="ea9e7-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="ea9e7-307">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="ea9e7-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="ea9e7-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="ea9e7-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-309">OrderID</span></span></td>
<td><p><span data-ttu-id="ea9e7-310">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="ea9e7-311">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="ea9e7-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="ea9e7-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="ea9e7-314">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="ea9e7-315">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="ea9e7-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="ea9e7-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="ea9e7-317">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ea9e7-318">Service Bus – Individual o Pack</span><span class="sxs-lookup"><span data-stu-id="ea9e7-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="ea9e7-319">SQL Azure database – Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="ea9e7-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="ea9e7-321">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="ea9e7-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="ea9e7-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-323">Nome della risorsa</span><span class="sxs-lookup"><span data-stu-id="ea9e7-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="ea9e7-324">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="ea9e7-325">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="ea9e7-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="ea9e7-326">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="ea9e7-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-327">Area geografica</span><span class="sxs-lookup"><span data-stu-id="ea9e7-327">Region</span></span></td>
<td><p><span data-ttu-id="ea9e7-328">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-328">The region the usage applies to.</span></span> <span data-ttu-id="ea9e7-329">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="ea9e7-330">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="ea9e7-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-331">SKU</span><span class="sxs-lookup"><span data-stu-id="ea9e7-331">SKU</span></span></td>
<td><p><span data-ttu-id="ea9e7-332">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="ea9e7-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="ea9e7-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="ea9e7-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="ea9e7-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="ea9e7-335">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="ea9e7-336">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="ea9e7-337">1</span><span class="sxs-lookup"><span data-stu-id="ea9e7-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="ea9e7-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-339">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="ea9e7-340">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="ea9e7-341">11</span><span class="sxs-lookup"><span data-stu-id="ea9e7-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="ea9e7-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-343">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-343">Units included as part of the offer.</span></span> <span data-ttu-id="ea9e7-344">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="ea9e7-345">0</span><span class="sxs-lookup"><span data-stu-id="ea9e7-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="ea9e7-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="ea9e7-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="ea9e7-347">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="ea9e7-348">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="ea9e7-349">11</span><span class="sxs-lookup"><span data-stu-id="ea9e7-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="ea9e7-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="ea9e7-351">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="ea9e7-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="ea9e7-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="ea9e7-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="ea9e7-354">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ea9e7-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="ea9e7-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="ea9e7-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="ea9e7-357">Addebito quantità, in base del mercato di imposta&#39;le regole di tassazione s e circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="ea9e7-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="ea9e7-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="ea9e7-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="ea9e7-360">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="ea9e7-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="ea9e7-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-362">Currency</span><span class="sxs-lookup"><span data-stu-id="ea9e7-362">Currency</span></span></td>
<td><p><span data-ttu-id="ea9e7-363">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-363">Currency type.</span></span> <span data-ttu-id="ea9e7-364">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="ea9e7-365">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="ea9e7-366">EUR</span><span class="sxs-lookup"><span data-stu-id="ea9e7-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ea9e7-368">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-368">Pretax price per unit.</span></span> <span data-ttu-id="ea9e7-369">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ea9e7-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="ea9e7-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="ea9e7-372">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-372">Post tax price per unit.</span></span> <span data-ttu-id="ea9e7-373">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="ea9e7-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="ea9e7-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="ea9e7-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="ea9e7-376">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-376">The type of charge or adjustment.</span></span> <span data-ttu-id="ea9e7-377">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ea9e7-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="ea9e7-378">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="ea9e7-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="ea9e7-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="ea9e7-380">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="ea9e7-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="ea9e7-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-383">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="ea9e7-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="ea9e7-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="ea9e7-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="ea9e7-386">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="ea9e7-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="ea9e7-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="ea9e7-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="ea9e7-389">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="ea9e7-390">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="ea9e7-391">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="ea9e7-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="ea9e7-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="ea9e7-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="ea9e7-394">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="ea9e7-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="ea9e7-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-396">Project</span><span class="sxs-lookup"><span data-stu-id="ea9e7-396">Project</span></span></td>
<td><p><span data-ttu-id="ea9e7-397">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="ea9e7-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="ea9e7-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ea9e7-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="ea9e7-400">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="ea9e7-401">Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days".</span><span class="sxs-lookup"><span data-stu-id="ea9e7-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="ea9e7-402">Se disponi di un pacchetto 25 di connessioni del bus di servizio eseguito il provisioning e si fosse utilizzato 1 durante il giorno, l'istruzione di utilizzo giornaliero per quel giorno indicherebbe "25 connessioni / 30 giorni: utilizzato: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="ea9e7-404">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="ea9e7-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="ea9e7-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ea9e7-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-406">DomainName</span></span></td>
<td><p><span data-ttu-id="ea9e7-407">Cliente&#39;nome di dominio s, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="ea9e7-408">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="ea9e7-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="ea9e7-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="ea9e7-410">Unità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-410">Unit</span></span></td>
<td><p><span data-ttu-id="ea9e7-411">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="ea9e7-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="ea9e7-412">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="ea9e7-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="ea9e7-413">Campi del file sia monouso che ricorrenti</span><span class="sxs-lookup"><span data-stu-id="ea9e7-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ea9e7-414">Colonna</span><span class="sxs-lookup"><span data-stu-id="ea9e7-414">Column</span></span></th>
<th><span data-ttu-id="ea9e7-415">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="ea9e7-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="ea9e7-417">Identificatore univoco tenant di Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="ea9e7-418">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="ea9e7-419">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-420">Id cliente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="ea9e7-421">Microsoft Azure Active Directory tenant ID univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-422">Nome cliente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="ea9e7-423">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ea9e7-425">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="ea9e7-426">Non dovrebbe utilizzabile per identificare in modo univoco il cliente, così come i clienti o del partner è possibile aggiornare il dominio personalizzato o predefinito tramite il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="ea9e7-427">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-428">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="ea9e7-429">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-430">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="ea9e7-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="ea9e7-431">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-432">MpnId</span></span></td>
<td><p><span data-ttu-id="ea9e7-433">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-434">MpnId rivenditore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="ea9e7-435">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-436">ID ordine</span><span class="sxs-lookup"><span data-stu-id="ea9e7-436">Order ID</span></span></td>
<td><p><span data-ttu-id="ea9e7-437">Identificatore univoco per un ordine in cui la piattaforma di e-commerce di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="ea9e7-438">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-439">Data ordine</span><span class="sxs-lookup"><span data-stu-id="ea9e7-439">Order date</span></span></td>
<td><p><span data-ttu-id="ea9e7-440">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-441">ProductId</span></span></td>
<td><p><span data-ttu-id="ea9e7-442">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-443">SkuId</span></span></td>
<td><p><span data-ttu-id="ea9e7-444">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ea9e7-446">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-446">The ID for a particular Availability.</span></span> <span data-ttu-id="ea9e7-447">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-448">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="ea9e7-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="ea9e7-449">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-450">Nome del prodotto</span><span class="sxs-lookup"><span data-stu-id="ea9e7-450">Product name</span></span></td>
<td><p><span data-ttu-id="ea9e7-451">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="ea9e7-453">Il nome del server di pubblicazione del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="ea9e7-455">ID univoco per questo server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-456">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ea9e7-457">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-458">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ea9e7-459">Identificatore univoco per una sottoscrizione nella piattaforma Microsoft e-commerce.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="ea9e7-460">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ea9e7-461">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-463">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-463">Start day of the charges.</span></span> <span data-ttu-id="ea9e7-464">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-466">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-466">End day of the charges.</span></span> <span data-ttu-id="ea9e7-467">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-468">Periodo di validità e Billingcycle</span><span class="sxs-lookup"><span data-stu-id="ea9e7-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="ea9e7-469">La durata del periodo e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="ea9e7-470">Ad esempio, "1 anno, mese."</span><span class="sxs-lookup"><span data-stu-id="ea9e7-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-471">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="ea9e7-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="ea9e7-472">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-473">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="ea9e7-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="ea9e7-474">Il prezzo come pubblicato nel listino prezzi dei contratti al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ea9e7-475">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-476">Prezzo unitario efficace</span><span class="sxs-lookup"><span data-stu-id="ea9e7-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="ea9e7-477">Il prezzo unitario dopo che sono state apportate modifiche.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-478">Quantità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-478">Quantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-479">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-479">Number of units.</span></span> <span data-ttu-id="ea9e7-480">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-481">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-481">Unit type</span></span></td>
<td><p><span data-ttu-id="ea9e7-482">Il tipo di unità acquistate.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="ea9e7-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="ea9e7-484">Spiegazione di eventuali sconti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-485">Subtotale</span><span class="sxs-lookup"><span data-stu-id="ea9e7-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="ea9e7-486">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-486">Total before tax.</span></span> <span data-ttu-id="ea9e7-487">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-488">Totale imposte</span><span class="sxs-lookup"><span data-stu-id="ea9e7-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="ea9e7-489">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-490">Totale</span><span class="sxs-lookup"><span data-stu-id="ea9e7-490">Total</span></span></td>
<td><p><span data-ttu-id="ea9e7-491">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-491">Total after tax.</span></span> <span data-ttu-id="ea9e7-492">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-493">Currency</span><span class="sxs-lookup"><span data-stu-id="ea9e7-493">Currency</span></span></td>
<td><p><span data-ttu-id="ea9e7-494">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-494">Currency type.</span></span> <span data-ttu-id="ea9e7-495">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="ea9e7-496">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="ea9e7-498">Un identificatore alternativo per un ID dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="ea9e7-499">Campi del file classificati giornaliera dell'utilizzo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ea9e7-500">Colonna</span><span class="sxs-lookup"><span data-stu-id="ea9e7-500">Column</span></span></th>
<th><span data-ttu-id="ea9e7-501">Descrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="ea9e7-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="ea9e7-503">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="ea9e7-505">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="ea9e7-507">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="ea9e7-509">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="ea9e7-510">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="ea9e7-512">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-512">The customer’s domain name.</span></span> <span data-ttu-id="ea9e7-513">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-514">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-514">Customer country</span></span></td>
<td><p><span data-ttu-id="ea9e7-515">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-516">MPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-517">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-518">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="ea9e7-519">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="ea9e7-520">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="ea9e7-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="ea9e7-522">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="ea9e7-523">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-524">ProductId</span></span></td>
<td><p><span data-ttu-id="ea9e7-525">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-526">SkuId</span></span></td>
<td><p><span data-ttu-id="ea9e7-527">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="ea9e7-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="ea9e7-529">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-529">The ID for a particular Availability.</span></span> <span data-ttu-id="ea9e7-530">"Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-531">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="ea9e7-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="ea9e7-532">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="ea9e7-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="ea9e7-534">Il nome del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="ea9e7-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="ea9e7-536">L'ID del server di pubblicazione, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="ea9e7-537">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="ea9e7-538">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="ea9e7-539">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="ea9e7-540">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-541">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="ea9e7-542">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="ea9e7-543">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="ea9e7-544">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-546">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ea9e7-547">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="ea9e7-549">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="ea9e7-550">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-551">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="ea9e7-552">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-553">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="ea9e7-554">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-555">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="ea9e7-556">Il servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-557">Id contatore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="ea9e7-558">L'ID del contatore in uso.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-559">Sottocategoria contatore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="ea9e7-560">Tipo di servizio di Azure che possa influire sulla tariffa.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-561">Nome contatore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="ea9e7-562">L'unità di misura per il contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-563">Area contatore</span><span class="sxs-lookup"><span data-stu-id="ea9e7-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="ea9e7-564">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-565">Unità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-565">Unit</span></span></td>
<td><p><span data-ttu-id="ea9e7-566">Unità di risorsa del nome.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-567">Quantità utilizzata</span><span class="sxs-lookup"><span data-stu-id="ea9e7-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-568">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="ea9e7-569">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-570">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="ea9e7-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="ea9e7-571">Il Data Center in cui il contatore è in esecuzione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-572">Servizio utilizzato</span><span class="sxs-lookup"><span data-stu-id="ea9e7-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="ea9e7-573">Il servizio della piattaforma Azure che è stato usato.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-574">Gruppo di risorse</span><span class="sxs-lookup"><span data-stu-id="ea9e7-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="ea9e7-575">Il gruppo di risorse in cui è in esecuzione il contatore distribuito.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-576">URI della risorsa</span><span class="sxs-lookup"><span data-stu-id="ea9e7-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="ea9e7-577">L'URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-578">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="ea9e7-578">Charge type</span></span></td>
<td><p><span data-ttu-id="ea9e7-579">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-579">The type of charge or adjustment.</span></span> <span data-ttu-id="ea9e7-580">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-581">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="ea9e7-581">Unit price</span></span></td>
<td><p><span data-ttu-id="ea9e7-582">Prezzo per ciascuna licenza, come pubblicato nel listino prezzi dei contratti al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="ea9e7-583">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-584">Quantità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-584">Quantity</span></span></td>
<td><p><span data-ttu-id="ea9e7-585">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-585">Number of licenses.</span></span> <span data-ttu-id="ea9e7-586">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-587">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="ea9e7-587">Unit type</span></span></td>
<td><p><span data-ttu-id="ea9e7-588">Il tipo di unità che in cui viene addebitato il contatore.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="ea9e7-589">Non è disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-590">La fatturazione pre fiscali</span><span class="sxs-lookup"><span data-stu-id="ea9e7-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="ea9e7-591">Quantità totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-592">Valuta di fatturazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="ea9e7-593">La valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-594">Prezzo totale al lordo di imposte</span><span class="sxs-lookup"><span data-stu-id="ea9e7-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="ea9e7-595">Il piano tariffario prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-596">Prezzi di valuta</span><span class="sxs-lookup"><span data-stu-id="ea9e7-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="ea9e7-597">La valuta nel prezzo di listino.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-598">Informazioni servizio 1</span><span class="sxs-lookup"><span data-stu-id="ea9e7-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="ea9e7-599">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-600">Informazioni servizio 2</span><span class="sxs-lookup"><span data-stu-id="ea9e7-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="ea9e7-601">Campo legacy che acquisisce i metadati specifici del servizio facoltativo.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="ea9e7-602">`Tags`</span><span class="sxs-lookup"><span data-stu-id="ea9e7-602">Tags</span></span></td>
<td><p><span data-ttu-id="ea9e7-603">Tag che è assegnare a misuratore in ordine per raggruppare i record di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="ea9e7-604">Ad esempio, è possibile usare tag per distribuire i costi in base al reparto che utilizza il contatore.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="ea9e7-605">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="ea9e7-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="ea9e7-606">Eventuali informazioni aggiuntive non incluse in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="ea9e7-607">Addebiti di mapping tra una fattura e i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="ea9e7-608">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="ea9e7-609">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="ea9e7-610">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="ea9e7-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="ea9e7-611">Sconti, rimborsi o crediti una tantum che vengono visualizzati nella fattura come "Rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="ea9e7-612">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="ea9e7-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="ea9e7-613"><strong>Descrizione di addebito della fattura</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-614"><strong>Descrizione di addebito file di riconciliazione (ChargeType colonna)</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-615"><strong>Che cos'è l'addebito?</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-616"><strong>Come è possibile associare queste ChargeTypes nella fattura?</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="ea9e7-617"><strong>Addebiti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-618">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-619">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="ea9e7-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="ea9e7-620">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-621">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="ea9e7-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-622">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-623">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="ea9e7-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-624">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-625">Istanza del ciclo rateizzata</span><span class="sxs-lookup"><span data-stu-id="ea9e7-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-626">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="ea9e7-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-627">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="ea9e7-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-628">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="ea9e7-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-629">Rateizza le tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="ea9e7-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-630">Il tipo di addebito per una sottoscrizione quando si usa la fatturazione annua</span><span class="sxs-lookup"><span data-stu-id="ea9e7-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-631">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="ea9e7-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-632">Il tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="ea9e7-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-633">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-634">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="ea9e7-635">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-636">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-637">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-638">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>


<tr>
<td rowspan="2">
<p><span data-ttu-id="ea9e7-639"><strong>Costi di utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-639"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-640">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="ea9e7-640">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-641">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-641">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="ea9e7-642">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-642">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-643">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-643">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-644">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="ea9e7-644">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="ea9e7-645"><strong>Crediti</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-645"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-646">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="ea9e7-646">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-647">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="ea9e7-647">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-648">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-648">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="ea9e7-649">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-649">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="ea9e7-650"><strong>Sconti basati sull'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-650"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-651">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-651">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-652">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-652">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="ea9e7-653">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-654">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-654">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-655">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="ea9e7-655">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-656">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="ea9e7-656">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-657">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="ea9e7-657">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-658">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="ea9e7-658">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-659">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="ea9e7-659">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="ea9e7-660"><strong>Sconti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-660"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-661"><em>Può essere applicato a più tipi di costo</em></span><span class="sxs-lookup"><span data-stu-id="ea9e7-661"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-662">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-662">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="ea9e7-663"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-663"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-664"><em>Può essere applicato a più tipi di costo</em></span><span class="sxs-lookup"><span data-stu-id="ea9e7-664"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="ea9e7-665"><em>Eccezione: &quot;Offset di una voce&quot; include già le imposte. Vedere i crediti, sopra.</em></span><span class="sxs-lookup"><span data-stu-id="ea9e7-665"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-666">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="ea9e7-666">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="ea9e7-667">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-667">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="ea9e7-668">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="ea9e7-668">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
