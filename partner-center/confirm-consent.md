---
title: Confermare l'accettazione del Contratto del cliente Microsoft da parte di un cliente
description: Scopri come confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Questa operazione potrebbe essere necessaria per ordinare prodotti e servizi Microsoft per i clienti.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354611"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="5ab52-104">Metodi aggiornati per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente</span><span class="sxs-lookup"><span data-stu-id="5ab52-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="5ab52-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="5ab52-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5ab52-106">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="5ab52-106">Admin agent</span></span>
- <span data-ttu-id="5ab52-107">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="5ab52-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="5ab52-108">La risorsa Contratto è attualmente supportata dal Centro per i partner solo nel cloud pubblico Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5ab52-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="5ab52-109">Non è applicabile a:</span><span class="sxs-lookup"><span data-stu-id="5ab52-109">It is not applicable to:</span></span>
> * <span data-ttu-id="5ab52-110">Centro per i partner gestito da 21Vianet</span><span class="sxs-lookup"><span data-stu-id="5ab52-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="5ab52-111">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="5ab52-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="5ab52-112">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="5ab52-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="5ab52-113">A partire dal 31 gennaio 2020, tutti i clienti (sia nuovi che già esistenti) devono firmare il nuovo Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5ab52-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="5ab52-114">Per altre informazioni, vedi [Confermare l'accettazione del Contratto del cliente Microsoft da parte di un cliente](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="5ab52-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="5ab52-115">In qualità di partner, devi ottenere l'accettazione del Contratto del cliente Microsoft da parte di un cliente prima di poter ordinare prodotti e servizi Microsoft per tale cliente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="5ab52-116">Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto:</span><span class="sxs-lookup"><span data-stu-id="5ab52-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="5ab52-117">Nome</span><span class="sxs-lookup"><span data-stu-id="5ab52-117">First name</span></span>

- <span data-ttu-id="5ab52-118">Cognome</span><span class="sxs-lookup"><span data-stu-id="5ab52-118">Last name</span></span>

- <span data-ttu-id="5ab52-119">Indirizzo di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="5ab52-119">Email address</span></span>

- <span data-ttu-id="5ab52-120">Numero di telefono (facoltativo)</span><span class="sxs-lookup"><span data-stu-id="5ab52-120">Phone number (optional)</span></span>

- <span data-ttu-id="5ab52-121">Data di accettazione</span><span class="sxs-lookup"><span data-stu-id="5ab52-121">Date of acceptance</span></span>

<span data-ttu-id="5ab52-122">I partner con fatturazione diretta e i provider indiretti devono confermare che un cliente ha accettato il Contratto del cliente Microsoft durante l'esecuzione della transazione tramite il Centro per i partner o la relativa API.</span><span class="sxs-lookup"><span data-stu-id="5ab52-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="5ab52-123">La conferma è *obbligatoria*.</span><span class="sxs-lookup"><span data-stu-id="5ab52-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="5ab52-124">Se non viene fornita la conferma per un determinato cliente:</span><span class="sxs-lookup"><span data-stu-id="5ab52-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="5ab52-125">Non sarai in grado di creare nuovi ordini per il cliente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="5ab52-126">Non sarà possibile modificare il numero di licenze degli abbonamenti esistenti basati su licenze per il cliente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="5ab52-127">La conferma dell'accettazione da parte del cliente può essere eseguita tramite il Centro per i partner o la relativa API.</span><span class="sxs-lookup"><span data-stu-id="5ab52-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="5ab52-128">Per eseguire questa operazione tramite l'API del Centro per i partner, vedi i seguenti argomenti:</span><span class="sxs-lookup"><span data-stu-id="5ab52-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="5ab52-129">Ottenere la conferma del consenso del cliente</span><span class="sxs-lookup"><span data-stu-id="5ab52-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="5ab52-130">Ottenere i metadati del contratto</span><span class="sxs-lookup"><span data-stu-id="5ab52-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="5ab52-131">Confermare il consenso del cliente</span><span class="sxs-lookup"><span data-stu-id="5ab52-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="5ab52-132">Questo vale sia per gli ambienti di produzione che per quelli sandbox.</span><span class="sxs-lookup"><span data-stu-id="5ab52-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="5ab52-133">Confermare l'accettazione da parte di un nuovo cliente</span><span class="sxs-lookup"><span data-stu-id="5ab52-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="5ab52-134">Usa la procedura seguente per confermare l'accettazione da parte del cliente durante la creazione di un nuovo tenant cliente nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="5ab52-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="5ab52-135">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="5ab52-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ab52-136">Seleziona **Clienti**, quindi **Nuovo cliente** e infine **Info account**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="5ab52-137">Immetti le informazioni nei campi **Società** e **Contatto principale**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informazioni sulla società":::

