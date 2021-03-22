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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="629f3-103">Effetti dei criteri fiscali sui pagamenti per Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="629f3-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="629f3-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="629f3-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="629f3-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="629f3-105">Global admin</span></span>
-    <span data-ttu-id="629f3-106">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="629f3-106">User management admin</span></span>
-    <span data-ttu-id="629f3-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="629f3-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="629f3-108">Introduzione</span><span class="sxs-lookup"><span data-stu-id="629f3-108">Introduction</span></span>

<span data-ttu-id="629f3-109">Microsoft Commercial Marketplace offre una copertura globale.</span><span class="sxs-lookup"><span data-stu-id="629f3-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="629f3-110">Le transazioni si verificano oltre i confini e, a seconda della posizione in cui si trovano gli ISV e i clienti, le implicazioni fiscali possono variare.</span><span class="sxs-lookup"><span data-stu-id="629f3-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="629f3-111">Microsoft AppSource e Azure Marketplace utilizzano le informazioni sul profilo fiscale del centro partner per determinare il paese dell'ISV.</span><span class="sxs-lookup"><span data-stu-id="629f3-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="629f3-112">Per determinare il paese del cliente, utilizzare le informazioni di fatturazione del cliente o, se il cliente si trova nell'Unione europea, vengono utilizzate due diverse informazioni.</span><span class="sxs-lookup"><span data-stu-id="629f3-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="629f3-113">Per comprendere meglio gli scenari seguenti, fare riferimento alla tabella [Dettagli fiscali](tax-details-marketplace.md) , che indica se Microsoft raccoglie e paga le imposte per conto dell'editore o se tale responsabilità appartiene al server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="629f3-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="629f3-114">Tutti gli esempi relativi ai valori di vendita e alle percentuali fiscali in questo argomento sono solo a scopo illustrativo e non a cifre esatte.</span><span class="sxs-lookup"><span data-stu-id="629f3-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="629f3-115">Il server di pubblicazione si transagisce in un paese fiscale gestito da Microsoft</span><span class="sxs-lookup"><span data-stu-id="629f3-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="629f3-116">**Scenario a** : transazioni che avvengono tra un server di pubblicazione e un cliente in un [paese fiscale gestito da Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="629f3-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="629f3-117">Queste transazioni avranno una tassa applicabile aggiuntiva al momento della vendita e Microsoft invierà il fisco al paese applicabile.</span><span class="sxs-lookup"><span data-stu-id="629f3-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="629f3-118">Le imposte non vengono trattenute dai calcoli di pagamento e dei pagamenti.</span><span class="sxs-lookup"><span data-stu-id="629f3-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="629f3-119">Vedere lo [scenario D](#foreign-publisher-transacts-with-us-customer) per le transazioni tra un editore non statunitense e un cliente degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="629f3-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="629f3-121">Il server di pubblicazione si transagisce in un paese fiscale gestito da Microsoft, dove il costo del Marketplace è un servizio</span><span class="sxs-lookup"><span data-stu-id="629f3-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="629f3-122">**Scenario B** : transazioni che avvengono tra un server di pubblicazione basato su US (come definito dalle informazioni del profilo fiscale del centro per i partner) a un cliente in un paese fiscale gestito da Microsoft in cui il paese impone una tassa sul Marketplace (un servizio imponibile).</span><span class="sxs-lookup"><span data-stu-id="629f3-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="629f3-123">In questo scenario, l'imposta sul costo del servizio del negozio viene sottratta dal pagamento del server di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="629f3-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra il flusso di lavoro per il processo di pagamento dello scenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="629f3-125">Il server di pubblicazione si transagisce in un paese fiscale gestito dal server di pubblicazione</span><span class="sxs-lookup"><span data-stu-id="629f3-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="629f3-126">**Scenario C** : transazioni che avvengono tra un server di pubblicazione e un cliente in un paese d'imposta gestito dall'editore che non impone un'imposta di ritenuta per i clienti.</span><span class="sxs-lookup"><span data-stu-id="629f3-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="629f3-127">I clienti non pagano alcuna tassa al punto di vendita ed è l'obbligo dell'editore a pagare tutte le tasse applicabili.</span><span class="sxs-lookup"><span data-stu-id="629f3-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="629f3-128">Per altre informazioni sui prezzi specifici del paese, ad esempio per compensare la tassazione imminente, vedere [piani e prezzi per le offerte per Marketplace commerciali](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="629f3-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="629f3-130">Publisher esterno transagisce con il cliente US</span><span class="sxs-lookup"><span data-stu-id="629f3-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="629f3-131">**Scenario D** : tutti i Publisher stranieri (definiti dalle informazioni relative al profilo fiscale del centro per i partner) in paesi senza un accordo degli Stati Uniti (vedere lo [scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) effettuare una vendita a un cliente basato sugli Stati Uniti (come definito dall'indirizzo dell'account cliente).</span><span class="sxs-lookup"><span data-stu-id="629f3-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="629f3-132">Per il governo degli Stati Uniti è necessario che Microsoft trattenga le imposte per conto dell'editore.</span><span class="sxs-lookup"><span data-stu-id="629f3-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="629f3-133">Il rimborso delle imposte al server di pubblicazione viene calcolato in base al prezzo dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="629f3-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="629f3-135">Publisher esterno con un trattato transagisce con il cliente US</span><span class="sxs-lookup"><span data-stu-id="629f3-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="629f3-136">**Scenario E** : tutti gli editori stranieri (definiti dalle informazioni sul profilo fiscale del centro per i partner) in paesi con un trattato USA che effettuano una vendita a un cliente basato sugli Stati Uniti (come definito dall'indirizzo dell'account cliente).</span><span class="sxs-lookup"><span data-stu-id="629f3-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="629f3-137">Il governo degli Stati Uniti non richiede a Microsoft di sospendere le imposte per conto dell'editore.</span><span class="sxs-lookup"><span data-stu-id="629f3-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="629f3-139">L'editore esterno si vende a un cliente IVA UE registrato in un paese gestito da Microsoft (al di fuori dell'Irlanda)</span><span class="sxs-lookup"><span data-stu-id="629f3-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="629f3-140">**Scenario F** : tutte le transazioni tra gli editori stranieri e i clienti registrati con IVA europea (al di fuori dell'Irlanda) in un paese Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="629f3-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="629f3-141">Il cliente non paga le tasse per la vendita.</span><span class="sxs-lookup"><span data-stu-id="629f3-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra il flusso di lavoro per lo scenario di elaborazione dei pagamenti F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="629f3-143">L'editore esterno si vende a un cliente IVA UE registrato in un paese gestito da Microsoft (in Irlanda)</span><span class="sxs-lookup"><span data-stu-id="629f3-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="629f3-144">**Scenario G** : tutte le transazioni tra gli editori stranieri e i clienti registrati con IVA UE (all'interno dell'Irlanda) in un paese Microsoft-Managed.</span><span class="sxs-lookup"><span data-stu-id="629f3-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="629f3-145">Il cliente paga l'IVA irlandese e Microsoft paga la tassa al governo irlandese.</span><span class="sxs-lookup"><span data-stu-id="629f3-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento G.":::

## <a name="next-steps"></a><span data-ttu-id="629f3-147">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="629f3-147">Next steps</span></span>

- [<span data-ttu-id="629f3-148">Domande frequenti sull'editore</span><span class="sxs-lookup"><span data-stu-id="629f3-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="629f3-149">Istruzioni per la creazione di profili di pagamento e fiscali</span><span class="sxs-lookup"><span data-stu-id="629f3-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)