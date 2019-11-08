---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753858"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="1052f-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="1052f-103">Use the reconciliation files</span></span>

<span data-ttu-id="1052f-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="1052f-104">**Applies to**</span></span>

-  <span data-ttu-id="1052f-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1052f-105">Partner Center</span></span>
-  <span data-ttu-id="1052f-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="1052f-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1052f-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="1052f-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1052f-108">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="1052f-108">Billing admin</span></span>
- <span data-ttu-id="1052f-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="1052f-109">Global admin</span></span>

<span data-ttu-id="1052f-110">Per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione, scaricare i file di riconciliazione dal centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="1052f-111">I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.</span><span class="sxs-lookup"><span data-stu-id="1052f-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="1052f-112">Problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="1052f-112">Formatting issues</span></span>

<span data-ttu-id="1052f-113">Occasionalmente il file di ricognizione potrebbe avere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="1052f-114">Questo può accadere, ad esempio, se le impostazioni locali EN-US non vengono usate. Per risolvere questi problemi, attenersi alla procedura riportata di seguito.</span><span class="sxs-lookup"><span data-stu-id="1052f-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="1052f-115">Aprire il file CSV in Excel e selezionare la prima colonna.</span><span class="sxs-lookup"><span data-stu-id="1052f-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="1052f-116">Sulla barra multifunzione selezionare <strong>dati</strong>, quindi selezionare <strong>testo in colonne</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="1052f-117">Nella procedura guidata Converti testo in colonne selezionare <strong>tipo di file delimitato</strong>e quindi fare clic su <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="1052f-118">Nel campo delimitatori selezionare <strong>virgola</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="1052f-119">Se la <strong>scheda</strong> è già selezionata, è possibile lasciarla invariata.</span><span class="sxs-lookup"><span data-stu-id="1052f-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="1052f-120">Seleziona <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="1052f-121">Nel campo formato dati colonna selezionare <strong>Data: MDY</strong>, quindi fare clic su <strong>Avanti</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="1052f-122">Nel campo formato dati colonna selezionare <strong>testo</strong> per tutte le colonne importo, quindi fare clic su <strong>fine</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="1052f-123">Download di un file di ricognizione di grandi dimensioni</span><span class="sxs-lookup"><span data-stu-id="1052f-123">Downloading a large recon file</span></span>

<span data-ttu-id="1052f-124">I file di ricognizione possono avere dimensioni molto elevate e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="1052f-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="1052f-125">Per uno script di PowerShell che consente di scaricare file di ricognizione di grandi dimensioni, vedere [ottenere le voci della fattura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="1052f-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="1052f-126">Descrivere per partner</span><span class="sxs-lookup"><span data-stu-id="1052f-126">Itemize by partner</span></span>


<span data-ttu-id="1052f-127">I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.</span><span class="sxs-lookup"><span data-stu-id="1052f-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1052f-128">ID MPN</span><span class="sxs-lookup"><span data-stu-id="1052f-128">MPN ID</span></span></th>
<th><span data-ttu-id="1052f-129">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1052f-130">ID MPN</span><span class="sxs-lookup"><span data-stu-id="1052f-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="1052f-131">ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="1052f-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-132">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="1052f-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="1052f-133">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="1052f-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="1052f-134">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1052f-135">Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="1052f-136">eTo visualizzare o aggiornare il rivenditore, dal menu centro per i partner selezionare <strong>Customers</strong>, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="1052f-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="1052f-137">Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="1052f-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="1052f-138">Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="1052f-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="1052f-139">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="1052f-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="1052f-140">Se un partner CSP ha un rivenditore senza ID MPN, questo valore viene impostato invece sull'ID MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="1052f-141">Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</span><span class="sxs-lookup"><span data-stu-id="1052f-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="1052f-142">Campi di file basati su licenza</span><span class="sxs-lookup"><span data-stu-id="1052f-142">License-based file fields</span></span>


