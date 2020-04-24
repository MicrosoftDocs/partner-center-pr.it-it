---
title: I clienti delegano i privilegi di amministratore ai partner | Centro per i partner
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descrive come chiedere ai clienti di delegare le autorizzazioni di amministratore a un rivenditore, rimuoverle e usarle.
author: LauraBrenner
ms.author: labrenne
keywords: privilegi di amministratore con delega, amministratore per conto terzi, rimuovere i privilegi
ms.localizationpriority: high
ms.openlocfilehash: 9b82ed4828a112f28f3e2ef1da1a64745c9ffdc0
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2020
ms.locfileid: "78340059"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>I clienti delegano i privilegi di amministratore ai partner

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Agente amministratore
- Agente di vendita

Per gestire un servizio o una sottoscrizione per conto di un cliente, quest'ultimo dovrà concederti le autorizzazioni di amministratore per tale servizio. Per ottenere le autorizzazioni di amministratore, invia al cliente una richiesta di relazione come rivenditore. Dopo che il cliente ha approvato la richiesta, potrai accedere al portale di amministrazione del servizio e gestire il servizio per conto del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire con l'utente una relazione come rivenditore

1.  Seleziona **Clienti** e quindi **Richiedi una relazione come rivenditore**.

2.  Nella pagina successiva esaminare la bozza del messaggio di posta elettronica. Puoi aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure puoi copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica. 

    >[!IMPORTANT]
    >Il testo nel messaggio di posta elettronica può essere modificato, ma è necessario assicurarsi di includere il collegamento, in quanto personalizzato, per collegare il cliente direttamente al proprio account. 
    
3.  Al termine di questo passaggio, seleziona **Fatto**.

4.  Inviare il messaggio di posta elettronica al cliente.

5.  Dopo aver accettato l'invito, il cliente verrà visualizzato nella pagina **Clienti** e potrai effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

6.  Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandi il record del cliente selezionando la freccia verso il basso accanto al nome e quindi seleziona il portale di amministrazione per il servizio che vuoi gestire.

>[!IMPORTANT]  
>I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione del servizio. Fino a quando il contratto non verrà rinegoziato con il cliente, il partner continua, tuttavia, ad avere la responsabilità di fornire supporto al cliente e rispettare le condizioni del contratto per rivenditori cloud, anche dopo che un cliente ha riassegnato o rimosso le autorizzazioni di amministratore. In questo caso, se il cliente ha bisogno di aiuto, puoi contattare il supporto tecnico Microsoft per aprire una richiesta di assistenza per conto del cliente.

I clienti possono scoprire quali partner hanno privilegi di amministratore per i propri tenant all'interno del portale di amministrazione di Office 365. A tale scopo:

1. Il cliente deve accedere al portale di amministrazione di Office 365 come amministratore globale.

2. Seleziona **Impostazioni** > **Relazioni con i partner**.

3. Nella pagina **Relazioni con i partner** il cliente visualizzerà un elenco dei partner con cui collabora e di quelli ai quali sono stati concessi privilegi di amministratore con delega per i tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>I clienti possono gestire i privilegi di amministratore con delega di un partner 

Il cliente può decidere di rimuovere i tuoi privilegi di amministratore con delega dal proprio tenant, ma di mantenere la relazione con te ai fini del rinnovo della licenza e della sottoscrizione. I clienti gestiscono i diritti e le autorizzazioni per i loro account di Office 365 nella pagina **Relazioni con i partner** nell'interfaccia di amministrazione di Office 365. In questa pagina i clienti possono:

- Vedere con quali partner hanno una relazione e quali partner dispongono dei privilegi di amministratore con delega

- Rimuovere i privilegi di amministratore con delega del partner dal tenant

Per rimuovere i privilegi di amministratore con delega di un partner:

1. Nella pagina **Relazioni con i partner** seleziona il partner di interesse.
2. Nel riquadro dei dettagli seleziona **Remove delegated admin (Rimuovi amministratore con delega)** .
3. Nel riquadro di conferma seleziona **Rimuovi**.

