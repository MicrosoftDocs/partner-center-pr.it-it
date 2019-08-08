---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 3/5/2019
description: A tutti i dipendenti che devono lavorare nel centro per i partner deve essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708861"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="aaa68-104">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="aaa68-104">Assign users roles and permissions</span></span>


<span data-ttu-id="aaa68-105">Il profilo partner è stato configurato, inclusi nome e indirizzo validi, informazioni di supporto, esenzioni fiscali per i file, informazioni bancarie e il contatto principale per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="aaa68-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="aaa68-106">Passaggio successivo: configurare gli utenti con password e ruoli in modo che possano iniziare a lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="aaa68-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="aaa68-107">Configurare i dipendenti per lavorare nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="aaa68-108">Si determinano i tipi di accesso che gli utenti devono avere al centro per i partner mediante i ruoli e le autorizzazioni che si forniscono.</span><span class="sxs-lookup"><span data-stu-id="aaa68-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="aaa68-109">I ruoli sono correlati ai programmi interessati dall'azienda.</span><span class="sxs-lookup"><span data-stu-id="aaa68-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="aaa68-110">Se, ad esempio, l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo i ruoli di gestione dei tenant di Azure AD standard, ad esempio l'amministratore globale, ma dovranno avere ruoli specifici per il programma CSP.</span><span class="sxs-lookup"><span data-stu-id="aaa68-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="aaa68-111">Ogni programma dispone di ruoli specifici.</span><span class="sxs-lookup"><span data-stu-id="aaa68-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="aaa68-112">I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, amministratore utente e ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="aaa68-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="aaa68-113">I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore del riferimento, l'amministratore di incentivi e l'utente di incentivi.</span><span class="sxs-lookup"><span data-stu-id="aaa68-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="aaa68-114">Gestire le transazioni commerciali nel centro per i partner (ruoli Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="aaa68-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="aaa68-115">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="aaa68-115">**Role**</span></span>|<span data-ttu-id="aaa68-116">**Cosa è possibile fare**</span><span class="sxs-lookup"><span data-stu-id="aaa68-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="aaa68-117">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="aaa68-117">Global admin</span></span>|<span data-ttu-id="aaa68-118">• Può accedere a tutti i account Microsoft/servizi con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="aaa68-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="aaa68-119">• Creare ticket di supporto per il centro per i partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaa68-120">• Visualizzare contratti, elenchi prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="aaa68-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="aaa68-121">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="aaa68-122">Visualizzare, creare e gestire la fatturazione, le fatture e i file di ricognizione</span><span class="sxs-lookup"><span data-stu-id="aaa68-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="aaa68-123">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-123">User management admin</span></span>   | <span data-ttu-id="aaa68-124">• Visualizzare, creare e gestire gli utenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="aaa68-125">• Visualizza tutti i profili partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-125">• View all partner profiles</span></span>
||<span data-ttu-id="aaa68-126">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="aaa68-127">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="aaa68-127">Billing admin</span></span> | <span data-ttu-id="aaa68-128">-Visualizzare, creare e gestire la fatturazione, le fatture e i file di ricognizione</span><span class="sxs-lookup"><span data-stu-id="aaa68-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="aaa68-129">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="aaa68-129">Default user</span></span>|  <span data-ttu-id="aaa68-130">Visualizza profilo personale</span><span class="sxs-lookup"><span data-stu-id="aaa68-130">View My profile</span></span>   |
|<span data-ttu-id="aaa68-131">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="aaa68-131">Admin agent</span></span> | <span data-ttu-id="aaa68-132">• Gestione clienti</span><span class="sxs-lookup"><span data-stu-id="aaa68-132">•    Customer management</span></span>
||<span data-ttu-id="aaa68-133">• Aggiungere un elenco di dispositivi al centro per i partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="aaa68-134">• Creare e applicare profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="aaa68-135">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="aaa68-135">• Subscription management</span></span>
||<span data-ttu-id="aaa68-136">• Richieste di assistenza e integrità dei servizi per i clienti</span><span class="sxs-lookup"><span data-stu-id="aaa68-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="aaa68-137">• Richiedere privilegi di amministratore delegato</span><span class="sxs-lookup"><span data-stu-id="aaa68-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="aaa68-138">• Visualizza prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="aaa68-138">• View pricing and offers</span></span>
||<span data-ttu-id="aaa68-139">• Fatturazione</span><span class="sxs-lookup"><span data-stu-id="aaa68-139">• Billing</span></span>
||<span data-ttu-id="aaa68-140">• Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="aaa68-141">• Registrare un valore aggiunto rivenditore</span><span class="sxs-lookup"><span data-stu-id="aaa68-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="aaa68-142">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="aaa68-142">Sales agent</span></span> | <span data-ttu-id="aaa68-143">• Gestione clienti</span><span class="sxs-lookup"><span data-stu-id="aaa68-143">•    Customer management</span></span>
||<span data-ttu-id="aaa68-144">• Aggiungere un elenco di dispositivi al centro per i partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="aaa68-145">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="aaa68-145">• Subscription management</span></span>
||<span data-ttu-id="aaa68-146">• Visualizza elenchi prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="aaa68-146">• View price lists and offers</span></span>
||<span data-ttu-id="aaa68-147">• Visualizzare i ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="aaa68-147">• View support tickets</span></span>
||<span data-ttu-id="aaa68-148">• Richiedere una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="aaa68-149">• Gestisci lead cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-149">• Manage customer leads</span></span>
||<span data-ttu-id="aaa68-150">• Visualizzare il contratto del cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-150">• View the customer agreement</span></span>
||<span data-ttu-id="aaa68-151">• Registrare un rivenditore con valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="aaa68-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="aaa68-152">Agente help desk</span><span class="sxs-lookup"><span data-stu-id="aaa68-152">Helpdesk agent</span></span>| <span data-ttu-id="aaa68-153">• Cercare e visualizzare un cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="aaa68-154">• Modificare i dettagli del cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-154">• Edit customer details</span></span>
||<span data-ttu-id="aaa68-155">• Risolvere i problemi del cliente con la fatturazione o la gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="aaa68-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="aaa68-156">• Richiedere supporto per conto dei clienti (Nota: Per completare questa attività per le sottoscrizioni di Office 365, è necessario essere un agente di amministrazione</span><span class="sxs-lookup"><span data-stu-id="aaa68-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="aaa68-157">• Gestire le sottoscrizioni e i problemi di fatturazione per conto dei clienti (Nota: Per completare questa attività per le sottoscrizioni di Office 365, è necessario essere un agente di amministrazione</span><span class="sxs-lookup"><span data-stu-id="aaa68-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="aaa68-158">Pannello di controllo Fornitore (CPV).</span><span class="sxs-lookup"><span data-stu-id="aaa68-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="aaa68-159">(Ruolo CSP e ruolo non AAD)</span><span class="sxs-lookup"><span data-stu-id="aaa68-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="aaa68-160">CPVs sviluppa le app per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="aaa68-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="aaa68-161">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="aaa68-161">**Role**</span></span>   |<span data-ttu-id="aaa68-162">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="aaa68-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="aaa68-163">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="aaa68-163">Global admin</span></span>| <span data-ttu-id="aaa68-164">Visualizzare e gestire il profilo CPV</span><span class="sxs-lookup"><span data-stu-id="aaa68-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="aaa68-165">Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV</span><span class="sxs-lookup"><span data-stu-id="aaa68-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="aaa68-166">Utente Guest (deve essere aggiunto al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="aaa68-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="aaa68-167">**Utente Guest**</span><span class="sxs-lookup"><span data-stu-id="aaa68-167">**Guest user**</span></span>   | <span data-ttu-id="aaa68-168">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="aaa68-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="aaa68-169">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="aaa68-169">MPN partner admin</span></span>|
||<span data-ttu-id="aaa68-170">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="aaa68-170">Accounts admin</span></span>|
||<span data-ttu-id="aaa68-171">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-171">Incentives admin</span></span>|
||<span data-ttu-id="aaa68-172">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="aaa68-172">Business profile admin</span></span>|
||<span data-ttu-id="aaa68-173">Amministratore riferimenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="aaa68-174">Gestire l'appartenenza a MPN e la società (ruoli non AAD: questi ruoli gestiscono l'azienda anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="aaa68-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="aaa68-175">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="aaa68-175">**Role**</span></span> | <span data-ttu-id="aaa68-176">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="aaa68-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="aaa68-177">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="aaa68-177">MPN partner admin</span></span>|<span data-ttu-id="aaa68-178">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="aaa68-179">• Visualizzare profili legali, aziendali, aziendali e MPN</span><span class="sxs-lookup"><span data-stu-id="aaa68-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="aaa68-180">• Visualizzare i dettagli dell'utente e i relativi dati di competenze</span><span class="sxs-lookup"><span data-stu-id="aaa68-180">• View user details and their skills data</span></span>
||<span data-ttu-id="aaa68-181">• Visualizzare le competenze</span><span class="sxs-lookup"><span data-stu-id="aaa68-181">• View competencies</span></span>
||<span data-ttu-id="aaa68-182">• Visualizzare e gestire i vantaggi</span><span class="sxs-lookup"><span data-stu-id="aaa68-182">• View and manage benefits</span></span>
||<span data-ttu-id="aaa68-183">• Visualizzare e acquistare offerte MPN</span><span class="sxs-lookup"><span data-stu-id="aaa68-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="aaa68-184">• View MPN offre la cronologia degli ordini e le fatture</span><span class="sxs-lookup"><span data-stu-id="aaa68-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="aaa68-185">• Visualizzare i dati degli indicatori di contributo partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="aaa68-186">• È possibile usare lo strumento di convalida del voucher</span><span class="sxs-lookup"><span data-stu-id="aaa68-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="aaa68-187">-Visualizzare analisi dei dati del cliente</span><span class="sxs-lookup"><span data-stu-id="aaa68-187">- View customer data analytics</span></span>
|| <span data-ttu-id="aaa68-188">Visualizza altri ruoli utente all'interno della società, ma non può assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="aaa68-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="aaa68-189">Amministratore account</span><span class="sxs-lookup"><span data-stu-id="aaa68-189">Account admin</span></span>| <span data-ttu-id="aaa68-190">Aggiungi percorsi</span><span class="sxs-lookup"><span data-stu-id="aaa68-190">Add locations</span></span>
|| <span data-ttu-id="aaa68-191">Gestire i profili correlati agli account per i quali si è amministratori</span><span class="sxs-lookup"><span data-stu-id="aaa68-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="aaa68-192">• Assegnare i ruoli per gli utenti nel tenant ai ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="aaa68-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="aaa68-193">• Registrare i percorsi nei programmi</span><span class="sxs-lookup"><span data-stu-id="aaa68-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="aaa68-194">Gestisci riferimenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-194">Manage referrals</span></span> 

|<span data-ttu-id="aaa68-195">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="aaa68-195">**Role**</span></span>|<span data-ttu-id="aaa68-196">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="aaa68-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="aaa68-197">Amministratore riferimenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-197">Referrals admin</span></span>       |<span data-ttu-id="aaa68-198">• Visualizzare, creare e gestire i profili di business</span><span class="sxs-lookup"><span data-stu-id="aaa68-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="aaa68-199">• Ricevere e gestire i riferimenti</span><span class="sxs-lookup"><span data-stu-id="aaa68-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="aaa68-200">• Visualizzare, creare e gestire i riferimenti di co-selling</span><span class="sxs-lookup"><span data-stu-id="aaa68-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="aaa68-201">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="aaa68-202">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="aaa68-202">Business profile admin</span></span>   |<span data-ttu-id="aaa68-203">• Visualizzare, creare e gestire il profilo di business</span><span class="sxs-lookup"><span data-stu-id="aaa68-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="aaa68-204">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="aaa68-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="aaa68-205">Gestisci incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-205">Manage incentives</span></span> 

|<span data-ttu-id="aaa68-206">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="aaa68-206">**Role**</span></span> | <span data-ttu-id="aaa68-207">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="aaa68-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="aaa68-208">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-208">Incentives admin</span></span>|<span data-ttu-id="aaa68-209">• Avvia e gestisce gli incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="aaa68-210">• Consente di visualizzare e modificare tutti gli aspetti dei programmi per gli incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="aaa68-211">• Consente di visualizzare e modificare le informazioni fiscali e bancarie</span><span class="sxs-lookup"><span data-stu-id="aaa68-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="aaa68-212">• Visualizzare i guadagni di sconto e co-op</span><span class="sxs-lookup"><span data-stu-id="aaa68-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="aaa68-213">• Supporto per l'accesso</span><span class="sxs-lookup"><span data-stu-id="aaa68-213">• Access support</span></span>
||<span data-ttu-id="aaa68-214">• Pagamenti di incentivi per controversie</span><span class="sxs-lookup"><span data-stu-id="aaa68-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="aaa68-215">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-215">Incentives user</span></span>|<span data-ttu-id="aaa68-216">• Può visualizzare i programmi per gli incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="aaa68-217">• Può visualizzare e avviare attestazioni per gli incentivi</span><span class="sxs-lookup"><span data-stu-id="aaa68-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="aaa68-218">• Visualizzare i guadagni di sconto e co-op</span><span class="sxs-lookup"><span data-stu-id="aaa68-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="aaa68-219">• Supporto per l'accesso</span><span class="sxs-lookup"><span data-stu-id="aaa68-219">• Access support</span></span>












