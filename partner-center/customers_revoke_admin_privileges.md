---
title: I clienti delegano i privilegi amministrativi ai partner | Centro per i partner
description: Come partner rivenditore, il cliente può delegarti a essere suo amministratore. Può anche rimuovere i privilegi.
author: labrenne
keywords: privilegi di amministratore delegato, amministrazione per conto di, rimuovere i privilegi
ms.openlocfilehash: 7f1bd81f40892f851e1582a7a842a64c55e4ff63
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2018
ms.locfileid: "1913949"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>I clienti delegano i privilegi amministrativi ai partner

**Ambito di applicazione:**

-  Centro per i partner

Come partner CSP e consulente fidato che supporta i clienti, puoi essere delegato come amministratore per i tenant di Azure AD e Office 365. Puoi avviare tale relazione tramite il dashboard per i partner inviando un invito. 

1. Seleziona **Clienti** dal **Dashboard**, quindi **Richiesta di una relazione con un cliente**.
2. Verrà visualizzato un messaggio e-mail con modulo contenente il tuo url. Puoi copiare e incollare il modulo in un messaggio e-mail da inviare al cliente. Sei libero di aggiungere altre informazioni, ma assicurati di includere l'url. Il cliente utilizzerà tale url per rispondere alla tua richiesta.  
3. Quando il cliente accetta l'invito, diventi l'amministratore dei suoi servizi.

I clienti possono scoprire quali partner hanno privilegi di amministratore per i propri tenant all'interno del portale del servizio Office 365. A tale scopo, effettua le seguenti operazioni:

1. Accedi al [portale di Amministrazione di Office 365](https://portal.office.com/adminportal) come amministratore globale.
2. Seleziona **Impostazioni** → **Relazioni con i partner**.
3. Nella pagina **Relazioni con i partner** verrà visualizzato un elenco dei partner con cui collaborano e di quelli ai quali sono stati concessi privilegi di amministratore delegato per i loro tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>I clienti possono gestire i privilegi di amministratore delegato di un partner. 

Il tuo cliente può decidere di rimuovere i tuoi privilegi di amministrazione dal proprio tenant, ma di mantenere la relazione con te ai fini del rinnovo della licenza e della sottoscrizione. I clienti gestiscono i diritti e le autorizzazioni per i loro account di Office 365 nella pagina **Relazioni con i partner** nell'interfaccia di amministrazione di Office 365. In questa pagina i clienti possono:

- Vedere con quali partner hanno una relazione e quali partner hanno privilegi di amministratore delegato

- Rimuovere i privilegi di amministratore delegato del partner dal tenant

Per rimuovere i privilegi di amministratore delegato di un partner:

1. Nella pagina **Relazioni con i partner** seleziona il partner di interesse.
2. Nel riquadro dei dettagli seleziona **Rimuovi amministratore delegato**.
3. Nel riquadro di conferma seleziona **Rimuovi**.

>**Importante**<br>
Le assegnazioni dei ruoli di Azure AD al partner sono implicite. Se tenti di elencare i membri dei ruoli di Azure AD tramite il portale di Azure AD/PowerShell/Graph, non verrà restituito il partner. Per scoprire se i partner vengono assegnati ai ruoli di Azure AD, devi consultare la pagina Relazioni con i partner nel portale di amministrazione di Office 365 e vedere se i privilegi di amministratore delegato sono stati concessi al partner.

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

Nel dashboard per i partner, i partner CSP possono gestire la configurazione Autopilot per i loro clienti anche senza privilegi di amministratore delegato. Scopri come [Semplificare la configurazione dei dispositivi con Windows Autopilot.](https://docs.microsoft.com/partner-center/autopilot)

Ciò che puoi fare dipende dal fatto che tu sia un rivenditore diretto o indiretto.

|**Operazione**   |**Rivenditore diretto o indiretto**   |**Rivenditore indiretto**   |
|-----------------|-----------------------------------| -----------------------------|
|Aggiungere dispositivi (tramite file csv)  |Sì      |No|
|Rimuovere dispositivi   |Sì   |No|
|Aggiungere profilo   |Sì   | Sì   |
|Aggiornare profilo   |Sì    |Sì   |
|Rimuovere profilo   |Sì   |Sì   |
|Applicare profilo a dispositivi   |Sì   |Sì   |
|Rimuovere profilo da dispositivi   |Sì   |Sì   | 

- I partner CSP possono continuare a gestire la configurazione Autopilot per i clienti esistenti con una relazione come rivenditore, anche se i clienti hanno rimosso i privilegi di amministratore delegato dai relativi partner.

- Puoi gestire i dispositivi esistenti per i clienti aggiunti da te o da un altro partner CSP.

- Non puoi gestire i dispositivi caricati dal cliente (tramite Microsoft Store per le aziende o il portale di Microsoft Intune).

>**Importante**: l'esperienza di gestione corrente di Autopilot nel Centro per i partner di Microsoft non è finale ed è soggetta a cambiamenti futuri. Al momento della realizzazione di questo articolo vengono considerate le modifiche seguenti:

  - Al partner devono essere concessi privilegi di amministratore delegato dal cliente prima che possa aggiungere/aggiornare/rimuovere profili dai dispositivi nel tenant del cliente.

- Al partner devono essere concessi privilegi di amministratore delegato dal cliente prima che possa rimuovere dispositivi caricati da altri partner o dal cliente nel tenant del cliente. In caso contrario, il partner può rimuovere solo i dispositivi aggiunti in precedenza dallo stesso partner.
