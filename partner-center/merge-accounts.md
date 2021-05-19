---
title: Unire l'account partner con un altro account partner
description: Informazioni su come unire l'account partner con un altro account partner in Partner Center, per le aziende che sono partner Microsoft attivi in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 8c47204d54cf05113eae73cede4afedf106ac121
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146511"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Unire l'account partner con un altro account partner

**Ruoli appropriati:** Amministratore account

Due o più aziende che sono partner Microsoft attivi e hanno account Partner Center scegliere di unire i propri account.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Cosa accade quando due partner sceglie di unire i propri account Partner Center partner

- L'organizzazione partner che avvia l'unione sarà l'account globale partner (PGA).

- La PGA dell'organizzazione invitata diventa una località dell'azienda che inizia.

- Tutte le posizioni dell'account di unione diventano posizioni sotto il PGA.

- Al termine della fusione dell'account, verranno visualizzati i dettagli dell'account, ad esempio località e utenti, all'interno del profilo PGA. Non è possibile invertire questo processo.

- Tutti gli ID MPN per le località vengono mantenuti durante questo consolidamento.

- I ruoli dell'utente vengono assegnati. Ad esempio, se un utente fosse stato l'amministratore degli incentivi per una località specifica, avrebbe comunque questo ruolo dopo la fusione e sarebbe in grado di visualizzare gli incentivi visualizzati prima della fusione.

- Azure AD tenant e gli account CSP non vengono uniti e non hanno alcun effetto.

- Le offerte pubblicate e i dati della pipeline di co-selling associati a entrambe le aziende vengono mantenuti

### <a name="view-of-merged-accounts"></a>Visualizzazione degli account uniti

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusione di account":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Cosa aspettarsi se si è stati invitati a unire l'account Partner Center con un altro account Partner Center

Se si decide di accettare l'invito a unire gli account: · Gli ID MPN e le località verranno uniti nella PGA dell'account partner che ha invitato l'utente.

- Gli utenti verranno portati nell'account unito con i relativi ruoli intatti.

- I vantaggi e le competenze esistenti verranno mantenuti per entrambe le società dopo la fusione fino al rinnovo. Al momento del rinnovo, gli account verranno considerati come una società e verranno applicate le regole di rinnovo standard.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Comprendere l'impatto sui programmi e sui vantaggi quando i partner decidono di unire gli account

- Tutte le competenze esistenti (Gold/Silver), gli acquisti (ad esempio Microsoft Action Pack) e i vantaggi associati vengono mantenuti durante il consolidamento. Se entrambe le aziende hanno la stessa competenza, ma una è gold e l'altra silver, la competenza con il livello di competenza più alto verrà assegnata e i partner avranno un set di vantaggi silver e un set di vantaggi gold per tale competenza fino al successivo rinnovo. 

- La data dell'anniversario più Action Pack Microsoft verrà mantenuta dopo la fusione. Ad esempio, se la data dell'anniversario per la società 1 è giugno 2020 per il rinnovo del Action Pack e la data dell'anniversario per il rinnovo del Action Pack per la società 2 è ottobre 2020, Microsoft userà la data di ottobre 2020 come nuova data di anniversario per la società unita.

- Durante la fusione dell'account e fino al successivo rinnovo, ogni account manterrà i Action Pack e/o i vantaggi di competenza. Al momento del rinnovo, vengono applicate Action Pack standard e di rinnovo delle competenze.

- Al momento del rinnovo, i vantaggi inclusi con il raggiungimento delle competenze e Action Pack vengono implementati per l'account globale partner dell'azienda partner:

  - Microsoft Action Pack: l'azienda partner sarà in grado di acquistare una Action Pack per ogni account globale partner.

  - Competenza: l'azienda partner riceverà un pacchetto di vantaggi principali, associati ai risultati più elevati, oltre ai vantaggi specifici delle competenze per cui il partner è idoneo per ogni account globale del partner.

