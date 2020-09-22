---
title: Vendere i clienti Microsoft Azure prenotazioni
description: Come provider di soluzioni cloud, è possibile acquistare, vendere o gestire prenotazioni di Azure per i clienti. Usare il centro per i partner, il portale di Azure o l'API del centro per i partner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000235"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="0ebe1-104">Vendere Microsoft Azure prenotazioni ai clienti tramite il centro per i partner, l'portale di Azure o le API</span><span class="sxs-lookup"><span data-stu-id="0ebe1-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="0ebe1-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="0ebe1-105">**Applies to**</span></span>

- <span data-ttu-id="0ebe1-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-106">Partner Center</span></span>
- <span data-ttu-id="0ebe1-107">Portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="0ebe1-108">Partner aderenti al programma CSP</span><span class="sxs-lookup"><span data-stu-id="0ebe1-108">Partners in the CSP program</span></span>

<span data-ttu-id="0ebe1-109">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="0ebe1-109">**Appropriate roles**</span></span>

- <span data-ttu-id="0ebe1-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="0ebe1-110">Admin agent</span></span>
- <span data-ttu-id="0ebe1-111">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="0ebe1-111">Global admin</span></span>
- <span data-ttu-id="0ebe1-112">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="0ebe1-112">Helpdesk agent</span></span>
- <span data-ttu-id="0ebe1-113">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="0ebe1-113">Sales agent</span></span>
- <span data-ttu-id="0ebe1-114">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="0ebe1-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="0ebe1-115">Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="0ebe1-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="0ebe1-116">I clienti che usano altri tipi di sottoscrizioni, ad esempio con pagamento in base al consumo, singoli contratti Microsoft o sottoscrizioni di Enterprise Agreement, dovranno invece leggere [la documentazione relativa alle prenotazioni di Azure](/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="0ebe1-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="0ebe1-117">I partner del programma CSP possono offrire ai clienti Microsoft Azure prenotazioni.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="0ebe1-118">I clienti possono ottenere risparmi significativi quando si riservano in anticipo.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="0ebe1-119">Le prenotazioni di Azure offrono ai clienti semplicità e flessibilità nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="0ebe1-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="0ebe1-120">Condizioni di prenotazione per uno o tre anni</span><span class="sxs-lookup"><span data-stu-id="0ebe1-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="0ebe1-121">Facile da iniziare; installazione completata in pochi secondi</span><span class="sxs-lookup"><span data-stu-id="0ebe1-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="0ebe1-122">Annulla o scambia le istanze riservate in qualsiasi momento per il rimborso modificato</span><span class="sxs-lookup"><span data-stu-id="0ebe1-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="0ebe1-123">Gestire l'utilizzo delle istanze riservate a livello di reparto aziendale o individuale</span><span class="sxs-lookup"><span data-stu-id="0ebe1-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="0ebe1-124">Le prenotazioni di Azure possono ricorrere ai clienti nei modi seguenti:</span><span class="sxs-lookup"><span data-stu-id="0ebe1-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="0ebe1-125">Le prenotazioni possono offrire risparmi significativi rispetto ai prezzi con pagamento in base al consumo (PAYG)</span><span class="sxs-lookup"><span data-stu-id="0ebe1-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="0ebe1-126">Budget e previsioni migliori con il pagamento anticipato per i termini di un anno o di tre anni</span><span class="sxs-lookup"><span data-stu-id="0ebe1-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="0ebe1-127">Capacità di calcolo con priorità nell'area di Azure più vicina ai loro uffici</span><span class="sxs-lookup"><span data-stu-id="0ebe1-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="0ebe1-128">Le prenotazioni di Azure forniscono la base per le soluzioni di infrastruttura end-to-end in combinazione con software come Microsoft Windows Server e il database SQL di Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="0ebe1-129">È possibile acquistare, vendere e gestire prenotazioni di Azure sia nel centro per i partner che nel portale di Azure e usando l'API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="0ebe1-130">È anche possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione di Azure acquistata per loro.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="0ebe1-131">Per informazioni, seguire i collegamenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="0ebe1-132">Risorse per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-132">Azure reservations resources</span></span>

|<span data-ttu-id="0ebe1-133">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="0ebe1-133">**For information about**</span></span>   |<span data-ttu-id="0ebe1-134">**Leggi**</span><span class="sxs-lookup"><span data-stu-id="0ebe1-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="0ebe1-135">Documentazione per le prenotazioni di Azure per i clienti</span><span class="sxs-lookup"><span data-stu-id="0ebe1-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="0ebe1-136">Che cosa sono le prenotazioni di Azure?</span><span class="sxs-lookup"><span data-stu-id="0ebe1-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="0ebe1-137">Acquisto di prenotazioni di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="0ebe1-138">Acquista prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="0ebe1-139">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="0ebe1-140">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="0ebe1-141">Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente</span><span class="sxs-lookup"><span data-stu-id="0ebe1-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="0ebe1-142">Dimensionamento delle VM per l'utilizzo massimo della prenotazione di Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="0ebe1-143">Acquisto di prenotazioni di Azure tramite l'API del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="0ebe1-144">[Acquistare istanze di VM riservate di Azure](/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="0ebe1-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="0ebe1-145">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure dalla sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="0ebe1-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="0ebe1-146">Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="0ebe1-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |