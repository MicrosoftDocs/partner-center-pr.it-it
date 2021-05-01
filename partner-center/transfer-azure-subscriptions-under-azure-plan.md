---
title: Trasferire una sottoscrizione di Azure in un piano di Azure a un altro partner CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il Cloud Solution Provider partner del programma associato alle sottoscrizioni di Azure di un cliente in un piano di Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284503"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="4a2e6-103">Trasferire le sottoscrizioni del piano di Azure di un cliente a un partner diverso</span><span class="sxs-lookup"><span data-stu-id="4a2e6-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="4a2e6-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4a2e6-105">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="4a2e6-105">Account admin</span></span>
- <span data-ttu-id="4a2e6-106">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="4a2e6-106">Sales agent</span></span>
- <span data-ttu-id="4a2e6-107">Agente di fatturazione</span><span class="sxs-lookup"><span data-stu-id="4a2e6-107">Billing agent</span></span>

<span data-ttu-id="4a2e6-108">Questo articolo descrive come un cliente può cambiare le sottoscrizioni di Azure in un piano di Azure da un Cloud Solution Provider (CSP) a un altro.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="4a2e6-109">Per cambiare le sottoscrizioni di Azure di un cliente da un partner diverso, seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="4a2e6-110">Sia il partner che il cliente devono completare i passaggi.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="4a2e6-111">Solo i partner con una relazione di fatturazione diretta con Microsoft possono accedere agli strumenti di transizione.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="4a2e6-112">I rivenditori indiretti devono collaborare con i propri provider indiretti per sfruttare questo strumento di transizione.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="4a2e6-113">Il cliente deve essere in conversazione con entrambi i partner (attuale e futuro) prima di sfruttare questo strumento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="4a2e6-114">Una conversazione offline deve essere stata per evitare confusione e varianza.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="4a2e6-115">Inoltre, i partner e i clienti devono comprendere queste considerazioni e prerequisiti prima di avviare una transizione:</span><span class="sxs-lookup"><span data-stu-id="4a2e6-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="4a2e6-116">**Considerazioni principali:**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-116">**Key considerations:**</span></span>

- <span data-ttu-id="4a2e6-117">Le prenotazioni di Azure non verranno spostate con la sottoscrizione a un partner futuro</span><span class="sxs-lookup"><span data-stu-id="4a2e6-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="4a2e6-118">La transizione dei prezzi CSP per i servizi di Azure con il partner corrente non verrà</span><span class="sxs-lookup"><span data-stu-id="4a2e6-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="4a2e6-119">Le responsabilità di supporto per il cliente verranno spostate nel partner futuro</span><span class="sxs-lookup"><span data-stu-id="4a2e6-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="4a2e6-120">La fatturazione e la fatturazione verranno trasferite al partner futuro al momento del trasferimento</span><span class="sxs-lookup"><span data-stu-id="4a2e6-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="4a2e6-121">Il trasferimento Role-Based controllo degli accessi in base al ruolo di Azure non è interessato dal trasferimento</span><span class="sxs-lookup"><span data-stu-id="4a2e6-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="4a2e6-122">L'amministratore per conto di (AOBO) non verrà concesso per impostazione predefinita al partner futuro</span><span class="sxs-lookup"><span data-stu-id="4a2e6-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="4a2e6-123">I prodotti del marketplace di terze parti verranno trasferiti fino a quando i prodotti superano il controllo di idoneità al Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="4a2e6-124">Non sono presenti sconti speciali o restrizioni a livello di regione</span><span class="sxs-lookup"><span data-stu-id="4a2e6-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="4a2e6-125">I prodotti non sono basati su sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="4a2e6-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="4a2e6-126">Il partner futuro deve collaborare con l'editore per assicurarsi che siano nell'elenco elementi consentiti per la distribuzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="4a2e6-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="4a2e6-127">Se non tutte queste condizioni vengono soddisfatte per trasferire i prodotti del Marketplace, è necessario annullare le sottoscrizioni di Azure e quindi riacquisire i prodotti del Marketplace con il nuovo partner</span><span class="sxs-lookup"><span data-stu-id="4a2e6-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="4a2e6-128">**Prerequisiti:**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-128">**Prerequisites:**</span></span>

