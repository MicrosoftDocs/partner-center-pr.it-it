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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040767"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="7d818-103">Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="7d818-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="7d818-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7d818-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="7d818-105">Global admin</span></span>
- <span data-ttu-id="7d818-106">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="7d818-106">User admin</span></span>
- <span data-ttu-id="7d818-107">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-107">MPN partner admin</span></span>

<span data-ttu-id="7d818-108">Ormai hai configurato il tuo profilo di partner, inclusi la ragione sociale e l'indirizzo, i dettagli per il supporto, le esenzioni fiscali, le coordinate bancarie e il contatto principale della tua azienda.</span><span class="sxs-lookup"><span data-stu-id="7d818-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7d818-109">Passaggio successivo: configurare gli utenti assegnando loro password e ruoli in modo che possano iniziare a lavorare con te nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="7d818-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7d818-110">Configurare i dipendenti in modo che possano lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7d818-111">Puoi determinare i tipi di accesso al Centro per i partner di cui dispongono gli utenti assegnando loro ruoli e autorizzazioni specifici.</span><span class="sxs-lookup"><span data-stu-id="7d818-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7d818-112">I ruoli sono correlati ai programmi in cui è coinvolta la tua azienda.</span><span class="sxs-lookup"><span data-stu-id="7d818-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7d818-113">Ad esempio, se si tratta di un'azienda CSP (Cloud Solution Provider), non solo avrai i ruoli di gestione del tenant di Azure AD standard (tra cui il ruolo di amministratore globale), ma avrai bisogno anche di ruoli specifici del programma CSP.</span><span class="sxs-lookup"><span data-stu-id="7d818-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7d818-114">Ogni programma prevede ruoli specifici.</span><span class="sxs-lookup"><span data-stu-id="7d818-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7d818-115">I ruoli relativi al tenant di Azure Active Directory (AAD) includono l'amministratore globale, l'amministratore utenti e i ruoli CSP.</span><span class="sxs-lookup"><span data-stu-id="7d818-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7d818-116">I ruoli non AAD sono i ruoli che non gestiscono il tenant e includono l'amministratore MPN, l'amministratore del profilo di business, l'amministratore delle segnalazioni, l'amministratore degli incentivi e l'utente di incentivi.</span><span class="sxs-lookup"><span data-stu-id="7d818-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7d818-117">Gestire le transazioni commerciali nel Centro per i partner (ruoli Azure AD e CSP)</span><span class="sxs-lookup"><span data-stu-id="7d818-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7d818-118">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-118">**Role**</span></span>|<span data-ttu-id="7d818-119">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7d818-120">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="7d818-120">Global admin</span></span>|<span data-ttu-id="7d818-121">\*    Accesso a tutti gli account/servizi Microsoft con privilegi completi</span><span class="sxs-lookup"><span data-stu-id="7d818-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7d818-122">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-123">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="7d818-124">\*    Visualizzazione di contratti, listini prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="7d818-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7d818-125">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="7d818-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7d818-126">Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="7d818-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7d818-127">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="7d818-127">User management admin</span></span>   | <span data-ttu-id="7d818-128">\*    Visualizzazione, creazione e gestione di utenti</span><span class="sxs-lookup"><span data-stu-id="7d818-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="7d818-129">\*    Visualizzazione di tutti i profili dei partner</span><span class="sxs-lookup"><span data-stu-id="7d818-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="7d818-130">\*    Visualizzazione, creazione e gestione di utenti partner</span><span class="sxs-lookup"><span data-stu-id="7d818-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="7d818-131">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-132">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="7d818-133">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="7d818-133">Billing admin</span></span> | <span data-ttu-id="7d818-134">- Visualizzazione, creazione e gestione della fatturazione, delle fatture e dei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="7d818-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="7d818-135">\*    Visualizzazione dei prezzi</span><span class="sxs-lookup"><span data-stu-id="7d818-135">\*    View pricing</span></span>
||<span data-ttu-id="7d818-136">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-137">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="7d818-138">Utente predefinito</span><span class="sxs-lookup"><span data-stu-id="7d818-138">Default user</span></span>|  <span data-ttu-id="7d818-139">Visualizzazione del profilo personale</span><span class="sxs-lookup"><span data-stu-id="7d818-139">View My profile</span></span>   |
|<span data-ttu-id="7d818-140">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="7d818-140">Admin agent</span></span> | <span data-ttu-id="7d818-141">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-141">\*    Customer management</span></span>
||<span data-ttu-id="7d818-142">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7d818-143">\*    Creazione e applicazione di profili ai dispositivi</span><span class="sxs-lookup"><span data-stu-id="7d818-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="7d818-144">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="7d818-144">\*    Subscription management</span></span>
||<span data-ttu-id="7d818-145">\*    Integrità del servizio e richieste di servizio per i clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="7d818-146">\*    Richiesta dei privilegi di amministratore con delega</span><span class="sxs-lookup"><span data-stu-id="7d818-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="7d818-147">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="7d818-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="7d818-148">\*    Fatturazione</span><span class="sxs-lookup"><span data-stu-id="7d818-148">\*    Billing</span></span>
||<span data-ttu-id="7d818-149">\*    Amministrazione per conto di un cliente</span><span class="sxs-lookup"><span data-stu-id="7d818-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="7d818-150">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="7d818-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="7d818-151">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-152">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="7d818-153">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="7d818-153">Sales agent</span></span> | <span data-ttu-id="7d818-154">\*    Gestione dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-154">\*    Customer management</span></span>
||<span data-ttu-id="7d818-155">\*    Aggiunta dell'elenco dei dispositivi al Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7d818-156">\*    Gestione degli abbonamenti</span><span class="sxs-lookup"><span data-stu-id="7d818-156">\*    Subscription management</span></span>
||<span data-ttu-id="7d818-157">\*    Visualizzazione dei ticket di supporto</span><span class="sxs-lookup"><span data-stu-id="7d818-157">\*    View support tickets</span></span>
||<span data-ttu-id="7d818-158">\*    Richiesta di una relazione con un cliente</span><span class="sxs-lookup"><span data-stu-id="7d818-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="7d818-159">\*    Visualizzazione di prezzi e offerte</span><span class="sxs-lookup"><span data-stu-id="7d818-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="7d818-160">\*    Gestione dei clienti potenziali</span><span class="sxs-lookup"><span data-stu-id="7d818-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="7d818-161">\*    Visualizzazione del contratto per il cliente</span><span class="sxs-lookup"><span data-stu-id="7d818-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="7d818-162">\*    Registrazione di un rivenditore a valore aggiunto</span><span class="sxs-lookup"><span data-stu-id="7d818-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="7d818-163">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-164">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="7d818-165">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="7d818-165">Helpdesk agent</span></span>| <span data-ttu-id="7d818-166">\*    Ricerca e visualizzazione di un cliente</span><span class="sxs-lookup"><span data-stu-id="7d818-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="7d818-167">\*    Modifica dei dettagli dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-167">\*    Edit customer details</span></span>
||<span data-ttu-id="7d818-168">\*    Supporto per la risoluzione dei problemi dei clienti con la gestione di fatturazioni o abbonamenti</span><span class="sxs-lookup"><span data-stu-id="7d818-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7d818-169">\*    Richiesta di supporto per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="7d818-170">\*    Gestione di abbonamenti e problemi di fatturazione per conto dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="7d818-171">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-172">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7d818-173">Fornitore del pannello di controllo (CPV)</span><span class="sxs-lookup"><span data-stu-id="7d818-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7d818-174">(ruolo CSP e ruolo non AAD)</span><span class="sxs-lookup"><span data-stu-id="7d818-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7d818-175">I CPV sviluppano app destinate ai partner CSP (Cloud Solution Provider) affinché possano integrare i loro sistemi con le API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="7d818-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7d818-176">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-176">**Role**</span></span>   |<span data-ttu-id="7d818-177">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7d818-178">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="7d818-178">Global admin</span></span>| <span data-ttu-id="7d818-179">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="7d818-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7d818-180">Visualizzazione e gestione degli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="7d818-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7d818-181">Utente guest (deve essere aggiunto al tenant di AAD)</span><span class="sxs-lookup"><span data-stu-id="7d818-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7d818-182">**Utente guest**</span><span class="sxs-lookup"><span data-stu-id="7d818-182">**Guest user**</span></span>   | <span data-ttu-id="7d818-183">**Ruoli**</span><span class="sxs-lookup"><span data-stu-id="7d818-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7d818-184">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-184">MPN partner admin</span></span>|
||<span data-ttu-id="7d818-185">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="7d818-185">Accounts admin</span></span>|
||<span data-ttu-id="7d818-186">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-186">Incentives admin</span></span>|
||<span data-ttu-id="7d818-187">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="7d818-187">Business profile admin</span></span>|
||<span data-ttu-id="7d818-188">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="7d818-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7d818-189">Gestione dell'appartenenza a MPN e dell'azienda (ruoli non AAD: questi ruoli gestiscono l'attività dell'azienda anziché il tenant)</span><span class="sxs-lookup"><span data-stu-id="7d818-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7d818-190">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-190">**Role**</span></span> | <span data-ttu-id="7d818-191">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7d818-192">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-192">MPN partner admin</span></span>|<span data-ttu-id="7d818-193">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="7d818-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7d818-194">\*    Visualizzazione di profili legali, aziendali, commerciali e MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7d818-195">\*    Visualizzazione dei dettagli dell'utente e dei relativi dati delle competenze</span><span class="sxs-lookup"><span data-stu-id="7d818-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="7d818-196">\*    Visualizzazione delle competenze</span><span class="sxs-lookup"><span data-stu-id="7d818-196">\*    View competencies</span></span>
||<span data-ttu-id="7d818-197">\*    Visualizzazione e gestione dei vantaggi</span><span class="sxs-lookup"><span data-stu-id="7d818-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="7d818-198">\*    Visualizzazione e acquisto di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="7d818-199">\*    Visualizzazione di fatture e cronologia degli ordini di offerte MPN</span><span class="sxs-lookup"><span data-stu-id="7d818-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7d818-200">\*    Visualizzazione dei dati degli indicatori di contributi dei partner</span><span class="sxs-lookup"><span data-stu-id="7d818-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="7d818-201">\*    Uso dello strumento di convalida dei giustificativi</span><span class="sxs-lookup"><span data-stu-id="7d818-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7d818-202">\*    Visualizzazione dell'analisi dei dati dei clienti</span><span class="sxs-lookup"><span data-stu-id="7d818-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="7d818-203">\*    Visualizzazione di altri ruoli utente all'interno dell'azienda, senza la possibilità di assegnare ruoli</span><span class="sxs-lookup"><span data-stu-id="7d818-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="7d818-204">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-205">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="7d818-206">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="7d818-206">Account admin</span></span>| <span data-ttu-id="7d818-207">Aggiunta di posizioni</span><span class="sxs-lookup"><span data-stu-id="7d818-207">Add locations</span></span>
|| <span data-ttu-id="7d818-208">Gestione di profili relativi agli account amministrati</span><span class="sxs-lookup"><span data-stu-id="7d818-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7d818-209">\*    Assegnazione di ruoli per gli utenti nel tenant a ruoli non AAD</span><span class="sxs-lookup"><span data-stu-id="7d818-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7d818-210">\*    Registrazione di posizioni nei programmi</span><span class="sxs-lookup"><span data-stu-id="7d818-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="7d818-211">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-212">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7d818-213">Gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="7d818-213">Manage referrals</span></span> 