>[!IMPORTANT]  
>Le assegnazioni dei ruoli di Azure AD al partner sono implicite. Se tenti di elencare i membri dei ruoli di Azure AD tramite il portale di Azure AD/PowerShell/Graph, non verrà restituito il partner. Per scoprire se i partner vengono assegnati ai ruoli di Azure AD, devi consultare la pagina Relazioni con i partner nel portale di amministrazione di Office 365 e verificare se i privilegi di amministratore con delega sono stati concessi al partner.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegi di amministratore con delega in Azure AD 

Esistono due gruppi di sicurezza, gli agenti amministratore e gli agenti help desk, nel tenant di Azure AD del partner che vengono usati per l'amministrazione con delega. Quando un cliente concede i privilegi di amministratore con delega a un partner:

- Il gruppo agente amministratore viene assegnato al ruolo di amministratore globale nel tenant di Azure AD del cliente.

- Il gruppo agente help desk viene assegnato al ruolo di amministratore help desk nel tenant di Azure AD del cliente.

In base ai ruoli directory assegnati, i membri di entrambi i gruppi possono accedere al tenant di Azure AD e ai servizi di Office 365 del cliente usando l'amministratore e le credenziali del partner per conto del cliente.

Se il cliente rimuove i privilegi di amministratore con delega, vengono rimosse le assegnazioni di ruolo di Azure AD e non sarai più in grado di gestire il tenant di Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Sottoscrizioni Azure e gestione delle risorse

Ogni sottoscrizione di Azure ha un proprio gruppo di ruoli di gestione delle risorse. Prima che un partner CSP possa gestire una sottoscrizione di Azure del cliente, il partner deve essere assegnato a uno o più ruoli nella sottoscrizione di Azure. In particolare:

- Quando un cliente accetta un invito per i rivenditori e concede privilegi di amministratore con delega a un partner, il partner non accede automaticamente alle sottoscrizioni di Azure esistenti nel tenant del cliente.

- Quando un partner CSP esegue il provisioning di una nuova sottoscrizione di Azure per il cliente, al gruppo agenti amministratore nel tenant del partner CSP viene automaticamente assegnato il ruolo di proprietario ai sensi della sottoscrizione. In base a questa assegnazione di ruolo, i membri del gruppo possono accedere e gestire le risorse associate alla sottoscrizione.

- Quando un cliente rimuove i privilegi di amministratore con delega da un partner tramite il portale di Office 365, il partner può comunque gestire la sottoscrizione di Azure del cliente, purché sia ancora assegnato a uno o più ruoli nella sottoscrizione. Perché il partner interrompa la gestione della sottoscrizione di Azure, il cliente deve rimuovere l'assegnazione del ruolo.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Dal Centro per i partner, i partner CSP possono gestire i profili di Autopilot per i clienti senza privilegi di amministratore con delega nelle circostanze seguenti: 

- Se un cliente rimuove i privilegi di amministratore con delega ma mantiene una relazione come rivenditore con l'utente, puoi continuare a gestire i profili di Autopilot per il cliente.

- Puoi gestire i dispositivi del cliente aggiunti dall'utente o da un altro partner. 

- Non puoi gestire i dispositivi aggiunti dal cliente tramite Microsoft Store per le aziende, Microsoft Store per la formazione o il portale di Microsoft Intune.

Per altre informazioni su Autopilot, vedi [Semplificare la configurazione dei dispositivi con Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>L'attuale esperienza di gestione di Autopilot nel Centro per i partner è soggetta a modifiche. Al momento della pubblicazione di questo articolo, vengono considerate le modifiche seguenti:

- Al partner devono essere concessi privilegi di amministratore con delega dal cliente prima che possa aggiungere/aggiornare/applicare/rimuovere profili dai dispositivi nel tenant del cliente.

- Al partner devono essere concessi privilegi di amministratore con delega dal cliente prima che possa rimuovere dispositivi aggiunti da altri partner o dal cliente nel tenant del cliente. In caso contrario, il partner può rimuovere solo i dispositivi aggiunti in precedenza dallo stesso partner.