<span data-ttu-id="1052f-143">Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1052f-144"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1052f-145"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1052f-146"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1052f-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="1052f-148">Identificatore univoco per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1052f-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1052f-149">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="1052f-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1052f-150">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="1052f-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="1052f-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="1052f-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1052f-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="1052f-153">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1052f-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="1052f-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="1052f-155">OrderID</span></span></td>
<td><p><span data-ttu-id="1052f-156">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1052f-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1052f-157">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1052f-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1052f-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1052f-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1052f-160">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1052f-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1052f-161">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1052f-162">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="1052f-163">Vedi Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="1052f-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="1052f-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1052f-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="1052f-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="1052f-166">Identificatore univoco per le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="1052f-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="1052f-167">Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="1052f-168">Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1052f-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="1052f-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="1052f-170">OfferID</span></span></td>
<td><p><span data-ttu-id="1052f-171">ID univoco dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="1052f-171">Unique offer ID.</span></span> <span data-ttu-id="1052f-172">ID dell'offerta standard in base al listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="1052f-173"><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="1052f-174">Vedi DurableOfferID di seguito.</span><span class="sxs-lookup"><span data-stu-id="1052f-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="1052f-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="1052f-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="1052f-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="1052f-177">ID dell'offerta durevole univoco, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="1052f-178"><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="1052f-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="1052f-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="1052f-180">OfferName</span></span></td>
<td><p><span data-ttu-id="1052f-181">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="1052f-182">Microsoft Office 365 (Piano E3)</span><span class="sxs-lookup"><span data-stu-id="1052f-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="1052f-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="1052f-184">Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine.</span><span class="sxs-lookup"><span data-stu-id="1052f-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="1052f-185">Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</span><span class="sxs-lookup"><span data-stu-id="1052f-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="1052f-186">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1052f-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1052f-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="1052f-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="1052f-189">Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</span><span class="sxs-lookup"><span data-stu-id="1052f-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="1052f-190">In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="1052f-191">È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</span><span class="sxs-lookup"><span data-stu-id="1052f-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="1052f-192">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1052f-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1052f-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1052f-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1052f-195">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="1052f-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="1052f-196">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="1052f-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1052f-197">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1052f-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1052f-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1052f-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1052f-200">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="1052f-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="1052f-201">Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</span><span class="sxs-lookup"><span data-stu-id="1052f-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1052f-202">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="1052f-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1052f-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="1052f-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1052f-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="1052f-205">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="1052f-205">The type of charge or adjustment.</span></span> <span data-ttu-id="1052f-206">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="1052f-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1052f-207">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="1052f-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="1052f-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="1052f-209">Prezzo per postazione, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="1052f-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1052f-210">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1052f-211">6.82</span><span class="sxs-lookup"><span data-stu-id="1052f-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-212">Quantità</span><span class="sxs-lookup"><span data-stu-id="1052f-212">Quantity</span></span></td>
<td><p><span data-ttu-id="1052f-213">Numero di postazioni.</span><span class="sxs-lookup"><span data-stu-id="1052f-213">Number of seats.</span></span> <span data-ttu-id="1052f-214">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1052f-215">2</span><span class="sxs-lookup"><span data-stu-id="1052f-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-216">Importo</span><span class="sxs-lookup"><span data-stu-id="1052f-216">Amount</span></span></td>
<td><p><span data-ttu-id="1052f-217">Prezzo totale per la quantità.</span><span class="sxs-lookup"><span data-stu-id="1052f-217">Total of price for quantity.</span></span> <span data-ttu-id="1052f-218">Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</span><span class="sxs-lookup"><span data-stu-id="1052f-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="1052f-219">13.32</span><span class="sxs-lookup"><span data-stu-id="1052f-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="1052f-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="1052f-221">Importo dello sconto applicato a questi addebiti.</span><span class="sxs-lookup"><span data-stu-id="1052f-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="1052f-222">Le licenze dei prodotti incluse con una competenza o mappe o nuove sottoscrizioni idonee per un incentivo conterranno anche un importo di sconto in questo articolo.</span><span class="sxs-lookup"><span data-stu-id="1052f-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="1052f-223">2.32</span><span class="sxs-lookup"><span data-stu-id="1052f-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-224">Subtotal</span><span class="sxs-lookup"><span data-stu-id="1052f-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="1052f-225">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-225">Total before tax.</span></span> <span data-ttu-id="1052f-226">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="1052f-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="1052f-227">11</span><span class="sxs-lookup"><span data-stu-id="1052f-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-228">Imposta</span><span class="sxs-lookup"><span data-stu-id="1052f-228">Tax</span></span></td>
<td><p><span data-ttu-id="1052f-229">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="1052f-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1052f-230">0</span><span class="sxs-lookup"><span data-stu-id="1052f-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="1052f-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="1052f-232">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-232">Total after tax.</span></span> <span data-ttu-id="1052f-233">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="1052f-234">11</span><span class="sxs-lookup"><span data-stu-id="1052f-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-235">Currency</span><span class="sxs-lookup"><span data-stu-id="1052f-235">Currency</span></span></td>
<td><p><span data-ttu-id="1052f-236">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-236">Currency type.</span></span> <span data-ttu-id="1052f-237">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="1052f-238">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1052f-239">EUR</span><span class="sxs-lookup"><span data-stu-id="1052f-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1052f-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="1052f-241">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1052f-242">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="1052f-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1052f-243">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="1052f-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-244">MPNID</span></span></td>
<td><p><span data-ttu-id="1052f-245">ID MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="1052f-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="1052f-246">4390934</span><span class="sxs-lookup"><span data-stu-id="1052f-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1052f-248">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1052f-249">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="1052f-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1052f-250">4390934</span><span class="sxs-lookup"><span data-stu-id="1052f-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="1052f-251">DomainName</span></span></td>
<td><p><span data-ttu-id="1052f-252">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1052f-253">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="1052f-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1052f-254">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1052f-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1052f-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1052f-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1052f-257">Nome alternativo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-257">Subscription nickname.</span></span> <span data-ttu-id="1052f-258">Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</span><span class="sxs-lookup"><span data-stu-id="1052f-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="1052f-259">PROGETTO ONLINE</span><span class="sxs-lookup"><span data-stu-id="1052f-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1052f-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1052f-261">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1052f-262">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="1052f-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="1052f-263">PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</span><span class="sxs-lookup"><span data-stu-id="1052f-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="1052f-264">Campi di file basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="1052f-264">Usage-based file fields</span></span>


