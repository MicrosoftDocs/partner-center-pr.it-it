---
title: Trasferire la sottoscrizione di Azure in un piano di Azure a un altro partner CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il partner del programma Cloud Solution provider associato alle sottoscrizioni di Azure di un cliente in un piano di Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980262"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="3b1dc-103">Trasferire le sottoscrizioni di piano di Azure di un cliente a un partner diverso</span><span class="sxs-lookup"><span data-stu-id="3b1dc-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

## <a name="applies-to"></a><span data-ttu-id="3b1dc-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="3b1dc-104">Applies to</span></span>

- <span data-ttu-id="3b1dc-105">Partner inclusi nel programma Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="3b1dc-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="3b1dc-106">Questo articolo descrive come un cliente può cambiare le sottoscrizioni di Azure in un piano di Azure da un provider di soluzioni cloud (CSP) a un altro.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="3b1dc-107">Per cambiare le sottoscrizioni di Azure di un cliente da un partner diverso, seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="3b1dc-108">Sia il partner che il cliente devono eseguire i passaggi necessari.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="3b1dc-109">Solo i partner con una relazione di fatturazione diretta con Microsoft possono accedere agli strumenti di transizione.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="3b1dc-110">I rivenditori indiretti devono collaborare con i provider indiretti per sfruttare questo strumento di transizione.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="3b1dc-111">Il cliente deve essere in conversazione con entrambi i partner (attuali e futuri) prima che questo strumento venga usato.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="3b1dc-112">È necessario che una conversazione offline eviti confusione e varianza.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="3b1dc-113">Inoltre, i partner e i clienti devono comprendere queste considerazioni e i prerequisiti prima di avviare una transizione:</span><span class="sxs-lookup"><span data-stu-id="3b1dc-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="3b1dc-114">**Considerazioni principali:**</span><span class="sxs-lookup"><span data-stu-id="3b1dc-114">**Key considerations:**</span></span>

- <span data-ttu-id="3b1dc-115">Le prenotazioni di Azure non vengono spostate con la sottoscrizione a partner futuri</span><span class="sxs-lookup"><span data-stu-id="3b1dc-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="3b1dc-116">I prezzi di CSP per i servizi di Azure in Current partner non vengono sottoposti a transizione</span><span class="sxs-lookup"><span data-stu-id="3b1dc-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="3b1dc-117">Le responsabilità del supporto per i clienti passeranno al partner futuro</span><span class="sxs-lookup"><span data-stu-id="3b1dc-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="3b1dc-118">La fatturazione e la fatturazione passeranno a partner futuri al momento del trasferimento</span><span class="sxs-lookup"><span data-stu-id="3b1dc-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="3b1dc-119">Il servizio di controllo di accesso (RBAC) di Azure Role-Based non è influenzato dal trasferimento</span><span class="sxs-lookup"><span data-stu-id="3b1dc-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="3b1dc-120">Per impostazione predefinita, l'amministratore per conto di (AOBO) non verrà concesso al partner futuro</span><span class="sxs-lookup"><span data-stu-id="3b1dc-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="3b1dc-121">I prodotti del Marketplace di terze parti vengono trasferiti fino a quando i prodotti passano il controllo di idoneità del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="3b1dc-122">Non sono previsti sconti speciali o restrizioni a livello di area</span><span class="sxs-lookup"><span data-stu-id="3b1dc-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="3b1dc-123">I prodotti non sono basati su sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="3b1dc-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="3b1dc-124">Il partner futuro dovrebbe collaborare con l'editore per assicurarsi che si trovino nell'elenco di elementi consentiti per la distribuzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="3b1dc-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="3b1dc-125">Se non vengono soddisfatte tutte queste condizioni per trasferire i prodotti del Marketplace, è necessario annullare le sottoscrizioni di Azure e quindi riacquistare i prodotti Marketplace con il nuovo partner</span><span class="sxs-lookup"><span data-stu-id="3b1dc-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="3b1dc-126">**Prerequisiti:**</span><span class="sxs-lookup"><span data-stu-id="3b1dc-126">**Prerequisites:**</span></span>

