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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP di un cliente  

**Ruoli applicabili**

- Amministratore globale
- Agente amministratore

Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto. A tale scopo, è necessario disporre dei privilegi di amministratore. Alcuni privilegi vengono concessi quando viene stabilita la relazione di rivenditore con il cliente, mentre altri ti vengono concessi dal cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegi di amministratore per Azure in CSP

Esistono due livelli di privilegi di amministratore per Azure in CSP.

**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti. In questo modo, i partner CSP possono accedere ai tenant dei clienti ed eseguire funzioni amministrative, ad esempio l'aggiunta o la gestione degli utenti, la reimpostazione delle password e la gestione delle licenze utente.

**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti. Con questi privilegi, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Ripristinare i privilegi di amministratore dei partner CSP

Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.

1. Accedi al dashboard Centro per i partner e scegli **Clienti** dal menu del Centro per i partner.

2. Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**. Viene generato un collegamento al cliente che ha diritti di amministratore del tenant.

3. Tale utente deve selezionare il collegamento e approvare la richiesta di relazione di rivenditore.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Relazione di rivenditore":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Aggiunta del gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP

Il cliente dovrà aggiungere il gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP.

1. Usa la console di PowerShell o l'ambiente di scripting integrato (ISE) di PowerShell. Verificare che i moduli AzureAD siano installati.

2. Connettiti al tenant di Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Ottieni ObjectId dei gruppi di agenti di amministrazione.

   ```powershell
   Get-AzureADGroup
   ```
   I passaggi seguenti vengono eseguiti dall'utente nell'azienda del cliente che ha accesso proprietario alla sottoscrizione di Azure CSP.

4. L'utente con accesso proprietario alla sottoscrizione di Azure CSP accede ad Azure usando le credenziali personali.

   ```powershell
   Connect-AzAccount
   ```

5. Può quindi aggiungere il gruppo di agenti di amministrazione come proprietario alla sottoscrizione di Azure CSP.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>Passaggi successivi

[Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
