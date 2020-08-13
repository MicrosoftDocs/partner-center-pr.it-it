---
title: Assegnare ruoli e autorizzazioni agli utenti
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri quali sono i ruoli più adatti per gli utenti della tua azienda che gestiscono transazioni commerciali, segnalazioni, incentivi o adesioni MPN nel Centro per i partner.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839186"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="dcb73-103">Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="dcb73-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="dcb73-104">**Appropriate roles**</span></span>

- <span data-ttu-id="dcb73-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="dcb73-105">Global admin</span></span>
- <span data-ttu-id="dcb73-106">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-106">User admin</span></span>
- <span data-ttu-id="dcb73-107">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-107">MPN partner admin</span></span>

<span data-ttu-id="dcb73-108">Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda.</span><span class="sxs-lookup"><span data-stu-id="dcb73-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="dcb73-109">Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dcb73-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="dcb73-110">Configurare i dipendenti in modo che possano lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="dcb73-111">Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici.</span><span class="sxs-lookup"><span data-stu-id="dcb73-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="dcb73-112">I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda.</span><span class="sxs-lookup"><span data-stu-id="dcb73-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="dcb73-113">Ad esempio, se si tratta di un'azienda CSP (Cloud Solution Provider), non solo avrai i ruoli di gestione del tenant di Azure AD standard (tra cui il ruolo di amministratore globale), ma avrai bisogno anche di ruoli specifici del programma CSP.</span><span class="sxs-lookup"><span data-stu-id="dcb73-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="dcb73-114">Ogni programma prevede ruoli specifici.</span><span class="sxs-lookup"><span data-stu-id="dcb73-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="dcb73-115">I ruoli relativi al tenant di Azure Active Directory (AAD) includono l'amministratore globale, l'amministratore utenti e i ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="dcb73-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="dcb73-116">I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente di incentivi.</span><span class="sxs-lookup"><span data-stu-id="dcb73-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="dcb73-117">Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="dcb73-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="dcb73-118">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-118">**Role**</span></span>|<span data-ttu-id="dcb73-119">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="dcb73-120">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="dcb73-120">Global admin</span></span>|<span data-ttu-id="dcb73-121">\*    Accesso a tutti gli account/servizi Microsoft con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="dcb73-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="dcb73-122">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="dcb73-123">\*    Visualizzazione di contratti, listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="dcb73-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="dcb73-124">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="dcb73-125">Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="dcb73-126">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-126">User management admin</span></span>   | <span data-ttu-id="dcb73-127">\*    Visualizzazione, creazione e gestione di utenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="dcb73-128">\*    Visualizzazione di tutti i profili dei partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="dcb73-129">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="dcb73-130">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-130">Billing admin</span></span> | <span data-ttu-id="dcb73-131">- Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="dcb73-132">\*    Visualizzazione dei prezzi</span><span class="sxs-lookup"><span data-stu-id="dcb73-132">\*    View pricing</span></span>
|<span data-ttu-id="dcb73-133">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="dcb73-133">Default user</span></span>|  <span data-ttu-id="dcb73-134">Visualizzazione del profilo personale</span><span class="sxs-lookup"><span data-stu-id="dcb73-134">View My profile</span></span>   |
|<span data-ttu-id="dcb73-135">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="dcb73-135">Admin agent</span></span> | <span data-ttu-id="dcb73-136">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-136">\*    Customer management</span></span>
||<span data-ttu-id="dcb73-137">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="dcb73-138">\*    Creazione e applicazione di profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="dcb73-139">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-139">\*    Subscription management</span></span>
||<span data-ttu-id="dcb73-140">\*    Integrità del servizio e richieste di servizio per i clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="dcb73-141">\*    Richiesta dei privilegi di amministratore con delega</span><span class="sxs-lookup"><span data-stu-id="dcb73-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="dcb73-142">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="dcb73-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="dcb73-143">\*    Fatturazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-143">\*    Billing</span></span>
||<span data-ttu-id="dcb73-144">\*    Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="dcb73-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="dcb73-145">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="dcb73-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="dcb73-146">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="dcb73-146">Sales agent</span></span> | <span data-ttu-id="dcb73-147">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-147">\*    Customer management</span></span>
||<span data-ttu-id="dcb73-148">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="dcb73-149">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-149">\*    Subscription management</span></span>
||<span data-ttu-id="dcb73-150">\*    Visualizzazione dei ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="dcb73-150">\*    View support tickets</span></span>
||<span data-ttu-id="dcb73-151">\*    Richiesta di una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="dcb73-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="dcb73-152">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="dcb73-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="dcb73-153">\*    Gestione dei clienti potenziali</span><span class="sxs-lookup"><span data-stu-id="dcb73-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="dcb73-154">\*    Visualizzazione del contratto per il cliente</span><span class="sxs-lookup"><span data-stu-id="dcb73-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="dcb73-155">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="dcb73-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="dcb73-156">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="dcb73-156">Helpdesk agent</span></span>| <span data-ttu-id="dcb73-157">\*    Ricerca e visualizzazione di un cliente</span><span class="sxs-lookup"><span data-stu-id="dcb73-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="dcb73-158">\*    Modifica dei dettagli dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-158">\*    Edit customer details</span></span>
||<span data-ttu-id="dcb73-159">\*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="dcb73-160">\*    Richiesta di supporto per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="dcb73-161">\*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="dcb73-162">Fornitore del pannello di controllo (CPV)</span><span class="sxs-lookup"><span data-stu-id="dcb73-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="dcb73-163">(ruolo CSP e ruolo non AAD)</span><span class="sxs-lookup"><span data-stu-id="dcb73-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="dcb73-164">I CPV sviluppano app destinate ai partner CSP (Cloud Solution Provider) affinché possano integrare i loro sistemi con le API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dcb73-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="dcb73-165">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-165">**Role**</span></span>   |<span data-ttu-id="dcb73-166">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="dcb73-167">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="dcb73-167">Global admin</span></span>| <span data-ttu-id="dcb73-168">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="dcb73-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="dcb73-169">Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="dcb73-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="dcb73-170">Utente guest (deve essere aggiunto al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="dcb73-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="dcb73-171">**Utente guest**</span><span class="sxs-lookup"><span data-stu-id="dcb73-171">**Guest user**</span></span>   | <span data-ttu-id="dcb73-172">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="dcb73-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="dcb73-173">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-173">MPN partner admin</span></span>|
||<span data-ttu-id="dcb73-174">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="dcb73-174">Accounts admin</span></span>|
||<span data-ttu-id="dcb73-175">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-175">Incentives admin</span></span>|
||<span data-ttu-id="dcb73-176">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="dcb73-176">Business profile admin</span></span>|
||<span data-ttu-id="dcb73-177">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="dcb73-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="dcb73-178">Gestione dell'appartenenza a MPN e dell'azienda (ruoli non AAD: questi ruoli gestiscono l'attività dell'azienda anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="dcb73-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="dcb73-179">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-179">**Role**</span></span> | <span data-ttu-id="dcb73-180">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="dcb73-181">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-181">MPN partner admin</span></span>|<span data-ttu-id="dcb73-182">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="dcb73-183">\*    Visualizzazione di profili legali, aziendali, commerciali e MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="dcb73-184">\*    Visualizzazione dei dettagli dell'utente e dei relativi dati delle competenze</span><span class="sxs-lookup"><span data-stu-id="dcb73-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="dcb73-185">\*    Visualizzazione delle competenze</span><span class="sxs-lookup"><span data-stu-id="dcb73-185">\*    View competencies</span></span>
||<span data-ttu-id="dcb73-186">\*    Visualizzazione e gestione dei vantaggi</span><span class="sxs-lookup"><span data-stu-id="dcb73-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="dcb73-187">\*    Visualizzazione e acquisto di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="dcb73-188">\*    Visualizzazione di fatture e cronologia degli ordini di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="dcb73-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="dcb73-189">\*    Visualizzazione dei dati degli indicatori di contributi dei partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="dcb73-190">\*    Uso dello strumento di convalida dei giustificativi</span><span class="sxs-lookup"><span data-stu-id="dcb73-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="dcb73-191">\*    Visualizzazione dell'analisi dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="dcb73-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="dcb73-192">\*    Visualizzazione di altri ruoli utente all'interno dell'azienda, senza la possibilità di assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="dcb73-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="dcb73-193">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="dcb73-193">Account admin</span></span>| <span data-ttu-id="dcb73-194">Aggiunta di posizioni</span><span class="sxs-lookup"><span data-stu-id="dcb73-194">Add locations</span></span>
|| <span data-ttu-id="dcb73-195">Gestione di profili relativi agli account amministrati</span><span class="sxs-lookup"><span data-stu-id="dcb73-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="dcb73-196">\*    Assegnazione di ruoli per gli utenti nel tenant a ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="dcb73-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="dcb73-197">\*    Registrazione di posizioni nei programmi</span><span class="sxs-lookup"><span data-stu-id="dcb73-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="dcb73-198">Gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="dcb73-198">Manage referrals</span></span> 