3. <span data-ttu-id="5ab52-139">In **Microsoft customer agreement** (Contratto del cliente Microsoft) seleziona **The customer has accepted the latest Microsoft customer agreement** (Il cliente ha accettato il Contratto del cliente Microsoft più recente).</span><span class="sxs-lookup"><span data-stu-id="5ab52-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="5ab52-140">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="5ab52-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ab52-141">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="5ab52-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5ab52-142">Immetti i dettagli dell'utente che ha fornito l'accettazione.</span><span class="sxs-lookup"><span data-stu-id="5ab52-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Aggiunta della data di accettazione":::

   <span data-ttu-id="5ab52-144">Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto principale.</span><span class="sxs-lookup"><span data-stu-id="5ab52-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="5ab52-145">Se queste informazioni non sono corrette, fai clic su **Aggiorna**, quindi riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e \**Numero di telefono* (facoltativo) della persona che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="5ab52-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="5ab52-146">Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="5ab52-147">Confermare l'accettazione da parte di un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="5ab52-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="5ab52-148">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="5ab52-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ab52-149">Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.</span><span class="sxs-lookup"><span data-stu-id="5ab52-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5ab52-150">Seleziona **Informazioni sull'account**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-150">Select **Account info**.</span></span>

3. <span data-ttu-id="5ab52-151">In **Microsoft customer agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Aggiornamento":::

4. <span data-ttu-id="5ab52-153">Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="5ab52-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="5ab52-154">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="5ab52-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ab52-155">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="5ab52-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="5ab52-156">Fai clic su **Salva e continua**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="5ab52-157">Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="5ab52-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="5ab52-158">Se si tenta di creare un nuovo ordine per un cliente esistente non confermato prima, si riceverà la richiesta di completare la conferma.</span><span class="sxs-lookup"><span data-stu-id="5ab52-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="5ab52-159">Utilizzare la procedura seguente per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="5ab52-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="5ab52-160">Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="5ab52-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="5ab52-161">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="5ab52-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5ab52-162">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="5ab52-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="5ab52-163">Fai clic su **Salva e continua**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="5ab52-164">Recuperare la conferma dell'accettazione da parte di un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="5ab52-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="5ab52-165">Puoi recuperare la conferma dell'accettazione da parte di un cliente esistente che hai fornito in precedenza usando la procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="5ab52-166">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="5ab52-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5ab52-167">Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.</span><span class="sxs-lookup"><span data-stu-id="5ab52-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5ab52-168">Seleziona **Informazioni sull'account**.</span><span class="sxs-lookup"><span data-stu-id="5ab52-168">Select **Account info**.</span></span>

3. <span data-ttu-id="5ab52-169">In **Microsoft customer agreement** (Contratto del cliente Microsoft) potrai vedere se la conferma è stata fornita o meno per tale cliente.</span><span class="sxs-lookup"><span data-stu-id="5ab52-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5ab52-170">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="5ab52-170">Next steps</span></span>

- [<span data-ttu-id="5ab52-171">Conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente nel programma per i partner CSP</span><span class="sxs-lookup"><span data-stu-id="5ab52-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="5ab52-172">Attestare l'accettazione del Contratto del cliente Microsoft per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="5ab52-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)