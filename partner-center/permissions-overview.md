---
title: Assegnare ruoli agli utenti e le autorizzazioni | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Tutti i dipendenti che devono lavorare nel centro per i Partner devono essere assegnato un ruolo.
author: labrenne
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086729"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="03611-104">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="03611-104">Assign users roles and permissions</span></span>


<span data-ttu-id="03611-105">Aver configurare il profilo del partner, tra cui nome legale e indirizzo, i dettagli di supporto, le esenzioni fiscali, informazioni bancarie e il contatto principale per la tua azienda.</span><span class="sxs-lookup"><span data-stu-id="03611-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="03611-106">Passaggio successivo: ottenere gli utenti configurato con ruoli e le password in modo che possono iniziare a lavorare con te nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="03611-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="03611-107">Configurare i dipendenti di lavorare nel centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="03611-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="03611-108">Determinare i tipi di accesso che agli utenti dispongono Centro per i Partner per i ruoli e autorizzazioni che assegnare loro.</span><span class="sxs-lookup"><span data-stu-id="03611-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="03611-109">Ruoli sono correlati per i programmi a cui che l'azienda è interessato.</span><span class="sxs-lookup"><span data-stu-id="03611-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="03611-110">Ad esempio, se l'azienda è un'azienda Cloud Solution Provider (CSP), non solo è standard ad Azure AD tenant ruoli di gestione come amministratore globale, ma dovrà ruoli specifici per il programma CSP.</span><span class="sxs-lookup"><span data-stu-id="03611-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="03611-111">Ciascun programma ha ruoli ad esso specifici.</span><span class="sxs-lookup"><span data-stu-id="03611-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="03611-112">Ruoli di tenant Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="03611-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="03611-113">Ruoli di AAD di non includono amministratore MPN, amministratore del profilo di lavoro, amministratore dei riferimenti, amministratore di incentivi e utente degli incentivi.</span><span class="sxs-lookup"><span data-stu-id="03611-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="03611-114">Gestire le transazioni commerciali nel centro per i Partner (Azure AD e ruoli CSP)</span><span class="sxs-lookup"><span data-stu-id="03611-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="03611-115">Ruolo</span><span class="sxs-lookup"><span data-stu-id="03611-115">Role</span></span>**|**<span data-ttu-id="03611-116">Operazioni consentite</span><span class="sxs-lookup"><span data-stu-id="03611-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="03611-117">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="03611-117">Global admin</span></span>|<span data-ttu-id="03611-118">• Possono accedere a tutti gli account/servizi Microsoft con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="03611-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="03611-119">• Creazione di ticket di supporto per il centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="03611-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="03611-120">• Visualizzazione di contratti, listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="03611-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="03611-121">• Visualizzazione, creazione e gestione utenti partner</span><span class="sxs-lookup"><span data-stu-id="03611-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="03611-122">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="03611-122">User Admin</span></span>   | <span data-ttu-id="03611-123">• Visualizzazione, creazione e gestione di utenti</span><span class="sxs-lookup"><span data-stu-id="03611-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="03611-124">• Visualizzare tutti i profili dei partner</span><span class="sxs-lookup"><span data-stu-id="03611-124">• View all partner profiles</span></span>
||<span data-ttu-id="03611-125">• Visualizzazione, creazione e gestione utenti partner</span><span class="sxs-lookup"><span data-stu-id="03611-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="03611-126">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="03611-126">Default user</span></span>|  <span data-ttu-id="03611-127">Visualizza il mio profilo</span><span class="sxs-lookup"><span data-stu-id="03611-127">View My profile</span></span>   |
|<span data-ttu-id="03611-128">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="03611-128">Admin agent</span></span> | <span data-ttu-id="03611-129">• Dei clienti</span><span class="sxs-lookup"><span data-stu-id="03611-129">•    Customer management</span></span>
||<span data-ttu-id="03611-130">• Aggiungere elenco dei dispositivi per il Center< per i Partner</span><span class="sxs-lookup"><span data-stu-id="03611-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="03611-131">• Creare e applicare i profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="03611-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="03611-132">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="03611-132">• Subscription management</span></span>
||<span data-ttu-id="03611-133">• Servizio integrità e richieste di servizio per i clienti</span><span class="sxs-lookup"><span data-stu-id="03611-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="03611-134">• Richiedere i privilegi di amministratore delegato</span><span class="sxs-lookup"><span data-stu-id="03611-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="03611-135">• Visualizzazione prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="03611-135">• View pricing and offers</span></span>
||<span data-ttu-id="03611-136">• La fatturazione</span><span class="sxs-lookup"><span data-stu-id="03611-136">• Billing</span></span>
||<span data-ttu-id="03611-137">• Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="03611-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="03611-138">• Registrazione un valore aggiunto come rivenditore</span><span class="sxs-lookup"><span data-stu-id="03611-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="03611-139">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="03611-139">Sales agent</span></span> | <span data-ttu-id="03611-140">• Dei clienti</span><span class="sxs-lookup"><span data-stu-id="03611-140">•    Customer management</span></span>
||<span data-ttu-id="03611-141">• Aggiungere l'elenco dei dispositivi al centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="03611-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="03611-142">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="03611-142">• Subscription management</span></span>
||<span data-ttu-id="03611-143">• Visualizzazione ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="03611-143">• View support tickets</span></span>
||<span data-ttu-id="03611-144">• Richiedi una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="03611-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="03611-145">• La gestione dei lead dei clienti</span><span class="sxs-lookup"><span data-stu-id="03611-145">• Manage customer leads</span></span>
||<span data-ttu-id="03611-146">• Visualizzazione contratto per il cliente</span><span class="sxs-lookup"><span data-stu-id="03611-146">• View the customer agreement</span></span>
||<span data-ttu-id="03611-147">• Registrare un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="03611-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="03611-148">Agente help desk</span><span class="sxs-lookup"><span data-stu-id="03611-148">Helpdesk agent</span></span>| <span data-ttu-id="03611-149">• La ricerca e visualizzazione di un cliente</span><span class="sxs-lookup"><span data-stu-id="03611-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="03611-150">• Modificare i dettagli dei clienti</span><span class="sxs-lookup"><span data-stu-id="03611-150">• Edit customer details</span></span>
||<span data-ttu-id="03611-151">• La Guida risolvere i problemi dei clienti con la gestione di fatturazioni o sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="03611-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="03611-152">• Richiesta di supporto per conto dei clienti (Nota: È necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="03611-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="03611-153">• Gestire le sottoscrizioni e conto dei clienti (Nota: È necessario essere un agente amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="03611-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="03611-154">Fornitore Pannello di controllo (CPV).</span><span class="sxs-lookup"><span data-stu-id="03611-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="03611-155">(Ruolo CSP e non AAD)</span><span class="sxs-lookup"><span data-stu-id="03611-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="03611-156">CPVs sviluppare App per l'uso da parte dei partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con API del centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="03611-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="03611-157">Ruolo</span><span class="sxs-lookup"><span data-stu-id="03611-157">Role</span></span>**   |**<span data-ttu-id="03611-158">Cosa puoi fare</span><span class="sxs-lookup"><span data-stu-id="03611-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="03611-159">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="03611-159">Global admin</span></span>| <span data-ttu-id="03611-160">Visualizzare e gestire il profilo CPV</span><span class="sxs-lookup"><span data-stu-id="03611-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="03611-161">Visualizzare e gestire uno qualsiasi degli utenti che necessitano dell'accesso a funzionalità CPV</span><span class="sxs-lookup"><span data-stu-id="03611-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="03611-162">Gestire l'appartenenza a MPN e la tua azienda (ruoli non AAD)</span><span class="sxs-lookup"><span data-stu-id="03611-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="03611-163">Ruolo</span><span class="sxs-lookup"><span data-stu-id="03611-163">Role</span></span>** | **<span data-ttu-id="03611-164">Cosa puoi fare</span><span class="sxs-lookup"><span data-stu-id="03611-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="03611-165">Amministratore MPN</span><span class="sxs-lookup"><span data-stu-id="03611-165">MPN admin</span></span>|<span data-ttu-id="03611-166">•CAN aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="03611-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="03611-167">• Visualizzazione, creazione e gestione delle richieste di servizio per i partner</span><span class="sxs-lookup"><span data-stu-id="03611-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="03611-168">• Visualizzazione legali, l'organizzazione, le aziende e dei profili MPN</span><span class="sxs-lookup"><span data-stu-id="03611-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="03611-169">• Visualizzare i dettagli utente e i relativi dati delle competenze</span><span class="sxs-lookup"><span data-stu-id="03611-169">• View user details and their skills data</span></span>
||<span data-ttu-id="03611-170">• Visualizzazione delle competenze</span><span class="sxs-lookup"><span data-stu-id="03611-170">• View competencies</span></span>
||<span data-ttu-id="03611-171">• Consente di visualizzare e gestire i vantaggi</span><span class="sxs-lookup"><span data-stu-id="03611-171">• View and manage benefits</span></span>
||<span data-ttu-id="03611-172">Acquisto e la visualizzazione • alle offerte MPN</span><span class="sxs-lookup"><span data-stu-id="03611-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="03611-173">• Visualizzazione MPN fatture e cronologia degli ordini di offerte</span><span class="sxs-lookup"><span data-stu-id="03611-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="03611-174">• Visualizzare i dati di contributo per i partner</span><span class="sxs-lookup"><span data-stu-id="03611-174">• Can view partner contribution data</span></span>
||<span data-ttu-id="03611-175">• Possono utilizzare lo strumento di convalida giustificativo</span><span class="sxs-lookup"><span data-stu-id="03611-175">• Can work in the Voucher Validation tool</span></span>|
|<span data-ttu-id="03611-176">Account amministratore</span><span class="sxs-lookup"><span data-stu-id="03611-176">Account admin</span></span>| <span data-ttu-id="03611-177">• Aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="03611-177">•   Can add non-tenant users</span></span>
||<span data-ttu-id="03611-178">• Aggiungere o eliminare i percorsi</span><span class="sxs-lookup"><span data-stu-id="03611-178">• Add or delete locations</span></span>
||<span data-ttu-id="03611-179">-Gestire i profili correlati agli account che sei amministratore</span><span class="sxs-lookup"><span data-stu-id="03611-179">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="03611-180">• Assegna ruoli per gli utenti nel tenant a ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="03611-180">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="03611-181">• Registrare posizioni in programmi</span><span class="sxs-lookup"><span data-stu-id="03611-181">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="03611-182">Gestire i riferimenti (ruoli non AAD)</span><span class="sxs-lookup"><span data-stu-id="03611-182">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="03611-183">Ruolo</span><span class="sxs-lookup"><span data-stu-id="03611-183">Role</span></span>**|**<span data-ttu-id="03611-184">Cosa puoi fare</span><span class="sxs-lookup"><span data-stu-id="03611-184">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="03611-185">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="03611-185">Referrals admin</span></span>       |<span data-ttu-id="03611-186">• Visualizzazione, creazione e gestione dei profili aziendali</span><span class="sxs-lookup"><span data-stu-id="03611-186">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="03611-187">• Ricevere e gestivi segnalazioni</span><span class="sxs-lookup"><span data-stu-id="03611-187">• Receive and manage referrals</span></span>
||<span data-ttu-id="03611-188">• Visualizzazione, creazione e gestione delle richieste di servizio per i partner</span><span class="sxs-lookup"><span data-stu-id="03611-188">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="03611-189">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="03611-189">Business profile admin</span></span>   |<span data-ttu-id="03611-190">•View, creare e gestire profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="03611-190">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="03611-191">• Visualizzazione, creazione e gestione delle richieste di servizio per i partner</span><span class="sxs-lookup"><span data-stu-id="03611-191">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="03611-192">Gestire gli incentivi (ruoli non AAD)</span><span class="sxs-lookup"><span data-stu-id="03611-192">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="03611-193">Ruolo</span><span class="sxs-lookup"><span data-stu-id="03611-193">Role</span></span>** | **<span data-ttu-id="03611-194">Cosa puoi fare</span><span class="sxs-lookup"><span data-stu-id="03611-194">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="03611-195">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-195">Incentives admin</span></span>|<span data-ttu-id="03611-196">• Avvia e gestisce gli incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-196">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="03611-197">• Può visualizzare e modificare tutti gli aspetti di programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-197">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="03611-198">• Può visualizzare e modificare i dettagli bancari e fiscali</span><span class="sxs-lookup"><span data-stu-id="03611-198">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="03611-199">• Visualizzazione sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="03611-199">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="03611-200">• Supporto per l'accesso</span><span class="sxs-lookup"><span data-stu-id="03611-200">• Access support</span></span>
||<span data-ttu-id="03611-201">Pagamenti di incentivi controversie •</span><span class="sxs-lookup"><span data-stu-id="03611-201">• Dispute incentives payments</span></span>|
|<span data-ttu-id="03611-202">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-202">Incentives user</span></span>|<span data-ttu-id="03611-203">• Può visualizzare i programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-203">•  Can view incentives programs</span></span>
||<span data-ttu-id="03611-204">• Può visualizzare e avviare attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="03611-204">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="03611-205">• Visualizzazione sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="03611-205">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="03611-206">• Visualizzazione sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="03611-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="03611-207">• Supporto per l'accesso</span><span class="sxs-lookup"><span data-stu-id="03611-207">• Access support</span></span>












