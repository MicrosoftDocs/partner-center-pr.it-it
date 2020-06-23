---
title: Prenotazioni di Azure & sottoscrizioni server
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle opportunità del provider di soluzioni cloud per acquisire, effettuare il provisioning e gestire le prenotazioni di Azure e le sottoscrizioni server per i clienti.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, sottoscrizioni, VM, prenotazione, istanza riservata
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4e5e5d88b1f629b07932d37dedb70d0309a26dce
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198629"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="0a6aa-104">Acquisire, effettuare il provisioning, & gestire le istanze di VM riservate di Azure e le sottoscrizioni server per i clienti</span><span class="sxs-lookup"><span data-stu-id="0a6aa-104">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="0a6aa-105">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="0a6aa-105">Applies to:</span></span>

- <span data-ttu-id="0a6aa-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0a6aa-106">Partner Center</span></span>

<span data-ttu-id="0a6aa-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="0a6aa-107">**Appropriate roles**</span></span>

- <span data-ttu-id="0a6aa-108">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="0a6aa-108">Admin agent</span></span>
- <span data-ttu-id="0a6aa-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="0a6aa-109">Global admin</span></span>
- <span data-ttu-id="0a6aa-110">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="0a6aa-110">Helpdesk agent</span></span>
- <span data-ttu-id="0a6aa-111">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="0a6aa-111">Sales agent</span></span>
- <span data-ttu-id="0a6aa-112">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="0a6aa-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="0a6aa-113">Informazioni sulle prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-113">What are Azure Reservations?</span></span>

