---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 07/08/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 7b27e99e5c0dc55fad3b06cc22316e8282dbe35c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653980"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="f4383-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="f4383-103">Use the reconciliation files</span></span>

<span data-ttu-id="f4383-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="f4383-104">**Applies to**</span></span>

-  <span data-ttu-id="f4383-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="f4383-105">Partner Center</span></span>
-  <span data-ttu-id="f4383-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f4383-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="f4383-107">Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="f4383-108">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="f4383-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="f4383-109">Problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="f4383-109">Formatting issues</span></span>

<span data-ttu-id="f4383-110">Occasionalmente il file di ricognizione potrebbe avere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="f4383-111">Questo può accadere, ad esempio, se le impostazioni locali EN-US non vengono usate. Per risolvere questi problemi, attenersi alla procedura riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="f4383-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="f4383-112">Aprire il file CSV in Excel e selezionare la prima colonna.</span><span class="sxs-lookup"><span data-stu-id="f4383-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="f4383-113">Sulla barra multifunzione selezionare <strong>dati</strong>, quindi selezionare <strong>testo in colonne</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="f4383-114">Nella procedura guidata Converti testo in colonne selezionare <strong>tipo di file delimitato</strong>e quindi fare clic su <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="f4383-115">Nel campo delimitatori selezionare <strong>virgola</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="f4383-116">Se la <strong>scheda</strong> è già selezionata, è possibile lasciarla invariata.</span><span class="sxs-lookup"><span data-stu-id="f4383-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="f4383-117">Seleziona <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="f4383-118">Nel campo formato dati colonna selezionare <strong>Data: MDY</strong>, quindi fare clic su <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="f4383-119">Nel campo formato dati colonna selezionare <strong>testo</strong> per tutte le colonne importo, quindi fare clic su <strong>fine</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="f4383-120">Download di un file di ricognizione di grandi dimensioni</span><span class="sxs-lookup"><span data-stu-id="f4383-120">Downloading a large recon file</span></span>

<span data-ttu-id="f4383-121">I file di ricognizione possono avere dimensioni molto elevate e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="f4383-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="f4383-122">Per uno script di PowerShell che consente di scaricare file di ricognizione di grandi dimensioni, vedere [ottenere le voci della fattura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="f4383-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="f4383-123">Descrivere per partner</span><span class="sxs-lookup"><span data-stu-id="f4383-123">Itemize by partner</span></span>


<span data-ttu-id="f4383-124">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="f4383-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f4383-125">ID MPN</span><span class="sxs-lookup"><span data-stu-id="f4383-125">MPN ID</span></span></th>
<th><span data-ttu-id="f4383-126">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f4383-127">ID MPN</span><span class="sxs-lookup"><span data-stu-id="f4383-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="f4383-128">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="f4383-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-129">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="f4383-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="f4383-130">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="f4383-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="f4383-131">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f4383-132">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="f4383-133">eTo visualizzare o aggiornare il rivenditore, dal menu centro per i partner selezionare <strong>Customers</strong>, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="f4383-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="f4383-134">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="f4383-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="f4383-135">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="f4383-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="f4383-136">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="f4383-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="f4383-137">Se un partner CSP ha un rivenditore senza ID MPN, questo valore viene impostato invece sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="f4383-138">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="f4383-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="f4383-139">Campi di file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="f4383-139">License-based file fields</span></span>


