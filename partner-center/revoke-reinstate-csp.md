---
title: Ripristinare i privilegi di amministratore per Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aiutare i clienti a ripristinare i privilegi di amministratore di un partner in modo che il partner possa gestire le sottoscrizioni di Azure Cloud Solution Provider (CSP) di un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510177"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="3abdc-103">Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente</span><span class="sxs-lookup"><span data-stu-id="3abdc-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="3abdc-104">**Ruoli appropriati:** Amministratore globale | Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="3abdc-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="3abdc-105">In quanto partner Cloud Solution Provider (CSP), i clienti spesso si aspettano di gestire l'utilizzo di Azure e i relativi sistemi.</span><span class="sxs-lookup"><span data-stu-id="3abdc-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="3abdc-106">A tale scopo, è necessario disporre dei privilegi di amministratore.</span><span class="sxs-lookup"><span data-stu-id="3abdc-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="3abdc-107">Alcuni privilegi vengono concessi quando viene stabilita la relazione del rivenditore con il cliente.</span><span class="sxs-lookup"><span data-stu-id="3abdc-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="3abdc-108">mentre altri ti vengono concessi dal cliente.</span><span class="sxs-lookup"><span data-stu-id="3abdc-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="3abdc-109">Privilegi di amministratore per Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="3abdc-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="3abdc-110">Esistono due livelli di privilegi di amministratore per Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="3abdc-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="3abdc-111">**Privilegi di amministratore a livello di** tenant (privilegi di amministratore delegato): i partner CSP ottengono questi privilegi stabilendo al tempo stesso una relazione di rivenditore CSP con i clienti.</span><span class="sxs-lookup"><span data-stu-id="3abdc-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="3abdc-112">I privilegi di amministratore delegato offrono ai partner CSP l'accesso ai tenant dei clienti.</span><span class="sxs-lookup"><span data-stu-id="3abdc-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="3abdc-113">Questo accesso consente loro di eseguire funzioni amministrative come l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.</span><span class="sxs-lookup"><span data-stu-id="3abdc-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="3abdc-114">**Privilegi di amministratore a livello di sottoscrizione:** i partner CSP ottengono questi privilegi durante la creazione Azure CSP sottoscrizioni per i clienti.</span><span class="sxs-lookup"><span data-stu-id="3abdc-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="3abdc-115">Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="3abdc-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="3abdc-116">Ripristinare i privilegi di amministratore di un partner CSP</span><span class="sxs-lookup"><span data-stu-id="3abdc-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="3abdc-117">Il cliente può creare nuovamente l'assegnazione di ruolo CSP se si specifica il del gruppo `object ID` AdminAgents al cliente.</span><span class="sxs-lookup"><span data-stu-id="3abdc-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="3abdc-118">Per ottenere nuovamente i privilegi di amministratore delegato, è necessario collaborare con il cliente seguendo questa procedura.</span><span class="sxs-lookup"><span data-stu-id="3abdc-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="3abdc-119">Accedere al dashboard Partner Center dati.</span><span class="sxs-lookup"><span data-stu-id="3abdc-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="3abdc-120">Nel menu Partner Center selezionare **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="3abdc-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="3abdc-121">Selezionare il cliente con cui si sta lavorando e **richiedere una relazione di rivenditore.**</span><span class="sxs-lookup"><span data-stu-id="3abdc-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="3abdc-122">Questa azione genera un collegamento al cliente con diritti di amministratore tenant.</span><span class="sxs-lookup"><span data-stu-id="3abdc-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="3abdc-123">Il cliente deve selezionare il collegamento e approvare la richiesta di relazione con il rivenditore.</span><span class="sxs-lookup"><span data-stu-id="3abdc-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di posta elettronica di creazione della relazione rivenditore.":::

5. <span data-ttu-id="3abdc-125">Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="3abdc-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="3abdc-126">Il cliente deve quindi eseguire la procedura seguente usando PowerShell o l'interfaccia della riga di comando di Azure.</span><span class="sxs-lookup"><span data-stu-id="3abdc-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="3abdc-127">Il cliente deve avere:</span><span class="sxs-lookup"><span data-stu-id="3abdc-127">Your customer must have:</span></span>

