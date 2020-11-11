---
title: Calcolo effettivo del prezzo unitario
ms.topic: how-to
ms.date: 11/10/2020
description: Informazioni sull'unità di prezzo effettiva e su come viene calcolata. Include un calcolo di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498568"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="c3f0d-104">Calcolo effettivo del prezzo unitario per il consumo di piani di Azure</span><span class="sxs-lookup"><span data-stu-id="c3f0d-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="c3f0d-105">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="c3f0d-105">The effective unit price</span></span>

<span data-ttu-id="c3f0d-106">Il prezzo unitario effettivo viene calcolato a livello di contatore (a differenza del livello di risorsa) e viene regolato quotidianamente in base all'utilizzo del contatore.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="c3f0d-107">Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:</span><span class="sxs-lookup"><span data-stu-id="c3f0d-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="c3f0d-108">Consumo, che viene monitorato ogni giorno durante il ciclo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="c3f0d-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="c3f0d-109">Costo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="c3f0d-109">Billable cost for the meter</span></span>
- <span data-ttu-id="c3f0d-110">Suddivisione in livelli (se applicabile)</span><span class="sxs-lookup"><span data-stu-id="c3f0d-110">Tiering (if applicable)</span></span>

<span data-ttu-id="c3f0d-111">Poiché il consumo giornaliero viene monitorato durante il ciclo di fatturazione, il prezzo unitario effettivo fluttua.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="c3f0d-112">Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="c3f0d-113">Si noterà la maggior parte delle modifiche a consumo dopo la quarta o la quinta posizione decimale.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="c3f0d-114">Verificare se il contatore usa i prezzi a livelli</span><span class="sxs-lookup"><span data-stu-id="c3f0d-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="c3f0d-115">Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="c3f0d-116">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="c3f0d-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="c3f0d-117">Selezionare **Vendi** , selezionare **prezzi e offerte** , quindi selezionare **piano tariffario di Azure**.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="c3f0d-118">Individuare il contatore in base all'ID e quindi scaricare i dati relativi ai prezzi.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="c3f0d-119">Calcolo di esempio</span><span class="sxs-lookup"><span data-stu-id="c3f0d-119">Sample calculation</span></span>

<span data-ttu-id="c3f0d-120">La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo di apertura.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="c3f0d-121">Nella tabella vengono applicati i valori seguenti:</span><span class="sxs-lookup"><span data-stu-id="c3f0d-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="c3f0d-122">**Up** = prezzo unitario della risorsa/ora = 0,868</span><span class="sxs-lookup"><span data-stu-id="c3f0d-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="c3f0d-123">**BCU** = unità di consumo fatturabile per il contatore</span><span class="sxs-lookup"><span data-stu-id="c3f0d-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="c3f0d-124">**BC** = costo fatturabile per il contatore = BCU \* fino \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="c3f0d-125">Ciò riflette una modifica per lo sconto del 15% PEC.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="c3f0d-126">Viene quindi usato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="c3f0d-127">**Prezzo unitario effettivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="c3f0d-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="c3f0d-128">Nota: il contatore in questo esempio non include livelli nei prezzi.</span><span class="sxs-lookup"><span data-stu-id="c3f0d-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="c3f0d-129">Data</span><span class="sxs-lookup"><span data-stu-id="c3f0d-129">Date</span></span> | <span data-ttu-id="c3f0d-130">BCU (unità fatturabile a consumo)</span><span class="sxs-lookup"><span data-stu-id="c3f0d-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="c3f0d-131">BC (costo fatturabile)</span><span class="sxs-lookup"><span data-stu-id="c3f0d-131">BC (Billable cost)</span></span> | <span data-ttu-id="c3f0d-132">Prezzo unitario effettivo</span><span class="sxs-lookup"><span data-stu-id="c3f0d-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="c3f0d-133">3 agosto</span><span class="sxs-lookup"><span data-stu-id="c3f0d-133">3-Aug</span></span> | <span data-ttu-id="c3f0d-134">29</span><span class="sxs-lookup"><span data-stu-id="c3f0d-134">29</span></span> | <span data-ttu-id="c3f0d-135">21,39</span><span class="sxs-lookup"><span data-stu-id="c3f0d-135">21.39</span></span> | <span data-ttu-id="c3f0d-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="c3f0d-136">0.737586206896552</span></span> |
| <span data-ttu-id="c3f0d-137">10 agosto</span><span class="sxs-lookup"><span data-stu-id="c3f0d-137">10-Aug</span></span> | <span data-ttu-id="c3f0d-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="c3f0d-138">210.950039</span></span> | <span data-ttu-id="c3f0d-139">155,63</span><span class="sxs-lookup"><span data-stu-id="c3f0d-139">155.63</span></span> | <span data-ttu-id="c3f0d-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="c3f0d-140">0.737757626107858</span></span> |
| <span data-ttu-id="c3f0d-141">25 agosto</span><span class="sxs-lookup"><span data-stu-id="c3f0d-141">25-Aug</span></span> | <span data-ttu-id="c3f0d-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="c3f0d-142">555.950039</span></span> | <span data-ttu-id="c3f0d-143">410,17</span><span class="sxs-lookup"><span data-stu-id="c3f0d-143">410.17</span></span> | <span data-ttu-id="c3f0d-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="c3f0d-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="c3f0d-145">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c3f0d-145">Next steps</span></span>

- [<span data-ttu-id="c3f0d-146">Fatturazione e imposte</span><span class="sxs-lookup"><span data-stu-id="c3f0d-146">Billing and taxes</span></span>](billing.md)
