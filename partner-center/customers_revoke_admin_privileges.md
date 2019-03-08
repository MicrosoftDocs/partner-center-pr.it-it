---
title: I clienti delegano i privilegi amministrativi ai partner | Centro per i partner
ms.topic: article
ms.date: 12/18/2018
description: I partner rivenditori può delegare il cliente è necessario essere l'amministratore. Inoltre, possono rimuovere i privilegi.
author: LauraBrenner
ms.author: labrenne
keywords: privilegi di amministratore delegato, amministratore per conto di, rimuovere i privilegi, delegato, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 9253bcca2d93d9f0d62d6d7241132f0c0c9bf5ec
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586154"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>I clienti delegano i privilegi amministrativi ai partner

**Si applica a**

-  Centro per i partner

Per gestire un servizio o una sottoscrizione per conto di un cliente, quest'ultimo dovrà concederti le autorizzazioni di amministratore per tale servizio. Per ottenere le autorizzazioni di amministratore, invia al cliente una richiesta di relazione come rivenditore. Dopo che il cliente ha approvato la richiesta, potrai accedere al portale di amministrazione del servizio e gestire il servizio per conto del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire con te una relazione come rivenditore

1.  Selezionare **clienti** e quindi selezionare **richiedere una relazione di rivendita**.

2.  Nella pagina successiva esamina la bozza del messaggio di posta elettronica. Puoi aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure puoi copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica. 

    >[!IMPORTANT]
    >Il testo nel messaggio di posta elettronica può essere modificato, ma assicurati di includere il collegamento poiché è personalizzato per collegare il cliente direttamente al tuo account. 
    
3.  Al termine di questo passaggio, seleziona **Fatto**.

4.  Invia il messaggio di posta elettronica al cliente.

5.  Dopo aver accettato l'invito, il cliente verrà visualizzato nella pagina **Clienti** e tu potrai effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

6.  Per gestire l'account del cliente, servizi, gli utenti e licenze, espandere il record del cliente, selezionando la freccia verso il basso accanto al nome e quindi selezionare il portale di amministrazione per il servizio che si desidera gestire.

>[!IMPORTANT]  
>I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione di un servizio. Tuttavia, fino a quando il contratto non verrà rinegoziato con il cliente, il partner continua ad avere la responsabilità di fornire supporto al cliente e rispettare le condizioni del contratto per rivenditori cloud, anche dopo che un cliente ha riassegnato o rimosso le autorizzazioni di amministratore. In questo caso, se il cliente richiede assistenza, contattare il supporto Microsoft per aprire una richiesta di servizio per conto del cliente.

I clienti possono scoprire quali i rispettivi partner hanno privilegi di amministratore per il tenant all'interno del portale di amministrazione di Office 365. A tale scopo, effettuare le seguenti operazioni:

1. Il cliente deve eseguire l'accesso al portale di amministrazione di Office 365 come amministratore globale.

2. Seleziona **Impostazioni** → **Relazioni con i partner**.

3. Nel **relazioni di Partner** pagina, il cliente verrà visualizzato un elenco dei partner con cui lavorano e quelli che sono stati concessi delegare i privilegi di amministrazione a loro tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>I clienti possono gestire i privilegi di amministratore delegato di un partner. 

Il cliente può decidere di rimuovere i privilegi di amministratore delegato dal tenant, ma conserva la relazione con l'utente per la sottoscrizione e i rinnovi di licenza. I clienti gestiscono i diritti e le autorizzazioni per i loro account di Office 365 nella pagina **Relazioni con i partner** nell'interfaccia di amministrazione di Office 365. In questa pagina i clienti possono:

- Vedere con quali partner hanno una relazione e quali partner hanno privilegi di amministratore delegato

- Rimuovere i privilegi di amministratore delegato del partner dal tenant

Per rimuovere i privilegi di amministratore delegato di un partner:

1. Nella pagina **Relazioni con i partner** seleziona il partner di interesse.
2. Nel riquadro dei dettagli seleziona **Rimuovi amministratore delegato**.
3. Nel riquadro di conferma seleziona **Rimuovi**.

