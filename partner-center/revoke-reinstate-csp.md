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
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855421"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente  

**Ruoli appropriati:** amministratore globale | Agente amministratore

Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto. A tale scopo, è necessario disporre dei privilegi di amministratore. Alcuni privilegi vengono concessi quando viene stabilita la relazione come rivenditore con il cliente. mentre altri ti vengono concessi dal cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegi di amministratore per Azure in CSP

Esistono due livelli di privilegi di amministratore per Azure in CSP.

**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti. I privilegi di amministratore con delega consentono ai partner CSP di accedere ai tenant dei clienti, che consentono loro di eseguire funzioni amministrative come l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.

**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti. Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Ripristinare i privilegi di amministratore dei partner CSP

Il cliente può creare nuovamente l'assegnazione di ruolo CSP, purché si fornisse l'ID oggetto del gruppo AdminAgents al cliente. Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.

1. Accedere al dashboard Partner Center e dal menu Partner Center selezionare **Clienti.**

2. Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**. Questa azione genera un collegamento al cliente che dispone dei diritti di amministratore del tenant.

3. Il cliente deve selezionare il collegamento e approvare la richiesta di relazione come rivenditore.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di messaggio di posta elettronica di creazione della relazione come rivenditore":::

4. Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Il cliente che ha il ruolo di proprietario o amministratore **accesso utenti** e ha l'autorizzazione per creare un'assegnazione di ruolo a livello di sottoscrizione esegue le operazioni seguenti:


    1. Si connette al tenant in cui è presente la sottoscrizione CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Si connette alla sottoscrizione (applicabile solo se l'utente ha autorizzazioni di assegnazione di ruolo per più sottoscrizioni nel tenant).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"'


    3. Crea l'assegnazione di ruolo
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Se si vuole concedere l'autorizzazione del ruolo proprietario a livello di gruppo di risorse o di risorsa anziché a livello di sottoscrizione, è possibile usare i comandi seguenti:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Passaggi successivi

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
