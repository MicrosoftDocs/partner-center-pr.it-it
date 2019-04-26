---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 3/5/19
description: Tutti i dipendenti che hanno necessità di lavorare in Partner Center devono essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133901"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="de5ae-104">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="de5ae-104">Assign users roles and permissions</span></span>


<span data-ttu-id="de5ae-105">È stata configurare il profilo di partner inclusi ragione sociale e indirizzi, i dettagli sul supporto, esenzione di file, informazioni bancarie e il contatto principale per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="de5ae-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="de5ae-106">Passaggio successivo: gli utenti configurati con le password e i ruoli in modo che possano iniziare a lavorare nel centro per i Partner con l'utente.</span><span class="sxs-lookup"><span data-stu-id="de5ae-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="de5ae-107">Configurare i dipendenti di lavorare in Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="de5ae-108">Determinare i tipi di accesso che al centro per i Partner gli utenti dispongono per i ruoli e autorizzazioni che finti.</span><span class="sxs-lookup"><span data-stu-id="de5ae-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="de5ae-109">I ruoli sono correlati per le applicazioni che è interessata dalla propria azienda.</span><span class="sxs-lookup"><span data-stu-id="de5ae-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="de5ae-110">Ad esempio, se l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo è il standard di Azure AD i ruoli di gestione, ad esempio amministratore globale del tenant, ma sarà necessario ruoli specifici per il programma CSP.</span><span class="sxs-lookup"><span data-stu-id="de5ae-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="de5ae-111">Ogni programma svolge ruoli specifici a esso.</span><span class="sxs-lookup"><span data-stu-id="de5ae-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="de5ae-112">I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="de5ae-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="de5ae-113">Ruoli AAD-non includono MPN amministratore, amministratore profilo business, amministrazione di referral, admin incentivi e incentivi utente.</span><span class="sxs-lookup"><span data-stu-id="de5ae-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="de5ae-114">Gestire le transazioni commerciali nel centro per i Partner (Azure AD e i ruoli CSP)</span><span class="sxs-lookup"><span data-stu-id="de5ae-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="de5ae-115">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="de5ae-115">**Role**</span></span>|<span data-ttu-id="de5ae-116">**Le operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="de5ae-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="de5ae-117">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="de5ae-117">Global admin</span></span>|<span data-ttu-id="de5ae-118">• Possono accedere a tutti i Microsoft account/servizi con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="de5ae-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="de5ae-119">• Creare ticket di supporto per il centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="de5ae-120">• Visualizzare gli accordi sui listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="de5ae-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="de5ae-121">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="de5ae-122">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="de5ae-122">User Admin</span></span>   | <span data-ttu-id="de5ae-123">• Visualizzare, creare e gestire gli utenti</span><span class="sxs-lookup"><span data-stu-id="de5ae-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="de5ae-124">• Visualizzare tutti i profili partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-124">• View all partner profiles</span></span>
||<span data-ttu-id="de5ae-125">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="de5ae-126">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="de5ae-126">Billing admin</span></span> | <span data-ttu-id="de5ae-127">-Visualizzare, creare e gestire la fatturazione, fatture e i file di riconoscimento</span><span class="sxs-lookup"><span data-stu-id="de5ae-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="de5ae-128">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="de5ae-128">Default user</span></span>|  <span data-ttu-id="de5ae-129">Visualizza profilo personale</span><span class="sxs-lookup"><span data-stu-id="de5ae-129">View My profile</span></span>   |
|<span data-ttu-id="de5ae-130">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="de5ae-130">Admin agent</span></span> | <span data-ttu-id="de5ae-131">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="de5ae-131">•    Customer management</span></span>
||<span data-ttu-id="de5ae-132">• Aggiungere l'elenco dei dispositivi al centro per i Partner <</span><span class="sxs-lookup"><span data-stu-id="de5ae-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="de5ae-133">• Creare e applicare i profili nei dispositivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="de5ae-134">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="de5ae-134">• Subscription management</span></span>
||<span data-ttu-id="de5ae-135">• Servizio integrità e soddisfare richieste per i clienti</span><span class="sxs-lookup"><span data-stu-id="de5ae-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="de5ae-136">• Richiesta delegati i privilegi di amministratore</span><span class="sxs-lookup"><span data-stu-id="de5ae-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="de5ae-137">• Visualizza i prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="de5ae-137">• View pricing and offers</span></span>
||<span data-ttu-id="de5ae-138">• La fatturazione</span><span class="sxs-lookup"><span data-stu-id="de5ae-138">• Billing</span></span>
||<span data-ttu-id="de5ae-139">• Amministra per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="de5ae-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="de5ae-140">• Registra un valore aggiunto rivenditore</span><span class="sxs-lookup"><span data-stu-id="de5ae-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="de5ae-141">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="de5ae-141">Sales agent</span></span> | <span data-ttu-id="de5ae-142">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="de5ae-142">•    Customer management</span></span>
||<span data-ttu-id="de5ae-143">• Aggiungere l'elenco dei dispositivi al centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="de5ae-144">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="de5ae-144">• Subscription management</span></span>
||<span data-ttu-id="de5ae-145">Ticket di supporto di visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="de5ae-145">• View support tickets</span></span>
||<span data-ttu-id="de5ae-146">• Richiesta una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="de5ae-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="de5ae-147">• Gestire i lead dei clienti</span><span class="sxs-lookup"><span data-stu-id="de5ae-147">• Manage customer leads</span></span>
||<span data-ttu-id="de5ae-148">• Visualizzare il contratto del cliente</span><span class="sxs-lookup"><span data-stu-id="de5ae-148">• View the customer agreement</span></span>
||<span data-ttu-id="de5ae-149">• Registro un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="de5ae-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="de5ae-150">Agente help desk</span><span class="sxs-lookup"><span data-stu-id="de5ae-150">Helpdesk agent</span></span>| <span data-ttu-id="de5ae-151">• Cercare e visualizzare un cliente</span><span class="sxs-lookup"><span data-stu-id="de5ae-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="de5ae-152">• Modificare i dettagli cliente</span><span class="sxs-lookup"><span data-stu-id="de5ae-152">• Edit customer details</span></span>
||<span data-ttu-id="de5ae-153">• Guida risolvere cliente i problemi con la gestione di fatturazione o alla sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="de5ae-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="de5ae-154">• Richiedere il supporto per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="de5ae-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="de5ae-155">• Gestire le sottoscrizioni e fatturazione problemi per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="de5ae-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="de5ae-156">Fornitore del Pannello di controllo (CPV).</span><span class="sxs-lookup"><span data-stu-id="de5ae-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="de5ae-157">(Non-AAD ruolo e ruolo CSP)</span><span class="sxs-lookup"><span data-stu-id="de5ae-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="de5ae-158">CPVs lo sviluppo di App per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="de5ae-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="de5ae-159">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="de5ae-159">**Role**</span></span>   |<span data-ttu-id="de5ae-160">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="de5ae-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="de5ae-161">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="de5ae-161">Global admin</span></span>| <span data-ttu-id="de5ae-162">Visualizzare e gestire il profilo CPV</span><span class="sxs-lookup"><span data-stu-id="de5ae-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="de5ae-163">Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV</span><span class="sxs-lookup"><span data-stu-id="de5ae-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="de5ae-164">Gestire l'appartenenza MPN e la propria azienda (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="de5ae-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="de5ae-165">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="de5ae-165">**Role**</span></span> | <span data-ttu-id="de5ae-166">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="de5ae-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="de5ae-167">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="de5ae-167">MPN partner admin</span></span>|<span data-ttu-id="de5ae-168">•CAN aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="de5ae-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="de5ae-169">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="de5ae-170">• Vista legale, l'organizzazione, business e i profili MPN</span><span class="sxs-lookup"><span data-stu-id="de5ae-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="de5ae-171">• Visualizzare i dettagli di utente e i relativi dati di competenze</span><span class="sxs-lookup"><span data-stu-id="de5ae-171">• View user details and their skills data</span></span>
||<span data-ttu-id="de5ae-172">• Visualizza competenze</span><span class="sxs-lookup"><span data-stu-id="de5ae-172">• View competencies</span></span>
||<span data-ttu-id="de5ae-173">• Visualizzare e gestire i vantaggi</span><span class="sxs-lookup"><span data-stu-id="de5ae-173">• View and manage benefits</span></span>
||<span data-ttu-id="de5ae-174">Acquisto e la visualizzazione • ottenuta MPN</span><span class="sxs-lookup"><span data-stu-id="de5ae-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="de5ae-175">• Visualizzare MPN offre le fatture e cronologia degli ordini</span><span class="sxs-lookup"><span data-stu-id="de5ae-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="de5ae-176">• Visualizza dati contributi di partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-176">• View partner contribution data</span></span>
||<span data-ttu-id="de5ae-177">• Possono utilizzare lo strumento di convalida Voucher</span><span class="sxs-lookup"><span data-stu-id="de5ae-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="de5ae-178">-Visualizzare analitica dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="de5ae-178">- View customer data analytics</span></span>
|<span data-ttu-id="de5ae-179">Amministratore account</span><span class="sxs-lookup"><span data-stu-id="de5ae-179">Account admin</span></span>| <span data-ttu-id="de5ae-180">• È possibile aggiungere gli utenti non tenant</span><span class="sxs-lookup"><span data-stu-id="de5ae-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="de5ae-181">• Aggiunta o eliminazione di percorsi</span><span class="sxs-lookup"><span data-stu-id="de5ae-181">• Add or delete locations</span></span>
||<span data-ttu-id="de5ae-182">-Gestire i profili relativi agli account di per che amministratore</span><span class="sxs-lookup"><span data-stu-id="de5ae-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="de5ae-183">• Assegnare ruoli per gli utenti nel tenant per i ruoli AAD non</span><span class="sxs-lookup"><span data-stu-id="de5ae-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="de5ae-184">• Percorsi nei programmi di registrazione</span><span class="sxs-lookup"><span data-stu-id="de5ae-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="de5ae-185">Utente guest (devono essere aggiunti al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="de5ae-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="de5ae-186">**Utente Guest**</span><span class="sxs-lookup"><span data-stu-id="de5ae-186">**Guest user**</span></span>   | <span data-ttu-id="de5ae-187">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="de5ae-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="de5ae-188">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="de5ae-188">MPN partner admin</span></span>|
||<span data-ttu-id="de5ae-189">Gli account amministratore</span><span class="sxs-lookup"><span data-stu-id="de5ae-189">Accounts admin</span></span>|
||<span data-ttu-id="de5ae-190">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-190">Incentives admin</span></span>|
||<span data-ttu-id="de5ae-191">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="de5ae-191">Business profile admin</span></span>|
||<span data-ttu-id="de5ae-192">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="de5ae-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="de5ae-193">Gestire i riferimenti (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="de5ae-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="de5ae-194">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="de5ae-194">**Role**</span></span>|<span data-ttu-id="de5ae-195">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="de5ae-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="de5ae-196">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="de5ae-196">Referrals admin</span></span>       |<span data-ttu-id="de5ae-197">• Visualizzare, creare e gestire i profili di business</span><span class="sxs-lookup"><span data-stu-id="de5ae-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="de5ae-198">• Ricevere e gestire i riferimenti</span><span class="sxs-lookup"><span data-stu-id="de5ae-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="de5ae-199">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="de5ae-200">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="de5ae-200">Business profile admin</span></span>   |<span data-ttu-id="de5ae-201">• Visualizzare, creare e gestire il profilo di business</span><span class="sxs-lookup"><span data-stu-id="de5ae-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="de5ae-202">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="de5ae-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="de5ae-203">Gestire gli incentivi (ruoli non-AAD)</span><span class="sxs-lookup"><span data-stu-id="de5ae-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="de5ae-204">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="de5ae-204">**Role**</span></span> | <span data-ttu-id="de5ae-205">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="de5ae-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="de5ae-206">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-206">Incentives admin</span></span>|<span data-ttu-id="de5ae-207">• Avvia e gestisce gli incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="de5ae-208">• È possibile visualizzare e modificare tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="de5ae-209">• È possibile visualizzare e modificare i dettagli fiscali e bancarie</span><span class="sxs-lookup"><span data-stu-id="de5ae-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="de5ae-210">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="de5ae-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="de5ae-211">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="de5ae-211">• Access support</span></span>
||<span data-ttu-id="de5ae-212">Pagamenti di incentivi controversia •</span><span class="sxs-lookup"><span data-stu-id="de5ae-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="de5ae-213">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-213">Incentives user</span></span>|<span data-ttu-id="de5ae-214">• Consente di visualizzare i programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="de5ae-215">• È possibile visualizzare e avviare le attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="de5ae-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="de5ae-216">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="de5ae-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="de5ae-217">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="de5ae-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="de5ae-218">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="de5ae-218">• Access support</span></span>












