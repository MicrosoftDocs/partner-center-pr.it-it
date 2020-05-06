---
title: Concedi ai clienti l'autorizzazione per acquistare i propri servizi
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri in che modo i partner del programma CSP possono consentire ai clienti di acquistare i propri servizi, ad esempio le prenotazioni di Azure, per una sottoscrizione acquistata per loro.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: sottoscrizione, acquisto self-service, riservatezza self-service, abilitazione di ri, disabilitazione di RI, self-service, acquisto di clienti, autorizzazioni dei clienti, istanza riservata di acquisto del cliente, prenotazione dei clienti di Azure, attivare la funzionalità self-service, disattivare la funzionalità self-service
ms.localizationpriority: medium
ms.openlocfilehash: ee8f1221344ce2375aff63c52bbfd42350a29839
ms.sourcegitcommit: 8359f618426e341180b0380367dd9d16dfd6623c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/29/2020
ms.locfileid: "82255465"
---
# <a name="learn-how-to-give-customers-permission-to-buy-their-own-products-or-services"></a><span data-ttu-id="93636-104">Informazioni su come concedere ai clienti l'autorizzazione per acquistare prodotti o servizi propri</span><span class="sxs-lookup"><span data-stu-id="93636-104">Learn how to give customers permission to buy their own products or services</span></span>

<span data-ttu-id="93636-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="93636-105">**Applies to**</span></span>

- <span data-ttu-id="93636-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="93636-106">Partner Center</span></span>
- <span data-ttu-id="93636-107">Partner aderenti al programma CSP</span><span class="sxs-lookup"><span data-stu-id="93636-107">Partners in the CSP program</span></span>

<span data-ttu-id="93636-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="93636-108">**Appropriate roles**</span></span>

- <span data-ttu-id="93636-109">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="93636-109">Admin agent</span></span>
- <span data-ttu-id="93636-110">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="93636-110">Sales agent</span></span>

<span data-ttu-id="93636-111">Questo articolo illustra in che modo un partner nel programma Cloud Solution Provider (CSP) può concedere a un cliente l'autorizzazione per acquistare alcuni dei propri servizi o risorse.</span><span class="sxs-lookup"><span data-stu-id="93636-111">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="93636-112">I partner del programma CSP spesso usano il centro per i partner e il suo Marketplace commerciale per acquistare soluzioni e servizi per i clienti.</span><span class="sxs-lookup"><span data-stu-id="93636-112">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="93636-113">I partner consentono quindi ad alcuni clienti di effettuare il provisioning di questi servizi direttamente dalla portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-113">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="93636-114">Di seguito è riportato un esempio.</span><span class="sxs-lookup"><span data-stu-id="93636-114">Here's an example.</span></span> <span data-ttu-id="93636-115">Supponiamo di acquistare una sottoscrizione di piano di Azure per un cliente nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-115">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="93636-116">Si decide quindi di aggiungere altre risorse o servizi alla sottoscrizione per conto dell'utente.</span><span class="sxs-lookup"><span data-stu-id="93636-116">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="93636-117">In questo caso, è possibile aggiungere prenotazioni di Azure alla sottoscrizione del cliente, ad esempio aggiungendo istanze di macchine virtuali riservate.</span><span class="sxs-lookup"><span data-stu-id="93636-117">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="93636-118">È quindi possibile consentire al cliente di eseguire ulteriormente il provisioning delle risorse di prenotazione di Azure nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-118">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="93636-119">Con la funzionalità per le **autorizzazioni** dei clienti, ora è possibile offrire ai clienti più opzioni self-service con le risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-119">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="93636-120">Attivando le autorizzazioni per il cliente, si consente ai clienti di acquistare le proprie risorse (ad esempio, acquistando le proprie prenotazioni di Azure).</span><span class="sxs-lookup"><span data-stu-id="93636-120">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="93636-121">Panoramica delle autorizzazioni dei clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="93636-121">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="93636-122">Utilizzare la pagina **account** cliente per attivare o disattivare le autorizzazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-122">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="93636-123">Attualmente questa funzionalità supporta:</span><span class="sxs-lookup"><span data-stu-id="93636-123">Currently, this feature supports:</span></span>

