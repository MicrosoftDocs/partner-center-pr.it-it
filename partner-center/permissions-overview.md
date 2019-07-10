---
title: Assegnare autorizzazioni e ruoli utente | Centro per i partner
ms.topic: article
ms.date: 3/5/19
description: Tutti i dipendenti che hanno necessità di lavorare in Partner Center devono essere assegnato un ruolo.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690845"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="dcff0-104">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="dcff0-104">Assign users roles and permissions</span></span>


<span data-ttu-id="dcff0-105">È stata configurare il profilo di partner inclusi ragione sociale e indirizzi, i dettagli sul supporto, esenzione di file, informazioni bancarie e il contatto principale per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="dcff0-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="dcff0-106">Passaggio successivo: gli utenti configurati con le password e i ruoli in modo che possano iniziare a lavorare nel centro per i Partner con l'utente.</span><span class="sxs-lookup"><span data-stu-id="dcff0-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="dcff0-107">Configurare i dipendenti di lavorare in Centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="dcff0-108">Determinare i tipi di accesso che al centro per i Partner gli utenti dispongono per i ruoli e autorizzazioni che finti.</span><span class="sxs-lookup"><span data-stu-id="dcff0-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="dcff0-109">I ruoli sono correlati per le applicazioni che è interessata dalla propria azienda.</span><span class="sxs-lookup"><span data-stu-id="dcff0-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="dcff0-110">Ad esempio, se l'azienda è un'azienda di Cloud Solution Provider (CSP), non solo è il standard di Azure AD i ruoli di gestione, ad esempio amministratore globale del tenant, ma sarà necessario ruoli specifici per il programma CSP.</span><span class="sxs-lookup"><span data-stu-id="dcff0-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="dcff0-111">Ogni programma svolge ruoli specifici a esso.</span><span class="sxs-lookup"><span data-stu-id="dcff0-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="dcff0-112">I ruoli tenant di Azure Active Directory (AAD) includono amministratore globale, Amministratore utenti e ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="dcff0-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="dcff0-113">Non-AAD ruoli sono tali che non si gestisce il tenant e includono amministratore MPN, admin profilo business, amministrazione di referral, admin incentivi e incentivi utente.</span><span class="sxs-lookup"><span data-stu-id="dcff0-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="dcff0-114">Gestire le transazioni commerciali nel centro per i Partner (Azure AD e i ruoli CSP)</span><span class="sxs-lookup"><span data-stu-id="dcff0-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="dcff0-115">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcff0-115">**Role**</span></span>|<span data-ttu-id="dcff0-116">**Le operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="dcff0-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="dcff0-117">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="dcff0-117">Global admin</span></span>|<span data-ttu-id="dcff0-118">• Possono accedere a tutti i Microsoft account/servizi con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="dcff0-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="dcff0-119">• Creare ticket di supporto per il centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="dcff0-120">• Visualizzare gli accordi sui listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="dcff0-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="dcff0-121">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="dcff0-122">Visualizzare, creare e gestire la fatturazione, fatture e i file di riconoscimento</span><span class="sxs-lookup"><span data-stu-id="dcff0-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="dcff0-123">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-123">User management admin</span></span>   | <span data-ttu-id="dcff0-124">• Visualizzare, creare e gestire gli utenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="dcff0-125">• Visualizzare tutti i profili partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-125">• View all partner profiles</span></span>
||<span data-ttu-id="dcff0-126">• Visualizzare, creare e gestire gli utenti partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="dcff0-127">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="dcff0-127">Billing admin</span></span> | <span data-ttu-id="dcff0-128">-Visualizzare, creare e gestire la fatturazione, fatture e i file di riconoscimento</span><span class="sxs-lookup"><span data-stu-id="dcff0-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="dcff0-129">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="dcff0-129">Default user</span></span>|  <span data-ttu-id="dcff0-130">Visualizza profilo personale</span><span class="sxs-lookup"><span data-stu-id="dcff0-130">View My profile</span></span>   |
|<span data-ttu-id="dcff0-131">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="dcff0-131">Admin agent</span></span> | <span data-ttu-id="dcff0-132">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="dcff0-132">•    Customer management</span></span>
||<span data-ttu-id="dcff0-133">• Aggiungere l'elenco dei dispositivi al centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="dcff0-134">• Creare e applicare i profili nei dispositivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="dcff0-135">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="dcff0-135">• Subscription management</span></span>
||<span data-ttu-id="dcff0-136">• Servizio integrità e soddisfare richieste per i clienti</span><span class="sxs-lookup"><span data-stu-id="dcff0-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="dcff0-137">• Richiesta delegati i privilegi di amministratore</span><span class="sxs-lookup"><span data-stu-id="dcff0-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="dcff0-138">• Visualizza i prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="dcff0-138">• View pricing and offers</span></span>
||<span data-ttu-id="dcff0-139">• La fatturazione</span><span class="sxs-lookup"><span data-stu-id="dcff0-139">• Billing</span></span>
||<span data-ttu-id="dcff0-140">• Amministra per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="dcff0-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="dcff0-141">• Registra un valore aggiunto rivenditore</span><span class="sxs-lookup"><span data-stu-id="dcff0-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="dcff0-142">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="dcff0-142">Sales agent</span></span> | <span data-ttu-id="dcff0-143">• Gestione con i clienti</span><span class="sxs-lookup"><span data-stu-id="dcff0-143">•    Customer management</span></span>
||<span data-ttu-id="dcff0-144">• Aggiungere l'elenco dei dispositivi al centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="dcff0-145">• Gestione delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="dcff0-145">• Subscription management</span></span>
||<span data-ttu-id="dcff0-146">• Visualizzare prezzi sono elencati e offre</span><span class="sxs-lookup"><span data-stu-id="dcff0-146">• View price lists and offers</span></span>
||<span data-ttu-id="dcff0-147">Ticket di supporto di visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="dcff0-147">• View support tickets</span></span>
||<span data-ttu-id="dcff0-148">• Richiesta una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="dcff0-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="dcff0-149">• Gestire i lead dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcff0-149">• Manage customer leads</span></span>
||<span data-ttu-id="dcff0-150">• Visualizzare il contratto del cliente</span><span class="sxs-lookup"><span data-stu-id="dcff0-150">• View the customer agreement</span></span>
||<span data-ttu-id="dcff0-151">• Registro un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="dcff0-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="dcff0-152">Agente help desk</span><span class="sxs-lookup"><span data-stu-id="dcff0-152">Helpdesk agent</span></span>| <span data-ttu-id="dcff0-153">• Cercare e visualizzare un cliente</span><span class="sxs-lookup"><span data-stu-id="dcff0-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="dcff0-154">• Modificare i dettagli cliente</span><span class="sxs-lookup"><span data-stu-id="dcff0-154">• Edit customer details</span></span>
||<span data-ttu-id="dcff0-155">• Guida risolvere cliente i problemi con la gestione di fatturazione o alla sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="dcff0-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="dcff0-156">• Richiedere il supporto per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="dcff0-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="dcff0-157">• Gestire le sottoscrizioni e fatturazione problemi per conto dei clienti (Nota: È necessario essere un agente di amministratore per completare questa attività per le sottoscrizioni di Office 365)</span><span class="sxs-lookup"><span data-stu-id="dcff0-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="dcff0-158">Fornitore del Pannello di controllo (CPV).</span><span class="sxs-lookup"><span data-stu-id="dcff0-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="dcff0-159">(Non-AAD ruolo e ruolo CSP)</span><span class="sxs-lookup"><span data-stu-id="dcff0-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="dcff0-160">CPVs lo sviluppo di App per l'uso da partner Cloud Solution Provider (CSP) per consentire loro di integrare i sistemi con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="dcff0-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="dcff0-161">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcff0-161">**Role**</span></span>   |<span data-ttu-id="dcff0-162">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="dcff0-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="dcff0-163">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="dcff0-163">Global admin</span></span>| <span data-ttu-id="dcff0-164">Visualizzare e gestire il profilo CPV</span><span class="sxs-lookup"><span data-stu-id="dcff0-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="dcff0-165">Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV</span><span class="sxs-lookup"><span data-stu-id="dcff0-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="dcff0-166">Utente guest (devono essere aggiunti al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="dcff0-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="dcff0-167">**Utente Guest**</span><span class="sxs-lookup"><span data-stu-id="dcff0-167">**Guest user**</span></span>   | <span data-ttu-id="dcff0-168">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="dcff0-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="dcff0-169">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="dcff0-169">MPN partner admin</span></span>|
||<span data-ttu-id="dcff0-170">Gli account amministratore</span><span class="sxs-lookup"><span data-stu-id="dcff0-170">Accounts admin</span></span>|
||<span data-ttu-id="dcff0-171">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-171">Incentives admin</span></span>|
||<span data-ttu-id="dcff0-172">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="dcff0-172">Business profile admin</span></span>|
||<span data-ttu-id="dcff0-173">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="dcff0-174">Gestire l'appartenenza MPN e la propria azienda (ruoli non AAD: questi ruoli di gestire attività aziendale anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="dcff0-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="dcff0-175">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcff0-175">**Role**</span></span> | <span data-ttu-id="dcff0-176">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="dcff0-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="dcff0-177">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="dcff0-177">MPN partner admin</span></span>|<span data-ttu-id="dcff0-178">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="dcff0-179">• Vista legale, aziendale, business e i profili MPN</span><span class="sxs-lookup"><span data-stu-id="dcff0-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="dcff0-180">• Visualizzare i dettagli di utente e i relativi dati di competenze</span><span class="sxs-lookup"><span data-stu-id="dcff0-180">• View user details and their skills data</span></span>
||<span data-ttu-id="dcff0-181">• Visualizza competenze</span><span class="sxs-lookup"><span data-stu-id="dcff0-181">• View competencies</span></span>
||<span data-ttu-id="dcff0-182">• Visualizzare e gestire i vantaggi</span><span class="sxs-lookup"><span data-stu-id="dcff0-182">• View and manage benefits</span></span>
||<span data-ttu-id="dcff0-183">Acquisto e la visualizzazione • ottenuta MPN</span><span class="sxs-lookup"><span data-stu-id="dcff0-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="dcff0-184">• Visualizzare MPN offre le fatture e cronologia degli ordini</span><span class="sxs-lookup"><span data-stu-id="dcff0-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="dcff0-185">• Visualizza partner contributo indicatori dati</span><span class="sxs-lookup"><span data-stu-id="dcff0-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="dcff0-186">• Possono utilizzare lo strumento di convalida Voucher</span><span class="sxs-lookup"><span data-stu-id="dcff0-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="dcff0-187">-Visualizzare analitica dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcff0-187">- View customer data analytics</span></span>
|| <span data-ttu-id="dcff0-188">Visualizzare altri ruoli utente all'interno della società, ma non è possibile assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="dcff0-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="dcff0-189">Amministratore account</span><span class="sxs-lookup"><span data-stu-id="dcff0-189">Account admin</span></span>| <span data-ttu-id="dcff0-190">Aggiungere percorsi</span><span class="sxs-lookup"><span data-stu-id="dcff0-190">Add locations</span></span>
|| <span data-ttu-id="dcff0-191">Gestire i profili relativi agli account di per che amministratore</span><span class="sxs-lookup"><span data-stu-id="dcff0-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="dcff0-192">• Assegnare ruoli per gli utenti nel tenant per i ruoli AAD non</span><span class="sxs-lookup"><span data-stu-id="dcff0-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="dcff0-193">• Percorsi nei programmi di registrazione</span><span class="sxs-lookup"><span data-stu-id="dcff0-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="dcff0-194">Gestire i riferimenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-194">Manage referrals</span></span> 

|<span data-ttu-id="dcff0-195">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcff0-195">**Role**</span></span>|<span data-ttu-id="dcff0-196">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="dcff0-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="dcff0-197">Amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-197">Referrals admin</span></span>       |<span data-ttu-id="dcff0-198">• Visualizzare, creare e gestire i profili di business</span><span class="sxs-lookup"><span data-stu-id="dcff0-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="dcff0-199">• Ricevere e gestire i riferimenti</span><span class="sxs-lookup"><span data-stu-id="dcff0-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="dcff0-200">• Visualizzare, creare e gestire le segnalazioni di CO-Selling</span><span class="sxs-lookup"><span data-stu-id="dcff0-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="dcff0-201">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="dcff0-202">Amministratore profilo di lavoro</span><span class="sxs-lookup"><span data-stu-id="dcff0-202">Business profile admin</span></span>   |<span data-ttu-id="dcff0-203">• Visualizzare, creare e gestire il profilo di business</span><span class="sxs-lookup"><span data-stu-id="dcff0-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="dcff0-204">• Visualizzare, creare e gestire le richieste di servizio partner</span><span class="sxs-lookup"><span data-stu-id="dcff0-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="dcff0-205">Gestire gli incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-205">Manage incentives</span></span> 

|<span data-ttu-id="dcff0-206">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcff0-206">**Role**</span></span> | <span data-ttu-id="dcff0-207">**Operazioni possibili**</span><span class="sxs-lookup"><span data-stu-id="dcff0-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="dcff0-208">Amministratore di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-208">Incentives admin</span></span>|<span data-ttu-id="dcff0-209">• Avvia e gestisce gli incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="dcff0-210">• È possibile visualizzare e modificare tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="dcff0-211">• È possibile visualizzare e modificare i dettagli fiscali e bancarie</span><span class="sxs-lookup"><span data-stu-id="dcff0-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="dcff0-212">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="dcff0-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="dcff0-213">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="dcff0-213">• Access support</span></span>
||<span data-ttu-id="dcff0-214">Pagamenti di incentivi controversia •</span><span class="sxs-lookup"><span data-stu-id="dcff0-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="dcff0-215">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-215">Incentives user</span></span>|<span data-ttu-id="dcff0-216">• Consente di visualizzare i programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="dcff0-217">• È possibile visualizzare e avviare le attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcff0-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="dcff0-218">Utili sugli sconti e cooperativa visualizzazione •</span><span class="sxs-lookup"><span data-stu-id="dcff0-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="dcff0-219">• Supporto dell'accesso</span><span class="sxs-lookup"><span data-stu-id="dcff0-219">• Access support</span></span>












