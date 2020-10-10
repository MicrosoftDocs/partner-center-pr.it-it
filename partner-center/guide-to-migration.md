---
title: Eseguire la migrazione da Partner Membership Center al Centro per i partner
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come eseguire la migrazione dell'organizzazione da Partner Membership Center (PMC) al Centro per i partner.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c863f8b0942b38bab80cd97e72a85935bde2ba7c
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663832"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guida alla migrazione da Partner Membership Center (PMC) al Centro per i partner

**Ruoli appropriati**

- Amministratore globale

Il sito Web dei partner Microsoft disponibile all'indirizzo partner.microsoft.com offre ai partner un'esperienza digitale unificata. Dal sito Web dei partner potrai esplorare le opportunità disponibili e lasciarti coinvolgere in esperienze guidate che aiuteranno la tua azienda a creare e vendere app e servizi con Microsoft. Tramite il collegamento Dashboard, disponibile ovunque nel sito Web dei partner, i membri di Microsoft Partner Network possono accedere al Centro per i partner per gestire il rapporto con Microsoft, iscriversi ai programmi e registrarsi per le offerte.

Le autorizzazioni a Partner Membership Center (PMC) stanno per essere rimosse. La tua azienda è stata invitata a eseguire la transizione dalla gestione delle appartenenze di Microsoft Partner Network al Centro per i partner. Questa guida ti preparerà a eseguire le attività previste quando si passa da PMC al Centro per i partner.

>[!NOTE]
>Anche se la tua azienda ha più account o posizioni, il passaggio al Centro per i partner inizia con lo spostamento di un account (il primo) al Centro per i partner.

## <a name="get-started"></a>Operazioni preliminari

Lo spostamento inizia in PMC. L'amministratore globale riceverà un invito per iniziare lo spostamento.

### <a name="prepare-in-pmc"></a>Eseguire la preparazione in PMC

- Verifica i dettagli aziendali.
- Verifica il contatto principale del programma.
- Verifica le sedi aziendali.
- Aggiorna gli utenti approvati.

### <a name="when-youre-ready"></a>Quando si è pronti

Seleziona **Inizia** nell'invito ricevuto. Verrà visualizzata la pagina di accesso al Centro per i partner.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Attività iniziali":::

## <a name="start-with-your-work-email"></a>Inizia con l'indirizzo e-mail di lavoro

Se la tua azienda non dispone di un indirizzo e-mail aziendale e di un tenant AAD, potrai configurarli durante la procedura di accesso al Centro per i partner. Quando provi ad accedere con un account e-mail non aziendale, ad esempio con l'account personale, ti verrà chiesto di fornire informazioni sulla tua azienda in modo che sia possibile configurare un tenant AAD e un indirizzo e-mail aziendale. Poiché questi dettagli aziendali verranno usati per finalizzare il tuo account nel Centro per i partner, assicurati che siano corretti.

>[!NOTE]
>Se sei un partner con sede in Cina e sei iscritto ai programmi Microsoft Partner Network e Cloud Solution Provider (CSP), avrai un tenant separato per ogni account. L'account del programma Cloud Solution Provider viene gestito nel cloud nazionale, mentre l'account di Microsoft Partner Network viene gestito nel cloud globale. Non è possibile collegare i due account.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Attività iniziali":::

Dopo aver verificato o aggiornato le informazioni, seleziona **Accetta e continua**.
Le condizioni riportate in questa pagina sono **esattamente le stesse** contenute nel contratto firmato dalla tua azienda in PMC.  
In questo modo verrà avviata la creazione del tuo tenant di Azure AD e ti verrà fornito l'account aziendale.

Selezionando **Accetta e continua** vengono eseguite anche le operazioni seguenti:

- Migrazione del tuo account insieme a TUTTE le relative posizioni al Centro per i partner

- Migrazione di tutti i MAP o le competenze che hai acquistato in PMC

- Migrazione di eventuali risorse, offerte e programmi di marketing (MAP, Silver e Gold) disponibili in PMC

## <a name="invite-employees-to-join-you"></a>Invitare i dipendenti a partecipare