|<span data-ttu-id="7d818-214">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-214">**Role**</span></span>|<span data-ttu-id="7d818-215">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7d818-216">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="7d818-216">Referrals admin</span></span>       |<span data-ttu-id="7d818-217">\*    Visualizzazione, creazione e gestione dei profili di business</span><span class="sxs-lookup"><span data-stu-id="7d818-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="7d818-218">\*    Ricezione e gestione delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="7d818-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="7d818-219">\*    Visualizzazione, creazione e gestione delle segnalazioni di co-selling</span><span class="sxs-lookup"><span data-stu-id="7d818-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7d818-220">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="7d818-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7d818-221">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="7d818-221">Business profile admin</span></span>   |<span data-ttu-id="7d818-222">\*    Visualizzazione, creazione e gestione del profilo di business</span><span class="sxs-lookup"><span data-stu-id="7d818-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="7d818-223">\*    Visualizzazione, creazione e gestione delle richieste di servizio dei partner</span><span class="sxs-lookup"><span data-stu-id="7d818-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="7d818-224">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-225">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7d818-226">Gestione degli incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-226">Manage incentives</span></span> 

|<span data-ttu-id="7d818-227">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-227">**Role**</span></span> | <span data-ttu-id="7d818-228">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7d818-229">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-229">Incentives admin</span></span>|<span data-ttu-id="7d818-230">\*    Avvio e gestione di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="7d818-231">\*    Visualizzazione e modifica di tutti gli aspetti dei programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7d818-232">\*    Visualizzazione e modifica dei dettagli bancari e fiscali</span><span class="sxs-lookup"><span data-stu-id="7d818-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7d818-233">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="7d818-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7d818-234">\*    Accesso al supporto</span><span class="sxs-lookup"><span data-stu-id="7d818-234">\*    Access support</span></span>
||<span data-ttu-id="7d818-235">\*    Controversie sui pagamenti di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="7d818-236">Utente di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-236">Incentives user</span></span>|<span data-ttu-id="7d818-237">\*    Visualizzazione di programmi di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="7d818-238">\*    Visualizzazione e avvio di attestazioni di incentivi</span><span class="sxs-lookup"><span data-stu-id="7d818-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7d818-239">\*    Visualizzazione di sconti e utili in collaborazione</span><span class="sxs-lookup"><span data-stu-id="7d818-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7d818-240">\*    Creazione di ticket di supporto per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d818-241">\*    Visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="7d818-242">Visualizzare i dati di Insights del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7d818-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="7d818-243">**Ruolo**</span><span class="sxs-lookup"><span data-stu-id="7d818-243">**Role**</span></span> | <span data-ttu-id="7d818-244">**Operazioni consentite**</span><span class="sxs-lookup"><span data-stu-id="7d818-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7d818-245">Visualizzatore di report esecutivi</span><span class="sxs-lookup"><span data-stu-id="7d818-245">Executive report viewer</span></span>|<span data-ttu-id="7d818-246">Accesso a tutti i set di dati di reporting, creazione di ticket di supporto per i partner, visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="7d818-247">Visualizzatore di report</span><span class="sxs-lookup"><span data-stu-id="7d818-247">Report viewer</span></span>|<span data-ttu-id="7d818-248">Accesso ai report di dati tranne quelli relativi ai ricavi e ai dati personali di clienti e dipendenti, creazione di ticket di supporto per i partner, visualizzazione dei ticket di supporto per i partner creati</span><span class="sxs-lookup"><span data-stu-id="7d818-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
