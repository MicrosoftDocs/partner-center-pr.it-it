---
title: Creare account utente e assegnare ruoli
description: A ogni dipendente deve essere assegnato un ruolo per poter accedere al Centro per i partner. Scopri come creare gli account utente, assegnare ruoli e impostare le autorizzazioni.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: f71df7df213b2c6410fab37ce323825511a18b6d
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846931"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="a322d-104">Creare account utente e assegnare ruoli e autorizzazioni</span><span class="sxs-lookup"><span data-stu-id="a322d-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="a322d-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="a322d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a322d-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="a322d-106">Account admin</span></span>
- <span data-ttu-id="a322d-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a322d-107">Global admin</span></span>
- <span data-ttu-id="a322d-108">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="a322d-108">User management admin</span></span>

<span data-ttu-id="a322d-109">Crea gli account utente per i dipendenti che hanno bisogno di accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a322d-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="a322d-110">Questa operazione deve essere eseguita dall'amministratore per la gestione degli utenti, dall'amministratore degli account o dall'amministratore globale. All'utente che esegue queste attività devono essere assegnati anche i ruoli di amministratore degli utenti o amministratore globale di Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="a322d-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="a322d-111">Per altre informazioni sui ruoli di AAD, vedi [Autorizzazioni dei ruoli di amministratore in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="a322d-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="a322d-112">Aggiungere un nuovo utente</span><span class="sxs-lookup"><span data-stu-id="a322d-112">Add a new user</span></span>

1. <span data-ttu-id="a322d-113">Dall'icona **Impostazioni** in alto a destra nel Centro per i partner seleziona **Gestione utenti**.</span><span class="sxs-lookup"><span data-stu-id="a322d-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="a322d-114">Selezionare **Aggiungi utente**.</span><span class="sxs-lookup"><span data-stu-id="a322d-114">Select **Add user**.</span></span>

3. <span data-ttu-id="a322d-115">Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.</span><span class="sxs-lookup"><span data-stu-id="a322d-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="a322d-116">Seleziona il tipo di agente e/o il tipo di amministratore da assegnare all'utente.</span><span class="sxs-lookup"><span data-stu-id="a322d-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="a322d-117">L'accesso al Centro per i partner è basato sui ruoli, quindi è possibile assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche.</span><span class="sxs-lookup"><span data-stu-id="a322d-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="a322d-118">Se gli utenti vogliono l'assegnazione di un ruolo, possono trovare gli amministratori globali da contattare accedendo a **Gestione utenti** e filtrando in base all'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="a322d-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="a322d-119">Selezionare **Aggiungi** per creare l'account utente.</span><span class="sxs-lookup"><span data-stu-id="a322d-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="a322d-120">Verificare i dettagli dell'utente nella pagina successiva.</span><span class="sxs-lookup"><span data-stu-id="a322d-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a322d-121">Prendere nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina.</span><span class="sxs-lookup"><span data-stu-id="a322d-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="a322d-122">Copiarle e inviarle al nuovo utente perché in seguito non sarà più possibile accedervi.</span><span class="sxs-lookup"><span data-stu-id="a322d-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="a322d-123">L'utente dovrà accedere al Centro per i partner con il nome utente e la password temporanea.</span><span class="sxs-lookup"><span data-stu-id="a322d-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="a322d-124">Quando l'utente accede al Centro per i partner per la prima volta, gli viene chiesto di modificare la password.</span><span class="sxs-lookup"><span data-stu-id="a322d-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="a322d-125">Trovare il ruolo assegnato all'utente</span><span class="sxs-lookup"><span data-stu-id="a322d-125">Find the role you've been assigned</span></span>

<span data-ttu-id="a322d-126">In mancanza di comunicazioni da parte dell'amministratore globale, è possibile individuare il ruolo ricoperto nel Centro per i partner eseguendo le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a322d-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="a322d-127">Accedere al Centro per i partner [dashboard]https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="a322d-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="a322d-128">Selezionare l'icona **Impostazioni account** e quindi **Il mio profilo**.</span><span class="sxs-lookup"><span data-stu-id="a322d-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="a322d-129">Selezionare la scheda **Ruoli e autorizzazioni**. Vengono visualizzati i ruoli e le autorizzazioni.</span><span class="sxs-lookup"><span data-stu-id="a322d-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="a322d-130">Se al momento dell'accesso non viene visualizzato un programma, significa in genere che non si hanno le autorizzazioni corrette per usare tale programma.</span><span class="sxs-lookup"><span data-stu-id="a322d-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="a322d-131">Ad esempio, se al momento dell'accesso non viene visualizzata la pagina Incentivi, non si hanno le autorizzazioni necessarie per il programma Incentivi.</span><span class="sxs-lookup"><span data-stu-id="a322d-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="a322d-132">L'amministratore globale può concedere le autorizzazioni necessarie.</span><span class="sxs-lookup"><span data-stu-id="a322d-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="a322d-133">Trovare l'amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a322d-133">Find your global admin</span></span>

<span data-ttu-id="a322d-134">A volte può essere necessario modificare il ruolo di un utente oppure un nuovo utente può desiderare un'assegnazione di ruolo specifica.</span><span class="sxs-lookup"><span data-stu-id="a322d-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="a322d-135">Per trovare un amministratore globale che possa apportare modifiche ai ruoli o assegnare ruoli a un nuovo utente, fare clic sull'icona **Impostazioni account** in alto a destra del Centro per i partner, selezionare **Gestione utenti** e filtrare in base all'amministratore globale. In alternativa, è possibile passare a **Il mio profilo**, selezionare **Ruoli e autorizzazioni** e visualizzare l'elenco dei vari amministratori in grado di elevare le autorizzazioni.</span><span class="sxs-lookup"><span data-stu-id="a322d-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="a322d-136">Nuovo amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a322d-136">New global admin</span></span>

