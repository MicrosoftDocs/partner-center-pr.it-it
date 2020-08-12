---
title: Ripristinare i privilegi di amministratore per Azure CSP
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aiutare i clienti a ripristinare i privilegi di amministratore di un partner in modo che il partner possa contribuire alla gestione delle sottoscrizioni di Azure CSP di un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811331"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="13787-103">Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente</span><span class="sxs-lookup"><span data-stu-id="13787-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="13787-104">**Ruoli applicabili**</span><span class="sxs-lookup"><span data-stu-id="13787-104">**Applicable roles**</span></span>

- <span data-ttu-id="13787-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="13787-105">Global admin</span></span>
- <span data-ttu-id="13787-106">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="13787-106">Admin agent</span></span>

<span data-ttu-id="13787-107">Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto.</span><span class="sxs-lookup"><span data-stu-id="13787-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="13787-108">A tale scopo, è necessario disporre dei privilegi di amministratore.</span><span class="sxs-lookup"><span data-stu-id="13787-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="13787-109">Alcuni privilegi vengono concessi quando viene stabilita la relazione di rivenditore con il cliente,</span><span class="sxs-lookup"><span data-stu-id="13787-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="13787-110">mentre altri ti vengono concessi dal cliente.</span><span class="sxs-lookup"><span data-stu-id="13787-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="13787-111">Privilegi di amministratore per Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="13787-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="13787-112">Esistono due livelli di privilegi di amministratore per Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="13787-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="13787-113">**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti.</span><span class="sxs-lookup"><span data-stu-id="13787-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="13787-114">In questo modo, i partner CSP possono accedere ai tenant dei clienti ed eseguire funzioni amministrative, ad esempio l'aggiunta o la gestione degli utenti, la reimpostazione delle password e la gestione delle licenze utente.</span><span class="sxs-lookup"><span data-stu-id="13787-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="13787-115">**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti.</span><span class="sxs-lookup"><span data-stu-id="13787-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="13787-116">Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="13787-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="13787-117">Ripristinare i privilegi di amministratore dei partner CSP</span><span class="sxs-lookup"><span data-stu-id="13787-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="13787-118">Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.</span><span class="sxs-lookup"><span data-stu-id="13787-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="13787-119">Accedi al dashboard Centro per i partner e scegli **Clienti** dal menu del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="13787-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="13787-120">Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="13787-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="13787-121">Viene generato un collegamento al cliente che ha diritti di amministratore del tenant.</span><span class="sxs-lookup"><span data-stu-id="13787-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="13787-122">Tale utente deve selezionare il collegamento e approvare la richiesta di relazione di rivenditore.</span><span class="sxs-lookup"><span data-stu-id="13787-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Relazione di rivenditore":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="13787-124">Aggiunta del gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP</span><span class="sxs-lookup"><span data-stu-id="13787-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="13787-125">Il cliente dovrà aggiungere il gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP.</span><span class="sxs-lookup"><span data-stu-id="13787-125">Your customer will need to add your admin agent group as the owner of the Azure CSP subscription.</span></span>

1. <span data-ttu-id="13787-126">Usa la console di PowerShell o l'ambiente di scripting integrato (ISE) di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="13787-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="13787-127">Verificare che i moduli AzureAD siano installati.</span><span class="sxs-lookup"><span data-stu-id="13787-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="13787-128">Connettiti al tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13787-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="13787-129">Ottieni ObjectId dei gruppi di agenti di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="13787-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="13787-130">I passaggi seguenti vengono eseguiti dall'utente nell'azienda del cliente che ha accesso proprietario alla sottoscrizione di Azure CSP.</span><span class="sxs-lookup"><span data-stu-id="13787-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="13787-131">L'utente con accesso proprietario alla sottoscrizione di Azure CSP accede ad Azure usando le credenziali personali.</span><span class="sxs-lookup"><span data-stu-id="13787-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzAccount
   ```

5. <span data-ttu-id="13787-132">Può quindi aggiungere il gruppo di agenti di amministrazione come proprietario alla sottoscrizione di Azure CSP.</span><span class="sxs-lookup"><span data-stu-id="13787-132">She can then add your admin agent group as owner to the CSP Azure subscription.</span></span>

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a><span data-ttu-id="13787-133">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="13787-133">Next steps</span></span>

[<span data-ttu-id="13787-134">Gestire sottoscrizioni e risorse nel piano di Azure</span><span class="sxs-lookup"><span data-stu-id="13787-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
