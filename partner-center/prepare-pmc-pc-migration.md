---
title: Preparare la migrazione da Partner Membership Center al centro per i Partner | Centro per i partner
ms.topic: article
ms.date: 06/13/2019
description: Aspetti da considerare prima di passare l'azienda dalla console di gestione pacchetti al centro per i Partner
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 16c29bdccd4c4853fcc28ed4f2752270415449b1
ms.sourcegitcommit: 8305d8d1da404d75ce3120085724fe67da733eec
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/14/2019
ms.locfileid: "67145351"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Preparazione per lo spostamento da Partner Membership Center (PMC) al centro per i Partner

Passare gestione delle appartenenze da Partner Membership Center (PMC) al centro per i partner, l'unica destinazione per gestire la relazione di business con Microsoft. Vogliamo che la migrazione a Centro per i Partner a essere quanto efficiente e più semplice possibile. Abbiamo stabilito alcune aree in cui il centro per i Partner è diversa dalla console di gestione pacchetti e riteniamo che si desidera comprendere e prepararsi di conseguenza, prima di effettuare lo spostamento.

## <a name="account-and-identity-setup"></a>Programma di installazione di identità e account

**Che cos'è un account di lavoro di Azure Active Directory (Azure AD)?**

Un account aziendale Azure è una rappresentazione virtuale dedicata e isolata della società nel cloud pubblico di Azure e viene creato quando sottoscrivi un servizio cloud Microsoft, ad esempio Azure, Microsoft Intune o Office 365.

L'account di lavoro ospita gli utenti di Azure AD e le informazioni su di essi, i messaggio di posta elettronica, password, i dati del profilo, le autorizzazioni e così via. L'account di lavoro contiene anche i gruppi, applicazioni e altre informazioni relative all'azienda e alla sicurezza. Per altre informazioni, vedere...

Nel centro per i Partner si utilizzerà la posta elettronica aziendale per accedere al proprio account non di posta elettronica personale.
- L'account aziendale: john@contoso.com
- L'account personale: John@outlook.com

