---
title: Imposizione del limite di credito
ms.topic: how-to
ms.date: 05/11/2021
description: Informazioni sul limite di credito e su come viene calcolato. Include domande frequenti.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819209"
---
# <a name="credit-limit-enforcement-cle"></a>Imposizione del limite di credito (CLE)

**Ruoli appropriati**

- Amministratore fatturazione

## <a name="your-credit-limit-and-how-it-works"></a>Limite di credito e funzionamento

Il limite di credito è l'importo massimo (in dollari STATUNITENSI) che il partner può spendere per acquistare prodotti o sottoscrizioni in Partner Center. Se si supera il limite di credito, non sarà possibile effettuare nuovi acquisti fino a quando non viene effettuato un pagamento sufficiente. Le sottoscrizioni esistenti continueranno senza interruzioni.

I limiti di credito si applicano alle offerte nei prodotti Piano di Azure, Prenotazioni di Azure, Software, Marketplace, Azure 145 P, Office e Dynamics. I limiti di credito non si applicano ai rinnovi e al consumo in corso.

Il limite di credito viene assegnato a livello di tenant durante il periodo di onboarding. Si basa sui ricavi previsti, sulle prodeghe di acquisto e sulla cronologia dei pagamenti. Viene quindi utilizzata la formula seguente per calcolare il saldo disponibile:

**[Limite di credito : (Acquisto in entrata + Fatture non pagate in sospeso + Addebiti non fatturati - Eccedenza pagamento)]**

## <a name="frequently-asked-questions"></a>Domande frequenti

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Il limite di credito è impostato a livello tenant o globale?

Livello del tenant. Si supponga, ad esempio, di operare da Stati Uniti, Canada e Giappone. Se il tenant canadese raggiunge il limite di credito, il tenant riceverà una notifica quando tenterà di effettuare un acquisto Partner Center. Gli altri tenant non saranno interessati. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Se si supera il limite di credito, è possibile continuare a eseguire la manutenzione dei clienti e delle sottoscrizioni esistenti con accesso completo?

Sì. Le sottoscrizioni esistenti dei clienti continueranno senza interruzioni. Non è tuttavia possibile acquistare nuove sottoscrizioni per i clienti.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>CLE si applica sia ai partner con fatturazione diretta che ai provider indiretti?

Sì, si applica a entrambi.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Dopo aver inviato il pagamento per ripristinare l'account, quando è possibile acquistare altre sottoscrizioni? 

Dovrebbe essere possibile riprendere l'acquisto entro 24 ore dal pagamento, presupponendo che Microsoft abbia ricevuto tutti i requisiti per procedere con il processo di verifica del credito.

### <a name="how-can-i-check-my-credit-limit"></a>Come è possibile controllare il limite di credito?

Contattare [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) per visualizzare il limite di credito e ottenere informazioni sugli acquisti recenti.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>Le fatture in conflitto vengono conteggiata rispetto al limite di credito?

Sì. È tuttavia possibile contattare Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) all'indirizzo per risolvere il problema.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Quanto tempo verrà visualizzato se si scrive in ucmwrcsp@microsoft.com ?

Si dovrebbe avere una risposta in meno di 24 ore. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Quali criteri vengono utilizzati da Microsoft per impostare il limite di credito di un partner?

Il limite di credito viene determinato in base ai ricavi previsti, alle prodeghe di acquisto e alla cronologia dei pagamenti.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>Il limite di credito è attualmente applicato alla nuova esperienza commerciale?

Sì. I limiti di credito si applicano a tutti i programmi e prodotti CSP in Partner Center.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Chi riceverà la notifica quando l'organizzazione sta per essere prossima al limite di credito?

La notifica deve essere ricevuta dal contatto Finance Account Payable dell'organizzazione.

## <a name="next-steps"></a>Passaggi successivi

[Nozioni di base sulla fatturazione](./billing-basics.md)
