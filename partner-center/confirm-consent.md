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
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333918"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="bcba8-104">Metodi aggiornati per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente</span><span class="sxs-lookup"><span data-stu-id="bcba8-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="bcba8-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="bcba8-105">**Applies to**</span></span>

-  <span data-ttu-id="bcba8-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="bcba8-106">Partner Center</span></span>

<span data-ttu-id="bcba8-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="bcba8-107">**Appropriate roles**</span></span>

- <span data-ttu-id="bcba8-108">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="bcba8-108">Admin agent</span></span>
- <span data-ttu-id="bcba8-109">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="bcba8-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="bcba8-110">La risorsa Contratto è attualmente supportata dal Centro per i partner solo nel cloud pubblico Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bcba8-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="bcba8-111">Non è applicabile a:</span><span class="sxs-lookup"><span data-stu-id="bcba8-111">It is not applicable to:</span></span>
> * <span data-ttu-id="bcba8-112">Centro per i partner gestito da 21Vianet</span><span class="sxs-lookup"><span data-stu-id="bcba8-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="bcba8-113">Centro per i partner per Microsoft Cloud Germania</span><span class="sxs-lookup"><span data-stu-id="bcba8-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="bcba8-114">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="bcba8-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="bcba8-115">A partire dal 31 gennaio 2020, tutti i clienti (sia nuovi che già esistenti) devono firmare il nuovo Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bcba8-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="bcba8-116">Per altre informazioni, vedi [Confermare l'accettazione del Contratto del cliente Microsoft da parte di un cliente](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="bcba8-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="bcba8-117">In qualità di partner, devi ottenere l'accettazione del Contratto del cliente Microsoft da parte di un cliente prima di poter ordinare prodotti e servizi Microsoft per tale cliente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="bcba8-118">Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto:</span><span class="sxs-lookup"><span data-stu-id="bcba8-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="bcba8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bcba8-119">First name</span></span>

- <span data-ttu-id="bcba8-120">Cognome</span><span class="sxs-lookup"><span data-stu-id="bcba8-120">Last name</span></span>

- <span data-ttu-id="bcba8-121">Indirizzo di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="bcba8-121">Email address</span></span>

- <span data-ttu-id="bcba8-122">Numero di telefono (facoltativo)</span><span class="sxs-lookup"><span data-stu-id="bcba8-122">Phone number (optional)</span></span>

- <span data-ttu-id="bcba8-123">Data di accettazione</span><span class="sxs-lookup"><span data-stu-id="bcba8-123">Date of acceptance</span></span>

<span data-ttu-id="bcba8-124">I partner con fatturazione diretta e i provider indiretti devono confermare che un cliente ha accettato il Contratto del cliente Microsoft durante l'esecuzione della transazione tramite il Centro per i partner o la relativa API.</span><span class="sxs-lookup"><span data-stu-id="bcba8-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="bcba8-125">La conferma è *obbligatoria* .</span><span class="sxs-lookup"><span data-stu-id="bcba8-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="bcba8-126">Se non viene fornita la conferma per un determinato cliente:</span><span class="sxs-lookup"><span data-stu-id="bcba8-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="bcba8-127">Non sarai in grado di creare nuovi ordini per il cliente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="bcba8-128">Non sarà possibile modificare il numero di licenze degli abbonamenti esistenti basati su licenze per il cliente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="bcba8-129">La conferma dell'accettazione da parte del cliente può essere eseguita tramite il Centro per i partner o la relativa API.</span><span class="sxs-lookup"><span data-stu-id="bcba8-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="bcba8-130">Per eseguire questa operazione tramite l'API del Centro per i partner, vedi i seguenti argomenti:</span><span class="sxs-lookup"><span data-stu-id="bcba8-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="bcba8-131">Ottenere la conferma del consenso del cliente</span><span class="sxs-lookup"><span data-stu-id="bcba8-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="bcba8-132">Ottenere i metadati del contratto</span><span class="sxs-lookup"><span data-stu-id="bcba8-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="bcba8-133">Confermare il consenso del cliente</span><span class="sxs-lookup"><span data-stu-id="bcba8-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="bcba8-134">Questo vale sia per gli ambienti di produzione che per quelli sandbox.</span><span class="sxs-lookup"><span data-stu-id="bcba8-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="bcba8-135">Confermare l'accettazione da parte di un nuovo cliente</span><span class="sxs-lookup"><span data-stu-id="bcba8-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="bcba8-136">Usa la procedura seguente per confermare l'accettazione da parte del cliente durante la creazione di un nuovo tenant cliente nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="bcba8-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="bcba8-137">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="bcba8-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="bcba8-138">Seleziona **Clienti** , quindi **Nuovo cliente** e infine **Info account** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="bcba8-139">Immetti le informazioni nei campi **Società** e **Contatto principale** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informazioni sulla società":::

