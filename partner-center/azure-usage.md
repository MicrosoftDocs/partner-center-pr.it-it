---
title: Ridimensionamento della macchina virtuale Microsoft Azure per un utilizzo ottimale delle prenotazioni | Dashboard del partner
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, prenotazioni, vm, gestire, utilizzo, ridimensionamento
ms.openlocfilehash: 4050780f9d3dc3ad7d3c4ece0d363845ec1efe9c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/11/2018
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="b77af-103">Ridimensionamento della macchina virtuale Microsoft Azure per un utilizzo ottimale delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="b77af-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="b77af-104">Ambito di applicazione:</span><span class="sxs-lookup"><span data-stu-id="b77af-104">Applies to</span></span>**

-  <span data-ttu-id="b77af-105">Dashboard del partner</span><span class="sxs-lookup"><span data-stu-id="b77af-105">Partner Dashboard</span></span>
-  <span data-ttu-id="b77af-106">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-106">Azure portal</span></span>
-  <span data-ttu-id="b77af-107">Partner di CSP</span><span class="sxs-lookup"><span data-stu-id="b77af-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="b77af-108">Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente</span><span class="sxs-lookup"><span data-stu-id="b77af-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="b77af-109">Quando acquisti prenotazioni di Microsoft Azure per conto dei clienti, dovrai scegliere una macchina virtuale (VM) le cui dimensioni soddisfino le esigenze informatiche del cliente.</span><span class="sxs-lookup"><span data-stu-id="b77af-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="b77af-110">Puoi trovare queste informazioni scegliendo uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="b77af-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="b77af-111">API di utilizzo Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-111">Azure utilization API</span></span>
-   <span data-ttu-id="b77af-112">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-112">The Azure portal</span></span>
-   <span data-ttu-id="b77af-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b77af-113">Azure PowerShell</span></span>
-   <span data-ttu-id="b77af-114">L'API di Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b77af-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="b77af-115">Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="b77af-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="b77af-116">Dopo aver acquistato una prenotazione, il relativo sconto verrà applicato automaticamente alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b77af-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="b77af-117">Non è necessario assegnare la prenotazione a una macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="b77af-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="b77af-118">Gli sconti relativi alla prenotazione non vengono applicati alle macchine virtuali classiche o promozionali.</span><span class="sxs-lookup"><span data-stu-id="b77af-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="b77af-119">Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, dovrai utilizzare uno dei metodi descritti di seguito poiché la serie della macchina virtuale non viene visualizzata correttamente nei file di riconciliazione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b77af-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="b77af-120">Ottenere informazioni sul dimensionamento di una macchina virtuale mediante l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="b77af-121">Utilizza il valore dell'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare.</span><span class="sxs-lookup"><span data-stu-id="b77af-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="b77af-122">Per ulteriori informazioni, vedi [Ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell'[API del dashboard del partner](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="b77af-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="b77af-123">Ottenere informazioni sul dimensionamento di una macchina virtuale mediante il portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="b77af-124">Nel dashboard del partner, vai alla pagina **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="b77af-124">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="b77af-125">Trova il cliente che desidera acquistare prenotazioni della macchina virtuale di Azure, quindi seleziona la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="b77af-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="b77af-126">Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="b77af-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="b77af-127">Seleziona **Macchine virtuali** dal menu del portale, quindi seleziona la macchina virtuale per cui desideri acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b77af-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="b77af-128">Nella pagina dei dettagli della macchina virtuale, trova informazioni in merito a dimensioni e area geografica, come illustrato di seguito, e usa queste informazioni per acquistare la prenotazione nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b77af-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="b77af-129">Ottenere informazioni sul dimensionamento di una macchina virtuale mediante Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b77af-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="b77af-130">Per ottenere la posizione e le dimensioni della macchina virtuale per cui desideri acquistare una prenotazione, utilizza le informazioni nell'immagine seguente.</span><span class="sxs-lookup"><span data-stu-id="b77af-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="b77af-131">Ottenere informazioni sul dimensionamento di una macchina virtuale mediante l'API di Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="b77af-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="b77af-132">Tramite le API di ARMClient o ARM, chiama il client ARM per la macchina virtuale per cui desideri acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b77af-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="b77af-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="b77af-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="b77af-134">La chiamata restituisce valori per **vmSize** e **location**, come illustrato di seguito.</span><span class="sxs-lookup"><span data-stu-id="b77af-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="b77af-135">Verificare lo sconto su prenotazione e utilizzo della macchina virtuale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="b77af-136">Dopo l'acquisto di un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento anticipato dello spazio della macchina virtuale viene automaticamente applicato alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="b77af-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="b77af-137">Puoi verificare l'utilizzo della prenotazione del cliente e vedere le macchine virtuali a cui sono applicati gli sconti relativi alla prenotazione utilizzando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="b77af-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="b77af-138">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-138">The Azure portal</span></span>
-   <span data-ttu-id="b77af-139">API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-139">Azure utilization API</span></span>

