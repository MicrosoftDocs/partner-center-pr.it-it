---
title: Ridimensionamento della macchina virtuale Microsoft Azure per l'utilizzo massimo della prenotazione | Centro per i partner
ms.topic: article
ms.date: 08/05/2019
Description: Quando acquisti prenotazioni di Microsoft Azure per conto dei clienti, dovrai scegliere una macchina virtuale (VM) le cui dimensioni soddisfino le esigenze informatiche del cliente.
author: LauraBrenner
ms.author: labrenne
keywords: azure, prenotazioni, vm, gestire, utilizzo, ridimensionamento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 1c1c0170c5efd8abf2e1afb7bb6ef1dfac2b7e5b
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820198"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="2ac5b-104">Ridimensionamento della macchina virtuale Microsoft Azure per un utilizzo ottimale delle prenotazioni</span><span class="sxs-lookup"><span data-stu-id="2ac5b-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="2ac5b-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-105">**Applies to**</span></span>

- <span data-ttu-id="2ac5b-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-106">Partner Center</span></span>
- <span data-ttu-id="2ac5b-107">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-107">Azure portal</span></span>
- <span data-ttu-id="2ac5b-108">Partner di CSP</span><span class="sxs-lookup"><span data-stu-id="2ac5b-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="2ac5b-109">Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente</span><span class="sxs-lookup"><span data-stu-id="2ac5b-109">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="2ac5b-110">Quando acquisti prenotazioni di Microsoft Azure per conto dei clienti, dovrai scegliere una macchina virtuale (VM) le cui dimensioni soddisfino le esigenze informatiche del cliente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-110">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="2ac5b-111">Puoi trovare queste informazioni scegliendo uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2ac5b-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="2ac5b-112">API di utilizzo Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-112">Azure utilization API</span></span>
- <span data-ttu-id="2ac5b-113">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-113">The Azure portal</span></span>
- <span data-ttu-id="2ac5b-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2ac5b-114">Azure PowerShell</span></span>
- <span data-ttu-id="2ac5b-115">L'API di Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="2ac5b-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="2ac5b-116">Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="2ac5b-117">Dopo aver acquistato una prenotazione, il relativo sconto verrà applicato automaticamente alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="2ac5b-118">Non è necessario assegnare la prenotazione a una macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-118">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="2ac5b-119">Gli sconti relativi alla prenotazione non vengono applicati alle macchine virtuali classiche o promozionali.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-119">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="2ac5b-120">Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, dovrai utilizzare uno dei metodi descritti di seguito poiché la serie della macchina virtuale non viene visualizzata correttamente nei file di riconciliazione del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="2ac5b-121">**Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API di utilizzo di Azure**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="2ac5b-122">Utilizza il valore dell'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="2ac5b-123">Per ulteriori informazioni, vedi [Ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell'[API del Centro per i partner](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="2ac5b-123">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="2ac5b-124">**Ottenere informazioni sul dimensionamento della macchina virtuale usando il portale di Microsoft Azure**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="2ac5b-125">Nel centro per i partner passare alla pagina Customers ( **clienti** ).</span><span class="sxs-lookup"><span data-stu-id="2ac5b-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="2ac5b-126">Trova il cliente che desidera acquistare prenotazioni della macchina virtuale di Azure, quindi seleziona la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="2ac5b-127">Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-127">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span>
3. <span data-ttu-id="2ac5b-128">Seleziona **Macchine virtuali** dal menu del portale, quindi seleziona la macchina virtuale per cui desideri acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="2ac5b-129">Nella pagina dei dettagli della macchina virtuale, trova informazioni in merito a dimensioni e area geografica, come illustrato di seguito, e usa queste informazioni per acquistare la prenotazione nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-129">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Informazioni sulle dimensioni e sull'area nella pagina Dettagli](images/usage1.png)

<span data-ttu-id="2ac5b-131">**Ottenere informazioni sul dimensionamento della macchina virtuale usando Microsoft Azure PowerShell**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="2ac5b-132">Per ottenere la posizione e le dimensioni della macchina virtuale per cui desideri acquistare una prenotazione, utilizza le informazioni nell'immagine seguente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Posizione e dimensioni della macchina virtuale](images/usage2.png)

<span data-ttu-id="2ac5b-134">**Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API Azure Resource Manager (ARM)**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="2ac5b-135">Tramite le API di ARMClient o ARM, chiama il client ARM per la macchina virtuale per cui desideri acquistare una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="2ac5b-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="2ac5b-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="2ac5b-137">La chiamata restituisce valori per **vmSize** e **location**, come illustrato di seguito.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="2ac5b-138">![valore percorso](images/usage3.png) valore ![vmSize](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="2ac5b-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span></span>

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="2ac5b-139">Verificare lo sconto su prenotazione e utilizzo della macchina virtuale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="2ac5b-140">Dopo l'acquisto di un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento anticipato dello spazio della macchina virtuale viene automaticamente applicato alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span>

<span data-ttu-id="2ac5b-141">Puoi verificare l'utilizzo della prenotazione del cliente e vedere le macchine virtuali a cui sono applicati gli sconti relativi alla prenotazione utilizzando uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2ac5b-141">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="2ac5b-142">Portale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-142">The Azure portal</span></span>
- <span data-ttu-id="2ac5b-143">API di utilizzo Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-143">Azure utilization API</span></span>

<span data-ttu-id="2ac5b-144">Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="2ac5b-145">Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="2ac5b-146">Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-146">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="2ac5b-147">Nel centro per i partner passare alla pagina Customers ( **clienti** ).</span><span class="sxs-lookup"><span data-stu-id="2ac5b-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="2ac5b-148">Trova il cliente di cui desideri verificare lo sconto e l'utilizzo della prenotazione, quindi seleziona la freccia giù per espandere le informazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="2ac5b-149">Seleziona **Portale di gestione di Microsoft Azure** per aprire il record del cliente nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-149">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span>
3. <span data-ttu-id="2ac5b-150">Seleziona **Prenotazioni** dal menu del portale, quindi seleziona la prenotazione di cui desideri verificare l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="2ac5b-151">Nella pagina **Panoramica** controlla il grafico sull'utilizzo della prenotazione, che mostra in che parte la prenotazione è stata applicata alle macchine virtuali.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-151">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2ac5b-152">I dati di utilizzo possono essere ritardati fino a 8 ore.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="2ac5b-153">a.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-153">a.</span></span> <span data-ttu-id="2ac5b-154">Se l'utilizzo della prenotazione è pari al 100%, il cliente ottiene tutto il risparmio che l'acquisto della prenotazione è in grado di offrire.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-154">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="2ac5b-155">b.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-155">b.</span></span> <span data-ttu-id="2ac5b-156">Se l'utilizzo della prenotazione è pari allo 0%, lo sconto non viene applicato a nessuna macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-156">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="2ac5b-157">c.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-157">c.</span></span> <span data-ttu-id="2ac5b-158">Se l'utilizzo della prenotazione è compreso tra 1% e 99%, esistono vantaggi inutilizzati.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-158">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="2ac5b-159">Per evitare questa situazione, scegli la macchina virtuale delle dimensioni corrette per supportare le esigenze di elaborazione del cliente prima di effettuare l'acquisto.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-159">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="2ac5b-160">Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-160">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="2ac5b-161">Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="2ac5b-162">Puoi ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente riceva lo sconto prenotazione e per vedere a quali macchine virtuali è applicato lo sconto.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="2ac5b-163">Confronta l'esempio A con l'esempio B per scoprire come verificare l'utilizzo della prenotazione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-163">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span>

![Esempi di utilizzo della prenotazione](images/usage5.png)

- <span data-ttu-id="2ac5b-165">reservationId identifica la prenotazione di Azure utilizzata per applicare lo sconto alla macchina virtuale.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="2ac5b-166">consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto della prenotazione.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="2ac5b-167">ReservationMeter mostra un costo di $ 0 perché è stato applicato lo sconto prenotazione.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="2ac5b-168">Per ulteriori informazioni, vedi [Ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell'[API del Centro per i partner](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="2ac5b-168">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="2ac5b-169">I costi relativi al software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="2ac5b-170">Tuttavia, se un cliente ha il Vantaggio Azure Hybrid Use, i costi del software non verranno applicati.</span><span class="sxs-lookup"><span data-stu-id="2ac5b-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="2ac5b-171">Per ulteriori informazioni, vedi [I costi del software Windows non sono inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="2ac5b-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="2ac5b-172">Risorse sulle prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-172">Azure reservations resources</span></span>

|<span data-ttu-id="2ac5b-173">**Per informazioni su**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-173">**For information about**</span></span>   |<span data-ttu-id="2ac5b-174">**Leggi questo**</span><span class="sxs-lookup"><span data-stu-id="2ac5b-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="2ac5b-175">Panoramica delle prenotazioni di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="2ac5b-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="2ac5b-176">Vendere Microsoft Azure istanze di VM riservate</span><span class="sxs-lookup"><span data-stu-id="2ac5b-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="2ac5b-177">Acquisto di prenotazioni di Azure per i clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="2ac5b-178">Acquista prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="2ac5b-179">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="2ac5b-180">Gestione delle prenotazioni di Azure nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2ac5b-181">Acquisto di prenotazioni di Azure nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="2ac5b-182">[Pagare in anticipo per macchine virtuali con istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="2ac5b-183">Gestione di prenotazioni di Azure nel portale di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="2ac5b-184">[Gestire le istanze di macchina virtuale riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure</span><span class="sxs-lookup"><span data-stu-id="2ac5b-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="2ac5b-185">Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2ac5b-186">[Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2ac5b-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
