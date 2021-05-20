---
title: Prenotazioni di Azure & server
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle Cloud Solution Provider di acquisire, effettuare il provisioning e gestire le prenotazioni di Azure e le sottoscrizioni server per i clienti.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 79175fc7e67fdcdc3195b33859f3609c4caf942f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149418"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="ed910-103">Acquisire, effettuare il provisioning e & le istanze di macchina virtuale riservate di Azure e le sottoscrizioni server per i clienti</span><span class="sxs-lookup"><span data-stu-id="ed910-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="ed910-104">**Ruoli appropriati:** agente di amministrazione | Amministratore globale | Agente del supporto | Agente di vendita | Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="ed910-104">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="ed910-105">Informazioni sulle prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-105">What are Azure Reservations?</span></span>

<span data-ttu-id="ed910-106">Le prenotazioni di Azure consentono di risparmiare denaro pagando in modo preliminare per una o tre anni di macchina virtuale, capacità di calcolo del database SQL, velocità effettiva Azure Cosmos DB o altre risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-106">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="ed910-107">Il pagamento anticipato consente di ottenere uno sconto sulle risorse usate.</span><span class="sxs-lookup"><span data-stu-id="ed910-107">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="ed910-108">Le prenotazioni possono ridurre significativamente i costi di macchina virtuale, calcolo del database SQL, Azure Cosmos DB e altre risorse fino al 72% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="ed910-108">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="ed910-109">Le prenotazioni offrono uno sconto a livello di fatturazione e non hanno alcuna ripercussione sullo stato di runtime delle risorse.</span><span class="sxs-lookup"><span data-stu-id="ed910-109">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="ed910-110">Per altre informazioni, vedere [Che cosa sono le prenotazioni di Azure?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="ed910-110">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="ed910-111">Perché i clienti devono acquistare una prenotazione?</span><span class="sxs-lookup"><span data-stu-id="ed910-111">Why should customers buy a reservation?</span></span>