>[!IMPORTANT]  
>Le assegnazioni dei ruoli di Azure AD al partner sono implicite. Se tenti di elencare i membri dei ruoli di Azure AD tramite il portale di Azure AD/PowerShell/Graph, non verrà restituito il partner. Per scoprire se i partner vengono assegnati ai ruoli di Azure AD, devi consultare la pagina Relazioni con i partner nel portale di amministrazione di Office 365 e vedere se i privilegi di amministratore delegato sono stati concessi al partner.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegi di amministratore delegato in Azure AD 

Esistono due gruppi di sicurezza, gli Agenti amministratore e gli Agenti help desk, nel tenant di Azure AD del partner che vengono utilizzati per l'amministrazione delegata. Quando un cliente concede i privilegi di amministratore delegato a un partner:

- Il gruppo Agente amministratore viene assegnato al ruolo di Amministratore globale nel tenant di Azure AD del cliente.

- Il gruppo Agente help desk viene assegnato al ruolo di Amministratore help desk nel tenant di Azure AD del cliente.

In base ai ruoli directory assegnati, i membri di entrambi i gruppi possono accedere al tenant di Azure AD e ai servizi di Office 365 del cliente utilizzando l'amministratore e le credenziali del partner per conto del cliente.

Se il cliente rimuove i privilegi di amministratore delegato, vengono rimosse le assegnazioni di ruolo di Azure AD e non sarai più in grado di gestire il tenant di Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Sottoscrizioni Azure e gestione delle risorse

Ogni sottoscrizione di Azure ha un proprio gruppo di ruoli di gestione delle risorse. Prima che un partner CSP possa gestire una sottoscrizione di Azure del cliente, il partner deve essere assegnato a uno o più ruoli nella sottoscrizione di Azure. In particolare:

- Quando un cliente accetta un invito per i rivenditori e concede privilegi di amministratore delegato a un partner, il partner non accede automaticamente alle sottoscrizioni di Azure esistenti nel tenant del cliente.

- Quando un partner CSP esegue il provisioning di una nuova sottoscrizione di Azure per il cliente, al gruppo Agenti amministratore nel tenant del partner CSP viene automaticamente assegnato il ruolo di proprietario ai sensi della sottoscrizione. In base a questa assegnazione di ruolo, i membri del gruppo possono accedere e gestire le risorse associate alla sottoscrizione.

- Quando un cliente rimuove i privilegi di amministratore delegato da un partner tramite il portale di Office 365, il partner può comunque gestire la sottoscrizione di Azure del cliente, purché sia ancora assegnato a uno o più ruoli nella sottoscrizione. Perché il partner interrompa la gestione della sottoscrizione di Azure, il cliente deve rimuovere l'assegnazione del ruolo.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Dal centro per i Partner, i partner CSP possono gestire i profili di Autopilot per i clienti senza privilegi di amministratore con delega in queste circostanze: 

- Se un cliente rimuove i privilegi di amministrazione delegata, ma mantiene una relazione di rivendita con l'utente, è possibile continuare a gestire i profili di Autopilot per loro.

- È possibile gestire i dispositivi dei clienti che hanno aggiunto si o un altro partner. 

- Non è possibile gestire i dispositivi che del cliente ha aggiunto tramite il Microsoft Store per le aziende, Microsoft Store per la formazione o il portale di Microsoft Intune.

Per altre informazioni sulle Autopilot, vedere [semplificare l'installazione del dispositivo con Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L'esperienza di gestione di Autopilot corrente nel centro per i Partner potrà continuare a modificare. Al momento che della pubblicazione dell'articolo, vengono considerate le modifiche seguenti:

- Al partner devono essere concessi privilegi di amministratore delegato dal cliente prima che possa aggiungere/aggiornare/rimuovere profili dai dispositivi nel tenant del cliente.

- Partner è necessario concedere i privilegi di amministrazione delegata dal cliente prima che il partner può rimuovere i dispositivi aggiunti da altri partner o dal cliente nel tenant del cliente. In caso contrario, il partner può rimuovere solo i dispositivi aggiunti in precedenza dal partner stesso.
