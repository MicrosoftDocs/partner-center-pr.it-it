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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="b1f15-103">Impatto dei criteri fiscali sui pagamenti per Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="b1f15-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="b1f15-104">**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="b1f15-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="b1f15-105">Introduzione</span><span class="sxs-lookup"><span data-stu-id="b1f15-105">Introduction</span></span>

<span data-ttu-id="b1f15-106">Il marketplace commerciale Microsoft ha una copertura globale.</span><span class="sxs-lookup"><span data-stu-id="b1f15-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="b1f15-107">Le transazioni si verificano oltre i confini e a seconda della posizione del fornitore di software indipendente (ISV) e del cliente, le implicazioni fiscali possono variare.</span><span class="sxs-lookup"><span data-stu-id="b1f15-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="b1f15-108">Microsoft AppSource e Azure Marketplace le informazioni Partner Center profilo fiscale per determinare il paese dell'ISV.</span><span class="sxs-lookup"><span data-stu-id="b1f15-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="b1f15-109">Per determinare il paese del cliente, usare le informazioni di fatturazione del cliente o, se il cliente si trova nell'Unione Europea, vengono usate due informazioni diverse.</span><span class="sxs-lookup"><span data-stu-id="b1f15-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="b1f15-110">Per comprendere meglio gli scenari seguenti, vedere la tabella [Dettagli](tax-details-marketplace.md) fiscali, che mostra se Microsoft raccoglie e paga le imposte per conto dell'editore o se tale responsabilità appartiene all'editore.</span><span class="sxs-lookup"><span data-stu-id="b1f15-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="b1f15-111">Tutti gli esempi di valori di vendita e percentuali fiscali in questo argomento sono solo a scopo illustrativo, non per cifre esatte.</span><span class="sxs-lookup"><span data-stu-id="b1f15-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="b1f15-112">Publisher Transacts in Microsoft-managed Tax Country</span><span class="sxs-lookup"><span data-stu-id="b1f15-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="b1f15-113">**Scenario A:** transazioni che si svolgono tra un editore e un cliente in un paese fiscale [gestito da Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="b1f15-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="b1f15-114">Queste transazioni avranno l'imposta applicabile aggiunta al momento della vendita e Microsoft invia tale imposta al paese applicabile.</span><span class="sxs-lookup"><span data-stu-id="b1f15-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="b1f15-115">Nessuna imposta viene trattenuta dai pagamenti e i calcoli dei pagamenti sono escludono le imposte.</span><span class="sxs-lookup"><span data-stu-id="b1f15-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="b1f15-116">Vedere [Lo scenario D](#foreign-publisher-transacts-with-us-customer) per le transazioni tra un editore non statunitense e un cliente degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="b1f15-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="b1f15-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span><span class="sxs-lookup"><span data-stu-id="b1f15-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="b1f15-119">**Scenario B:** transazioni che si verificano tra un editore basato negli Stati Uniti (come definito dalle informazioni sul profilo fiscale Partner Center) a un cliente in un paese fiscale gestito da Microsoft in cui il paese impone un'imposta sulla tariffa del Marketplace (un servizio imponibile).</span><span class="sxs-lookup"><span data-stu-id="b1f15-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="b1f15-120">In questo scenario, l'imposta sulla tariffa del servizio del negozio viene sottratta dal pagamento dell'editore.</span><span class="sxs-lookup"><span data-stu-id="b1f15-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Mostra il flusso di lavoro per lo scenario B del processo di pagamento.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="b1f15-122">Publisher Transacts in Publisher-managed Tax Country</span><span class="sxs-lookup"><span data-stu-id="b1f15-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="b1f15-123">**Scenario C:** transazioni che si svolgono tra un editore e un cliente in un paese fiscale gestito dall'editore che non impone una ritenuta d'acconto ai clienti.</span><span class="sxs-lookup"><span data-stu-id="b1f15-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="b1f15-124">I clienti non pagano alcuna imposta al punto di vendita ed è obbligatorio dell'editore pagare tutte le imposte applicabili.</span><span class="sxs-lookup"><span data-stu-id="b1f15-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="b1f15-125">Per altre informazioni sui prezzi specifici del paese (ad esempio, per compensare le imposte imminenti), vedere Piani e prezzi per le [offerte del marketplace commerciale.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="b1f15-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="b1f15-127">Foreign Publisher Transacts with US Customer</span><span class="sxs-lookup"><span data-stu-id="b1f15-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="b1f15-128">**Scenario D:** tutti gli editori estere (come definito dalle informazioni sul profilo fiscale Partner Center) in paesi senza trattato degli Stati Uniti (vedere [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) che effettuano una vendita a un cliente con sede negli Stati Uniti (come definito dall'indirizzo dell'account del cliente).</span><span class="sxs-lookup"><span data-stu-id="b1f15-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="b1f15-129">Il governo degli Stati Uniti richiede la ritenuta d'acconto di Microsoft per conto dell'editore.</span><span class="sxs-lookup"><span data-stu-id="b1f15-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="b1f15-130">Le imposte trattenute dal pagamento all'editore vengono calcolate in base al prezzo dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="b1f15-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="b1f15-132">Editore estraneo con un'accordo con il cliente degli Stati Uniti</span><span class="sxs-lookup"><span data-stu-id="b1f15-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="b1f15-133">**Scenario E:** tutti gli editori estere (come definito dalle informazioni sul profilo fiscale Partner Center) nei paesi con un trattato degli Stati Uniti che effettuano una vendita a un cliente con sede negli Stati Uniti (come definito dall'indirizzo dell'account del cliente).</span><span class="sxs-lookup"><span data-stu-id="b1f15-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="b1f15-134">Il governo degli Stati Uniti non richiede a Microsoft di ritenuta d'acconto per conto dell'editore.</span><span class="sxs-lookup"><span data-stu-id="b1f15-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="b1f15-136">L'editore estraneo vende a un cliente ue con partita IVA in un paese gestito da Microsoft (al di fuori dell'Irlanda)</span><span class="sxs-lookup"><span data-stu-id="b1f15-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="b1f15-137">Scenario F: tutte le transazioni tra editori esterni e clienti con imposta sul valore aggiunto dell'UNIONE **(IVA)** registrati (al di fuori dell'Irlanda) in un Microsoft-Managed paese.</span><span class="sxs-lookup"><span data-stu-id="b1f15-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="b1f15-138">Il cliente non paga le imposte sulla vendita.</span><span class="sxs-lookup"><span data-stu-id="b1f15-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="b1f15-140">L'editore estraneo vende a un cliente con partita IVA ue in un paese gestito da Microsoft (in Irlanda)</span><span class="sxs-lookup"><span data-stu-id="b1f15-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="b1f15-141">**Scenario G:** tutte le transazioni tra editori e clienti con iva ue (all'interno dell'Irlanda) in un Microsoft-Managed paese.</span><span class="sxs-lookup"><span data-stu-id="b1f15-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="b1f15-142">Il cliente paga l'IVA in Irlanda e Microsoft paga questa imposta al governo dell'Irlanda.</span><span class="sxs-lookup"><span data-stu-id="b1f15-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Mostra il flusso di lavoro per lo scenario del processo di pagamento G.":::

## <a name="next-steps"></a><span data-ttu-id="b1f15-144">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b1f15-144">Next steps</span></span>

- [<span data-ttu-id="b1f15-145">Domande frequenti sul server di pubblicazione</span><span class="sxs-lookup"><span data-stu-id="b1f15-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="b1f15-146">Istruzioni per la creazione di profili di pagamento e fiscali</span><span class="sxs-lookup"><span data-stu-id="b1f15-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)