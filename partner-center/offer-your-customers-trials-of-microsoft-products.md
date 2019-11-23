---
title: Offrire ai clienti le versioni di valutazione dei prodotti Microsoft | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I tuoi clienti possono testare i prodotti a sottoscrizione Microsoft per 30 giorni. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384836"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Offrire ai clienti le versioni di valutazione dei prodotti Microsoft

Si applica a:

- Centro per i partner

Un buon metodo per presentare ai clienti i nuovi prodotti Microsoft è offrire versioni di valutazione gratuite di 30 giorni. Puoi registrarti per le versioni di valutazione nel catalogo esattamente come per molti altri servizi online. Tutti i partner.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Possono ad esempio ottenere una versione di valutazione gratuita per Office 365 Business Premium e un'altra per Office 365 E3. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

Sono disponibili versioni di valutazione gratuite per i seguenti prodotti:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Piano 1
- Dynamics 365 for Financials
- Microsoft 365 Business

Offriamo versioni di valutazione gratuite per questi prodotti perché sono le offerte aziendali più complete e popolari. È possibile che in futuro siano disponibili altre offerte di versioni di valutazione gratuite.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. Nel catalogo fai clic su **Trial offer** in **Frequenza fatturazione**. Questa operazione consente di abilitare solo le versioni di valutazione gratuite e disabilitare altre offerte non gratuite. Le versioni di valutazione verranno visualizzate nella scheda **Versioni di valutazione** del catalogo.
3. Seleziona la versione di valutazione gratuita che desideri offrire, quindi seleziona **Invia**. Tutte le versioni di valutazione sono valide per 30 giorni e durante questo periodo non ti verrà addebitato alcun costo. Inoltre puoi convertirla in una sottoscrizione a pagamento in qualsiasi momento durante il periodo della versione di valutazione.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Vai alla pagina della sottoscrizione del cliente e seleziona la versione di valutazione gratuita.
2. Seleziona **Convertire una versione di valutazione in sottoscrizione a pagamento**
3. Immetti il numero di licenze desiderato e la frequenza di fatturazione, quindi seleziona **Applica**.
4. La fatturazione per la sottoscrizione a pagamento inizia alla data di conversione e la sottoscrizione si rinnova automaticamente dopo 12 mesi dalla data di conversione. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Convertire una sottoscrizione di valutazione in una a pagamento](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Ottenere un elenco delle offerte di conversione della copia di valutazione](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. È consigliabile monitorare queste date di frequente in modo da poter intraprendere le azioni appropriate quando si avvicinano i momenti critici in cui i clienti devono prendere una decisione.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Fatturazione

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione annuale, la data di rinnovo dell'abbonamento cade 12 mesi dopo la data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione mensile, la data di rinnovo dell'abbonamento cade 12 mesi dopo la data di fatturazione successiva alla data di conversione.

### <a name="invoices"></a>Fatture

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Incentivi

Free trials do not have an impact on incentives.

## <a name="support"></a>Supporto tecnico

For support on free trials, submit a service request through Partner Center.
