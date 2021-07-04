---
title: Come verificare che il cliente abbia accettato l'Contratto del cliente Microsoft al programma CSP
description: I partner Cloud Solution Provider (CSP) devono confermare l'accettazione del Contratto del cliente Microsoft prima di ordinare i servizi Microsoft per i clienti.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277012"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="c78cd-103">Come verificare che il cliente abbia accettato l'Contratto del cliente Microsoft al programma CSP</span><span class="sxs-lookup"><span data-stu-id="c78cd-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="c78cd-104">**Ruoli appropriati:** agente di amministrazione | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c78cd-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="c78cd-105">I clienti hanno due opzioni per il modo in cui accettano il Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="c78cd-106">**Opzione 1**: attestazione del partner dell'accettazione da parte di un cliente. Il partner può confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner o tramite il dashboard Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c78cd-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="c78cd-107">**Opzione 2**: accettazione diretta del cliente. Il partner può invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="c78cd-108">Accedere al modello del contratto del cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="c78cd-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="c78cd-109">Puoi scaricare manualmente la versione più recente del modello di contratto del cliente Microsoft [qui](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="c78cd-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="c78cd-110">Il Contratto del cliente Microsoft è specifico del paese.</span><span class="sxs-lookup"><span data-stu-id="c78cd-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="c78cd-111">Quando richiedi il modello del contratto del cliente Microsoft, assicurati di selezionare il paese corretto in base alla località in cui si trova il cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="c78cd-112">Opzione 1: Confermare l'accettazione da parte di un cliente nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="c78cd-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="c78cd-113">I partner con fatturazione diretta possono confermare l'accettazione del Contratto del cliente Microsoft in Partner Center per i clienti nuovi ed esistenti.</span><span class="sxs-lookup"><span data-stu-id="c78cd-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="c78cd-114">I rivenditori indiretti non possono eseguire l'attestazione per conto dei clienti e devono collaborare con il provider indiretto per completare l'attestazione.</span><span class="sxs-lookup"><span data-stu-id="c78cd-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="c78cd-115">Confermare l'accettazione per i nuovi clienti</span><span class="sxs-lookup"><span data-stu-id="c78cd-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="c78cd-116">Quando si crea il tenant di un nuovo cliente in Centro per i partner, segui questa procedura per confermare l'accettazione del contratto del cliente Microsoft da parte del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="c78cd-117">Devi essere un agente amministratore o di vendita per eseguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="c78cd-118">Seleziona **Clienti** e quindi **Nuovo cliente**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="c78cd-119">In **Informazioni sull'account** immetti le informazioni relative alla società e al contatto principale.</span><span class="sxs-lookup"><span data-stu-id="c78cd-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="c78cd-120">In **Microsoft agreement** (Contratto Microsoft) seleziona la casella per attestare che il cliente ha accettato il contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="c78cd-121">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="c78cd-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c78cd-122">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="c78cd-123">Verifica che le informazioni di contatto dell'utente principale visualizzate siano corrette.</span><span class="sxs-lookup"><span data-stu-id="c78cd-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="c78cd-124">Se non è corretto, selezionare **Aggiorna** e immettere le informazioni accurate per la persona che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="c78cd-125">Selezionare **Avanti** per continuare a creare il tenant del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nuovo cliente.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="c78cd-127">Confermare l'accettazione del cliente per i clienti esistenti</span><span class="sxs-lookup"><span data-stu-id="c78cd-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="c78cd-128">Devi essere un agente amministratore o di vendita per eseguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="c78cd-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="c78cd-129">Seleziona **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-129">Select **Customers**.</span></span> <span data-ttu-id="c78cd-130">Individua e seleziona il cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-130">Find and select the customer.</span></span>

2. <span data-ttu-id="c78cd-131">Seleziona **Informazioni sull'account**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-131">Select **Account info**.</span></span>

3. <span data-ttu-id="c78cd-132">In **Microsoft Customer Agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="c78cd-133">Completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="c78cd-134">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="c78cd-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c78cd-135">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="c78cd-136">Scegli **Salva** e continua.</span><span class="sxs-lookup"><span data-stu-id="c78cd-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente esistente.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="c78cd-138">Recuperare la conferma dell'accettazione del cliente</span><span class="sxs-lookup"><span data-stu-id="c78cd-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="c78cd-139">Per recuperare la conferma che un cliente esistente ha accettato il Contratto del cliente Microsoft, seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="c78cd-140">Devi essere un agente amministratore o di vendita per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="c78cd-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="c78cd-141">Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.</span><span class="sxs-lookup"><span data-stu-id="c78cd-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="c78cd-142">Seleziona **Informazioni sull'account**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-142">Select **Account info**.</span></span>

3. <span data-ttu-id="c78cd-143">In **Microsoft customer agreement** (Contratto del cliente Microsoft) visualizza se il cliente ha fornito o meno la conferma.</span><span class="sxs-lookup"><span data-stu-id="c78cd-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="c78cd-144">Confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="c78cd-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="c78cd-145">Puoi usare l'API/SDK del Centro per i partner per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="c78cd-146">Per informazioni dettagliate su API/SDK, vedere:</span><span class="sxs-lookup"><span data-stu-id="c78cd-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="c78cd-147">Ottenere i metadati per il contratto del cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="c78cd-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="c78cd-148">Confermare l'accettazione del contratto del cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="c78cd-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="c78cd-149">Ottenere la conferma dell'accettazione del Contratto del cliente Microsoft da parte di un cliente</span><span class="sxs-lookup"><span data-stu-id="c78cd-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="c78cd-150">Ottenere un collegamento per il download del modello di contratto del cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="c78cd-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="c78cd-151">Opzione 2: Accettazione da parte del cliente nell'interfaccia di amministrazione di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c78cd-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="c78cd-152">I partner possono invitare tramite un URL clienti nuovi ed esistenti a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="c78cd-153">Nelle prossime sezioni verrà illustrato come effettuare le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c78cd-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="c78cd-154">Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="c78cd-155">Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="c78cd-156">Invitare un cliente esistente a esaminare e accettare il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="c78cd-157">Per ottenere lo stato dell'accettazione diretta del Contratto del cliente Microsoft da parte di un cliente, puoi usare l'[API/SDK del Centro per i partner](/partner-center/develop/get-direct-sign-status-of-customer-agreement).</span><span class="sxs-lookup"><span data-stu-id="c78cd-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="c78cd-158">Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto</span><span class="sxs-lookup"><span data-stu-id="c78cd-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="c78cd-159">Segui questa procedura per creare un nuovo cliente nel Centro per i partner e quindi invitarlo a esaminare e accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="c78cd-160">Dalla scheda **Clienti** nel Centro per i partner seleziona **Add customer** (Aggiungi cliente).</span><span class="sxs-lookup"><span data-stu-id="c78cd-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="c78cd-161">In **Informazioni sull'account** immetti le informazioni sul nuovo cliente in tutti i campi obbligatori, inclusi il nome della società e il contatto principale del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="c78cd-162">In **Contratto del** cliente selezionare Customer will be asked to accept the Contratto del cliente Microsoft in Amministrazione Microsoft 365 **Center**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="c78cd-163">Completa gli altri campi obbligatori nella pagina.</span><span class="sxs-lookup"><span data-stu-id="c78cd-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="c78cd-164">Seleziona **Successivo: Rivedi** e quindi continua la procedura per creare il tenant del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="c78cd-165">I nuovi clienti non possono effettuare un acquisto fino a quando non accettano il Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Creare un nuovo cliente.":::

5. <span data-ttu-id="c78cd-167">Quando raggiungi la schermata **Conferma** nel flusso di lavoro per il nuovo cliente, salva le credenziali del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="c78cd-168">Dovrai fornire queste credenziali al cliente in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="c78cd-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="c78cd-169">All'esterno del Centro per i partner crea e invia un'e-mail per invitare il cliente ad accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="c78cd-170">Assicurati di includere questi elementi nell'e-mail:</span><span class="sxs-lookup"><span data-stu-id="c78cd-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="c78cd-171">Collegamento a questo [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (sono necessarie le informazioni di accesso)</span><span class="sxs-lookup"><span data-stu-id="c78cd-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="c78cd-172">Le credenziali del cliente salvate nel passaggio 5.</span><span class="sxs-lookup"><span data-stu-id="c78cd-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="c78cd-173">Il cliente riceverà quindi l'invito tramite e-mail dal partner e selezionerà l'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="c78cd-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="c78cd-174">Il cliente accede Amministrazione Microsoft 365 Center usando le credenziali del cliente specificate.</span><span class="sxs-lookup"><span data-stu-id="c78cd-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="c78cd-175">Il cliente controlla la casella per accettare il Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="c78cd-176">Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft</span><span class="sxs-lookup"><span data-stu-id="c78cd-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="c78cd-177">Segui questa procedura per invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="c78cd-178">Dalla scheda **Clienti** nell'ambito del Centro per i partner seleziona il collegamento **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="c78cd-179">Verrà generato un modello di e-mail automatico contenente il testo e un URL con parametri in grado di indirizzare il cliente all'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="c78cd-180">Puoi personalizzare il modello di e-mail generato automaticamente e quindi selezionare **Copia negli Appunti** o **Apri nell'email**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="c78cd-181">Usa questo modello di e-mail per invitare il cliente ad accettare la richiesta di **relazione come rivenditore** e il **contratto del cliente Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="c78cd-182">Nota: nell'invito tramite e-mail assicurati che il partner includa anche l'URL fornito automaticamente e le credenziali del cliente create di recente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="creare una relazione.":::

5. <span data-ttu-id="c78cd-184">Il cliente riceve l'invito tramite e-mail e fa clic sull'URL con parametri.</span><span class="sxs-lookup"><span data-stu-id="c78cd-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="c78cd-185">Il cliente usa le credenziali specificate all'interno della posta elettronica per accedere Amministrazione Microsoft 365 Center.</span><span class="sxs-lookup"><span data-stu-id="c78cd-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="c78cd-186">Il cliente seleziona la casella per accettare la **relazione come rivenditore** e il **contratto cliente Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="c78cd-187">Nello stesso URL il cliente è in grado di visualizzare un elenco consolidato di partner diversi con cui lavora</span><span class="sxs-lookup"><span data-stu-id="c78cd-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="c78cd-188">e può selezionare un partner per visualizzare i dettagli.</span><span class="sxs-lookup"><span data-stu-id="c78cd-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Accettare il contratto.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="c78cd-190">Invitare un cliente esistente a esaminare e accettare il contratto</span><span class="sxs-lookup"><span data-stu-id="c78cd-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="c78cd-191">Segui questa procedura per invitare un cliente esistente a esaminare e accettare il contratto cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="c78cd-192">Crea l'e-mail del cliente con l'URL incorporato per invitare il cliente ad accettare il contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="c78cd-193">Il cliente riceve l'invito tramite posta elettronica e fa clic sull'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="c78cd-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="c78cd-194">Il cliente immette le proprie credenziali nell'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c78cd-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="c78cd-195">Il cliente seleziona la casella per accettare il contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="c78cd-196">Nello stesso URL il cliente è in grado di visualizzare l'elenco consolidato di partner diversi con cui lavora</span><span class="sxs-lookup"><span data-stu-id="c78cd-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="c78cd-197">e può selezionare un partner per visualizzare i dettagli.</span><span class="sxs-lookup"><span data-stu-id="c78cd-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente.":::

>[!NOTE]
><span data-ttu-id="c78cd-199">In alcuni scenari i clienti potrebbero non essere in grado di accettare direttamente il contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="c78cd-200">Per altre informazioni su queste situazioni, vedere Due scenari in cui è necessario attestare per conto del cliente, di seguito.</span><span class="sxs-lookup"><span data-stu-id="c78cd-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="c78cd-201">Due scenari in cui è necessaria l'attestazione per conto del cliente</span><span class="sxs-lookup"><span data-stu-id="c78cd-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="c78cd-202">Esistono due scenari in cui i clienti potrebbero non essere in grado di accettare direttamente il Contratto del cliente Microsoft all'interno Amministrazione Microsoft 365 Center.</span><span class="sxs-lookup"><span data-stu-id="c78cd-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="c78cd-203">**Scenario 1:** un cliente esistente ha acquistato uno degli elementi seguenti tramite una relazione partner esistente: offerte, sottoscrizioni software o software, istanze riservate o piano di Azure.</span><span class="sxs-lookup"><span data-stu-id="c78cd-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="c78cd-204">Il cliente tenta ora di effettuare un nuovo acquisto (escluso il rinnovo automatico).</span><span class="sxs-lookup"><span data-stu-id="c78cd-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="c78cd-205">Quando il cliente seleziona l'URL, riceve un messaggio che indica di rivolgersi al partner per confermare l'accettazione del Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="c78cd-206">**Per risolvere il problema**: devi attestare l'accettazione per conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot della pagina dell'interfaccia di amministrazione di Microsoft 365 che chiede di contattare il proprio partner per confermare l'accettazione del Contratto del cliente Microsoft.":::

<span data-ttu-id="c78cd-208">**Scenario 2**: un cliente esistente ha acquistato una delle opzioni seguenti: offerta, software o abbonamento software, istanza riservata o piano di Azure.</span><span class="sxs-lookup"><span data-stu-id="c78cd-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="c78cd-209">Il cliente tenta ora di effettuare un nuovo acquisto con un nuovo partner.</span><span class="sxs-lookup"><span data-stu-id="c78cd-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="c78cd-210">Quando il cliente seleziona l'URL dell'interfaccia di amministrazione di Microsoft 365 per accettare la relazione con il nuovo partner e il contratto, riceve un messaggio che indica di rivolgersi al partner per confermare l'accettazione del Contratto del cliente Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c78cd-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="c78cd-211">**Per risolvere il problema**: devi attestare l'accettazione per conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="c78cd-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="c78cd-212">Verificare che un cliente abbia accettato il contratto</span><span class="sxs-lookup"><span data-stu-id="c78cd-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="c78cd-213">Se si tenta di creare un nuovo ordine per un cliente esistente non confermato prima, si riceverà la richiesta di completare la conferma.</span><span class="sxs-lookup"><span data-stu-id="c78cd-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="c78cd-214">Utilizzare la procedura seguente per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="c78cd-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="c78cd-215">Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.</span><span class="sxs-lookup"><span data-stu-id="c78cd-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="c78cd-216">In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata.</span><span class="sxs-lookup"><span data-stu-id="c78cd-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="c78cd-217">Non puoi impostare questo campo su una data futura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="c78cd-218">Fai clic su **Salva e continua**.</span><span class="sxs-lookup"><span data-stu-id="c78cd-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c78cd-219">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c78cd-219">Next steps</span></span>

- [<span data-ttu-id="c78cd-220">Verificare o aggiornare le informazioni del profilo aziendale</span><span class="sxs-lookup"><span data-stu-id="c78cd-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="c78cd-221">Contratti del cliente Microsoft (per area geografica e lingua)</span><span class="sxs-lookup"><span data-stu-id="c78cd-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