<span data-ttu-id="0a6aa-114">Le prenotazioni di Azure ti aiutano a risparmiare denaro pagando in anticipo per un anno o tre anni di macchine virtuali, capacità di calcolo del database SQL, velocità effettiva Azure Cosmos DB o altre risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="0a6aa-115">Il pagamento anticipato consente di ottenere uno sconto sulle risorse usate.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="0a6aa-116">Le prenotazioni possono ridurre significativamente la macchina virtuale, il calcolo del database SQL, Azure Cosmos DB e altri costi delle risorse fino al 72% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="0a6aa-117">Le prenotazioni offrono uno sconto a livello di fatturazione e non hanno alcuna ripercussione sullo stato di runtime delle risorse.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="0a6aa-118">Per altre informazioni, vedere [che cosa sono le prenotazioni di Azure?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-118">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="0a6aa-119">Perché i clienti devono acquistare una prenotazione?</span><span class="sxs-lookup"><span data-stu-id="0a6aa-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="0a6aa-120">Se i clienti hanno macchine virtuali, Azure Cosmos DB o database SQL in esecuzione per lunghi periodi di tempo, l'acquisto di una prenotazione offre loro l'opzione più conveniente.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="0a6aa-121">Se, ad esempio, un cliente esegue continuamente quattro istanze di un servizio senza prenotazione, viene addebitata una tariffa con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="0a6aa-122">Se acquistano una prenotazione per tali risorse, ricevono immediatamente lo sconto relativo alla prenotazione.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="0a6aa-123">Per le risorse non verranno più addebitate tariffe in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="0a6aa-124">Nuova offerta di Azure interessante in CSP</span><span class="sxs-lookup"><span data-stu-id="0a6aa-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="0a6aa-125">Con le prenotazioni di Azure e le sottoscrizioni server al suo programma CSP, Microsoft è in grado di consentire ai partner di affrontare in modo più rapido la richiesta dei clienti per soluzioni più convenienti per supportare carichi di lavoro cloud persistenti e altamente prevedibili.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="0a6aa-126">Il programma CSP consente ai partner di acquisire, effettuare il provisioning e gestire le prenotazioni di Azure e le sottoscrizioni server per conto dei clienti commerciali tramite il centro per i partner Microsoft e portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-126">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="0a6aa-127">Microsoft fornisce ai partner le scelte del programma CSP sulle modalità di acquisto delle prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-127">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="0a6aa-128">I partner CSP possono [acquistare prenotazioni di Azure per conto di un cliente](azure-reservations-buying.md) oppure possono [consentire al cliente di acquistare](give-customers-permission.md) le proprie prenotazioni da una sottoscrizione di Azure precedente acquistata dal partner.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-128">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="0a6aa-129">Le prenotazioni di Azure offrono ai clienti la flessibilità della virtualizzazione per un'ampia gamma di soluzioni di calcolo, tra cui sviluppo e test, esecuzione di applicazioni ed estensione del data center.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="0a6aa-130">Con le [istanze di VM riservate di Azure](https://azure.microsoft.com/pricing/reserved-vm-instances/) , ad esempio, i clienti commerciali possono ora risparmiare fino al 72% rispetto ai prezzi di VM di Azure con pagamento in base al consumo semplicemente acquistando o "riservando" la macchina virtuale per un periodo di 1 o 3 anni.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-130">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="0a6aa-131">I clienti di Windows Server con Vantaggio Azure Hybrid, incluso con Software Assurance, potranno risparmiare fino al 80% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-131">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="0a6aa-132">Con una combinazione non corrispondente di prezzi interessanti e flessibilità di distribuzione non corrispondente, i clienti visualizzeranno il valore complessivo migliore quando scelgono prenotazioni di Azure:</span><span class="sxs-lookup"><span data-stu-id="0a6aa-132">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="0a6aa-133">Prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-133">Azure reservations</span></span>

- <span data-ttu-id="0a6aa-134">Istanze di VM riservate di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-134">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="0a6aa-135">Prenotazioni database SQL</span><span class="sxs-lookup"><span data-stu-id="0a6aa-135">SQL DB Reservations</span></span>
- <span data-ttu-id="0a6aa-136">Istanza gestita di SQL</span><span class="sxs-lookup"><span data-stu-id="0a6aa-136">SQL Managed Instance</span></span>
- <span data-ttu-id="0a6aa-137">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="0a6aa-137">Azure Cosmos DB</span></span>
- <span data-ttu-id="0a6aa-138">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="0a6aa-138">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="0a6aa-139">Servizi app</span><span class="sxs-lookup"><span data-stu-id="0a6aa-139">App Services</span></span>
- <span data-ttu-id="0a6aa-140">Prenotazioni unità Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="0a6aa-140">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="0a6aa-141">Managed Disks</span><span class="sxs-lookup"><span data-stu-id="0a6aa-141">Managed Disk</span></span>
- <span data-ttu-id="0a6aa-142">BLOB in blocchi</span><span class="sxs-lookup"><span data-stu-id="0a6aa-142">Block blob</span></span>
- <span data-ttu-id="0a6aa-143">MySQL</span><span class="sxs-lookup"><span data-stu-id="0a6aa-143">MySQL</span></span>
- <span data-ttu-id="0a6aa-144">Esplora dati di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-144">Azure Data explorer</span></span>
- <span data-ttu-id="0a6aa-145">MariaDB</span><span class="sxs-lookup"><span data-stu-id="0a6aa-145">MariaDB</span></span>
- <span data-ttu-id="0a6aa-146">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="0a6aa-146">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="0a6aa-147">Sottoscrizioni server</span><span class="sxs-lookup"><span data-stu-id="0a6aa-147">Server subscriptions</span></span>

- <span data-ttu-id="0a6aa-148">Windows Server</span><span class="sxs-lookup"><span data-stu-id="0a6aa-148">Windows Server</span></span>
- <span data-ttu-id="0a6aa-149">Licenze CAL Servizi Desktop remoto (RDS)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-149">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="0a6aa-150">SQL Server</span><span class="sxs-lookup"><span data-stu-id="0a6aa-150">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="0a6aa-151">Sottoscrizioni annuali per ISV Linux</span><span class="sxs-lookup"><span data-stu-id="0a6aa-151">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="0a6aa-152">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="0a6aa-152">SUSE Linux</span></span>
- <span data-ttu-id="0a6aa-153">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="0a6aa-153">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="0a6aa-154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="0a6aa-154">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="0a6aa-155">Sottoscrizioni annuali ISV</span><span class="sxs-lookup"><span data-stu-id="0a6aa-155">ISV annual subscriptions</span></span>

- <span data-ttu-id="0a6aa-156">Soluzione Azure VMware di CloudSimple</span><span class="sxs-lookup"><span data-stu-id="0a6aa-156">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="0a6aa-157">Guida introduttiva</span><span class="sxs-lookup"><span data-stu-id="0a6aa-157">Getting started</span></span>

<span data-ttu-id="0a6aa-158">Per comprendere come è possibile posizionare le prenotazioni di Azure con i clienti e iniziare a usare il più rapidamente possibile, è consigliabile adottare l'approccio seguente per esaminare i materiali di conformità:</span><span class="sxs-lookup"><span data-stu-id="0a6aa-158">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="0a6aa-159">Esaminare le presentazioni di panoramica e i webinar associati per la proposta e il posizionamento dei valori del cliente</span><span class="sxs-lookup"><span data-stu-id="0a6aa-159">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="0a6aa-160">Esaminare e comprendere la moderna guida operativa di Commerce</span><span class="sxs-lookup"><span data-stu-id="0a6aa-160">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="0a6aa-161">Consultare le domande frequenti sulle sottoscrizioni di Azure RI e server</span><span class="sxs-lookup"><span data-stu-id="0a6aa-161">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="0a6aa-162">Informazioni sugli aggiornamenti per le prenotazioni di Azure e le sottoscrizioni server nell'API del centro per i [partner (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-162">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="0a6aa-163">Risorse</span><span class="sxs-lookup"><span data-stu-id="0a6aa-163">Resources</span></span>

<span data-ttu-id="0a6aa-164">Di seguito è riportato un elenco completo delle risorse che consentono di eseguire rapidamente le operazioni di onboarding delle prenotazioni di Azure tramite il centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="0a6aa-164">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="0a6aa-165">Conformità vendite</span><span class="sxs-lookup"><span data-stu-id="0a6aa-165">Sales readiness</span></span>

- [<span data-ttu-id="0a6aa-166">Prenotazioni di Azure e sottoscrizioni server con Vantaggio Azure Hybrid Panoramica</span><span class="sxs-lookup"><span data-stu-id="0a6aa-166">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="0a6aa-167">Foglio vendite</span><span class="sxs-lookup"><span data-stu-id="0a6aa-167">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="0a6aa-168">Domande frequenti sui partner per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-168">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="0a6aa-169">Domande frequenti sui partner per le prenotazioni di Azure e il database SQL</span><span class="sxs-lookup"><span data-stu-id="0a6aa-169">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="0a6aa-170">CAL (Client Access License) Servizi Desktop remoto (RDS) (annuncio)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-170">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="0a6aa-171">Istanze di VM riservate di Azure (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-171">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="0a6aa-172">Sottoscrizioni server</span><span class="sxs-lookup"><span data-stu-id="0a6aa-172">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="0a6aa-173">Panoramica di database SQL in Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-173">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="0a6aa-174">Prenotazioni database SQL (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-174">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="0a6aa-175">Azure Cosmos DB (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-175">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="0a6aa-176">Istanza gestita SQL (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-176">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="0a6aa-177">SUSE e Red Hat Enterprise Linux (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-177">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="0a6aa-178">Red Hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-178">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="0a6aa-179">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-179">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="0a6aa-180">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-180">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="0a6aa-181">Panoramica dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-181">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="0a6aa-182">Calcolatore dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-182">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="0a6aa-183">Prenotazioni unità Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="0a6aa-183">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="0a6aa-184">Elenchi prezzi CSP: le **istanze riservate Microsoft Azure** e gli elenchi prezzi delle **sottoscrizioni software** si trovano entrambi nella pagina dei prezzi del centro per i partner [&](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="0a6aa-184">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="0a6aa-185">Formazione</span><span class="sxs-lookup"><span data-stu-id="0a6aa-185">Training</span></span>

<span data-ttu-id="0a6aa-186">Iscriviti per visualizzare i webinar di conformità per le [licenze commerciali](https://commercial-licensing.eventbuilder.com/FY2019_ALL) e gli eventi su richiesta.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-186">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="0a6aa-187">Gli eventi di conformità su richiesta delle licenze includono argomenti come:</span><span class="sxs-lookup"><span data-stu-id="0a6aa-187">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="0a6aa-188">CSP Online Services, CSP Azure e General Licensing Updates, incluso Azure (novembre 2018)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-188">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="0a6aa-189">Capacità riservata del database SQL & flessibilità delle dimensioni delle istanze (agosto 2018)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-189">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="0a6aa-190">Sottoscrizioni server in CSP (2018 luglio)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-190">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="0a6aa-191">Panoramica delle prenotazioni di Azure in CSP (2018 maggio)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-191">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="0a6aa-192">Altri corsi di formazione utili includono il [modulo di licenze di Azure nell'Università partner](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="0a6aa-192">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="0a6aa-193">Operazioni</span><span class="sxs-lookup"><span data-stu-id="0a6aa-193">Operations</span></span>

- <span data-ttu-id="0a6aa-194">[Guida operativa moderna di Commerce](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aggiornata): una guida completa che copre i criteri chiave e gli aspetti operativi, ad esempio i contratti, l'ordinamento tramite il centro per i partner, la fattura, i dettagli dell'elenco prezzi, gli incentivi, il file di riconciliazione, l'API/SDK, sandbox e i servizi condivisi del partner</span><span class="sxs-lookup"><span data-stu-id="0a6aa-194">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="0a6aa-195">Offerta moderna di disponibilità dei paesi e matrice di valuta dei clienti</span><span class="sxs-lookup"><span data-stu-id="0a6aa-195">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="0a6aa-196">Vendere Microsoft Azure istanze riservate</span><span class="sxs-lookup"><span data-stu-id="0a6aa-196">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="0a6aa-197">Acquistare prenotazioni di Microsoft Azure per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="0a6aa-197">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="0a6aa-198">Gestisci prenotazioni di Azure per conto dei tuoi clienti</span><span class="sxs-lookup"><span data-stu-id="0a6aa-198">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="0a6aa-199">Fatturazione per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0a6aa-199">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="0a6aa-200">Ridimensionamento della macchina virtuale per l'utilizzo massimo delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="0a6aa-200">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="0a6aa-201">API del centro per i partner (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-201">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="0a6aa-202">Servizi Desktop remoto</span><span class="sxs-lookup"><span data-stu-id="0a6aa-202">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="0a6aa-203">Vantaggio Azure Hybrid</span><span class="sxs-lookup"><span data-stu-id="0a6aa-203">Azure Hybrid Benefit</span></span>

<span data-ttu-id="0a6aa-204">Il [vantaggio Azure Hybrid](https://azure.microsoft.com/pricing/hybrid-benefit) consente di ottenere più valore dalle licenze di Windows Server e di risparmiare fino al 47% sulle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-204">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="0a6aa-205">Puoi usare il vantaggio con le licenze per le edizioni Windows Server Datacenter e Standard con copertura Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-205">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="0a6aa-206">A seconda dell'edizione, è possibile convertire o riutilizzare le licenze per eseguire macchine virtuali Windows Server in Azure e pagare una tariffa di calcolo di base inferiore (tariffe delle macchine virtuali Linux).</span><span class="sxs-lookup"><span data-stu-id="0a6aa-206">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="0a6aa-207">Vedere anche [vantaggio Azure Hybrid domande frequenti](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="0a6aa-207">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="0a6aa-208">\* I risparmi effettivi possono variare in base all'area, al tipo di istanza o all'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="0a6aa-208">\*Actual savings may vary based on region, instance type, or usage.</span></span>
