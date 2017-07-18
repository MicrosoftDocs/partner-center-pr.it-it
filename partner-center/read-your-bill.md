---
title: Leggere la fattura | Centro per i partner
description: "La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel dashboard del Centro per i partner."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 65c3777c0bd35933f2622fc0de105c051001974e
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/01/2017
---
# <a name="read-your-bill"></a><span data-ttu-id="47743-104">Leggere la fattura</span><span class="sxs-lookup"><span data-stu-id="47743-104">Read your bill</span></span>

**<span data-ttu-id="47743-105">Si applica a</span><span class="sxs-lookup"><span data-stu-id="47743-105">Applies to</span></span>**

-  <span data-ttu-id="47743-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="47743-106">Partner Center</span></span>
-  <span data-ttu-id="47743-107">Centro per i partner per Microsoft Cloud per il governo statunitense</span><span class="sxs-lookup"><span data-stu-id="47743-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="47743-108">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="47743-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="47743-109">La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente.</span><span class="sxs-lookup"><span data-stu-id="47743-109">Your invoice is a summary of all charges (across the program, products, and customers) for the current monthly period.</span></span> <span data-ttu-id="47743-110">È disponibile nel dashboard del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="47743-110">It is available on the Partner Center Dashboard.</span></span>

<span data-ttu-id="47743-111">Per i dettagli sugli addebiti, consulta i file di riconciliazione associati.</span><span class="sxs-lookup"><span data-stu-id="47743-111">For itemized details about the charges, use the accompanying reconciliation files.</span></span> <span data-ttu-id="47743-112">I file di riconciliazione includono gli ID dei clienti e gli ID delle sottoscrizioni che userai per creare le fatture per i clienti.</span><span class="sxs-lookup"><span data-stu-id="47743-112">The reconciliation files include the customer IDs and subscription IDs that you will use to create customer invoices.</span></span> <span data-ttu-id="47743-113">Per altre informazioni, vedi [Come usare i file di riconciliazione](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="47743-113">For more information, see [How to use the reconciliation files](use-the-reconciliation-files.md).</span></span>

## <a name="invoice-file-definitions"></a><span data-ttu-id="47743-114">Definizioni del file di fatturazione</span><span class="sxs-lookup"><span data-stu-id="47743-114">Invoice file definitions</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="47743-115">Campo</span><span class="sxs-lookup"><span data-stu-id="47743-115">Field</span></span></strong></td>
<td><strong><span data-ttu-id="47743-116">Descrizione</span><span class="sxs-lookup"><span data-stu-id="47743-116">Description</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-117">US FEIN</span><span class="sxs-lookup"><span data-stu-id="47743-117">US FEIN</span></span></td>
<td><span data-ttu-id="47743-118">ID fiscale federale.</span><span class="sxs-lookup"><span data-stu-id="47743-118">Your Federal Tax ID Number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-119">Numero cliente</span><span class="sxs-lookup"><span data-stu-id="47743-119">Customer number</span></span></td>
<td><span data-ttu-id="47743-120">Codice del cliente.</span><span class="sxs-lookup"><span data-stu-id="47743-120">Your customer number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-121">Indirizzo fatturazione</span><span class="sxs-lookup"><span data-stu-id="47743-121">Bill to</span></span></td>
<td><span data-ttu-id="47743-122">Indirizzo a cui inviare la fattura.</span><span class="sxs-lookup"><span data-stu-id="47743-122">The address where we send your invoice.</span></span> <span data-ttu-id="47743-123">Per cambiare questo indirizzo, modifica il tuo profilo dell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="47743-123">To change this address, edit your Partner Center account profile.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-124">Addebiti periodici</span><span class="sxs-lookup"><span data-stu-id="47743-124">Recurring charges</span></span></td>
<td><span data-ttu-id="47743-125">Gli addebiti fissi mensili o annuali per le licenze in base all'uso acquistate, fatturati prima del servizio.</span><span class="sxs-lookup"><span data-stu-id="47743-125">The flat monthly (or annual) charges for the purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="47743-126">Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</span><span class="sxs-lookup"><span data-stu-id="47743-126">This number is the sum of all charges in the &quot;Subtotal&quot; column in the License-based reconciliation file (column T).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-127">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="47743-127">Usage charges</span></span></td>
<td><span data-ttu-id="47743-128">Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="47743-128">Azure usage, including new services or applications enabled and used during the billing month.</span></span> <span data-ttu-id="47743-129">Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</span><span class="sxs-lookup"><span data-stu-id="47743-129">This number is the sum of all charges in the &quot;PretaxCharges&quot; column in the Usage-based reconciliation file (column Z).</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-130">Crediti e rettifiche</span><span class="sxs-lookup"><span data-stu-id="47743-130">Credits &amp; adjustments</span></span></td>
<td><span data-ttu-id="47743-131">Crediti o rettifiche per modifiche apportate alle sottoscrizioni, ad esempio aumento o riduzione delle postazioni.</span><span class="sxs-lookup"><span data-stu-id="47743-131">Credits or adjustments for changes made to subscriptions (example: seat increases or decreases).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-132">Altri sconti</span><span class="sxs-lookup"><span data-stu-id="47743-132">Other discounts</span></span></td>
<td><span data-ttu-id="47743-133">Ad esempio lo sconto che il cliente riceve sul prezzo normale della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="47743-133">For example, the discount that the customer receives from the normal price of the subscription.</span></span> <span data-ttu-id="47743-134">Lo sconto viene indicato come importo unico, non come prezzo per unità o licenza.</span><span class="sxs-lookup"><span data-stu-id="47743-134">This is shown as a flat amount, not as a price per unit or license.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-135">Imposte</span><span class="sxs-lookup"><span data-stu-id="47743-135">Taxes</span></span></td>
<td><span data-ttu-id="47743-136">Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura.</span><span class="sxs-lookup"><span data-stu-id="47743-136">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> <span data-ttu-id="47743-137">Questo numero è la somma di tutti gli addebiti che fanno riferimento a:</span><span class="sxs-lookup"><span data-stu-id="47743-137">This number is the sum of all the charges in:</span></span>
<ul>
<li><span data-ttu-id="47743-138">la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</span><span class="sxs-lookup"><span data-stu-id="47743-138">the &quot;TaxAmount&quot; column of the Usage-based reconciliation file (column AA), and</span></span></li>
<li><span data-ttu-id="47743-139">la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</span><span class="sxs-lookup"><span data-stu-id="47743-139">the &quot;Tax&quot; column of the License-based file (column U).</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-140">Costi attuali totali</span><span class="sxs-lookup"><span data-stu-id="47743-140">Total current charges</span></span></td>
<td><span data-ttu-id="47743-141">L'importo dovuto nella valuta della fattura per il periodo fatturato, da pagare entro la data di scadenza.</span><span class="sxs-lookup"><span data-stu-id="47743-141">The amount due in your billing currency for the billing period, due by the payment due date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-142">Istruzioni per il pagamento</span><span class="sxs-lookup"><span data-stu-id="47743-142">Payment instructions</span></span></td>
<td><span data-ttu-id="47743-143">Descrive come pagare la fattura, in base all'area geografica.</span><span class="sxs-lookup"><span data-stu-id="47743-143">Describes how to pay your invoice, based on your region.</span></span> <span data-ttu-id="47743-144">Includi sempre il numero di fattura quando effettui un pagamento.</span><span class="sxs-lookup"><span data-stu-id="47743-144">Always include your invoice number when making a payment.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-145">N. fattura</span><span class="sxs-lookup"><span data-stu-id="47743-145">Invoice no</span></span></td>
<td><span data-ttu-id="47743-146">Numero della fattura.</span><span class="sxs-lookup"><span data-stu-id="47743-146">The number of your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-147">Periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="47743-147">Billing period</span></span></td>
<td><span data-ttu-id="47743-148">I partner CSP ricevono una fattura mensile o annuale.</span><span class="sxs-lookup"><span data-stu-id="47743-148">CSP partners are billed either monthly or annually.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-149">Data fattura</span><span class="sxs-lookup"><span data-stu-id="47743-149">Invoice date</span></span></td>
<td><span data-ttu-id="47743-150">Data in cui ricevi la fattura.</span><span class="sxs-lookup"><span data-stu-id="47743-150">The date you receive your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-151">Data scadenza pagamento</span><span class="sxs-lookup"><span data-stu-id="47743-151">Payment due date</span></span></td>
<td><span data-ttu-id="47743-152">Data entro cui effettuare il pagamento.</span><span class="sxs-lookup"><span data-stu-id="47743-152">Your payment must be received by this date.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-153">Ordine d'acquisto del cliente</span><span class="sxs-lookup"><span data-stu-id="47743-153">Customer PO</span></span></td>
<td><span data-ttu-id="47743-154">Il numero del tuo ordine di acquisto.</span><span class="sxs-lookup"><span data-stu-id="47743-154">Your purchase order number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="47743-155">Servizio clienti</span><span class="sxs-lookup"><span data-stu-id="47743-155">Customer service</span></span></td>
<td><span data-ttu-id="47743-156">Indirizzo del sito Web per accedere al servizio clienti.</span><span class="sxs-lookup"><span data-stu-id="47743-156">The website address to access customer service.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="47743-157">Destinatario del servizio</span><span class="sxs-lookup"><span data-stu-id="47743-157">Service recipient</span></span></td>
<td><span data-ttu-id="47743-158">Indirizzo in cui viene usato il servizio.</span><span class="sxs-lookup"><span data-stu-id="47743-158">The address where the service is used.</span></span> <span data-ttu-id="47743-159">(Questo è l'indirizzo legale della società associato alla verifica della società e non può essere modificato.)</span><span class="sxs-lookup"><span data-stu-id="47743-159">(This is the legal company address associated with company vetting and cannot be changed.)</span></span></td>
</tr>
</tbody>
</table>

 

 

 