- <span data-ttu-id="4a2e6-129">Il cliente interagisce con il partner CSP corrente per la transizione</span><span class="sxs-lookup"><span data-stu-id="4a2e6-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="4a2e6-130">Il futuro partner CSP collabora con il cliente per garantire che le esigenze dei clienti possano essere soddisfatte</span><span class="sxs-lookup"><span data-stu-id="4a2e6-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="4a2e6-131">Il futuro partner CSP stabilisce una relazione con il cliente e acquista un piano di Azure prima dell'inizio della transizione</span><span class="sxs-lookup"><span data-stu-id="4a2e6-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="4a2e6-132">Il cliente deve firmare Contratto del cliente Microsoft partner CSP futuro</span><span class="sxs-lookup"><span data-stu-id="4a2e6-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="4a2e6-133">Il partner CSP futuro deve aver firmato il Contratto Microsoft Partner per usare questo strumento</span><span class="sxs-lookup"><span data-stu-id="4a2e6-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="4a2e6-134">Attività del cliente da completare</span><span class="sxs-lookup"><span data-stu-id="4a2e6-134">Customer tasks to be completed</span></span>

<span data-ttu-id="4a2e6-135">Per trasferire una sottoscrizione di Azure in un piano di Azure, il cliente deve avviare il processo contattando il partner corrente.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="4a2e6-136">Devono raccogliere il nome della società e il dominio del partner corrente in modo che il partner futuro possa completare il modulo di richiesta di trasferimento per loro conto.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="4a2e6-137">Il cliente deve anche identificare le sottoscrizioni da trasferire dal partner corrente.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="4a2e6-138">Non è possibile modificare i partner per le sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="4a2e6-139">È responsabilità del partner futuro completare il modulo di richiesta di trasferimento che avvia il processo di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="4a2e6-140">Microsoft non può intervenire per conto del cliente o del partner corrente.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="4a2e6-141">Il cliente deve pianificare di collaborare a stretto contatto con il partner futuro e attuale per rendere la transizione senza problemi.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="4a2e6-142">Attività future dei partner da completare</span><span class="sxs-lookup"><span data-stu-id="4a2e6-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="4a2e6-143">Il partner futuro della sottoscrizione deve completare un modulo di richiesta di trasferimento Partner Center per richiedere un trasferimento di sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="4a2e6-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="4a2e6-144">Dal menu Partner Center selezionare **Clienti,** quindi selezionare il cliente per cui si vuole completare un modulo di richiesta di trasferimento per conto di .</span><span class="sxs-lookup"><span data-stu-id="4a2e6-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="4a2e6-145">Scegliere Sottoscrizioni dal menu **Cliente.**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4a2e6-146">Selezionare la **sezione Richiesta di** trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4a2e6-147">Nella sezione **Richiesta di trasferimento** selezionare Aggiungi nuova **richiesta.**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sezione Trasferimenti":::

5.  <span data-ttu-id="4a2e6-149">Completare il **modulo Nuova richiesta di** trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="4a2e6-150">Selezionare Send transfer request Send **(Invia richiesta di**  >  **trasferimento) Send (Invia).**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Modulo di richiesta di trasferimento completo":::

7.  <span data-ttu-id="4a2e6-152">Verificare la conferma della richiesta di trasferimento</span><span class="sxs-lookup"><span data-stu-id="4a2e6-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Verifica trasferimento in sospeso":::

    >[!Note]
    ><span data-ttu-id="4a2e6-154">Il partner futuro può annullare la richiesta di trasferimento selezionando **Annulla** richiesta nell'angolo superiore destro solo quando lo stato della richiesta di trasferimento è "in sospeso".</span><span class="sxs-lookup"><span data-stu-id="4a2e6-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="4a2e6-155">Quando lo stato della richiesta di trasferimento è "in corso" o "completato", gli annullamenti non saranno possibili.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="4a2e6-156">Attività partner correnti da completare</span><span class="sxs-lookup"><span data-stu-id="4a2e6-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="4a2e6-157">L'agente amministratore del partner corrente del cliente riceverà un messaggio di posta elettronica che indica che il cliente richiede un trasferimento delle sottoscrizioni:</span><span class="sxs-lookup"><span data-stu-id="4a2e6-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisione":::

<span data-ttu-id="4a2e6-159">Esaminare e accettare il modulo di richiesta di trasferimento Partner Center per completare il trasferimento della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="4a2e6-160">Se il partner corrente non ha intrapreso alcuna azione entro 30 giorni, la richiesta scadrà e il partner futuro avrà un oggetto per creare una nuova richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="4a2e6-161">Selezionare **Rivedi richiesta di trasferimento** dal messaggio di posta elettronica OPPURE</span><span class="sxs-lookup"><span data-stu-id="4a2e6-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="4a2e6-162">Nel menu Partner Center clienti selezionare **Clienti** e quindi selezionare il cliente di cui è stata inviata una richiesta di trasferimento per conto di .</span><span class="sxs-lookup"><span data-stu-id="4a2e6-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="4a2e6-163">Scegliere Sottoscrizioni dal menu **Cliente.**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="4a2e6-164">Selezionare la **sezione Richiesta di** trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="4a2e6-165">Espandere le informazioni di trasferimento selezionando **l'ID richiesta di trasferimento selezionato** in Richieste **ricevute**</span><span class="sxs-lookup"><span data-stu-id="4a2e6-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Richiesta di trasferimento delle verifiche di origine":::