|<span data-ttu-id="dcb73-199">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-199">**Role**</span></span>|<span data-ttu-id="dcb73-200">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="dcb73-201">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="dcb73-201">Referrals admin</span></span>       |<span data-ttu-id="dcb73-202">\*    Visualizzazione, creazione e gestione dei profili di business</span><span class="sxs-lookup"><span data-stu-id="dcb73-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="dcb73-203">\*    Ricezione e gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="dcb73-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="dcb73-204">\*    Visualizzazione, creazione e gestione delle segnalazioni di co-selling</span><span class="sxs-lookup"><span data-stu-id="dcb73-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="dcb73-205">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="dcb73-206">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="dcb73-206">Business profile admin</span></span>   |<span data-ttu-id="dcb73-207">\*    Visualizzazione, creazione e gestione del profilo di business</span><span class="sxs-lookup"><span data-stu-id="dcb73-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="dcb73-208">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="dcb73-209">Gestione degli incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-209">Manage incentives</span></span> 

|<span data-ttu-id="dcb73-210">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-210">**Role**</span></span> | <span data-ttu-id="dcb73-211">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="dcb73-212">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-212">Incentives admin</span></span>|<span data-ttu-id="dcb73-213">\*    Avvio e gestione di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="dcb73-214">\*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="dcb73-215">\*    Visualizzazione e modifica dei dettagli bancari e fiscali</span><span class="sxs-lookup"><span data-stu-id="dcb73-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="dcb73-216">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="dcb73-217">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="dcb73-217">\*    Access support</span></span>
||<span data-ttu-id="dcb73-218">\*    Controversie sui pagamenti di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="dcb73-219">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-219">Incentives user</span></span>|<span data-ttu-id="dcb73-220">\*    Visualizzazione di programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="dcb73-221">\*    Visualizzazione e avvio di attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="dcb73-222">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="dcb73-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="dcb73-223">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="dcb73-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="dcb73-224">Visualizzare i dati di Insights del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dcb73-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="dcb73-225">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="dcb73-225">**Role**</span></span> | <span data-ttu-id="dcb73-226">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="dcb73-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="dcb73-227">Visualizzatore di report esecutivi</span><span class="sxs-lookup"><span data-stu-id="dcb73-227">Executive report viewer</span></span>|<span data-ttu-id="dcb73-228">Accedere a tutti i set di dati di reporting</span><span class="sxs-lookup"><span data-stu-id="dcb73-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="dcb73-229">Visualizzatore di report</span><span class="sxs-lookup"><span data-stu-id="dcb73-229">Report viewer</span></span>|<span data-ttu-id="dcb73-230">Accedere ai report di dati, ad eccezione dei ricavi e dei dati personali di clienti e dipendenti</span><span class="sxs-lookup"><span data-stu-id="dcb73-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
