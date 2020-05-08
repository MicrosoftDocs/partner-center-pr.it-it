---
title: Vendere i clienti Microsoft Azure prenotazioni
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Come provider di soluzioni cloud, è possibile acquistare, vendere o gestire prenotazioni di Azure per i clienti. Usare il centro per i partner, il portale di Azure o l'API del centro per i partner.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, prenotazioni, gestione, fatturazione, acquisto, Azure RI, istanze riservate di Azure
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19c156f0b47ccb39bc678cdd2ae9cce9db5c5ebd
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908294"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="2e4e3-105">Vendere Microsoft Azure prenotazioni ai clienti tramite il centro per i partner, l'portale di Azure o le API</span><span class="sxs-lookup"><span data-stu-id="2e4e3-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<!--Maggie, 12/7/18 - Added "Partner Center" to metadata title and H1 title as per Catherine Watson in bug #19868631-->

<span data-ttu-id="2e4e3-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="2e4e3-106">**Applies to**</span></span>

- <span data-ttu-id="2e4e3-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-107">Partner Center</span></span>
- <span data-ttu-id="2e4e3-108">Portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="2e4e3-109">Partner in CSP</span><span class="sxs-lookup"><span data-stu-id="2e4e3-109">Partners in CSP</span></span>

<span data-ttu-id="2e4e3-110">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="2e4e3-110">**Appropriate roles**</span></span>

- <span data-ttu-id="2e4e3-111">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="2e4e3-111">Admin agent</span></span>
- <span data-ttu-id="2e4e3-112">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="2e4e3-112">Global admin</span></span>
- <span data-ttu-id="2e4e3-113">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="2e4e3-113">Helpdesk agent</span></span>
- <span data-ttu-id="2e4e3-114">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="2e4e3-114">Sales agent</span></span>
- <span data-ttu-id="2e4e3-115">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="2e4e3-115">User management admin</span></span>

<span data-ttu-id="2e4e3-116">I partner del programma Cloud Solution Provider (CSP) possono offrire ai clienti Microsoft Azure prenotazioni.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="2e4e3-117">I clienti possono ottenere risparmi significativi quando si riservano in anticipo.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="2e4e3-118">Le prenotazioni di Azure offrono ai clienti semplicità e flessibilità nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2e4e3-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="2e4e3-119">Condizioni di prenotazione per uno o tre anni</span><span class="sxs-lookup"><span data-stu-id="2e4e3-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="2e4e3-120">Facile da iniziare; installazione completata in pochi secondi</span><span class="sxs-lookup"><span data-stu-id="2e4e3-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="2e4e3-121">Annulla o scambia le istanze riservate in qualsiasi momento per il rimborso modificato</span><span class="sxs-lookup"><span data-stu-id="2e4e3-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="2e4e3-122">Gestire l'utilizzo delle istanze riservate a livello di reparto aziendale o individuale</span><span class="sxs-lookup"><span data-stu-id="2e4e3-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="2e4e3-123">Le prenotazioni di Azure possono ricorrere ai clienti nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2e4e3-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="2e4e3-124">Le prenotazioni possono offrire risparmi significativi rispetto ai prezzi con pagamento in base al consumo (PAYG)</span><span class="sxs-lookup"><span data-stu-id="2e4e3-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="2e4e3-125">Budget e previsioni migliori con il pagamento anticipato per i termini di un anno o di tre anni</span><span class="sxs-lookup"><span data-stu-id="2e4e3-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="2e4e3-126">Capacità di calcolo con priorità nell'area di Azure più vicina ai loro uffici</span><span class="sxs-lookup"><span data-stu-id="2e4e3-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="2e4e3-127">Le prenotazioni di Azure forniscono la base per le soluzioni di infrastruttura end-to-end in combinazione con software come Microsoft Windows Server e il database SQL di Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="2e4e3-128">È possibile acquistare, vendere e gestire prenotazioni di Azure sia nel centro per i partner che nel portale di Azure e usando l'API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="2e4e3-129">È anche possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione di Azure acquistata per loro.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="2e4e3-130">Per informazioni, seguire i collegamenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="2e4e3-131">Risorse per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-131">Azure reservations resources</span></span>

|<span data-ttu-id="2e4e3-132">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="2e4e3-132">**For information about**</span></span>   |<span data-ttu-id="2e4e3-133">**Leggi**</span><span class="sxs-lookup"><span data-stu-id="2e4e3-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="2e4e3-134">Documentazione per le prenotazioni di Azure per i clienti</span><span class="sxs-lookup"><span data-stu-id="2e4e3-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="2e4e3-135">Cosa sono le prenotazioni di Azure?</span><span class="sxs-lookup"><span data-stu-id="2e4e3-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="2e4e3-136">Acquisto di prenotazioni di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="2e4e3-137">Acquista prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="2e4e3-138">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="2e4e3-139">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2e4e3-140">Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente</span><span class="sxs-lookup"><span data-stu-id="2e4e3-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="2e4e3-141">Dimensionamento delle VM per l'utilizzo massimo della prenotazione di Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="2e4e3-142">Acquisto di prenotazioni di Azure tramite l'API del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2e4e3-143">[Acquistare istanze di VM riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2e4e3-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="2e4e3-144">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure dalla sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="2e4e3-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="2e4e3-145">Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="2e4e3-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