- <span data-ttu-id="3abdc-128">Ruolo del proprietario **o dell'amministratore** **dell'accesso utente**</span><span class="sxs-lookup"><span data-stu-id="3abdc-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="3abdc-129">Autorizzazioni per creare assegnazioni di ruolo a livello di sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="3abdc-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="3abdc-130">a.</span><span class="sxs-lookup"><span data-stu-id="3abdc-130">a.</span></span> <span data-ttu-id="3abdc-131">Solo per PowerShell, il cliente deve aggiornare il `Az.Resources` modulo.</span><span class="sxs-lookup"><span data-stu-id="3abdc-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="3abdc-132">b.</span><span class="sxs-lookup"><span data-stu-id="3abdc-132">b.</span></span> <span data-ttu-id="3abdc-133">Il cliente si connette al tenant in cui è presente la sottoscrizione CSP.</span><span class="sxs-lookup"><span data-stu-id="3abdc-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="3abdc-134">c.</span><span class="sxs-lookup"><span data-stu-id="3abdc-134">c.</span></span> <span data-ttu-id="3abdc-135">Il cliente si connette alla sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="3abdc-135">The customer connects to the subscription.</span></span> <span data-ttu-id="3abdc-136">Questa opzione *è applicabile* solo se l'utente dispone di autorizzazioni di assegnazione di ruolo su più sottoscrizioni nel tenant.</span><span class="sxs-lookup"><span data-stu-id="3abdc-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="3abdc-137">d.</span><span class="sxs-lookup"><span data-stu-id="3abdc-137">d.</span></span> <span data-ttu-id="3abdc-138">Il cliente crea quindi l'assegnazione di ruolo.</span><span class="sxs-lookup"><span data-stu-id="3abdc-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="3abdc-139">Anziché concedere autorizzazioni di proprietario nell'ambito della sottoscrizione, è possibile concedere a livello di gruppo di risorse o di risorsa.</span><span class="sxs-lookup"><span data-stu-id="3abdc-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="3abdc-140">A livello di gruppo di risorse</span><span class="sxs-lookup"><span data-stu-id="3abdc-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="3abdc-141">A livello di risorsa</span><span class="sxs-lookup"><span data-stu-id="3abdc-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="3abdc-142">Se i passaggi precedenti non funzionano o si verificano errori durante il tentativo, provare la procedura "catch-all" seguente per ripristinare i diritti di amministratore per il cliente.</span><span class="sxs-lookup"><span data-stu-id="3abdc-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="3abdc-143">Risoluzione dei problemi</span><span class="sxs-lookup"><span data-stu-id="3abdc-143">Troubleshooting</span></span>

<span data-ttu-id="3abdc-144">Se il cliente non è in grado di completare il passaggio 6 precedente, fare in modo che il cliente eserciti il comando seguente:</span><span class="sxs-lookup"><span data-stu-id="3abdc-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="3abdc-145">Fornire il `newRoleAssignment.log` file risultante a Microsoft per un'ulteriore analisi.</span><span class="sxs-lookup"><span data-stu-id="3abdc-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="3abdc-146">Se la procedura "catch-all" ha esito negativo durante `Import-Module` , provare a seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="3abdc-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="3abdc-147">Se l'importazione non riesce perché il modulo è in uso, riavviare la sessione di PowerShell chiudendo e riaprendo tutte le finestre.</span><span class="sxs-lookup"><span data-stu-id="3abdc-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="3abdc-148">Controllare la versione `Az.Resources` di con `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="3abdc-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="3abdc-149">Se la versione 4.1.1 non è in elenco disponibile, è necessario usare `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="3abdc-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="3abdc-150">Se l'errore indica che deve essere una versione specifica, aggiornare anche il `Az.Accounts` modulo, sostituendo con `Az.Resources` `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="3abdc-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="3abdc-151">È quindi necessario riavviare la sessione di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3abdc-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="3abdc-152">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="3abdc-152">Next steps</span></span>

- [<span data-ttu-id="3abdc-153">Gestire sottoscrizioni e risorse nel piano di Azure</span><span class="sxs-lookup"><span data-stu-id="3abdc-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