<span data-ttu-id="f4383-140">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f4383-141"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f4383-142"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f4383-143"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f4383-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="f4383-145">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f4383-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f4383-146">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="f4383-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f4383-147">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="f4383-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="f4383-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="f4383-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f4383-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="f4383-150">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f4383-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="f4383-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="f4383-152">OrderID</span></span></td>
<td><p><span data-ttu-id="f4383-153">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f4383-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f4383-154">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f4383-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f4383-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f4383-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f4383-157">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f4383-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f4383-158">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f4383-159">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="f4383-160">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="f4383-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="f4383-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f4383-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="f4383-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="f4383-163">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="f4383-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="f4383-164">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="f4383-165">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f4383-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="f4383-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="f4383-167">OfferID</span></span></td>
<td><p><span data-ttu-id="f4383-168">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="f4383-168">Unique offer ID.</span></span> <span data-ttu-id="f4383-169">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="f4383-170"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="f4383-171">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="f4383-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="f4383-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="f4383-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="f4383-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="f4383-174">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="f4383-175"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="f4383-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="f4383-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="f4383-177">OfferName</span></span></td>
<td><p><span data-ttu-id="f4383-178">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="f4383-179">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="f4383-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="f4383-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="f4383-181">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="f4383-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="f4383-182">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="f4383-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="f4383-183">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f4383-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f4383-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="f4383-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="f4383-186">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="f4383-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="f4383-187">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="f4383-188">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="f4383-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="f4383-189">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f4383-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f4383-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f4383-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f4383-192">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="f4383-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="f4383-193">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="f4383-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f4383-194">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f4383-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f4383-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f4383-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f4383-197">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="f4383-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="f4383-198">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="f4383-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f4383-199">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="f4383-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f4383-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="f4383-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f4383-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="f4383-202">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="f4383-202">The type of charge or adjustment.</span></span> <span data-ttu-id="f4383-203">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="f4383-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f4383-204">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="f4383-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="f4383-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="f4383-206">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="f4383-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f4383-207">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f4383-208">6.82</span><span class="sxs-lookup"><span data-stu-id="f4383-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-209">Quantità</span><span class="sxs-lookup"><span data-stu-id="f4383-209">Quantity</span></span></td>
<td><p><span data-ttu-id="f4383-210">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="f4383-210">Number of seats.</span></span> <span data-ttu-id="f4383-211">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f4383-212">2</span><span class="sxs-lookup"><span data-stu-id="f4383-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-213">Importo</span><span class="sxs-lookup"><span data-stu-id="f4383-213">Amount</span></span></td>
<td><p><span data-ttu-id="f4383-214">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="f4383-214">Total of price for quantity.</span></span> <span data-ttu-id="f4383-215">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="f4383-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="f4383-216">13.32</span><span class="sxs-lookup"><span data-stu-id="f4383-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="f4383-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="f4383-218">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="f4383-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="f4383-219">Le licenze dei prodotti incluse con una competenza o mappe o nuove sottoscrizioni idonee per un incentivo conterranno anche un importo di sconto in questo articolo.</span><span class="sxs-lookup"><span data-stu-id="f4383-219">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="f4383-220">2.32</span><span class="sxs-lookup"><span data-stu-id="f4383-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="f4383-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="f4383-222">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-222">Total before tax.</span></span> <span data-ttu-id="f4383-223">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="f4383-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="f4383-224">11</span><span class="sxs-lookup"><span data-stu-id="f4383-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-225">Imposta</span><span class="sxs-lookup"><span data-stu-id="f4383-225">Tax</span></span></td>
<td><p><span data-ttu-id="f4383-226">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="f4383-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f4383-227">0</span><span class="sxs-lookup"><span data-stu-id="f4383-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="f4383-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="f4383-229">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-229">Total after tax.</span></span> <span data-ttu-id="f4383-230">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="f4383-231">11</span><span class="sxs-lookup"><span data-stu-id="f4383-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-232">Currency</span><span class="sxs-lookup"><span data-stu-id="f4383-232">Currency</span></span></td>
<td><p><span data-ttu-id="f4383-233">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-233">Currency type.</span></span> <span data-ttu-id="f4383-234">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="f4383-235">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f4383-236">EUR</span><span class="sxs-lookup"><span data-stu-id="f4383-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f4383-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="f4383-238">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f4383-239">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="f4383-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f4383-240">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="f4383-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-241">MPNID</span></span></td>
<td><p><span data-ttu-id="f4383-242">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="f4383-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="f4383-243">4390934</span><span class="sxs-lookup"><span data-stu-id="f4383-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f4383-245">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f4383-246">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="f4383-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f4383-247">4390934</span><span class="sxs-lookup"><span data-stu-id="f4383-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="f4383-248">DomainName</span></span></td>
<td><p><span data-ttu-id="f4383-249">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f4383-250">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="f4383-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f4383-251">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f4383-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f4383-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f4383-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f4383-254">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-254">Subscription nickname.</span></span> <span data-ttu-id="f4383-255">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="f4383-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="f4383-256">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="f4383-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f4383-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f4383-258">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f4383-259">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="f4383-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="f4383-260">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="f4383-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="f4383-261">Campi di file basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="f4383-261">Usage-based file fields</span></span>