5.  <span data-ttu-id="4a2e6-167">Esaminare la richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-167">Review transfer request.</span></span> <span data-ttu-id="4a2e6-168">Selezionare le sottoscrizioni di Azure richieste da trasferire.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="4a2e6-169">Prima di procedere, tenere presente che non si avrà più accesso alle sottoscrizioni selezionate.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="4a2e6-170">Non verrà fatturata l'ulteriore utilizzo.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="4a2e6-171">Le prenotazioni di Azure non vengono trasferite con le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="4a2e6-172">Selezionare quindi **Accetta e trasferisci** per completare il processo di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selezionare le sottoscrizioni da trasferire nei piani di Azure":::

7.  <span data-ttu-id="4a2e6-174">Visualizzare la conferma di accettazione del trasferimento.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="4a2e6-175">A questo punto, il partner futuro, il cliente e il partner corrente riceveranno una notifica della richiesta di trasferimento accettata tramite posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="4a2e6-176">Dopo, la transizione è stata accettata, lo stato del trasferimento potrebbe rimanere In sospeso per un massimo di 15 minuti durante l'aggiornamento del sistema.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="4a2e6-177">Se l'operazione richiede più tempo, il sistema continuerà a provare per tre giorni.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="4a2e6-178">Se lo stato del trasferimento rimane ancora In sospeso, il partner deve inviare una richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="4a2e6-179">Al termine del trasferimento, le sottoscrizioni incluse nella richiesta verranno visualizzate nel piano di Azure del partner futuro e non verranno più elencate con l'utente.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="4a2e6-180">Per i provider indiretti: informare il rivenditore indiretto che la richiesta di trasferimento è stata accettata.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="4a2e6-181">Gestione delle sottoscrizioni dei clienti trasferite</span><span class="sxs-lookup"><span data-stu-id="4a2e6-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="4a2e6-182">La transizione non influisce sull'accesso per utenti, gruppi o entità servizio esistenti assegnati con il controllo degli accessi in base al ruolo di Azure.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="4a2e6-183">Il controllo degli accessi in base al ruolo di [Azure](/azure/role-based-access-control/overview) consente al cliente di gestire chi può accedere alle risorse di Azure, cosa può fare con tali risorse e a quali aree può accedere.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="4a2e6-184">Come nuovo partner non si ha accesso al controllo degli accessi in base al ruolo alle risorse del cliente dopo il trasferimento della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="4a2e6-185">Il partner precedente del cliente mantiene l'accesso RBAC.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="4a2e6-186">Collaborare con il cliente per comprendere chi ha informazioni dettagliate sulle sottoscrizioni e come apportare le modifiche desiderate.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="4a2e6-187">Di conseguenza, è importante che il cliente rimova l'accesso al controllo degli accessi in base al ruolo di Azure per il partner precedente e aggiunge l'accesso per il nuovo partner.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="4a2e6-188">Per altre informazioni sul nuovo accesso del cliente, vedere Che cos'è il controllo degli accessi in base [al ruolo di Azure?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="4a2e6-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="4a2e6-189">Per altre informazioni sulla rimozione dell'accesso RBAC del partner precedente da parte del cliente, vedere [Rimuovere un'assegnazione di ruolo.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="4a2e6-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="4a2e6-190">Inoltre, non si ottiene automaticamente l'accesso [admin on behalf of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) alle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="4a2e6-191">AOBO è necessario per i partner per gestire le sottoscrizioni di Azure del cliente per loro conto.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="4a2e6-192">Per altre informazioni sui privilegi di Azure, vedere [Ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="4a2e6-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="4a2e6-193">Passaggi successivi:</span><span class="sxs-lookup"><span data-stu-id="4a2e6-193">Next steps:</span></span>

- [<span data-ttu-id="4a2e6-194">(Controllo degli accessi in base al ruolo di Azure)</span><span class="sxs-lookup"><span data-stu-id="4a2e6-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="4a2e6-195">Ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="4a2e6-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
