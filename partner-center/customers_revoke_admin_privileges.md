---
title: I clienti delegano i privilegi amministrativi ai partner | Centro per i partner
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come richiedere ai clienti di delegare le autorizzazioni di amministratore a un rivenditore o rimuovere le stesse autorizzazioni e come usare le autorizzazioni.
author: LauraBrenner
ms.author: labrenne
keywords: privilegi amministrativi delegati, amministratore per conto di, Rimuovi privilegi, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253476"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>I clienti delegano i privilegi amministrativi ai partner

**Si applica a**

-  Centro per i partner

Per gestire un servizio o una sottoscrizione per conto di un cliente, quest'ultimo dovrà concederti le autorizzazioni di amministratore per tale servizio. Per ottenere le autorizzazioni di amministratore, invia al cliente una richiesta di relazione come rivenditore. Dopo che il cliente ha approvato la richiesta, potrai accedere al portale di amministrazione del servizio e gestire il servizio per conto del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire con te una relazione come rivenditore

1.  Selezionare **Customers** e quindi selezionare **Richiedi una relazione Reseller**.

2.  Nella pagina successiva esaminare la bozza del messaggio di posta elettronica. Puoi aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure puoi copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica. 

    >[!IMPORTANT]
    >Il testo nel messaggio di posta elettronica può essere modificato, ma assicurati di includere il collegamento poiché è personalizzato per collegare il cliente direttamente al tuo account. 
    
3.  Selezionare **fine** al termine di questo passaggio.

4.  Invia il messaggio di posta elettronica al cliente.

5.  Dopo aver accettato l'invito, il cliente verrà visualizzato nella pagina **Clienti** e tu potrai effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

6.  Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandere il record del cliente selezionando la freccia verso il basso accanto al nome e quindi selezionare il portale di amministrazione per il servizio che si vuole gestire.

>[!IMPORTANT]  
>I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione del servizio. Tuttavia, fino a quando il contratto non verrà rinegoziato con il cliente, il partner continua ad avere la responsabilità di fornire supporto al cliente e rispettare le condizioni del contratto per rivenditori cloud, anche dopo che un cliente ha riassegnato o rimosso le autorizzazioni di amministratore. In questa situazione, se il cliente richiede assistenza, contattare il supporto tecnico Microsoft per aprire una richiesta di assistenza per conto del cliente.

I clienti possono scoprire quale partner hanno privilegi di amministratore per il tenant dall'interno del portale di amministrazione di Office 365. A tale scopo, effettua le seguenti operazioni:

1. Il cliente deve accedere al portale di amministrazione di Office 365 come amministratore globale.

2. Selezionare **impostazioni** > **Relazioni partner**.

3. Nella pagina **Relazioni partner** , il cliente visualizzerà un elenco dei partner a cui lavorano e quelli a cui sono stati concessi privilegi di Amministrazione delegati al tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>I clienti possono gestire i privilegi amministrativi delegati di un partner 

Il cliente può decidere di rimuovere i privilegi amministrativi delegati dal tenant, mantenendo la relazione con l'utente per finalità di rinnovo della licenza e della sottoscrizione. I clienti gestiscono i diritti e le autorizzazioni per i loro account di Office 365 nella pagina **Relazioni con i partner** nell'interfaccia di amministrazione di Office 365. In questa pagina i clienti possono:

- Vedere con quali partner hanno una relazione e quali partner hanno privilegi di amministratore delegato

- Rimuovere i privilegi di amministrazione delegata di un partner dal tenant

Per rimuovere i privilegi di amministratore delegato di un partner:

1. Nella pagina **Relazioni con i partner** seleziona il partner di interesse.
2. Nel riquadro dei dettagli seleziona **Rimuovi amministratore delegato**.
3. Nel riquadro di conferma seleziona **Rimuovi**.

