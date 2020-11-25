---
title: Acquista offerte per Marketplace commerciali
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sul modo in cui i partner del programma CSP possono usare il centro per i partner per l'acquisto di offerte SaaS da parte dei fornitori di software indipendenti (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d8eb2faec7c2ddd70ed0cacedebf4f9824441a7a
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038857"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Acquistare prodotti Marketplace commerciali per i clienti nel centro per i partner

**Si applica a**

- Centro per i partner
- Partner aderenti al programma CSP

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

Un partner del programma Cloud Solution Provider (CSP) può utilizzare il Marketplace commerciale per acquistare sottoscrizioni per i clienti a determinati prodotti SaaS (software as a Service) offerti da fornitori di software indipendenti (ISV).

Offrendo sottoscrizioni SaaS ISV ai tuoi clienti, puoi contribuire a differenziare il tuo business. È anche possibile concedere ai clienti l'accesso ai bundle software che risolvono le specifiche esigenze aziendali. È possibile gestire le licenze e le sottoscrizioni per questi prodotti SaaS del Marketplace dagli editori ISV proprio come si gestiscono le licenze e le sottoscrizioni per i prodotti Microsoft.

È possibile acquistare sottoscrizioni Saas **basate su licenza** o sottoscrizioni **basate sull'utilizzo** . Per ulteriori informazioni sulla differenza tra la fatturazione basata su licenze e l'utilizzo, vedere [nozioni fondamentali sulla fatturazione](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Acquistare sottoscrizioni SaaS basate su licenza e a consumo nel centro per i partner

Le sottoscrizioni vengono acquistate per i prodotti SaaS basati su licenza o a consumo offerti dagli editori ISV utilizzando lo stesso processo utilizzato per acquistare le sottoscrizioni per i prodotti Microsoft.

Per acquistare una sottoscrizione SaaS basata su licenza o a consumo nel centro per i partner, vedere [creare, sospendere o annullare le sottoscrizioni dei clienti](create-a-new-subscription.md#create-a-new-subscription).

Puoi anche possibile usare le [API del Centro per i partner](/partner-center/develop/) per creare sottoscrizioni del Marketplace commerciale per i clienti. (Per altre informazioni sull'uso delle API del centro per i partner, vedere [creare una sottoscrizione per prodotti Marketplace commerciali](/partner-center/develop/create-subscription-azure-marketplace-products)).

>[!IMPORTANT]
> Come partner del programma CSP, è possibile acquistare sottoscrizioni Saas **basate su licenza** o a **consumo** dagli editori ISV all'interno del centro per i partner. Ciò significa che è possibile acquistare qualsiasi offerta SaaS **basata su licenza** o a **consumo** che l'editore ISV ha reso disponibile, incluse le [offerte esclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a cui si ha accesso. Per acquistare o gestire altre offerte di Marketplace commerciali dagli ISV, ad esempio offerte basate sull'utilizzo che coinvolgono applicazioni, contenitori o macchine virtuali di Azure, è necessario passare al [portale di Azure](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Acquistare sottoscrizioni basate sull'utilizzo nel portale di Azure

Diversamente dalle sottoscrizioni SaaS basate su licenza di autori ISV di terze parti, le sottoscrizioni basate sull'utilizzo richiedono prima di tutto una sottoscrizione di Azure. Fatturazione per il Marketplace commerciale, le risorse basate sull'utilizzo sono soggette alla sottoscrizione di Azure del cliente. Quando il cliente ha una sottoscrizione di Azure, un partner del programma CSP può seguire questa procedura per acquistare una sottoscrizione di Marketplace commerciale:

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **Customers** dal menu a sinistra.

2. Selezionare il cliente specifico, quindi selezionare **sottoscrizioni**.  

3. In **sottoscrizioni basate su utilizzo** selezionare **tutte le risorse**. In questo modo si passa al portale di gestione di Azure.

4. Nel portale di gestione di Azure selezionare **Crea una risorsa** dal menu a sinistra.

5. Selezionare **Visualizza tutto** nella parte superiore dell'elenco di Azure Marketplace.

6. Per restringere l'elenco, usare i filtri nella parte superiore dell'elenco del Marketplace. È ad esempio possibile selezionare **Microsoft** o **partner** dall'elenco a discesa **editore** per visualizzare solo le offerte di Microsoft o quelle di un editore ISV.

7. Scegliere un'offerta specifica, quindi selezionare **Crea**.

## <a name="next-steps"></a>Passaggi successivi

- [Gestisci le offerte del Marketplace commerciale](csp-commercial-marketplace-purchase.md)