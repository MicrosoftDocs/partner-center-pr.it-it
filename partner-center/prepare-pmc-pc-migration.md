---
title: Passaggio da Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Leggi le informazioni utili e le domande frequenti prima di far passare la tua azienda da Partner Membership Center al Centro per i partner.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f9085a4faaea4ac028633eb669212af5afbcb3d4
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749162"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Eseguire la preparazione per il passaggio da Partner Membership Center (PMC) al Centro per i partner

**Ruoli appropriati**
- Amministratore globale
- Amministratore utenti
- Agente di vendita
- Agente amministratore

La gestione degli account di appartenenza sta passando da Partner Membership Center (PMC) al Centro per i partner, l'unica destinazione in cui gestire la tua relazione aziendale con Microsoft. Il passaggio al Centro per i partner deve avvenire con la massima efficienza e facilità. Sono state pertanto identificate alcune aree in cui il Centro per i partner differisce da PMC, quindi è opportuno comprendere queste differenze e prepararsi prima di effettuare tale passaggio.

## <a name="account-and-identity-setup"></a>Impostazione di account e identità

**Che cos'è un account aziendale Azure Active Directory (Azure AD)?**

Un account aziendale Azure è una rappresentazione virtuale, dedicata e isolata, della tua azienda nel cloud pubblico di Azure che viene creata al momento della sottoscrizione di un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.

Il tuo account aziendale ospita gli utenti di Azure AD e le informazioni correlate: indirizzo di posta elettronica, password, dati del profilo, autorizzazioni e così via. L'account aziendale contiene anche gruppi, applicazioni e altre informazioni relative a una società e alla sua sicurezza. 