- <span data-ttu-id="93636-124">**Prenotazioni di Azure:** L'attivazione di questa autorizzazione consente al cliente di acquistare le proprie prenotazioni di Azure per una sottoscrizione di Azure specifica acquistata per loro.</span><span class="sxs-lookup"><span data-stu-id="93636-124">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="93636-125">Prima di attivare le autorizzazioni dei clienti, tenere presenti i seguenti punti importanti:</span><span class="sxs-lookup"><span data-stu-id="93636-125">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="93636-126">Per impostazione predefinita, le autorizzazioni dei clienti vengono disabilitate automaticamente (disattivate) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-126">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>
- <span data-ttu-id="93636-127">Prima di poter attivare o disattivare le autorizzazioni per un cliente, è necessario disporre del ruolo di agente di amministrazione nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-127">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>
  <span data-ttu-id="93636-128">I partner a cui è stato assegnato il ruolo di agente di vendita o di supporto tecnico hanno accesso in sola lettura e non possono attivare o disattivare le autorizzazioni dei clienti.</span><span class="sxs-lookup"><span data-stu-id="93636-128">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>
- <span data-ttu-id="93636-129">È possibile attivare le autorizzazioni (Abilita) per qualsiasi cliente scelto.</span><span class="sxs-lookup"><span data-stu-id="93636-129">You can turn on (enable) permissions for any customer you choose.</span></span>
- <span data-ttu-id="93636-130">È possibile attivare o disattivare le autorizzazioni dei clienti usando il dashboard del centro per i partner o le [API del centro](https://docs.microsoft.com/partner-center/develop/manage-customers)per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-130">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>
- <span data-ttu-id="93636-131">Dopo aver attivato (abilitato) le autorizzazioni per un cliente specifico, si sarà responsabili del pagamento di eventuali acquisti successivi effettuati dal cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-131">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="93636-132">Se i clienti vogliono scambiare, annullare o rinnovare un acquisto effettuato, non saranno in grado di eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="93636-132">If customers want to exchange, cancel or renew a purchase they have made, they will not be able to do so themselves.</span></span> <span data-ttu-id="93636-133">È necessario chiedere all'utente, come partner, di aiutarli a scambiare, annullare o rinnovare questi acquisti.</span><span class="sxs-lookup"><span data-stu-id="93636-133">They need to ask you, as the partner, to help them exchange, cancel, or renew these purchases.</span></span>
- <span data-ttu-id="93636-134">Dopo aver immesso le autorizzazioni per un cliente specifico, l'utente **non** riceverà alcuna notifica per eventuali acquisti successivi effettuati dal cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-134">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>
- <span data-ttu-id="93636-135">Gli acquisti successivi effettuati dal cliente verranno visualizzati nel centro per i partner insieme a eventuali acquisti effettuati dall'utente.</span><span class="sxs-lookup"><span data-stu-id="93636-135">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="93636-136">È possibile trovare questi acquisti nella pagina della **cronologia dell'ordine** del cliente, nella relativa pagina **prenotazioni** o nel [**log attività**](activity-logs.md).</span><span class="sxs-lookup"><span data-stu-id="93636-136">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="93636-137">Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="93636-137">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="93636-138">Le prenotazioni di Azure sono un ottimo modo per acquistare i servizi di Azure a una tariffa scontata.</span><span class="sxs-lookup"><span data-stu-id="93636-138">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="93636-139">Per altre informazioni sui vantaggi delle prenotazioni di Azure, vedere [che cosa sono le prenotazioni di Azure?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="93636-139">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="93636-140">È ora possibile scegliere di acquistare prenotazioni di Azure per conto dei clienti, come è già stato fatto.</span><span class="sxs-lookup"><span data-stu-id="93636-140">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="93636-141">In alternativa, è possibile concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-141">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="93636-142">Dopo aver fornito ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è possibile aiutarli a comprendere come gestire le prenotazioni acquistate.</span><span class="sxs-lookup"><span data-stu-id="93636-142">After you give customers permission to buy their own Azure reservations, you can help them understand how to manage any reservations they purchase.</span></span> <span data-ttu-id="93636-143">È ad esempio possibile che i clienti desiderino ottenere informazioni su come ottimizzare l'uso di una prenotazione o su come modificare l'ambito di una prenotazione.</span><span class="sxs-lookup"><span data-stu-id="93636-143">For instance, customers might want to know how to optimize their use of a reservation or how to change a reservation’s scope.</span></span> <span data-ttu-id="93636-144">Per altre informazioni su questi argomenti, chiedere ai clienti di leggere [gestire le prenotazioni per le risorse di Azure]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span><span class="sxs-lookup"><span data-stu-id="93636-144">For more information about these topics, ask customers to read [Manage reservations for Azure resources]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="93636-145">Per consentire ai clienti di acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="93636-145">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="93636-146">Verificare che il cliente disponga di un piano di Azure esistente o di una sottoscrizione globale di Azure acquistata per loro conto.</span><span class="sxs-lookup"><span data-stu-id="93636-146">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="93636-147">Verificare che al cliente sia stato assegnato il ruolo **proprietario** per questa sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="93636-147">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="93636-148">Abilitare le autorizzazioni dei clienti (attivare **questa funzionalità)** per acquistare le proprie prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-148">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="93636-149">Ogni passaggio viene visualizzato di seguito.</span><span class="sxs-lookup"><span data-stu-id="93636-149">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="93636-150">Verificare che il cliente disponga di una sottoscrizione di Azure esistente</span><span class="sxs-lookup"><span data-stu-id="93636-150">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="93636-151">Prima di concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure, è necessario verificare che il cliente disponga di un piano di Azure o di una sottoscrizione globale di Azure esistente.</span><span class="sxs-lookup"><span data-stu-id="93636-151">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="93636-152">Se il cliente non visualizza alcuna sottoscrizione di Azure corrente nel centro per i partner, è necessario acquistare una sottoscrizione prima di attivare le autorizzazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-152">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="93636-153">Per verificare se un cliente dispone già di una sottoscrizione di Azure, accedere al dashboard del centro per i partner, quindi selezionare **CSP** seguito dai **clienti**.</span><span class="sxs-lookup"><span data-stu-id="93636-153">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="93636-154">Selezionare il cliente specifico dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="93636-154">Select the specific customer from the list.</span></span> <span data-ttu-id="93636-155">Selezionare quindi **sottoscrizioni** e cercare eventuali sottoscrizioni basate sull'utilizzo per piano Azure o Azure globale.</span><span class="sxs-lookup"><span data-stu-id="93636-155">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="93636-156">Se un cliente non ha una sottoscrizione di Azure esistente, è possibile acquistarne una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="93636-156">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="93636-157">Vedere [acquistare il piano di Azure](purchase-azure-plan.md).</span><span class="sxs-lookup"><span data-stu-id="93636-157">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="93636-158">Verificare che al cliente sia stato assegnato il ruolo corretto in Azure</span><span class="sxs-lookup"><span data-stu-id="93636-158">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="93636-159">Dopo aver verificato che il cliente disponga di una sottoscrizione di Azure esistente, è necessario verificare anche che agli utenti chiave associati al cliente sia stato assegnato il ruolo di **proprietario** corretto per la sottoscrizione di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-159">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="93636-160">Questo è l'accesso in base al ruolo (RBAC) a cui il cliente deve acquistare le prenotazioni di Azure per una sottoscrizione di Azure acquistata.</span><span class="sxs-lookup"><span data-stu-id="93636-160">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="93636-161">Alcuni partner potrebbero avere già assegnato il ruolo di **proprietario** ai clienti che desiderano gestire attivamente ed effettuare il provisioning delle proprie risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-161">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="93636-162">Se lo stato del **proprietario** è già stato assegnato a un cliente per gestire le sottoscrizioni acquistate in precedenza, è possibile ignorare questo passaggio.</span><span class="sxs-lookup"><span data-stu-id="93636-162">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="93636-163">Se a un cliente non è stato assegnato il ruolo di **proprietario** , riceverà un errore nel portale di Azure impedendo loro di acquistare prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="93636-163">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="93636-164">Per verificare che al cliente sia stato assegnato il ruolo **proprietario** per una sottoscrizione di Azure:</span><span class="sxs-lookup"><span data-stu-id="93636-164">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="93636-165">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="93636-166">Selezionare **CSP**, **Customers** e selezionare il cliente specifico.</span><span class="sxs-lookup"><span data-stu-id="93636-166">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="93636-167">Selezionare le **sottoscrizioni** per il cliente e individuare la sottoscrizione di Azure specifica.</span><span class="sxs-lookup"><span data-stu-id="93636-167">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="93636-168">Selezionare il pulsante **Gestisci** accanto alla sottoscrizione del cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-168">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="93636-169">In questo modo si apre il [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="93636-169">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="93636-170">Per assegnare il ruolo **proprietario** a un utente specifico, attenersi alla procedura seguente [per assegnare un utente come amministratore](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span><span class="sxs-lookup"><span data-stu-id="93636-170">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="93636-171">Attivare o disattivare le autorizzazioni del cliente per acquistare le proprie prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="93636-171">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="93636-172">Dopo aver verificato che il cliente dispone di una sottoscrizione di Azure esistente e che agli utenti viene assegnato il ruolo di **proprietario** per la sottoscrizione, è possibile attivare le autorizzazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-172">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="93636-173">È anche possibile usare questi passaggi per disattivare (disabilitare) le autorizzazioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-173">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="93636-174">È possibile abilitare o disabilitare le autorizzazioni dei clienti usando il dashboard del centro per i partner o le [API del centro](https://docs.microsoft.com/partner-center/develop/manage-customers)per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-174">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="93636-175">Per attivare o disattivare le autorizzazioni dei clienti nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="93636-175">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="93636-176">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="93636-176">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="93636-177">Nel menu di spostamento a sinistra selezionare **CSP**e quindi **Customers**.</span><span class="sxs-lookup"><span data-stu-id="93636-177">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="93636-178">Verrà visualizzato un elenco di clienti.</span><span class="sxs-lookup"><span data-stu-id="93636-178">A customer list appears.</span></span>

3. <span data-ttu-id="93636-179">Selezionare un nome di cliente specifico.</span><span class="sxs-lookup"><span data-stu-id="93636-179">Select a specific customer name.</span></span>

4. <span data-ttu-id="93636-180">Selezionare **account** dal menu Customer.</span><span class="sxs-lookup"><span data-stu-id="93636-180">Select **Account** from the customer menu.</span></span> <span data-ttu-id="93636-181">Viene visualizzata la pagina **account** cliente.</span><span class="sxs-lookup"><span data-stu-id="93636-181">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="93636-182">Individuare l'area **autorizzazioni del cliente** nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="93636-182">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   ![Autorizzazioni del cliente nella pagina dell'account](images/give-customers-permission-reservations.png)

6. <span data-ttu-id="93636-184">In **prenotazioni di Azure**individuare l'opzione **Consenti al cliente di acquistare** .</span><span class="sxs-lookup"><span data-stu-id="93636-184">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="93636-185">Per attivare le autorizzazioni del cliente, spostare il commutatore accanto a questa opzione in posizione **on** .</span><span class="sxs-lookup"><span data-stu-id="93636-185">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="93636-186">Per disattivare le autorizzazioni del cliente, spostare il commutatore nella posizione **off** .</span><span class="sxs-lookup"><span data-stu-id="93636-186">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="93636-187">Per altre informazioni su ciò che accade quando si attivano le autorizzazioni di un cliente per acquistare le proprie prenotazioni di Azure, vedere [Panoramica delle autorizzazioni dei clienti nel centro per i partner](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="93636-187">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span> <span data-ttu-id="93636-188">Quando si attivano o disattivano le autorizzazioni del cliente, il log attività registra ciascuna azione.</span><span class="sxs-lookup"><span data-stu-id="93636-188">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="93636-189">(Questo log è accessibile quando si seleziona l'icona a forma di ingranaggio nella parte superiore del dashboard del centro per i partner).</span><span class="sxs-lookup"><span data-stu-id="93636-189">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="93636-190">Quando si attivano o disattivano le autorizzazioni del cliente, l'azione verrà visualizzata come **creare autorizzazioni di acquisto del cliente** o **eliminare le autorizzazioni di acquisto del cliente** nel log attività.</span><span class="sxs-lookup"><span data-stu-id="93636-190">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="see-also"></a><span data-ttu-id="93636-191">Vedere anche</span><span class="sxs-lookup"><span data-stu-id="93636-191">See also</span></span>

- [<span data-ttu-id="93636-192">Acquista prenotazioni di Azure per conto dei tuoi clienti</span><span class="sxs-lookup"><span data-stu-id="93636-192">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="93636-193">Centro per i partner-vendere prenotazioni Microsoft</span><span class="sxs-lookup"><span data-stu-id="93636-193">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)
- [<span data-ttu-id="93636-194">Gestisci prenotazioni di Azure per conto dei tuoi clienti</span><span class="sxs-lookup"><span data-stu-id="93636-194">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md) 