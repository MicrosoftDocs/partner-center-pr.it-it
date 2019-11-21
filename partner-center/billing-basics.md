---
title: Billing overview | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn basic billing scenarios in Partner Center for Azure subscriptions and reservations and the differences between license-based and usage-based billing.
author: LauraBrenner
ms.author: labrenne
keywords: fatturazione, pagamenti, ordini, annullamento, gestione degli ordini, insolvenza, frode, utilizzo improprio, imposta, esenzioni fiscali, file di riconciliazione, file riconciliazione
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2087b75419e0f5235e1efcc67ecdd8f203f382c1
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253204"
---
# <a name="billing-overview"></a>Billing overview

**Si applica a**

-  Centro per i partner
-  Partner aderenti al programma CSP

Depending on the products, solutions, and services you buy on behalf of your customers, you'll be billed for these purchases in one or more of the following ways:
-   [License-based billing](#licensebasedbilling)

    When you buy products or online services that require licenses, you're billed for each license you bought (not on license usage). You can choose whether to be billed once a month or once a year. If your business needs change, you can switch from one to the other and back again. 
    
    For more information about monthly vs. annual billing, see the billing [FAQ](https://docs.microsoft.com/partner-center/faq-about-new-billing-features).

-   [Usage-based billing](#usagebasedbilling)

    When you buy online services such as Azure subscriptions, you're billed for monthly usage rates. Only monthly billing is available for usage-based products. Usage-based services, such as Azure, are billed according to metered rates, based on consumption.

-   [One-time billing](#onetimebilling)

    When you buy Azure reservations or other software subscriptions, you pay in advance for a pre-set term. Because you're paying in advance, you're billed in one lump sum. 
    
If you've chosen to be billed monthly or if you've bought usage-based products that are billed monthly, your monthly billing date is the day of the month you selected when you created your CSP account on Partner Center. After you've successfully created your CSP account, Microsoft will send a confirmation email that includes your billing date. Once created, this date cannot be changed. 

## <a name="pricing-and-invoicing"></a>Pricing and invoicing
I listini prezzi sono disponibili con un (1) mese di anticipo, dato che vengono aggiornati mensilmente. I prezzi in base alle licenze sono garantiti per l'intera durata dell'abbonamento, in genere 12 mesi dalla data di acquisto. I prezzi in base all'uso possono variare di mese in mese. 

Prices for products, services, and software subscriptions are guaranteed through the subscription duration, however prices may change when you renew.

Vedrai le rettifiche e i crediti posticipati nella fattura successiva, dopo l'applicazione del credito o della rettifica.

Puoi visualizzare e scaricare le fatture e i file riconciliazione dalla pagina Fatturazione nel Centro per i partner. Nota che le fatture mensili sono disponibili nel Centro per i partner entro quattro (4) giorni dalla data di fatturazione selezionata.

## <a name="payment-terms"></a>Condizioni di pagamento

Payment terms are net 60 days. Invoices must be paid by the invoice due date (60 days after the billing date), or your account will be delinquent, which may impact your enrollment in CSP. You can regain full functionality of your suspended accounts when you pay the past due amount.

### <a name="tax"></a>Imposta

You are taxed based on your details, (not your customers') as the billing relationship is between Microsoft and you. You can submit your tax ID during the account setup process or by submitting a support request later. Le modifiche saranno riportate nel ciclo di fatturazione successivo.

-   For withholding and sales tax exemption, you must submit tax documentation through a support request. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

-   For value added tax (VAT) exemption, you must submit your VAT ID (validated by Microsoft) via a service request. Le modifiche e i rimborsi appropriati saranno visibili nel ciclo di fatturazione successivo.

You can find further tax details from your local tax office or tax advisor.

## <a href="" id="licensebasedbilling"></a>License-based billing

When you buy a license-based product on behalf of a customer, you can choose to be billed monthly or annually. If you want to change your billing frequency at a later time, use the procedure below. 

Switching from monthly billing to annual billing is useful if you have numerous subscriptions that are billed monthly and you want to align them to a common billing date. Switching from annual billing to monthly billing is useful in tailoring your billing dates to those of your individual customers. 

When you change the billing frequency, the annual term is updated to reflect the date you changed the billing frequency and a new renewal date is established. 

You can change the billing frequency whenever your business needs change. 

### <a name="billing-rules-for-annual-billing"></a>Billing rules for annual billing

-   Le sottoscrizioni sono annuali e rinnovate automaticamente.

-   La fatturazione avviene in 12 rate mensili o con un pagamento annuo per ogni sottoscrizione annuale.

-   La fatturazione avviene in anticipo per il periodo di fatturazione successivo per i servizi in base alle licenze, in base al numero di licenze alla fine del periodo di fatturazione precedente.

-   Eventuali modifiche del numero di licenze verranno addebitate/accreditate posticipatamente (con un calcolo proporzionale basato su licenza/giorni). Per il calcolo proporzionale viene usata la formula seguente: [ARROTONDA((ARROTONDA(Prezzo unitario * Quantità / Numero di giorni nel mese della ripartizione, 2) * Numero di giorni per la ripartizione) / Quantità, 2) * Quantità]

-   Payments are billed for licenses sold (not licenses provisioned).

### <a name="to-change-the-billing-frequency-of-an-online-service"></a>To change the billing frequency of an online service

1.  Select **Customers** from the Partner Center menu and then select the customer with the subscription you want to change. 

2.  On the customer's Subscriptions page, select the subscription you want to change. 

3.  On the details page, under **Billing frequency**, select **Monthly** or **Annual**. You'll see a confirmation page with important information about changing billing frequency, as well as a list of the subscriptions about to be changed. 

4.  Select **OK** to make the change, or **Cancel** to undo it. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

Microsoft does not charge early termination fees for cancellation of license-based services. 

I crediti per l'annullamento dei servizi in base alle licenze vengono calcolati in modo proporzionale per i giorni inutilizzati nel caso di annullamenti precedenti alla data di scadenza (così come le riduzioni di licenze in base alla formula precedente).

## <a href="" id="usagebasedbilling"></a>Usage-based billing

Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used. For example, Microsoft Azure uses this model. 

### <a name="billing-rules"></a>Regole per la fatturazione
-   Subscriptions are month-to-month and automatically renew at the new metered service rates. You're billed each month for the previous month's usage.

-   Le tariffe per i servizi a consumo possono variare all'interno del ciclo di fatturazione. 

    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni

    -   Riduzioni del prezzo: attive dal giorno della modifica.

    -   Per le sottoscrizioni esistenti verranno usate le tariffe in vigore all'inizio del ciclo di fatturazione.

    -   New subscriptions, when created within the same billing cycle, use the rate in effect on the date you create them. 

### <a name="adjustmentscreditscancellations"></a>Rettifiche/crediti/annullamenti

I pagamenti con rettifiche compariranno nella fattura mensile successiva.

Microsoft does not charge early termination fees for cancellation of usage-based services. 

I crediti di qualsiasi tipo, inclusi quelli per il contratto di servizio, compariranno nella fattura mensile successiva.

## <a href="" id="onetimebilling"></a>One-time billing

You can purchase software subscriptions and Azure reservations in advance, for one- or three-year terms. When you purchase in advance, you're billed for the entire cost in a one-lump sum. This type of billing is called one-time billing.

>[!IMPORTANT]
>If you purchase Azure reservations and/or software subscriptions for a customer in a location with a currency different from yours, the default billing currency is based on the customer's location, not your location. If you have customers in multiple locations, you'll receive separate invoices and reconciliation files for each currency customers need to be billed in, allowing you to invoice your customers in the appropriate currency. 

### <a name="manage-your-one-time-billing"></a>Gestire la fatturazione una tantum

**View your current billing status, invoices, and recon files**

1.  In Partner Center, select **Billing** and then **One time** to view your billing status. 

2.  Seleziona una fattura o un file di riconoscimento per visualizzare informazioni più dettagliate. 

**View a customer's order history**

1.  Select **Customers** from the Partner Center menu.

2.  On your **Customers** page, find the customer whose order history you want to view and then select the down arrow to expand the customer's record. 

3.  Seleziona **Visualizza ordini** per visualizzare la cronologia degli ordini.

**Download a credit note**

If you need to request a credit or rebill, we'll give you a credit note to cancel the original invoice. You might request a credit/rebill for the following reasons:

-   Correzioni all'ordine di acquisto o all'indirizzo

-   La fattura è stata generata e quindi è stato applicato un rimborso d'imposte. Puoi richiedere un credito/rifatturazione per ottenere il rimborso fiscale a fronte della fattura originale. Ciò vale anche per i rimborsi, in quanto puoi richiedere un credito/rifatturazione della fattura originale e quindi ottenere un rimborso.
