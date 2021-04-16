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
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528567"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="67245-104">Calcolo del prezzo unitario effettivo per il consumo del piano di Azure</span><span class="sxs-lookup"><span data-stu-id="67245-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="67245-105">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="67245-105">The effective unit price</span></span>

<span data-ttu-id="67245-106">Il prezzo unitario effettivo viene calcolato a livello di contatore (anziché a livello di risorsa) e viene regolato ogni giorno in base all'utilizzo del contatore.</span><span class="sxs-lookup"><span data-stu-id="67245-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="67245-107">Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:</span><span class="sxs-lookup"><span data-stu-id="67245-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="67245-108">Consumo, che viene monitorato quotidianamente durante tutto il ciclo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="67245-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="67245-109">Costo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="67245-109">Billable cost for the meter</span></span>
- <span data-ttu-id="67245-110">Tiering (se applicabile)</span><span class="sxs-lookup"><span data-stu-id="67245-110">Tiering (if applicable)</span></span>

<span data-ttu-id="67245-111">Poiché il consumo viene monitorato quotidianamente durante tutto il ciclo di fatturazione, il prezzo unitario effettivo varia.</span><span class="sxs-lookup"><span data-stu-id="67245-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="67245-112">Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="67245-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="67245-113">La maggior parte delle modifiche al consumo si verifica dopo la quarta o la quinta posizione decimale.</span><span class="sxs-lookup"><span data-stu-id="67245-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="67245-114">Scoprire se il contatore usa i prezzi a più livelli</span><span class="sxs-lookup"><span data-stu-id="67245-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="67245-115">Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo.</span><span class="sxs-lookup"><span data-stu-id="67245-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="67245-116">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="67245-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="67245-117">Selezionare **Sell (Vendi),** **selezionare Pricing and offers (Prezzi e** offerte) e quindi selezionare Azure plan pricing **(Prezzi del piano di Azure).**</span><span class="sxs-lookup"><span data-stu-id="67245-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="67245-118">Individuare il contatore in base all'ID e quindi scaricare i dati sui prezzi.</span><span class="sxs-lookup"><span data-stu-id="67245-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="67245-119">Calcolo di esempio</span><span class="sxs-lookup"><span data-stu-id="67245-119">Sample calculation</span></span>

<span data-ttu-id="67245-120">La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo di apertura.</span><span class="sxs-lookup"><span data-stu-id="67245-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="67245-121">Nella tabella si applicano i valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="67245-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="67245-122">**UP** = Prezzo unitario della risorsa/ora = 0,868</span><span class="sxs-lookup"><span data-stu-id="67245-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="67245-123">**BCU** = unità di consumo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="67245-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="67245-124">**BC** = Costo fatturabile per il contatore = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="67245-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="67245-125">Ciò riflette una rettifica per lo sconto pec del 15%.</span><span class="sxs-lookup"><span data-stu-id="67245-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="67245-126">Viene quindi utilizzato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo.</span><span class="sxs-lookup"><span data-stu-id="67245-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="67245-127">**Prezzo unitario effettivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="67245-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="67245-128">Nota: il contatore in questo esempio non ha livelli di prezzi o altri sconti, ovvero i fattori prezzo unitario effettivo nelle percentuali di sconto e altre rettifiche.</span><span class="sxs-lookup"><span data-stu-id="67245-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="67245-129">Data</span><span class="sxs-lookup"><span data-stu-id="67245-129">Date</span></span> | <span data-ttu-id="67245-130">BCU (unità di consumo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="67245-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="67245-131">BC (costo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="67245-131">BC (Billable cost)</span></span> | <span data-ttu-id="67245-132">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="67245-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="67245-133">3 ago</span><span class="sxs-lookup"><span data-stu-id="67245-133">3-Aug</span></span> | <span data-ttu-id="67245-134">29</span><span class="sxs-lookup"><span data-stu-id="67245-134">29</span></span> | <span data-ttu-id="67245-135">21.39</span><span class="sxs-lookup"><span data-stu-id="67245-135">21.39</span></span> | <span data-ttu-id="67245-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="67245-136">0.737586206896552</span></span> |
| <span data-ttu-id="67245-137">10 ago</span><span class="sxs-lookup"><span data-stu-id="67245-137">10-Aug</span></span> | <span data-ttu-id="67245-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="67245-138">210.950039</span></span> | <span data-ttu-id="67245-139">155.63</span><span class="sxs-lookup"><span data-stu-id="67245-139">155.63</span></span> | <span data-ttu-id="67245-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="67245-140">0.737757626107858</span></span> |
| <span data-ttu-id="67245-141">25 ago</span><span class="sxs-lookup"><span data-stu-id="67245-141">25-Aug</span></span> | <span data-ttu-id="67245-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="67245-142">555.950039</span></span> | <span data-ttu-id="67245-143">410.17</span><span class="sxs-lookup"><span data-stu-id="67245-143">410.17</span></span> | <span data-ttu-id="67245-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="67245-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="67245-145">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="67245-145">Next steps</span></span>

- [<span data-ttu-id="67245-146">Fatturazione e imposte</span><span class="sxs-lookup"><span data-stu-id="67245-146">Billing and taxes</span></span>](billing.md)