La posta elettronica aziendale fa parte del tenant di Azure active directory. Per ottenere un account in Partner Center, è necessario disporre di un tenant AAD. Per altre informazioni su Azure Active Directory, leggere [creare la directory in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Quando si sposta in Partner Center dalla console di gestione pacchetti, quali account devono si accede a Centro per i Partner con se si hanno un tenant di AAD con Microsoft (per Office 365, ad esempio) ed è inoltre dispone di un tenant per la tua azienda CSP?**

È possibile accedere a Centro per i Partner con l'account CSP o l'account di posta elettronica aziendale MPN. Se si sceglie di accedere usando la posta elettronica aziendale CSP, di spostamento a sinistra nel dashboard visualizzerà le informazioni sul programma MPN sia CSP. Se si accede con la posta elettronica aziendale tenant AD Azure MPN, vedrete solo informazioni relative al programma MPN. I ruoli utente sono diversi tra MPN e CSP pertanto se si usa lo stesso account per le aziende sia MPN e CSP, assicurarsi assegnare i ruoli utente di conseguenza. Per informazioni sui ruoli utente, leggere [assegnare le autorizzazioni e ruoli utente](permissions-overview.md).

**Che cos'è la differenza tra il ruolo di amministratore globale AAD e il ruolo di amministratore globale PMC MPN?**

Questi sono due completamente diversi ruoli con autorizzazioni diverse. L'amministratore globale tenant AAD nel centro per i Partner consente di amministrare il tenant: aggiunge o rimuove gli utenti, fornisce e gestisce le password, ruoli e autorizzazioni e ha accesso ai programmi tutte della propria azienda nel centro per i Partner. 

Il ruolo di amministratore globale di MPN nella console di gestione pacchetti è stato possibile eseguire le operazioni seguenti:

- Visualizzare e modificare tutti i dati associati con la società e tutte le posizioni dell'azienda

-  Aggiungere gli amministratori a livello globale o locale.  Inoltre, gli amministratori globali possono assegnare qualsiasi persona in qualsiasi posizione di accesso di amministratore globale che consente l'accesso globale indipendentemente dalla posizione da cui sono associate.
-  Seguire un partner qualsiasi con connessione incluse funzioni dell'interfaccia utente: 

-  Aggiungere/rimuovere utenti

 - Assegnare o rimuovere ruoli 

 - Aggiungere/rimuovere/aggiornare percorsi 

 - Acquisto di competenza e mappe 

-  Vantaggi di visualizzazione

Quando l'amministratore globale di MPN si sposta al centro per i Partner il ruolo viene chiamato l'amministratore di partner MPN con autorizzazioni diverse e attività che l'amministratore globale di Partner Center. Per altre informazioni sui ruoli e autorizzazioni nel centro per i Partner, Leggi [assegnare ruoli agli utenti e autorizzazioni](permissions-overview.md)

**Ruoli utente in Partner Center**

Centro per i partner dispone di diversi tipi di ruoli a seconda dei tipi di lavoro da eseguire. Sono disponibili ruoli, ad esempio amministratore globale che sono ruoli di Azure AD. Alcuni dei ruoli sono specifici per i programmi, ad esempio il programma di Provider di servizi Cloud o incentivi e sono disponibili ruoli specifici di MPN. Per scoprire quali sono tutti i ruoli del centro per i Partner, leggere [assegnare ruoli agli utenti e autorizzazioni](permissions-overview.md).

**Cosa accade ai ruoli degli utenti quando si spostano dalla console di gestione pacchetti in Partner Center?**

Fatta eccezione per il contatto di programma principale che esegue la migrazione o amministratore globale di MPN, tutti gli utenti nella console di gestione pacchetti perderanno ai ruoli di amministratore. Persona che ha completato la migrazione sarà necessario assegnare i ruoli nel centro per i Partner. I ruoli nel centro per i Partner diversi da quelli nella console di gestione pacchetti. Lettura [assegnare ruoli agli utenti e autorizzazioni](permissions-overview) e [spostarsi dalla console di gestione pacchetti in Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) per più ruoli utente in Partner Center.


**Che cos'è la differenza tra il mio profilo aziendale e il mio profilo aziendale?**

Il profilo aziendale è le informazioni sulla società che includa indirizzo, posizioni, contatto principale, i dettagli fiscali e bancarie.

Il profilo di business è come se stessi presentare ai clienti e una pagina di marketing che riporti il logo, informazioni dettagliate sull'attenzione di business, l'esperienza e così via.

**Ciò che tiene conto del valore medio di consolidamento per il mio account?**

Se si usa lo stesso tenant di Azure AD per eseguire la migrazione di più account MPN nel centro per i Partner, il sistema verrà automaticamente riconoscere la modifica e chiedere di consolidare gli account. Questo vale anche se si hanno più domini associati allo stesso tenant di Azure AD. 

Si potrebbe comunque decidere di eseguire la migrazione al centro per i Partner usando separare i tenant di AAD, ma tenere presente che i costi di acquisto il risultato è isolata di valutazione delle competenze e aggiuntive. 

**Se si hanno più tenant AAD e un singolo account MPN, è possibile collegarli nel centro per i Partner?**

Sì, nel centro per i Partner è possibile collegare più tenant di Azure AD per singolo account Partner Center.
Altre informazioni sono disponibili qui. 


## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migrazione di appartenenza Microsoft Partner Network (MPN) 

**Chi può eseguire lo spostamento dalla console di gestione pacchetti al centro per i Partner?**

L'amministratore globale di MPN aziendale o il contatto di programma principale (questi due ruoli sono spesso utilizzati dalla stessa persona) puoi avviare ed eseguire lo spostamento.

**La persona che completa la migrazione diventerà il contatto principale sul profilo legali società nel centro per i Partner?**

Non necessariamente, tuttavia, il contatto principale deve essere un utente che ha l'autorizzazione per la firma di accordi.

**Microsoft migrare mio abbonamento a MPN per me?**

No. Microsoft non consente di spostare l'account di appartenenza al centro per i partner. È necessario spostare l'account accedendo a console di gestione pacchetti con l'account aziendale (credenziali di accesso) avviare il processo di migrazione. Dopo aver completato i passaggi per spostare l'account è possibile iniziare a gestire l'appartenenza e assegnare autorizzazioni e ruoli utente per il team affinché possano accedere ai vantaggi e consentono di gestire l'appartenenza. Microsoft esegue automaticamente la migrazione di competenze correnti, vantaggi, località, le informazioni bancarie o fiscali per incentivi e le associazioni MCP, incluso l'accesso Partner University.

Microsoft esegue automaticamente la migrazione di competenze correnti, vantaggi, località, le informazioni bancarie o fiscali per incentivi e le associazioni MCP, incluso l'accesso Partner University.

**Come cambierà la politica di rinnovo?**

 Nel centro per i Partner, la finestra di rinnovo è dalla data di anniversario tramite i seguenti 30 giorni.

**Saranno nostro competenze rimangono invariate dopo che si passa al centro per i Partner?**

Sì, alle competenze non influirà dallo spostamento al centro per i Partner. Se si notano discrepanze, contattare [supporto](https://partner.microsoft.com/support).


 **Vantaggi offerti da (inclusi i vantaggi del cloud, supporto tecnico, vantaggi di software, Visual Studio) cambierà dopo abbiamo spostato?**

 I tuoi vantaggi idonei non verranno modificato. Se si notano discrepanze, contattare [supporto](https://partner.microsoft.com/support).

 **Verrà rispettato l'account Microsoft che ha allocazioni di vantaggi di Visual Studio?**

 Sì. Vantaggi di Wisual Studio allocati a MSAs verranno rispettati e conservati. Verranno inoltre mantenuti dopo il rinnovo nel centro per i Partner. Tuttavia, se si rimuove un'allocazione di account del servizio gestito di una volta eseguita la migrazione nel centro per i Partner, non può essere aggiunto nuovamente al Partner Center.

Solo l'amministratore MPN è possibile aggiungere le allocazioni di vantaggio di Visual Studio per usare gli account nel tenant di Azure AD della società.

L'amministratore globale per più tenant AAD quando tutti i tenant siano associati allo stesso account, Centro per i Partner possono aggiungere utenti in tutti i tenant di questi vantaggi di Visual Studio e le allocazioni basate sull'utilizzo di Azure. 

 **Come dovremmo vengono gestiti gli associazioni MCP e l'accesso Partner University?**

 Sono state apportate modifiche alle associazioni MCP che si spostano dalla console di gestione pacchetti. Tuttavia, eventuali nuovi dipendenti di nuovo dopo aver spostato al centro per i Partner dovrà essere associato nel centro per i Partner. Tutte le autorizzazioni di Partner University per gli utenti esistenti verranno mantenuti, ma eventuali nuovi dipendenti devono accedere al [centro di formazione](https://partner.microsoft.com/training) per informazioni su come effettuare l'accesso in Partner University.

 **Riferimenti al cliente vengono usati nel centro per i Partner?**

 No, non occorre riferimenti al cliente per soddisfare i requisiti di competenza nel centro per i Partner.

 **Le associazioni di Partner of Record passerà al centro per i Partner?**

 Sì, non è disponibile alcuna modifica al Partner of Record. Altre informazioni sulle [il collegamento all'ID partner ai tuoi clienti](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**È previsto un impatto sull'incentivi?**

Non vi è alcun impatto sugli incentivi. Inoltre, se l'azienda dispone di più account nella console di gestione pacchetti e, quando si sposta in Partner Center tali account sono consolidati in un account globale, non sarà alcun impatto per i partner di incentivi in base al record.

**Quali sono i ruoli utente incentivi nel centro per i Partner?** 

Incentivi ruoli nel centro per i Partner sono basati sulla posizione e includono amministratore di incentivi e incentivi utente. Per altre informazioni sulle funzionalità di questi ruoli, vedere [assegnare ruoli agli utenti e autorizzazioni](permissions-overview.md).

**Incentivi possono essere gestiti a livello di globale e la posizione?**

 Sì. È possibile assegnare un amministratore di incentivi per essere l'amministratore di incentivi per tutte le posizioni oppure ogni percorso può avere un proprio amministratore di incentivi.

**Riguardanti i riferimenti, quanti profili business possiamo creare?**

La società possibile creare diversi profili di business come la necessità di rappresentano completamente gli interessi dell'azienda. In ogni profilo business, è possibile elencare fino a cinque aree, un'unica posizione per ogni paese. Ogni profilo business per usufruire dei riferimenti per ognuno dei relativi percorsi.

**Modo in cui saranno dei riferimenti assegnati, le modifiche che posso aspettarmi? Ad esempio, se si dispone di un'azienda in un mercato globale e i percorsi in altri mercati, come i riferimenti riceveranno?**

I riferimenti vengono assegnati in base ai parametri di ricerca che definisce il cliente. Quindi, indipendentemente dal fatto che un'unica posizione o molti, se i clienti specifica una posizione desiderata e si dispone sono un'azienda che soddisfa gli altri parametri, quindi il riferimento andrebbe in tale posizione.








