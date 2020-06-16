---
title: Iscriversi al programma Cloud Solution Provider
ms.topic: article
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui requisiti del programma CSP per i partner che vogliono iscriversi al programma Cloud Solution Provider per Microsoft Cloud per il governo degli Stati Uniti.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 060fd94567c84e7c1652fb538cc1786d8b807787
ms.sourcegitcommit: c89ddcf8b366f56dc123936cbda2d0001c9f0d8e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/15/2020
ms.locfileid: "84788785"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Iscriversi al programma Cloud Solution Provider per Microsoft Cloud per il governo degli Stati Uniti

**Si applica a**

- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale

I partner Microsoft possono ora vendere le soluzioni e i servizi cloud Microsoft a entità federali, statali, locali e tribali degli Stati Uniti tramite il programma Cloud Solution Provider (CSP) per Microsoft Cloud per il governo degli Stati Uniti. 

Microsoft Cloud per il governo degli Stati Uniti fornisce un'istanza privata, dedicata e isolata di Microsoft Azure che soddisfa i requisiti del governo degli Stati Uniti per la sicurezza dei dati, la privacy e la conformità. La società deve soddisfare i requisiti di idoneità di Microsoft per partecipare al programma CSP per Microsoft Cloud per il governo degli Stati Uniti. Per altre informazioni, vedere [centro per i partner per Microsoft Cloud per il governo degli Stati Uniti](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Prima di iniziare

Prima di poter iscriversi al programma CSP per Microsoft Cloud per il governo degli Stati Uniti, è necessario verificare che l'azienda soddisfi i requisiti per la vendita agli enti pubblici degli Stati Uniti. Prima di avviare il processo di iscrizione, completare il modulo di [convalida del cloud di Microsoft Government](https://azuregov.microsoft.com/csp) per poter verificare l'idoneità dell'azienda. Una volta verificata l'idoneità dell'azienda, verrà fornito un tenant di Azure Active Directory (Azure AD) specifico per l'Microsoft Cloud per il governo degli Stati Uniti.  

Per creare un account del centro per i partner e registrarsi in CSP per Microsoft Cloud per il governo degli Stati Uniti, è necessario fornire le informazioni seguenti (è possibile raccogliere queste informazioni prima di avviare il processo di registrazione):

-  Credenziali di amministratore globale per il nuovo tenant di Azure AD dell'organizzazione per Microsoft Cloud per il governo degli Stati Uniti
-  ID dell'organizzazione Microsoft Partner Network (MPN) 
-  Un indirizzo aziendale nella Stati Uniti

> [!IMPORTANT]  
> Se si dispone di un account esistente nel centro per i partner e si desidera registrarsi in CSP per Microsoft Cloud per il governo degli Stati Uniti, è necessario creare un nuovo account separato specificamente per il mercato degli Stati Uniti.

## <a name="how-to-enroll"></a>Come effettuare la registrazione 

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Passaggio 1: creare un account del centro per i partner per Microsoft Cloud per il governo degli Stati Uniti

1.  Avviare il processo di registrazione [qui](https://partnercenter.microsoft.com/register/resellerusgjoinnow). 

2.  Accedere con le credenziali di amministratore globale per il tenant di Azure AD dell'organizzazione per Microsoft Cloud per il governo degli Stati Uniti. Se l'organizzazione non ha un account per questo portale, è possibile richiederne una completando il [modulo di convalida del cloud di Microsoft Government](https://azuregov.microsoft.com/csp).


### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Passaggio 2: richiedere la partecipazione al programma Cloud Solution Provider per Microsoft Cloud per il governo degli Stati Uniti

1.  Inserire le informazioni mancanti nel modulo di registrazione, inclusi l'ID Microsoft Partner Network e i dettagli del supporto tecnico dell'organizzazione. 

2.  Seleziona **Accetta e continua**. Potrebbero essere necessari diversi giorni per rivedere la tua richiesta. Ti invieremo un'e-mail al termine della revisione.

    > [!IMPORTANT]  
    > Selezionando **accetta e continua**, stai confermando che sei autorizzato a agire per conto dell'organizzazione e accetti di consentire a Microsoft di eseguire una verifica del credito in background prima di esaminare l'applicazione Cloud Solution Provider dell'organizzazione.


### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Passaggio 3: firmare il contratto rivenditore per Microsoft Cloud per il governo degli Stati Uniti

1. Accedere al centro per i partner per Microsoft Cloud per il governo degli Stati Uniti usando il collegamento fornito nel messaggio di posta elettronica di approvazione dell'applicazione. 

2. Nella pagina del **contratto** leggere le condizioni e, se si accettano le condizioni, selezionare **Accetto e continuare** con la firma digitale del [contratto rivenditore per Microsoft Cloud per il governo degli Stati Uniti](https://go.microsoft.com/fwlink/p/?linkid=843364). La creazione dell'account potrebbe richiedere diverse ore. Disconnettersi dal centro per i partner per Microsoft Cloud per il governo degli Stati Uniti e quindi eseguire nuovamente l'accesso in un secondo momento.


### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Passaggio 4: assegnare gli utenti al ruolo di agente di amministrazione nel portale di amministrazione di Microsoft Azure per Microsoft Cloud per il governo degli Stati Uniti

Microsoft Cloud per il governo degli Stati Uniti fornisce un'istanza separata di Microsoft Azure che soddisfa gli standard per la conformità, la sicurezza e la privacy degli enti pubblici. Per consentire agli amministratori di gestire gli utenti e le licenze nella portale di Microsoft Azure, è necessario assegnare manualmente il ruolo di agente di amministrazione a tali utenti.

> [!NOTE]  
> Dopo aver assegnato gli utenti al ruolo di amministratore dell'agente, potranno accedere all'elenco dei clienti nella pagina **Customers** e [aggiungere nuovi clienti](add-a-new-customer.md).   

1.  Accedere al portale di amministrazione di Microsoft Azure all'indirizzo https://portal.azure.us/ .

2.  Assegnare il ruolo di agente di amministrazione agli utenti appropriati nell'organizzazione. A tale scopo, è necessario aggiungere questi utenti al gruppo **AdminAgent** incorporato. Per informazioni su come eseguire questa operazione, vedere [gestire i membri di un gruppo in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-groups-members-azure-portal) .
 
## <a name="connect-with-us"></a>Contatti

- Domande? Invia un messaggio di posta elettronica all'indirizzoazgovcsp@microsoft.com

- Partecipa a [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777&view=all) 

## <a name="related-topics"></a>Argomenti correlati

-  [Centro per i partner per Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

-  [Gestione di utenti e licenze nel Centro per i partner per Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)


