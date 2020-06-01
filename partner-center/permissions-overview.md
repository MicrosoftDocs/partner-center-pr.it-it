---
title: Assegnare ruoli e autorizzazioni agli utenti
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri quali sono i ruoli più adatti per gli utenti della tua azienda che gestiscono transazioni commerciali, segnalazioni, incentivi o adesioni MPN nel Centro per i partner.
author: LauraBrenner
ms.author: labrenne
keywords: ruoli, autorizzazioni, amministratore, agente
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 0858340c6965ac932f0d4694f6f21be89ca5f817
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795880"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="946fa-104">Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="946fa-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="946fa-105">**Appropriate roles**</span></span>

- <span data-ttu-id="946fa-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="946fa-106">Global admin</span></span>
- <span data-ttu-id="946fa-107">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="946fa-107">User admin</span></span>
- <span data-ttu-id="946fa-108">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-108">MPN partner admin</span></span>

<span data-ttu-id="946fa-109">Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda.</span><span class="sxs-lookup"><span data-stu-id="946fa-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="946fa-110">Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="946fa-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="946fa-111">Configurare i dipendenti in modo che possano lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="946fa-112">Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici.</span><span class="sxs-lookup"><span data-stu-id="946fa-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="946fa-113">I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda.</span><span class="sxs-lookup"><span data-stu-id="946fa-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="946fa-114">Ad esempio, se si tratta di un'azienda CSP (Cloud Solution Provider), non solo avrai i ruoli di gestione del tenant di Azure AD standard (tra cui il ruolo di amministratore globale), ma avrai bisogno anche di ruoli specifici del programma CSP.</span><span class="sxs-lookup"><span data-stu-id="946fa-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="946fa-115">Ogni programma prevede ruoli specifici.</span><span class="sxs-lookup"><span data-stu-id="946fa-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="946fa-116">I ruoli relativi al tenant di Azure Active Directory (AAD) includono l'amministratore globale, l'amministratore utenti e i ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="946fa-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="946fa-117">I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente di incentivi.</span><span class="sxs-lookup"><span data-stu-id="946fa-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="946fa-118">Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="946fa-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="946fa-119">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-119">**Role**</span></span>|<span data-ttu-id="946fa-120">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="946fa-121">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="946fa-121">Global admin</span></span>|<span data-ttu-id="946fa-122">\*    Accesso a tutti gli account/servizi Microsoft con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="946fa-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="946fa-123">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="946fa-124">\*    Visualizzazione di contratti, listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="946fa-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="946fa-125">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="946fa-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="946fa-126">Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="946fa-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="946fa-127">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="946fa-127">User management admin</span></span>   | <span data-ttu-id="946fa-128">\*    Visualizzazione, creazione e gestione di utenti</span><span class="sxs-lookup"><span data-stu-id="946fa-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="946fa-129">\*    Visualizzazione di tutti i profili dei partner</span><span class="sxs-lookup"><span data-stu-id="946fa-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="946fa-130">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="946fa-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="946fa-131">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="946fa-131">Billing admin</span></span> | <span data-ttu-id="946fa-132">- Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="946fa-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="946fa-133">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="946fa-133">Default user</span></span>|  <span data-ttu-id="946fa-134">Visualizzazione del profilo personale</span><span class="sxs-lookup"><span data-stu-id="946fa-134">View My profile</span></span>   |
|<span data-ttu-id="946fa-135">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="946fa-135">Admin agent</span></span> | <span data-ttu-id="946fa-136">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-136">\*    Customer management</span></span>
||<span data-ttu-id="946fa-137">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="946fa-138">\*    Creazione e applicazione di profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="946fa-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="946fa-139">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="946fa-139">\*    Subscription management</span></span>
||<span data-ttu-id="946fa-140">\*    Integrità del servizio e richieste di servizio per i clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="946fa-141">\*    Richiesta dei privilegi di amministratore con delega</span><span class="sxs-lookup"><span data-stu-id="946fa-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="946fa-142">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="946fa-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="946fa-143">\*    Fatturazione</span><span class="sxs-lookup"><span data-stu-id="946fa-143">\*    Billing</span></span>
||<span data-ttu-id="946fa-144">\*    Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="946fa-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="946fa-145">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="946fa-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="946fa-146">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="946fa-146">Sales agent</span></span> | <span data-ttu-id="946fa-147">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-147">\*    Customer management</span></span>
||<span data-ttu-id="946fa-148">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="946fa-149">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="946fa-149">\*    Subscription management</span></span>
||<span data-ttu-id="946fa-150">\*    Visualizzazione dei ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="946fa-150">\*    View support tickets</span></span>
||<span data-ttu-id="946fa-151">\*    Richiesta di una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="946fa-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="946fa-152">\*    Gestione dei clienti potenziali</span><span class="sxs-lookup"><span data-stu-id="946fa-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="946fa-153">\*    Visualizzazione del contratto per il cliente</span><span class="sxs-lookup"><span data-stu-id="946fa-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="946fa-154">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="946fa-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="946fa-155">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="946fa-155">Helpdesk agent</span></span>| <span data-ttu-id="946fa-156">\*    Ricerca e visualizzazione di un cliente</span><span class="sxs-lookup"><span data-stu-id="946fa-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="946fa-157">\*    Modifica dei dettagli dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-157">\*    Edit customer details</span></span>
||<span data-ttu-id="946fa-158">\*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti</span><span class="sxs-lookup"><span data-stu-id="946fa-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="946fa-159">\*    Richiesta di supporto per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="946fa-160">\*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="946fa-161">Fornitore del pannello di controllo (CPV)</span><span class="sxs-lookup"><span data-stu-id="946fa-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="946fa-162">(ruolo CSP e ruolo non AAD)</span><span class="sxs-lookup"><span data-stu-id="946fa-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="946fa-163">I CPV sviluppano app destinate ai partner CSP (Cloud Solution Provider) affinché possano integrare i loro sistemi con le API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="946fa-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="946fa-164">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-164">**Role**</span></span>   |<span data-ttu-id="946fa-165">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="946fa-166">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="946fa-166">Global admin</span></span>| <span data-ttu-id="946fa-167">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="946fa-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="946fa-168">Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="946fa-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="946fa-169">Utente guest (deve essere aggiunto al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="946fa-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="946fa-170">**Utente guest**</span><span class="sxs-lookup"><span data-stu-id="946fa-170">**Guest user**</span></span>   | <span data-ttu-id="946fa-171">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="946fa-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="946fa-172">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-172">MPN partner admin</span></span>|
||<span data-ttu-id="946fa-173">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="946fa-173">Accounts admin</span></span>|
||<span data-ttu-id="946fa-174">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-174">Incentives admin</span></span>|
||<span data-ttu-id="946fa-175">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="946fa-175">Business profile admin</span></span>|
||<span data-ttu-id="946fa-176">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="946fa-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="946fa-177">Gestione dell'appartenenza a MPN e dell'azienda (ruoli non AAD: questi ruoli gestiscono l'attività dell'azienda anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="946fa-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="946fa-178">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-178">**Role**</span></span> | <span data-ttu-id="946fa-179">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="946fa-180">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-180">MPN partner admin</span></span>|<span data-ttu-id="946fa-181">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="946fa-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="946fa-182">\*    Visualizzazione di profili legali, aziendali, commerciali e MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="946fa-183">\*    Visualizzazione dei dettagli dell'utente e dei relativi dati delle competenze</span><span class="sxs-lookup"><span data-stu-id="946fa-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="946fa-184">\*    Visualizzazione delle competenze</span><span class="sxs-lookup"><span data-stu-id="946fa-184">\*    View competencies</span></span>
||<span data-ttu-id="946fa-185">\*    Visualizzazione e gestione dei vantaggi</span><span class="sxs-lookup"><span data-stu-id="946fa-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="946fa-186">\*    Visualizzazione e acquisto di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="946fa-187">\*    Visualizzazione di fatture e cronologia degli ordini di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="946fa-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="946fa-188">\*    Visualizzazione dei dati degli indicatori di contributi dei partner</span><span class="sxs-lookup"><span data-stu-id="946fa-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="946fa-189">\*    Uso dello strumento di convalida dei giustificativi</span><span class="sxs-lookup"><span data-stu-id="946fa-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="946fa-190">\*    Visualizzazione dell'analisi dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="946fa-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="946fa-191">\*    Visualizzazione di altri ruoli utente all'interno dell'azienda, senza la possibilità di assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="946fa-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="946fa-192">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="946fa-192">Account admin</span></span>| <span data-ttu-id="946fa-193">Aggiunta di posizioni</span><span class="sxs-lookup"><span data-stu-id="946fa-193">Add locations</span></span>
|| <span data-ttu-id="946fa-194">Gestione di profili relativi agli account amministrati</span><span class="sxs-lookup"><span data-stu-id="946fa-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="946fa-195">\*    Assegnazione di ruoli per gli utenti nel tenant a ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="946fa-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="946fa-196">\*    Registrazione di posizioni nei programmi</span><span class="sxs-lookup"><span data-stu-id="946fa-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="946fa-197">Gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="946fa-197">Manage referrals</span></span> 

