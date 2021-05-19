---
title: Collegare l'ID MCP di Microsoft Learn all'account del Centro per i partner
ms.topic: how-to
ms.date: 01/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come associare l'ID MCP all'account del Centro per i partner, in modo che l'azienda possa visualizzare i percorsi di training e apprendimento svolti per l'acquisizione delle competenze.
author: kbangalore
ms.author: kiranban
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b5487addd5bf4cd53eacaa95c4e2e602a7279bad
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151237"
---
# <a name="link-or-unlink-a-microsoft-certification-profile-id-mcid-to-a-microsoft-partner-network-mpn-account"></a>Collegare o scollegare un ID profilo di certificazione Microsoft (MCID) a un account Microsoft Partner Network (MPN)

**Ruoli appropriati:** tutti Partner Center utenti

Questo articolo descrive come i clienti che detendono certificazioni attive nel Programma di certificazione Microsoft possono collegare o scollegare l'ID del profilo di certificazione Microsoft (MCID) con un'organizzazione mpn (Microsoft Partner Network).

È necessario essere un amministratore partner MPN o un amministratore globale per esaminare lo stato delle competenze [(necessario](https://partner.microsoft.com/pcv/partnership/competencies) per l'accesso) per gli esami o per scaricare i report sulle competenze per la revisione degli esami associati. L'organizzazione partner soddisfa i requisiti di competenza grazie alla presenza di singoli utenti con ID MCID collegati associati all'organizzazione. Un MCID può essere collegato solo a una singola appartenenza MPN alla volta.

## <a name="get-partner-university-access"></a>Ottenere l'accesso a Partner University

Per associare la certificazione Microsoft, è necessario avere un account Partner Center (Active AD) associato all'organizzazione partner. I membri delle organizzazioni partner MPN devono usare il nome utente e la password aziendale dell'organizzazione partner MPN (account aziendale) per accedere Partner Center.
Usare la procedura seguente per ottenere l'accesso a Partner University.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Selezionare **l'icona blu Profilo** personale nell'angolo superiore destro
3. Nel campo **Your Learning (Apprendimento)** selezionare **Get Partner University Access (Ottieni l'accesso a Partner University).** È necessario immettere le credenziali dell'account Partner University (non l'account del Centro per i partner) L'account dell'università partner verrà ora associato all'account utente Partner Center partner. Le valutazioni verranno riflesse nel report Partner Center competenze utente entro 72 ore. Le valutazioni appena superate possono richiedere da 7 a 10 giorni per riflettere il report.
4. Per rimuovere l'associazione, selezionare **Rimuovi accesso**.

## <a name="associate-a-microsoft-learning-account"></a>Associare un account Microsoft Learning locale

Usare la procedura seguente per associare un Microsoft Learning account. 

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nella pagina del profilo scorrere verso il basso fino al **campo Certificazioni** e esami Microsoft e selezionare Associa Microsoft Learning **account**.
3. Quando richiesto, immettere le credenziali usate per accedere al profilo di certificazione Microsoft (MCID).

>[!NOTE]
>Se le Microsoft Learning dell'account sono le stesse delle credenziali dell'account Partner University, selezionare Usa per associare l'account Microsoft Learning **email@address personale.**

## <a name="download-skills-report-microsoft-certification-list"></a>Scaricare il report sulle competenze (elenco di certificazione Microsoft)
Se sono necessari dettagli, il report delle competenze può essere accessibile e scaricato da qualsiasi amministratore globale o amministratore partner MPN da Partner Center. Per [altre informazioni, vedere](./mpn-skills-report.md#view-skills-report-data).


## <a name="frequently-asked-questions-about-linking-accounts"></a>Domande frequenti sul collegamento di account

### <a name="how-can-a-user-link-their-microsoft-certification-profile-id-mcid-with-the-microsoft-partner-network-mpn-organization-they-work-for"></a>In che modo un utente può collegare il proprio ID profilo di certificazione Microsoft (MCID) all'organizzazione Microsoft Partner Network (MPN) per cui lavora?

Gli utenti devono accedere a Partner Center e passare a **Mio profilo** e quindi selezionare Get Partner University account (Ottieni **account Partner University)** o Associate Microsoft Learning account (Associa **Microsoft Learning account)** e immettere le proprie credenziali. Per associarlo a un account Microsoft Learning l'utente dovrà immettere il nome utente e la password usati per accedere al proprio profilo di certificazione Microsoft (MCID). A causa di considerazioni sulla privacy, gli utenti devono completare il processo di collegamento dell'account.  

### <a name="how-can-a-user-unlink-their-mcid-from-the-mpn-organization-they-work-for"></a>Come può un utente scollegare il proprio MCID dall'organizzazione MPN per cui lavora?

Accedere a Partner Center, passare a **Profilo personale** e quindi selezionare Rimuovi **accesso.** A causa di considerazioni sulla privacy, l'utente deve completare il processo di collegamento dell'account.

### <a name="the-user-left-company-a-and-now-works-for-company-b-how-can-they-link-their-microsoft-certification-profile-id-mcid-with-company-b"></a>L'utente ha lasciato la società A e ora lavora per la società B. Come possono collegare l'ID profilo di certificazione Microsoft (MCID) alla società B?

L'utente deve collegare il proprio MCID alla società B seguendo la procedura precedente. Quando l'utente collega il proprio MCID alla società B, verrà scollegato automaticamente dalla società A.

### <a name="the-user-left-company-a-and-no-longer-has-access-to-partner-center-they-want-to-unlink-their-mcid-from-company-a-and-are-not-planning-to-link-it-with-another-mpn-organization-at-the-moment"></a>L'utente ha lasciato la società A e non ha più accesso Partner Center. Vogliono scollegare il proprio MCID dalla società A e non hanno intenzione di collegarlo a un'altra organizzazione MPN al momento.

L'account dell'utente deve essere eliminato dall'amministratore globale dopo aver lasciato l'azienda. Se il MCID dell'utente viene ancora visualizzato come collegato alla società nel report delle competenze, l'utente deve richiedere all'amministratore globale di rimuoverli dal report.

### <a name="the-admin-provided-sign-in-details-for-a-work-email-account-to-a-user-and-they-have-had-no-response"></a>L'amministratore ha fornito i dettagli di accesso per un account di posta elettronica aziendale a un utente e non ha avuto risposta.

L'amministratore deve prima verificare l'indirizzo di posta elettronica usato e quindi contattare l'utente a cui sono stati forniti i dati dell'account.

### <a name="a-user-tries-to-associate-their-mcp-learning-account-to-their-profile-in-partner-center-and-receives-a-message-that-their-association-is-limited-for-example-you-have-attempted-to-associate-with-a-partner-organization-however-we-require-a-period-of-30-days-between-associations-your-next-available-date-for-a-subsequent-association-is-xxx"></a>Un utente tenta di associare l'account MCP Learning al proprio profilo Partner Center e riceve un messaggio che indica che l'associazione è limitata. Ad esempio, "Si è tentato di associare un'organizzazione partner. Tuttavia, è necessario un periodo di 30 giorni tra le associazioni. La data disponibile successiva per un'associazione successiva è XXX"

Per proteggersi da abusi, un utente MCP ha un numero limitato di 3 associazioni consentite ogni anno e tra ogni associazione è consentito un periodo di raffreddamento di 30 giorni, che inizia all'inizio dell'associazione. Ogni utente può controllare la data nel profilo per verificare quando può avviare una nuova associazione. Se l'utente ha problemi di associazione dopo tale data, deve contattare il supporto tecnico.  

## <a name="how-to-get-support"></a>Come ottenere supporto

Per problemi tecnici relativi al collegamento o alla scollegamento di MCID con organizzazioni partner MPN non trattate nelle domande frequenti, aprire un ticket con il [supporto](https://partner.microsoft.com/support)tecnico Microsoft .

Per domande relative al processo di unione del profilo di certificazione Microsoft ,contattare [il supporto tecnico microsoft.](https://aka.ms/mcpforum)

## <a name="next-steps"></a>Passaggi successivi

- [Usare ruoli e autorizzazioni](./permissions-overview.md)
- [Competenze](https://partner.microsoft.com/membership/competencies)
- [Report di analisi di Microsoft Learn che mostra lo stato degli studenti nella società](ms-learn-analytics.md)
