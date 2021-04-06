---
title: Tipi di addebito dei file di riconciliazione
ms.topic: article
ms.date: 06/05/2020
description: Individuare i tipi di addebiti (ad esempio, basati su licenza, utilizzo e una volta), crediti e sconti nei file di riconciliazione del centro per i partner.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441598"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="1e6d4-103">Informazioni sui diversi tipi di addebito nei file di riconciliazione del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="1e6d4-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="1e6d4-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="1e6d4-104">**Applies to**</span></span>

- <span data-ttu-id="1e6d4-105">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="1e6d4-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="1e6d4-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="1e6d4-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1e6d4-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="1e6d4-107">Admin agent</span></span>
- <span data-ttu-id="1e6d4-108">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-108">Billing admin</span></span>
- <span data-ttu-id="1e6d4-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="1e6d4-109">Global admin</span></span>

<span data-ttu-id="1e6d4-110">Questo articolo descrive i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere presenti nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="1e6d4-111">La fattura fornisce un riepilogo degli addebiti.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="1e6d4-112">Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di elementi riga, inclusi i tipi di addebito.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="1e6d4-113">Per ulteriori informazioni sui file di riconciliazione, vedere [come utilizzare i file di riconciliazione](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="1e6d4-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="1e6d4-114">Sia [i file di riconciliazione basati sull'utilizzo](usage-based-recon-files.md) che [i file di riconciliazione basati sulle licenze](license-based-recon-files.md) mostrano solo le transazioni e gli addebiti relativi all'utilizzo (unità utilizzate e addebiti correlati).</span><span class="sxs-lookup"><span data-stu-id="1e6d4-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="1e6d4-115">I crediti, gli sconti o i rimborsi unidirezionali visualizzati nella fattura come **modifiche** non vengono visualizzati nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="1e6d4-116">Mappare i tipi di addebito ai costi fattura</span><span class="sxs-lookup"><span data-stu-id="1e6d4-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="1e6d4-117">Per fare riferimento incrociato agli importi tra la fattura e il file di riconciliazione, utilizzare le opzioni di filtro in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="1e6d4-118">Filtrare in base ai tipi di addebito sul file di riconciliazione per eseguire il mapping degli addebiti per la fattura a un set di suddivisione dei costi nel file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="1e6d4-119">Addebiti basati su licenza</span><span class="sxs-lookup"><span data-stu-id="1e6d4-119">License-based charges</span></span>

<span data-ttu-id="1e6d4-120">Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="1e6d4-121">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="1e6d4-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="1e6d4-122">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="1e6d4-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="1e6d4-123">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-123">Activation fee</span></span> | <span data-ttu-id="1e6d4-124">Importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="1e6d4-125">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="1e6d4-125">Cancel fee</span></span> | <span data-ttu-id="1e6d4-126">Addebiti rivalutati per il cliente quando vengono modificate le licenze associate.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="1e6d4-127">Annulla profrequenza istanza</span><span class="sxs-lookup"><span data-stu-id="1e6d4-127">Cancel instance prorate</span></span> | <span data-ttu-id="1e6d4-128">Addebiti rivalutati annullati quando al cliente con sottoscrizione mensile è stata sospesa la sottoscrizione e le licenze associate sono state modificate nello stesso mese.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="1e6d4-129">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="1e6d4-129">Cycle fee</span></span> | <span data-ttu-id="1e6d4-130">Addebiti periodici per una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="1e6d4-131">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-131">Cycle instance prorate</span></span> | <span data-ttu-id="1e6d4-132">Addebiti rivalutati dal cliente quando vengono modificate le licenze associate.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="1e6d4-133">Tariffe propagate quando si annulla</span><span class="sxs-lookup"><span data-stu-id="1e6d4-133">Prorate fees when cancel</span></span> | <span data-ttu-id="1e6d4-134">Rimborso proporzionale per la parte di servizio inutilizzata al momento dell'annullamento.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="1e6d4-135">Tariffe propagate quando si esegue la conversione a partire dall'offerta corrente</span><span class="sxs-lookup"><span data-stu-id="1e6d4-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="1e6d4-136">Addebiti rivalutati dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="1e6d4-137">Tariffe della propagazione durante la conversione in una nuova offerta</span><span class="sxs-lookup"><span data-stu-id="1e6d4-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="1e6d4-138">Addebiti rivalutati dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="1e6d4-139">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="1e6d4-139">Prorate fees when purchase</span></span> | <span data-ttu-id="1e6d4-140">Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile o annuale.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="1e6d4-141">Tariffa della propagazione al rinnovo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-141">Prorate fee when renew</span></span> | <span data-ttu-id="1e6d4-142">Tariffe riordinate al rinnovo della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="1e6d4-143">Tassa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-143">Renew fee</span></span> | <span data-ttu-id="1e6d4-144">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="1e6d4-145">Tariffe propagate all'attivazione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-145">Prorate fees when activate</span></span> | <span data-ttu-id="1e6d4-146">Tariffe rivalutate dall'attivazione fino alla fine del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="1e6d4-147">Addebiti monouso</span><span class="sxs-lookup"><span data-stu-id="1e6d4-147">One-time charges</span></span>

<span data-ttu-id="1e6d4-148">Per eseguire il mapping di questi addebiti monouso alla fattura, sommare la colonna **Amount** del file basato su licenze.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="1e6d4-149">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="1e6d4-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="1e6d4-150">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="1e6d4-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="1e6d4-151">Nuova</span><span class="sxs-lookup"><span data-stu-id="1e6d4-151">New</span></span> | <span data-ttu-id="1e6d4-152">Utilizzato quando viene creato un nuovo acquisto.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="1e6d4-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="1e6d4-153">addQuantity</span></span> | <span data-ttu-id="1e6d4-154">Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo un aumento.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="1e6d4-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="1e6d4-155">removeQuantity</span></span> | <span data-ttu-id="1e6d4-156">Utilizzato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo una riduzione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="1e6d4-157">Annulla</span><span class="sxs-lookup"><span data-stu-id="1e6d4-157">Cancel</span></span> | <span data-ttu-id="1e6d4-158">Utilizzato quando viene annullata una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="1e6d4-159">Conversione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-159">Convert</span></span> | <span data-ttu-id="1e6d4-160">Usato quando viene aggiornata una licenza, ma il numero di licenze rimane invariato.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="1e6d4-161">Addebiti per utilizzo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-161">Usage charges</span></span>

<span data-ttu-id="1e6d4-162">Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="1e6d4-163">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="1e6d4-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="1e6d4-164">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="1e6d4-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="1e6d4-165">Valutazione della tariffa di utilizzo quando viene annullata</span><span class="sxs-lookup"><span data-stu-id="1e6d4-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="1e6d4-166">Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="1e6d4-167">Valutazione della tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="1e6d4-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="1e6d4-168">Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="1e6d4-169">Credits</span><span class="sxs-lookup"><span data-stu-id="1e6d4-169">Credits</span></span>

<span data-ttu-id="1e6d4-170">Per eseguire il mapping di questi crediti alla fattura:</span><span class="sxs-lookup"><span data-stu-id="1e6d4-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="1e6d4-171">Sommare il **TotalForCustomer** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="1e6d4-172">Sommare la colonna **PostTaxTotal** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="1e6d4-173">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="1e6d4-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="1e6d4-174">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="1e6d4-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="1e6d4-175">Offset di un elemento linea</span><span class="sxs-lookup"><span data-stu-id="1e6d4-175">Offset a line item</span></span> | <span data-ttu-id="1e6d4-176">Rimborso parziale o totale per una voce, incluse le imposte.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="1e6d4-177">Sconti basati sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-177">Usage-based discounts</span></span>

<span data-ttu-id="1e6d4-178">Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="1e6d4-179">Descrizione addebito (colonna ChargeType nel file di riconciliazione)</span><span class="sxs-lookup"><span data-stu-id="1e6d4-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="1e6d4-180">Spiegazione di addebito</span><span class="sxs-lookup"><span data-stu-id="1e6d4-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="1e6d4-181">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="1e6d4-181">Activation discount</span></span> | <span data-ttu-id="1e6d4-182">Sconto applicato quando la sottoscrizione è stata attivata.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="1e6d4-183">Sconto del ciclo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-183">Cycle discount</span></span> | <span data-ttu-id="1e6d4-184">Sconto applicato agli addebiti periodici.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="1e6d4-185">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="1e6d4-185">Renew discount</span></span> | <span data-ttu-id="1e6d4-186">Sconto applicato quando la sottoscrizione è stata rinnovata.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="1e6d4-187">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="1e6d4-187">Cancel discount</span></span> | <span data-ttu-id="1e6d4-188">Addebiti applicati quando vengono annullati gli sconti.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="1e6d4-189">Sconti basati su licenza</span><span class="sxs-lookup"><span data-stu-id="1e6d4-189">License-based discounts</span></span>

<span data-ttu-id="1e6d4-190">Per eseguire il mapping degli sconti basati sulle licenze alla fattura, sommare la colonna **TotalOtherDiscount** del file basato su licenza.</span><span class="sxs-lookup"><span data-stu-id="1e6d4-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="1e6d4-191">*Gli sconti basati sulle licenze possono essere applicati a più tipi di addebito.*</span><span class="sxs-lookup"><span data-stu-id="1e6d4-191">*License-based discounts may be applied to multiple charge types.*</span></span>
