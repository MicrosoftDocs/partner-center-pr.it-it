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
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434320"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="9e1d6-103">Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="9e1d6-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9e1d6-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9e1d6-105">Global admin</span></span>
- <span data-ttu-id="9e1d6-106">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-106">User admin</span></span>
- <span data-ttu-id="9e1d6-107">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-107">MPN partner admin</span></span>

<span data-ttu-id="9e1d6-108">Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="9e1d6-109">Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="9e1d6-110">Configurare i dipendenti in modo che possano lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="9e1d6-111">Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="9e1d6-112">I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="9e1d6-113">Ad esempio, se si tratta di un'azienda CSP (Cloud Solution Provider), non solo avrai i ruoli di gestione del tenant di Azure AD standard (tra cui il ruolo di amministratore globale), ma avrai bisogno anche di ruoli specifici del programma CSP.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="9e1d6-114">Ogni programma prevede ruoli specifici.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="9e1d6-115">I ruoli relativi al tenant di Azure Active Directory (AAD) includono l'amministratore globale, l'amministratore utenti e i ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="9e1d6-116">I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente di incentivi.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="9e1d6-117">Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="9e1d6-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="9e1d6-118">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-118">**Role**</span></span>|<span data-ttu-id="9e1d6-119">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="9e1d6-120">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9e1d6-120">Global admin</span></span>|<span data-ttu-id="9e1d6-121">\*    Accesso a tutti gli account/servizi Microsoft con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="9e1d6-122">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="9e1d6-123">\*    Visualizzazione di contratti, listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="9e1d6-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="9e1d6-124">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="9e1d6-125">Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="9e1d6-126">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-126">User management admin</span></span>   | <span data-ttu-id="9e1d6-127">\*    Visualizzazione, creazione e gestione di utenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="9e1d6-128">\*    Visualizzazione di tutti i profili dei partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="9e1d6-129">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="9e1d6-130">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-130">Billing admin</span></span> | <span data-ttu-id="9e1d6-131">- Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="9e1d6-132">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="9e1d6-132">Default user</span></span>|  <span data-ttu-id="9e1d6-133">Visualizzazione del profilo personale</span><span class="sxs-lookup"><span data-stu-id="9e1d6-133">View My profile</span></span>   |
|<span data-ttu-id="9e1d6-134">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="9e1d6-134">Admin agent</span></span> | <span data-ttu-id="9e1d6-135">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-135">\*    Customer management</span></span>
||<span data-ttu-id="9e1d6-136">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="9e1d6-137">\*    Creazione e applicazione di profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="9e1d6-138">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-138">\*    Subscription management</span></span>
||<span data-ttu-id="9e1d6-139">\*    Integrità del servizio e richieste di servizio per i clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="9e1d6-140">\*    Richiesta dei privilegi di amministratore con delega</span><span class="sxs-lookup"><span data-stu-id="9e1d6-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="9e1d6-141">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="9e1d6-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="9e1d6-142">\*    Fatturazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-142">\*    Billing</span></span>
||<span data-ttu-id="9e1d6-143">\*    Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="9e1d6-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="9e1d6-144">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="9e1d6-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="9e1d6-145">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="9e1d6-145">Sales agent</span></span> | <span data-ttu-id="9e1d6-146">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-146">\*    Customer management</span></span>
||<span data-ttu-id="9e1d6-147">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="9e1d6-148">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-148">\*    Subscription management</span></span>
||<span data-ttu-id="9e1d6-149">\*    Visualizzazione dei ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="9e1d6-149">\*    View support tickets</span></span>
||<span data-ttu-id="9e1d6-150">\*    Richiesta di una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="9e1d6-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="9e1d6-151">\*    Gestione dei clienti potenziali</span><span class="sxs-lookup"><span data-stu-id="9e1d6-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="9e1d6-152">\*    Visualizzazione del contratto per il cliente</span><span class="sxs-lookup"><span data-stu-id="9e1d6-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="9e1d6-153">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="9e1d6-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="9e1d6-154">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="9e1d6-154">Helpdesk agent</span></span>| <span data-ttu-id="9e1d6-155">\*    Ricerca e visualizzazione di un cliente</span><span class="sxs-lookup"><span data-stu-id="9e1d6-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="9e1d6-156">\*    Modifica dei dettagli dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-156">\*    Edit customer details</span></span>
||<span data-ttu-id="9e1d6-157">\*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="9e1d6-158">\*    Richiesta di supporto per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="9e1d6-159">\*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="9e1d6-160">Fornitore del pannello di controllo (CPV)</span><span class="sxs-lookup"><span data-stu-id="9e1d6-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="9e1d6-161">(ruolo CSP e ruolo non AAD)</span><span class="sxs-lookup"><span data-stu-id="9e1d6-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="9e1d6-162">I CPV sviluppano app destinate ai partner CSP (Cloud Solution Provider) affinché possano integrare i loro sistemi con le API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9e1d6-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="9e1d6-163">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-163">**Role**</span></span>   |<span data-ttu-id="9e1d6-164">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="9e1d6-165">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9e1d6-165">Global admin</span></span>| <span data-ttu-id="9e1d6-166">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="9e1d6-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="9e1d6-167">Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="9e1d6-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="9e1d6-168">Utente guest (deve essere aggiunto al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="9e1d6-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="9e1d6-169">**Utente guest**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-169">**Guest user**</span></span>   | <span data-ttu-id="9e1d6-170">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="9e1d6-171">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-171">MPN partner admin</span></span>|
||<span data-ttu-id="9e1d6-172">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="9e1d6-172">Accounts admin</span></span>|
||<span data-ttu-id="9e1d6-173">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-173">Incentives admin</span></span>|
||<span data-ttu-id="9e1d6-174">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="9e1d6-174">Business profile admin</span></span>|
||<span data-ttu-id="9e1d6-175">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="9e1d6-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="9e1d6-176">Gestione dell'appartenenza a MPN e dell'azienda (ruoli non AAD: questi ruoli gestiscono l'attività dell'azienda anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="9e1d6-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="9e1d6-177">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-177">**Role**</span></span> | <span data-ttu-id="9e1d6-178">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="9e1d6-179">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-179">MPN partner admin</span></span>|<span data-ttu-id="9e1d6-180">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="9e1d6-181">\*    Visualizzazione di profili legali, aziendali, commerciali e MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="9e1d6-182">\*    Visualizzazione dei dettagli dell'utente e dei relativi dati delle competenze</span><span class="sxs-lookup"><span data-stu-id="9e1d6-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="9e1d6-183">\*    Visualizzazione delle competenze</span><span class="sxs-lookup"><span data-stu-id="9e1d6-183">\*    View competencies</span></span>
||<span data-ttu-id="9e1d6-184">\*    Visualizzazione e gestione dei vantaggi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="9e1d6-185">\*    Visualizzazione e acquisto di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="9e1d6-186">\*    Visualizzazione di fatture e cronologia degli ordini di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="9e1d6-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="9e1d6-187">\*    Visualizzazione dei dati degli indicatori di contributi dei partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="9e1d6-188">\*    Uso dello strumento di convalida dei giustificativi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="9e1d6-189">\*    Visualizzazione dell'analisi dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="9e1d6-190">\*    Visualizzazione di altri ruoli utente all'interno dell'azienda, senza la possibilità di assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="9e1d6-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="9e1d6-191">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="9e1d6-191">Account admin</span></span>| <span data-ttu-id="9e1d6-192">Aggiunta di posizioni</span><span class="sxs-lookup"><span data-stu-id="9e1d6-192">Add locations</span></span>
|| <span data-ttu-id="9e1d6-193">Gestione di profili relativi agli account amministrati</span><span class="sxs-lookup"><span data-stu-id="9e1d6-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="9e1d6-194">\*    Assegnazione di ruoli per gli utenti nel tenant a ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="9e1d6-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="9e1d6-195">\*    Registrazione di posizioni nei programmi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="9e1d6-196">Gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="9e1d6-196">Manage referrals</span></span> 

|<span data-ttu-id="9e1d6-197">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-197">**Role**</span></span>|<span data-ttu-id="9e1d6-198">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="9e1d6-199">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="9e1d6-199">Referrals admin</span></span>       |<span data-ttu-id="9e1d6-200">\*    Visualizzazione, creazione e gestione dei profili di business</span><span class="sxs-lookup"><span data-stu-id="9e1d6-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="9e1d6-201">\*    Ricezione e gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="9e1d6-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="9e1d6-202">\*    Visualizzazione, creazione e gestione delle segnalazioni di co-selling</span><span class="sxs-lookup"><span data-stu-id="9e1d6-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="9e1d6-203">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="9e1d6-204">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="9e1d6-204">Business profile admin</span></span>   |<span data-ttu-id="9e1d6-205">\*    Visualizzazione, creazione e gestione del profilo di business</span><span class="sxs-lookup"><span data-stu-id="9e1d6-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="9e1d6-206">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="9e1d6-207">Gestione degli incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-207">Manage incentives</span></span> 

|<span data-ttu-id="9e1d6-208">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-208">**Role**</span></span> | <span data-ttu-id="9e1d6-209">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="9e1d6-210">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-210">Incentives admin</span></span>|<span data-ttu-id="9e1d6-211">\*    Avvio e gestione di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="9e1d6-212">\*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="9e1d6-213">\*    Visualizzazione e modifica dei dettagli bancari e fiscali</span><span class="sxs-lookup"><span data-stu-id="9e1d6-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="9e1d6-214">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="9e1d6-215">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="9e1d6-215">\*    Access support</span></span>
||<span data-ttu-id="9e1d6-216">\*    Controversie sui pagamenti di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="9e1d6-217">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-217">Incentives user</span></span>|<span data-ttu-id="9e1d6-218">\*    Visualizzazione di programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="9e1d6-219">\*    Visualizzazione e avvio di attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="9e1d6-220">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="9e1d6-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="9e1d6-221">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="9e1d6-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="9e1d6-222">Visualizzare i dati di Insights del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="9e1d6-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="9e1d6-223">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-223">**Role**</span></span> | <span data-ttu-id="9e1d6-224">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="9e1d6-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="9e1d6-225">Visualizzatore di report esecutivi</span><span class="sxs-lookup"><span data-stu-id="9e1d6-225">Executive report viewer</span></span>|<span data-ttu-id="9e1d6-226">Accedere a tutti i set di dati di reporting</span><span class="sxs-lookup"><span data-stu-id="9e1d6-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="9e1d6-227">Visualizzatore di report</span><span class="sxs-lookup"><span data-stu-id="9e1d6-227">Report viewer</span></span>|<span data-ttu-id="9e1d6-228">Accedere ai report di dati, ad eccezione dei ricavi e dei dati personali di clienti e dipendenti</span><span class="sxs-lookup"><span data-stu-id="9e1d6-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    