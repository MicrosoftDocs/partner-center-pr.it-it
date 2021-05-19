---
title: Acquistare offerte del marketplace commerciale
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come i partner del programma CSP possono usare il marketplace Partner Center per effettuare acquisti da parte dei clienti di offerte SaaS da fornitori di software indipendenti (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147854"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Acquistare prodotti del marketplace commerciale per i clienti in Partner Center


**Ruoli appropriati:** amministratore globale | Agente amministratore

I partner del programma Cloud Solution Provider (CSP) possono usare il marketplace commerciale per acquistare sottoscrizioni per i clienti di determinati prodotti SaaS (Software as a Service) offerti da fornitori di software indipendenti (ISV).

Offrendo sottoscrizioni IsV SaaS ai clienti, è possibile differenziare l'azienda. È anche possibile concedere ai clienti l'accesso a aggregazioni software in grado di soddisfare esigenze aziendali specifiche. È possibile gestire licenze e sottoscrizioni per questi prodotti SaaS del marketplace da editori ISV esattamente come si gestiscono le licenze e le sottoscrizioni per i prodotti Microsoft.

È possibile acquistare sottoscrizioni SaaS **basate** su licenza o **sottoscrizioni basate sull'utilizzo.** Per altre informazioni sulla differenza tra fatturazione basata su licenza e fatturazione basata sull'utilizzo, vedere [Nozioni di base sulla fatturazione.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Acquistare sottoscrizioni SaaS basate su licenza e a consumo in Partner Center

È possibile acquistare sottoscrizioni per prodotti SaaS basati su licenza o a consumo offerti da editori ISV usando lo stesso processo utilizzato per acquistare sottoscrizioni per prodotti Microsoft.

Per acquistare una sottoscrizione SaaS basata su licenza o a consumo in Partner Center, vedere Creare, sospendere o annullare [le sottoscrizioni dei clienti.](create-a-new-subscription.md#create-a-new-subscription)

Puoi anche possibile usare le [API del Centro per i partner](/partner-center/develop/) per creare sottoscrizioni del Marketplace commerciale per i clienti. Per altre informazioni sull'uso Partner Center API, vedere Creare una sottoscrizione per [i prodotti del marketplace commerciale.](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> I partner del programma CSP possono  acquistare sottoscrizioni **SaaS** basate su licenza o a consumo da editori ISV all'interno Partner Center. Ciò significa che è possibile acquistare **qualsiasi** offerta **SaaS** basata su licenza o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a consumo resa disponibile dall'editore isv, incluse le offerte esclusive a cui si ha accesso. Per acquistare o gestire altre offerte del marketplace commerciale dagli ISV (ad esempio offerte basate sull'utilizzo che coinvolgono applicazioni di Azure, contenitori o macchine virtuali), è necessario passare al [portale di Azure](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Acquistare sottoscrizioni basate sull'utilizzo nel portale di Azure

A differenza delle sottoscrizioni SaaS basate su licenza di editori ISV di terze parti, le sottoscrizioni basate sull'utilizzo richiedono prima di tutto che un cliente abbia una sottoscrizione di Azure. La fatturazione per il marketplace commerciale, le risorse basate sull'utilizzo rientrano nella sottoscrizione di Azure del cliente. Dopo che il cliente ha una sottoscrizione di Azure, un partner del programma CSP può seguire questa procedura per acquistare una sottoscrizione del marketplace commerciale:

1. Accedere al dashboard Partner Center [e](https://partner.microsoft.com/dashboard)quindi selezionare **Clienti** dal menu a sinistra.

2. Selezionare il cliente specifico, quindi selezionare **Sottoscrizioni**.  

3. In **Sottoscrizioni basate sull'utilizzo** selezionare **Tutte le risorse**. Verrà quindi possibile accedere al portale di gestione di Azure.

4. Nel portale di gestione di Azure selezionare **Crea** una risorsa dal menu a sinistra.

5. Selezionare **Visualizza tutto** nella parte superiore dell'Azure Marketplace elenco.

6. Per restringere l'elenco, usare i filtri nella parte superiore dell'elenco del Marketplace. Ad esempio, è possibile selezionare **Microsoft** o **Partner** nell'elenco a discesa **Editore** per visualizzare solo le offerte di Microsoft o di un editore ISV.

7. Scegliere un'offerta specifica e quindi **selezionare Crea**.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire le offerte del marketplace commerciale](csp-commercial-marketplace-purchase.md)