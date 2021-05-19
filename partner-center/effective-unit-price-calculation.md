---
title: Calcolo del prezzo unitario effettivo
ms.topic: how-to
ms.date: 04/02/2021
description: Informazioni sul prezzo unitario effettivo e su come viene calcolato. Questo articolo include anche un calcolo di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147123"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="1b30c-104">Calcolo del prezzo unitario effettivo per il consumo del piano di Azure</span><span class="sxs-lookup"><span data-stu-id="1b30c-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="1b30c-105">**Ruoli appropriati:** Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="1b30c-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="1b30c-106">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="1b30c-106">The effective unit price</span></span>

<span data-ttu-id="1b30c-107">Il prezzo unitario effettivo viene calcolato a livello di contatore (anziché a livello di risorsa) e viene regolato ogni giorno in base all'utilizzo del contatore.</span><span class="sxs-lookup"><span data-stu-id="1b30c-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="1b30c-108">Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:</span><span class="sxs-lookup"><span data-stu-id="1b30c-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="1b30c-109">Consumo, che viene monitorato quotidianamente durante tutto il ciclo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="1b30c-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="1b30c-110">Costo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="1b30c-110">Billable cost for the meter</span></span>
- <span data-ttu-id="1b30c-111">A livelli (se applicabile)</span><span class="sxs-lookup"><span data-stu-id="1b30c-111">Tiering (if applicable)</span></span>

<span data-ttu-id="1b30c-112">Poiché il consumo viene monitorato quotidianamente durante tutto il ciclo di fatturazione, il prezzo unitario effettivo varia.</span><span class="sxs-lookup"><span data-stu-id="1b30c-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="1b30c-113">Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="1b30c-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="1b30c-114">La maggior parte delle modifiche al consumo si verifica dopo la quarta o la quinta posizione decimale.</span><span class="sxs-lookup"><span data-stu-id="1b30c-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="1b30c-115">Scoprire se il contatore usa i prezzi a livelli</span><span class="sxs-lookup"><span data-stu-id="1b30c-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="1b30c-116">Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo.</span><span class="sxs-lookup"><span data-stu-id="1b30c-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="1b30c-117">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="1b30c-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1b30c-118">Selezionare **Sell (Vendi),** **selezionare Pricing and offers (Prezzi e** offerte) e quindi selezionare Azure plan pricing **(Prezzi del piano di Azure).**</span><span class="sxs-lookup"><span data-stu-id="1b30c-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="1b30c-119">Individuare il contatore in base all'ID e quindi scaricare i dati sui prezzi.</span><span class="sxs-lookup"><span data-stu-id="1b30c-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="1b30c-120">Calcolo di esempio</span><span class="sxs-lookup"><span data-stu-id="1b30c-120">Sample calculation</span></span>

<span data-ttu-id="1b30c-121">La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo di apertura.</span><span class="sxs-lookup"><span data-stu-id="1b30c-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="1b30c-122">Nella tabella si applicano i valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="1b30c-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="1b30c-123">**UP** = Prezzo unitario della risorsa/ora = 0,868</span><span class="sxs-lookup"><span data-stu-id="1b30c-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="1b30c-124">**BCU** = unità di consumo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="1b30c-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="1b30c-125">**BC** = Costo fatturabile per il contatore = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="1b30c-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="1b30c-126">Ciò riflette una rettifica per lo sconto pec del 15%.</span><span class="sxs-lookup"><span data-stu-id="1b30c-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="1b30c-127">Viene quindi utilizzato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo.</span><span class="sxs-lookup"><span data-stu-id="1b30c-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="1b30c-128">**Prezzo unitario effettivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="1b30c-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="1b30c-129">Nota: il contatore in questo esempio non ha livelli di prezzi o altri sconti, ovvero i fattori prezzo unitario effettivo nelle percentuali di sconto e altre rettifiche.</span><span class="sxs-lookup"><span data-stu-id="1b30c-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="1b30c-130">Data</span><span class="sxs-lookup"><span data-stu-id="1b30c-130">Date</span></span> | <span data-ttu-id="1b30c-131">BCU (unità di consumo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="1b30c-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="1b30c-132">BC (costo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="1b30c-132">BC (Billable cost)</span></span> | <span data-ttu-id="1b30c-133">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="1b30c-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="1b30c-134">3 ago</span><span class="sxs-lookup"><span data-stu-id="1b30c-134">3-Aug</span></span> | <span data-ttu-id="1b30c-135">29</span><span class="sxs-lookup"><span data-stu-id="1b30c-135">29</span></span> | <span data-ttu-id="1b30c-136">21.39</span><span class="sxs-lookup"><span data-stu-id="1b30c-136">21.39</span></span> | <span data-ttu-id="1b30c-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="1b30c-137">0.737586206896552</span></span> |
| <span data-ttu-id="1b30c-138">10 ago</span><span class="sxs-lookup"><span data-stu-id="1b30c-138">10-Aug</span></span> | <span data-ttu-id="1b30c-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="1b30c-139">210.950039</span></span> | <span data-ttu-id="1b30c-140">155.63</span><span class="sxs-lookup"><span data-stu-id="1b30c-140">155.63</span></span> | <span data-ttu-id="1b30c-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="1b30c-141">0.737757626107858</span></span> |
| <span data-ttu-id="1b30c-142">25 ago</span><span class="sxs-lookup"><span data-stu-id="1b30c-142">25-Aug</span></span> | <span data-ttu-id="1b30c-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="1b30c-143">555.950039</span></span> | <span data-ttu-id="1b30c-144">410.17</span><span class="sxs-lookup"><span data-stu-id="1b30c-144">410.17</span></span> | <span data-ttu-id="1b30c-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="1b30c-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="1b30c-146">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="1b30c-146">Next steps</span></span>

- [<span data-ttu-id="1b30c-147">Fatturazione e imposte</span><span class="sxs-lookup"><span data-stu-id="1b30c-147">Billing and taxes</span></span>](billing.md)
