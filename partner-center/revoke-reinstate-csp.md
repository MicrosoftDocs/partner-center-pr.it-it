---
title: Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP | Centro per i partner
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Questo documento illustra come aiutare i clienti a ripristinare i privilegi di amministratore del partner
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 1bcbcf32e3b3f4513ed3e55984b49b090da4a734
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2020
ms.locfileid: "73651708"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP  

**Ruoli applicabili**

- Amministratore globale
- Agente amministratore

Da un partner CSP come te, i clienti si aspettano in genere che tu gestisca l'utilizzo di Azure e i sistemi per loro conto. A questo scopo, devi avere privilegi di amministratore. Alcuni privilegi vengono concessi quando viene stabilita la relazione di rivenditore con il cliente, mentre altri ti vengono concessi dal cliente.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegi di amministratore per Azure in CSP 

Esistono due livelli di privilegi di amministratore per Azure in CSP. 

**Privilegi di amministratore a livello di tenant** (**privilegi di amministratore con delega**): i partner CSP ottengono questi privilegi quando stabiliscono la relazione di rivenditore CSP con i clienti. In questo modo, i partner CSP possono accedere ai tenant dei clienti ed eseguire funzioni amministrative, ad esempio l'aggiunta o la gestione degli utenti, la reimpostazione delle password e la gestione delle licenze utente. 

**Privilegi di amministratore a livello di sottoscrizione**: i partner CSP ottengono questi privilegi durante la creazione delle sottoscrizioni di Azure CSP per i clienti. In questo modo, i partner CSP possono accedere a queste sottoscrizioni ed effettuare il provisioning e la gestione delle risorse di Azure. 


## <a name="reinstate-csp-partners-admin-privileges"></a>Ripristinare i privilegi di amministratore dei partner CSP

Per ottenere nuovamente i privilegi amministrativi delegati, devi collaborare con il cliente.
 
 1. Accedi al dashboard Centro per i partner e scegli **Clienti** dal menu del Centro per i partner.

 2. Seleziona il cliente con cui stai collaborando e **richiedi una relazione di rivenditore**. Viene generato un collegamento al cliente che ha diritti di amministratore del tenant.

 3. Tale utente deve selezionare il collegamento e approvare la richiesta di relazione di rivenditore.
 
![relazione di rivenditore](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Aggiunta del gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP

 Il cliente dovrà aggiungere il gruppo di agenti di amministrazione come proprietario della sottoscrizione di Azure CSP.

1. Usa la console di PowerShell o l'ambiente di scripting integrato (ISE) di PowerShell. Verifica che siano installati i moduli AzureRM e AzureAD. 

2.  Connettiti al tenant di Azure AD.
Cmdlet di PowerShell: Connect-AzureAD

3.  Ottieni ObjectId dei gruppi di agenti di amministrazione.
Cmdlet di PowerShell: Get-AzureADGroup`1nn

![gruppo di agenti di amministrazione](images/azure/revoke5.png)

I passaggi seguenti vengono eseguiti dall'utente nell'azienda del cliente che ha accesso proprietario alla sottoscrizione di Azure CSP.

4. L'utente con accesso proprietario alla sottoscrizione di Azure CSP accede ad Azure Resource Manager usando le proprie credenziali.

    Cmdlet di PowerShell: Login-AzureRMAccount

5.  Può quindi aggiungere il gruppo di agenti di amministrazione come proprietario alla sottoscrizione di Azure CSP.

    Cmdlet di PowerShell: New-AzureRMRoleAssignment -ObjectId < ID oggetto ottenuto dal passaggio 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![proprietari agenti di amministrazione](images/azure/revoke6.png)    

**Per altre informazioni**

[Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)