<span data-ttu-id="a322d-137">Se l'amministratore globale lascia l'organizzazione ed è necessario che un altro utente ricopra questo ruolo, puoi inviare un ticket al team di Azure o di Office 365.</span><span class="sxs-lookup"><span data-stu-id="a322d-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="a322d-138">Per informazioni su come eseguire questa operazione, seleziona una delle opzioni riportate di seguito.</span><span class="sxs-lookup"><span data-stu-id="a322d-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="a322d-139">Nuovo amministratore globale per Azure</span><span class="sxs-lookup"><span data-stu-id="a322d-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="a322d-140">Nuovo amministratore globale per Office 365</span><span class="sxs-lookup"><span data-stu-id="a322d-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="a322d-141">Assegnare ruoli utente</span><span class="sxs-lookup"><span data-stu-id="a322d-141">Assign user roles</span></span>

<span data-ttu-id="a322d-142">Per usare il Centro per i partner, devi avere un ruolo assegnato.</span><span class="sxs-lookup"><span data-stu-id="a322d-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="a322d-143">I ruoli includono attualmente i ruoli tenant di Azure Active Directory, i ruoli del programma Cloud Solution Provider (CSP) e i ruoli aziendali non AAD.</span><span class="sxs-lookup"><span data-stu-id="a322d-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="a322d-144">Una singola azienda può avere bisogno di tutti questi ruoli.</span><span class="sxs-lookup"><span data-stu-id="a322d-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="a322d-145">Per accedere al Centro per i partner, i singoli utenti devono essere elencati nel tenant.</span><span class="sxs-lookup"><span data-stu-id="a322d-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="a322d-146">Le assegnazioni di ruoli forniscono possibilità di accesso aggiuntive.</span><span class="sxs-lookup"><span data-stu-id="a322d-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="a322d-147">**I ruoli tenant di AAD includono**:</span><span class="sxs-lookup"><span data-stu-id="a322d-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="a322d-148">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a322d-148">Global admin</span></span>
- <span data-ttu-id="a322d-149">Amministratore utenti</span><span class="sxs-lookup"><span data-stu-id="a322d-149">User admin</span></span>

<span data-ttu-id="a322d-150">**I ruoli CSP includono**:</span><span class="sxs-lookup"><span data-stu-id="a322d-150">**CSP roles include**:</span></span>
- <span data-ttu-id="a322d-151">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="a322d-151">Admin agent</span></span>
- <span data-ttu-id="a322d-152">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="a322d-152">Billing admin</span></span>
- <span data-ttu-id="a322d-153">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="a322d-153">Sales agent</span></span>
- <span data-ttu-id="a322d-154">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="a322d-154">Helpdesk agent</span></span>

<span data-ttu-id="a322d-155">**Ruoli che gestiscono l'appartenenza a MPN e la società (non AAD)**</span><span class="sxs-lookup"><span data-stu-id="a322d-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="a322d-156">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="a322d-156">MPN partner admin</span></span>
- <span data-ttu-id="a322d-157">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="a322d-157">Account admin</span></span>
- <span data-ttu-id="a322d-158">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="a322d-158">Referral admin</span></span>
- <span data-ttu-id="a322d-159">Amministratore del profilo di business</span><span class="sxs-lookup"><span data-stu-id="a322d-159">Business profile admin</span></span>
- <span data-ttu-id="a322d-160">Utente e amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="a322d-160">Incentives admin and user</span></span>

<span data-ttu-id="a322d-161">**Produttore del pannello di controllo è un ruolo CSP e non AAD**.</span><span class="sxs-lookup"><span data-stu-id="a322d-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="a322d-162">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a322d-162">Global admin</span></span>

<span data-ttu-id="a322d-163">L'**utente guest** deve essere incluso nel tenant AAD e può avere qualsiasi ruolo non AAD.</span><span class="sxs-lookup"><span data-stu-id="a322d-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="a322d-164">Per informazioni specifiche sui ruoli e sulle operazioni possibili con ciascun ruolo, vedi [Assegnare le autorizzazioni utente](permissions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="a322d-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="a322d-165">Associare l'account Microsoft Learn di un utente nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a322d-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="a322d-166">Per consentire di visualizzare i percorsi di formazione e apprendimento seguiti per l'acquisizione delle competenze, gli utenti devono associare il proprio ID MCP al corrispondente account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a322d-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="a322d-167">Come amministratore globale, quando aggiungi nuovi utenti ricorda loro di associare l'ID MCP al relativo account.</span><span class="sxs-lookup"><span data-stu-id="a322d-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="a322d-168">Come associare l'ID MCP all'account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a322d-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="a322d-169">Dal dashboard del Centro per i partner seleziona l'icona **Il tuo account** nell'angolo destro del dashboard e quindi **Profilo personale**.</span><span class="sxs-lookup"><span data-stu-id="a322d-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="a322d-170">In **Your learning** (La tua formazione) potrai associare il tuo account Microsoft Learning e connettere anche il tuo account Microsoft a Partner University.</span><span class="sxs-lookup"><span data-stu-id="a322d-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a322d-171">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="a322d-171">Next steps</span></span>

- [<span data-ttu-id="a322d-172">Assegnare ruoli utente e autorizzazioni per gli utenti di un'azienda che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a322d-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)