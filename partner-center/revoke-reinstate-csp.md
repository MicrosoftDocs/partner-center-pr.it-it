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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente  

**Ruoli applicabili**

- Amministratore globale
- Agente amministratore

Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto. A tale scopo, è necessario disporre dei privilegi di amministratore. Alcuni privilegi vengono concessi quando viene stabilita la relazione del rivenditore con il cliente. mentre altri ti vengono concessi dal cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegi di amministratore per Azure in CSP

Esistono due livelli di privilegi di amministratore per Azure in CSP.

**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti. I privilegi amministrativi delegati forniscono ai partner CSP l'accesso ai tenant dei clienti, che consentono loro di eseguire funzioni amministrative quali l'aggiunta/gestione di utenti, la reimpostazione delle password e la gestione delle licenze utente.

**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti. Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Ripristinare i privilegi di amministratore dei partner CSP

Il cliente è in grado di ricreare l'assegnazione di ruolo CSP purché si fornisca all'utente l'ID oggetto del gruppo AdminAgents. Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.

1. Accedere al dashboard del centro per i partner e scegliere **clienti** dal menu centro partner.

2. Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**. Viene generato un collegamento al cliente che ha diritti di amministratore del tenant.

3. Il cliente deve selezionare il collegamento e approvare la richiesta di relazione Reseller.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Esempio di messaggio di posta elettronica di Crea relazione rivenditore":::

4. Il partner deve connettersi al tenant partner per ottenere l'ID oggetto del gruppo AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Il cliente che ha il ruolo di **proprietario o amministratore accesso utenti** e dispone dell'autorizzazione per creare un'assegnazione di ruolo a livello di sottoscrizione esegue le operazioni seguenti:


    1. Stabilisce la connessione al tenant in cui esiste la sottoscrizione CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Si connette alla sottoscrizione (applicabile solo se l'utente dispone di autorizzazioni di assegnazione di ruolo per più sottoscrizioni nel tenant).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "ID sottoscrizione CSP" "


    3. Crea l'assegnazione di ruolo
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Se si desidera concedere l'autorizzazione per il ruolo di proprietario a livello di gruppo di risorse o di risorse anziché ambito di sottoscrizione, è possibile usare i comandi seguenti:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Passaggi successivi

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
