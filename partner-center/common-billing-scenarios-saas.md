---
title: Fatturazione - Transazioni SaaS basate su licenza
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sugli scenari di fatturazione comuni Partner Center transazioni SaaS (Software-as-a-Service) basate su licenza.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148636"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Scenari di fatturazione comuni per le transazioni SaaS basate su licenza in Partner Center

**Ruoli appropriati:** agente di amministrazione | Amministratore fatturazione | Agente del supporto | Agente di vendita


Questi scenari [di fatturazione comuni di](common-billing-scenarios.md) esempio sono applicabili alle sottoscrizioni saaS (Software as a Service) basate su licenza in Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertire una sottoscrizione SaaS di valutazione gratuita in una sottoscrizione a pagamento

Questo scenario descrive la fatturazione per il rinnovo di una sottoscrizione SaaS di valutazione gratuita basata su licenza. Il rinnovo converte la versione di valutazione gratuita in una sottoscrizione a pagamento alla fine del periodo di valutazione gratuita.

In questo esempio è stata acquistata una versione di valutazione gratuita di una sottoscrizione SaaS (Software as a Service) basata su licenza il 10 giugno. Questa versione di valutazione gratuita viene rinnovata automaticamente come sottoscrizione a pagamento al termine del periodo di valutazione gratuita.

I file di ricognizione includeranno gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità di unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 1 | $ 0 | Nuova | Versione di prova gratuita |
| 07/10/2019 | 07/10/2019 | 09/08/2019 | $ 2 | 1 | $ 2 | Renew | Sottoscrizione a pagamento |

## <a name="cancel-a-free-trial-saas-subscription"></a>Annullare una sottoscrizione SaaS di valutazione gratuita

> [!TIP]
> È possibile annullare una sottoscrizione SaaS di valutazione gratuita basata su licenza in qualsiasi momento, anche durante il periodo di valutazione gratuita.

In questo scenario è stata acquistata una sottoscrizione SaaS di valutazione gratuita basata su licenza il 1° luglio e quindi è stata annullata immediatamente in Partner Center.

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità di unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Nuova | Versione di prova gratuita |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Annulla | Versione di prova gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertire la sottoscrizione SaaS del contatore personalizzato in un altro SKU

Questo scenario descrive come convertire una sottoscrizione SaaS del contatore personalizzato da un'unità di mantenimento delle scorte (SKU) a un altro SKU per lo stesso prodotto, nella stessa data.

In questo scenario è stato acquistato uno SKU (Silver) in un prodotto e lo si è convertito in un altro SKU disponibile (Bronze) in questo prodotto nella stessa data.

Il file di ricognizione includerà gli addebiti seguenti:

| Data di acquisto | SKU | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità di unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Argento | 10/06/2019 | 10/06/2019 | $ 20 | 1 | $ 20 | Nuova | Sottoscrizione SaaS del contatore personalizzato |
| 10/06/2019 | Argento | 10/06/2019 | 10/06/2019 | $ 20 | 1 | -$20 | Conversione | Nuova fattura rivalorata per la sottoscrizione SaaS del contatore personalizzato |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Conversione | Sottoscrizione SaaS del contatore personalizzato |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Acquistare e annullare una sottoscrizione SaaS del contatore del cliente nella stessa data

Questo scenario descrive la fatturazione per una sottoscrizione SaaS del contatore del cliente acquistata e annullata tramite il portale di Azure nella stessa data.

In questo scenario è stata acquistata una sottoscrizione SaaS del contatore personalizzato nel portale di Azure. La sottoscrizione è stata quindi annullata nella stessa data.

| Data di acquisto | SKU | Data di inizio addebito | Data di fine addebito | Prezzo unitario | Quantità unità | Importo totale | Tipo di addebito | Descrizione della sottoscrizione |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | $10 | Nuova | Sottoscrizione SaaS del contatore personalizzato |
| 10/06/2019 | Bronzo | 10/06/2019 | 10/06/2019 | $10 | 1 | -$10 | CancelImmediate | Sottoscrizione SaaS del contatore personalizzato |
