---
title: Preparare lo spostamento da partner Membership Center a partner Center | Centro per i partner
ms.topic: article
ms.date: 06/13/2019
description: Aspetti da considerare prima di spostare l'azienda da PMC al centro per i partner
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: bbce4677e88c82cb3f2826fb37823d2746d12e61
ms.sourcegitcommit: f54b679ce5058793a52795c6f93b0e98311805e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/17/2019
ms.locfileid: "71060497"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Prepararsi al passaggio da partner Membership Center (PMC) a partner Center

Si sta migrando la gestione delle appartenenze da partner Membership Center (PMC) al centro per i partner, ovvero la singola destinazione per gestire la relazione aziendale con Microsoft. Si vuole che il passaggio al centro per i partner sia il più efficiente e semplice possibile. Sono state identificate alcune aree in cui il centro per i partner è diverso da PMC e si ritiene che sia necessario comprenderle e prepararle prima di eseguire lo spostamento.

## <a name="account-and-identity-setup"></a>Configurazione dell'account e dell'identità

**Che cos'è un account di lavoro di Azure Active Directory (Azure AD)?**

Un account aziendale Azure è una rappresentazione virtuale dedicata e isolata della società nel cloud pubblico di Azure e viene creato quando sottoscrivi un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.

L'account aziendale ospita gli utenti Azure AD e le informazioni su di essi, ovvero posta elettronica, password, dati del profilo, autorizzazioni e così via. L'account di lavoro contiene anche gruppi, applicazioni e altre informazioni relative a una società e alla relativa sicurezza. Per ulteriori informazioni, vedere...

Nel centro per i partner si userà l'indirizzo di posta elettronica dell'ufficio per accedere al proprio account e non alla posta elettronica personale.
- Account aziendale: john@contoso.com
- Account personale: John@outlook.com

