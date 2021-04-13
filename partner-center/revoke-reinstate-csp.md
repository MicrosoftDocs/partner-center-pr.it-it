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
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315848"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="6aead-103">Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente</span><span class="sxs-lookup"><span data-stu-id="6aead-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="6aead-104">**Ruoli applicabili**</span><span class="sxs-lookup"><span data-stu-id="6aead-104">**Applicable roles**</span></span>

- <span data-ttu-id="6aead-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="6aead-105">Global admin</span></span>
- <span data-ttu-id="6aead-106">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="6aead-106">Admin agent</span></span>

<span data-ttu-id="6aead-107">Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto.</span><span class="sxs-lookup"><span data-stu-id="6aead-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="6aead-108">A tale scopo, è necessario disporre dei privilegi di amministratore.</span><span class="sxs-lookup"><span data-stu-id="6aead-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="6aead-109">Alcuni privilegi vengono concessi quando viene stabilita la relazione del rivenditore con il cliente.</span><span class="sxs-lookup"><span data-stu-id="6aead-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="6aead-110">mentre altri ti vengono concessi dal cliente.</span><span class="sxs-lookup"><span data-stu-id="6aead-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="6aead-111">Privilegi di amministratore per Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="6aead-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="6aead-112">Esistono due livelli di privilegi di amministratore per Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="6aead-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="6aead-113">**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti.</span><span class="sxs-lookup"><span data-stu-id="6aead-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="6aead-114">I privilegi amministrativi delegati forniscono ai partner CSP l'accesso ai tenant dei clienti, che consentono loro di eseguire funzioni amministrative quali l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.</span><span class="sxs-lookup"><span data-stu-id="6aead-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="6aead-115">**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti.</span><span class="sxs-lookup"><span data-stu-id="6aead-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="6aead-116">Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="6aead-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="6aead-117">Ripristinare i privilegi di amministratore dei partner CSP</span><span class="sxs-lookup"><span data-stu-id="6aead-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="6aead-118">Il cliente è in grado di ricreare l'assegnazione di ruolo CSP purché si fornisca all'utente l'ID oggetto del gruppo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="6aead-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="6aead-119">Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.</span><span class="sxs-lookup"><span data-stu-id="6aead-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="6aead-120">Accedere al dashboard del centro per i partner e scegliere **clienti** dal menu centro partner.</span><span class="sxs-lookup"><span data-stu-id="6aead-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="6aead-121">Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="6aead-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="6aead-122">Viene generato un collegamento al cliente che ha diritti di amministratore del tenant.</span><span class="sxs-lookup"><span data-stu-id="6aead-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="6aead-123">Il cliente deve selezionare il collegamento e approvare la richiesta di relazione Reseller.</span><span class="sxs-lookup"><span data-stu-id="6aead-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di messaggio di posta elettronica di Crea relazione rivenditore":::

4. <span data-ttu-id="6aead-125">Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="6aead-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="6aead-126">Il cliente che ha il ruolo di **proprietario o amministratore accesso utenti** e dispone dell'autorizzazione per creare un'assegnazione di ruolo a livello di sottoscrizione esegue le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="6aead-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="6aead-127">Stabilisce la connessione al tenant in cui esiste la sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="6aead-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="6aead-128">Si connette alla sottoscrizione (applicabile solo se l'utente dispone di autorizzazioni di assegnazione di ruolo per più sottoscrizioni nel tenant).</span><span class="sxs-lookup"><span data-stu-id="6aead-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="6aead-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "ID sottoscrizione CSP" "</span><span class="sxs-lookup"><span data-stu-id="6aead-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="6aead-130">Crea l'assegnazione di ruolo</span><span class="sxs-lookup"><span data-stu-id="6aead-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="6aead-131">Se si desidera concedere l'autorizzazione per il ruolo di proprietario a livello di gruppo di risorse o di risorse anziché ambito di sottoscrizione, è possibile usare i comandi seguenti:</span><span class="sxs-lookup"><span data-stu-id="6aead-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="6aead-132">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="6aead-132">Next steps</span></span>

- [<span data-ttu-id="6aead-133">Gestire sottoscrizioni e risorse nel piano di Azure</span><span class="sxs-lookup"><span data-stu-id="6aead-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