Quando viene creato il nuovo tenant di Azure AD, puoi invitare i tuoi dipendenti ad accedere al Centro per i partner.

:::image type="content" source="images/migration/invite.png" alt-text="Attività iniziali":::

Se hai eseguito l'accesso con un tenant AAD esistente, i dipendenti sono stati spostati con te. In questo caso, assegna ai dipendenti ruoli specifici per definire le operazioni che possono eseguire nel Centro per i partner. 

>[!NOTE] 
>i ruoli nel Centro per i partner sono diversi dai ruoli in PMC. Per altre informazioni, vedi [Passaggio dal Partner Membership Center al Centro per i partner](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Verificare il dominio e diventare un amministratore globale  

Se il tenant AAD è nuovo, il ruolo di amministratore globale non è assegnato a nessuno. Per diventare l'amministratore globale, devi verificare la proprietà del dominio. A tale scopo, potresti aver bisogno dell'assistenza dell'amministratore di dominio.

Fino a quando il passaggio di assegnazione di un amministratore globale non sarà stato completato, le nuove offerte non risulteranno disponibili per l'acquisto, mentre quelle già acquistate potranno continuare a essere usate.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Attività iniziali":::

Quando selezioni Inizia, verrà visualizzata la schermata seguente:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Attività iniziali":::

Il registrar risulterà già compilato. Solo il proprietario del dominio può aggiornare il file DNS. Copiando e aggiungendo il file di testo al tuo record DNS, potremo quindi verificare che tu sei il proprietario. L'aggiornamento può richiedere alcuni minuti. Dovrai disconnetterti dal Centro per i partner e quindi eseguire di nuovo l'accesso. A questo punto, il tuo ruolo risulterà modificato in amministratore globale.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Acquisire familiarità con il dashboard e il Centro per i partner

Segui la presentazione del dashboard. In questo ambiente puoi gestire l'appartenenza, aggiungere un profilo di business per le segnalazioni, iscriverti al programma Cloud Solution Provider e visualizzare le notifiche e le offerte pertinenti per la tua azienda in qualsiasi momento selezionando **Dashboard**. Puoi anche gestire gli incentivi, acquistare nel marketplace, registrarti per i servizi go-to-market e molto altro.  

:::image type="content" source="images/migration/fre.png" alt-text="Attività iniziali":::

## <a name="sign-the-microsoft-partner-agreement"></a>Firmare il Contratto Microsoft Partner

Un rivenditore indiretto, dopo aver configurato l'account del Centro per i partner, deve comunque iscriversi ufficialmente al programma Cloud Solution Provider. Per controllare lo stato dell'iscrizione, passare a [Profilo partner](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) e confermare il tipo di account. Iscriversi quindi a CSP come [rivenditore indiretto](enrolling-in-the-csp-program.md).

 Dopo aver effettuato l'iscrizione come rivenditore indiretto, accettare la [richiesta di relazione CSP con il provider indiretto](indirect-reseller-tasks-in-partner-center.md).

In seguito, accettare il Contratto Microsoft Partner nella panoramica del [dashboard](https://partner.microsoft.com/pvc/dashboard) Centro per i partner usando le credenziali di amministratore globale. Confermare di aver firmato il Contratto Microsoft Partner nella sezione Info sul programma del profilo partner. Verrà anche visualizzata una notifica banner di conferma nella pagina Panoramica di CSP. 

## <a name="next-steps"></a>Passaggi successivi

- [Trovare l'amministratore globale](become-global-admin.md)

- [Contratto Microsoft Partner](microsoft-partner-agreement.md)

- [Creare account utente](create-user-accounts-and-set-permissions.md)

- [Assegnare autorizzazioni e ruoli utente](permissions-overview.md)

- [Gestire i programmi dell'iscrizione come membro](renew-mpn-offers.md)

- [Creare il profilo di business](create-a-marketing-profile.md)

- [Connettersi con i clienti tramite segnalazioni](manage-leads.md)

- [Guida alla migrazione di più aziende da PMC al Centro per i partner](move-multiple-companies.md)
