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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172218"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="597a1-104">Calcolo del prezzo unitario effettivo per l'utilizzo del piano di Azure</span><span class="sxs-lookup"><span data-stu-id="597a1-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="597a1-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="597a1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="597a1-106">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="597a1-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="597a1-107">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="597a1-107">The effective unit price</span></span>

<span data-ttu-id="597a1-108">Il prezzo unitario effettivo viene calcolato a livello di contatore (anziché a livello di risorsa) e viene modificato ogni giorno in base all'utilizzo del contatore.</span><span class="sxs-lookup"><span data-stu-id="597a1-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="597a1-109">Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:</span><span class="sxs-lookup"><span data-stu-id="597a1-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="597a1-110">Consumo, monitorato ogni giorno durante tutto il ciclo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="597a1-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="597a1-111">Costo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="597a1-111">Billable cost for the meter</span></span>
- <span data-ttu-id="597a1-112">Livelli (se applicabile)</span><span class="sxs-lookup"><span data-stu-id="597a1-112">Tiering (if applicable)</span></span>

<span data-ttu-id="597a1-113">Poiché il consumo viene monitorato ogni giorno durante l'intero ciclo di fatturazione, il prezzo unitario effettivo varia.</span><span class="sxs-lookup"><span data-stu-id="597a1-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="597a1-114">Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="597a1-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="597a1-115">La maggior parte delle modifiche al consumo si verifica dopo la quarta o la quinta posizione decimale.</span><span class="sxs-lookup"><span data-stu-id="597a1-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="597a1-116">Scoprire se il contatore usa i prezzi a livelli</span><span class="sxs-lookup"><span data-stu-id="597a1-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="597a1-117">Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo.</span><span class="sxs-lookup"><span data-stu-id="597a1-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="597a1-118">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="597a1-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="597a1-119">Selezionare **Vendi,** selezionare **Prezzi e offerte** e quindi selezionare Prezzi del piano di **Azure.**</span><span class="sxs-lookup"><span data-stu-id="597a1-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="597a1-120">Individuare il contatore in base all'ID e quindi scaricare i dati sui prezzi.</span><span class="sxs-lookup"><span data-stu-id="597a1-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="597a1-121">Calcolo di esempio</span><span class="sxs-lookup"><span data-stu-id="597a1-121">Sample calculation</span></span>

<span data-ttu-id="597a1-122">La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo aperto.</span><span class="sxs-lookup"><span data-stu-id="597a1-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="597a1-123">Nella tabella si applicano i valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="597a1-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="597a1-124">**UP** = Prezzo unitario della risorsa/ora = 0,868</span><span class="sxs-lookup"><span data-stu-id="597a1-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="597a1-125">**BCU** = unità di consumo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="597a1-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="597a1-126">**BC** = Costo fatturabile per il contatore = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="597a1-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="597a1-127">Ciò riflette una rettifica per lo sconto pec del 15%.</span><span class="sxs-lookup"><span data-stu-id="597a1-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="597a1-128">Viene quindi utilizzato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo.</span><span class="sxs-lookup"><span data-stu-id="597a1-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="597a1-129">**Prezzo unitario effettivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="597a1-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="597a1-130">Nota: il contatore in questo esempio non ha livelli di prezzi o altri sconti, ovvero i fattori prezzo unitario effettivo nelle percentuali di sconto e altre rettifiche.</span><span class="sxs-lookup"><span data-stu-id="597a1-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="597a1-131">Data</span><span class="sxs-lookup"><span data-stu-id="597a1-131">Date</span></span> | <span data-ttu-id="597a1-132">BCU (unità di consumo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="597a1-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="597a1-133">BC (costo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="597a1-133">BC (Billable cost)</span></span> | <span data-ttu-id="597a1-134">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="597a1-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="597a1-135">3 ago</span><span class="sxs-lookup"><span data-stu-id="597a1-135">3-Aug</span></span> | <span data-ttu-id="597a1-136">29</span><span class="sxs-lookup"><span data-stu-id="597a1-136">29</span></span> | <span data-ttu-id="597a1-137">21.39</span><span class="sxs-lookup"><span data-stu-id="597a1-137">21.39</span></span> | <span data-ttu-id="597a1-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="597a1-138">0.737586206896552</span></span> |
| <span data-ttu-id="597a1-139">10 ago</span><span class="sxs-lookup"><span data-stu-id="597a1-139">10-Aug</span></span> | <span data-ttu-id="597a1-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="597a1-140">210.950039</span></span> | <span data-ttu-id="597a1-141">155.63</span><span class="sxs-lookup"><span data-stu-id="597a1-141">155.63</span></span> | <span data-ttu-id="597a1-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="597a1-142">0.737757626107858</span></span> |
| <span data-ttu-id="597a1-143">25 ago</span><span class="sxs-lookup"><span data-stu-id="597a1-143">25-Aug</span></span> | <span data-ttu-id="597a1-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="597a1-144">555.950039</span></span> | <span data-ttu-id="597a1-145">410.17</span><span class="sxs-lookup"><span data-stu-id="597a1-145">410.17</span></span> | <span data-ttu-id="597a1-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="597a1-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="597a1-147">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="597a1-147">Next steps</span></span>

- [<span data-ttu-id="597a1-148">Fatturazione e imposte</span><span class="sxs-lookup"><span data-stu-id="597a1-148">Billing and taxes</span></span>](billing.md)
