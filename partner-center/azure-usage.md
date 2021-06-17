---
title: Dimensionamento delle VM di Azure per l'utilizzo massimo delle prenotazioni
description: Informazioni su come ridimensionare una macchina virtuale (VM) in base alle esigenze di calcolo dei clienti quando si acquistano Microsoft Azure prenotazioni per loro.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 2d8bc76e0da51abf433e49028445b398c6a1db31
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276995"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="60c2b-103">Ridimensionamento della macchina virtuale di Microsoft Azure per l'utilizzo massimo delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="60c2b-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="60c2b-104">**Ruoli appropriati:** amministrazione dell'agente | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="60c2b-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="60c2b-105">Questo articolo illustra come ridimensionare una macchina virtuale (VM) in base alle esigenze di calcolo dei clienti quando si acquistano Microsoft Azure prenotazioni.</span><span class="sxs-lookup"><span data-stu-id="60c2b-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="60c2b-106">Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="60c2b-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="60c2b-107">I clienti che usano altri tipi di sottoscrizioni (ad esempio, sottoscrizioni con pagamento in base al go, singole, Contratto del cliente Microsoft o Contratto Enterprise) devono invece leggere la documentazione sulle prenotazioni di [Azure.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="60c2b-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="60c2b-108">Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente</span><span class="sxs-lookup"><span data-stu-id="60c2b-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="60c2b-109">Quando si Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) dimensionata per soddisfare le esigenze di calcolo del cliente.</span><span class="sxs-lookup"><span data-stu-id="60c2b-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="60c2b-110">È possibile trovare queste informazioni usando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="60c2b-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="60c2b-111">API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-111">Azure utilization API</span></span>
- <span data-ttu-id="60c2b-112">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-112">The Azure portal</span></span>
- <span data-ttu-id="60c2b-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="60c2b-113">Azure PowerShell</span></span>
- <span data-ttu-id="60c2b-114">The Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="60c2b-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="60c2b-115">Le istruzioni per l'uso di ognuno di questi metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="60c2b-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="60c2b-116">Dopo aver acquistato una prenotazione, lo sconto per la prenotazione viene applicato automaticamente alle macchine virtuali corrispondenti agli attributi e alla quantità della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="60c2b-117">Non è necessario assegnare la prenotazione a una macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="60c2b-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="60c2b-118">Gli sconti per la prenotazione non si applicano alle macchine virtuali classiche o promozionali.</span><span class="sxs-lookup"><span data-stu-id="60c2b-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="60c2b-119">Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, è necessario usare uno dei metodi descritti di seguito perché il tipo di serie di macchine virtuali non viene visualizzato correttamente nei file Partner Center di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="60c2b-120">Ottenere informazioni sul dimensionamento delle macchine virtuali usando l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="60c2b-121">Usare il valore per l'attributo ServiceType di additionalInfo nella risposta api per identificare le dimensioni della macchina virtuale da acquistare.</span><span class="sxs-lookup"><span data-stu-id="60c2b-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="60c2b-122">Per altre informazioni, vedere Ottenere i record di utilizzo di un cliente [per Azure nell'API](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [Partner Center .](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="60c2b-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="60c2b-123">Ottenere informazioni sul dimensionamento delle macchine virtuali usando il portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="60c2b-124">In Partner Center passare alla **pagina** Clienti.</span><span class="sxs-lookup"><span data-stu-id="60c2b-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="60c2b-125">Trovare il cliente che vuole acquistare prenotazioni di macchine virtuali di Azure e quindi selezionare la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="60c2b-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="60c2b-126">Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="60c2b-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="60c2b-127">Selezionare **Macchine virtuali** dal menu del portale e quindi selezionare la macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="60c2b-128">Nella pagina dei dettagli della macchina virtuale trovare le informazioni sulle dimensioni e sull'area, come illustrato di seguito, e usare queste informazioni per acquistare la prenotazione in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="60c2b-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informazioni su dimensioni e area nella pagina dei dettagli.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="60c2b-130">Ottenere informazioni sul dimensionamento delle macchine virtuali usando Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="60c2b-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="60c2b-131">Usare le informazioni nell'immagine seguente per ottenere la posizione e le dimensioni della macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Posizione e dimensioni della macchina virtuale.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="60c2b-133">Ottenere informazioni sul dimensionamento delle macchine virtuali usando l'API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="60c2b-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="60c2b-134">Usando ARMClient o le API arm, chiamare il client ARM per la macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="60c2b-135">/subscriptions/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="60c2b-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="60c2b-136">La chiamata restituisce i valori per **vmSize** **e location**, come illustrato di seguito.</span><span class="sxs-lookup"><span data-stu-id="60c2b-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="Valore vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valore location.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="60c2b-139">Verificare l'utilizzo delle macchine virtuali di Azure e lo sconto per la prenotazione</span><span class="sxs-lookup"><span data-stu-id="60c2b-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="60c2b-140">Dopo aver acquistato un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento anticipato dello spazio della macchina virtuale viene applicato automaticamente alle macchine virtuali che corrispondono agli attributi e alla quantità della prenotazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="60c2b-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="60c2b-141">È possibile verificare l'utilizzo della prenotazione del cliente e vedere a quali macchine virtuali vengono applicati gli sconti della prenotazione usando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="60c2b-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="60c2b-142">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-142">The Azure portal</span></span>
- <span data-ttu-id="60c2b-143">API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-143">Azure utilization API</span></span>

<span data-ttu-id="60c2b-144">Le istruzioni per l'uso di ognuno di questi metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="60c2b-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="60c2b-145">Solo l'API di utilizzo di Azure mostra la macchina virtuale a cui viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="60c2b-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="60c2b-146">Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="60c2b-147">In Partner Center passare alla **pagina** Clienti.</span><span class="sxs-lookup"><span data-stu-id="60c2b-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="60c2b-148">Trovare il cliente di cui si desidera verificare lo sconto e l'utilizzo della prenotazione e quindi selezionare la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="60c2b-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="60c2b-149">Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="60c2b-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="60c2b-150">Selezionare **Prenotazioni dal** menu del portale e quindi selezionare la prenotazione per cui si vuole verificare l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="60c2b-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="60c2b-151">Nella pagina **Panoramica** controllare il grafico di utilizzo della prenotazione, che mostra la quantità di prenotazione applicata alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="60c2b-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="60c2b-152">I dati di utilizzo possono essere posticipati fino a 8 ore.</span><span class="sxs-lookup"><span data-stu-id="60c2b-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="60c2b-153">a.</span><span class="sxs-lookup"><span data-stu-id="60c2b-153">a.</span></span> <span data-ttu-id="60c2b-154">Se l'utilizzo della prenotazione è del 100%, il cliente sta ottenendo tutti i risparmi possibili che l'acquisto della prenotazione può offrire.</span><span class="sxs-lookup"><span data-stu-id="60c2b-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="60c2b-155">b.</span><span class="sxs-lookup"><span data-stu-id="60c2b-155">b.</span></span> <span data-ttu-id="60c2b-156">Se l'utilizzo della prenotazione è 0%, lo sconto non viene applicato ad alcuna macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="60c2b-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="60c2b-157">c.</span><span class="sxs-lookup"><span data-stu-id="60c2b-157">c.</span></span> <span data-ttu-id="60c2b-158">Se l'utilizzo della prenotazione è compreso tra l'1% e il 99%, si verificano vantaggi inutilizzati.</span><span class="sxs-lookup"><span data-stu-id="60c2b-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="60c2b-159">Per evitare questa situazione, determinare le dimensioni corrette della macchina virtuale per supportare le esigenze di calcolo del cliente prima di effettuare l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="60c2b-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="60c2b-160">Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="60c2b-161">Solo l'API di utilizzo di Azure mostra la macchina virtuale a cui viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="60c2b-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="60c2b-162">È possibile ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente otterrà lo sconto per la prenotazione e per vedere a quali macchine virtuali (macchine virtuali) viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="60c2b-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="60c2b-163">Confrontare l'esempio A con l'esempio B per verificare l'utilizzo della prenotazione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="60c2b-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Esempi di utilizzo della prenotazione.":::

- <span data-ttu-id="60c2b-165">ReservationId identifica la prenotazione di Azure usata per applicare lo sconto alla macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="60c2b-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="60c2b-166">consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto per la prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="60c2b-167">ReservationMeter mostra il costo di $ 0 dopo l'applicazione dello sconto per la prenotazione.</span><span class="sxs-lookup"><span data-stu-id="60c2b-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="60c2b-168">Per altre informazioni, vedere Ottenere i record di utilizzo di un cliente [per Azure nell'API](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [Partner Center .](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="60c2b-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="60c2b-169">I costi software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di vm e verranno visualizzati come voci separate nel record dell'ordine e nella fattura.</span><span class="sxs-lookup"><span data-stu-id="60c2b-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="60c2b-170">Tuttavia, se un cliente ha il vantaggio Azure Hybrid Use, i costi del software non verranno applicati.</span><span class="sxs-lookup"><span data-stu-id="60c2b-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="60c2b-171">Per altre informazioni, vedere [Costi software Windows non inclusi in Istanze riservate](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="60c2b-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="60c2b-172">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="60c2b-172">Next steps</span></span>

|<span data-ttu-id="60c2b-173">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="60c2b-173">**For information about**</span></span>   |<span data-ttu-id="60c2b-174">**Leggi**</span><span class="sxs-lookup"><span data-stu-id="60c2b-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="60c2b-175">Panoramica delle prenotazioni di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="60c2b-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="60c2b-176">Vendere Microsoft Azure di macchine virtuali riservate</span><span class="sxs-lookup"><span data-stu-id="60c2b-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="60c2b-177">Acquisto di prenotazioni di Azure per i clienti in Partner Center</span><span class="sxs-lookup"><span data-stu-id="60c2b-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="60c2b-178">Acquistare prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="60c2b-179">Gestione delle prenotazioni di Azure in Partner Center</span><span class="sxs-lookup"><span data-stu-id="60c2b-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="60c2b-180">Gestione delle prenotazioni di Azure in Partner Center</span><span class="sxs-lookup"><span data-stu-id="60c2b-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="60c2b-181">Acquisto di prenotazioni di Azure nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="60c2b-182">[Pagamento preliminare per le macchine virtuali con istanze di macchine](/azure/virtual-machines/windows/prepay-reserved-vm-instances) virtuali riservate di Azure nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="60c2b-183">Gestione delle prenotazioni di Azure nell'portale di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="60c2b-184">[Gestire le istanze di macchine virtuali riservate](/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="60c2b-185">Acquisto di prenotazioni di Azure tramite l'API Partner Center azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="60c2b-186">[Acquistare istanze di macchine virtuali riservate di Azure](/partner-center/develop/purchase-azure-reservations) nella documentazione Partner Center per sviluppatori</span><span class="sxs-lookup"><span data-stu-id="60c2b-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="60c2b-187">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata per loro.</span><span class="sxs-lookup"><span data-stu-id="60c2b-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="60c2b-188">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="60c2b-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |