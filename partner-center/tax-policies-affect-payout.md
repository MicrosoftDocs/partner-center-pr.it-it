---
title: Impatto dei criteri fiscali sui pagamenti per Azure Marketplace
description: Informazioni su come i criteri fiscali influiscono sui Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489969"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Impatto dei criteri fiscali sui pagamenti per Azure Marketplace

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore

## <a name="introduction"></a>Introduzione

Il marketplace commerciale Microsoft ha una copertura globale. Le transazioni si verificano oltre i confini e a seconda della posizione del fornitore di software indipendente (ISV) e del cliente, le implicazioni fiscali possono variare. Microsoft AppSource e Azure Marketplace le informazioni Partner Center profilo fiscale per determinare il paese dell'ISV. Per determinare il paese del cliente, usare le informazioni di fatturazione del cliente o, se il cliente si trova nell'Unione Europea, vengono usate due informazioni diverse.

Per comprendere meglio gli scenari seguenti, vedere la tabella [Dettagli](tax-details-marketplace.md) fiscali, che mostra se Microsoft raccoglie e paga le imposte per conto dell'editore o se tale responsabilità appartiene all'editore.

> [!NOTE]
> Tutti gli esempi di valori di vendita e percentuali fiscali in questo argomento sono solo a scopo illustrativo, non per cifre esatte.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher Transacts in Microsoft-managed Tax Country

**Scenario A:** transazioni che si svolgono tra un editore e un cliente in un paese fiscale [gestito da Microsoft.](tax-details-marketplace.md#microsoft-managed-countries) Queste transazioni avranno l'imposta applicabile aggiunta al momento della vendita e Microsoft invia tale imposta al paese applicabile. Nessuna imposta viene trattenuta dai pagamenti e i calcoli dei pagamenti sono escludono le imposte.

Vedere [Lo scenario D](#foreign-publisher-transacts-with-us-customer) per le transazioni tra un editore non statunitense e un cliente degli Stati Uniti.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service

**Scenario B:** transazioni che si verificano tra un editore basato negli Stati Uniti (come definito dalle informazioni sul profilo fiscale Partner Center) a un cliente in un paese fiscale gestito da Microsoft in cui il paese impone un'imposta sulla tariffa del Marketplace (un servizio imponibile). In questo scenario, l'imposta sulla tariffa del servizio del negozio viene sottratta dal pagamento dell'editore.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra il flusso di lavoro per lo scenario B del processo di pagamento.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher Transacts in Publisher-managed Tax Country

**Scenario C:** transazioni che si svolgono tra un editore e un cliente in un paese fiscale gestito dall'editore che non impone una ritenuta d'acconto ai clienti. I clienti non pagano alcuna imposta al punto di vendita ed è obbligatorio dell'editore pagare tutte le imposte applicabili.

Per altre informazioni sui prezzi specifici del paese (ad esempio, per compensare le imposte imminenti), vedere Piani e prezzi per le [offerte del marketplace commerciale.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**Scenario D:** tutti gli editori estere (come definito dalle informazioni sul profilo fiscale Partner Center) in paesi senza trattato degli Stati Uniti (vedere [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) che effettuano una vendita a un cliente con sede negli Stati Uniti (come definito dall'indirizzo dell'account del cliente). Il governo degli Stati Uniti richiede la ritenuta d'acconto di Microsoft per conto dell'editore. Le imposte trattenute dal pagamento all'editore vengono calcolate in base al prezzo dell'offerta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Editore estraneo con un'accordo con il cliente degli Stati Uniti

**Scenario E:** tutti gli editori estere (come definito dalle informazioni sul profilo fiscale Partner Center) nei paesi con un trattato degli Stati Uniti che effettuano una vendita a un cliente con sede negli Stati Uniti (come definito dall'indirizzo dell'account del cliente). Il governo degli Stati Uniti non richiede a Microsoft di ritenuta d'acconto per conto dell'editore.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>L'editore estraneo vende a un cliente ue con partita IVA in un paese gestito da Microsoft (al di fuori dell'Irlanda)

Scenario F: tutte le transazioni tra editori esterni e clienti con imposta sul valore aggiunto dell'UNIONE **(IVA)** registrati (al di fuori dell'Irlanda) in un Microsoft-Managed paese. Il cliente non paga le imposte sulla vendita.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>L'editore estraneo vende a un cliente con partita IVA ue in un paese gestito da Microsoft (in Irlanda)

**Scenario G:** tutte le transazioni tra editori e clienti con iva ue (all'interno dell'Irlanda) in un Microsoft-Managed paese. Il cliente paga l'IVA in Irlanda e Microsoft paga questa imposta al governo dell'Irlanda.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento G.":::

## <a name="next-steps"></a>Passaggi successivi

- [Domande frequenti sul server di pubblicazione](/azure/marketplace/marketplace-faq-publisher-guide)
- [Istruzioni per la creazione di profili di pagamento e fiscali](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)