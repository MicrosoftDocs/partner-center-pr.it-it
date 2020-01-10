---
title: Tipi di addebito file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 01/06/2020
description: Tipi di addebiti (basati su licenza, utilizzo e una volta), crediti e sconti sui file di riconciliazione del centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b18a2a7d53e2f9d35baac2412c1710c21d6d98eb
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716872"
---
# <a name="understand-charge-types"></a><span data-ttu-id="99d0d-103">Informazioni sui tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-103">Understand charge types</span></span>

<span data-ttu-id="99d0d-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="99d0d-104">**Applies to**</span></span>

- <span data-ttu-id="99d0d-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="99d0d-105">Partner Center</span></span>
- <span data-ttu-id="99d0d-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="99d0d-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="99d0d-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="99d0d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="99d0d-108">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="99d0d-108">Admin agent</span></span>
- <span data-ttu-id="99d0d-109">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="99d0d-109">Billing admin</span></span>
- <span data-ttu-id="99d0d-110">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="99d0d-110">Global admin</span></span>

<span data-ttu-id="99d0d-111">In questo argomento vengono descritti i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere presenti nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="99d0d-112">La fattura fornisce un riepilogo degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="99d0d-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="99d0d-113">Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di elementi riga, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="99d0d-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="99d0d-114">Per ulteriori informazioni sui file di riconciliazione, vedere [come utilizzare i file di riconciliazione](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="99d0d-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="99d0d-115">Sia [i file di riconciliazione basati sull'utilizzo](usage-based-recon-files.md) che [i file di riconciliazione basati sulle licenze](license-based-recon-files.md) mostrano solo le transazioni e gli addebiti relativi all'utilizzo (unità utilizzate e addebiti correlati).</span><span class="sxs-lookup"><span data-stu-id="99d0d-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="99d0d-116">I crediti, gli sconti o i rimborsi unidirezionali visualizzati nella fattura come **modifiche** non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="99d0d-117">Mappare i tipi di addebito ai costi fattura</span><span class="sxs-lookup"><span data-stu-id="99d0d-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="99d0d-118">Per fare riferimento incrociato agli importi tra la fattura e il file di riconciliazione, utilizzare le opzioni di filtro in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="99d0d-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="99d0d-119">Filtrare in base ai tipi di addebito sul file di riconciliazione per eseguire il mapping degli addebiti per la fattura a un set di suddivisione dei costi nel file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="99d0d-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="99d0d-120">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="99d0d-120">License-based charges</span></span>

<span data-ttu-id="99d0d-121">Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="99d0d-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="99d0d-122">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="99d0d-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="99d0d-123">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="99d0d-124">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="99d0d-124">Activation fee</span></span> | <span data-ttu-id="99d0d-125">Importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="99d0d-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="99d0d-126">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="99d0d-126">Cancel fee</span></span> | <span data-ttu-id="99d0d-127">Addebiti rivalutati per il cliente quando vengono modificate le postazioni associate.</span><span class="sxs-lookup"><span data-stu-id="99d0d-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="99d0d-128">Istanza di annullamento ripartita proporzionalmente</span><span class="sxs-lookup"><span data-stu-id="99d0d-128">Cancel instance prorate</span></span> | <span data-ttu-id="99d0d-129">Addebiti rivalutati annullati quando al cliente con sottoscrizione mensile è stata sospesa la sottoscrizione e le postazioni associate sono state modificate nello stesso mese</span><span class="sxs-lookup"><span data-stu-id="99d0d-129">Prorated charges cancelled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="99d0d-130">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="99d0d-130">Cycle fee</span></span> | <span data-ttu-id="99d0d-131">Addebiti periodici per una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="99d0d-132">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="99d0d-132">Cycle instance prorate</span></span> | <span data-ttu-id="99d0d-133">Addebiti rivalutati dal cliente quando vengono modificate le postazioni associate.</span><span class="sxs-lookup"><span data-stu-id="99d0d-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="99d0d-134">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="99d0d-134">Prorate fees when cancel</span></span> | <span data-ttu-id="99d0d-135">Rimborso proporzionale per la parte di servizio inutilizzata al momento dell'annullamento.</span><span class="sxs-lookup"><span data-stu-id="99d0d-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="99d0d-136">Tariffe propagate quando si esegue la conversione a partire dall'offerta corrente</span><span class="sxs-lookup"><span data-stu-id="99d0d-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="99d0d-137">Addebiti rivalutati dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale.</span><span class="sxs-lookup"><span data-stu-id="99d0d-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="99d0d-138">Tariffe della propagazione durante la conversione in una nuova offerta</span><span class="sxs-lookup"><span data-stu-id="99d0d-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="99d0d-139">Addebiti rivalutati dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale.</span><span class="sxs-lookup"><span data-stu-id="99d0d-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="99d0d-140">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="99d0d-140">Prorate fees when purchase</span></span> | <span data-ttu-id="99d0d-141">Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale.</span><span class="sxs-lookup"><span data-stu-id="99d0d-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="99d0d-142">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="99d0d-142">Purchase fee</span></span> | <span data-ttu-id="99d0d-143">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile.</span><span class="sxs-lookup"><span data-stu-id="99d0d-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="99d0d-144">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="99d0d-144">Prorate fee when renew</span></span> | <span data-ttu-id="99d0d-145">Tariffe riordinate al rinnovo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="99d0d-146">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="99d0d-146">Renew fee</span></span> | <span data-ttu-id="99d0d-147">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="99d0d-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="99d0d-148">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="99d0d-148">Prorate fees when activate</span></span> | <span data-ttu-id="99d0d-149">> tariffe rivalutate dall'attivazione fino alla fine del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-149">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="99d0d-150">Addebiti monouso</span><span class="sxs-lookup"><span data-stu-id="99d0d-150">One-time charges</span></span>

<span data-ttu-id="99d0d-151">Per eseguire il mapping di questi addebiti monouso alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="99d0d-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="99d0d-152">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="99d0d-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="99d0d-153">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="99d0d-154">Nuova</span><span class="sxs-lookup"><span data-stu-id="99d0d-154">New</span></span> | <span data-ttu-id="99d0d-155">Utilizzato quando viene creato un nuovo acquisto.</span><span class="sxs-lookup"><span data-stu-id="99d0d-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="99d0d-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="99d0d-156">addQuantity</span></span> | <span data-ttu-id="99d0d-157">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo un aumento.</span><span class="sxs-lookup"><span data-stu-id="99d0d-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="99d0d-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="99d0d-158">removeQuantity</span></span> | <span data-ttu-id="99d0d-159">Utilizzato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo una riduzione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="99d0d-160">Annulla</span><span class="sxs-lookup"><span data-stu-id="99d0d-160">Cancel</span></span> | <span data-ttu-id="99d0d-161">Utilizzato quando viene annullata una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="99d0d-161">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="99d0d-162">Convert</span><span class="sxs-lookup"><span data-stu-id="99d0d-162">Convert</span></span> | <span data-ttu-id="99d0d-163">Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato.</span><span class="sxs-lookup"><span data-stu-id="99d0d-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="99d0d-164">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="99d0d-164">Usage charges</span></span>

<span data-ttu-id="99d0d-165">Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="99d0d-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="99d0d-166">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="99d0d-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="99d0d-167">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="99d0d-168">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="99d0d-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="99d0d-169">Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="99d0d-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="99d0d-170">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="99d0d-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="99d0d-171">Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="99d0d-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="99d0d-172">Crediti</span><span class="sxs-lookup"><span data-stu-id="99d0d-172">Credits</span></span>

<span data-ttu-id="99d0d-173">Per eseguire il mapping di questi crediti alla fattura:</span><span class="sxs-lookup"><span data-stu-id="99d0d-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="99d0d-174">Sommare il **TotalForCustomer** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="99d0d-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="99d0d-175">Sommare la colonna **PostTaxTotal** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="99d0d-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="99d0d-176">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="99d0d-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="99d0d-177">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="99d0d-178">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="99d0d-178">Offset a line item</span></span> | <span data-ttu-id="99d0d-179">Rimborso parziale o totale per una voce, incluse le imposte.</span><span class="sxs-lookup"><span data-stu-id="99d0d-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="99d0d-180">Sconti in base all'uso</span><span class="sxs-lookup"><span data-stu-id="99d0d-180">Usage-based discounts</span></span>

<span data-ttu-id="99d0d-181">Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="99d0d-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="99d0d-182">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="99d0d-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="99d0d-183">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="99d0d-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="99d0d-184">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="99d0d-184">Activation discount</span></span> | <span data-ttu-id="99d0d-185">Sconto applicato quando la sottoscrizione è stata attivata.</span><span class="sxs-lookup"><span data-stu-id="99d0d-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="99d0d-186">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="99d0d-186">Cycle discount</span></span> | <span data-ttu-id="99d0d-187">Sconto applicato agli addebiti periodici.</span><span class="sxs-lookup"><span data-stu-id="99d0d-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="99d0d-188">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="99d0d-188">Renew discount</span></span> | <span data-ttu-id="99d0d-189">Sconto applicato quando la sottoscrizione è stata rinnovata.</span><span class="sxs-lookup"><span data-stu-id="99d0d-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="99d0d-190">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="99d0d-190">Cancel discount</span></span> | <span data-ttu-id="99d0d-191">Addebiti applicati quando gli sconti vengono annullati.</span><span class="sxs-lookup"><span data-stu-id="99d0d-191">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="99d0d-192">Sconti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="99d0d-192">License-based discounts</span></span>

<span data-ttu-id="99d0d-193">Per eseguire il mapping degli sconti basati sulle licenze alla fattura, sommare la colonna **TotalOtherDiscount** del file basato su licenza.</span><span class="sxs-lookup"><span data-stu-id="99d0d-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="99d0d-194">*Gli sconti basati sulle licenze possono essere applicati a più tipi di addebito.*</span><span class="sxs-lookup"><span data-stu-id="99d0d-194">*License-based discounts may be applied to multiple charge types.*</span></span>
