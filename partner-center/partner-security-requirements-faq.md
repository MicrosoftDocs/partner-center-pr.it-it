---
title: Domande frequenti sui requisiti di sicurezza per i partner
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Domande frequenti sui requisiti di sicurezza dei partner: cosa sono, come devono essere implementate dai partner e come sapere se sono state soddisfatte.'
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 203afa3fd238222e902a06ac3c173876e185f025
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679273"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Domande frequenti sui requisiti di sicurezza per i partner

**Utenti appropriati**

- Tutti gli utenti abilitati, inclusi gli utenti guest

Questo articolo contiene alcune domande frequenti sui [requisiti di sicurezza per i partner](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisiti di sicurezza per i partner

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>Quali sono i requisiti di sicurezza dei partner e perché devono essere implementati dai partner?

Tra le nostre priorità principali vi è una maggiore e costante tutela della sicurezza e della privacy e continuiamo ad aiutare i partner a proteggere i loro clienti e tenant. Continuano infatti a perpetrarsi attacchi alla sicurezza sempre più sofisticati, principalmente correlati a eventi imprevisti di compromissione dell'identità. Poiché i controlli preventivi svolgono un ruolo fondamentale in una strategia di difesa complessiva volta a contrastare gli attacchi alla sicurezza, nel 2019 abbiamo introdotto una serie di [requisiti di sicurezza obbligatori](partner-security-requirements.md). Per essere conformi, tutti i partner che partecipano al programma Cloud Solution Provider (CSP), i fornitori di pannelli di controllo e gli Advisor devono implementare i requisiti.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quali sono le tempistiche e le attività cardine?

Le condizioni associate ai requisiti di sicurezza sono incluse nel Contratto Microsoft Partner del 2019. Questi requisiti di sicurezza dovranno essere implementati prima possibile per la conformità alla partecipazione al programma CSP.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Cosa accade se non vengono implementati questi requisiti di sicurezza dei partner?

Il Contratto Microsoft Partner prevede che venga imposta l'autenticazione a più fattori per gli account utente e che venga adottato il modello di applicazione sicura per l'interazione con l'API di Partner Center. 

I partner che non rispettano queste procedure di sicurezza possono perdere la facoltà di effettuare transazioni nel programma CSP o gestire i tenant dei clienti usando i diritti di amministratore delegato.

### <a name="does-this-apply-to-all-geographies"></a>Queste informazioni sono valide per tutte le aree geografiche?

Sì, queste informazioni fanno riferimento a tutte le aree geografiche? È fortemente consigliabile che tutti i partner che effettuino transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, non è necessario che questi partner soddisfino i nuovi requisiti di sicurezza a partire dal 1° agosto. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>È possibile ottenere un'esclusione per un account?

No, non è possibile escludere alcun account utente dal requisito di imposizione dell'autenticazione MFA. Considerati i privilegi elevati della condizione di partner, il Contratto Microsoft Partner prevede che l'autenticazione a più fattori venga imposta a tutti gli account utente presenti nel tenant del partner.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Come faccio a sapere se soddisfo i requisiti di sicurezza per i partner?

Devi verificare i punti seguenti:

- Devi soddisfare tutti i requisiti indicati nei [requisiti di sicurezza dei partner](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Devi assicurarti che per tutti gli account utente del tuo tenant partner sia applicata l'autenticazione a più fattori.

Per identificare le principali aree in cui puoi eseguire azioni, tramite il Centro per i partner forniamo il report sullo [stato dei requisiti di sicurezza](https://partner.microsoft.com/pcv/security/compliance).

Per altre informazioni sul report di stato, vedi [Stato dei requisiti di sicurezza per i partner](https://docs.microsoft.com/partner-center/partner-security-compliance).

## <a name="required-actions"></a>Azioni richieste

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quali sono le azioni chiave che è necessario intraprendere per soddisfare i requisiti?

Tutti i partner del programma CSP (partner con fatturazione diretta, provider indiretto e rivenditore indiretto), gli Advisor e i fornitori di pannelli di controllo devono soddisfare i requisiti.

1. **Applicazione di MFA a tutti gli utenti**

    Tutti i partner del programma CSP, gli Advisor e i fornitori di pannelli di controllo devono applicare l'autenticazione MFA a tutti gli utenti inclusi nel tenant del partner.

    Considerazioni aggiuntive:

    - I provider indiretti devono collaborare con rivenditori indiretti per poter eseguire l'onboarding nel Centro per i partner, qualora non lo abbiano già fatto, e incoraggiare i rivenditori a soddisfare i requisiti.
    - L'autenticazione MFA di Azure viene resa disponibile per tutti gli utenti del tenant del partner senza costi aggiuntivi tramite le impostazioni predefinite per la sicurezza Azure AD con l'unico metodo di verifica di un'applicazione di autenticazione che supporta Time-Based One-Time Passwords (TOTP).
    - Se sono necessari altri metodi di verifica, ad esempio una telefonata o un SMS, è possibile ricorrere a metodi aggiuntivi tramite le SKU [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).
    - Quando accedono ai servizi cloud commerciali Microsoft, i partner possono usare anche una soluzione MFA di terze parti per ogni account.

2. **Adottare il framework del modello di applicazione sicura**

    Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un errore correlato alla distribuzione della soluzione MFA. Le risorse seguenti offrono una panoramica e preziose indicazioni su come adottare il modello.

    - [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro per i partner: guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Se usi un pannello di controllo per l'adozione del framework del modello di applicazione sicura, rivolgiti al fornitore.

    I fornitori di pannelli di controllo devono infatti eseguire l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro per i partner come fornitore di pannelli di controllo e avviare subito l'implementazione di questo requisito. Vedere [Centro per i partner: framework del modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). I fornitori di pannelli di controllo devono accettare e usare il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Che cos'è la Multi-Factor Authentication (MFA)?

MFA è un meccanismo di sicurezza che consente agli utenti di eseguire l'autenticazione tramite più di una procedura di sicurezza e convalida. In particolare, richiede due o più dei seguenti metodi di verifica:

- Un elemento noto, in genere una password
- Un oggetto fisico (un dispositivo attendibile non facilmente duplicabile, come un telefono)
- Una caratteristica personale (biometria)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Quanto costa abilitare l'autenticazione MFA?

Microsoft offre l'autenticazione MFA senza costi aggiuntivi tramite l'implementazione delle impostazioni predefinite per la sicurezza Azure AD. L'unica opzione di verifica disponibile con questa versione di MFA è un'applicazione di autenticazione. Se si preferisce usare una telefonata o un SMS come opzione di verifica, sarà necessario acquistare una licenza di [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). In alternativa, puoi usare una soluzione di terze parti per fornire l'autenticazione MFA per ogni utente incluso nel tenant del partner. In questo caso, è tua responsabilità assicurare che la soluzione MFA venga applicata e che siano rispettati tutti i requisiti.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Se ho già una soluzione MFA, quali azioni devo eseguire?

Attraverso questi requisiti di sicurezza, agli utenti inclusi nel tenant di un partner sarà richiesto di eseguire l'autenticazione MFA quando accedono ai servizi cloud commerciali Microsoft. Per soddisfare questi requisiti, puoi usare una soluzione di terze parti. Microsoft non fornisce più test di convalida ai provider di identità indipendenti per la compatibilità con Azure Active Directory. Per testare l'interoperabilità del prodotto, consulta queste [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Se usi una soluzione di terze parti, è importante verificare che la soluzione rilasci l'attestazione AMR (Authentication Method Reference) contenente il valore MFA. Per informazioni dettagliate su come verificare che la soluzione di terze parti rilasci l'attestazione prevista, vedi [Test dei requisiti di sicurezza dei partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements).

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Se vengono usati più tenant di partner per eseguire la transazione, e necessario implementare l'autenticazione MFA su tutti i tenant?

Sì, devi applicare l'autenticazione MFA per ogni tenant di Azure Active Directory associato al programma CSP o al programma Advisor. Per acquistare una licenza Premium di Azure Active Directory, è necessario acquistare una licenza per l'utente in ogni tenant di Azure Active Directory.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>È necessario che l'autenticazione MFA venga imposta a ogni account utente incluso nel tenant del partner?

Sì, per ogni utente sarà necessario imporre l'autenticazione MFA. Tuttavia, se usi le impostazioni predefinite per la sicurezza Azure AD, non è necessaria alcuna azione aggiuntiva perché tale funzionalità applica l'autenticazione MFA a tutti gli account utente. L'abilitazione delle impostazioni predefinite per la sicurezza è un modo semplice e gratuito per garantire che gli account utente siano conformi all'autenticazione MFA e non subiscano effetti quando questa viene applicata.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sono un partner con fatturazione diretta con Microsoft. Come devo procedere?

I partner Cloud Solution Provider con fatturazione diretta devono applicare l'autenticazione MFA per ogni utente incluso nel tenant del partner.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Sono un rivenditore indiretto ed eseguo le transazioni solo tramite un distributore. Devo comunque effettuare questa procedura?

Tutti i rivenditori indiretti sono tenuti ad applicare l'autenticazione MFA per ogni utente incluso nel tenant del partner. Questa azione deve essere eseguita dal rivenditore indiretto.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Se non uso l'API di Partner Center, è comunque necessario implementare l'autenticazione MFA?

Sì, questo requisito di sicurezza è valido per tutti gli utenti, inclusi gli utenti amministratori del partner e gli utenti finali di un tenant del partner.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quali fornitori di terze parti offrono soluzioni MFA compatibili con Azure Active Directory?

Quando valutano fornitori e soluzioni MFA, i partner devono accertarsi che la soluzione scelta sia compatibile con Azure Active Directory.

Microsoft non fornisce più test di convalida ai provider di identità indipendenti per la compatibilità con Azure Active Directory. Se vuoi testare l'interoperabilità di un prodotto, consulta queste [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

Per altre informazioni, vedi [Elenco di compatibilità della federazione di Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Come è possibile testare l'autenticazione MFA in una sandbox di integrazione?

Le impostazioni predefinite per la sicurezza Azure AD devono essere abilitate o in alternativa puoi usare una soluzione di terze parti basata sulla federazione.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>L'abilitazione dell'autenticazione MFA influirà sulla modalità di interazione con il tenant del mio cliente?

No. L'applicazione di questi requisiti di sicurezza non avrà alcun effetto sulle modalità di gestione dei clienti. Non verrà ad esempio annullata la possibilità di eseguire operazioni amministrative delegate.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Anche i clienti devono soddisfare i requisiti di sicurezza dei partner?

No, non è necessario applicare l'autenticazione MFA anche agli utenti inclusi nei tenant Azure AD dei clienti. Si consiglia tuttavia di collaborare con ogni cliente per determinare le procedure migliori per proteggere i rispettivi utenti.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>È possibile escludere un utente da questi requisiti?

No, l'autenticazione MFA è prevista per tutti gli utenti inclusi nel tenant del partner, inclusi gli account di servizio.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>I requisiti di sicurezza dei partner vengono applicati anche alla sandbox di integrazione?

Sì, i requisiti di sicurezza dei partner vengono applicati anche alla sandbox di integrazione. Questo significa che dovrai implementare la soluzione MFA appropriata per gli utenti inclusi nel tenant della sandbox di integrazione. Per fornire l'autenticazione MFA, è consigliabile implementare le impostazioni predefinite per la sicurezza Azure AD.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Come è possibile configurare un account di accesso di emergenza (break glass)?

È consigliabile creare uno o due account di accesso di emergenza per evitare di non poter accedere accidentalmente al tenant di Azure AD. In merito ai requisiti di sicurezza dei partner, è necessario che ogni utente esegua l'autenticazione tramite Multi-Factor Authentication. Questo significa dovrai modificare la definizione di un account di accesso di emergenza. Potrebbe trattarsi, ad esempio, di un account che usa una soluzione di terze parti per l'autenticazione MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Se uso una soluzione di terze parti, è necessario Active Directory Federation Services (ADFS)?

No, non è necessario avere Active Directory Federation Services (ADFS) se usi una soluzione di terze parti. Si consiglia di rivolgersi al fornitore della soluzione per determinare quali sono i requisiti per la soluzione.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>È necessario abilitare le impostazioni predefinite per la sicurezza Azure AD?

No, non è necessario abilitarle.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>È possibile usare l'accesso condizionale per soddisfare il requisito di autenticazione MFA?

Sì, è possibile usare l'accesso condizionale per applicare l'autenticazione MFA a ogni utente presente nel tenant del partner, inclusi gli account di servizio. Considerati i privilegi elevati della condizione di partner, è tuttavia necessario garantire che ogni utente disponga di una richiesta MFA per ogni singola autenticazione. Questo significa che non potrai usare la funzionalità di accesso condizionale che elude il requisito dell'autenticazione MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>L'account di servizio usato da Azure AD Connect sarà interessato dai requisiti di sicurezza dei partner?

No, l'account di servizio usato da Azure AD Connect non sarà interessato dai requisiti di sicurezza dei partner. Se si verifica un problema con Azure AD Connect in seguito all'applicazione dell'autenticazione MFA, aprire una richiesta di assistenza tecnica con il servizio di supporto tecnico Microsoft.

## <a name="secure-application-model"></a>Modello di applicazione sicura

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Chi deve adottare il modello di applicazione sicura per soddisfare i requisiti?

Microsoft sta introducendo un framework scalabile e sicuro per l'autenticazione dei partner Cloud Solution Provider (CSP) e dei fornitori di pannelli di controllo (CPV) che usano Multi-Factor Authentication. Per altre informazioni, vedere la [Guida del modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Che cos'è il modello di applicazione sicura?

Microsoft sta introducendo un framework scalabile e sicuro per l'autenticazione dei partner Cloud Solution Provider (CSP) e dei fornitori di pannelli di controllo (CPV) che usano Multi-Factor Authentication. Per altre informazioni, vedere la [Guida del modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Come viene implementato il modello di applicazione sicura?

Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un errore correlato alla distribuzione della soluzione MFA. Le risorse seguenti offrono una panoramica e preziose indicazioni su come adottare il modello.

- [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Se usi un pannello di controllo, devi rivolgerti al fornitore per informazioni sull'adozione del framework del modello di applicazione sicura.

I fornitori di pannelli di controllo devono infatti eseguire l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro per i partner come fornitore di pannelli di controllo e avviare subito l'implementazione di questo requisito. Vedere [Centro per i partner: framework del modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). I fornitori di pannelli di controllo devono accettare e usare il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Il modello di applicazione sicura deve essere implementato solo per l'API/SDK del Centro per i partner?

L'applicazione dell'autenticazione a più fattori per tutti gli account utente influirà su ogni automazione o integrazione progettata per essere eseguita in modalità non interattiva. Anche se i requisiti di sicurezza per i partner richiedano di abilitare il modello di applicazione sicura per l'API del Centro per i partner, è possibile sfruttarlo per soddisfare la necessità di un secondo fattore di autenticazione con l'automazione e l'integrazione. 

>[!Note] 
>La risorsa a cui si accede deve supportare l'autenticazione basata su token di accesso.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Sono in uso strumenti di automazione come PowerShell. Come viene implementato il modello di applicazione sicura?

Se la tua automazione è progettata per essere eseguita in modo non interattivo e si basa su credenziali utente per l'autenticazione, dovrai implementare il modello di applicazione sicura. Vedere [Modello di applicazione sicura | PowerShell per Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) per informazioni su come implementare questo framework.  

>[!Note] 
>Non tutti gli strumenti di automazione offrono la possibilità di eseguire l'autenticazione usando token di accesso. Per assistenza nella comprensione delle modifiche da apportare, pubblica un messaggio nel gruppo [Partner Center Security Guidance](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance). 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quali credenziali utente devono essere fornite dall'amministratore dell'applicazione durante l'esecuzione del processo di consenso?

Si consiglia di usare un account di servizio a cui sono assegnate autorizzazioni con privilegi minimi. Per quanto riguarda l'API del Centro per i partner, questo significa che devi usare un account a cui è assegnato il ruolo Agente di vendita o Agente amministratore.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Perché l'amministratore dell'applicazione non deve fornire credenziali di amministratore globale durante l'esecuzione del processo di consenso?

Per ridurre i rischi, è consigliabile usare identità con privilegi minimi e non un account con privilegi di amministratore globale, perché in questo modo verrebbero fornite autorizzazioni superiori al necessario.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Com'è possibile per i partner CSP sapere se i rispettivi fornitori di pannelli di controllo (CPV) stanno lavorando all'implementare della soluzione?

I partner che usano una soluzione sviluppata da un fornitore di pannelli di controllo (CPV) per eseguire transazioni nel programma Cloud Solution Provider (CSP) sono tenuti a rivolgersi direttamente al fornitore.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Chi sono i fornitori di pannelli di controllo (CPV)?

Un fornitore di pannelli di controllo è un fornitore di software indipendente che sviluppa app a disposizione dei partner CSP che eseguono l'integrazione con un'API del Centro per i partner. Un fornitore di pannelli di controllo non è un partner CSP con accesso diretto al dashboard o alle API del Centro per i partner. Una descrizione dettagliata è disponibile nell'articolo [Centro per i partner: Guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Come può essere eseguita la registrazione dai fornitori di pannelli di controllo (CPV)?

Per registrarsi come fornitore di pannelli di controllo, attenersi alle linee guida riportate [qui](https://docs.microsoft.com/partner-center/enroll-as-cpv).

I fornitori di pannelli di controllo devono contattare [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) per ricevere il collegamento di iscrizione e specificare un dipendente Microsoft sponsor che abbia una relazione commerciale con il fornitore di pannelli di controllo e ne conosca il tipo di attività, ad esempio un Partner Development Manager (PDM).

Dopo l'iscrizione al Centro per i partner e la registrazione delle applicazioni, potrai accedere alle API del Centro per i partner. Se sei un nuovo fornitore di pannelli di controllo, riceverai le informazioni sulla sandbox tramite una notifica del Centro per i partner. Dopo aver completato la registrazione come fornitore di pannelli di controllo Microsoft e aver accettato il contratto per CPV, è possibile:

1. Gestire un'applicazione multi-tenant (aggiungere applicazioni al portale di Azure, registrare e annullare la registrazione di applicazioni nel Centro per i partner). 
     >[!Note] 
     >per ottenere l'autorizzazione per le API del Centro per i partner, i fornitori di pannelli di controllo devono registrare le proprie applicazioni nel Centro per i partner. La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner.
2. Visualizzare e gestire il profilo dei fornitori di pannelli di controllo.
3. Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo. L'unico ruolo che un fornitore di pannelli di controllo può avere è quello di amministratore globale.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Per i partner che usano il Partner Center SDK, l'SDK adotterà automaticamente il modello di applicazione sicura?

No, dovrai seguire le indicazioni fornite nella [guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Posso generare un token di aggiornamento per il modello di applicazione sicura con account per i quali non è abilitata l'autenticazione MFA?

Sì, è possibile generare un token di aggiornamento anche con un account per il quale non è abilitata l'autenticazione MFA. Questa operazione, tuttavia, non dovrebbe essere eseguita perché tutti i token generati con un account che non usa l'autenticazione MFA non potranno accedere alle risorse a causa dei requisiti previsti per l'autenticazione MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>In che modo un'applicazione può ottenere un token di accesso se si abilita l'autenticazione MFA?

È necessario attenersi alla [guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf), che fornisce informazioni dettagliate su come eseguire questa operazione rispettando al tempo stesso i nuovi requisiti di sicurezza. È possibile trovare il codice di esempio .NET [qui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e il codice di esempio Java [qui](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>I fornitori di pannelli di controllo devono creare un'applicazione Azure AD nel tenant del CPV o nel tenant del partner CSP?

I fornitori di pannelli di controllo dovranno creare l'applicazione Azure Active Directory nel tenant associato alla rispettiva registrazione come fornitore di pannello di controllo.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>I partner CSP che usano l'autenticazione solo tramite app devono apportare modifiche?

L'autenticazione solo tramite app non subisce modifiche perché le credenziali utente non vengono usate per richiedere un token di accesso. Se le credenziali utente vengono condivise, i fornitori di pannelli di controllo devono adottare il [framework del modello applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) ed eliminare eventuali credenziali di partner esistenti.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>I fornitori di pannelli di controllo possono sfruttare il metodo di autenticazione solo tramite app per ottenere i token di accesso?

No, i partner fornitori di pannelli di controllo non possono usare il metodo di autenticazione solo tramite app per richiedere token di accesso per conto del partner. Devono invece implementare il modello di applicazione sicura, che usa il metodo di autenticazione app + utente.

## <a name="technical-enforcement"></a>Applicazione tecnica

### <a name="what-is-the-activation-of-security-safeguards"></a>Che cos'è l'attivazione di misure di sicurezza?

Per essere conformi, tutti i partner che partecipano al programma Cloud Solution Provider (CSP), i fornitori di pannelli di controllo (CPV) e gli Advisor devono implementare i requisiti di sicurezza obbligatori.

Per fornire protezione aggiuntiva, Microsoft ha avviato l'attivazione di misure di sicurezza che consentono ai partner di proteggere i loro tenant e clienti imponendo la verifica dell'autenticazione a più fattori (MFA) per evitare accessi non autorizzati.  

Abbiamo completato l'attivazione delle funzionalità di amministrazione per conto terzi (AOBO, Admin On Behalf Of) per tutti i tenant del partner. Per proteggere ulteriormente partner e clienti, puntando al secondo trimestre dell'anno 2020 avvieremo l'attivazione delle transazioni del Centro per i partner in CSP, aiutando i partner a proteggere le loro attività e i clienti da eventi imprevisti correlati al furto di identità.

Per altre informazioni, visita la pagina [Imposizione dell'autenticazione a più fattori per il tenant del partner](partner-security-requirements-mandating-mfa.md).

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Uso una soluzione MFA di terze parti e vengo bloccato. Cosa devo fare?

Per verificare che l'account per l'accesso alle risorse sia stato testato per l'autenticazione a più fattori, controlleremo l'attestazione [AMR (Authentication Method Reference)](https://tools.ietf.org/html/rfc8176) per vedere che nell'elenco sia presente l'autenticazione MFA. Alcune soluzioni di terze parti non rilasciano questa attestazione o non includono il valore MFA. Se l'attestazione non è presente o il valore MFA non è elencato, non esiste alcun modo per determinare se l'account autenticato è stato testato per l'autenticazione a più fattori. Dovrai collaborare con il fornitore della soluzione di terze parti per determinare quali azioni eseguire affinché la soluzione rilasci l'attestazione Authentication Method Reference.

Se non sei certo che la soluzione di terze parti rilasci l'attestazione prevista, vedi [Test dei requisiti di sicurezza dei partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0).

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA mi impedisce di supportare i miei clienti usando Amministra per conto terzi. Come posso procedere?

L'applicazione tecnica dei requisiti di sicurezza per i partner verificherà se l'account autenticato è stato testato per l'autenticazione a più fattori. Se l'account non è stato sottoposto a questa verifica, verrai reindirizzato alla pagina di accesso e ti verrà chiesto di eseguire di nuovo l'autenticazione. Per consultare esperienze e indicazioni più dettagliate, vedi il documento [Imposizione dell'autenticazione a più fattori per il tenant del partner](partner-security-requirements-mandating-mfa.md#partner-delegated-administration). Nello scenario in cui il tuo dominio non è federato, dopo l'autenticazione ti verrà chiesto di configurare l'autenticazione a più fattori. Al termine, potrai gestire i clienti usando la funzionalità di amministrazione per conto terzi (AOBO). Nello scenario in cui invece il tuo dominio è federato, dovrai assicurarti che l'account venga testato per l'autenticazione a più fattori.

## <a name="security-defaults-transition"></a>Transizione alle impostazioni predefinite per la sicurezza

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>In che modo posso passare dai criteri di base alle impostazioni predefinite per la sicurezza o ad altre soluzioni MFA?

I [criteri di base di Azure Active Directory (Azure AD) vengono rimossi e sostituiti](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) con le impostazioni predefinite per la sicurezza, un set completo di criteri di protezione per te e i tuoi clienti. Le [impostazioni predefinite per la sicurezza](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) aiutano a proteggere la tua organizzazione da attacchi alla sicurezza correlati al furto di identità.

Se non sei passato dai criteri di base al criterio delle impostazioni predefinite per la sicurezza o ad altre [opzioni di implementazione MFA](partner-security-requirements.md#actions-that-you-need-to-take), la tua implementazione dell'autenticazione a più fattori verrà rimossa a causa del ritiro dei criteri di base. A tutti gli utenti dei tuoi tenant del partner che eseguono operazioni protette dall'autenticazione a più fattori verrà richiesto di effettuare la verifica dell'autenticazione a più fattori. Per indicazioni più dettagliate, consulta [qui](partner-security-requirements-mandating-mfa.md).
Per essere conforme e ridurre le interruzioni, esegui una delle azioni seguenti:

- Transizione alle impostazioni predefinite per la sicurezza
    - Il criterio delle impostazioni predefinite per la sicurezza è una delle opzioni che possono essere scelte dai partner per implementare l'autenticazione a più fattori. Viene offerto un livello di sicurezza di case, abilitato senza costi aggiuntivi.
    - Scopri come abilitare l'autenticazione a più fattori per la tua organizzazione usando Azure AD ed esamina le [considerazioni principali sulle impostazioni predefinite per la sicurezza](partner-security-requirements.md#security-defaults).
    - Abilita il criterio delle impostazioni predefinite per la sicurezza se risponde alle tue esigenze aziendali.
- Transizione all'accesso condizionale
    - Se il criterio delle impostazioni predefinite per la sicurezza non risponde alle tue esigenze, abilita l'accesso condizionale. Per altre informazioni, consulta la documentazione relativa all'accesso condizionale di Azure AD.

## <a name="key-resources"></a>Risorse principali

### <a name="how-to-get-started"></a>Operazioni preliminari

- [Requisiti di sicurezza per i partner: guida dettagliata](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Indirizzare eventuali domande e commenti a questo [gruppo di linee guida per la sicurezza del Centro per i partner](https://aka.ms/MPCSecurityGuidance).
- Partecipare ai prossimi webinar per i partner. Controlla [qui il programma dettagliato e le risorse](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Risorse per l'adozione di un modello di applicazione sicura

- [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: guida al modello di applicazione sicura](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Supporto

### <a name="where-can-i-get-support"></a>Dove è possibile richiedere il supporto tecnico?

Per le risorse di supporto a cui è possibile ricorrere per soddisfare i requisiti di sicurezza, se si dispone del supporto avanzato per i partner (ASfP), contattare il servizio Gestione account servizio; se invece si dispone del supporto tecnico Premier per i partner (PSfP), contattare il servizio Gestione account servizio o il Technical Account Manager.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Come è possibile ottenere assistenza e informazioni tecniche per l'adozione del framework del modello di applicazione sicura?

Le opzioni di supporto tecnico di prodotto per Azure Active Directory sono disponibili tramite i vantaggi MPN. I partner con accesso a una sottoscrizione ASfP o PSfP attiva possono collaborare con il rispettivo Account Manager (SAM/TAM) per comprendere meglio le opzioni disponibili.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Come è possibile contattare il supporto se si perde l'accesso al Centro per i partner?

Passa a [Supporto Microsoft Partner](https://partner.microsoft.com/support) e quindi scegli **Show all support options** (Mostra tutte le opzioni di supporto). Visualizzerai le opzioni disponibili per contattare il supporto per i partner Microsoft. Le opzioni includono un numero di telefono per chiamare il supporto e un'opzione per chattare con il supporto. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Dove è possibile trovare altre informazioni sui problemi tecnici più comuni?

Informazioni sui problemi tecnici sono comuni disponibili [qui.](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)