- <span data-ttu-id="3b1dc-127">Il cliente si impegna a eseguire la transizione del partner CSP corrente</span><span class="sxs-lookup"><span data-stu-id="3b1dc-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="3b1dc-128">Il partner CSP futuro collabora con il cliente per garantire che le esigenze dei clienti possano essere soddisfatte</span><span class="sxs-lookup"><span data-stu-id="3b1dc-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="3b1dc-129">Il partner CSP futuro stabilisce una relazione con il cliente prima dell'inizio della transizione</span><span class="sxs-lookup"><span data-stu-id="3b1dc-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="3b1dc-130">Il cliente deve firmare il contratto per i clienti Microsoft con il partner CSP futuro</span><span class="sxs-lookup"><span data-stu-id="3b1dc-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="3b1dc-131">Il partner CSP futuro deve avere firmato il contratto per i partner Microsoft per usare questo strumento</span><span class="sxs-lookup"><span data-stu-id="3b1dc-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="3b1dc-132">Attività del cliente da completare</span><span class="sxs-lookup"><span data-stu-id="3b1dc-132">Customer tasks to be completed</span></span>

<span data-ttu-id="3b1dc-133">Per trasferire una sottoscrizione di Azure in un piano di Azure, il cliente deve avviare il processo contattando il partner corrente.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="3b1dc-134">Devono raccogliere il nome e il dominio della società del partner corrente, in modo che il partner futuro possa completare il modulo di richiesta di trasferimento per loro conto.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="3b1dc-135">Il cliente deve inoltre identificare le sottoscrizioni che si desidera trasferire dal partner corrente.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="3b1dc-136">Non è possibile modificare i partner per le sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="3b1dc-137">È responsabilità del partner futuro completare il modulo di richiesta di trasferimento che avvia il processo di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="3b1dc-138">Microsoft non può intervenire per conto del cliente o del partner corrente.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="3b1dc-139">Il cliente deve pianificare di collaborare con il partner futuro e corrente per rendere la transizione senza problemi.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="3b1dc-140">Attività future del partner da completare</span><span class="sxs-lookup"><span data-stu-id="3b1dc-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="3b1dc-141">Il partner futuro della sottoscrizione deve completare un modulo di richiesta di trasferimento dal centro per i partner per richiedere il trasferimento di una sottoscrizione:</span><span class="sxs-lookup"><span data-stu-id="3b1dc-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="3b1dc-142">Dal menu centro per i partner selezionare **Customers**, quindi selezionare il cliente per il quale si desidera completare un modulo di richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="3b1dc-143">Dal menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="3b1dc-144">Selezionare la sezione **richiesta di trasferimento** .</span><span class="sxs-lookup"><span data-stu-id="3b1dc-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="3b1dc-145">Nella **sezione richiesta di trasferimento**selezionare **Aggiungi nuova richiesta**.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sezione trasferimenti":::

5.  <span data-ttu-id="3b1dc-147">Completare il modulo **nuova richiesta di trasferimento** .</span><span class="sxs-lookup"><span data-stu-id="3b1dc-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="3b1dc-148">Selezionare **Invia richiesta di trasferimento**  >  **invio**.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Sezione trasferimenti":::

7.  <span data-ttu-id="3b1dc-150">Verificare la conferma della richiesta di trasferimento</span><span class="sxs-lookup"><span data-stu-id="3b1dc-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Sezione trasferimenti":::

    >[!Note]
    ><span data-ttu-id="3b1dc-152">Il partner futuro può annullare la richiesta di trasferimento selezionando **Annulla richiesta** nell'angolo superiore destro solo quando lo stato della richiesta di trasferimento è "in sospeso".</span><span class="sxs-lookup"><span data-stu-id="3b1dc-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="3b1dc-153">Quando lo stato della richiesta di trasferimento è "in corso" o "completo", gli annullamenti non saranno possibili.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="3b1dc-154">Attività correnti del partner da completare</span><span class="sxs-lookup"><span data-stu-id="3b1dc-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="3b1dc-155">L'agente di amministrazione del partner corrente riceverà un messaggio di posta elettronica che indica che il cliente richiede il trasferimento delle sottoscrizioni:</span><span class="sxs-lookup"><span data-stu-id="3b1dc-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Sezione trasferimenti":::

<span data-ttu-id="3b1dc-157">Esaminare e accettare il modulo di richiesta di trasferimento dal centro per i partner per completare il trasferimento della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="3b1dc-158">Se non viene eseguita alcuna azione da parte del partner corrente entro 30 giorni, la richiesta scadrà e il partner futuro avrà un per creare una nuova richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="3b1dc-159">Selezionare **Verifica trasferimento richiesta** dal messaggio di posta elettronica o</span><span class="sxs-lookup"><span data-stu-id="3b1dc-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="3b1dc-160">Dal menu centro partner selezionare **Customers**, quindi selezionare il cliente a cui è stata inviata una richiesta di trasferimento per conto di.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="3b1dc-161">Dal menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="3b1dc-162">Selezionare la sezione **richiesta di trasferimento** .</span><span class="sxs-lookup"><span data-stu-id="3b1dc-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="3b1dc-163">Espandi le informazioni sul trasferimento selezionando l' **ID richiesta di trasferimento** selezionato in **richieste ricevute**</span><span class="sxs-lookup"><span data-stu-id="3b1dc-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Sezione trasferimenti":::

