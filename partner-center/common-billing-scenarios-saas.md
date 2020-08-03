---
title: Transazioni SaaS basate su licenze di fatturazione
ms.topic: article
ms.date: 05/05/2020
description: Informazioni sugli scenari di fatturazione comuni nel centro per i partner per le transazioni SaaS basate su licenze.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d65d23057ea0354fc77b1cc8a9c7fb16a343b3ee
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444567"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Scenari di fatturazione comuni per le transazioni SaaS basate su licenze nel centro per i partner

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di supporto tecnico
- Agente di vendita


Questi [scenari di fatturazione comuni](common-billing-scenarios.md) di esempio sono applicabili alle sottoscrizioni SaaS (License-based software as a Service) nel centro per i partner.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertire una sottoscrizione SaaS di valutazione gratuita in una sottoscrizione a pagamento

Questo scenario descrive la fatturazione per il rinnovo di una sottoscrizione SaaS di valutazione gratuita basata su licenza. Il rinnovo converte la versione di valutazione gratuita in una sottoscrizione a pagamento al termine del periodo di valutazione gratuita.

In questo esempio è stata acquistata una versione di valutazione gratuita di una sottoscrizione SaaS (Software as a Service) basata su licenza il 10 giugno. Questa versione di valutazione gratuita viene rinnovata automaticamente come sottoscrizione a pagamento al termine del periodo di valutazione gratuita.

I file di ricognizione includeranno gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 1 | $ 0 | Nuovo | Versione di prova gratuita |
| 07/10/2019 | 07/10/2019 | 09/08/2019 | $ 2 | 1 | $ 2 | Renew | Sottoscrizione a pagamento |

## <a name="cancel-a-free-trial-saas-subscription"></a>Annulla una sottoscrizione SaaS per la versione di valutazione gratuita

> [!TIP]
> È possibile annullare una sottoscrizione SaaS della versione di valutazione gratuita basata su licenze in qualsiasi momento, anche durante il periodo di valutazione gratuita.

In questo scenario è stata acquistata una sottoscrizione SaaS di valutazione gratuita basata su licenza il 1 ° luglio, che è stata quindi annullata immediatamente nel centro per i partner.

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Nuovo | Versione di prova gratuita |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Annulla | Versione di prova gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertire una sottoscrizione SaaS per il contatore personalizzato in un altro SKU

Questo scenario descrive come convertire una sottoscrizione SaaS di misurazione personalizzata da un'unità di conservazione (SKU) a un altro SKU per lo stesso prodotto, nella stessa data.

In questo scenario è stato acquistato uno SKU (Silver) in un prodotto e lo si è convertito in un altro SKU disponibile (bronzo) in questo prodotto nella stessa data.

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | SKU | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Argento | 10/06/2019 | 10/06/2019 | $ 20 | 1 | $ 20 | Nuovo | Sottoscrizione SaaS del contatore personalizzato |
| 10/06/2019 | Argento | 10/06/2019 | 10/06/2019 | $ 20 | 1 | -$20 | Conversione | Rifatturato in base alla sottoscrizione SaaS personalizzata del contatore |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Conversione | Sottoscrizione SaaS del contatore personalizzato |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Acquistare e annullare una sottoscrizione SaaS del contatore clienti nella stessa data

Questo scenario descrive la fatturazione per una sottoscrizione SaaS del contatore clienti acquistata e annullata tramite il portale di Azure nella stessa data.

In questo scenario è stata acquistata una sottoscrizione SaaS personalizzata Meter nel portale di Azure. La sottoscrizione è stata quindi annullata nella stessa data.

| Data di acquisto | SKU | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Nuovo | Sottoscrizione SaaS del contatore personalizzato |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | -$10 | CancelImmediate | Sottoscrizione SaaS del contatore personalizzato |