|<span data-ttu-id="946fa-198">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-198">**Role**</span></span>|<span data-ttu-id="946fa-199">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="946fa-200">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="946fa-200">Referrals admin</span></span>       |<span data-ttu-id="946fa-201">\*    Visualizzazione, creazione e gestione dei profili di business</span><span class="sxs-lookup"><span data-stu-id="946fa-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="946fa-202">\*    Ricezione e gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="946fa-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="946fa-203">\*    Visualizzazione, creazione e gestione delle segnalazioni di co-selling</span><span class="sxs-lookup"><span data-stu-id="946fa-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="946fa-204">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="946fa-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="946fa-205">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="946fa-205">Business profile admin</span></span>   |<span data-ttu-id="946fa-206">\*    Visualizzazione, creazione e gestione del profilo di business</span><span class="sxs-lookup"><span data-stu-id="946fa-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="946fa-207">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="946fa-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="946fa-208">Gestione degli incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-208">Manage incentives</span></span> 

|<span data-ttu-id="946fa-209">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-209">**Role**</span></span> | <span data-ttu-id="946fa-210">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="946fa-211">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-211">Incentives admin</span></span>|<span data-ttu-id="946fa-212">\*    Avvio e gestione di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="946fa-213">\*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="946fa-214">\*    Visualizzazione e modifica dei dettagli bancari e fiscali</span><span class="sxs-lookup"><span data-stu-id="946fa-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="946fa-215">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="946fa-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="946fa-216">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="946fa-216">\*    Access support</span></span>
||<span data-ttu-id="946fa-217">\*    Controversie sui pagamenti di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="946fa-218">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-218">Incentives user</span></span>|<span data-ttu-id="946fa-219">\*    Visualizzazione di programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="946fa-220">\*    Visualizzazione e avvio di attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="946fa-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="946fa-221">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="946fa-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="946fa-222">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="946fa-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="946fa-223">Visualizzare i dati di Insights del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="946fa-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="946fa-224">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="946fa-224">**Role**</span></span> | <span data-ttu-id="946fa-225">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="946fa-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="946fa-226">Visualizzatore di report esecutivi</span><span class="sxs-lookup"><span data-stu-id="946fa-226">Executive report viewer</span></span>|<span data-ttu-id="946fa-227">Accedere a tutti i set di dati di reporting</span><span class="sxs-lookup"><span data-stu-id="946fa-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="946fa-228">Visualizzatore di report</span><span class="sxs-lookup"><span data-stu-id="946fa-228">Report viewer</span></span>|<span data-ttu-id="946fa-229">Accedere ai report di dati, ad eccezione dei ricavi e dei dati personali di clienti e dipendenti</span><span class="sxs-lookup"><span data-stu-id="946fa-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    