---
title: Effetti dei criteri fiscali sui pagamenti per Azure Marketplace
description: Informazioni sul modo in cui i criteri fiscali influiscono sui pagamenti per Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768823"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Effetti dei criteri fiscali sui pagamenti per Azure Marketplace

**Ruoli appropriati**
-    Amministratore globale
-    Amministratore gestione utenti
-    Agente amministratore

## <a name="introduction"></a>Introduzione

Microsoft Commercial Marketplace offre una copertura globale. Le transazioni si verificano oltre i confini e, a seconda della posizione in cui si trovano gli ISV e i clienti, le implicazioni fiscali possono variare. Microsoft AppSource e Azure Marketplace utilizzano le informazioni sul profilo fiscale del centro partner per determinare il paese dell'ISV. Per determinare il paese del cliente, utilizzare le informazioni di fatturazione del cliente o, se il cliente si trova nell'Unione europea, vengono utilizzate due diverse informazioni.

Per comprendere meglio gli scenari seguenti, fare riferimento alla tabella [Dettagli fiscali](tax-details-marketplace.md) , che indica se Microsoft raccoglie e paga le imposte per conto dell'editore o se tale responsabilità appartiene al server di pubblicazione.

> [!NOTE]
> Tutti gli esempi relativi ai valori di vendita e alle percentuali fiscali in questo argomento sono solo a scopo illustrativo e non a cifre esatte.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Il server di pubblicazione si transagisce in un paese fiscale gestito da Microsoft

**Scenario a** : transazioni che avvengono tra un server di pubblicazione e un cliente in un [paese fiscale gestito da Microsoft](tax-details-marketplace.md#microsoft-managed-countries). Queste transazioni avranno una tassa applicabile aggiuntiva al momento della vendita e Microsoft invierà il fisco al paese applicabile. Le imposte non vengono trattenute dai calcoli di pagamento e dei pagamenti.

Vedere lo [scenario D](#foreign-publisher-transacts-with-us-customer) per le transazioni tra un editore non statunitense e un cliente degli Stati Uniti.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Il server di pubblicazione si transagisce in un paese fiscale gestito da Microsoft, dove il costo del Marketplace è un servizio

**Scenario B** : transazioni che avvengono tra un server di pubblicazione basato su US (come definito dalle informazioni del profilo fiscale del centro per i partner) a un cliente in un paese fiscale gestito da Microsoft in cui il paese impone una tassa sul Marketplace (un servizio imponibile). In questo scenario, l'imposta sul costo del servizio del negozio viene sottratta dal pagamento del server di pubblicazione.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra il flusso di lavoro per il processo di pagamento dello scenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Il server di pubblicazione si transagisce in un paese fiscale gestito dal server di pubblicazione

**Scenario C** : transazioni che avvengono tra un server di pubblicazione e un cliente in un paese d'imposta gestito dall'editore che non impone un'imposta di ritenuta per i clienti. I clienti non pagano alcuna tassa al punto di vendita ed è l'obbligo dell'editore a pagare tutte le tasse applicabili.

Per altre informazioni sui prezzi specifici del paese, ad esempio per compensare la tassazione imminente, vedere [piani e prezzi per le offerte per Marketplace commerciali](/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Publisher esterno transagisce con il cliente US

**Scenario D** : tutti i Publisher stranieri (definiti dalle informazioni relative al profilo fiscale del centro per i partner) in paesi senza un accordo degli Stati Uniti (vedere lo [scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) effettuare una vendita a un cliente basato sugli Stati Uniti (come definito dall'indirizzo dell'account cliente). Per il governo degli Stati Uniti è necessario che Microsoft trattenga le imposte per conto dell'editore. Il rimborso delle imposte al server di pubblicazione viene calcolato in base al prezzo dell'offerta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Publisher esterno con un trattato transagisce con il cliente US

**Scenario E** : tutti gli editori stranieri (definiti dalle informazioni sul profilo fiscale del centro per i partner) in paesi con un trattato USA che effettuano una vendita a un cliente basato sugli Stati Uniti (come definito dall'indirizzo dell'account cliente). Il governo degli Stati Uniti non richiede a Microsoft di sospendere le imposte per conto dell'editore.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>L'editore esterno si vende a un cliente IVA UE registrato in un paese gestito da Microsoft (al di fuori dell'Irlanda)

**Scenario F** : tutte le transazioni tra gli editori stranieri e i clienti registrati con IVA europea (al di fuori dell'Irlanda) in un paese Microsoft-Managed. Il cliente non paga le tasse per la vendita.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra il flusso di lavoro per lo scenario di elaborazione dei pagamenti F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>L'editore esterno si vende a un cliente IVA UE registrato in un paese gestito da Microsoft (in Irlanda)

**Scenario G** : tutte le transazioni tra gli editori stranieri e i clienti registrati con IVA UE (all'interno dell'Irlanda) in un paese Microsoft-Managed. Il cliente paga l'IVA irlandese e Microsoft paga la tassa al governo irlandese.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento G.":::

## <a name="next-steps"></a>Passaggi successivi

- [Domande frequenti sull'editore](/azure/marketplace/marketplace-faq-publisher-guide)
- [Istruzioni per la creazione di profili di pagamento e fiscali](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)