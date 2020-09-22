---
title: Prenotazioni di Azure & sottoscrizioni server
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle opportunità del provider di soluzioni cloud per acquisire, effettuare il provisioning e gestire le prenotazioni di Azure e le sottoscrizioni server per i clienti.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000205"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="11db8-103">Acquisire, effettuare il provisioning, & gestire le istanze di VM riservate di Azure e le sottoscrizioni server per i clienti</span><span class="sxs-lookup"><span data-stu-id="11db8-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="11db8-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="11db8-104">Applies to:</span></span>

- <span data-ttu-id="11db8-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="11db8-105">Partner Center</span></span>

<span data-ttu-id="11db8-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="11db8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="11db8-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="11db8-107">Admin agent</span></span>
- <span data-ttu-id="11db8-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="11db8-108">Global admin</span></span>
- <span data-ttu-id="11db8-109">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="11db8-109">Helpdesk agent</span></span>
- <span data-ttu-id="11db8-110">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="11db8-110">Sales agent</span></span>
- <span data-ttu-id="11db8-111">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="11db8-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="11db8-112">Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="11db8-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="11db8-113">I clienti che usano altri tipi di sottoscrizioni, ad esempio con pagamento in base al consumo, singoli contratti Microsoft o sottoscrizioni di Enterprise Agreement, dovranno invece leggere [la documentazione relativa alle prenotazioni di Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="11db8-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="11db8-114">Informazioni sulle prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-114">What are Azure Reservations?</span></span>

<span data-ttu-id="11db8-115">Le prenotazioni di Azure ti aiutano a risparmiare denaro pagando in anticipo per un anno o tre anni di macchine virtuali, capacità di calcolo del database SQL, velocità effettiva Azure Cosmos DB o altre risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="11db8-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="11db8-116">Il pagamento anticipato consente di ottenere uno sconto sulle risorse usate.</span><span class="sxs-lookup"><span data-stu-id="11db8-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="11db8-117">Le prenotazioni possono ridurre significativamente la macchina virtuale, il calcolo del database SQL, Azure Cosmos DB e altri costi delle risorse fino al 72% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="11db8-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="11db8-118">Le prenotazioni offrono uno sconto a livello di fatturazione e non hanno alcuna ripercussione sullo stato di runtime delle risorse.</span><span class="sxs-lookup"><span data-stu-id="11db8-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="11db8-119">Per altre informazioni, vedere [che cosa sono le prenotazioni di Azure?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="11db8-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="11db8-120">Perché i clienti devono acquistare una prenotazione?</span><span class="sxs-lookup"><span data-stu-id="11db8-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="11db8-121">Se i clienti hanno macchine virtuali, Azure Cosmos DB o database SQL in esecuzione per lunghi periodi di tempo, l'acquisto di una prenotazione offre loro l'opzione più conveniente.</span><span class="sxs-lookup"><span data-stu-id="11db8-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="11db8-122">Se, ad esempio, un cliente esegue continuamente quattro istanze di un servizio senza prenotazione, viene addebitata una tariffa con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="11db8-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="11db8-123">Se acquistano una prenotazione per tali risorse, ricevono immediatamente lo sconto relativo alla prenotazione.</span><span class="sxs-lookup"><span data-stu-id="11db8-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="11db8-124">Per le risorse non verranno più addebitate tariffe in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="11db8-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="11db8-125">Nuova offerta di Azure interessante in CSP</span><span class="sxs-lookup"><span data-stu-id="11db8-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="11db8-126">Con le prenotazioni di Azure e le sottoscrizioni server al suo programma CSP, Microsoft è in grado di consentire ai partner di affrontare in modo più rapido la richiesta dei clienti per soluzioni più convenienti per supportare carichi di lavoro cloud persistenti e altamente prevedibili.</span><span class="sxs-lookup"><span data-stu-id="11db8-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="11db8-127">Il programma CSP consente ai partner di acquisire, effettuare il provisioning e gestire le prenotazioni di Azure e le sottoscrizioni server per conto dei clienti commerciali tramite il centro per i partner Microsoft e portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="11db8-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="11db8-128">Microsoft fornisce ai partner le scelte del programma CSP sulle modalità di acquisto delle prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="11db8-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="11db8-129">I partner CSP possono [acquistare prenotazioni di Azure per conto di un cliente](azure-reservations-buying.md) oppure possono [consentire al cliente di acquistare](give-customers-permission.md) le proprie prenotazioni da una sottoscrizione di Azure precedente acquistata dal partner.</span><span class="sxs-lookup"><span data-stu-id="11db8-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="11db8-130">Le prenotazioni di Azure offrono ai clienti la flessibilità della virtualizzazione per un'ampia gamma di soluzioni di calcolo, tra cui sviluppo e test, esecuzione di applicazioni ed estensione del data center.</span><span class="sxs-lookup"><span data-stu-id="11db8-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="11db8-131">Con le [istanze di VM riservate di Azure](https://azure.microsoft.com/pricing/reserved-vm-instances/) , ad esempio, i clienti commerciali possono ora risparmiare fino al 72% rispetto ai prezzi di VM di Azure con pagamento in base al consumo semplicemente acquistando o "riservando" la macchina virtuale per un periodo di 1 o 3 anni.</span><span class="sxs-lookup"><span data-stu-id="11db8-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="11db8-132">I clienti di Windows Server con Vantaggio Azure Hybrid, incluso con Software Assurance, potranno risparmiare fino al 80% rispetto ai prezzi con pagamento in base al consumo.</span><span class="sxs-lookup"><span data-stu-id="11db8-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="11db8-133">Con una combinazione non corrispondente di prezzi interessanti e flessibilità di distribuzione non corrispondente, i clienti visualizzeranno il valore complessivo migliore quando scelgono prenotazioni di Azure:</span><span class="sxs-lookup"><span data-stu-id="11db8-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="11db8-134">Prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-134">Azure reservations</span></span>

- <span data-ttu-id="11db8-135">Istanze di VM riservate di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="11db8-136">Prenotazioni database SQL</span><span class="sxs-lookup"><span data-stu-id="11db8-136">SQL DB Reservations</span></span>
- <span data-ttu-id="11db8-137">Istanza gestita di SQL</span><span class="sxs-lookup"><span data-stu-id="11db8-137">SQL Managed Instance</span></span>
- <span data-ttu-id="11db8-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="11db8-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="11db8-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="11db8-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="11db8-140">Servizi app</span><span class="sxs-lookup"><span data-stu-id="11db8-140">App Services</span></span>
- <span data-ttu-id="11db8-141">Prenotazioni unità Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="11db8-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="11db8-142">Managed Disks</span><span class="sxs-lookup"><span data-stu-id="11db8-142">Managed Disk</span></span>
- <span data-ttu-id="11db8-143">BLOB in blocchi</span><span class="sxs-lookup"><span data-stu-id="11db8-143">Block blob</span></span>
- <span data-ttu-id="11db8-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="11db8-144">MySQL</span></span>
- <span data-ttu-id="11db8-145">Esplora dati di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-145">Azure Data explorer</span></span>
- <span data-ttu-id="11db8-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="11db8-146">MariaDB</span></span>
- <span data-ttu-id="11db8-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="11db8-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="11db8-148">Sottoscrizioni server</span><span class="sxs-lookup"><span data-stu-id="11db8-148">Server subscriptions</span></span>

- <span data-ttu-id="11db8-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="11db8-149">Windows Server</span></span>
- <span data-ttu-id="11db8-150">Licenze CAL Servizi Desktop remoto (RDS)</span><span class="sxs-lookup"><span data-stu-id="11db8-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="11db8-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="11db8-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="11db8-152">Sottoscrizioni annuali per ISV Linux</span><span class="sxs-lookup"><span data-stu-id="11db8-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="11db8-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="11db8-153">SUSE Linux</span></span>
- <span data-ttu-id="11db8-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="11db8-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="11db8-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="11db8-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="11db8-156">Sottoscrizioni annuali ISV</span><span class="sxs-lookup"><span data-stu-id="11db8-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="11db8-157">Soluzione Azure VMware di CloudSimple</span><span class="sxs-lookup"><span data-stu-id="11db8-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="11db8-158">Guida introduttiva</span><span class="sxs-lookup"><span data-stu-id="11db8-158">Getting started</span></span>

<span data-ttu-id="11db8-159">Per comprendere come è possibile posizionare le prenotazioni di Azure con i clienti e iniziare a usare il più rapidamente possibile, è consigliabile adottare l'approccio seguente per esaminare i materiali di conformità:</span><span class="sxs-lookup"><span data-stu-id="11db8-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="11db8-160">Esaminare le presentazioni di panoramica e i webinar associati per la proposta e il posizionamento dei valori del cliente</span><span class="sxs-lookup"><span data-stu-id="11db8-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="11db8-161">Esaminare e comprendere la moderna guida operativa di Commerce</span><span class="sxs-lookup"><span data-stu-id="11db8-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="11db8-162">Consultare le domande frequenti sulle sottoscrizioni di Azure RI e server</span><span class="sxs-lookup"><span data-stu-id="11db8-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="11db8-163">Informazioni sugli aggiornamenti per le prenotazioni di Azure e le sottoscrizioni server nell'API del centro per i [partner (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="11db8-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="11db8-164">Risorse</span><span class="sxs-lookup"><span data-stu-id="11db8-164">Resources</span></span>

<span data-ttu-id="11db8-165">Di seguito è riportato un elenco completo delle risorse che consentono di eseguire rapidamente le operazioni di onboarding delle prenotazioni di Azure tramite il centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="11db8-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="11db8-166">Conformità vendite</span><span class="sxs-lookup"><span data-stu-id="11db8-166">Sales readiness</span></span>

- [<span data-ttu-id="11db8-167">Prenotazioni di Azure e sottoscrizioni server con Vantaggio Azure Hybrid Panoramica</span><span class="sxs-lookup"><span data-stu-id="11db8-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="11db8-168">Foglio vendite</span><span class="sxs-lookup"><span data-stu-id="11db8-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="11db8-169">Domande frequenti sui partner per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="11db8-170">Domande frequenti sui partner per le prenotazioni di Azure e il database SQL</span><span class="sxs-lookup"><span data-stu-id="11db8-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="11db8-171">CAL (Client Access License) Servizi Desktop remoto (RDS) (annuncio)</span><span class="sxs-lookup"><span data-stu-id="11db8-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="11db8-172">Istanze di VM riservate di Azure (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="11db8-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="11db8-173">Sottoscrizioni server</span><span class="sxs-lookup"><span data-stu-id="11db8-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="11db8-174">Panoramica di database SQL in Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="11db8-175">Prenotazioni database SQL (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="11db8-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="11db8-176">Azure Cosmos DB (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="11db8-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="11db8-177">Istanza gestita SQL (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="11db8-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="11db8-178">SUSE e Red Hat Enterprise Linux (portale di Azure)</span><span class="sxs-lookup"><span data-stu-id="11db8-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="11db8-179">Red Hat Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="11db8-180">SUSE Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="11db8-181">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="11db8-182">Panoramica dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="11db8-183">Calcolatore dei prezzi di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="11db8-184">Prenotazioni unità Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="11db8-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="11db8-185">Elenchi prezzi CSP: le **istanze riservate Microsoft Azure** e gli elenchi prezzi delle **sottoscrizioni software** si trovano entrambi nella pagina dei prezzi del centro per i partner [&](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="11db8-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="11db8-186">Formazione</span><span class="sxs-lookup"><span data-stu-id="11db8-186">Training</span></span>

<span data-ttu-id="11db8-187">Iscriviti per visualizzare i webinar di conformità per le [licenze commerciali](https://commercial-licensing.eventbuilder.com/FY2019_ALL) e gli eventi su richiesta.</span><span class="sxs-lookup"><span data-stu-id="11db8-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="11db8-188">Gli eventi di conformità su richiesta delle licenze includono argomenti come:</span><span class="sxs-lookup"><span data-stu-id="11db8-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="11db8-189">CSP Online Services, CSP Azure e General Licensing Updates, incluso Azure (novembre 2018)</span><span class="sxs-lookup"><span data-stu-id="11db8-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="11db8-190">Capacità riservata del database SQL & flessibilità delle dimensioni delle istanze (agosto 2018)</span><span class="sxs-lookup"><span data-stu-id="11db8-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="11db8-191">Sottoscrizioni server in CSP (2018 luglio)</span><span class="sxs-lookup"><span data-stu-id="11db8-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="11db8-192">Panoramica delle prenotazioni di Azure in CSP (2018 maggio)</span><span class="sxs-lookup"><span data-stu-id="11db8-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="11db8-193">Altri corsi di formazione utili includono il [modulo di licenze di Azure nell'Università partner](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="11db8-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="11db8-194">Gestione operativa</span><span class="sxs-lookup"><span data-stu-id="11db8-194">Operations</span></span>

- <span data-ttu-id="11db8-195">[Guida operativa moderna di Commerce](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aggiornata): una guida completa che copre i criteri chiave e gli aspetti operativi, ad esempio i contratti, l'ordinamento tramite il centro per i partner, la fattura, i dettagli dell'elenco prezzi, gli incentivi, il file di riconciliazione, l'API/SDK, sandbox e i servizi condivisi del partner</span><span class="sxs-lookup"><span data-stu-id="11db8-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="11db8-196">Offerta moderna di disponibilità dei paesi e matrice di valuta dei clienti</span><span class="sxs-lookup"><span data-stu-id="11db8-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="11db8-197">Vendere Microsoft Azure istanze riservate</span><span class="sxs-lookup"><span data-stu-id="11db8-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="11db8-198">Acquistare prenotazioni di Microsoft Azure per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="11db8-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="11db8-199">Gestisci prenotazioni di Azure per conto dei tuoi clienti</span><span class="sxs-lookup"><span data-stu-id="11db8-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="11db8-200">Fatturazione per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="11db8-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="11db8-201">Ridimensionamento della macchina virtuale per l'utilizzo massimo delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="11db8-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="11db8-202">API del centro per i partner (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="11db8-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="11db8-203">Servizi Desktop remoto</span><span class="sxs-lookup"><span data-stu-id="11db8-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="11db8-204">Vantaggio Azure Hybrid</span><span class="sxs-lookup"><span data-stu-id="11db8-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="11db8-205">Il [vantaggio Azure Hybrid](https://azure.microsoft.com/pricing/hybrid-benefit) consente di ottenere più valore dalle licenze di Windows Server e di risparmiare fino al 47% sulle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="11db8-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="11db8-206">Puoi usare il vantaggio con le licenze per le edizioni Windows Server Datacenter e Standard con copertura Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="11db8-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="11db8-207">A seconda dell'edizione, è possibile convertire o riutilizzare le licenze per eseguire macchine virtuali Windows Server in Azure e pagare una tariffa di calcolo di base inferiore (tariffe delle macchine virtuali Linux).</span><span class="sxs-lookup"><span data-stu-id="11db8-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="11db8-208">Vedere anche [vantaggio Azure Hybrid domande frequenti](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="11db8-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="11db8-209">\* I risparmi effettivi possono variare in base all'area, al tipo di istanza o all'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="11db8-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
