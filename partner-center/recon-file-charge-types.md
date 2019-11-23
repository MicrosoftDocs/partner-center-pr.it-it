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
# <a name="understand-charge-types"></a>Understand charge types

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file. Your invoice provides a summary of charges. Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types. For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).

Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).

> [!NOTE]
> One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.

## <a name="map-charge-types-to-invoice-charges"></a>Map charge types to invoice charges

To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel. Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.

## <a name="license-based-charges"></a>Addebiti in base alle licenze

To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Commissione di attivazione | The amount charged to the customer when they use the subscription after purchase. |
| Commissione di annullamento | Prorated charges refunded to the customer when associated seats are changed. |
| Tariffa periodica | Periodic charges for a subscription. |
| Ripartizione dell'istanza del ciclo | Prorated charges assessed from the customer when associated seats are changed. |
| Rateizza le tariffe in caso di annullamento | Prorated refund for unused portion of service upon cancellation. |
| Ripartizione delle tariffe all'acquisto | The charge type for a subscription when using annual billing. |
| Tariffa di acquisto | The charge type for a subscription when using monthly billing. |
| Rateizza la tariffa al rinnovo | Prorated fees upon subscription renewal. |
| Tariffa di rinnovo | Addebito per il rinnovo di una sottoscrizione |
| Rateizza le tariffe all'attivazione | >Prorated fees from activation until end of billing period. |

## <a name="one-time-charges"></a>One-time charges

To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Nuova | Used when a new purchase is created. |
| addQuantity | Used in both the refund of the original purchase and the new quantity after an increase. |
| removeQuantity | Used in both the refund of the original purchase and the new quantity after a decrease. |
| Annulla | Used when a subscription is cancelled. |
| Convertire | Used when a license is upgraded but the number of seats remains unchanged. |

## <a name="usage-charges"></a>Costi di utilizzo

To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Valuta la tariffa di utilizzo all'annullamento | Access usage fee upon cancellation for unpaid usage during the current billing period. |
| Valuta la tariffa di utilizzo per il ciclo corrente | Access usage fee for the current billing period. |

### <a name="credits"></a>Crediti

To map these credits to your invoice:

- Sum the **TotalForCustomer** from the license-based file.
- Sum the **PostTaxTotal** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Compensa una voce | Partial or whole refund to a line item, including taxes. |

### <a name="usage-based-discounts"></a>Sconti in base all'uso

To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| Sconto attivazione | Discount applied when subscription activated. |
| Sconto ciclo | Discount applied on periodic charges. |
| Sconto rinnovo | Discount applied when subscription renewed. |
| Annulla sconto | Charges applied when discounts cancelled. |

### <a name="license-based-discounts"></a>Sconti in base alle licenze

To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.

*License-based discounts may be applied to multiple charge types.*
