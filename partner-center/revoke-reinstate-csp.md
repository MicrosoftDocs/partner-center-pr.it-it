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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente  

**Ruoli appropriati:** Amministratore globale | Agente amministratore

In quanto partner Cloud Solution Provider (CSP), i clienti spesso si aspettano di gestire l'utilizzo di Azure e i relativi sistemi. A tale scopo, è necessario disporre dei privilegi di amministratore. Alcuni privilegi vengono concessi quando viene stabilita la relazione del rivenditore con il cliente. mentre altri ti vengono concessi dal cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegi di amministratore per Azure in CSP

Esistono due livelli di privilegi di amministratore per Azure in CSP.

- **Privilegi di amministratore a livello di** tenant (privilegi di amministratore delegato): i partner CSP ottengono questi privilegi stabilendo al tempo stesso una relazione di rivenditore CSP con i clienti. I privilegi di amministratore delegato offrono ai partner CSP l'accesso ai tenant dei clienti. Questo accesso consente loro di eseguire funzioni amministrative come l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.
- **Privilegi di amministratore a livello di sottoscrizione:** i partner CSP ottengono questi privilegi durante la creazione Azure CSP sottoscrizioni per i clienti. Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Ripristinare i privilegi di amministratore di un partner CSP

Il cliente può creare nuovamente l'assegnazione di ruolo CSP se si specifica il del gruppo `object ID` AdminAgents al cliente. Per ottenere nuovamente i privilegi di amministratore delegato, è necessario collaborare con il cliente seguendo questa procedura.

1. Accedere al dashboard Partner Center dati.

2. Nel menu Partner Center selezionare **Clienti**.

3. Selezionare il cliente con cui si sta lavorando e **richiedere una relazione di rivenditore.** Questa azione genera un collegamento al cliente con diritti di amministratore tenant.

4. Il cliente deve selezionare il collegamento e approvare la richiesta di relazione con il rivenditore.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di posta elettronica di creazione della relazione rivenditore.":::

5. Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Il cliente deve quindi eseguire la procedura seguente usando PowerShell o l'interfaccia della riga di comando di Azure. Il cliente deve avere:

- Ruolo del proprietario **o dell'amministratore** **dell'accesso utente** 
- Autorizzazioni per creare assegnazioni di ruolo a livello di sottoscrizione

   a. Solo per PowerShell, il cliente deve aggiornare il `Az.Resources` modulo.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Il cliente si connette al tenant in cui è presente la sottoscrizione CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Il cliente si connette alla sottoscrizione. Questa opzione *è applicabile* solo se l'utente dispone di autorizzazioni di assegnazione di ruolo su più sottoscrizioni nel tenant.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Il cliente crea quindi l'assegnazione di ruolo.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Anziché concedere autorizzazioni di proprietario nell'ambito della sottoscrizione, è possibile concedere a livello di gruppo di risorse o di risorsa. 

- A livello di gruppo di risorse

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- A livello di risorsa

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Se i passaggi precedenti non funzionano o si verificano errori durante il tentativo, provare la procedura "catch-all" seguente per ripristinare i diritti di amministratore per il cliente.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Risoluzione dei problemi

Se il cliente non è in grado di completare il passaggio 6 precedente, fare in modo che il cliente eserciti il comando seguente:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Fornire il `newRoleAssignment.log` file risultante a Microsoft per un'ulteriore analisi.

Se la procedura "catch-all" ha esito negativo durante `Import-Module` , provare a seguire questa procedura:
- Se l'importazione non riesce perché il modulo è in uso, riavviare la sessione di PowerShell chiudendo e riaprendo tutte le finestre.
- Controllare la versione `Az.Resources` di con `Get-Module Az.Resources -ListAvailable` .
- Se la versione 4.1.1 non è in elenco disponibile, è necessario usare `Update-Module Az.Resources -Force` .
- Se l'errore indica che deve essere una versione specifica, aggiornare anche il `Az.Accounts` modulo, sostituendo con `Az.Resources` `Az.Accounts` . È quindi necessario riavviare la sessione di PowerShell.


## <a name="next-steps"></a>Passaggi successivi

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