<span data-ttu-id="b77af-140">Le istruzioni per l'uso di ciascuno di questi metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="b77af-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="b77af-141">Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="b77af-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="b77af-142">Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="b77af-143">Nel dashboard del partner, vai alla pagina **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="b77af-143">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="b77af-144">Trova il cliente di cui desideri verificare lo sconto e l'utilizzo della prenotazione, quindi seleziona la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="b77af-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="b77af-145">Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="b77af-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="b77af-146">Seleziona **Prenotazioni** dal menu del portale, quindi seleziona la prenotazione di cui desideri verificare l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="b77af-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="b77af-147">Nella pagina **Panoramica** controlla il grafico sull'utilizzo della prenotazione, che mostra in che parte la prenotazione è stata applicata alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="b77af-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="b77af-148">I dati di utilizzo possono essere ritardati fino a 8 ore.</span><span class="sxs-lookup"><span data-stu-id="b77af-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="b77af-149">a.</span><span class="sxs-lookup"><span data-stu-id="b77af-149">a.</span></span>  <span data-ttu-id="b77af-150">Se l'utilizzo della prenotazione è pari al 100%, il cliente ottiene tutto il risparmio che l'acquisto della prenotazione è in grado di offrire.</span><span class="sxs-lookup"><span data-stu-id="b77af-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="b77af-151">b.</span><span class="sxs-lookup"><span data-stu-id="b77af-151">b.</span></span>  <span data-ttu-id="b77af-152">Se l'utilizzo della prenotazione è pari allo 0%, lo sconto non viene applicato a nessuna macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="b77af-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="b77af-153">c.</span><span class="sxs-lookup"><span data-stu-id="b77af-153">c.</span></span>  <span data-ttu-id="b77af-154">Se l'utilizzo della prenotazione è compreso tra 1% e 99%, esistono vantaggi inutilizzati.</span><span class="sxs-lookup"><span data-stu-id="b77af-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="b77af-155">Per evitare questa situazione, scegli la macchina virtuale delle dimensioni corrette per supportare le esigenze di elaborazione del cliente prima di effettuare l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="b77af-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="b77af-156">Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="b77af-157">Solo l'API di utilizzo di Azure mostra a quale macchina virtuale viene applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="b77af-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="b77af-158">Puoi ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente riceva lo sconto prenotazione e per vedere a quali macchine virtuali è applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="b77af-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="b77af-159">Confronta l'esempio A con l'esempio B per scoprire come verificare l'utilizzo della prenotazione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="b77af-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="b77af-160">reservationId identifica la prenotazione di Azure utilizzata per applicare lo sconto alla macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="b77af-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="b77af-161">consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b77af-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="b77af-162">ReservationMeter mostra un costo di $ 0 perché è stato applicato lo sconto prenotazione.</span><span class="sxs-lookup"><span data-stu-id="b77af-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="b77af-163">Per ulteriori informazioni, vedi [Ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell'[API del dashboard del partner](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="b77af-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="b77af-164">I costi relativi al software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura.</span><span class="sxs-lookup"><span data-stu-id="b77af-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="b77af-165">Tuttavia, se un cliente ha il vantaggio Azure Hybrid Use, i costi del software non verranno applicati.</span><span class="sxs-lookup"><span data-stu-id="b77af-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="b77af-166">Per ulteriori informazioni, vedi [I costi del software Windows non sono inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="b77af-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="b77af-167">Risorse sulle prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-167">Azure reservations resources</span></span>
|**<span data-ttu-id="b77af-168">Per informazioni su</span><span class="sxs-lookup"><span data-stu-id="b77af-168">For information about</span></span>**   |**<span data-ttu-id="b77af-169">Leggi</span><span class="sxs-lookup"><span data-stu-id="b77af-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="b77af-170">Panoramica delle prenotazioni di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="b77af-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="b77af-171">Vendere istanze di macchina virtuale riservate di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="b77af-172">Acquisto di prenotazioni di Azure per i clienti nel dashboard del partner</span><span class="sxs-lookup"><span data-stu-id="b77af-172">Purchasing Azure reservations for your customers in your Partner Dashboard</span></span>   |[<span data-ttu-id="b77af-173">Acquistare prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="b77af-174">Fatturazione per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-174">Billing for Azure reservations</span></span>   |[<span data-ttu-id="b77af-175">Fatturazione per le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-175">Billing for Azure reservations</span></span>](azure-reservations-billing.md)   |
| <span data-ttu-id="b77af-176">Gestione delle prenotazioni di Azure nel dashboard del partner</span><span class="sxs-lookup"><span data-stu-id="b77af-176">Managing Azure reservations in your Partner Dashboard</span></span> | [<span data-ttu-id="b77af-177">Gestione delle prenotazioni di Azure nel dashboard del partner</span><span class="sxs-lookup"><span data-stu-id="b77af-177">Managing Azure reservations in your Partner Dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="b77af-178">Acquisto di prenotazioni di Azure nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-178">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="b77af-179">[Pagare in anticipo per macchine virtuali con istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-179">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="b77af-180">Gestione di prenotazioni di Azure nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-180">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="b77af-181">[Gestire le istanze di macchina virtuale riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="b77af-181">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="b77af-182">Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b77af-182">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="b77af-183">[Acquistare istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) nella documentazione per sviluppatori del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b77af-183">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) in the Partner Center developer documentation</span></span>