<span data-ttu-id="f4383-262">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="f4383-263">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="f4383-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f4383-264"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f4383-265"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f4383-266"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f4383-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="f4383-268">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f4383-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="f4383-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f4383-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f4383-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="f4383-271">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="f4383-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="f4383-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="f4383-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="f4383-274">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="f4383-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="f4383-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f4383-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="f4383-277">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f4383-278">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="f4383-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f4383-279">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="f4383-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-280">MPNID</span></span></td>
<td><p><span data-ttu-id="f4383-281">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f4383-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="f4383-282">4390934</span><span class="sxs-lookup"><span data-stu-id="f4383-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f4383-284">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f4383-285">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="f4383-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f4383-286">4390934</span><span class="sxs-lookup"><span data-stu-id="f4383-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f4383-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f4383-288">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="f4383-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="f4383-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="f4383-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f4383-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f4383-291">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="f4383-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f4383-292">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f4383-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f4383-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f4383-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f4383-295">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="f4383-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f4383-296">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="f4383-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f4383-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="f4383-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f4383-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f4383-299">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f4383-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f4383-300">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f4383-301">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f4383-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f4383-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f4383-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f4383-304">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="f4383-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="f4383-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f4383-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f4383-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f4383-307">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="f4383-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="f4383-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f4383-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="f4383-309">OrderID</span></span></td>
<td><p><span data-ttu-id="f4383-310">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f4383-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f4383-311">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f4383-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f4383-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="f4383-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="f4383-314">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="f4383-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="f4383-315">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="f4383-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="f4383-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="f4383-317">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="f4383-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f4383-318">Bus di servizio-singolo o Pack</span><span class="sxs-lookup"><span data-stu-id="f4383-318">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="f4383-319">SQL Azure database-Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="f4383-319">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="f4383-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="f4383-321">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="f4383-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="f4383-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f4383-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-323">Resource Name</span><span class="sxs-lookup"><span data-stu-id="f4383-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="f4383-324">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="f4383-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f4383-325">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="f4383-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="f4383-326">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="f4383-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-327">Area geografica</span><span class="sxs-lookup"><span data-stu-id="f4383-327">Region</span></span></td>
<td><p><span data-ttu-id="f4383-328">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="f4383-328">The region the usage applies to.</span></span> <span data-ttu-id="f4383-329">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="f4383-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="f4383-330">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="f4383-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-331">SKU</span><span class="sxs-lookup"><span data-stu-id="f4383-331">SKU</span></span></td>
<td><p><span data-ttu-id="f4383-332">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="f4383-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="f4383-333">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="f4383-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="f4383-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="f4383-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="f4383-335">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="f4383-336">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="f4383-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="f4383-337">1</span><span class="sxs-lookup"><span data-stu-id="f4383-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="f4383-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="f4383-339">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="f4383-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="f4383-340">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="f4383-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="f4383-341">11</span><span class="sxs-lookup"><span data-stu-id="f4383-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="f4383-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="f4383-343">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="f4383-343">Units included as part of the offer.</span></span> <span data-ttu-id="f4383-344">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="f4383-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="f4383-345">0</span><span class="sxs-lookup"><span data-stu-id="f4383-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f4383-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="f4383-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="f4383-347">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="f4383-348">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="f4383-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="f4383-349">11</span><span class="sxs-lookup"><span data-stu-id="f4383-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="f4383-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="f4383-351">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="f4383-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="f4383-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="f4383-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="f4383-354">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="f4383-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f4383-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="f4383-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="f4383-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="f4383-357">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="f4383-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f4383-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="f4383-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="f4383-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="f4383-360">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="f4383-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="f4383-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="f4383-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-362">Currency</span><span class="sxs-lookup"><span data-stu-id="f4383-362">Currency</span></span></td>
<td><p><span data-ttu-id="f4383-363">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-363">Currency type.</span></span> <span data-ttu-id="f4383-364">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="f4383-365">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f4383-366">EUR</span><span class="sxs-lookup"><span data-stu-id="f4383-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f4383-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f4383-368">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-368">Pretax price per unit.</span></span> <span data-ttu-id="f4383-369">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="f4383-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f4383-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="f4383-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f4383-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f4383-372">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-372">Post tax price per unit.</span></span> <span data-ttu-id="f4383-373">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="f4383-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f4383-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="f4383-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f4383-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="f4383-376">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="f4383-376">The type of charge or adjustment.</span></span> <span data-ttu-id="f4383-377">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="f4383-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f4383-378">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="f4383-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="f4383-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="f4383-380">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="f4383-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="f4383-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="f4383-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="f4383-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="f4383-383">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="f4383-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="f4383-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f4383-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="f4383-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="f4383-386">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="f4383-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="f4383-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="f4383-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="f4383-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="f4383-389">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="f4383-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="f4383-390">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="f4383-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="f4383-391">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="f4383-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="f4383-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="f4383-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="f4383-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="f4383-394">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="f4383-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="f4383-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="f4383-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-396">Project</span><span class="sxs-lookup"><span data-stu-id="f4383-396">Project</span></span></td>
<td><p><span data-ttu-id="f4383-397">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="f4383-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="f4383-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f4383-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="f4383-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="f4383-400">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="f4383-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="f4383-401">Ad esempio, se si dispone di una connessione di cui è stato effettuato il provisioning individualmente durante un mese di 30 giorni, Service Info 1 leggerà "1,000000 connessioni/30 giorni".</span><span class="sxs-lookup"><span data-stu-id="f4383-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="f4383-402">Se è stato effettuato il provisioning di un pacchetto di 25 connessioni ServiceBus e l'utilizzo di 1 durante tale giorno, l'utilizzo giornaliero per quel giorno indicherebbe "25 connessioni/30 giorni-usato: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="f4383-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f4383-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="f4383-404">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f4383-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f4383-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f4383-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="f4383-406">DomainName</span></span></td>
<td><p><span data-ttu-id="f4383-407">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f4383-408">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f4383-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f4383-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="f4383-410">Unit</span><span class="sxs-lookup"><span data-stu-id="f4383-410">Unit</span></span></td>
<td><p><span data-ttu-id="f4383-411">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="f4383-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="f4383-412">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="f4383-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="f4383-413">Campi di file una sola volta e ricorrenti</span><span class="sxs-lookup"><span data-stu-id="f4383-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f4383-414">Column</span><span class="sxs-lookup"><span data-stu-id="f4383-414">Column</span></span></th>
<th><span data-ttu-id="f4383-415">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-415">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="f4383-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f4383-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="f4383-417">Identificatore univoco del tenant Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f4383-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f4383-418">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="f4383-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f4383-419">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="f4383-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-420">ID cliente</span><span class="sxs-lookup"><span data-stu-id="f4383-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="f4383-421">Univoco Microsoft Azure Active Directory ID tenant, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-422">Nome cliente</span><span class="sxs-lookup"><span data-stu-id="f4383-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="f4383-423">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f4383-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f4383-425">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="f4383-426">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="f4383-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f4383-427">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-428">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="f4383-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="f4383-429">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-430">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="f4383-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="f4383-431">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="f4383-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="f4383-432">MpnId</span></span></td>
<td><p><span data-ttu-id="f4383-433">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f4383-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-434">Rivenditore MpnId</span><span class="sxs-lookup"><span data-stu-id="f4383-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="f4383-435">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-436">ID ordine</span><span class="sxs-lookup"><span data-stu-id="f4383-436">Order ID</span></span></td>
<td><p><span data-ttu-id="f4383-437">Identificatore univoco per un ordine in Microsoft Commerce platform.</span><span class="sxs-lookup"><span data-stu-id="f4383-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="f4383-438">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-439">Data ordine</span><span class="sxs-lookup"><span data-stu-id="f4383-439">Order date</span></span></td>
<td><p><span data-ttu-id="f4383-440">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="f4383-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="f4383-441">ProductId</span></span></td>
<td><p><span data-ttu-id="f4383-442">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="f4383-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="f4383-443">SkuId</span></span></td>
<td><p><span data-ttu-id="f4383-444">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="f4383-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f4383-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f4383-446">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="f4383-446">The ID for a particular Availability.</span></span> <span data-ttu-id="f4383-447">"Disponibilità" indica se un particolare SKU è disponibile per l'acquisto per il paese, la valuta, il segmento di settore e così via.</span><span class="sxs-lookup"><span data-stu-id="f4383-447">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-448">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="f4383-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="f4383-449">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="f4383-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-450">Nome del prodotto</span><span class="sxs-lookup"><span data-stu-id="f4383-450">Product name</span></span></td>
<td><p><span data-ttu-id="f4383-451">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="f4383-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f4383-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="f4383-453">Nome del server di pubblicazione del prodotto.</span><span class="sxs-lookup"><span data-stu-id="f4383-453">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f4383-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="f4383-455">ID univoco per questo server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-456">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f4383-457">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-458">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f4383-459">Identificatore univoco per una sottoscrizione nella piattaforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="f4383-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="f4383-460">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f4383-461">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f4383-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f4383-463">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="f4383-463">Start day of the charges.</span></span> <span data-ttu-id="f4383-464">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f4383-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f4383-466">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="f4383-466">End day of the charges.</span></span> <span data-ttu-id="f4383-467">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="f4383-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-468">Termini e billingcycle</span><span class="sxs-lookup"><span data-stu-id="f4383-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="f4383-469">Durata e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="f4383-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="f4383-470">Ad esempio, "1 anno, mensile".</span><span class="sxs-lookup"><span data-stu-id="f4383-470">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-471">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="f4383-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="f4383-472">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="f4383-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-473">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="f4383-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="f4383-474">Prezzo pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="f4383-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f4383-475">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-476">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="f4383-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="f4383-477">Prezzo unitario dopo le rettifiche apportate.</span><span class="sxs-lookup"><span data-stu-id="f4383-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-478">Quantità</span><span class="sxs-lookup"><span data-stu-id="f4383-478">Quantity</span></span></td>
<td><p><span data-ttu-id="f4383-479">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="f4383-479">Number of units.</span></span> <span data-ttu-id="f4383-480">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-481">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="f4383-481">Unit type</span></span></td>
<td><p><span data-ttu-id="f4383-482">Tipo di unità da acquistare.</span><span class="sxs-lookup"><span data-stu-id="f4383-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="f4383-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="f4383-484">Spiegazione di qualsiasi sconto applicabile.</span><span class="sxs-lookup"><span data-stu-id="f4383-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-485">Totale parziale</span><span class="sxs-lookup"><span data-stu-id="f4383-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="f4383-486">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-486">Total before tax.</span></span> <span data-ttu-id="f4383-487">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="f4383-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-488">Imposta totale</span><span class="sxs-lookup"><span data-stu-id="f4383-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="f4383-489">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="f4383-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-490">Totale</span><span class="sxs-lookup"><span data-stu-id="f4383-490">Total</span></span></td>
<td><p><span data-ttu-id="f4383-491">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-491">Total after tax.</span></span> <span data-ttu-id="f4383-492">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-493">Currency</span><span class="sxs-lookup"><span data-stu-id="f4383-493">Currency</span></span></td>
<td><p><span data-ttu-id="f4383-494">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-494">Currency type.</span></span> <span data-ttu-id="f4383-495">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="f4383-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="f4383-496">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="f4383-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="f4383-498">Identificatore alternativo a un ID dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="f4383-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-499">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="f4383-499">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="f4383-500">Visualizza mensilmente quando è abilitata la fatturazione mensile.</span><span class="sxs-lookup"><span data-stu-id="f4383-500">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="f4383-501">Altrimenti vuoto.</span><span class="sxs-lookup"><span data-stu-id="f4383-501">Otherwise blank.</span></span> </p></td>
</tr>