<span data-ttu-id="ed910-112">Se i clienti hanno macchine virtuali, Azure Cosmos DB o database SQL eseguiti per lunghi periodi di tempo, l'acquisto di una prenotazione offre loro l'opzione più conveniente.</span><span class="sxs-lookup"><span data-stu-id="ed910-112">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="ed910-113">Ad esempio, se un cliente esegue continuamente quattro istanze di un servizio senza una prenotazione, vengono addebitate le tariffe con pagamento in base al carico.</span><span class="sxs-lookup"><span data-stu-id="ed910-113">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="ed910-114">Se acquistano una prenotazione per tali risorse, ottengono immediatamente lo sconto per la prenotazione.</span><span class="sxs-lookup"><span data-stu-id="ed910-114">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="ed910-115">Per le risorse non verranno più addebitate tariffe in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="ed910-115">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="ed910-116">Nuova offerta di Azure interessante in CSP</span><span class="sxs-lookup"><span data-stu-id="ed910-116">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="ed910-117">Grazie all'integrazione delle prenotazioni di Azure e delle sottoscrizioni server nel programma CSP, Microsoft consente ai partner di affrontare la richiesta in rapida crescita dei clienti di soluzioni più conveniente per supportare carichi di lavoro cloud altamente prevedibili e persistenti.</span><span class="sxs-lookup"><span data-stu-id="ed910-117">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="ed910-118">Il programma CSP consente ai partner di acquisire, effettuare il provisioning e gestire le prenotazioni e le sottoscrizioni server di Azure per conto dei clienti commerciali tramite Microsoft Partner Center e portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-118">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="ed910-119">I partner del programma CSP possono anche scegliere come acquistare le prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-119">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="ed910-120">I partner CSP possono acquistare prenotazioni di [Azure](azure-reservations-buying.md) per conto di un cliente oppure possono consentire al cliente di acquistare le proprie prenotazioni da una sottoscrizione di Azure precedente acquistata dal partner. [](give-customers-permission.md)</span><span class="sxs-lookup"><span data-stu-id="ed910-120">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="ed910-121">Le prenotazioni di Azure offrono ai clienti la flessibilità della virtualizzazione per un'ampia gamma di soluzioni di calcolo, tra cui sviluppo e test, esecuzione di applicazioni ed estensione della data center.</span><span class="sxs-lookup"><span data-stu-id="ed910-121">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="ed910-122">Con le istanze di macchine virtuali riservate di [Azure,](https://azure.microsoft.com/pricing/reserved-vm-instances/) ad esempio, i clienti commerciali possono ora risparmiare fino al 72% rispetto ai prezzi delle macchine virtuali di Azure con pagamento in base al consumo semplicemente acquistando o riservando la macchina virtuale per un periodo di 1 o 3 anni.</span><span class="sxs-lookup"><span data-stu-id="ed910-122">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="ed910-123">I clienti di Windows Server Vantaggio Azure Hybrid, inclusi in Software Assurance, potranno risparmiare fino all'80% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="ed910-123">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="ed910-124">Con una combinazione ineguagliata di prezzi interessanti e flessibilità di distribuzione senza pari, i clienti potranno vedere il miglior valore complessivo quando scelgono Prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-124">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="ed910-125">Vedere [Acquistare prenotazioni nel](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-125">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="ed910-126">Vedere il **listino** prezzi commerciale di Azure RI CSP [](https://partner.microsoft.com/dashboard/sell/pricingandoffers) nella categoria Istanze riservate **Microsoft Azure** nella pagina Prezzi e offerte in Partner Center per le sottoscrizioni software e le sottoscrizioni annuali ISV Linux.</span><span class="sxs-lookup"><span data-stu-id="ed910-126">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="ed910-127">**Sottoscrizioni annuali isv Linux**</span><span class="sxs-lookup"><span data-stu-id="ed910-127">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="ed910-128">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="ed910-128">SUSE Linux</span></span>
- <span data-ttu-id="ed910-129">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="ed910-129">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="ed910-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="ed910-130">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="ed910-131">**Sottoscrizioni annuali ISV**</span><span class="sxs-lookup"><span data-stu-id="ed910-131">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="ed910-132">Soluzione Azure VMware di CloudSimple</span><span class="sxs-lookup"><span data-stu-id="ed910-132">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="ed910-133">Per iniziare</span><span class="sxs-lookup"><span data-stu-id="ed910-133">Getting started</span></span>

<span data-ttu-id="ed910-134">Per comprendere come è possibile posizionare le prenotazioni di Azure con i clienti e iniziare a operare il più rapidamente possibile, è consigliabile usare l'approccio seguente per esaminare i materiali di idoneità:</span><span class="sxs-lookup"><span data-stu-id="ed910-134">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="ed910-135">Esaminare e comprendere la nuova [guida Partner Center delle operazioni commerciali.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)</span><span class="sxs-lookup"><span data-stu-id="ed910-135">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="ed910-136">Informazioni su aggiornamenti per prenotazioni di Azure e sottoscrizioni server [nell'API Partner Center (API/SDK).](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="ed910-136">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="ed910-137">Idoneità alle vendite</span><span class="sxs-lookup"><span data-stu-id="ed910-137">Sales readiness</span></span>

- [<span data-ttu-id="ed910-138">Servizi Desktop remoto licenza CAL (Client Access License) (annuncio)</span><span class="sxs-lookup"><span data-stu-id="ed910-138">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="ed910-139">Istanze di macchine virtuali riservate di Azure (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="ed910-139">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="ed910-140">Sottoscrizioni server</span><span class="sxs-lookup"><span data-stu-id="ed910-140">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="ed910-141">Prenotazioni di database SQL (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="ed910-141">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="ed910-142">Azure Cosmos DB (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="ed910-142">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="ed910-143">SQL Istanza gestita (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="ed910-143">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="ed910-144">SUSE e Red Hat Enterprise Linux (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="ed910-144">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="ed910-145">Red Hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-145">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="ed910-146">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-146">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="ed910-147">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-147">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="ed910-148">Panoramica dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-148">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="ed910-149">Calcolatore dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="ed910-149">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="ed910-150">Azure Databricks prenotazioni di unità</span><span class="sxs-lookup"><span data-stu-id="ed910-150">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="ed910-151">Formazione</span><span class="sxs-lookup"><span data-stu-id="ed910-151">Training</span></span>

<span data-ttu-id="ed910-152">Registrarsi per [visualizzare webinar](https://commercial-licensing.eventbuilder.com/FY2019_ALL) commercial licensing readiness ed eventi su richiesta.</span><span class="sxs-lookup"><span data-stu-id="ed910-152">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="ed910-153">Gli eventi on demand registrati in precedenza per l'idoneità alle licenze includono argomenti come:</span><span class="sxs-lookup"><span data-stu-id="ed910-153">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="ed910-154">CSP Online Services, CSP Azure e aggiornamenti delle licenze generali, tra cui Azure (novembre 2018)</span><span class="sxs-lookup"><span data-stu-id="ed910-154">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="ed910-155">Capacità riservata del database SQL & flessibilità delle dimensioni dell'istanza (agosto 2018)</span><span class="sxs-lookup"><span data-stu-id="ed910-155">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="ed910-156">Sottoscrizioni server in CSP (luglio 2018)</span><span class="sxs-lookup"><span data-stu-id="ed910-156">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="ed910-157">Panoramica delle prenotazioni di Azure in CSP (maggio 2018)</span><span class="sxs-lookup"><span data-stu-id="ed910-157">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="ed910-158">Gestione operativa</span><span class="sxs-lookup"><span data-stu-id="ed910-158">Operations</span></span>

<span data-ttu-id="ed910-159">[Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)nuova guida operativa commerciale: guida completa che tratta i criteri chiave e gli aspetti operativi, ad esempio contratti, ordinamento tramite Partner Center, fattura, dettagli del listino prezzi, incentivi, file di riconciliazione, API/SDK, Sandbox e Servizi condivisi per partner di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-159">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="ed910-160">Vantaggio Azure Hybrid</span><span class="sxs-lookup"><span data-stu-id="ed910-160">Azure Hybrid Benefit</span></span>

<span data-ttu-id="ed910-161">Il [Vantaggio Azure Hybrid](https://azure.microsoft.com/pricing/hybrid-benefit) è un vantaggio per i clienti che hanno licenze con Software Assurance, che consente di ottimizzare il valore degli investimenti esistenti in windows Server e/o SQL Server per la migrazione ad Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-161">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="ed910-162">I clienti idonei possono risparmiare fino al 40%\* nelle macchine virtuali di Azure (infrastruttura come servizio o IaaS) e risparmiare fino al 55% su database SQL di Azure (platform as a service o PaaS) e SQL Server in macchine virtuali di Azure (IaaS) con Vantaggio Azure Hybrid, che aumenta fino all'80% se combinato con istanze riservate di Azure.</span><span class="sxs-lookup"><span data-stu-id="ed910-162">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ed910-163">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="ed910-163">Next steps</span></span>

- [<span data-ttu-id="ed910-164">Domande frequenti sul Vantaggio Azure Hybrid</span><span class="sxs-lookup"><span data-stu-id="ed910-164">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="ed910-165">\*I risparmi effettivi possono variare in base all'area, al tipo di istanza o all'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="ed910-165">\*Actual savings may vary based on region, instance type, or usage.</span></span>