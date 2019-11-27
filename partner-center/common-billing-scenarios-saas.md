---
title: Scenari di fatturazione comuni per le transazioni SaaS basate su licenze | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Scenari di fatturazione comuni nel centro per i partner per le transazioni SaaS basate su licenze.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: fatturazione, pagamenti, acquisto monouso, acquisto ricorrente, sottoscrizioni, postazioni
ms.localizationpriority: medium
ms.openlocfilehash: b808a3bbfc0856e03f1c775d7e3145a29c2239fb
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389609"
---
# <a name="billing-scenarios-for-license-based-saas-transactions"></a>Scenari di fatturazione per le transazioni SaaS basate su licenze

Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili alle sottoscrizioni SaaS (License-based software as a Service) nel centro per i partner.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertire una sottoscrizione SaaS di valutazione gratuita in una sottoscrizione a pagamento

Questo scenario descrive la fatturazione per il rinnovo di una sottoscrizione SaaS di valutazione gratuita basata su licenza. Il rinnovo converte la versione di valutazione gratuita in una sottoscrizione a pagamento al termine del periodo di valutazione gratuita.

In questo esempio è stata acquistata una versione di valutazione gratuita di una sottoscrizione SaaS (Software as a Service) basata su licenza il 10 giugno. Questa versione di valutazione gratuita viene rinnovata automaticamente come sottoscrizione a pagamento al termine del periodo di valutazione gratuita.

I file di ricognizione includeranno gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 1 | $ 0 | Nuova | Versione di prova gratuita |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $ 2 | 1 | $ 2 | Rinnova | Sottoscrizione a pagamento |

## <a name="cancel-a-free-trial-saas-subscription"></a>Annulla una sottoscrizione SaaS per la versione di valutazione gratuita

> [!TIP]
> È possibile annullare una sottoscrizione SaaS della versione di valutazione gratuita basata su licenze in qualsiasi momento, anche durante il periodo di valutazione gratuita.

In questo scenario è stata acquistata una sottoscrizione SaaS per la versione di valutazione gratuita basata su licenza il 1 ° luglio, che è stata quindi annullata immediatamente nel centro per i partner. 

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Nuova | Versione di prova gratuita |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Cancel | Versione di prova gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertire una sottoscrizione SaaS per il contatore personalizzato in un altro SKU

Questo scenario descrive come convertire una sottoscrizione SaaS di misurazione personalizzata da un'unità di conservazione (SKU) a un altro SKU per lo stesso prodotto, nella stessa data.

In questo scenario è stato acquistato uno SKU (Silver) in un prodotto e lo si è convertito in un altro SKU disponibile (bronzo) in questo prodotto nella stessa data.

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | $ 20 | Nuova | Sottoscrizione SaaS del contatore personalizzato |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | -$20 | Convertire | Rifatturato in base alla sottoscrizione SaaS personalizzata del contatore |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Convertire | Sottoscrizione SaaS del contatore personalizzato |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Acquistare e annullare una sottoscrizione SaaS del contatore clienti nella stessa data

Questo scenario descrive la fatturazione per una sottoscrizione SaaS del contatore clienti acquistata e annullata tramite il portale di Azure nella stessa data.

In questo scenario è stata acquistata una sottoscrizione SaaS personalizzata Meter nel portale di Azure. La sottoscrizione è stata quindi annullata nella stessa data.

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Nuova | Sottoscrizione SaaS del contatore personalizzato |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | -$10 | CancelImmediate | Sottoscrizione SaaS del contatore personalizzato |
