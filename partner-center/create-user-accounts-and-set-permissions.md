---
title: Creare account utente e assegnare ruoli
description: A ogni dipendente deve essere assegnato un ruolo per poter accedere al Centro per i partner. Scopri come creare gli account utente, assegnare ruoli e impostare le autorizzazioni.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148143"
---
# <a name="create-user-accounts"></a><span data-ttu-id="a65fe-104">Creare account utente</span><span class="sxs-lookup"><span data-stu-id="a65fe-104">Create user accounts</span></span>  

<span data-ttu-id="a65fe-105">**Ruoli appropriati:** amministratore account | Amministratore globale | Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="a65fe-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="a65fe-106">Crea gli account utente per i dipendenti che hanno bisogno di accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a65fe-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="a65fe-107">Questa operazione deve essere eseguita dall'amministratore per la gestione degli utenti, dall'amministratore degli account o dall'amministratore globale. All'utente che esegue queste attività devono essere assegnati anche i ruoli di amministratore degli utenti o amministratore globale di Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="a65fe-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="a65fe-108">Per altre informazioni sui ruoli di AAD, vedi [Autorizzazioni dei ruoli di amministratore in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="a65fe-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="a65fe-109">Aggiungere un nuovo utente</span><span class="sxs-lookup"><span data-stu-id="a65fe-109">Add a new user</span></span>

1. <span data-ttu-id="a65fe-110">Dall'icona **Impostazioni** in alto a destra nel Centro per i partner selezionare **Impostazioni account** e quindi **Gestione utenti**.</span><span class="sxs-lookup"><span data-stu-id="a65fe-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="a65fe-111">Selezionare **Aggiungi utente**.</span><span class="sxs-lookup"><span data-stu-id="a65fe-111">Select **Add user**.</span></span>

3. <span data-ttu-id="a65fe-112">Immetti il nome completo e l'indirizzo di posta elettronica univoco dell'utente.</span><span class="sxs-lookup"><span data-stu-id="a65fe-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="a65fe-113">Seleziona il tipo di agente e/o il tipo di amministratore da assegnare all'utente.</span><span class="sxs-lookup"><span data-stu-id="a65fe-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="a65fe-114">L'accesso al Centro per i partner è basato sui ruoli, quindi è possibile assegnare autorizzazioni per personalizzare la visualizzazione dell'utente in modo da mostrargli solo le funzionalità utili per completare le attività specifiche.</span><span class="sxs-lookup"><span data-stu-id="a65fe-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="a65fe-115">Se gli utenti vogliono l'assegnazione di un ruolo, possono trovare gli amministratori globali da contattare accedendo a **Gestione utenti** e filtrando in base all'amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="a65fe-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="a65fe-116">Selezionare **Aggiungi** per creare l'account utente.</span><span class="sxs-lookup"><span data-stu-id="a65fe-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="a65fe-117">Verificare i dettagli dell'utente nella pagina successiva.</span><span class="sxs-lookup"><span data-stu-id="a65fe-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a65fe-118">Prendere nota delle informazioni di accesso del nuovo utente visualizzate in questa pagina.</span><span class="sxs-lookup"><span data-stu-id="a65fe-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="a65fe-119">Copiarle e inviarle al nuovo utente perché in seguito non sarà più possibile accedervi.</span><span class="sxs-lookup"><span data-stu-id="a65fe-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="a65fe-120">L'utente dovrà accedere al Centro per i partner con il nome utente e la password temporanea.</span><span class="sxs-lookup"><span data-stu-id="a65fe-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="a65fe-121">Quando l'utente accede al Centro per i partner per la prima volta, gli viene chiesto di modificare la password.</span><span class="sxs-lookup"><span data-stu-id="a65fe-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="a65fe-122">Assegnare ruoli utente</span><span class="sxs-lookup"><span data-stu-id="a65fe-122">Assign user roles</span></span>

<span data-ttu-id="a65fe-123">Per usare il Centro per i partner, devi avere un ruolo assegnato.</span><span class="sxs-lookup"><span data-stu-id="a65fe-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="a65fe-124">I ruoli includono attualmente i ruoli tenant di Azure Active Directory, i ruoli del programma Cloud Solution Provider (CSP) e i ruoli aziendali non AAD.</span><span class="sxs-lookup"><span data-stu-id="a65fe-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="a65fe-125">Una singola azienda può avere bisogno di tutti questi ruoli.</span><span class="sxs-lookup"><span data-stu-id="a65fe-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="a65fe-126">Per accedere al Centro per i partner, i singoli utenti devono essere elencati nel tenant.</span><span class="sxs-lookup"><span data-stu-id="a65fe-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="a65fe-127">Le assegnazioni di ruoli forniscono possibilità di accesso aggiuntive.</span><span class="sxs-lookup"><span data-stu-id="a65fe-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a65fe-128">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="a65fe-128">Next steps</span></span>

- [<span data-ttu-id="a65fe-129">Assegnare ruoli utente e autorizzazioni per i dipendenti che devono usare il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a65fe-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