Il tuo indirizzo di posta elettronica aziendale fa parte del tenant Azure Active Directory. Per avere un account nel Centro per i partner, devi disporre di un tenant AAD. Per altre informazioni su Azure Active Directory, leggi [Creare la directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

Nel Centro per i partner userai il tuo indirizzo di posta elettronica aziendale, non quello personale, per accedere al tuo account.
- Account aziendale: john@contoso.com
- Account personale: John@outlook.com

**Con quale account devi accedere al Centro per i partner se disponi di un tenant AAD presso Microsoft (ad esempio, per Office 365) e anche di un tenant per l'attività CSP?**

Puoi accedere al Centro per i partner con l'account CSP o con il tuo account di posta elettronica aziendale MPN. Se scegli di accedere con il tuo indirizzo di posta elettronica aziendale CSP, nel riquadro di spostamento nella parte sinistra del dashboard vengono visualizzate le informazioni sia per il programma MPN che per il programma CSP. Se accedi con il tuo indirizzo di posta elettronica aziendale del tenant Azure AD di MPN, vengono visualizzate solo le informazioni relative al programma MPN. 

**Se non vuoi usare il tenant Azure AD di Office 365 esistente per il Centro per i partner, puoi creare un nuovo tenant prima di eseguire la migrazione da PMC.**

Possono essere numerose le ragioni per cui non vuoi usare un tenant Azure AD esistente per impostare il tuo account del Centro per i partner. Prima di avviare la migrazione al Centro per i partner, vai al [portale di Azure](https://ms.portal.azure.com/#home) per creare un nuovo tenant Azure AD. Segui le indicazioni contenute in [Creare un nuovo tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Usare il nuovo tenant AAD per configurare l'account del Centro per i partner. Per creare il tenant, devi essere un amministratore globale. 


**Ruoli utente, inclusi i ruoli utente guest nel Centro per i partner**

Il Centro per i partner prevede diversi tipi di ruoli a seconda dei tipi di lavoro da svolgere. Sono presenti ruoli, come l'amministratore globale, che sono di Azure AD. Alcuni ruoli sono specifici dei programmi, ad esempio il programma Cloud Service Provider o Incentivi, mentre altri ruoli sono specifici di MPN. Per informazioni su tutti i ruoli del Centro per i partner, vedi [Assegnare autorizzazioni e ruoli utente](permissions-overview.md).

**Che cosa accade ai ruoli dei miei utenti quando passano da PMC al Centro per i partner?**

Ad eccezione dell'amministratore globale MPN o del contatto principale del programma che esegue la migrazione, tutti gli utenti di PMC perderanno i ruoli di amministratore. L'utente che completa la migrazione dovrà assegnare i ruoli nel Centro per i partner. I ruoli nel Centro per i partner sono diversi da quelli in PMC. Per altre informazioni sui ruoli utente nel Centro per i partner, vedi [Assegnare autorizzazioni e ruoli utente] (permissions-overview.md) e [Passaggio da Partner Membership Center al Centro per i partner](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles).


**Qual è la differenza tra il mio profilo aziendale e il mio profilo di business?**

Il profilo aziendale è costituito dalle informazioni sulla tua società, che includono indirizzo, sedi, contatto principale e dettagli bancari e fiscali.

Il profilo di business ti consente di presentarti ai clienti ed è una pagina di marketing che visualizza il tuo logo, i dettagli relativi all'attività che svolgi, la tua esperienza e così via.

**Che cosa accade al mio account con il consolidamento?**

Se usi lo stesso tenant Azure AD per eseguire la migrazione di più account MPN al Centro per i partner, il sistema lo riconosce automaticamente e chiede di consolidare gli account. Questo vale anche se hai più domini associati allo stesso tenant Azure AD. 

Puoi comunque decidere di eseguire la migrazione al Centro per i partner usando tenant AAD distinti, ma tieni presente che questo porta a una valutazione isolata delle tue competenze e quindi a costi di acquisto aggiuntivi. Per altre informazioni sul consolidamento dell'account, vedi [Consolidare gli account aziendali](consolidate-accounts.md).

**Se ho più tenant AAD e un solo account MPN, è possibile collegarli nel Centro per i partner?**

Sì, nel Centro per i partner puoi collegare più tenant Azure AD a un singolo account del Centro per i partner.
Per altre informazioni sul consolidamento dell'account, vedi [Consolidare gli account aziendali](consolidate-accounts.md).

**Sono previste limitazioni per l'aggiunta di più tenant Azure AD a un singolo account del Centro per i partner?**

Se il tenant Azure AD è già associato a un account esistente del Centro per i partner, non può essere associato a nuovi account del Centro per i partner con la funzionalità multi-tenancy. In altri termini, un tenant Azure AD può essere associato a un solo account del Centro per i partner, ma a un account del Centro per i partner possono essere associati più tenant.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migrazione degli account di appartenenza MPN (Microsoft Partner Network) 

**Chi può effettuare il passaggio da PMC al Centro per i partner?**

Questo passaggio può essere avviato ed effettuato dall'amministratore globale MPN dell'azienda o dal contatto principale del programma (questi due ruoli sono spesso assegnati alla stessa persona).

**La persona che completa la migrazione diventa il contatto principale per il profilo legale dell'azienda nel Centro per i partner?**

Non necessariamente. Tuttavia, il contatto principale deve essere un utente autorizzato a firmare contratti.

**Microsoft può eseguire la migrazione del mio account di appartenenza MPN per mio conto?**

No. Microsoft non può aiutarti a trasferire il tuo account di appartenenza nel Centro per i partner. Per avviare il processo di migrazione, dovrai spostare l'account accedendo a PMC con il tuo account aziendale (credenziali di accesso). Dopo aver completato le operazioni necessarie per spostare l'account, puoi iniziare a gestire il tuo account di appartenenza e assegnare ruoli utente e autorizzazioni al tuo team in modo che i relativi membri possano accedere ai benefit previsti e contribuire alla gestione dell'appartenenza. 

Microsoft eseguirà automaticamente la migrazione delle competenze, dei benefit, delle informazioni sulle sedi, dei dettagli bancari e fiscali per gli incentivi e delle associazioni MCP correnti, incluso l'accesso a Partner University.

**In che modo cambieranno i criteri di rinnovo?**

 Nel Centro per i partner la finestra di rinnovo inizia dalla data di ricorrenza annuale e si estende sui successivi 30 giorni.

**Le competenze resteranno invariate dopo il passaggio al Centro per i partner?**

Sì, il passaggio al Centro per i partner non inciderà sulle competenze. Se noti discrepanze, contatta il [Supporto](https://partner.microsoft.com/support).


 **I benefit di cui dispongo (inclusi i benefit cloud, il supporto tecnico, i benefit software e Visual Studio) cambieranno dopo il passaggio al Centro per i partner?**

 I benefit per cui sei idoneo resteranno invariati. Se noti discrepanze, contatta il [Supporto](https://partner.microsoft.com/support).

 **Verranno mantenute le allocazioni di benefit Visual Studio per gli account Microsoft?**


 Sì. I benefit Visual Studio allocati agli account Microsoft verranno onorati e mantenuti. Verranno conservati anche dopo il rinnovo nel Centro per i partner. Tuttavia, se rimuovi l'allocazione a un account Microsoft una volta eseguita la migrazione al Centro per i partner, non sarà possibile aggiungerla nuovamente nel Centro per i partner.

Nel Centro per i partner un partner può aggiungere account aziendali e account utente guest, che sono account Microsoft dello stesso tenant in cui il partner è amministratore MPN nel tenant Azure AD. Se il partner è amministratore globale in più tenant di Azure AD e tutti questi tenant sono associati allo stesso account del Centro per i partner, il partner può aggiungere utenti di tutti questi tenant ai benefit Visual Studio e alle allocazioni in base all'uso di Azure.

Anche se l'amministratore MPN o l'amministratore globale può assegnare agli utenti guest sottoscrizioni in base all'uso di Visual Studio, gli utenti guest non possono accedere al Centro per i partner usando il proprio account Microsoft. Gli utenti guest, tuttavia, possono accedere ad Azure e a Visual Studio per convalidare e usare i benefit che gli sono stati assegnati.


 **In che modo è opportuno gestire le associazioni MCP e l'accesso a Partner University?**

 Non vengono apportate modifiche alle associazioni MCP spostate da PMC. Tuttavia, tutti i nuovi dipendenti aggiunti dopo il passaggio al Centro per i partner dovranno essere associati nel Centro per i partner. Tutte le autorizzazioni relative a Partner University per gli utenti esistenti verranno mantenute, ma tutti i nuovi dipendenti dovranno andare al [centro di formazione](https://partner.microsoft.com/training) per avere informazioni su come ottenere l'accesso a Partner University.

 **In che modo posso visualizzare le informazioni MCP dopo il passaggio al Centro per i partner?**

Seleziona **Competenze** nel riquadro di spostamento nella parte sinistra del dashboard. Nella pagina **Competenze** puoi scaricare il report sulle competenze. In tale report sono elencati gli utenti che hanno acquisito conoscenze rilevanti per le competenze e i programmi nel Centro per i partner. Se i tuoi utenti hanno acquisito conoscenze che però non sono rilevanti per le competenze per cui stai lavorando, non saranno elencati nel report.


 **Nel Centro per i partner vengono usate le segnalazioni dei clienti?**

 No, non sono necessarie segnalazioni dei clienti per soddisfare i requisiti di competenza nel Centro per i partner.

 **Le associazioni di Partner of Record vengono spostate nel Centro per i partner?**

 Sì, tutto resta invariato per Partner of Record. Per altre informazioni, vedi come [collegare il tuo ID partner ai tuoi clienti](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Ci sono ripercussioni sugli incentivi a seguito del passaggio al Centro per i partner?**

No, non ci sono ripercussioni sugli incentivi se hai spostato il tuo account senza consolidare le località/sedi. Se la tua azienda dispone di più account in PMC e, quando passi al Centro per i partner, decidi di eseguire il consolidamento in un account globale, gli incentivi non andranno persi, ma potrebbe verificarsi un ritardo nel loro versamento. Se non sposti tutti gli account PMC interessati da programmi per incentivi, potresti non ricevere più i proventi derivanti dagli incentivi legati a tali account.


**Quali sono i ruoli Incentivi nel Centro per i partner?** 

I ruoli Incentivi nel Centro per i partner dipendono dalla località/sede e includono amministratori Incentivi e utenti Incentivi. Per altre informazioni sulle operazioni che possono essere eseguite da tali ruoli, vedi [Assegnare autorizzazioni e ruoli utente](permissions-overview.md).

**Gli amministratori Incentivi possono essere assegnati a livello globale e a livello di località/sede?**

 Sì. Puoi assegnare un amministratore Incentivi come tale per tutte le località/sedi oppure ogni località/sede può avere un proprio amministratore Incentivi.

 **Gli incentivi possono essere corrisposti a livello globale o a livello di località/sede?**

 Gli incentivi vengono corrisposti solo a livello di località/sede.

**Per quanto riguarda le segnalazioni, quanti profili di business è possibile creare?**

La tua azienda può creare tutti i profili di business necessari per rappresentare a pieno gli interessi societari. In ogni profilo di business puoi elencare fino a cinque località/sedi, una per ogni paese. Ciascun profilo di business può ricevere segnalazioni per ognuna delle relative località/sedi.

**Come verranno assegnate le segnalazioni? Quali cambiamenti devo aspettarmi? Ad esempio, se ho una società globale in un mercato e sedi in altri mercati, secondo quali criteri verranno assegnate le segnalazioni?**

Le segnalazioni vengono assegnate in base ai parametri di ricerca definiti dal cliente. Indipendentemente dal fatto che tu disponga di una o più località/sede, se i clienti specificano una località/sede desiderata e presso quella località/sede hai un'azienda che soddisfa gli altri parametri, la segnalazione viene assegnata a tale località/sede.








