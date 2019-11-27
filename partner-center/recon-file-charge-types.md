---
title: Tipi di addebito file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 08/26/2019
description: Tipi di addebiti (basati su licenza, utilizzo e una volta), crediti e sconti sui file di riconciliazione del centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389809"
---
# <a name="understand-charge-types"></a><span data-ttu-id="24028-103">Informazioni sui tipi di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-103">Understand charge types</span></span>

<span data-ttu-id="24028-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="24028-104">Applies to:</span></span>

- <span data-ttu-id="24028-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="24028-105">Partner Center</span></span>
- <span data-ttu-id="24028-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="24028-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="24028-107">In questo argomento vengono descritti i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere presenti nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="24028-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="24028-108">La fattura fornisce un riepilogo degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="24028-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="24028-109">Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di elementi riga, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="24028-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="24028-110">Per ulteriori informazioni sui file di riconciliazione, vedere [come utilizzare i file di riconciliazione](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="24028-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="24028-111">Sia [i file di riconciliazione basati sull'utilizzo](usage-based-recon-files.md) che [i file di riconciliazione basati sulle licenze](license-based-recon-files.md) mostrano solo le transazioni e gli addebiti relativi all'utilizzo (unità utilizzate e addebiti correlati).</span><span class="sxs-lookup"><span data-stu-id="24028-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="24028-112">I crediti, gli sconti o i rimborsi unidirezionali visualizzati nella fattura come **modifiche** non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="24028-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="24028-113">Mappare i tipi di addebito ai costi fattura</span><span class="sxs-lookup"><span data-stu-id="24028-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="24028-114">Per fare riferimento incrociato agli importi tra la fattura e il file di riconciliazione, utilizzare le opzioni di filtro in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="24028-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="24028-115">Filtrare in base ai tipi di addebito sul file di riconciliazione per eseguire il mapping degli addebiti per la fattura a un set di suddivisione dei costi nel file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="24028-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="24028-116">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="24028-116">License-based charges</span></span>

<span data-ttu-id="24028-117">Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="24028-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24028-118">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="24028-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24028-119">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24028-120">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="24028-120">Activation fee</span></span> | <span data-ttu-id="24028-121">Importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="24028-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="24028-122">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="24028-122">Cancel fee</span></span> | <span data-ttu-id="24028-123">Addebiti rivalutati per il cliente quando vengono modificate le postazioni associate.</span><span class="sxs-lookup"><span data-stu-id="24028-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="24028-124">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="24028-124">Cycle fee</span></span> | <span data-ttu-id="24028-125">Addebiti periodici per una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="24028-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="24028-126">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="24028-126">Cycle instance prorate</span></span> | <span data-ttu-id="24028-127">Addebiti rivalutati dal cliente quando vengono modificate le postazioni associate.</span><span class="sxs-lookup"><span data-stu-id="24028-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="24028-128">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="24028-128">Prorate fees when cancel</span></span> | <span data-ttu-id="24028-129">Rimborso proporzionale per la parte di servizio inutilizzata al momento dell'annullamento.</span><span class="sxs-lookup"><span data-stu-id="24028-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="24028-130">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="24028-130">Prorate fees when purchase</span></span> | <span data-ttu-id="24028-131">Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale.</span><span class="sxs-lookup"><span data-stu-id="24028-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="24028-132">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="24028-132">Purchase fee</span></span> | <span data-ttu-id="24028-133">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile.</span><span class="sxs-lookup"><span data-stu-id="24028-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="24028-134">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="24028-134">Prorate fee when renew</span></span> | <span data-ttu-id="24028-135">Tariffe riordinate al rinnovo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="24028-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="24028-136">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="24028-136">Renew fee</span></span> | <span data-ttu-id="24028-137">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="24028-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="24028-138">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="24028-138">Prorate fees when activate</span></span> | <span data-ttu-id="24028-139">> tariffe rivalutate dall'attivazione fino alla fine del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="24028-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="24028-140">Addebiti monouso</span><span class="sxs-lookup"><span data-stu-id="24028-140">One-time charges</span></span>

<span data-ttu-id="24028-141">Per eseguire il mapping di questi addebiti monouso alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="24028-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="24028-142">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="24028-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24028-143">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24028-144">Nuova</span><span class="sxs-lookup"><span data-stu-id="24028-144">New</span></span> | <span data-ttu-id="24028-145">Utilizzato quando viene creato un nuovo acquisto.</span><span class="sxs-lookup"><span data-stu-id="24028-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="24028-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="24028-146">addQuantity</span></span> | <span data-ttu-id="24028-147">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo un aumento.</span><span class="sxs-lookup"><span data-stu-id="24028-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="24028-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="24028-148">removeQuantity</span></span> | <span data-ttu-id="24028-149">Utilizzato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo una riduzione.</span><span class="sxs-lookup"><span data-stu-id="24028-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="24028-150">Cancel</span><span class="sxs-lookup"><span data-stu-id="24028-150">Cancel</span></span> | <span data-ttu-id="24028-151">Utilizzato quando viene annullata una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="24028-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="24028-152">Convertire</span><span class="sxs-lookup"><span data-stu-id="24028-152">Convert</span></span> | <span data-ttu-id="24028-153">Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato.</span><span class="sxs-lookup"><span data-stu-id="24028-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="24028-154">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="24028-154">Usage charges</span></span>

<span data-ttu-id="24028-155">Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="24028-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24028-156">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="24028-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24028-157">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24028-158">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="24028-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="24028-159">Costo di utilizzo dell'accesso al momento dell'annullamento per l'utilizzo non retribuito durante il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="24028-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="24028-160">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="24028-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="24028-161">Costo di utilizzo dell'accesso per il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="24028-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="24028-162">Crediti</span><span class="sxs-lookup"><span data-stu-id="24028-162">Credits</span></span>

<span data-ttu-id="24028-163">Per eseguire il mapping di questi crediti alla fattura:</span><span class="sxs-lookup"><span data-stu-id="24028-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="24028-164">Sommare il **TotalForCustomer** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="24028-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="24028-165">Sommare la colonna **PostTaxTotal** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="24028-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="24028-166">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="24028-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24028-167">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24028-168">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="24028-168">Offset a line item</span></span> | <span data-ttu-id="24028-169">Rimborso parziale o totale a una voce di riga, incluse le imposte.</span><span class="sxs-lookup"><span data-stu-id="24028-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="24028-170">Sconti in base all'uso</span><span class="sxs-lookup"><span data-stu-id="24028-170">Usage-based discounts</span></span>

<span data-ttu-id="24028-171">Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="24028-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="24028-172">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="24028-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="24028-173">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="24028-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="24028-174">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="24028-174">Activation discount</span></span> | <span data-ttu-id="24028-175">Sconto applicato quando la sottoscrizione è stata attivata.</span><span class="sxs-lookup"><span data-stu-id="24028-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="24028-176">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="24028-176">Cycle discount</span></span> | <span data-ttu-id="24028-177">Sconto applicato agli addebiti periodici.</span><span class="sxs-lookup"><span data-stu-id="24028-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="24028-178">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="24028-178">Renew discount</span></span> | <span data-ttu-id="24028-179">Sconto applicato quando la sottoscrizione è stata rinnovata.</span><span class="sxs-lookup"><span data-stu-id="24028-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="24028-180">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="24028-180">Cancel discount</span></span> | <span data-ttu-id="24028-181">Addebiti applicati quando gli sconti vengono annullati.</span><span class="sxs-lookup"><span data-stu-id="24028-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="24028-182">Sconti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="24028-182">License-based discounts</span></span>

<span data-ttu-id="24028-183">Per eseguire il mapping degli sconti basati sulle licenze alla fattura, sommare la colonna **TotalOtherDiscount** del file basato su licenza.</span><span class="sxs-lookup"><span data-stu-id="24028-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="24028-184">*Gli sconti basati sulle licenze possono essere applicati a più tipi di addebito.*</span><span class="sxs-lookup"><span data-stu-id="24028-184">*License-based discounts may be applied to multiple charge types.*</span></span>