5.  <span data-ttu-id="3b1dc-165">Esaminare la richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-165">Review transfer request.</span></span> <span data-ttu-id="3b1dc-166">Selezionare le sottoscrizioni di Azure richieste da trasferire.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="3b1dc-167">Prima di procedere, tenere presente che non sarà più possibile accedere alle sottoscrizioni selezionate.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="3b1dc-168">Non verrà fatturato alcun ulteriore utilizzo.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="3b1dc-169">Le prenotazioni di Azure non vengono trasferite con le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="3b1dc-170">Selezionare quindi **Accept e transfer** per completare il processo di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sezione trasferimenti":::

7.  <span data-ttu-id="3b1dc-172">Visualizza conferma accettazione trasferimento.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="3b1dc-173">A questo punto, il partner futuro, il cliente e il partner corrente riceveranno una notifica della richiesta di trasferimento accettata tramite posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="3b1dc-174">Dopo che la transizione è stata accettata, lo stato del trasferimento potrebbe rimanere in sospeso per un massimo di 15 minuti durante l'aggiornamento del sistema.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="3b1dc-175">Se richiede più tempo, il sistema continuerà a provare per tre giorni.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="3b1dc-176">Se lo stato del trasferimento rimane ancora in sospeso, il partner deve inviare una richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="3b1dc-177">Al termine del trasferimento, le sottoscrizioni incluse nella richiesta verranno visualizzate nel piano Azure del partner futuro e non verranno più elencate.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="3b1dc-178">Per i provider indiretti, indicare al rivenditore indiretto che la richiesta di trasferimento è stata accettata.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="3b1dc-179">Gestione delle sottoscrizioni dei clienti trasferiti</span><span class="sxs-lookup"><span data-stu-id="3b1dc-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="3b1dc-180">La transizione non influisce sull'accesso per utenti, gruppi o entità servizio esistenti assegnati con il controllo degli accessi in base al ruolo di Azure.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="3b1dc-181">Il controllo degli accessi in base al ruolo di Azure [(RBAC di Azure)](/azure/role-based-access-control/overview) consente ai clienti di gestire gli utenti che hanno accesso alle risorse di Azure, le operazioni che possono eseguire con tali risorse e le aree a cui hanno accesso.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="3b1dc-182">Con il nuovo partner, dopo il trasferimento della sottoscrizione non viene fornito alcun accesso RBAC alle risorse del cliente.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="3b1dc-183">Il partner precedente del cliente mantiene il controllo degli accessi in base al ruolo.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="3b1dc-184">Collaborare con il cliente per comprendere chi ha informazioni dettagliate sulle sottoscrizioni e come apportare le modifiche desiderate.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="3b1dc-185">Di conseguenza, è importante che il cliente elimini l'accesso RBAC di Azure per il partner precedente e aggiunga l'accesso per il nuovo partner.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="3b1dc-186">Per altre informazioni sul cliente che fornisce un nuovo accesso, vedere [che cos'è il controllo degli accessi in base al ruolo di Azure (RBAC di Azure)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="3b1dc-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="3b1dc-187">Per ulteriori informazioni sul cliente che rimuove l'accesso RBAC del partner precedente, vedere [rimuovere un'assegnazione di ruolo](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="3b1dc-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="3b1dc-188">Inoltre, non è possibile ottenere automaticamente l'accesso [dell'amministratore per conto di (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) alle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="3b1dc-189">AOBO è necessario per i partner per gestire le sottoscrizioni di Azure del cliente per loro conto.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="3b1dc-190">Per altre informazioni sui privilegi di Azure, vedere [ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="3b1dc-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b1dc-191">Passaggi successivi:</span><span class="sxs-lookup"><span data-stu-id="3b1dc-191">Next steps:</span></span>

- [<span data-ttu-id="3b1dc-192">(RBAC di Azure)</span><span class="sxs-lookup"><span data-stu-id="3b1dc-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="3b1dc-193">Ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.</span><span class="sxs-lookup"><span data-stu-id="3b1dc-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)