- Tutti i vantaggi sono soggetti alla guida [all Microsoft Partner Network di utilizzo dei vantaggi.](https://aka.ms/partner-benefits-use-guide) Ad esempio, un token di O365 E3 attivato funziona per 12 mesi dopo l'attivazione. Dopo aver attivato un token per le licenze in un tenant, tali licenze potrebbero non essere spostate in un altro tenant.

- Le associazioni DI ID MCP per entrambe le società verranno mantenute e associate all'ID MPN PGA.

- I vantaggi tecnici e di go-to-market vengono offerti come vantaggio principale per le competenze. Dopo la unione, è consigliabile controllare le informazioni bancarie e fiscali per garantire l'accuratezza.

- Se la società è in programma Azure Expert MSP, i vantaggi vengono mantenuti fino al rinnovo.

- Se l'azienda ha ottenuto specializzazioni avanzate, vengono mantenute in entrambi gli account.

- Tutti i voucher Software Assurance vengono conservati in entrambi gli account. 

- Non esiste alcun effetto sull'associazione DPOR o PAL. Tutti i contributi ai ricavi associati inizieranno a confluire nel nuovo account globale del partner

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Invitare un'azienda a unire il proprio account Partner Center con l'account Partner Center aziendale

>[!Note]
>Per eseguire la fusione degli account, è necessario essere **l'amministratore account** della società.

1. Selezionare **Impostazioni** nel dashboard Partner Center dati. 

2. Selezionare **Account merge**.

3. Aggiungere l'ID MPN che si trova nel **profilo partner** dell'account che si vuole invitare a unire con l'utente. È necessario usare l'ID MPN globale del partner. Non è possibile usare un ID MPN della posizione.

4. Quando si seleziona **Unisci**, viene inviato un invito alla società partner. Quando accettano la richiesta, è possibile avviare l'unione dell'account all'interno Partner Center. Se la società rifiuta la richiesta di unione degli account, può spiegare perché ha rifiutato la richiesta. Un elenco di tutte le unioni di account è disponibile in **Cronologia unione**.
 
### <a name="example-of-two-companies-merging-accounts"></a>Esempio di due società che uniscono account

1. Contoso, Ltd. ha 

    a. un [ID MPN globale di 1111111 e](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) un ID MPN di posizione subordinata di [2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).
  
    b. un tenant Azure AD = @contoso.com
 
    c. una competenza gold che scade il 1° ottobre 2020
2. Fabrikam, Inc. ha
 
    a.  un ID MPN globale 3333333 e due ID MPN di posizione subordinata 4444444 e 5555555

    b.  un tenant Azure AD = @fabrikam.com

    c.  due competenze gold che scadono il 1° dicembre 2020
3.  Contoso acquista Fabrikam e viene qui [per](https://partner.microsoft.com/dashboard/account/merger) avviare una richiesta di unione.
4.  Fabrikam accede Partner Center e passa alla stessa pagina di Contoso nel passaggio #3, per approvare la richiesta di Contoso.
5.  Contoso esamina i dettagli dell'unione nella stessa pagina e fornisce una conferma per procedere con la fusione dell'account.
6.  Dopo la fusione, l'account aziendale verrà visualizzato come:

    a.  Una società denominata Contoso con ID MPN globale 1111111 e 4 ID MPN di posizione subordinata 222222, 3333333, 4444444 e 5555555
    
    b.  Avrà due tenant Azure AD ( @contoso.com + @fabrikam.com ) che hanno accesso allo stesso account Partner Center account
    
    c.  Avrà due pacchetti di vantaggi per le competenze, uno che scade il 1° ottobre 2020 e l'altro il 1° dicembre 2020. Il 1° dicembre 2020 sarà possibile rinnovare come singolo pacchetto di vantaggi per le competenze. Al momento del rinnovo, Contoso manterrà tutte e tre le competenze anche se può gestire un solo pacchetto di vantaggi.
    
7.  Gli amministratori di Contoso continueranno a gestire i Partner Center per gli @contoso.com utenti di . Gli amministratori di Fabrikam continueranno a gestire i Partner Center per @fabrikam.com gli utenti di . Gli amministratori di Contoso possono amministrare gli utenti di Fabrikam solo se vengono invitati come guest nel tenant di Fabrikam.
8.  Contoso potrebbe decidere di ignorare il tenant e riemettere ai dipendenti di Fabrikam nuove credenziali @fabrikam.com con nuovi ruoli e @contoso.com autorizzazioni.

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare autorizzazioni e ruoli utente](permissions-overview.md)

- [Verificare le informazioni del profilo partner](update-your-partner-profile.md)

- [Aggiungere Servizi condivisi per partner di Azure in modo che i partner possano acquistare sottoscrizioni di Azure per uso personale](shared-services.md)
