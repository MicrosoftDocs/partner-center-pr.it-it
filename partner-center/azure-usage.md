---
title: Dimensionamento delle VM di Azure per l'utilizzo massimo delle prenotazioni
ms.topic: how-to
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come ridimensionare una macchina virtuale (VM) in base alle esigenze di elaborazione dei clienti quando si acquistano Microsoft Azure prenotazioni.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: bc9fc14598e7c96f9cc1b55eba7c59af68ad84a9
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900109"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="652cb-103">Ridimensionamento della macchina virtuale di Microsoft Azure per l'utilizzo massimo delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="652cb-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="652cb-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="652cb-104">**Applies to**</span></span>

- <span data-ttu-id="652cb-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-105">Partner Center</span></span>
- <span data-ttu-id="652cb-106">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-106">Azure portal</span></span>
- <span data-ttu-id="652cb-107">Partner aderenti al programma CSP</span><span class="sxs-lookup"><span data-stu-id="652cb-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="652cb-108">Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="652cb-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="652cb-109">I clienti che usano altri tipi di sottoscrizioni, ad esempio con pagamento in base al consumo, singoli contratti Microsoft o sottoscrizioni di Enterprise Agreement, dovranno invece leggere [la documentazione relativa alle prenotazioni di Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="652cb-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="652cb-110">Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente</span><span class="sxs-lookup"><span data-stu-id="652cb-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="652cb-111">Quando si acquistano Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) ridimensionata per soddisfare le esigenze di calcolo del cliente.</span><span class="sxs-lookup"><span data-stu-id="652cb-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="652cb-112">È possibile trovare queste informazioni usando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="652cb-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="652cb-113">API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-113">Azure utilization API</span></span>
- <span data-ttu-id="652cb-114">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-114">The Azure portal</span></span>
- <span data-ttu-id="652cb-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="652cb-115">Azure PowerShell</span></span>
- <span data-ttu-id="652cb-116">API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="652cb-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="652cb-117">Di seguito sono riportate le istruzioni per l'uso di ognuno di questi metodi.</span><span class="sxs-lookup"><span data-stu-id="652cb-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="652cb-118">Dopo l'acquisto di una prenotazione, lo sconto relativo alla prenotazione viene applicato automaticamente alle macchine virtuali corrispondenti agli attributi e alla quantità della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="652cb-119">Non è necessario assegnare la prenotazione a una macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="652cb-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="652cb-120">Gli sconti per le prenotazioni non si applicano alle VM classiche o promozionali.</span><span class="sxs-lookup"><span data-stu-id="652cb-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="652cb-121">Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, è necessario usare uno dei metodi descritti di seguito poiché il tipo di serie di VM non viene visualizzato correttamente nei file di riconciliazione del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="652cb-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="652cb-122">Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="652cb-123">Usare il valore per l'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare.</span><span class="sxs-lookup"><span data-stu-id="652cb-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="652cb-124">Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="652cb-124">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="652cb-125">Ottenere informazioni sul dimensionamento della macchina virtuale usando il portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="652cb-126">Nel centro per i partner passare alla pagina **Customers (clienti** ).</span><span class="sxs-lookup"><span data-stu-id="652cb-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="652cb-127">Trovare il cliente che desidera acquistare le prenotazioni di macchine virtuali di Azure e quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="652cb-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="652cb-128">Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="652cb-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="652cb-129">Selezionare **macchine virtuali** dal menu del portale e quindi selezionare la macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="652cb-130">Nella pagina dei dettagli della macchina virtuale individuare le informazioni sulle dimensioni e sull'area, come illustrato di seguito, e usare queste informazioni per acquistare la prenotazione nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="652cb-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informazioni sulle dimensioni e sull'area nella pagina Dettagli":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="652cb-132">Ottenere informazioni sul dimensionamento della macchina virtuale usando Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="652cb-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="652cb-133">Usare le informazioni nell'immagine seguente per ottenere la posizione e le dimensioni della macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Posizione e dimensioni della macchina virtuale":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="652cb-135">Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="652cb-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="652cb-136">Usando le API ARMClient o ARM, chiamare il client ARM per la macchina virtuale per cui si vuole acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="652cb-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="652cb-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="652cb-138">La chiamata restituisce i valori per **vmSize** e **location**, come illustrato di seguito.</span><span class="sxs-lookup"><span data-stu-id="652cb-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valore vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valore Location":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="652cb-141">Verificare l'utilizzo della macchina virtuale di Azure e lo sconto per</span><span class="sxs-lookup"><span data-stu-id="652cb-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="652cb-142">Dopo aver acquistato un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento dello spazio della VM in anticipo viene applicato automaticamente alle macchine virtuali che corrispondono agli attributi e alla quantità della prenotazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="652cb-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="652cb-143">È possibile verificare l'utilizzo della prenotazione del cliente e vedere a quali macchine virtuali vengono applicati gli sconti per la prenotazione utilizzando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="652cb-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="652cb-144">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-144">The Azure portal</span></span>
- <span data-ttu-id="652cb-145">API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-145">Azure utilization API</span></span>

