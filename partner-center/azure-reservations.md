---
title: Vendere i clienti Microsoft Azure prenotazioni
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Come provider di soluzioni cloud, è possibile acquistare, vendere o gestire prenotazioni di Azure per i clienti. Usare il centro per i partner, il portale di Azure o l'API del centro per i partner.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3efe8ae6a955dee5cfe01d0571cd107f8ee50f5c
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900086"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="cc287-104">Vendere Microsoft Azure prenotazioni ai clienti tramite il centro per i partner, l'portale di Azure o le API</span><span class="sxs-lookup"><span data-stu-id="cc287-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="cc287-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="cc287-105">**Applies to**</span></span>

- <span data-ttu-id="cc287-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-106">Partner Center</span></span>
- <span data-ttu-id="cc287-107">Portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="cc287-108">Partner aderenti al programma CSP</span><span class="sxs-lookup"><span data-stu-id="cc287-108">Partners in the CSP program</span></span>

<span data-ttu-id="cc287-109">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="cc287-109">**Appropriate roles**</span></span>

- <span data-ttu-id="cc287-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="cc287-110">Admin agent</span></span>
- <span data-ttu-id="cc287-111">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="cc287-111">Global admin</span></span>
- <span data-ttu-id="cc287-112">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="cc287-112">Helpdesk agent</span></span>
- <span data-ttu-id="cc287-113">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="cc287-113">Sales agent</span></span>
- <span data-ttu-id="cc287-114">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="cc287-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="cc287-115">Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="cc287-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="cc287-116">I clienti che usano altri tipi di sottoscrizioni, ad esempio con pagamento in base al consumo, singoli contratti Microsoft o sottoscrizioni di Enterprise Agreement, dovranno invece leggere [la documentazione relativa alle prenotazioni di Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="cc287-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="cc287-117">I partner del programma CSP possono offrire ai clienti Microsoft Azure prenotazioni.</span><span class="sxs-lookup"><span data-stu-id="cc287-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="cc287-118">I clienti possono ottenere risparmi significativi quando si riservano in anticipo.</span><span class="sxs-lookup"><span data-stu-id="cc287-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="cc287-119">Le prenotazioni di Azure offrono ai clienti semplicità e flessibilità nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="cc287-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="cc287-120">Condizioni di prenotazione per uno o tre anni</span><span class="sxs-lookup"><span data-stu-id="cc287-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="cc287-121">Facile da iniziare; installazione completata in pochi secondi</span><span class="sxs-lookup"><span data-stu-id="cc287-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="cc287-122">Annulla o scambia le istanze riservate in qualsiasi momento per il rimborso modificato</span><span class="sxs-lookup"><span data-stu-id="cc287-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="cc287-123">Gestire l'utilizzo delle istanze riservate a livello di reparto aziendale o individuale</span><span class="sxs-lookup"><span data-stu-id="cc287-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="cc287-124">Le prenotazioni di Azure possono ricorrere ai clienti nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="cc287-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="cc287-125">Le prenotazioni possono offrire risparmi significativi rispetto ai prezzi con pagamento in base al consumo (PAYG)</span><span class="sxs-lookup"><span data-stu-id="cc287-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="cc287-126">Budget e previsioni migliori con il pagamento anticipato per i termini di un anno o di tre anni</span><span class="sxs-lookup"><span data-stu-id="cc287-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="cc287-127">Capacità di calcolo con priorità nell'area di Azure più vicina ai loro uffici</span><span class="sxs-lookup"><span data-stu-id="cc287-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="cc287-128">Le prenotazioni di Azure forniscono la base per le soluzioni di infrastruttura end-to-end in combinazione con software come Microsoft Windows Server e il database SQL di Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="cc287-129">È possibile acquistare, vendere e gestire prenotazioni di Azure sia nel centro per i partner che nel portale di Azure e usando l'API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="cc287-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="cc287-130">È anche possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione di Azure acquistata per loro.</span><span class="sxs-lookup"><span data-stu-id="cc287-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="cc287-131">Per informazioni, seguire i collegamenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="cc287-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="cc287-132">Risorse per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-132">Azure reservations resources</span></span>

|<span data-ttu-id="cc287-133">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="cc287-133">**For information about**</span></span>   |<span data-ttu-id="cc287-134">**Leggi**</span><span class="sxs-lookup"><span data-stu-id="cc287-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="cc287-135">Documentazione per le prenotazioni di Azure per i clienti</span><span class="sxs-lookup"><span data-stu-id="cc287-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="cc287-136">Che cosa sono le prenotazioni di Azure?</span><span class="sxs-lookup"><span data-stu-id="cc287-136">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="cc287-137">Acquisto di prenotazioni di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="cc287-138">Acquista prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="cc287-139">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="cc287-140">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="cc287-141">Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente</span><span class="sxs-lookup"><span data-stu-id="cc287-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="cc287-142">Dimensionamento delle VM per l'utilizzo massimo della prenotazione di Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="cc287-143">Acquisto di prenotazioni di Azure tramite l'API del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="cc287-144">[Acquistare istanze di VM riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="cc287-144">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="cc287-145">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure dalla sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="cc287-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="cc287-146">Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="cc287-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
