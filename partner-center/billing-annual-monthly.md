---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389769"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>Applicabilità

Most licensed-based subscriptions have the option for either monthly or annual billing option. Gli abbonamenti basati su utilizzo hanno solo l'opzione di fatturazione mensile.

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

La fatturazione annuale offre i vantaggi seguenti:

- Maggiore flessibilità nelle opzioni di pagamento.
- Migliore allineamento con la fatturazione dei clienti.
- Impatto ridotto delle fluttuazioni di valuta.
- Costi operativi di fatturazione ridotti.

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

Per utilizzare la fatturazione annuale è necessario apportare alcune modifiche alle API.

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. Puoi tuttavia rinominare un'offerta con un nome descrittivo per il cliente per distinguerne il tipo.

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. A questo punto puoi scegliere l'opzione di fatturazione annuale. When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

La fattura verrà emessa alla data di fatturazione successiva. For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. Il periodo del servizio inizia il giorno in cui viene creato l'abbonamento.  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

La fattura verrà emessa alla data di fatturazione successiva alla data di rinnovo dell'abbonamento. Se, ad esempio, acquisti un abbonamento con fatturazione annuale addebitato il 15 gennaio 2018 e la data di fatturazione è il 20 gennaio, l'abbonamento verrà rinnovato il 15 gennaio 2019. La fattura per il rinnovo verrà addebitata il 20 gennaio 2019.

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. Alcune offerte sono limitate a un abbonamento per cliente. Se l'offerta non è limitata, un cliente può avere più abbonamenti della stessa offerta con frequenze di fatturazione diverse. Puoi trovare i dettagli di tutti i limiti e le restrizioni delle offerte nella colonna I della matrice dell'offerta. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. Questi abbonamenti sono diversi da quelli con fatturazione mensile che invece prevedono un periodo gratuito a partire dalla data di acquisto fino alla successiva data di fatturazione.

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

Puoi modificare la quantità di licenze per gli abbonamenti in qualsiasi momento. L'aggiunta di altre licenze non influirà sulla frequenza di fatturazione.

Puoi aggiungere o rimuovere licenze in qualsiasi momento.  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. Quando acquisti un abbonamento con fatturazione annuale, eventuali licenze aggiuntive seguiranno la stessa frequenza di fatturazione. Se quindi devi acquistare licenze con fatturazione mensile, dovrai acquistare un nuovo abbonamento.

### <a name="add-on-offers"></a>Add-on offers

L'abbonamento per un componente aggiuntivo avrà automaticamente la stessa frequenza di fatturazione dell'abbonamento principale. Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

I criteri di annullamento sono identici per tutte le frequenze di fatturazione.

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. Questo si applica a entrambi i tipi di abbonamenti fatturati mensilmente e annualmente.

Il nuovo partner deve acquistare una nuova sottoscrizione per conto del cliente. It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. Riceverai un addebito ripartito proporzionalmente alla data di fatturazione successiva. La data di rinnovo dell'abbonamento rimane invariata.

## <a name="pricing"></a>Prezzi

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). Quando un abbonamento viene rinnovato, il prezzo viene reimpostato in base al listino prezzi corrente alla data di rinnovo. The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

Se non vengono apportate modifiche all'abbonamento, non verrà visualizzata alcuna riga nei file di riconciliazione per i mesi da due a dodici del periodo di validità dell'abbonamento. If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. alla prima data di fatturazione dopo il rinnovo.

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. Se l'annullamento si verifica dopo i primi 30 giorni, la sottoscrizione verrà accreditata proporzionalmente.

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. Puoi calcolare il prezzo annuale moltiplicando per dodici il prezzo mensile.

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>Incentivi

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. I pagamenti degli incentivi realizzati verranno visualizzati in base ai criteri disponibili nelle nostre guide agli incentivi CSP.

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>Proventi

Currently, all incentive payments are made twice a year. 45 giorni dopo la fine del semestre.

### <a name="rates"></a>Tariffe

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>Contatti

For questions about incentives, contact the appropriate regional incentives support team:

| Area geografica | Indirizzo e-mail |
| ------ | ------------- |
| America del Nord | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| Giappone | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