<span data-ttu-id="652cb-146">Di seguito sono riportate le istruzioni per l'uso di ognuno di questi metodi.</span><span class="sxs-lookup"><span data-stu-id="652cb-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="652cb-147">Solo l'API di utilizzo di Azure indica a quale macchina virtuale viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="652cb-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="652cb-148">Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="652cb-149">Nel centro per i partner passare alla pagina **Customers (clienti** ).</span><span class="sxs-lookup"><span data-stu-id="652cb-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="652cb-150">Individuare il cliente per cui si desidera verificare lo sconto e l'utilizzo della prenotazione, quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="652cb-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="652cb-151">Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="652cb-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="652cb-152">Selezionare **prenotazioni** dal menu del portale e quindi selezionare la prenotazione per cui si vuole controllare l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="652cb-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="652cb-153">Nella pagina **Panoramica** controllare il grafico di utilizzo della prenotazione, che mostra la quantità di prenotazione applicata alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="652cb-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="652cb-154">I dati di utilizzo possono essere posticipati di un massimo di 8 ore.</span><span class="sxs-lookup"><span data-stu-id="652cb-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="652cb-155">a.</span><span class="sxs-lookup"><span data-stu-id="652cb-155">a.</span></span> <span data-ttu-id="652cb-156">Se l'utilizzo della prenotazione è pari al 100%, il cliente è in grado di ottenere tutti i risparmi possibili che possono essere forniti dall'acquisto della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="652cb-157">b.</span><span class="sxs-lookup"><span data-stu-id="652cb-157">b.</span></span> <span data-ttu-id="652cb-158">Se l'utilizzo della prenotazione è 0%, lo sconto non viene applicato a nessuna macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="652cb-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="652cb-159">c.</span><span class="sxs-lookup"><span data-stu-id="652cb-159">c.</span></span> <span data-ttu-id="652cb-160">Se l'utilizzo della prenotazione è compreso tra 1% e 99%, i vantaggi non vengono usati.</span><span class="sxs-lookup"><span data-stu-id="652cb-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="652cb-161">Per evitare questa situazione, determinare la VM di dimensioni corrette per supportare le esigenze di calcolo del cliente prima di effettuare l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="652cb-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="652cb-162">Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="652cb-163">Solo l'API di utilizzo di Azure indica a quale macchina virtuale viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="652cb-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="652cb-164">È possibile ottenere i dati di utilizzo delle prenotazioni con l'API di utilizzo di Azure per verificare che il cliente ottenga lo sconto per la prenotazione e per vedere a quali macchine virtuali (macchine virtuali) viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="652cb-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="652cb-165">Confrontare l'esempio a all'esempio B per vedere come verificare l'utilizzo della prenotazione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="652cb-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Esempi di utilizzo della prenotazione":::

- <span data-ttu-id="652cb-167">ReservationId identifica la prenotazione di Azure usata per applicare lo sconto alla macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="652cb-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="652cb-168">consumptionMeter è il ID contatore per la macchina virtuale a cui è applicato lo sconto di prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="652cb-169">Il ReservationMeter Mostra il costo $0 poiché è stato applicato lo sconto di prenotazione.</span><span class="sxs-lookup"><span data-stu-id="652cb-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="652cb-170">Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.</span><span class="sxs-lookup"><span data-stu-id="652cb-170">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="652cb-171">I costi del software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione della macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura.</span><span class="sxs-lookup"><span data-stu-id="652cb-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="652cb-172">Tuttavia, se un cliente ha il vantaggio Azure Hybrid use, i costi del software non verranno applicati.</span><span class="sxs-lookup"><span data-stu-id="652cb-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="652cb-173">Per ulteriori informazioni, vedere [costi del software Windows non inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="652cb-173">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="652cb-174">Risorse per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-174">Azure reservations resources</span></span>

|<span data-ttu-id="652cb-175">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="652cb-175">**For information about**</span></span>   |<span data-ttu-id="652cb-176">**Leggi**</span><span class="sxs-lookup"><span data-stu-id="652cb-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="652cb-177">Panoramica sulle prenotazioni di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="652cb-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="652cb-178">Vendere Microsoft Azure istanze di VM riservate</span><span class="sxs-lookup"><span data-stu-id="652cb-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="652cb-179">Acquisto di prenotazioni di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="652cb-180">Acquista prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="652cb-181">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="652cb-182">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="652cb-183">Acquisto di prenotazioni di Azure nell'portale di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="652cb-184">[Pagamento anticipato per le macchine virtuali con le istanze di VM riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-184">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="652cb-185">Gestione delle prenotazioni di Azure nell'portale di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="652cb-186">[Gestire le istanze di VM riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-186">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="652cb-187">Acquisto di prenotazioni di Azure tramite l'API del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="652cb-188">[Acquistare istanze di VM riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="652cb-188">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="652cb-189">Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata.</span><span class="sxs-lookup"><span data-stu-id="652cb-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="652cb-190">Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="652cb-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