</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="f4383-502">Campi del file di utilizzo con classificazione giornaliera</span><span class="sxs-lookup"><span data-stu-id="f4383-502">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f4383-503">Column</span><span class="sxs-lookup"><span data-stu-id="f4383-503">Column</span></span></th>
<th><span data-ttu-id="f4383-504">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-504">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="f4383-505">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f4383-505">PartnerId</span></span></td>
<td><p><span data-ttu-id="f4383-506">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f4383-506">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-507">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f4383-507">PartnerName</span></span></td>
<td><p><span data-ttu-id="f4383-508">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-508">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-509">CustomerId</span><span class="sxs-lookup"><span data-stu-id="f4383-509">CustomerId</span></span></td>
<td><p><span data-ttu-id="f4383-510">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-510">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-511">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="f4383-511">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="f4383-512">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-512">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="f4383-513">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="f4383-513">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-514">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f4383-514">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f4383-515">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-515">The customer's domain name.</span></span> <span data-ttu-id="f4383-516">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-516">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-517">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="f4383-517">Customer country</span></span></td>
<td><p><span data-ttu-id="f4383-518">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="f4383-518">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-519">MPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-519">MPNID</span></span></td>
<td><p><span data-ttu-id="f4383-520">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f4383-520">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-521">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="f4383-521">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="f4383-522">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f4383-522">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f4383-523">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-524">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f4383-524">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f4383-525">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="f4383-525">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="f4383-526">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-526">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-527">ProductId</span><span class="sxs-lookup"><span data-stu-id="f4383-527">ProductId</span></span></td>
<td><p><span data-ttu-id="f4383-528">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="f4383-528">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-529">SkuId</span><span class="sxs-lookup"><span data-stu-id="f4383-529">SkuId</span></span></td>
<td><p><span data-ttu-id="f4383-530">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="f4383-530">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-531">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f4383-531">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f4383-532">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="f4383-532">The ID for a particular Availability.</span></span> <span data-ttu-id="f4383-533">"Disponibilità" indica se un particolare SKU è disponibile per l'acquisto per il paese, la valuta, il segmento di settore e così via.</span><span class="sxs-lookup"><span data-stu-id="f4383-533">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-534">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="f4383-534">SKU Name</span></span></td>
<td><p><span data-ttu-id="f4383-535">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="f4383-535">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-536">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f4383-536">PublisherName</span></span></td>
<td><p><span data-ttu-id="f4383-537">Nome del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-537">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-538">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f4383-538">PublisherID</span></span></td>
<td><p><span data-ttu-id="f4383-539">ID del server di pubblicazione in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f4383-539">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="f4383-540">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-540">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-541">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-541">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f4383-542">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-542">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f4383-543">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="f4383-543">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-544">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-544">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f4383-545">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f4383-545">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f4383-546">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-546">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f4383-547">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="f4383-547">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-548">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f4383-548">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f4383-549">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="f4383-549">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f4383-550">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="f4383-550">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-551">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f4383-551">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f4383-552">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="f4383-552">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f4383-553">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="f4383-553">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-554">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="f4383-554">Usage Date</span></span></td>
<td><p><span data-ttu-id="f4383-555">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="f4383-555">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-556">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="f4383-556">Meter Type</span></span></td>
<td><p><span data-ttu-id="f4383-557">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="f4383-557">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-558">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="f4383-558">Meter Category</span></span></td>
<td><p><span data-ttu-id="f4383-559">Servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="f4383-559">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-560">ID contatore</span><span class="sxs-lookup"><span data-stu-id="f4383-560">Meter Id</span></span></td>
<td><p><span data-ttu-id="f4383-561">ID del contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="f4383-561">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-562">Sottocategoria contatore</span><span class="sxs-lookup"><span data-stu-id="f4383-562">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="f4383-563">Tipo di servizio di Azure che può influire sulla frequenza.</span><span class="sxs-lookup"><span data-stu-id="f4383-563">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-564">Nome contatore</span><span class="sxs-lookup"><span data-stu-id="f4383-564">Meter Name</span></span></td>
<td><p><span data-ttu-id="f4383-565">Unità di misura per il contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="f4383-565">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-566">Area del contatore</span><span class="sxs-lookup"><span data-stu-id="f4383-566">Meter Region</span></span></td>
<td><p><span data-ttu-id="f4383-567">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="f4383-567">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-568">Unit</span><span class="sxs-lookup"><span data-stu-id="f4383-568">Unit</span></span></td>
<td><p><span data-ttu-id="f4383-569">Unità del nome della risorsa.</span><span class="sxs-lookup"><span data-stu-id="f4383-569">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-570">Quantità utilizzata</span><span class="sxs-lookup"><span data-stu-id="f4383-570">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="f4383-571">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="f4383-571">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="f4383-572">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="f4383-572">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-573">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="f4383-573">Resource Location</span></span></td>
<td><p><span data-ttu-id="f4383-574">Data Center in cui è in esecuzione il contatore.</span><span class="sxs-lookup"><span data-stu-id="f4383-574">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-575">Servizio utilizzato</span><span class="sxs-lookup"><span data-stu-id="f4383-575">Consumed Service</span></span></td>
<td><p><span data-ttu-id="f4383-576">Il servizio della piattaforma Azure usato.</span><span class="sxs-lookup"><span data-stu-id="f4383-576">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="f4383-577">URI risorsa</span><span class="sxs-lookup"><span data-stu-id="f4383-577">Resource URI</span></span></td>
<td><p><span data-ttu-id="f4383-578">URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="f4383-578">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-579">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="f4383-579">Charge type</span></span></td>
<td><p><span data-ttu-id="f4383-580">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="f4383-580">The type of charge or adjustment.</span></span> <span data-ttu-id="f4383-581">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-581">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-582">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="f4383-582">Unit price</span></span></td>
<td><p><span data-ttu-id="f4383-583">Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="f4383-583">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f4383-584">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-585">Quantità</span><span class="sxs-lookup"><span data-stu-id="f4383-585">Quantity</span></span></td>
<td><p><span data-ttu-id="f4383-586">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="f4383-586">Number of licenses.</span></span> <span data-ttu-id="f4383-587">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-587">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-588">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="f4383-588">Unit type</span></span></td>
<td><p><span data-ttu-id="f4383-589">Tipo di unità in cui viene addebitato il contatore.</span><span class="sxs-lookup"><span data-stu-id="f4383-589">The type of unit the meter is charged in.</span></span> <span data-ttu-id="f4383-590">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="f4383-590">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-591">Pre-imposta fatturazione</span><span class="sxs-lookup"><span data-stu-id="f4383-591">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="f4383-592">Importo totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-592">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-593">Valuta fatturazione</span><span class="sxs-lookup"><span data-stu-id="f4383-593">Billing currency</span></span></td>
<td><p><span data-ttu-id="f4383-594">Valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="f4383-594">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-595">Prezzi pretassazione totali</span><span class="sxs-lookup"><span data-stu-id="f4383-595">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="f4383-596">I prezzi prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="f4383-596">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-597">Valuta prezzi</span><span class="sxs-lookup"><span data-stu-id="f4383-597">Pricing currency</span></span></td>
<td><p><span data-ttu-id="f4383-598">Valuta nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="f4383-598">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f4383-599">Informazioni servizio 1</span><span class="sxs-lookup"><span data-stu-id="f4383-599">Service Info 1</span></span></td>
<td><p><span data-ttu-id="f4383-600">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="f4383-600">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-601">Informazioni servizio 2</span><span class="sxs-lookup"><span data-stu-id="f4383-601">Service Info 2</span></span></td>
<td><p><span data-ttu-id="f4383-602">Campo legacy che acquisisce i metadati facoltativi specifici del servizio.</span><span class="sxs-lookup"><span data-stu-id="f4383-602">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f4383-603">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="f4383-603">Additional Info</span></span></td>
<td><p><span data-ttu-id="f4383-604">Eventuali informazioni aggiuntive non incluse in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="f4383-604">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="f4383-605">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="f4383-605">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="f4383-606">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="f4383-606">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="f4383-607">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-607">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="f4383-608">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="f4383-608">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="f4383-609">Uno sconto sui crediti, gli sconti o i rimborsi visualizzati nella fattura come "rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-609">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="f4383-610">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="f4383-610">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="f4383-611"><strong>Descrizione addebito fattura</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-611"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-612"><strong>Descrizione addebito file di riconciliazione (colonna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-612"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-613"><strong>Qual è il costo?</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-613"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-614"><strong>Ricerca per categorie mappare questi ChargeTypes alla fattura?</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-614"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="f4383-615"><strong>Addebiti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-615"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-616">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="f4383-616">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-617">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="f4383-617">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="f4383-618">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-618">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-619">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="f4383-619">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-620">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="f4383-620">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-621">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="f4383-621">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-622">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-622">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-623">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="f4383-623">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-624">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="f4383-624">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-625">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="f4383-625">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-626">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="f4383-626">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-627">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="f4383-627">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-628">Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale</span><span class="sxs-lookup"><span data-stu-id="f4383-628">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-629">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="f4383-629">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-630">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="f4383-630">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-631">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="f4383-631">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-632">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-632">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="f4383-633">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="f4383-633">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-634">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-634">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-635">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="f4383-635">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-636">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="f4383-636">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="f4383-637"><strong>Addebiti monouso</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-637"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="f4383-638">Nuova</span><span class="sxs-lookup"><span data-stu-id="f4383-638">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-639">Utilizzato quando viene creato un nuovo acquisto</span><span class="sxs-lookup"><span data-stu-id="f4383-639">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-640">addQuantity</span><span class="sxs-lookup"><span data-stu-id="f4383-640">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-641">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo l'aumento</span><span class="sxs-lookup"><span data-stu-id="f4383-641">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-642">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="f4383-642">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-643">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo la riduzione</span><span class="sxs-lookup"><span data-stu-id="f4383-643">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-644">Annulla</span><span class="sxs-lookup"><span data-stu-id="f4383-644">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-645">Utilizzato quando viene annullata una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-645">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-646">Convertire</span><span class="sxs-lookup"><span data-stu-id="f4383-646">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-647">Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato</span><span class="sxs-lookup"><span data-stu-id="f4383-647">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="f4383-648"><strong>Addebiti per l'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-648"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-649">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="f4383-649">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-650">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="f4383-650">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="f4383-651">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-651">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-652">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="f4383-652">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-653">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="f4383-653">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="f4383-654"><strong>Crediti</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-654"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-655">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="f4383-655">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-656">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="f4383-656">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-657">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-657">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="f4383-658">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-658">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="f4383-659"><strong>Sconti basati sull'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-659"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-660">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="f4383-660">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-661">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-661">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="f4383-662">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-662">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-663">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="f4383-663">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-664">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="f4383-664">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-665">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="f4383-665">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-666">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="f4383-666">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-667">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="f4383-667">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-668">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="f4383-668">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="f4383-669"><strong>Sconti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-669"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-670"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="f4383-670"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="f4383-671">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-671">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f4383-672"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-672"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-673"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="f4383-673"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="f4383-674"><em>Eccezione: &quot;Offset una voce &quot; include già le imposte. Vedere crediti, sopra.</em></span><span class="sxs-lookup"><span data-stu-id="f4383-674"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-675">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="f4383-675">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="f4383-676">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-676">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="f4383-677">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="f4383-677">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