<span data-ttu-id="1052f-265">Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="1052f-266">I campi seguenti illustrano quali servizi sono stati usati e la tariffa.</span><span class="sxs-lookup"><span data-stu-id="1052f-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1052f-267"><strong>Colonna</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1052f-268"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1052f-269"><strong>Valore di esempio</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="1052f-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="1052f-271">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1052f-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="1052f-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1052f-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1052f-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="1052f-274">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="1052f-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="1052f-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="1052f-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="1052f-277">ID account partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="1052f-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="1052f-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1052f-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="1052f-280">Nome&#39;dell'organizzazione del cliente come indicato nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1052f-281">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="1052f-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1052f-282">Cliente di prova A</span><span class="sxs-lookup"><span data-stu-id="1052f-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-283">MPNID</span></span></td>
<td><p><span data-ttu-id="1052f-284">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="1052f-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="1052f-285">4390934</span><span class="sxs-lookup"><span data-stu-id="1052f-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1052f-287">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1052f-288">Vedi <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Eseguire la scomposizione dei dati in base al partner</a>.</span><span class="sxs-lookup"><span data-stu-id="1052f-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1052f-289">4390934</span><span class="sxs-lookup"><span data-stu-id="1052f-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1052f-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1052f-291">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="1052f-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="1052f-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="1052f-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1052f-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1052f-294">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="1052f-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1052f-295">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1052f-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1052f-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1052f-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1052f-298">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="1052f-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1052f-299">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="1052f-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1052f-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="1052f-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1052f-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1052f-302">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1052f-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1052f-303">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1052f-304">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1052f-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1052f-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1052f-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1052f-307">Nome alternativo dell'offerta di servizio.</span><span class="sxs-lookup"><span data-stu-id="1052f-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="1052f-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1052f-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1052f-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1052f-310">Line-of-business dell'offerta di servizio</span><span class="sxs-lookup"><span data-stu-id="1052f-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="1052f-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1052f-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="1052f-312">OrderID</span></span></td>
<td><p><span data-ttu-id="1052f-313">Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1052f-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1052f-314">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1052f-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1052f-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="1052f-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="1052f-317">Nome del servizio di Azure in questione.</span><span class="sxs-lookup"><span data-stu-id="1052f-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="1052f-318">MACCHINE VIRTUALI</span><span class="sxs-lookup"><span data-stu-id="1052f-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="1052f-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="1052f-320">Tipo specifico di servizio di Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="1052f-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1052f-321">Bus di servizio-singolo o Pack</span><span class="sxs-lookup"><span data-stu-id="1052f-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="1052f-322">SQL Azure database-Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="1052f-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="1052f-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="1052f-324">Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</span><span class="sxs-lookup"><span data-stu-id="1052f-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="1052f-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1052f-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-326">Resource Name</span><span class="sxs-lookup"><span data-stu-id="1052f-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="1052f-327">Nome della risorsa Azure.</span><span class="sxs-lookup"><span data-stu-id="1052f-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1052f-328">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="1052f-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="1052f-329">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="1052f-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-330">Area geografica</span><span class="sxs-lookup"><span data-stu-id="1052f-330">Region</span></span></td>
<td><p><span data-ttu-id="1052f-331">Area geografica a cui si applica l'uso.</span><span class="sxs-lookup"><span data-stu-id="1052f-331">The region the usage applies to.</span></span> <span data-ttu-id="1052f-332">Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="1052f-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="1052f-333">Asia Pacifico, Europa, America Latina, America del Nord</span><span class="sxs-lookup"><span data-stu-id="1052f-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-334">SKU</span><span class="sxs-lookup"><span data-stu-id="1052f-334">SKU</span></span></td>
<td><p><span data-ttu-id="1052f-335">Identificatore univoco MSFT per l'offerta</span><span class="sxs-lookup"><span data-stu-id="1052f-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="1052f-336">7UD-00001</span><span class="sxs-lookup"><span data-stu-id="1052f-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1052f-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="1052f-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="1052f-338">ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="1052f-339">Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</span><span class="sxs-lookup"><span data-stu-id="1052f-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="1052f-340">1</span><span class="sxs-lookup"><span data-stu-id="1052f-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="1052f-342">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="1052f-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="1052f-343">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="1052f-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="1052f-344">11</span><span class="sxs-lookup"><span data-stu-id="1052f-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="1052f-346">Unità incluse nell'ambito dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="1052f-346">Units included as part of the offer.</span></span> <span data-ttu-id="1052f-347">In genere non presente in CSP.</span><span class="sxs-lookup"><span data-stu-id="1052f-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="1052f-348">0</span><span class="sxs-lookup"><span data-stu-id="1052f-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1052f-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="1052f-350">Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="1052f-351">Uguale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="1052f-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="1052f-352">11</span><span class="sxs-lookup"><span data-stu-id="1052f-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="1052f-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="1052f-354">Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="1052f-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="1052f-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="1052f-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="1052f-357">ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</span><span class="sxs-lookup"><span data-stu-id="1052f-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1052f-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="1052f-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="1052f-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="1052f-360">Addebito IVA, in base alle regole&#39;fiscali del mercato e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="1052f-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1052f-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="1052f-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="1052f-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="1052f-363">Totale al netto delle imposte, se le imposte sono applicabili.</span><span class="sxs-lookup"><span data-stu-id="1052f-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="1052f-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="1052f-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-365">Currency</span><span class="sxs-lookup"><span data-stu-id="1052f-365">Currency</span></span></td>
<td><p><span data-ttu-id="1052f-366">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-366">Currency type.</span></span> <span data-ttu-id="1052f-367">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="1052f-368">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1052f-369">EUR</span><span class="sxs-lookup"><span data-stu-id="1052f-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1052f-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1052f-371">Prezzo unitario prima dell'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-371">Pretax price per unit.</span></span> <span data-ttu-id="1052f-372">Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="1052f-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1052f-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="1052f-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1052f-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1052f-375">Prezzo unitario dopo l'applicazione delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-375">Post tax price per unit.</span></span> <span data-ttu-id="1052f-376">Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</span><span class="sxs-lookup"><span data-stu-id="1052f-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1052f-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="1052f-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1052f-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="1052f-379">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="1052f-379">The type of charge or adjustment.</span></span> <span data-ttu-id="1052f-380">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="1052f-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1052f-381">Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></span><span class="sxs-lookup"><span data-stu-id="1052f-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="1052f-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="1052f-383">ID account univoco nella piattaforma di fatturazione MSFT.</span><span class="sxs-lookup"><span data-stu-id="1052f-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="1052f-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="1052f-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="1052f-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="1052f-386">Data di distribuzione del servizio.</span><span class="sxs-lookup"><span data-stu-id="1052f-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="1052f-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1052f-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="1052f-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="1052f-389">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="1052f-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="1052f-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="1052f-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="1052f-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="1052f-392">Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="1052f-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="1052f-393">I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name.</span><span class="sxs-lookup"><span data-stu-id="1052f-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="1052f-394">La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="1052f-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="1052f-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="1052f-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="1052f-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="1052f-397">Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="1052f-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="1052f-398">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="1052f-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-399">Project</span><span class="sxs-lookup"><span data-stu-id="1052f-399">Project</span></span></td>
<td><p><span data-ttu-id="1052f-400">Nome definito dal cliente per l'istanza del servizio</span><span class="sxs-lookup"><span data-stu-id="1052f-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="1052f-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1052f-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="1052f-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="1052f-403">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="1052f-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="1052f-404">Ad esempio, se si dispone di una connessione di cui è stato effettuato il provisioning individualmente durante un mese di 30 giorni, Service Info 1 leggerà "1,000000 connessioni/30 giorni".</span><span class="sxs-lookup"><span data-stu-id="1052f-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="1052f-405">Se è stato effettuato il provisioning di un pacchetto di 25 connessioni ServiceBus e l'utilizzo di 1 durante tale giorno, l'utilizzo giornaliero per quel giorno indicherebbe "25 connessioni/30 giorni-usato: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="1052f-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1052f-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="1052f-407">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1052f-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1052f-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="1052f-409">DomainName</span></span></td>
<td><p><span data-ttu-id="1052f-410">Nome&#39;di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1052f-411">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1052f-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1052f-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-413">Unit</span><span class="sxs-lookup"><span data-stu-id="1052f-413">Unit</span></span></td>
<td><p><span data-ttu-id="1052f-414">Nome dell'unità della risorsa</span><span class="sxs-lookup"><span data-stu-id="1052f-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="1052f-415">GB o ORE</span><span class="sxs-lookup"><span data-stu-id="1052f-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="1052f-416">Campi di file una sola volta e ricorrenti</span><span class="sxs-lookup"><span data-stu-id="1052f-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1052f-417">Column</span><span class="sxs-lookup"><span data-stu-id="1052f-417">Column</span></span></th>
<th><span data-ttu-id="1052f-418">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="1052f-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1052f-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="1052f-420">Identificatore univoco del tenant Microsoft Azure Active Directory per un'entità di fatturazione specifica, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1052f-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1052f-421">Non è necessario per la riconciliazione, ma può risultare utile.</span><span class="sxs-lookup"><span data-stu-id="1052f-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1052f-422">È lo stesso per tutte le righe.</span><span class="sxs-lookup"><span data-stu-id="1052f-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-423">ID cliente</span><span class="sxs-lookup"><span data-stu-id="1052f-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="1052f-424">Univoco Microsoft Azure Active Directory ID tenant, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-425">Nome cliente</span><span class="sxs-lookup"><span data-stu-id="1052f-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="1052f-426">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1052f-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1052f-428">Nome di dominio del cliente, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="1052f-429">Questo non deve essere usato per identificare in modo univoco il cliente, perché il cliente/partner può aggiornare il dominio Vanity/default tramite il portale O365.</span><span class="sxs-lookup"><span data-stu-id="1052f-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1052f-430">Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-431">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="1052f-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="1052f-432">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-433">Numero fattura</span><span class="sxs-lookup"><span data-stu-id="1052f-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="1052f-434">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="1052f-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="1052f-435">MpnId</span></span></td>
<td><p><span data-ttu-id="1052f-436">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="1052f-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-437">Rivenditore MpnId</span><span class="sxs-lookup"><span data-stu-id="1052f-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="1052f-438">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-439">ID ordine</span><span class="sxs-lookup"><span data-stu-id="1052f-439">Order ID</span></span></td>
<td><p><span data-ttu-id="1052f-440">Identificatore univoco per un ordine in Microsoft Commerce platform.</span><span class="sxs-lookup"><span data-stu-id="1052f-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="1052f-441">Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-442">Data ordine</span><span class="sxs-lookup"><span data-stu-id="1052f-442">Order date</span></span></td>
<td><p><span data-ttu-id="1052f-443">Data di effettuazione dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="1052f-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="1052f-444">ProductId</span></span></td>
<td><p><span data-ttu-id="1052f-445">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="1052f-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="1052f-446">SkuId</span></span></td>
<td><p><span data-ttu-id="1052f-447">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="1052f-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1052f-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1052f-449">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="1052f-449">The ID for a particular Availability.</span></span> <span data-ttu-id="1052f-450">"Disponibilità" indica se un particolare SKU è disponibile per l'acquisto per il paese, la valuta, il segmento di settore e così via.</span><span class="sxs-lookup"><span data-stu-id="1052f-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-451">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="1052f-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="1052f-452">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="1052f-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-453">Nome del prodotto</span><span class="sxs-lookup"><span data-stu-id="1052f-453">Product name</span></span></td>
<td><p><span data-ttu-id="1052f-454">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="1052f-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1052f-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="1052f-456">Nome del server di pubblicazione del prodotto.</span><span class="sxs-lookup"><span data-stu-id="1052f-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1052f-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="1052f-458">ID univoco per questo server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-459">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1052f-460">Nome descrittivo di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-461">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1052f-462">Identificatore univoco per una sottoscrizione nella piattaforma Microsoft Commerce.</span><span class="sxs-lookup"><span data-stu-id="1052f-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="1052f-463">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1052f-464">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1052f-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1052f-466">Giorno di inizio degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="1052f-466">Start day of the charges.</span></span> <span data-ttu-id="1052f-467">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1052f-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1052f-469">Giorno di fine degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="1052f-469">End day of the charges.</span></span> <span data-ttu-id="1052f-470">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="1052f-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-471">Termini e billingcycle</span><span class="sxs-lookup"><span data-stu-id="1052f-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="1052f-472">Durata e ciclo di fatturazione per l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="1052f-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="1052f-473">Ad esempio, "1 anno, mensile".</span><span class="sxs-lookup"><span data-stu-id="1052f-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-474">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="1052f-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="1052f-475">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="1052f-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-476">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="1052f-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="1052f-477">Prezzo pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="1052f-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1052f-478">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-479">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="1052f-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="1052f-480">Prezzo unitario dopo le rettifiche apportate.</span><span class="sxs-lookup"><span data-stu-id="1052f-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-481">Quantità</span><span class="sxs-lookup"><span data-stu-id="1052f-481">Quantity</span></span></td>
<td><p><span data-ttu-id="1052f-482">Numero di unità.</span><span class="sxs-lookup"><span data-stu-id="1052f-482">Number of units.</span></span> <span data-ttu-id="1052f-483">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-484">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="1052f-484">Unit type</span></span></td>
<td><p><span data-ttu-id="1052f-485">Tipo di unità da acquistare.</span><span class="sxs-lookup"><span data-stu-id="1052f-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="1052f-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="1052f-487">Spiegazione di qualsiasi sconto applicabile.</span><span class="sxs-lookup"><span data-stu-id="1052f-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-488">Totale parziale</span><span class="sxs-lookup"><span data-stu-id="1052f-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="1052f-489">Totale al lordo delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-489">Total before tax.</span></span> <span data-ttu-id="1052f-490">Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</span><span class="sxs-lookup"><span data-stu-id="1052f-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-491">Imposta totale</span><span class="sxs-lookup"><span data-stu-id="1052f-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="1052f-492">Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</span><span class="sxs-lookup"><span data-stu-id="1052f-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-493">Totale</span><span class="sxs-lookup"><span data-stu-id="1052f-493">Total</span></span></td>
<td><p><span data-ttu-id="1052f-494">Totale al netto delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-494">Total after tax.</span></span> <span data-ttu-id="1052f-495">Verifica se nella fattura sono addebitate imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-496">Currency</span><span class="sxs-lookup"><span data-stu-id="1052f-496">Currency</span></span></td>
<td><p><span data-ttu-id="1052f-497">Tipo di valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-497">Currency type.</span></span> <span data-ttu-id="1052f-498">Ogni entità di fatturazione ha una sola valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="1052f-499">Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="1052f-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="1052f-501">Identificatore alternativo a un ID dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="1052f-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="1052f-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="1052f-503">Visualizza mensilmente quando è abilitata la fatturazione mensile.</span><span class="sxs-lookup"><span data-stu-id="1052f-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="1052f-504">Altrimenti vuoto.</span><span class="sxs-lookup"><span data-stu-id="1052f-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="1052f-506">Rappresenta le unità totali acquistate o utilizzate.</span><span class="sxs-lookup"><span data-stu-id="1052f-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-507">pricingCurrency</span><span class="sxs-lookup"><span data-stu-id="1052f-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="1052f-508">Elenca il prezzo per la risorsa o l'offerta</span><span class="sxs-lookup"><span data-stu-id="1052f-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="1052f-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="1052f-510">Tasso di cambio applicato per la valuta tariffaria (clienti)</span><span class="sxs-lookup"><span data-stu-id="1052f-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="1052f-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="1052f-512">Data in cui è determinata la valuta tariffaria per il tasso di cambio di valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="1052f-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="1052f-514">Descrizione contatore per l'elemento della riga consumo</span><span class="sxs-lookup"><span data-stu-id="1052f-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="1052f-515">Campi del file di utilizzo con classificazione giornaliera</span><span class="sxs-lookup"><span data-stu-id="1052f-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1052f-516">Column</span><span class="sxs-lookup"><span data-stu-id="1052f-516">Column</span></span></th>
<th><span data-ttu-id="1052f-517">Descrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="1052f-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1052f-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="1052f-519">ID del partner, in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1052f-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1052f-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="1052f-521">Nome partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="1052f-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="1052f-523">ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="1052f-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="1052f-525">Nome dell'organizzazione del cliente registrato nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1052f-526">Molto importante per la riconciliazione della fattura con le informazioni di sistema.</span><span class="sxs-lookup"><span data-stu-id="1052f-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1052f-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1052f-528">Nome di dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-528">The customer's domain name.</span></span> <span data-ttu-id="1052f-529">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-530">Paese del cliente</span><span class="sxs-lookup"><span data-stu-id="1052f-530">Customer country</span></span></td>
<td><p><span data-ttu-id="1052f-531">Paese in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="1052f-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-532">MPNID</span></span></td>
<td><p><span data-ttu-id="1052f-533">ID MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="1052f-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-534">Rivenditore MPNID</span><span class="sxs-lookup"><span data-stu-id="1052f-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="1052f-535">ID MPN del rivenditore nel record per la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1052f-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1052f-536">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1052f-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1052f-538">Numero di fattura in cui viene visualizzata la transazione specificata.</span><span class="sxs-lookup"><span data-stu-id="1052f-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="1052f-539">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="1052f-540">ProductId</span></span></td>
<td><p><span data-ttu-id="1052f-541">ID del prodotto.</span><span class="sxs-lookup"><span data-stu-id="1052f-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="1052f-542">SkuId</span></span></td>
<td><p><span data-ttu-id="1052f-543">ID di una SKU particolare.</span><span class="sxs-lookup"><span data-stu-id="1052f-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1052f-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1052f-545">ID di una disponibilità particolare.</span><span class="sxs-lookup"><span data-stu-id="1052f-545">The ID for a particular Availability.</span></span> <span data-ttu-id="1052f-546">"Disponibilità" indica se un particolare SKU è disponibile per l'acquisto per il paese, la valuta, il segmento di settore e così via.</span><span class="sxs-lookup"><span data-stu-id="1052f-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-547">Nome SKU</span><span class="sxs-lookup"><span data-stu-id="1052f-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="1052f-548">Titolo di una particolare SKU.</span><span class="sxs-lookup"><span data-stu-id="1052f-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1052f-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="1052f-550">Nome del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1052f-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="1052f-552">ID del server di pubblicazione in formato GUID.</span><span class="sxs-lookup"><span data-stu-id="1052f-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="1052f-553">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-554">Descrizione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1052f-555">Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1052f-556">Questo è un campo identico a Nome offerta.</span><span class="sxs-lookup"><span data-stu-id="1052f-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-557">ID sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1052f-558">Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1052f-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1052f-559">Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1052f-560">Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</span><span class="sxs-lookup"><span data-stu-id="1052f-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1052f-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1052f-562">Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="1052f-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1052f-563">L'ora indicata è sempre l'inizio della giornata, le 0:00.</span><span class="sxs-lookup"><span data-stu-id="1052f-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1052f-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1052f-565">Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</span><span class="sxs-lookup"><span data-stu-id="1052f-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1052f-566">L'ora indicata è sempre la fine della giornata, le 23:59.</span><span class="sxs-lookup"><span data-stu-id="1052f-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-567">Data di utilizzo</span><span class="sxs-lookup"><span data-stu-id="1052f-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="1052f-568">Data di utilizzo del servizio.</span><span class="sxs-lookup"><span data-stu-id="1052f-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-569">Tipo di misuratore</span><span class="sxs-lookup"><span data-stu-id="1052f-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="1052f-570">Tipo di misuratore.</span><span class="sxs-lookup"><span data-stu-id="1052f-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-571">Categoria misuratore</span><span class="sxs-lookup"><span data-stu-id="1052f-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="1052f-572">Servizio di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="1052f-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-573">ID contatore</span><span class="sxs-lookup"><span data-stu-id="1052f-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="1052f-574">ID del contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="1052f-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-575">Sottocategoria contatore</span><span class="sxs-lookup"><span data-stu-id="1052f-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="1052f-576">Tipo di servizio di Azure che può influire sulla frequenza.</span><span class="sxs-lookup"><span data-stu-id="1052f-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-577">Nome contatore</span><span class="sxs-lookup"><span data-stu-id="1052f-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="1052f-578">Unità di misura per il contatore utilizzato.</span><span class="sxs-lookup"><span data-stu-id="1052f-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-579">Area del contatore</span><span class="sxs-lookup"><span data-stu-id="1052f-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="1052f-580">Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</span><span class="sxs-lookup"><span data-stu-id="1052f-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-581">Unit</span><span class="sxs-lookup"><span data-stu-id="1052f-581">Unit</span></span></td>
<td><p><span data-ttu-id="1052f-582">Unità del nome della risorsa.</span><span class="sxs-lookup"><span data-stu-id="1052f-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-583">Quantità utilizzata</span><span class="sxs-lookup"><span data-stu-id="1052f-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="1052f-584">La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</span><span class="sxs-lookup"><span data-stu-id="1052f-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="1052f-585">Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</span><span class="sxs-lookup"><span data-stu-id="1052f-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-586">Percorso della risorsa</span><span class="sxs-lookup"><span data-stu-id="1052f-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="1052f-587">Data Center in cui è in esecuzione il contatore.</span><span class="sxs-lookup"><span data-stu-id="1052f-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-588">Servizio utilizzato</span><span class="sxs-lookup"><span data-stu-id="1052f-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="1052f-589">Il servizio della piattaforma Azure usato.</span><span class="sxs-lookup"><span data-stu-id="1052f-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="1052f-590">URI risorsa</span><span class="sxs-lookup"><span data-stu-id="1052f-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="1052f-591">URI della risorsa in uso.</span><span class="sxs-lookup"><span data-stu-id="1052f-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-592">Tipo di addebito</span><span class="sxs-lookup"><span data-stu-id="1052f-592">Charge type</span></span></td>
<td><p><span data-ttu-id="1052f-593">Tipo di addebito o rettifica.</span><span class="sxs-lookup"><span data-stu-id="1052f-593">The type of charge or adjustment.</span></span> <span data-ttu-id="1052f-594">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-595">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="1052f-595">Unit price</span></span></td>
<td><p><span data-ttu-id="1052f-596">Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto.</span><span class="sxs-lookup"><span data-stu-id="1052f-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1052f-597">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-598">Quantità</span><span class="sxs-lookup"><span data-stu-id="1052f-598">Quantity</span></span></td>
<td><p><span data-ttu-id="1052f-599">Numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="1052f-599">Number of licenses.</span></span> <span data-ttu-id="1052f-600">Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-601">Tipo di unità</span><span class="sxs-lookup"><span data-stu-id="1052f-601">Unit type</span></span></td>
<td><p><span data-ttu-id="1052f-602">Tipo di unità in cui viene addebitato il contatore.</span><span class="sxs-lookup"><span data-stu-id="1052f-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="1052f-603">Non disponibile per l'attività corrente.</span><span class="sxs-lookup"><span data-stu-id="1052f-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-604">Pre-imposta fatturazione</span><span class="sxs-lookup"><span data-stu-id="1052f-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="1052f-605">Importo totale prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-606">Valuta fatturazione</span><span class="sxs-lookup"><span data-stu-id="1052f-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="1052f-607">Valuta nell'area geografica del cliente</span><span class="sxs-lookup"><span data-stu-id="1052f-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-608">Prezzi pretassazione totali</span><span class="sxs-lookup"><span data-stu-id="1052f-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="1052f-609">I prezzi prima dell'aggiunta delle imposte.</span><span class="sxs-lookup"><span data-stu-id="1052f-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-610">Valuta prezzi</span><span class="sxs-lookup"><span data-stu-id="1052f-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="1052f-611">Valuta nel listino prezzi.</span><span class="sxs-lookup"><span data-stu-id="1052f-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-612">Informazioni servizio 1</span><span class="sxs-lookup"><span data-stu-id="1052f-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="1052f-613">Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</span><span class="sxs-lookup"><span data-stu-id="1052f-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1052f-614">Informazioni servizio 2</span><span class="sxs-lookup"><span data-stu-id="1052f-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="1052f-615">Campo legacy che acquisisce i metadati facoltativi specifici del servizio.</span><span class="sxs-lookup"><span data-stu-id="1052f-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1052f-616">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="1052f-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="1052f-617">Eventuali informazioni aggiuntive non incluse in altre colonne.</span><span class="sxs-lookup"><span data-stu-id="1052f-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="1052f-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="1052f-619">Valore effettivo addebitato per unità (inclusi sconti, credito guadagnato e così via).</span><span class="sxs-lookup"><span data-stu-id="1052f-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="1052f-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="1052f-621">Tasso di cambio applicato per la valuta tariffaria (clienti).</span><span class="sxs-lookup"><span data-stu-id="1052f-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="1052f-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="1052f-623">Data in cui è determinata la valuta tariffaria per il tasso di cambio di valuta.</span><span class="sxs-lookup"><span data-stu-id="1052f-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1052f-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="1052f-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="1052f-625">Rappresenta il subscriptionID di Azure.</span><span class="sxs-lookup"><span data-stu-id="1052f-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1052f-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="1052f-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="1052f-627">Rappresenta il nome della sottoscrizione di Azure.</span><span class="sxs-lookup"><span data-stu-id="1052f-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="1052f-628">Mapping degli addebiti tra una fattura e il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="1052f-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="1052f-629">La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="1052f-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="1052f-630">Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="1052f-631">I file di riconciliazione, sia basati sull'utilizzo che basati su licenza, mostrano solo transazioni e addebiti correlati all'utilizzo (unità consumate e costi correlati).</span><span class="sxs-lookup"><span data-stu-id="1052f-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="1052f-632">Uno sconto sui crediti, gli sconti o i rimborsi visualizzati nella fattura come "rettifiche" non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="1052f-633">Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1052f-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="1052f-634"><strong>Descrizione addebito fattura</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-635"><strong>Descrizione addebito file di riconciliazione (colonna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-636"><strong>Qual è il costo?</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-637"><strong>Ricerca per categorie mappare questi ChargeTypes alla fattura?</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="1052f-638"><strong>Addebiti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-639">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="1052f-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-640">L'importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto</span><span class="sxs-lookup"><span data-stu-id="1052f-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="1052f-641">Dal file in base alle licenze, somma la colonna <strong>Amount</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-642">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="1052f-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-643">Addebiti ripartiti proporzionalmente rimborsati al cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="1052f-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-644">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="1052f-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-645">Addebiti periodici per una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-646">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="1052f-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-647">Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</span><span class="sxs-lookup"><span data-stu-id="1052f-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-648">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="1052f-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-649">Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</span><span class="sxs-lookup"><span data-stu-id="1052f-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-650">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="1052f-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-651">Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale</span><span class="sxs-lookup"><span data-stu-id="1052f-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-652">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="1052f-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-653">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile</span><span class="sxs-lookup"><span data-stu-id="1052f-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-654">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="1052f-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-655">Tariffe rateizzate al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="1052f-656">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="1052f-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-657">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-658">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="1052f-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-659">Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="1052f-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="1052f-660"><strong>Addebiti monouso</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="1052f-661">Nuova</span><span class="sxs-lookup"><span data-stu-id="1052f-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-662">Utilizzato quando viene creato un nuovo acquisto</span><span class="sxs-lookup"><span data-stu-id="1052f-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-664">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo l'aumento</span><span class="sxs-lookup"><span data-stu-id="1052f-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="1052f-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-666">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo la riduzione</span><span class="sxs-lookup"><span data-stu-id="1052f-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-667">Annulla</span><span class="sxs-lookup"><span data-stu-id="1052f-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-668">Utilizzato quando viene annullata una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-669">Convertire</span><span class="sxs-lookup"><span data-stu-id="1052f-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-670">Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato</span><span class="sxs-lookup"><span data-stu-id="1052f-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="1052f-671"><strong>Addebiti per l'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-672">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="1052f-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-673">Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="1052f-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="1052f-674">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-675">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="1052f-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-676">Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</span><span class="sxs-lookup"><span data-stu-id="1052f-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="1052f-677"><strong>Crediti</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-678">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="1052f-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-679">Rimborso parziale o totale per una voce, comprese le imposte</span><span class="sxs-lookup"><span data-stu-id="1052f-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-680">Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="1052f-681">Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="1052f-682"><strong>Sconti basati sull'utilizzo</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-683">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="1052f-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-684">Sconto applicato all'attivazione della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="1052f-685">Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-686">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="1052f-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-687">Sconto applicato su addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="1052f-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-688">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="1052f-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-689">Sconto applicato al rinnovo della sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1052f-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-690">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="1052f-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-691">Addebiti applicati all'annullamento degli sconti</span><span class="sxs-lookup"><span data-stu-id="1052f-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="1052f-692"><strong>Sconti basati su licenza</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-693"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="1052f-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="1052f-694">Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1052f-695"><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-696"><em>Può essere applicato a più tipi di addebito</em></span><span class="sxs-lookup"><span data-stu-id="1052f-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="1052f-697"><em>Eccezione: &quot;Offset una voce &quot; include già le imposte. Vedere crediti, sopra.</em></span><span class="sxs-lookup"><span data-stu-id="1052f-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-698">Imposte o imposte sul valore aggiunto (IVA)</span><span class="sxs-lookup"><span data-stu-id="1052f-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="1052f-699">Dal file in base alle licenze, somma la colonna <strong>Tax</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="1052f-700">Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></span><span class="sxs-lookup"><span data-stu-id="1052f-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
