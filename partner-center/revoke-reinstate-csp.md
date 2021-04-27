---
title: Ripristinare i privilegi di amministratore per Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aiutare i clienti a ripristinare i privilegi di amministratore di un partner in modo che il partner possa contribuire alla gestione delle sottoscrizioni di Azure CSP di un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018188"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="d090b-103">Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente</span><span class="sxs-lookup"><span data-stu-id="d090b-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="d090b-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="d090b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d090b-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="d090b-105">Global admin</span></span>
- <span data-ttu-id="d090b-106">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="d090b-106">Admin agent</span></span>

<span data-ttu-id="d090b-107">Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto.</span><span class="sxs-lookup"><span data-stu-id="d090b-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="d090b-108">A tale scopo, è necessario disporre dei privilegi di amministratore.</span><span class="sxs-lookup"><span data-stu-id="d090b-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="d090b-109">Alcuni privilegi vengono concessi quando viene stabilita la relazione del rivenditore con il cliente.</span><span class="sxs-lookup"><span data-stu-id="d090b-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="d090b-110">mentre altri ti vengono concessi dal cliente.</span><span class="sxs-lookup"><span data-stu-id="d090b-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="d090b-111">Privilegi di amministratore per Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="d090b-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="d090b-112">Esistono due livelli di privilegi di amministratore per Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="d090b-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="d090b-113">**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti.</span><span class="sxs-lookup"><span data-stu-id="d090b-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="d090b-114">I privilegi di amministratore delegato consentono ai partner CSP di accedere ai tenant dei clienti, che consentono loro di eseguire funzioni amministrative come l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.</span><span class="sxs-lookup"><span data-stu-id="d090b-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="d090b-115">**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti.</span><span class="sxs-lookup"><span data-stu-id="d090b-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="d090b-116">Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="d090b-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="d090b-117">Ripristinare i privilegi di amministratore dei partner CSP</span><span class="sxs-lookup"><span data-stu-id="d090b-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="d090b-118">Il cliente può creare nuovamente l'assegnazione di ruolo CSP purché si fornisse l'ID oggetto del gruppo AdminAgents al cliente.</span><span class="sxs-lookup"><span data-stu-id="d090b-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="d090b-119">Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.</span><span class="sxs-lookup"><span data-stu-id="d090b-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="d090b-120">Accedere al dashboard Partner Center e dal menu Partner Center selezionare **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="d090b-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="d090b-121">Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="d090b-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="d090b-122">Questa azione genera un collegamento al cliente che dispone dei diritti di amministratore del tenant.</span><span class="sxs-lookup"><span data-stu-id="d090b-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="d090b-123">Il cliente deve selezionare il collegamento e approvare la richiesta di relazione con il rivenditore.</span><span class="sxs-lookup"><span data-stu-id="d090b-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di posta elettronica di creazione di una relazione rivenditore":::

4. <span data-ttu-id="d090b-125">Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="d090b-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="d090b-126">Il cliente che ha il ruolo di proprietario o amministratore **dell'accesso utente** e ha l'autorizzazione per creare un'assegnazione di ruolo a livello di sottoscrizione esegue le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d090b-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="d090b-127">Si connette al tenant in cui è presente la sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="d090b-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="d090b-128">Si connette alla sottoscrizione (applicabile solo se l'utente dispone di autorizzazioni di assegnazione di ruolo su più sottoscrizioni nel tenant).</span><span class="sxs-lookup"><span data-stu-id="d090b-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="d090b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "ID sottoscrizione CSP"'</span><span class="sxs-lookup"><span data-stu-id="d090b-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="d090b-130">Crea l'assegnazione di ruolo</span><span class="sxs-lookup"><span data-stu-id="d090b-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="d090b-131">Se si vuole concedere l'autorizzazione del ruolo proprietario a livello di gruppo di risorse o di risorsa anziché a livello di sottoscrizione, i comandi seguenti possono funzionare:</span><span class="sxs-lookup"><span data-stu-id="d090b-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="d090b-132">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d090b-132">Next steps</span></span>

- [<span data-ttu-id="d090b-133">Gestire sottoscrizioni e risorse nel piano di Azure</span><span class="sxs-lookup"><span data-stu-id="d090b-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
