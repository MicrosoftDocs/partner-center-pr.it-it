---
title: Scenari comuni di fatturazione (centro per i Partner gestito da 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l'annullamento di una sottoscrizione.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132341"
---
# <a name="common-billing-scenarios"></a><span data-ttu-id="620c4-103">Scenari di fatturazione comuni</span><span class="sxs-lookup"><span data-stu-id="620c4-103">Common billing scenarios</span></span>

<span data-ttu-id="620c4-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="620c4-104">**Applies to**</span></span>

-   <span data-ttu-id="620c4-105">Centro per i partner gestito da 21Vianet</span><span class="sxs-lookup"><span data-stu-id="620c4-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="620c4-106">Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l'annullamento di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="620c4-106">This topic explains what you should expect to see on your bill after you add new subscriptions, adjust the number of seats in a subscription, or cancel a subscription.</span></span> 


## <a name="licence-based-billing"></a><span data-ttu-id="620c4-107">Fatturazione in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="620c4-107">Licence-based billing</span></span>


<span data-ttu-id="620c4-108">Per i mesi senza apportare modifiche alle sottoscrizioni in base al titolo, si noterà una singola voce per ogni sottoscrizione nel file di riconciliazione e fattura per l'addebito di avanzamento per il mese prossimo.</span><span class="sxs-lookup"><span data-stu-id="620c4-108">For months without changes to licence-based subscriptions, you'll see a single line item for each subscription on your reconciliation file and invoice for the advance charge for the coming month.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="620c4-109">Scenario</span><span class="sxs-lookup"><span data-stu-id="620c4-109">Scenario</span></span></td>
<td><span data-ttu-id="620c4-110">Descrizione</span><span class="sxs-lookup"><span data-stu-id="620c4-110">Description</span></span></td>
<td><span data-ttu-id="620c4-111">Esempio</span><span class="sxs-lookup"><span data-stu-id="620c4-111">Example</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="620c4-112">Nuova sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="620c4-112">New subscription</span></span></td>
<td><p><span data-ttu-id="620c4-113">Il periodo tra la data di inizio della sottoscrizione e la prima data di fatturazione è GRATIS.</span><span class="sxs-lookup"><span data-stu-id="620c4-113">The period between the start date of the subscription and the first billing date is FREE.</span></span></p>
<p><span data-ttu-id="620c4-114">Il file di riconciliazione conterrà una sola voce:</span><span class="sxs-lookup"><span data-stu-id="620c4-114">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-115">l'addebito dell'anticipo per il mese successivo</span><span class="sxs-lookup"><span data-stu-id="620c4-115">next month's advance charge</span></span></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="620c4-116">Nuova sottoscrizione con annullamento prima della scadenza di fatturazione</span><span class="sxs-lookup"><span data-stu-id="620c4-116">New subscription: cancelled before the billing cut</span></span></td>
<td><span data-ttu-id="620c4-117">Non verrà effettuato alcun addebito sull'account.</span><span class="sxs-lookup"><span data-stu-id="620c4-117">Charges will not be applied to the account.</span></span> <span data-ttu-id="620c4-118">La sottoscrizione non comparirà nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="620c4-118">The subscription won't appear in the reconciliation file.</span></span> <span data-ttu-id="620c4-119">Questa opzione è utile se vuoi eseguire test senza sostenere le spese della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="620c4-119">This is useful if you want to perform testing without incurring subscription charges.</span></span></td>
<td></td>
</tr>
<tr class="even">
<td><span data-ttu-id="620c4-120">Nuova sottoscrizione con rettifiche della quantità di licenze durante il periodo gratuito</span><span class="sxs-lookup"><span data-stu-id="620c4-120">New subscription: with licence quantity adjustments during the free period</span></span></td>
<td><p><span data-ttu-id="620c4-121">Il file di riconciliazione conterrà più voci:</span><span class="sxs-lookup"><span data-stu-id="620c4-121">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-122">modifiche alla quantità di licenze, con prezzo unitario 0</span><span class="sxs-lookup"><span data-stu-id="620c4-122">license quantity changes, charged at 0 Unit Price.</span></span> <span data-ttu-id="620c4-123">(per le modifiche di postazioni apportate durante il periodo gratuito non vengono effettuati addebiti).</span><span class="sxs-lookup"><span data-stu-id="620c4-123">(There is no cost for seat changes during the free period)</span></span></li>
<li><span data-ttu-id="620c4-124">addebito dell'anticipo per il mese successivo, in base alla nuova quantità.</span><span class="sxs-lookup"><span data-stu-id="620c4-124">advance charge for the next month, reflecting the new quantity.</span></span></li>
</ul></td>
<td><span data-ttu-id="620c4-125">Uso ripartito:</span><span class="sxs-lookup"><span data-stu-id="620c4-125">Prorated usage:</span></span>
<ul>
<li><span data-ttu-id="620c4-126">Dal 3 giugno al 7 giugno per 10 postazioni = addebito ZERO</span><span class="sxs-lookup"><span data-stu-id="620c4-126">June 3rd to June 7th for 10 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="620c4-127">Dall'8 giugno all'11 giugno per 20 postazioni = addebito ZERO</span><span class="sxs-lookup"><span data-stu-id="620c4-127">June 8th to June 11th for 20 seats = ZERO charge</span></span></li>
<li><span data-ttu-id="620c4-128">Dal 12 giugno al 14 giugno per 15 postazioni = addebito ZERO</span><span class="sxs-lookup"><span data-stu-id="620c4-128">June 12th to June 14th for 15 seats = ZERO charge</span></span></li>
</ul>
<p><span data-ttu-id="620c4-129">Taglia la fatturazione: Passare l'addebito per il periodo di tutto il mese dal 15 giugno al 14 luglio per 15 postazioni.</span><span class="sxs-lookup"><span data-stu-id="620c4-129">Billing cut: Advance charge for the whole month period from June 15th to July 14th for 15 seats.</span></span> <span data-ttu-id="620c4-130">Supponendo che l'addebito mensile per la sottoscrizione sia di 10 euro, l'addebito sarebbe 10 euro x 15 postazioni = 150 euro.</span><span class="sxs-lookup"><span data-stu-id="620c4-130">Assuming the charge per subscription per month is 10 USD, the charge would be 10 USD x 15 seats = 150 USD.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="620c4-131">Sottoscrizione esistente: Aumentare o ridurre una quantità licenze</span><span class="sxs-lookup"><span data-stu-id="620c4-131">Existing subscription: Increase or decrease in licence quantity</span></span></td>
<td><p><span data-ttu-id="620c4-132">Il file di riconciliazione conterrà più voci:</span><span class="sxs-lookup"><span data-stu-id="620c4-132">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-133">lo storno dell'anticipo</span><span class="sxs-lookup"><span data-stu-id="620c4-133">the advance charge reversal</span></span></li>
<li><span data-ttu-id="620c4-134">l'addebito per l'uso ripartito</span><span class="sxs-lookup"><span data-stu-id="620c4-134">prorated usage charges</span></span></li>
<li><span data-ttu-id="620c4-135">l'addebito dell'anticipo per il mese successivo</span><span class="sxs-lookup"><span data-stu-id="620c4-135">next month's advance charge</span></span></li>
</ul></td>
<td><p><span data-ttu-id="620c4-136">Uso ripartito:</span><span class="sxs-lookup"><span data-stu-id="620c4-136">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-137">Dal 15 luglio al 19 luglio per 15 postazioni = 26,61 euro</span><span class="sxs-lookup"><span data-stu-id="620c4-137">July 15th to July 19th for 15 seats = 26.61 USD</span></span></li>
<li><span data-ttu-id="620c4-138">Dal 20 luglio al 30 luglio per 12 postazioni = 46,84 euro</span><span class="sxs-lookup"><span data-stu-id="620c4-138">July 20th to July 30th for 12 seats = 46.84 USD</span></span></li>
<li><span data-ttu-id="620c4-139">Dal 31 luglio al 9 agosto per 18 postazioni = 63,87 euro</span><span class="sxs-lookup"><span data-stu-id="620c4-139">July 31st to August 9th for 18 seats = 63.87 USD</span></span></li>
<li><span data-ttu-id="620c4-140">Dal 10 agosto al 14 agosto per 10 postazioni = 17,74 euro</span><span class="sxs-lookup"><span data-stu-id="620c4-140">August 10th to August 14th for 10 seats = 17.74 USD</span></span></li>
</ul>
<span data-ttu-id="620c4-141">Storno dell'anticipo per il periodo mensile completo dal 15 luglio al 14 agosto = 165 euro.</span><span class="sxs-lookup"><span data-stu-id="620c4-141">Reversal of the advance charge for the whole month period from July 15th to August 14th = -165 USD.</span></span>
<p><span data-ttu-id="620c4-142">Taglia la fatturazione: Passare l'addebito per il periodo di tutto il mese da 15 agosto al 14 settembre per 10 postazioni = USD 110.</span><span class="sxs-lookup"><span data-stu-id="620c4-142">Billing cut: Advance charge for the whole month period from August 15th to September 14th for 10 seats = 110 USD.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="620c4-143">Annullamento senza modifiche precedenti delle postazioni</span><span class="sxs-lookup"><span data-stu-id="620c4-143">Cancellation: no prior seat changes</span></span></td>
<td><p><span data-ttu-id="620c4-144">Il file di riconciliazione conterrà una sola voce:</span><span class="sxs-lookup"><span data-stu-id="620c4-144">Your reconciliation file will contain a single line-item:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-145">Un credito per i giorni inutilizzati, poiché l'intero periodo è stato addebitato in anticipo nell'ultima distinta di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="620c4-145">A credit for unused days, because the whole period was billed in advance in the previous billing statement.</span></span> <span data-ttu-id="620c4-146">Viene calcolato in base alla data di fine della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="620c4-146">This is calculated based on the Subscription End date.</span></span></li>
</ul></td>
<td><span data-ttu-id="620c4-147">In precedenza fatturati in anticipo addebito: Postazioni 15 agosto a 14 settembre per 10 = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="620c4-147">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="620c4-148">Parte usata dell'anticipo dal 15 agosto al 24 agosto.</span><span class="sxs-lookup"><span data-stu-id="620c4-148">Consumed portion of the advance charge from August 15th to August 24th.</span></span></p>
<p><span data-ttu-id="620c4-149">Carta di credito per i giorni non utilizzati: 25 agosto a 14 settembre per 10 postazioni =-74.51.</span><span class="sxs-lookup"><span data-stu-id="620c4-149">Credit for unused days: August 25th to September 14th for 10 seats = -74.51.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="620c4-150">Annullamento con modifiche precedenti delle postazioni</span><span class="sxs-lookup"><span data-stu-id="620c4-150">Cancellation: with prior seat changes</span></span></td>
<td><p><span data-ttu-id="620c4-151">Il file di riconciliazione conterrà più voci:</span><span class="sxs-lookup"><span data-stu-id="620c4-151">Your reconciliation file will contain multiple line-items:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-152">lo storno dell'anticipo</span><span class="sxs-lookup"><span data-stu-id="620c4-152">the advance charge reversal</span></span></li>
<li><span data-ttu-id="620c4-153">l'addebito per l'uso ripartito</span><span class="sxs-lookup"><span data-stu-id="620c4-153">prorated usage charges</span></span></li>
<li><span data-ttu-id="620c4-154">un credito per eventuali giorni inutilizzati</span><span class="sxs-lookup"><span data-stu-id="620c4-154">a credit for any unused days</span></span></li>
</ul></td>
<td><span data-ttu-id="620c4-155">In precedenza fatturati in anticipo addebito: Postazioni 15 agosto a 14 settembre per 10 = 100 USD.</span><span class="sxs-lookup"><span data-stu-id="620c4-155">Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.</span></span>
<p><span data-ttu-id="620c4-156">Uso ripartito:</span><span class="sxs-lookup"><span data-stu-id="620c4-156">Prorated usage:</span></span></p>
<ul>
<li><span data-ttu-id="620c4-157">Dal 15 agosto al 24 agosto per 10 postazioni</span><span class="sxs-lookup"><span data-stu-id="620c4-157">August 15th to August 24th for 10 seats</span></span></li>
<li><span data-ttu-id="620c4-158">Dal 25 agosto al 14 settembre per 5 postazioni</span><span class="sxs-lookup"><span data-stu-id="620c4-158">August 25th to September 14th for 5 seats</span></span></li>
</ul>
<p><span data-ttu-id="620c4-159">Carta di credito per i giorni non utilizzati: Il 1 ° settembre a 14 settembre per 5 postazioni.</span><span class="sxs-lookup"><span data-stu-id="620c4-159">Credit for unused days: September 1st to September 14th for 5 seats.</span></span></p>
<p><span data-ttu-id="620c4-160">Storno dell'anticipo per il periodo mensile completo dal 15 agosto al 14 settembre = 100 euro.</span><span class="sxs-lookup"><span data-stu-id="620c4-160">Reversal of the advance charge for the whole month period from August 15th to September 14th = -100 USD.</span></span></p></td>
</tr>
</tbody>
</table>
