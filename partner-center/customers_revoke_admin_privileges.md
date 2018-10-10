---
title: I clienti delegano i privilegi amministrativi ai partner | Centro per i partner
description: Come partner rivenditore, il cliente può puoi essere delegato loro come amministratore. È possibile anche rimuovere i privilegi.
author: labrenne
keywords: privilegi di amministratore delegato, amministrazione per conto di, rimuovere i privilegi, DAP, of AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 224ed2ea2485420761c7a5f85db5a7a37fd245af
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489877"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>I clienti delegano i privilegi amministrativi ai partner

**Ambito di applicazione:**

-  Centro per i partner

Per gestire un servizio o una sottoscrizione per conto di un cliente, quest'ultimo dovrà concederti le autorizzazioni di amministratore per tale servizio. Per ottenere le autorizzazioni di amministratore, invia al cliente una richiesta di relazione come rivenditore. Dopo che il cliente ha approvato la richiesta, potrai accedere al portale di amministrazione del servizio e gestire il servizio per conto del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire una relazione come rivenditore con te

1.  Seleziona **i clienti** e quindi seleziona **richiedere una relazione come rivenditore**.

2.  Nella pagina successiva controlla la bozza del messaggio di posta elettronica. Puoi aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure puoi copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica. 

    >! IMPORTANTE<br>
    >Il testo nel messaggio di posta elettronica può essere modificato, ma assicurati di includere il collegamento poiché è personalizzato per collegare il cliente direttamente al tuo account. 
    
3.  Al termine di questo passaggio, seleziona **Fatto**.

4.  Invia il messaggio di posta elettronica al cliente.

5.  Dopo aver accettato l'invito, il cliente verrà visualizzato nella pagina **Clienti** e tu potrai effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

6.  Per la gestione di account, servizi, gli utenti e licenze del cliente, Espandi il record del cliente selezionando la freccia giù accanto al nome e quindi seleziona il portale di amministrazione per il servizio che desideri gestire.


> [!IMPORTANT]  
> I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione del servizio. Tuttavia, fino a quando il contratto non verrà rinegoziato con il cliente, il partner continua ad avere la responsabilità di fornire supporto al cliente e rispettare le condizioni del contratto per rivenditori cloud, anche dopo che un cliente ha riassegnato o rimosso le autorizzazioni di amministratore. In questo caso, se il cliente ha bisogno di assistenza, contattare il supporto Microsoft per aprire una richiesta di servizio per conto del cliente.

I clienti possono scoprire quali i partner hanno privilegi di amministratore per i propri tenant all'interno del portale di amministrazione di Office 365. A tale scopo, effettua le seguenti operazioni:

1. Il cliente necessita di accedere al portale di amministrazione di Office 365 come un amministratore globale.

2. Seleziona **Impostazioni** → **Relazioni con i partner**.

3. Nella pagina **relazioni con i Partner** , il cliente verrà visualizzato un elenco dei partner con cui funzionano e quelli che sono stati concessi privilegi di amministrazione per i propri tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>I clienti possono gestire i privilegi di amministratore delegato di un partner. 

Il cliente può decidere di rimuovere i privilegi di amministratore delegato dal proprio tenant, ma di mantenere la relazione con te ai fini del rinnovo della licenza e della sottoscrizione. I clienti gestiscono i diritti e le autorizzazioni per i loro account di Office 365 nella pagina **Relazioni con i partner** nell'interfaccia di amministrazione di Office 365. In questa pagina i clienti possono:

- Vedere con quali partner hanno una relazione e quali partner hanno privilegi di amministratore delegato

- Rimuovere i privilegi di amministratore delegato del partner dal tenant

Per rimuovere i privilegi di amministratore delegato di un partner:

1. Nella pagina **Relazioni con i partner** seleziona il partner di interesse.
2. Nel riquadro dei dettagli seleziona **Rimuovi amministratore delegato**.
3. Nel riquadro di conferma seleziona **Rimuovi**.

> [!IMPORTANT]  
> Le assegnazioni dei ruoli di Azure AD al partner sono implicite. Se tenti di elencare i membri dei ruoli di Azure AD tramite il portale di Azure AD/PowerShell/Graph, non verrà restituito il partner. Per scoprire se i partner vengono assegnati ai ruoli di Azure AD, devi consultare la pagina Relazioni con i partner nel portale di amministrazione di Office 365 e vedere se i privilegi di amministratore delegato sono stati concessi al partner.

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

Centro per i Partner, i partner CSP possono gestire i profili Autopilot per i loro clienti senza privilegi di amministratore. Scopri come [Semplificare la configurazione dei dispositivi con Windows Autopilot.](https://docs.microsoft.com/partner-center/autopilot)

Cosa puoi fare dipende dal modo in quale modello CSP sei iscritto.

|**Operazione**   |**Per i partner di addebito diretto e provider indiretto**   |**Rivenditore indiretto**   |
|-----------------|-----------------------------------| -----------------------------|
|Aggiungere dispositivi (tramite file csv)  |Sì      |No|
|Rimuovere dispositivi   |Sì   |No|
|Aggiungere profilo   |Sì   | Sì   |
|Aggiornare profilo   |Sì    |Sì   |
|Rimuovere profilo   |Sì   |Sì   |
|Applicare profilo a dispositivi   |Sì   |Sì   |
|Rimuovere profilo da dispositivi   |Sì   |Sì   | 

- Se un cliente rimuove i privilegi aministration privilegi di amministratore delegato, ma mantiene una relazione come rivenditore con te, puoi continuare a gestire i profili Autopilot per loro.

- È possibile gestire i dispositivi dei clienti che hanno aggiunto puoi o un altro partner. 

- Non puoi gestire i dispositivi che il cliente ha aggiunto tramite il Microsoft Store per le aziende, Microsoft Store per gli istituti di istruzione o portale di Microsoft Intune.

> [!IMPORTANT]  
> L'esperienza di gestione corrente di Autopilot nel centro per i Partner possa continuare a modificare. Al momento della che pubblicazione di questo articolo, vengono considerate le modifiche seguenti:

  - Al partner devono essere concessi privilegi di amministratore delegato dal cliente prima che possa aggiungere/aggiornare/rimuovere profili dai dispositivi nel tenant del cliente.

- Per i partner devono essere concessi privilegi di amministratore delegato dal cliente prima che il partner può rimuovere i dispositivi aggiunti da altri partner o dal cliente nel tenant del cliente. In caso contrario, il partner può rimuovere solo i dispositivi aggiunti in precedenza dallo stesso partner.
