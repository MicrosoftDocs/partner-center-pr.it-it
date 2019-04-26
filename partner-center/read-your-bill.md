---
title: Leggere la fattura | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
description: La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel centro per i Partner.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione abbonamenti, fatturazione, fatturazione nel centro per i partner, centri per i partner fatturazione, leggere la fattura, fattura, fattura del centro per i partner, fattura CSP, dove è la fattura?
ms.localizationpriority: medium
ms.openlocfilehash: 9754127cf02d8c8a1098d4a3045b8960978483cc
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133961"
---
# <a name="read-your-bill"></a><span data-ttu-id="53a96-105">Leggere la fattura</span><span class="sxs-lookup"><span data-stu-id="53a96-105">Read your bill</span></span>

<span data-ttu-id="53a96-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="53a96-106">**Applies to**</span></span>

-  <span data-ttu-id="53a96-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="53a96-107">Partner Center</span></span>
-  <span data-ttu-id="53a96-108">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="53a96-108">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="53a96-109">Per la fattura, visitare il **Centro per i Partner** menu e quindi selezionare **fatturazione** per visualizzare la cronologia di fatturazione e le tendenze, collegamenti a file di riconciliazione e fatturazione e il pagamento più recente.</span><span class="sxs-lookup"><span data-stu-id="53a96-109">For your bill, go to the **Partner Center** menu and then select **Billing** to see your billing history and trends, links to your invoice and reconciliation file, and your most recent payment.</span></span>

