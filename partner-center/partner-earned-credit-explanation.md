---
title: Credito ottenuto dai partner per i servizi gestiti
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come viene calcolato e pagato il credito ottenuto dai partner Microsoft (PEC) per i servizi gestiti e come verificare se possiedi i requisiti richiesti.
author: dineshvu
ms.author: dineshvu
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 553d23fcd33f290d976f789657ee9ad71dbcae46
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949399"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="d9e3b-103">Come viene calcolato e pagato il credito ottenuto dai partner</span><span class="sxs-lookup"><span data-stu-id="d9e3b-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="d9e3b-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="d9e3b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d9e3b-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="d9e3b-105">Global admin</span></span>
- <span data-ttu-id="d9e3b-106">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="d9e3b-106">User admin</span></span>
- <span data-ttu-id="d9e3b-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="d9e3b-107">Admin agent</span></span>
- <span data-ttu-id="d9e3b-108">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="d9e3b-108">Billing admin</span></span>
- <span data-ttu-id="d9e3b-109">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="d9e3b-109">Sales agent</span></span>

<span data-ttu-id="d9e3b-110">Il credito ottenuto dai partner per i servizi gestiti (PEC) riconosce e premia i partner a cui sono affidati il controllo e la gestione operativi IT 24 ore su 24, 7 giorni su 7, dell'ambiente Azure intero o parziale dei clienti.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="d9e3b-111">Per impostazione predefinita, in CSP ai partner vengono concessi i necessari diritti di accesso alla sottoscrizione del cliente, in modo che possano eseguire 24 ore su 24, 7 giorni su 7 la gestione e il controllo operativi delle risorse della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="d9e3b-112">Nella sezione seguente vengono descritti altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="d9e3b-113">L'importo delle fatture mensili è al netto del credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="d9e3b-114">I partner possono esaminare nel file di riconciliazione mensile i dettagli del credito ottenuto.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="d9e3b-115">Per gli altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione, leggi [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="d9e3b-116">Leggi anche [Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="d9e3b-117">Importanti informazioni su idoneità e calcolo</span><span class="sxs-lookup"><span data-stu-id="d9e3b-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="d9e3b-118">Il partner deve disporre di un contratto MPN attivo e di un ruolo Controllo degli accessi in base al ruolo valido per ricevere il credito ottenuto per gli asset di Azure gestiti.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="d9e3b-119">Nel caso di provider indiretti e dei relativi rivenditori indiretti, il provider indiretto sarà idoneo per il credito ottenuto dai partner se egli stesso, il rivenditore indiretto oppure entrambi esercitano 24 ore su 24, 7 giorni su 7 il controllo e la gestione operativi delle risorse di Azure del cliente in CSP.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="d9e3b-120">Il credito ottenuto dai partner è associato all'utilizzo (addebitabile) fatturato dell'ambiente Azure del cliente in CSP gestito dal partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="d9e3b-121">Il credito ottenuto dai partner viene reso disponibile solo ai partner in CSP fatturati da Microsoft (provider indiretto e partner con fatturazione diretta).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="d9e3b-122">Servizi idonei: il credito ottenuto dai partner è applicabile ai servizi elencati nei **prezzi per l'utilizzo del piano di Azure** che i partner possono esportare dalla pagina dei [prezzi del piano di Azure](https://partner.microsoft.com/commerce/sales).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="d9e3b-123">Si noti che esistono eccezioni, tra cui i prodotti di terze parti identificati come **Terze parti** nella colonna **Tags** del listino prezzi relativo ai consumi del piano di Azure, le prenotazioni del piano di Azure e i prodotti del listino prezzi di Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-123">Note, there are exceptions including, but not limited to, third-party products identified as **Third Party** in  the **Tags** column of the Azure plan consumption price list and Azure Plan reservations, and products in the Marketplace price list.</span></span>

- <span data-ttu-id="d9e3b-124">Il credito ottenuto dai partner viene calcolato quotidianamente e può essere controllato nel file di utilizzo giornaliero e nel file di riconciliazione della fattura mensile.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="d9e3b-125">Un partner (provider indiretto o rivenditore indiretto) deve avere accesso per l'intero giorno (24 ore su 24, 7 giorni su 7) per ottenere il credito.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>  

- <span data-ttu-id="d9e3b-126">Il credito viene ottenuto dai partner a livello delle risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-126">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="d9e3b-127">Se il partner dispone di un accesso valido a livello di sottoscrizione o di gruppo di risorse, otterrà il credito ogni risorsa con ruolo autorizzato fino all'entità più alta.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-127">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="d9e3b-128">I dettagli relativi al credito ottenuto dai partner saranno disponibili anche in [Gestione costi di Azure](https://go.microsoft.com/fwlink/?linkid=2106482).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-128">PEC details will also be available on [Azure Cost management](https://go.microsoft.com/fwlink/?linkid=2106482)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="d9e3b-129">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="d9e3b-129">Azure Cost Management</span></span>

 <span data-ttu-id="d9e3b-130">Gestione costi di Azure (ACM) con Analisi dei costi consente a ogni partner di visualizzare i costi che hanno ricevuto il vantaggio di credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-130">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="d9e3b-131">Nel portale di Azure accedi al tenant partner e seleziona **Gestione dei costi e fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-131">In the Azure Portal, sign into your partner tenant and select **Cost Management + Billing**.</span></span>
2.  <span data-ttu-id="d9e3b-132">Seleziona **Gestione costi**.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-132">Select **Cost management**</span></span>
3.  <span data-ttu-id="d9e3b-133">Seleziona **Analisi dei costi**.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-133">Select **Cost Analysis**</span></span>

<span data-ttu-id="d9e3b-134">Nella visualizzazione Analisi dei costi verranno visualizzati i costi per l'account di fatturazione relativi a tutti i servizi acquistati e utilizzati ai prezzi pagati a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-134">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4.  <span data-ttu-id="d9e3b-135">Seleziona **PartnerEarnedCreditApplied** nell'elenco a discesa di un grafico pivot per visualizzare i costi a cui è applicato il credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-135">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="d9e3b-136">Quando la proprietà **PartnerEarnedCreditApplied** è True, il costo associato ha il vantaggio di credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-136">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="d9e3b-137">Quando la proprietà PartnerEarnedCreditApplied è False, il costo associato non soddisfa il criterio di idoneità del credito o il servizio acquistato non è idoneo al credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-137">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="d9e3b-138">Sono in genere necessarie 8-24 ore prima che l'uso dei servizi in **Gestione costi** diventi visibile, mentre i crediti ottenuti dai partner vengono visualizzati entro 48 ore dal momento dell'accesso in Gestione costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-138">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="d9e3b-139">Puoi anche raggruppare o filtrare in base alla proprietà **PartnerEarnedCreditApplied** usando le funzionalità di filtro **Raggruppa per e Aggiungi** per visualizzare in dettaglio i costi a cui è applicato il credito ottenuto dai partner e quelli a cui tale credito non è applicato.</span><span class="sxs-lookup"><span data-stu-id="d9e3b-139">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d9e3b-140">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d9e3b-140">Next steps</span></span>

- [<span data-ttu-id="d9e3b-141">Credito ottenuto dai partner - Panoramica</span><span class="sxs-lookup"><span data-stu-id="d9e3b-141">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="d9e3b-142">Esempi dettagliati di calcoli di credito ottenuto dai partner sono disponibili nel listino prezzi accessibile tramite il dashboard del Centro per i partner (informazioni di accesso obbligatorie).</span><span class="sxs-lookup"><span data-stu-id="d9e3b-142">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="d9e3b-143">Passare al piano di Azure - Introduzione</span><span class="sxs-lookup"><span data-stu-id="d9e3b-143">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="d9e3b-144">Gestire sottoscrizioni e risorse nel piano di Azure</span><span class="sxs-lookup"><span data-stu-id="d9e3b-144">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="d9e3b-145">Revocare e ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP</span><span class="sxs-lookup"><span data-stu-id="d9e3b-145">Revoke or re-instate admin privileges for Azure CSP subscriptions  </span></span>](revoke-reinstate-csp.md)