3. <span data-ttu-id="bcba8-141">In **Microsoft customer agreement** (Contratto del cliente Microsoft) seleziona **The customer has accepted the latest Microsoft customer agreement** (Il cliente ha accettato il Contratto del cliente Microsoft più recente).</span><span class="sxs-lookup"><span data-stu-id="bcba8-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="bcba8-142">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="bcba8-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="bcba8-143">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="bcba8-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="bcba8-144">Immetti i dettagli dell'utente che ha fornito l'accettazione.</span><span class="sxs-lookup"><span data-stu-id="bcba8-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Aggiunta della data di accettazione":::

   <span data-ttu-id="bcba8-146">Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto principale.</span><span class="sxs-lookup"><span data-stu-id="bcba8-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="bcba8-147">Se queste informazioni non sono corrette, fai clic su **Aggiorna** , quindi riempi i campi **Nome** , **Cognome** , **Indirizzo e-mail** e \* *Numero di telefono* (facoltativo) della persona che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="bcba8-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="bcba8-148">Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="bcba8-149">Confermare l'accettazione da parte di un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="bcba8-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="bcba8-150">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="bcba8-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="bcba8-151">Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.</span><span class="sxs-lookup"><span data-stu-id="bcba8-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="bcba8-152">Seleziona **Informazioni sull'account** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-152">Select **Account info** .</span></span>

3. <span data-ttu-id="bcba8-153">In **Microsoft customer agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Aggiornamento":::

4. <span data-ttu-id="bcba8-155">Riempi i campi **Nome** , **Cognome** , **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="bcba8-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="bcba8-156">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="bcba8-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="bcba8-157">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="bcba8-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="bcba8-158">Fai clic su **Salva e continua** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="bcba8-159">Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="bcba8-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="bcba8-160">Se si tenta di creare un nuovo ordine per un cliente esistente non confermato prima, si riceverà la richiesta di completare la conferma.</span><span class="sxs-lookup"><span data-stu-id="bcba8-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="bcba8-161">Utilizzare la procedura seguente per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="bcba8-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="bcba8-162">Riempi i campi **Nome** , **Cognome** , **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="bcba8-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="bcba8-163">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="bcba8-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="bcba8-164">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="bcba8-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="bcba8-165">Fai clic su **Salva e continua** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="bcba8-166">Recuperare la conferma dell'accettazione da parte di un cliente esistente</span><span class="sxs-lookup"><span data-stu-id="bcba8-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="bcba8-167">Puoi recuperare la conferma dell'accettazione da parte di un cliente esistente che hai fornito in precedenza usando la procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="bcba8-168">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="bcba8-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="bcba8-169">Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.</span><span class="sxs-lookup"><span data-stu-id="bcba8-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="bcba8-170">Seleziona **Informazioni sull'account** .</span><span class="sxs-lookup"><span data-stu-id="bcba8-170">Select **Account info** .</span></span>

3. <span data-ttu-id="bcba8-171">In **Microsoft customer agreement** (Contratto del cliente Microsoft) potrai vedere se la conferma è stata fornita o meno per tale cliente.</span><span class="sxs-lookup"><span data-stu-id="bcba8-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bcba8-172">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="bcba8-172">Next steps</span></span>

- [<span data-ttu-id="bcba8-173">Conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente nel programma per i partner CSP</span><span class="sxs-lookup"><span data-stu-id="bcba8-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="bcba8-174">Attestare l'accettazione del Contratto del cliente Microsoft per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="bcba8-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)