<span data-ttu-id="53a96-110">I partner del programma Cloud Solution Provider che hanno scelto la fatturazione mensile pagheranno Microsoft per gli abbonamenti dei clienti (sia in base a licenza che in base all'uso) in via posticipata, dopo 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="53a96-110">Partners in the Cloud Solution Provider program who have chosen to be billed monthly pay Microsoft 60 days in arrears for their customers' subscriptions (both license-based and usage-based).</span></span>

> [!NOTE]  
> <span data-ttu-id="53a96-111">La fattura è riportato un riepilogo di tutti gli addebiti, attraverso il programma, i prodotti e clienti, per il periodo di fatturazione corrente ed è disponibile entro due (2) della data di fatturazione selezionata in formato UTC.</span><span class="sxs-lookup"><span data-stu-id="53a96-111">Your invoice is a summary of all charges -- across the program, products, and customers -- for the current billing period and is available within two (2) days of your selected billing date in UTC time.</span></span> <span data-ttu-id="53a96-112">Ad esempio, se hai il 12 settembre data di fatturazione, il processo di generazione della fattura verrà iniziano alle 12:00 AM UTC nel 13 e completare da 12:00 AM UTC su 14.</span><span class="sxs-lookup"><span data-stu-id="53a96-112">For example, if you have a September 12th billing date, the invoice generation process will begin at 12:00AM UTC on the 13th and complete by 12:00AM UTC on the 14th.</span></span> <span data-ttu-id="53a96-113">Se non è possibile visualizzare la fattura da 11 alle 23.59.59 UTC il giorno 15, vengono all'esterno del contratto di servizio, che deve inviare una richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="53a96-113">If you do not see your invoice by 11:59PM UTC on the 15th, you’re out of your Service Level Agreement and should file a service request.</span></span> 

<span data-ttu-id="53a96-114">Riceverai una fattura per gli addebiti basati sulla licenza (Office365) e basati sull'utilizzo (Azure) e una fattura separata per addebiti una tantum (istanze di macchina virtuale riservate di Azure).</span><span class="sxs-lookup"><span data-stu-id="53a96-114">You will receive one invoice for license-based (Office365) and usage-based (Azure) charges, and a separate invoice for one-time (Azure reserved VM instances) charges.</span></span>

<span data-ttu-id="53a96-115">Per i dettagli sugli addebiti, consulta i file di riconciliazione associati.</span><span class="sxs-lookup"><span data-stu-id="53a96-115">For itemized details about the charges, use the accompanying reconciliation files.</span></span> <span data-ttu-id="53a96-116">I file di riconciliazione includono gli ID dei clienti e gli ID delle sottoscrizioni che userai per creare le fatture per i clienti.</span><span class="sxs-lookup"><span data-stu-id="53a96-116">The reconciliation files include the customer IDs and subscription IDs that you will use to create customer invoices.</span></span> <span data-ttu-id="53a96-117">Per altre informazioni, vedi [Come usare i file di riconciliazione](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="53a96-117">For more information, see [How to use the reconciliation files](use-the-reconciliation-files.md).</span></span>

## <a name="invoice-file-definitions"></a><span data-ttu-id="53a96-118">Definizioni del file di fatturazione</span><span class="sxs-lookup"><span data-stu-id="53a96-118">Invoice file definitions</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="53a96-119"><strong>Campo</strong></span><span class="sxs-lookup"><span data-stu-id="53a96-119"><strong>Field</strong></span></span></td>
<td><span data-ttu-id="53a96-120"><strong>Descrizione</strong></span><span class="sxs-lookup"><span data-stu-id="53a96-120"><strong>Description</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-121">US FEIN</span><span class="sxs-lookup"><span data-stu-id="53a96-121">US FEIN</span></span></td>
<td><span data-ttu-id="53a96-122">ID fiscale federale.</span><span class="sxs-lookup"><span data-stu-id="53a96-122">Your Federal Tax ID Number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-123">Numero cliente</span><span class="sxs-lookup"><span data-stu-id="53a96-123">Customer number</span></span></td>
<td><span data-ttu-id="53a96-124">Codice del cliente.</span><span class="sxs-lookup"><span data-stu-id="53a96-124">Your customer number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-125">Indirizzo fatturazione</span><span class="sxs-lookup"><span data-stu-id="53a96-125">Bill to</span></span></td>
<td><span data-ttu-id="53a96-126">Indirizzo a cui inviare la fattura.</span><span class="sxs-lookup"><span data-stu-id="53a96-126">The address where we send your invoice.</span></span> <span data-ttu-id="53a96-127">Per modificare il nome della società o l'indirizzo, modificare il centro per i Partner del profilo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53a96-127">To change the company name or address, edit your Partner Center billing profile.</span></span> </td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-128">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="53a96-128">License-based charges</span></span></td>
<td><span data-ttu-id="53a96-129">Gli addebiti fissi mensili o annuali per le licenze in base all'uso acquistate, fatturati prima del servizio.</span><span class="sxs-lookup"><span data-stu-id="53a96-129">The flat monthly (or annual) charges for the purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="53a96-130">Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</span><span class="sxs-lookup"><span data-stu-id="53a96-130">This number is the sum of all charges in the &quot;Subtotal&quot; column in the License-based reconciliation file (column T).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-131">Addebiti basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="53a96-131">Usage-based charges</span></span></td>
<td><span data-ttu-id="53a96-132">Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53a96-132">Azure usage, including new services or applications enabled and used during the billing month.</span></span> <span data-ttu-id="53a96-133">Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</span><span class="sxs-lookup"><span data-stu-id="53a96-133">This number is the sum of all charges in the &quot;PretaxCharges&quot; column in the Usage-based reconciliation file (column Z).</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-134">Sconti</span><span class="sxs-lookup"><span data-stu-id="53a96-134">Discounts</span></span></td>
<td><span data-ttu-id="53a96-135">Ad esempio lo sconto che il cliente riceve sul prezzo normale della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="53a96-135">For example, the discount that the customer receives from the normal price of the subscription.</span></span> <span data-ttu-id="53a96-136">Lo sconto viene indicato come importo unico, non come prezzo per unità o licenza.</span><span class="sxs-lookup"><span data-stu-id="53a96-136">This is shown as a flat amount, not as a price per unit or license.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-137">Crediti</span><span class="sxs-lookup"><span data-stu-id="53a96-137">Credits</span></span></td>
<td><span data-ttu-id="53a96-138">Crediti o rettifiche per modifiche apportate alle sottoscrizioni, ad esempio aumento o riduzione delle postazioni.</span><span class="sxs-lookup"><span data-stu-id="53a96-138">Credits or adjustments for changes made to subscriptions (example: seat increases or decreases).</span></span></td>
</tr>
<tr class="even">
<tr class="even">
<td><span data-ttu-id="53a96-139">Subtotal</span><span class="sxs-lookup"><span data-stu-id="53a96-139">Subtotal</span></span></td>
<td><span data-ttu-id="53a96-140">Totale al lordo delle imposte e crediti e addebiti netti.</span><span class="sxs-lookup"><span data-stu-id="53a96-140">Total before taxes and tax-exclusive charges and credits.</span></span></td>
</tr>
<td><span data-ttu-id="53a96-141">Imposta</span><span class="sxs-lookup"><span data-stu-id="53a96-141">Tax</span></span></td>
<td><span data-ttu-id="53a96-142">Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura.</span><span class="sxs-lookup"><span data-stu-id="53a96-142">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> <span data-ttu-id="53a96-143">Questo numero è la somma di tutti gli addebiti che fanno riferimento a:</span><span class="sxs-lookup"><span data-stu-id="53a96-143">This number is the sum of all the charges in:</span></span>
<ul>
<li><span data-ttu-id="53a96-144">la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</span><span class="sxs-lookup"><span data-stu-id="53a96-144">the &quot;TaxAmount&quot; column of the Usage-based reconciliation file (column AA), and</span></span></li>
<li><span data-ttu-id="53a96-145">la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</span><span class="sxs-lookup"><span data-stu-id="53a96-145">the &quot;Tax&quot; column of the License-based file (column U).</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-146">Altri crediti</span><span class="sxs-lookup"><span data-stu-id="53a96-146">Other credits</span></span></td>
<td><span data-ttu-id="53a96-147">Crediti netti.</span><span class="sxs-lookup"><span data-stu-id="53a96-147">Tax-exclusive credits.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-148">Costi attuali totali</span><span class="sxs-lookup"><span data-stu-id="53a96-148">Total current charges</span></span></td>
<td><span data-ttu-id="53a96-149">L'importo dovuto nella valuta della fattura per il periodo fatturato, da pagare entro la data di scadenza.</span><span class="sxs-lookup"><span data-stu-id="53a96-149">The amount due in your billing currency for the billing period, due by the payment due date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-150">Istruzioni per il pagamento</span><span class="sxs-lookup"><span data-stu-id="53a96-150">Payment instructions</span></span></td>
<td><span data-ttu-id="53a96-151">Descrive come pagare la fattura, in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="53a96-151">Describes how to pay your invoice, based on your region.</span></span> <span data-ttu-id="53a96-152">Includi sempre il numero di fattura quando effettui un pagamento.</span><span class="sxs-lookup"><span data-stu-id="53a96-152">Always include your invoice number when making a payment.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-153">N. fattura</span><span class="sxs-lookup"><span data-stu-id="53a96-153">Invoice no</span></span></td>
<td><span data-ttu-id="53a96-154">Numero della fattura.</span><span class="sxs-lookup"><span data-stu-id="53a96-154">The number of your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-155">Periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="53a96-155">Billing period</span></span></td>
<td><span data-ttu-id="53a96-156">Il periodo mensile conducono alla data di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53a96-156">The monthly period leading up to the invoice date.</span></span> <span data-ttu-id="53a96-157">Questo è il periodo durante il quale vengono utilizzati i servizi basati sull'utilizzo e servizi basati su licenza vengono riconciliati le regolazioni di carta di credito o la modifica di nel conteggio delle licenze.</span><span class="sxs-lookup"><span data-stu-id="53a96-157">This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-158">Data fattura</span><span class="sxs-lookup"><span data-stu-id="53a96-158">Invoice date</span></span></td>
<td><span data-ttu-id="53a96-159">La data di fatturazione o data di ricorrenza in cui la fattura viene generata ogni mese.</span><span class="sxs-lookup"><span data-stu-id="53a96-159">Your billing date or anniversary date on which your invoice is generated each month.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-160">Condizioni di pagamento</span><span class="sxs-lookup"><span data-stu-id="53a96-160">Payment terms</span></span></td>
<td><span data-ttu-id="53a96-161">Per gli acquisti una tantum sarà sempre 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="53a96-161">For one-time purchases this will always be 60 days.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-162">Data scadenza pagamento</span><span class="sxs-lookup"><span data-stu-id="53a96-162">Payment due date</span></span></td>
<td><span data-ttu-id="53a96-163">Data entro cui effettuare il pagamento.</span><span class="sxs-lookup"><span data-stu-id="53a96-163">Your payment must be received by this date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-164">Ordine d'acquisto del cliente</span><span class="sxs-lookup"><span data-stu-id="53a96-164">Customer PO</span></span></td>
<td><span data-ttu-id="53a96-165">Il numero del tuo ordine di acquisto.</span><span class="sxs-lookup"><span data-stu-id="53a96-165">Your purchase order number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="53a96-166">Servizio clienti</span><span class="sxs-lookup"><span data-stu-id="53a96-166">Customer service</span></span></td>
<td><span data-ttu-id="53a96-167">Indirizzo del sito Web per accedere al servizio clienti.</span><span class="sxs-lookup"><span data-stu-id="53a96-167">The website address to access customer service.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="53a96-168">Destinatario del servizio</span><span class="sxs-lookup"><span data-stu-id="53a96-168">Service recipient</span></span></td>
<td><span data-ttu-id="53a96-169">Indirizzo in cui viene usato il servizio.</span><span class="sxs-lookup"><span data-stu-id="53a96-169">The address where the service is used.</span></span> <span data-ttu-id="53a96-170">(Questo è l'indirizzo ragione sociale della società associato all'azienda consultazione).</span><span class="sxs-lookup"><span data-stu-id="53a96-170">(This is the legal company address associated with company vetting.)</span></span></td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a><span data-ttu-id="53a96-171">Elenco dettagliato dei costi una tantum</span><span class="sxs-lookup"><span data-stu-id="53a96-171">Itemized list of one-time charges</span></span>

|<span data-ttu-id="53a96-172">**Campo**</span><span class="sxs-lookup"><span data-stu-id="53a96-172">**Field**</span></span> |<span data-ttu-id="53a96-173">**Definizione**</span><span class="sxs-lookup"><span data-stu-id="53a96-173">**Definition**</span></span>|
|:----------------|:-----------------------------|
|<span data-ttu-id="53a96-174">Data</span><span class="sxs-lookup"><span data-stu-id="53a96-174">Date</span></span> |<span data-ttu-id="53a96-175">Data di acquisto.</span><span class="sxs-lookup"><span data-stu-id="53a96-175">Date of purchase.</span></span> |
|<span data-ttu-id="53a96-176">Descrizione</span><span class="sxs-lookup"><span data-stu-id="53a96-176">Description</span></span> |<span data-ttu-id="53a96-177">Nome del prodotto.</span><span class="sxs-lookup"><span data-stu-id="53a96-177">Product name.</span></span> |
|<span data-ttu-id="53a96-178">Quantità</span><span class="sxs-lookup"><span data-stu-id="53a96-178">Quantity</span></span> |<span data-ttu-id="53a96-179">Numero di prodotti (prenotazioni, ad esempio) acquistati.</span><span class="sxs-lookup"><span data-stu-id="53a96-179">The number of products (reservations, e.g.) purchased.</span></span> |
|<span data-ttu-id="53a96-180">Prezzo unitario</span><span class="sxs-lookup"><span data-stu-id="53a96-180">Unit price</span></span> |<span data-ttu-id="53a96-181">Prezzo per prodotto (prenotazione, ad esempio).</span><span class="sxs-lookup"><span data-stu-id="53a96-181">Price per product (reservation, e.g.).</span></span> |
|<span data-ttu-id="53a96-182">Sconti</span><span class="sxs-lookup"><span data-stu-id="53a96-182">Discounts</span></span> |<span data-ttu-id="53a96-183">Eventuali sconti applicabili.</span><span class="sxs-lookup"><span data-stu-id="53a96-183">Any applicable discounts.</span></span> |
|<span data-ttu-id="53a96-184">Importo pre-imposta</span><span class="sxs-lookup"><span data-stu-id="53a96-184">Pre-tax amount</span></span> |<span data-ttu-id="53a96-185">Totale parziale degli acquisti prima delle imposte.</span><span class="sxs-lookup"><span data-stu-id="53a96-185">Sub-total of the purchases before taxes.</span></span> |
|<span data-ttu-id="53a96-186">Imposta sulle vendite</span><span class="sxs-lookup"><span data-stu-id="53a96-186">Sales tax</span></span> |<span data-ttu-id="53a96-187">Importo dell'imposta.</span><span class="sxs-lookup"><span data-stu-id="53a96-187">Tax amount.</span></span> |
|<span data-ttu-id="53a96-188">Totale</span><span class="sxs-lookup"><span data-stu-id="53a96-188">Total</span></span> |<span data-ttu-id="53a96-189">Totale da pagare.</span><span class="sxs-lookup"><span data-stu-id="53a96-189">Total to be paid.</span></span> |
 