>[!IMPORTANT]  
>Le assegnazioni dei ruoli di Azure AD al partner sono implicite. Se tenti di elencare i membri dei ruoli di Azure AD tramite il portale di Azure AD/PowerShell/Graph, non verrà restituito il partner. Per scoprire se i partner vengono assegnati ai ruoli di Azure AD, devi consultare la pagina Relazioni con i partner nel portale di amministrazione di Office 365 e vedere se i privilegi di amministratore delegato sono stati concessi al partner.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegi di amministratore delegato in Azure AD 

Nel tenant Azure AD del partner sono presenti due gruppi di sicurezza, agenti di amministrazione e agenti helpdesk, usati per l'amministrazione delegata. Quando un cliente concede i privilegi di amministratore delegato a un partner:

- Il gruppo di agenti di amministrazione viene assegnato al ruolo di amministratore globale nel tenant Azure AD del cliente.

- Il gruppo di agenti helpdesk viene assegnato al ruolo di amministratore del supporto tecnico nel tenant Azure AD del cliente.

In base ai ruoli della directory assegnati, i membri di entrambi i gruppi possono accedere al tenant Azure AD del cliente e ai servizi O365 usando le credenziali del partner e l'amministratore per conto del cliente.

Se il cliente rimuove i privilegi amministrativi delegati, le assegnazioni di ruolo Azure AD vengono rimosse e non sarà più possibile gestire il tenant di Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Sottoscrizioni Azure e gestione delle risorse

Ogni sottoscrizione di Azure ha un proprio gruppo di ruoli di gestione delle risorse. Prima che un partner CSP possa gestire la sottoscrizione di Azure di un cliente, il partner deve essere assegnato a uno o più ruoli nella sottoscrizione di Azure. In particolare:

- Quando un cliente accetta un invito per i rivenditori e concede privilegi di amministratore delegato a un partner, il partner non accede automaticamente alle sottoscrizioni di Azure esistenti nel tenant del cliente.

- Quando un partner CSP esegue il provisioning di una nuova sottoscrizione di Azure per il cliente, al gruppo Agenti amministratore nel tenant del partner CSP viene automaticamente assegnato il ruolo di proprietario ai sensi della sottoscrizione. In base a questa assegnazione di ruolo, i membri del gruppo possono accedere e gestire le risorse associate alla sottoscrizione.

- Quando un cliente rimuove i privilegi di amministrazione delegata da un partner usando il portale di Office 365, il partner può comunque gestire la sottoscrizione di Azure del cliente, purché il partner sia ancora assegnato a uno o più ruoli nella sottoscrizione. Perché il partner interrompa la gestione della sottoscrizione di Azure, il cliente deve rimuovere l'assegnazione del ruolo.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Dal centro per i partner, i partner CSP possono gestire i profili di Autopilot per i clienti senza privilegi amministrativi delegati in queste circostanze: 

- Se un cliente rimuove i privilegi di amministrazione delegata ma mantiene una relazione del rivenditore, è possibile continuare a gestire i profili Autopilot.

- È possibile gestire i dispositivi dei clienti aggiunti dall'utente o da un altro partner. 

- Non è possibile gestire i dispositivi aggiunti dal cliente tramite il Microsoft Store per le aziende, Microsoft Store per la formazione o Microsoft Intune portale.

Per ulteriori informazioni su AUTOPILOT, vedere [semplificare la configurazione del dispositivo con Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L'esperienza di gestione di Autopilot attuale nel centro per i partner potrebbe continuare a cambiare. Al momento della pubblicazione di questo articolo, verranno prese in considerazione le seguenti modifiche:

- Al partner devono essere concessi privilegi di amministratore delegato dal cliente prima che possa aggiungere/aggiornare/rimuovere profili dai dispositivi nel tenant del cliente.

- Al partner è necessario concedere il privilegio di amministrazione delegata dal cliente prima che il partner possa rimuovere i dispositivi aggiunti da altri partner o dal cliente nel tenant del cliente. In caso contrario, il partner può rimuovere solo i dispositivi aggiunti in precedenza dallo stesso partner.
