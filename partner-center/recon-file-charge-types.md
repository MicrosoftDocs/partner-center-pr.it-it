---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a><span data-ttu-id="21251-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="21251-103">Understand charge types</span></span>

<span data-ttu-id="21251-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="21251-104">Applies to:</span></span>

- <span data-ttu-id="21251-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="21251-105">Partner Center</span></span>
- <span data-ttu-id="21251-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="21251-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="21251-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="21251-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="21251-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="21251-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="21251-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="21251-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="21251-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="21251-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="21251-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="21251-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="21251-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="21251-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="21251-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="21251-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="21251-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="21251-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="21251-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="21251-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="21251-116">Addebiti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="21251-116">License-based charges</span></span>

<span data-ttu-id="21251-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="21251-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="21251-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="21251-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="21251-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="21251-120">Commissione di attivazione</span><span class="sxs-lookup"><span data-stu-id="21251-120">Activation fee</span></span> | <span data-ttu-id="21251-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="21251-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="21251-122">Commissione di annullamento</span><span class="sxs-lookup"><span data-stu-id="21251-122">Cancel fee</span></span> | <span data-ttu-id="21251-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="21251-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="21251-124">Tariffa periodica</span><span class="sxs-lookup"><span data-stu-id="21251-124">Cycle fee</span></span> | <span data-ttu-id="21251-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="21251-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="21251-126">Ripartizione dell'istanza del ciclo</span><span class="sxs-lookup"><span data-stu-id="21251-126">Cycle instance prorate</span></span> | <span data-ttu-id="21251-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="21251-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="21251-128">Rateizza le tariffe in caso di annullamento</span><span class="sxs-lookup"><span data-stu-id="21251-128">Prorate fees when cancel</span></span> | <span data-ttu-id="21251-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="21251-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="21251-130">Ripartizione delle tariffe all'acquisto</span><span class="sxs-lookup"><span data-stu-id="21251-130">Prorate fees when purchase</span></span> | <span data-ttu-id="21251-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="21251-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="21251-132">Tariffa di acquisto</span><span class="sxs-lookup"><span data-stu-id="21251-132">Purchase fee</span></span> | <span data-ttu-id="21251-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="21251-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="21251-134">Rateizza la tariffa al rinnovo</span><span class="sxs-lookup"><span data-stu-id="21251-134">Prorate fee when renew</span></span> | <span data-ttu-id="21251-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="21251-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="21251-136">Tariffa di rinnovo</span><span class="sxs-lookup"><span data-stu-id="21251-136">Renew fee</span></span> | <span data-ttu-id="21251-137">Addebito per il rinnovo di una sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="21251-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="21251-138">Rateizza le tariffe all'attivazione</span><span class="sxs-lookup"><span data-stu-id="21251-138">Prorate fees when activate</span></span> | <span data-ttu-id="21251-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="21251-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="21251-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="21251-140">One-time charges</span></span>

<span data-ttu-id="21251-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="21251-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="21251-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="21251-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="21251-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="21251-144">Nuova</span><span class="sxs-lookup"><span data-stu-id="21251-144">New</span></span> | <span data-ttu-id="21251-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="21251-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="21251-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="21251-146">addQuantity</span></span> | <span data-ttu-id="21251-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="21251-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="21251-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="21251-148">removeQuantity</span></span> | <span data-ttu-id="21251-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="21251-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="21251-150">Annulla</span><span class="sxs-lookup"><span data-stu-id="21251-150">Cancel</span></span> | <span data-ttu-id="21251-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="21251-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="21251-152">Convertire</span><span class="sxs-lookup"><span data-stu-id="21251-152">Convert</span></span> | <span data-ttu-id="21251-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="21251-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="21251-154">Costi di utilizzo</span><span class="sxs-lookup"><span data-stu-id="21251-154">Usage charges</span></span>

<span data-ttu-id="21251-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="21251-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="21251-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="21251-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="21251-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="21251-158">Valuta la tariffa di utilizzo all'annullamento</span><span class="sxs-lookup"><span data-stu-id="21251-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="21251-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="21251-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="21251-160">Valuta la tariffa di utilizzo per il ciclo corrente</span><span class="sxs-lookup"><span data-stu-id="21251-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="21251-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="21251-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="21251-162">Crediti</span><span class="sxs-lookup"><span data-stu-id="21251-162">Credits</span></span>

<span data-ttu-id="21251-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="21251-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="21251-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="21251-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="21251-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="21251-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="21251-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="21251-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="21251-168">Compensa una voce</span><span class="sxs-lookup"><span data-stu-id="21251-168">Offset a line item</span></span> | <span data-ttu-id="21251-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="21251-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="21251-170">Sconti in base all'uso</span><span class="sxs-lookup"><span data-stu-id="21251-170">Usage-based discounts</span></span>

<span data-ttu-id="21251-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="21251-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="21251-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="21251-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="21251-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="21251-174">Sconto attivazione</span><span class="sxs-lookup"><span data-stu-id="21251-174">Activation discount</span></span> | <span data-ttu-id="21251-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="21251-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="21251-176">Sconto ciclo</span><span class="sxs-lookup"><span data-stu-id="21251-176">Cycle discount</span></span> | <span data-ttu-id="21251-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="21251-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="21251-178">Sconto rinnovo</span><span class="sxs-lookup"><span data-stu-id="21251-178">Renew discount</span></span> | <span data-ttu-id="21251-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="21251-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="21251-180">Annulla sconto</span><span class="sxs-lookup"><span data-stu-id="21251-180">Cancel discount</span></span> | <span data-ttu-id="21251-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="21251-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="21251-182">Sconti in base alle licenze</span><span class="sxs-lookup"><span data-stu-id="21251-182">License-based discounts</span></span>

<span data-ttu-id="21251-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="21251-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="21251-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="21251-184">*License-based discounts may be applied to multiple charge types.*</span></span>
