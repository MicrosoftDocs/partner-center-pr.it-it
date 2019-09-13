---
title: Guida alla migrazione da PMC al centro per i partner | Centro per i partner
ms.topic: article
ms.date: 04/25/2019
description: Cosa è importante sapere quando si esegue la migrazione della società da una console di gestione dei partner al centro
author: LauraBrenner
ms.author: labrenne
keywords: PMC, migrazione, passaggio al centro per i partner
ms.localizationpriority: medium
ms.openlocfilehash: f8e0b1fa4b31608ed4031832018c0a003abf0ae9
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708912"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guida alla migrazione da PMC al centro per i partner

Il sito Web del partner Microsoft in partner.microsoft.com è un'esperienza digitale unificata per i partner. Dal sito Web del partner, sarà possibile esplorare le opportunità e coinvolgere le esperienze guidate che consentono all'azienda di creare e vendere app e servizi con Microsoft. Usando il collegamento del dashboard disponibile nel sito Web del partner, i membri del Microsoft Partner Network possono accedere al centro per i partner, dove si gestisce la relazione con Microsoft, si registrano i programmi e si registrano le offerte. 

È in corso la rimozione delle autorizzazioni per partner Membership Center (PMC). La società è stata invitata a eseguire la transizione della gestione delle appartenenze Microsoft Partner Network al centro per i partner. Questa guida consente di preparare le attività da eseguire quando si passa da una console di gestione dei partner al centro per i partner.

>[!Note]
>Anche se la società ha più di un account o una località, il passaggio al centro per i partner inizia con lo spostamento di un account (il primo) nel centro per i partner.

## <a name="get-started"></a>Attività iniziali

Lo spostamento inizia in PMC. L'amministratore globale riceverà un invito per iniziare lo spostamento. 

**Preparare in PMC**
- Verificare i dettagli aziendali 
- Verificare il contatto del programma primario 
- Verificare i percorsi aziendali
- Aggiornare gli utenti approvati

**Quando si è pronti**

Selezionare **iniziare a usare** l'invito. Verrà eseguita la pagina di accesso al centro per i partner.

![Attività iniziali](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>Inizia a usare l'indirizzo di posta elettronica aziendale

Se la società non dispone di un indirizzo di posta elettronica di lavoro e di un tenant di AAD, è possibile configurarne uno durante il processo di accesso al centro per i partner. Quando si tenta di accedere con un account di posta elettronica che non è un indirizzo di posta elettronica di lavoro, ad esempio l'account personale, si verrà indirizzati a fornire informazioni sull'azienda in modo che sia possibile configurare un tenant AAD e un indirizzo di posta elettronica di lavoro.
Questi dettagli aziendali verranno usati per finalizzare l'account nel centro per i partner, quindi assicurarsi che siano accurati.

>[!Note]
>Se si è un partner in Cina ed è stato registrato nel programma Microsoft Partner Network e Cloud Solution Provider (CSP), si avrà un tenant separato per ogni account. L'account con il programma Cloud Solution Provider è gestito nel cloud nazionale e l'account Microsoft Partner Network è gestito nel cloud globale. Non è possibile collegare i due account.

![Informazioni sulla società](images/migration/newtellusabout.png)

Dopo aver verificato o aggiornato le informazioni, selezionare **accetta e continua**.
I termini e le condizioni in questa pagina sono **esattamente identici** a quelli del contratto che la società ha già effettuato l'accesso a PMC.  
Viene avviata la creazione del tenant di Azure AD e viene fornito l'account aziendale.

La selezione **di Accept e continue** esegue anche le operazioni seguenti:

• Esegue la migrazione dell'account insieme a tutte le relative posizioni al centro per i partner

• Esegue la migrazione di tutte le competenze o mappe acquistate in PMC

• Migra tutti i vantaggi (MAPs, Silver, Gold) disponibili in PMC

## <a name="invite-employees-to-join-you"></a>Invitare i dipendenti a partecipare

Quando viene creato il nuovo tenant di Azure AD, è possibile invitare i dipendenti a accedere al centro per i partner.

![Invitare i dipendenti](images/migration/invite.png)


Se è stato eseguito l'accesso con un tenant AAD esistente, i dipendenti si sono spostati. In questo caso, assegnare i ruoli dipendenti, che determinano le operazioni che è possibile eseguire nel centro per i partner. Nota: I ruoli nel centro per i partner sono diversi dai ruoli in PMC. Per altre informazioni, vedere [passaggio da una console di gestione dei partner a](move-pmc-pc-map.md)un altro.

## <a name="verify-your-domain-and-become-a-global-admin"></a>Verificare il dominio e diventare un amministratore globale  

Se il tenant di AAD è nuovo, a nessuno viene assegnato il ruolo di amministratore globale. Per diventare l'amministratore globale, è necessario verificare la proprietà del dominio. Per semplificare l'operazione, potrebbe essere necessario l'amministratore del dominio. Si noti che anche se è possibile usare le offerte già acquistate, non sarà possibile acquistare nuove offerte fino a quando non si completa il passaggio per ottenere un amministratore globale. 

![Assumere il controllo](images/migration/takecontrol.png)

Quando si seleziona inizia, viene visualizzata la schermata seguente:

![Verificare la proprietà del dominio](images/migration/verifytxt.png)

Il registrar sarà già compilato. Solo il proprietario del dominio può aggiornare il file DNS. Pertanto, copiando e aggiungendo il file di testo al record DNS, è possibile verificare di essere il proprietario. L'aggiornamento potrebbe richiedere alcuni minuti. Sarà necessario disconnettersi dal centro per i partner e quindi accedere di nuovo. Il ruolo sarà stato modificato in amministratore globale. 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Familiarizzare con il dashboard e il centro per i partner

Segui il tour del dashboard. Qui è possibile gestire l'appartenenza, aggiungere un profilo business per i riferimenti, iscriversi al programma Cloud Solution Provider e visualizzare le notifiche e le offerte rilevanti per l'azienda in qualsiasi momento selezionando **Dashboard**. Puoi anche gestire gli incentivi, acquistare nel Marketplace, iscriverti ai servizi go-to-Market e molto altro.  

![Segui la presentazione](images/migration/fre.png)

## <a name="next-steps"></a>Passaggi successivi

- [Creare gli account utente](create-user-accounts-and-set-permissions.md)
- [Assegnare ruoli utente e autorizzazioni](permissions-overview.md)
- [Gestione dei programmi di appartenenza](renew-mpn-offers.md)
- [Creare il profilo aziendale dell'azienda](create-a-marketing-profile.md)
- [Connettersi con i clienti tramite riferimenti](responding-to-referrals.md)

## <a name="see-also"></a>Vedere anche

- [Guida alla migrazione di più società da PMC al centro per i partner](move-multiple-companies.md)