Il tuo indirizzo di posta elettronica di lavoro fa parte del tenant di Azure Active Directory. Per avere un account nel centro per i partner, è necessario disporre di un tenant AAD. Per altre informazioni su Azure Active Directory, vedere [creare la directory in Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Quando si passa al centro per i partner da PMC, quale account dovrebbe accedere al centro per i partner se si dispone di un tenant AAD con Microsoft (per Office 365, ad esempio) e si dispone anche di un tenant per la propria azienda CSP?**

È possibile accedere al centro per i partner con l'account CSP o con l'account di posta elettronica dell'ufficio MPN. Se si sceglie di eseguire l'accesso con l'indirizzo di posta elettronica dell'ufficio CSP, nel riquadro di spostamento a sinistra del dashboard vengono visualizzate le informazioni sul programma MPN e CSP. Se si accede con il messaggio di posta elettronica dell'ufficio MPN Azure AD tenant, si vedranno solo le informazioni sul programma MPN. I ruoli utente sono diversi tra MPN e CSP, pertanto se si usa lo stesso account per le aziende MPN e CSP, assicurarsi di assegnare i ruoli utente di conseguenza. Per informazioni sui ruoli utente, vedere [assegnare ruoli utente e autorizzazioni](permissions-overview.md).

**Se non si vuole usare il tenant di Office 365 Azure AD esistente per il centro per i partner, è possibile creare un nuovo tenant prima di eseguire la migrazione da PMC.**

Ci possono essere diversi motivi per cui non si vuole usare un tenant di Azure AD esistente per configurare l'account del centro per i partner. Prima di iniziare la migrazione al centro per i partner, passare alla [portale di Azure](https://ms.portal.azure.com/#home) per creare un nuovo tenant di Azure ad. Seguire le istruzioni riportate in [creare un nuovo tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Dopo aver creato il nuovo tenant, usare questo tenant di AAD per configurare l'account del centro per i partner quando ci si sposta da PMC al centro per i partner. Per creare il tenant, è necessario essere un amministratore globale. Usare questa nuova directory per eseguire la migrazione al centro per i partner.


**Qual è la differenza tra il ruolo di amministratore globale di AAD e il ruolo di amministratore globale di PMC MPN?**

Si tratta di due ruoli completamente diversi con autorizzazioni diverse. L'amministratore globale del tenant AAD nel centro per i partner amministra il tenant: aggiunge o rimuove utenti, fornisce e gestisce password, ruoli e autorizzazioni e ha accesso a tutti i programmi aziendali nel centro per i partner. 

Il ruolo di amministratore globale MPN in PMC può eseguire le operazioni seguenti:

- Visualizza e modifica tutti i dati associati all'azienda e a tutte le sedi della società

-  Aggiungere amministratori a livello globale o locale.  Inoltre, gli amministratori globali possono assegnare a qualsiasi persona qualsiasi persona in qualsiasi posizione che conceda l'accesso globale indipendentemente dalla posizione a cui sono associati.
-  Eseguire qualsiasi funzione dell'interfaccia utente per partner, tra cui: 

-  Aggiungi/Rimuovi utenti

 - Assegna/Rimuovi ruoli 

 - Aggiungere/rimuovere/aggiornare i percorsi 

 - Acquistare competenze/mappe 

-  Visualizza i vantaggi

Quando l'amministratore globale MPN passa al centro per i partner, il ruolo è l'amministratore del partner MPN che dispone di autorizzazioni e attività diverse rispetto all'amministratore globale del centro per i partner. Per altre informazioni sui ruoli e sulle autorizzazioni in Partner Center, vedere [assegnare utenti ruoli e autorizzazioni](permissions-overview.md).

**Ruoli utente, inclusi i ruoli utente Guest nel centro per i partner**

Il centro per i partner dispone di diversi tipi di ruoli in base ai tipi di lavoro necessari. Sono presenti ruoli come amministratore globale Azure AD ruoli. Alcuni ruoli sono specifici dei programmi, ad esempio il programma o gli incentivi del provider di servizi cloud, e sono presenti ruoli specifici di MPN. Per informazioni su tutti i ruoli del centro per i partner, vedere [assegnare utenti ruoli e autorizzazioni](permissions-overview.md).



**Cosa accade ai ruoli degli utenti quando si spostano da un PMC a un centro per i partner?**

Ad eccezione dell'amministratore globale MPN o del contatto del programma principale che esegue la migrazione, tutti gli utenti nella console di gestione dei pacchetti perderanno i ruoli di amministratore. L'utente che completa la migrazione dovrà assegnare i ruoli nel centro per i partner. I ruoli nel centro per i partner sono diversi da quelli in PMC. Leggere [assegnare i ruoli e le autorizzazioni degli utenti] (autorizzazioni-overview.md e [passaggio da PMC al centro](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) per i partner per altre informazioni sui ruoli utente nel centro per i partner.


**Qual è la differenza tra il profilo aziendale e il profilo business?**

Il profilo aziendale è costituito dalle informazioni sull'azienda che includono indirizzo, località, contatto principale, banca e informazioni fiscali.

Il tuo profilo aziendale è il modo in cui si presenta ai clienti ed è una pagina di marketing in cui viene visualizzato il logo, i dettagli relativi alla tua attività, alla tua esperienza e così via.

**Che cosa significa il consolidamento dell'account per l'account?**

Se si usa lo stesso tenant di Azure AD per eseguire la migrazione di più account MPN nel centro per i partner, il sistema lo riconosce automaticamente e chiede di consolidare gli account. Questo vale anche se sono presenti più domini associati allo stesso tenant Azure AD. 

È comunque possibile decidere di eseguire la migrazione al centro per i partner usando tenant AAD distinti, ma si noti che questo comporta una valutazione isolata delle competenze e dei costi di acquisto aggiuntivi. 

**Se si hanno più tenant di AAD e un singolo account MPN, è possibile collegarli al centro per I partner?**

Sì, nel centro per i partner è possibile collegare più tenant di Azure AD a un singolo account del centro per i partner.
Altre informazioni sono disponibili qui. 

**Sono previste restrizioni per l'aggiunta di più tenant Azure AD a un singolo account del centro per i partner?**

Se il tenant Azure AD è già associato a un account del centro per i partner esistente, non può essere associato ai nuovi account del centro per i partner usando la funzionalità di multi-tenant. Un altro modo per considerarlo è che un tenant Azure AD può essere associato a un solo account del centro per i partner, ma a un account del centro per i partner possono essere associati più tenant.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migrazione dell'appartenenza Microsoft Partner Network (MPN) 

**Chi può eseguire lo spostamento da PMC al centro per i partner?**

L'amministratore globale MPN aziendale o il contatto del programma principale (questi due ruoli sono spesso conservati dalla stessa persona) può avviare ed eseguire lo spostamento.

**La persona che completa la migrazione diventa il contatto principale del profilo legale dell'azienda nel centro per i partner?**

Non necessariamente, tuttavia, il contatto principale deve essere un utente autorizzato a firmare i contratti.

**Microsoft può migrare l'appartenenza a MPN?**

No. Microsoft non può essere utile per spostare l'account di appartenenza al centro per i partner. Per avviare il processo di migrazione, è necessario spostare l'account accedendo a PMC con l'account aziendale (credenziali di accesso). Dopo aver completato i passaggi per spostare l'account, è possibile iniziare a gestire l'appartenenza e assegnare i ruoli utente e le autorizzazioni al team in modo che possano accedere ai vantaggi e gestire l'appartenenza. Microsoft migra automaticamente le competenze, i vantaggi, le informazioni sulla posizione, le informazioni bancarie e fiscali attuali per gli incentivi e le associazioni MCP, incluso l'accesso all'Università partner.

Microsoft migra automaticamente le competenze, i vantaggi, le informazioni sulla posizione, le informazioni bancarie e fiscali attuali per gli incentivi e le associazioni MCP, incluso l'accesso all'Università partner.

**In che modo vengono modificati i criteri di rinnovo?**

 Nel centro per i partner, la finestra di rinnovo è dalla data di ricorrenza dei 30 giorni successivi.

**Le nostre competenze rimarranno invariate dopo il passaggio al centro per i partner?**

Sì, Compentencies non sarà interessato dal passaggio al centro per i partner. Se si notano discrepanze, contattare il [supporto tecnico](https://partner.microsoft.com/support).


 **I vantaggi (inclusi i vantaggi del cloud, il supporto tecnico, i vantaggi software, Visual Studio) cambiano dopo lo spostamento?**

 I vantaggi idonei non vengono modificati. Se si notano discrepanze, contattare il [supporto tecnico](https://partner.microsoft.com/support).

 **Verranno rispettati gli account Microsoft con allocazione dei vantaggi di Visual Studio?**


 Sì. I benefit Visual Studio allocati agli account Microsoft verranno onorati e mantenuti. Verranno conservati anche dopo il rinnovo nel Centro per i partner. Tuttavia, se si rimuove l'allocazione a un account Microsoft una volta eseguita la migrazione nel Centro per i partner, non sarà possibile aggiungerla nuovamente nel Centro per i partner.

Nel Centro per i partner, un partner può aggiungere account aziendali e account utente Guest, che sono account Microsoft dello stesso tenant in cui il partner è amministratore MPN nel tenant di Azure AD. Se il partner è amministratore globale in più tenant di Azure AD e tutti questi tenant sono associati allo stesso account del Centro per i partner, il partner può aggiungere utenti di tutti questi tenant ai benefit Visual Studio e alle allocazioni in base all'uso di Azure.

Anche se l'amministratore MPN o l'amministratore globale può assegnare agli utenti guest sottoscrizioni in base all'uso di Visual Studio, gli utenti guest non possono accedere al Centro per i partner usando il proprio account Microsoft. Gli utenti guest, tuttavia, possono accedere ad Azure e a Visual Studio per convalidare e usare i benefit che gli sono stati assegnati.


 **Come si gestiscono le associazioni MCP e l'accesso all'Università partner?**

 Non sono state apportate modifiche alle associazioni MCP che passano da PMC. Tuttavia, tutti i nuovi nuovi dipendenti dopo lo spostamento al centro per i partner dovranno essere associati al centro per i partner. Tutte le autorizzazioni dell'Università partner per gli utenti esistenti rimarranno, ma tutti i nuovi dipendenti dovranno visitare [il centro formazione](https://partner.microsoft.com/training) per ottenere informazioni su come ottenere l'accesso all'Università partner.

 **Ricerca per categorie visualizzare le informazioni MCP una volta spostata al centro per I partner?**

Selezionare le **competenze** dal NAV di sinistra nel dashboard. Dalla pagina delle **competenze** è possibile scaricare il report Skills. Il report sulle competenze consente di elencare gli utenti che hanno acquisito competenze rilevanti per le competenze e i programmi nel centro per i partner. Se gli utenti hanno acquisito competenze ma tali competenze non sono rilevanti per le competenze a cui si sta lavorando, non verranno elencate nel report.


 **I riferimenti ai clienti vengono usati nel centro per i partner?**

 No, non sono necessari riferimenti ai clienti per soddisfare i requisiti di competenza nel centro per i partner.

 **Il partner delle associazioni di record passerà al centro per i partner?**

 Sì, non vi sono modifiche al partner del record. Scopri di più sul [collegamento dell'ID partner ai tuoi clienti](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**Si è verificato un effetto sugli incentivi a causa del passaggio al centro per i partner?**

No, non vi è alcun effetto sugli incentivi se il tuo account è stato spostato senza consolidare le località. Se l'azienda dispone di più account in PMC e, quando ci si sposta al centro per i partner, si decide di consolidare in un account globale, non ci saranno perdite per gli incentivi, ma potrebbe verificarsi un ritardo nel versamento di incentivi. Se non si spostano tutti gli account di PMC che sono stati interessati ai programmi per gli incentivi, è possibile che si arrestino gli incentivi legati a tali account.


**Quali sono i ruoli utente Incentive nel centro per i partner?** 

I ruoli Incentive nel centro per i partner sono basati sulla posizione e includono incentivi amministrativi e utenti incentivi. Per ulteriori informazioni sulle operazioni che questi ruoli possono eseguire, vedere [assegnare utenti ruoli e autorizzazioni](permissions-overview.md).

**Gli utenti possono incentivare l'assegnazione a livello globale e di località?**

 Sì. È possibile assegnare un amministratore di incentivi come amministratore di incentivi per tutte le località o ogni località può avere un proprio amministratore di incentivi.

 **È possibile pagare incentivi a livello globale o di posizione?**

 Gli incentivi vengono pagati solo a livello di località.

**Per quanto riguarda i riferimenti, quanti profili business è possibile creare?**

La tua azienda può creare tutti i profili aziendali necessari per rappresentare completamente gli interessi della tua azienda. In ogni profilo business è possibile elencare fino a cinque località, una località per paese. Ognuno dei profili di business può ricevere riferimenti per ogni posizione.

**Come verranno assegnati I riferimenti, quali modifiche è possibile prevedere? Se, ad esempio, si dispone di una società globale in un mercato e di posizioni in altri mercati, come verranno assegnati I riferimenti?**

I riferimenti vengono assegnati in base ai parametri di ricerca definiti dal cliente. Quindi, indipendentemente dal fatto che si disponga o meno di una località, se i clienti specificano una località desiderata ed è presente un'azienda che soddisfa gli altri parametri, il riferimento passa a tale posizione.








