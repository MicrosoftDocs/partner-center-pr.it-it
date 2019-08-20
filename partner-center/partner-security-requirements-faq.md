---
title: Domande frequenti sui requisiti di sicurezza dei partner | Centro per i partner
ms.topic: article
ms.date: 07/18/2019
description: Domande frequenti sui requisiti di sicurezza dei partner
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provider di soluzioni cloud, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, multi-factor authentication, autenticazione a più fattori, modello di applicazione sicura, modello di applicazione sicura, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820595"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Domande frequenti sui requisiti di sicurezza dei partner

Questo articolo contiene alcune domande frequenti sui requisiti di [sicurezza dei partner](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisiti di sicurezza dei partner

### <a name="what-are-the-new-partner-security-requirements"></a>Quali sono i nuovi requisiti di sicurezza dei partner?

Per proteggere i partner e i clienti, è necessario che i partner intraprendano immediatamente le azioni seguenti:  

1. **Abilitare l'autenticazione a più fattori per tutti gli utenti nei tenant partner**. Tutti gli utenti nei tenant partner devono usare l'autenticazione a più fattori quando accedono a servizi cloud commerciali Microsoft o a transazioni in CSP tramite il centro per i partner o tramite API. Grazie all'abilitazione dei criteri di protezione di base, l'autenticazione a più fattori è disponibile gratuitamente per tutti gli utenti dei tenant partner.

2. **Adottare il Framework del modello applicativo protetto**. Tutti i partner che si integrano con un'API Microsoft, ad esempio Azure Resource Manager, Microsoft Graph e l'API del centro per i partner, devono adottare il Framework del modello applicativo sicuro per evitare eventuali problemi di integrazione quando i criteri di base sono abilitati. 
 
L'abilitazione dell'autenticazione a più fattori e l'adozione del Framework del modello applicativo sicuro consentono di proteggere l'infrastruttura e salvaguardare i dati dei clienti da potenziali rischi per la sicurezza, ad esempio l'identificazione di furti o altri eventi illeciti.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quali partner devono soddisfare i requisiti?

Questi requisiti sono per i seguenti gruppi di partner:
- Tutte le organizzazioni partner che partecipano al programma Cloud Solution Provider (CSP) che operano usando i servizi cloud commerciali Microsoft
  - Partner di fatturazione diretta
  - Provider indiretti
  - Rivenditori indiretti
- Tutti i fornitori del pannello di controllo
- Tutti i partner del programma Advisor  

Tutti i partner che trasformano tramite un cloud sovrano (21Vianet, US Government e Germania) non devono soddisfare i nuovi requisiti di sicurezza a partire dal 1 ° agosto. Tuttavia, si consiglia vivamente che tutti i partner che usano un cloud sovrano agisca e adottino immediatamente questi nuovi requisiti di sicurezza. Microsoft fornirà ulteriori dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quali sono le tempistiche e le attività cardine chiave?

I termini associati a questi requisiti di sicurezza verranno aggiunti immediatamente alla guida del programma Cloud Solution Provider. È necessario implementare questi requisiti di sicurezza affinché siano conformi alla partecipazione del programma CSP a partire dal 1 ° agosto 2019. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Cosa accade se non si eseguono azioni?

I partner che non riescono a rispettare queste procedure e obblighi di sicurezza non saranno in grado di eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti di amministratore delegato, una volta applicati questi requisiti di sicurezza per i partner. È in corso il processo di creazione di una data di imposizione per i requisiti e invierà una notifica ai partner della data con informazioni dettagliate.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Perché Microsoft impone questi nuovi requisiti?
Sicurezza e privacy dei clienti e dei partner è la principale priorità di Microsoft. Continuiamo a vedere un numero più sofisticato di attacchi alla sicurezza, principalmente correlati a eventi imprevisti di compromissione dell'identità. Poiché i controlli preventivi svolgono un ruolo fondamentale in una strategia di difesa complessiva per contrastare gli attacchi alla sicurezza, si inizierà a applicare un set di requisiti di sicurezza obbligatori per aiutare a proteggere i partner e i clienti.

### <a name="does-this-apply-to-all-geographies"></a>Si applica a tutte le aree geografiche?

Sì, si applica a tutte le aree geografiche. Si consiglia vivamente che tutti i partner che trasformano attraverso un cloud sovrano (21Vianet, US Government e Germania) agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, questi partner non devono soddisfare i nuovi requisiti di sicurezza a partire dal 1 ° agosto. Microsoft fornirà ulteriori dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

## <a name="required-actions"></a>Azioni obbligatorie

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quali sono le azioni chiave che è necessario eseguire per soddisfare i requisiti?  
Tutti i partner del programma CSP (Direct Bill, indirect provider e Reseller indirect), Advisor e fornitori del pannello di controllo devono soddisfare i requisiti.

1. **Applicare l'autenticazione a più fattori per tutti gli utenti**

    Per applicare l'autenticazione a più fattori per tutti gli utenti del tenant partner, è necessario che tutti i partner del programma CSP, degli Advisor e dei fornitori del pannello di controllo. Questa operazione può essere eseguita abilitando la richiesta di autenticazione a più fattori [per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), la baseline per la [protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)e i criteri di base futuri. La funzionalità fornita dai criteri di base continuerà a evolversi per garantire che i partner e i clienti siano protetti dalle minacce alla sicurezza in continua evoluzione. È quindi importante esaminare la documentazione dei criteri di [base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) per altre informazioni.

    - Vedere [criteri di base: Richiedere l'autenticazione a più](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) fattori per gli amministratori per informazioni dettagliate su come abilitare i criteri di base Richiedi autenticazione a più fattori per l'amministratore.
    - Vedere [criteri di base: Protezione](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) dell'utente finale per informazioni dettagliate su come abilitare i criteri di base per la protezione degli utenti finali.
    - Comprendere il concetto di [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considerazioni aggiuntive:

    - I provider indiretti devono collaborare con i rivenditori indiretti per l'onboarding nel centro per i partner, qualora non lo abbiano già fatto e incoraggino i rivenditori a soddisfare i requisiti.
    - L'autenticazione a più fattori di Azure viene resa disponibile a tutti gli utenti del tenant partner senza costi aggiuntivi tramite i criteri di base con l'unico metodo di verifica per l'uso dell' [App Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Sono disponibili metodi di verifica aggiuntivi tramite gli SKU [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) , se sono necessari altri metodi quali SMS o posta elettronica.
    - I partner possono inoltre sfruttare una soluzione di autenticazione a più fattori di terze parti per ogni utente durante l'accesso ai servizi cloud commerciali Microsoft.

2. **Adottare il Framework del modello applicativo sicuro**

    Tutti i partner che hanno sviluppato l'integrazione personalizzata usando qualsiasi API, ad esempio Azure Resource Manager, Microsoft Graph, API del centro per i partner e così via, o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [modello di applicazione protetta Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un'interruzione a causa della distribuzione dell'autenticazione a più fattori. Le risorse seguenti forniscono una panoramica e istruzioni su come adottare il modello.

    - [Panoramica del modello di applicazione protetta](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro per i partner: Guida al modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner nel programma CSP: codice di esempio .NET per l'abilitazione del modello applicativo sicuro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Partner nel programma CSP: Codice di esempio Java per l'abilitazione del modello di applicazione protetto](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Documento di autenticazione del centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento dell'autenticazione a più fattori di PowerShell per il centro per i partner](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Se si usa un pannello di controllo, è necessario rivolgersi al fornitore in merito all'adozione del Framework del modello applicativo protetto.

    I fornitori del pannello di controllo sono necessari per l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) nel centro per i partner come fornitore del pannello di controllo e iniziare subito a implementare questo requisito. Vedere il centro [per i partner: Framework](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)del modello applicativo protetto. I fornitori del pannello di controllo devono accettare e gestire il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-mfa"></a>Che cos'è l'autenticazione a più fattori?

Multi-factor authentication è un meccanismo di sicurezza, sebbene gli utenti siano autenticati tramite più di una procedura di sicurezza e convalida richiesta. Funziona richiedendo due o più dei metodi di autenticazione seguenti:

- Un elemento noto, in genere una password
- Un oggetto fisico (un dispositivo attendibile non facilmente duplicabile, come un telefono)
- Una caratteristica personale (biometria)

### <a name="what-are-baseline-protection-policies"></a>Che cosa sono i criteri di protezione di base? 

[Criteri di protezione di base Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (attualmente anteprima) sono un set di criteri predefiniti che consentono di proteggere le organizzazioni da molti attacchi comuni. Questi attacchi comuni possono includere spray, riproduzione e phishing delle password. I criteri di base sono disponibili in tutte le edizioni di Azure Active Directory. Microsoft sta rendendo disponibili i criteri di protezione di base a tutti perché gli attacchi basati sull'identità sono stati in crescita negli ultimi anni. L'obiettivo di questi criteri è garantire che tutte le organizzazioni dispongano di un livello di sicurezza di base abilitato senza costi aggiuntivi.

> [!NOTE]
> I criteri di base di Microsoft e le funzionalità correlate continueranno a evolversi per proteggere meglio i partner e i clienti dalle minacce alla sicurezza in continua evoluzione. È possibile che vengano apportate alcune modifiche di denominazione e tassonomia ai criteri di base. Si consiglia vivamente di visitare direttamente le pagine dei criteri di base per estrarre le informazioni più recenti.

### <a name="what-baseline-policies-must-i-enable"></a>Quali criteri di base è necessario abilitare?

Se si prevede di usare i criteri di protezione di base correnti per fornire l'autenticazione a più fattori per ogni utente nel tenant partner, è necessario abilitare la [richiesta di](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) autenticazione a più fattori per gli amministratori e i criteri di base per la [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . Questi criteri di protezione di base soddisferanno i requisiti per l'autenticazione a più fattori per ogni utente nel tenant partner, senza costi aggiuntivi, solo per i partner che usano Microsoft Authenticator app tramite il dispositivo mobile.

Il [criterio Richiedi](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) autenticazione a più fattori per amministratori viene usato per gli utenti amministratori nella directory dei partner e i criteri di base per la [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) vengono usati per proteggere gli utenti non amministratori nel tenant partner. Per abilitare questi criteri, gli utenti dovranno registrarsi per l'autenticazione a più fattori. Dopo che l'utente ha eseguito la registrazione, verrà richiesta l'autenticazione a più fattori durante i tentativi di accesso in base ai criteri del criterio. La funzionalità fornita dai criteri di base continuerà a evolversi per garantire che i partner e i clienti siano protetti dalle minacce alla sicurezza in continua evoluzione. È quindi importante esaminare la documentazione dei criteri di [base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) per altre informazioni.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Ricerca per categorie abilitare i criteri Richiedi autenticazione a più fattori per gli amministratori? 

È possibile abilitare i criteri di base Richiedi autenticazione a più fattori per gli amministratori tramite il portale di gestione di Azure. Vedere [criteri di base: ](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) Per informazioni dettagliate su come abilitare i criteri di base, richiedere l'autenticazione a più fattori per gli amministratori.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Ricerca per categorie abilitare i criteri di protezione dell'utente finale?

I criteri di base per la protezione degli utenti finali possono essere abilitati tramite il portale di gestione di Azure. Vedere [criteri di base: Protezione](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) dell'utente finale per informazioni dettagliate su come abilitare i criteri di base.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>I criteri di base verranno abilitati automaticamente? 

No, per abilitare questi criteri, un utente membro del ruolo amministratore globale, amministratore della sicurezza o amministratore accesso condizionale dovrà configurare i criteri per l'uso immediato dei criteri.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Qual è il costo dell'abilitazione dell'autenticazione a più fattori?

Microsoft offre l'autenticazione a più fattori senza costi aggiuntivi tramite l'implementazione di criteri di protezione di base per la protezione [dell'](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) autenticazione e dell' [amministratore](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) . L'unica opzione di verifica disponibile tramite questa versione di multi-factor authentication è l' [app Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se è richiesta una telefonata o un messaggio SMS, sarà necessario acquistare una licenza di [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . In alternativa, è possibile usare una soluzione di terze parti per fornire l'autenticazione a più fattori per ogni utente nel tenant del partner. in questo caso, è responsabilità dell'utente assicurarsi che la soluzione di autenticazione a più fattori venga applicata e che sia conforme.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Se si dispone già di una soluzione di autenticazione a più fattori, quali azioni è necessario eseguire?

Attraverso questi requisiti di sicurezza, gli utenti in un tenant partner dovranno eseguire l'autenticazione con l'autenticazione a più fattori quando accedono ai servizi cloud commerciali Microsoft. Per soddisfare questi requisiti, è possibile usare una soluzione di terze parti. Microsoft non fornisce più i test di convalida per i provider di identità indipendenti per la compatibilità con Azure Active Directory. Se si desidera testare il prodotto per l'interoperabilità, consultare le [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Quale metodo di verifica è possibile usare per autenticare l'autenticazione a più fattori?

Microsoft offre l'autenticazione a più fattori senza costi aggiuntivi tramite l'implementazione di criteri di protezione di base per la protezione [dell'](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) autenticazione e dell' [amministratore](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) . L'unica opzione di verifica disponibile tramite questa versione di multi-factor authentication è l' [app Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se è richiesta una telefonata o un messaggio SMS, sarà necessario acquistare una licenza di [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . In alternativa, è possibile usare una soluzione di terze parti per fornire l'autenticazione a più fattori per ogni utente nel tenant del partner. in questo caso, è responsabilità dell'utente assicurarsi che la soluzione di autenticazione a più fattori venga applicata e che sia conforme.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Si utilizzano più tenant partner per eseguire transazioni. È necessario implementare l'autenticazione a più fattori?

Sì, sarà necessario imporre l'autenticazione a più fattori per ogni tenant Azure Active Directory associato al programma CSP o al programma Advisor. Se si prevede di acquistare una licenza di Azure Active Directory Premium, è necessario acquistare una licenza per l'utente in ogni tenant di Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>È necessario applicare l'autenticazione a più fattori per ogni utente del tenant partner? 

I criteri di protezione [Richiedi autenticazione a](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) più fattori per l'amministratore e la [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) applicano l'autenticazione a più fattori per ogni utente nel tenant partner. Se si utilizzano questi criteri per fornire l'autenticazione a più fattori e si sta utilizzando l'applicazione [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) , non è necessario acquistare licenze aggiuntive. In caso contrario, sarà necessario acquistare una soluzione appropriata per fornire l'autenticazione a più fattori per ogni utente nel tenant partner.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sono un partner di fatturazione diretta con Microsoft. Quali operazioni è necessario eseguire?

Direct Bill Cloud Solution Provider partner deve applicare l'autenticazione a più fattori per ogni utente nel tenant partner.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Sono un rivenditore indiretto ed è solo un database di distribuzione. È ancora necessario eseguire questa operazione?

Tutti i rivenditori indiretti sono necessari per applicare l'autenticazione a più fattori per ogni utente nel tenant partner. Si tratta di un'azione che deve essere eseguita dal rivenditore indiretto.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Non utilizzo l'API del centro per i partner. È ancora necessario implementare l'autenticazione a più fattori?

Sì, questo requisito di sicurezza è per tutti gli utenti, inclusi gli utenti amministratori partner e gli utenti finali in un tenant partner.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quali fornitori di terze parti forniscono soluzioni di autenticazione a più fattori compatibili con Azure Active Directory?

Sono disponibili molte revisioni indipendenti delle soluzioni multi-factor authentication, ad esempio [Gartner](https://www.gartner.com/en/webinars/3881781). Quando si esaminano i fornitori e le soluzioni di autenticazione a più fattori, è necessario che i partner garantiscano che la soluzione scelta sia compatibile con Azure Active Directory.

Microsoft non fornisce più i test di convalida per i provider di identità indipendenti per la compatibilità con Azure Active Directory. Se si desidera testare il prodotto per l'interoperabilità, consultare le [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

Per ulteriori informazioni, vedere la [Azure ad elenco di compatibilità di Federazione](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Come è possibile testare l'autenticazione a più fattori nella sandbox di integrazione?

I criteri Richiedi autenticazione a più fattori [per amministratore](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e di base per la [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) devono essere abilitati per il tenant sandbox di integrazione. Tramite questo criterio, ogni utente del tenant sarà tenuto a eseguire l'autenticazione con l'autenticazione a più fattori.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>L'abilitazione dell'autenticazione a più fattori consente di interagire con il tenant del cliente? 

No. L'evasione di questi requisiti di sicurezza non avrà alcun effetto sulle modalità di gestione dei clienti. La possibilità di eseguire operazioni amministrative delegate non verrà interrotta.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>I clienti sono soggetti ai requisiti di sicurezza dei partner?

No, non è necessario applicare l'autenticazione a più fattori per ogni utente nei tenant Azure AD del cliente. Tuttavia, si consiglia di collaborare con ogni cliente per determinare il modo migliore per proteggere gli utenti.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>È possibile usare le password delle app con i criteri di protezione di base?

Sì, è possibile usare le [password dell'app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) . Esaminare le considerazioni per l'uso delle password di app documentate [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) per determinare se sono supportate in base alle esigenze.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>È possibile escludere qualsiasi utente da questo requisito? 

No, per ogni utente, inclusi gli account del servizio, nel tenant partner verrà richiesto di eseguire l'autenticazione con l'autenticazione a più fattori.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>I requisiti di sicurezza dei partner si applicano alla sandbox di integrazione?

Sì, i requisiti di sicurezza del partner si applicano alla sandbox di integrazione. Ciò significa che sarà necessario implementare la soluzione di autenticazione a più fattori appropriata per gli utenti nel tenant sandbox di integrazione. È consigliabile implementare i criteri di protezione di base per fornire l'autenticazione a più fattori.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Ricerca per categorie configurare un account di accesso di emergenza (Break Glass)?

È stata considerata una procedura consigliata creare uno o due account di accesso di emergenza per impedire che il tenant Azure AD venga bloccato inavvertitamente. Per quanto riguarda i requisiti di sicurezza dei partner, è necessario che ogni utente esegua l'autenticazione con multi-factor authentication. Questo significa che sarà necessario modificare la definizione di un account di accesso di emergenza. Potrebbe trattarsi di un account che sfrutta una soluzione di terze parti per l'autenticazione a più fattori.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>In che modo gli utenti Guest saranno interessati dai requisiti di sicurezza dei partner?

Gli utenti Guest dovranno eseguire l'autenticazione con l'autenticazione a più fattori quando accedono alle risorse nel tenant partner. I requisiti di sicurezza dei partner non avranno alcun effetto sull'accesso delle risorse al tenant da parte dell'utente Guest.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se si usa una soluzione di terze parti è Active Directory è necessario Servizio federativo (ADFS)? 

No, non è necessario disporre di Active Directory Servizio federativo (ADFS) se si utilizza una soluzione di terze parti. Si consiglia di collaborare con il fornitore della soluzione per determinare quali sono i requisiti per la soluzione.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>È necessario abilitare i criteri di protezione di base?

No, non è necessario abilitare i criteri di protezione di base. L'unico requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>L'accesso condizionale può essere usato per soddisfare il requisito di autenticazione a più fattori?

Sì, è possibile usare l'accesso condizionale per applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner. Tuttavia, data la natura altamente privilegiata di essere un partner, è necessario assicurarsi che ogni utente abbia una richiesta di autenticazione a più fattori per ogni singola autenticazione. Ciò significa che non sarà possibile sfruttare la funzionalità di accesso condizionale che elude il requisito per l'autenticazione a più fattori.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quali opzioni di verifica vengono fornite tramite l'implementazione dei criteri di protezione di base? 

Per quanto riguarda la versione di multi-factor authentication disponibile tramite l'implementazione dei criteri di protezione di base, l'unica opzione di verifica disponibile è un'app di autenticazione. L'utilizzo di una telefonata e di un messaggio di SMS è considerato meno sicuro. Quindi, queste opzioni non sono disponibili tramite questa versione di autenticazione a più fattori.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>L'account del servizio usato da Azure AD Connect sarà influenzato dai requisiti di sicurezza dei partner?

No, l'account del servizio usato da Azure AD Connect non verrà influenzato dai requisiti di sicurezza dei partner. Se si verifica un problema con Azure AD Connect come risultato dell'applicazione dell'autenticazione a più fattori, aprire una richiesta di supporto tecnico con il supporto tecnico Microsoft.

## <a name="secure-application-model"></a>Modello di applicazione protetto

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Chi deve adottare il modello di applicazione sicura per soddisfare i requisiti?

Microsoft introduce un framework sicuro e scalabile per l'autenticazione dei partner Cloud Solution Provider (CSP) e del pannello di controllo (CPV) che sfrutta l'autenticazione a più fattori. Per ulteriori informazioni, vedere la [Guida del modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) . Tutti i partner che hanno sviluppato l'integrazione personalizzata usando qualsiasi API, ad esempio Azure Resource Manager, Microsoft Graph, API del centro per i partner e così via, o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [modello di applicazione protetta Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per l'integrazione con i servizi cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Che cos'è il modello di applicazione protetta?

Microsoft introduce un framework sicuro e scalabile per l'autenticazione dei partner Cloud Solution Provider (CSP) e del pannello di controllo (CPV) che sfrutta l'autenticazione a più fattori. Per ulteriori informazioni, vedere la [Guida del modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

### <a name="how-do-i-implement-the-secure-application-model"></a>Ricerca per categorie implementare il modello di applicazione protetta?

Tutti i partner che hanno sviluppato l'integrazione personalizzata usando qualsiasi API, ad esempio Azure Resource Manager, Microsoft Graph, API del centro per i partner e così via, o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [modello di applicazione protetta Framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un'interruzione a causa della distribuzione dell'autenticazione a più fattori. Le risorse seguenti forniscono una panoramica e istruzioni su come adottare il modello.

- [Panoramica del modello di applicazione protetta](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: Guida al modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner nel programma CSP: codice di esempio .NET per l'abilitazione del modello applicativo sicuro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partner nel programma CSP: Codice di esempio Java per l'abilitazione del modello di applicazione protetto](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento di autenticazione del centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento dell'autenticazione a più fattori di PowerShell per il centro per i partner](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Se si usa un pannello di controllo, è necessario rivolgersi al fornitore in merito all'adozione del Framework del modello applicativo protetto.

I fornitori del pannello di controllo sono necessari per l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) nel centro per i partner come fornitore del pannello di controllo e iniziare subito a implementare questo requisito. Vedere il centro [per i partner: Framework](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)del modello applicativo protetto. I fornitori del pannello di controllo devono accettare e gestire il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Chi è un fornitore del pannello di controllo (CPV)? 
Un fornitore di un pannello di controllo è un fornitore di software indipendente che sviluppa app utilizzabili dai partner CSP per l'integrazione con le API del centro per i partner. Un fornitore del pannello di controllo non è un partner CSP con accesso diretto al dashboard o alle API del centro per i partner. Una descrizione dettagliata è disponibile nel centro [per i partner: Guida](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)al modello di applicazioni sicure.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Il modello di applicazione protetta deve essere implementato solo per l'API/SDK del centro per i partner? 

Quando sono abilitati i criteri di base Richiedi autenticazione a più fattori *per gli amministratori* e la *protezione degli utenti finali* , ogni utente dovrà eseguire l'autenticazione con multi-factor authentication. Ciò significa che sarà necessario implementare il modello di applicazione protetta per ogni API, interfaccia della riga di comando e modulo di PowerShell, ad esempio Azure, Azure AD, MS online, centro per i partner e così via, che deve essere eseguito in modo non interattivo e si basa sull'uso delle credenziali utente per l'autenticazione.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Si usano strumenti di automazione come PowerShell. Ricerca per categorie implementare il modello di applicazione protetta?  

Se l'automazione è progettata per essere eseguita in modo non interattivo e si basa su credenziali utente per l'autenticazione, sarà necessario implementare il modello di applicazione protetta. Vedere [modello di applicazione protetta | Centro per i partner PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) per indicazioni su come implementare questo Framework.  Si noti che non tutti gli strumenti di automazione offrono la possibilità di eseguire l'autenticazione usando i token di accesso. Per informazioni sulle modifiche che devono essere apportate, inviare un messaggio al gruppo di [linee guida](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) per la sicurezza del centro per i partner.

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quali sono le credenziali utente fornite dall'amministratore dell'applicazione durante l'esecuzione del processo di consenso? 

Si consiglia di utilizzare un account del servizio a cui sono state assegnate le autorizzazioni con privilegi minimi. Per quanto riguarda l'API del centro per i partner, questo significa che è necessario usare un account a cui è stato assegnato il ruolo agente di vendita o agenti di amministrazione.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Perché l'amministratore dell'applicazione non deve fornire le credenziali utente dell'amministratore globale quando esegue il processo di consenso?

È consigliabile usare il privilegio con privilegi minimi in modo da ridurre il rischio. Non è consigliabile usare un account che disponga di privilegi di amministratore globale, perché in questo modo verranno fornite più autorizzazioni rispetto a quelle richieste

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Sono un partner CSP. Ricerca per categorie verificare se il produttore del pannello di controllo (CPV) sta lavorando per implementare la soluzione? 

Per i partner che usano una soluzione CPV (Control Panel Vendor) per eseguire transazioni nel programma Cloud Solution Provider (CSP), è responsabilità dell'utente consultare il CPV. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Sono un CPV. Ricerca per categorie registrare? 

Per iscriversi come fornitore del pannello di controllo, attenersi alle linee guida fornite [qui](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Per ricevere il collegamento di registrazione, CPVs deve contattare [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) e fornire uno sponsor di dipendenti Microsoft che abbia una relazione di business con il CPV o conosca la loro attività. Ad esempio, un partner Development Manager (PDM).

Una volta eseguita la registrazione al centro per i partner e la registrazione delle applicazioni, sarà possibile accedere alle API del centro per i partner. Se si è un nuovo CPV, le informazioni sulla sandbox verranno ricevute tramite una notifica del centro per i partner. Dopo aver completato la registrazione come Microsoft CPV e accettato il contratto CPV, è possibile:

1. Gestire un'applicazione multi-tenant (aggiungere applicazioni per portale di Azure, registrare e annullare la registrazione delle applicazioni nel centro per i partner). Nota: CPVs deve registrare le proprie applicazioni nel centro per i partner per ottenere l'autorizzazione per le API del centro per i partner. L'aggiunta di applicazioni solo al portale di Azure non autorizza le applicazioni CPV per le API del centro per i partner.
2. Visualizzare e gestire il profilo CPV.
3. Visualizzare e gestire gli utenti che devono accedere alle funzionalità CPV. L'unico ruolo che un CPV può avere è amministratore globale.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Sto utilizzando partner Center SDK. SDK adotterà automaticamente il modello di applicazione protetta? 

No, è necessario seguire le linee guida fornite nella Guida al [modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>È possibile generare un token di aggiornamento per il modello di applicazione protetta con account in cui non è abilitata l'autenticazione a più fattori?

Sì, è possibile generare un token di aggiornamento usando un account per cui non è applicato l'autenticazione a più fattori. Tuttavia, questa operazione non deve essere eseguita perché tutti i token generati con un account che non dispone di autenticazione a più fattori abilitata non potranno accedere alle risorse a causa del requisito per l'autenticazione a più fattori.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>In che modo l'applicazione deve ottenere un token di accesso se si Abilita l'autenticazione a più fattori?

È necessario seguire la guida del [modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) , che fornisce informazioni dettagliate su come eseguire questa operazione, rispettando al tempo stesso i nuovi requisiti di sicurezza. Qui è possibile trovare il [codice di esempio .NET](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e il [codice di esempio Java](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Come CPV, si crea un'applicazione Azure AD nel tenant CPV o nel tenant del partner CSP?

Il CPV dovrà creare l'applicazione Azure Active Directory nel tenant associato alla relativa registrazione come CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Sono un CSP che usa l'autenticazione solo app. È necessario apportare modifiche?

L'autenticazione solo app non ha alcun effetto perché le credenziali utente non vengono usate per richiedere un token di accesso. Se le credenziali utente vengono condivise, i fornitori del pannello di controllo (CPVs) devono adottare il [Framework del modello applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) ed eliminare eventuali credenziali partner esistenti.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Come CPV è possibile sfruttare lo stile di autenticazione solo app per ottenere i token di accesso?

No, i partner del fornitore del pannello di controllo non possono usare lo stile di autenticazione solo app per richiedere token di accesso per conto del partner. Devono implementare il modello di applicazione protetta, che usa lo stile di autenticazione utente e app.

## <a name="key-resources"></a>Risorse chiave

### <a name="how-to-get-started"></a>Operazioni preliminari

- [Requisiti di sicurezza dei partner: Guida dettagliata](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Indirizzare le domande e i commenti e suggerimenti a questo [gruppo di linee guida sulla sicurezza](https://aka.ms/MPCSecurityGuidance)per i partner.
- Partecipa all'orario e ai webinar futuri dell'ufficio partner. Per [informazioni dettagliate sulla pianificazione e sulle risorse](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance), vedere qui.

### <a name="resources-for-enabling-mfa"></a>Risorse per abilitare l'autenticazione a più fattori

- Comprendere il concetto di [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Vedere [criteri di base: Richiedere l'autenticazione a più](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) fattori per gli amministratori per informazioni dettagliate su come abilitare i criteri di base Richiedi autenticazione a più fattori per l'amministratore.
- Vedere [criteri di base: Protezione](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) dell'utente finale per informazioni dettagliate su come abilitare i criteri di base per la protezione degli utenti finali.

### <a name="resources-for-adopting-secure-application-model"></a>Risorse per l'adozione di un modello di applicazione sicuro

- [Panoramica del modello di applicazione protetta](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: Guida al modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner nel programma CSP: codice di esempio .NET per l'abilitazione del modello applicativo sicuro](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Partner nel programma CSP: Codice di esempio Java per l'abilitazione del modello di applicazione protetto](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento di autenticazione del centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento dell'autenticazione a più fattori di PowerShell per il centro per i partner](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Supporto

### <a name="where-can-i-ask-get-support"></a>Dove è possibile richiedere supporto?

Inoltre, per supportare l'utilizzo delle risorse per soddisfare i requisiti di sicurezza, se si dispone del supporto avanzato per i partner (ASfP), contattare il responsabile dell'account del servizio; per il contratto supporto tecnico Premier for Partners (PSfP), contattare il responsabile dell'account del servizio e Technical Account Manager.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Come è possibile ottenere assistenza per l'abilitazione dei criteri di base?

- I partner possono sfruttare le ore consultive dei vantaggi MPN per ottenere indicazioni più dettagliate su come implementare i requisiti di sicurezza.
- Le opzioni di supporto tecnico per i prodotti Azure Active Directory sono disponibili tramite i vantaggi MPN. I partner con accesso a un contratto ASfP o PSfP attivo possono collaborare con l'account Manager associato (SAM/TAM) per comprendere meglio le opzioni disponibili.
- È possibile accedere al supporto per l'implementazione dei criteri di base con partner Center tramite la [richiesta di servizio del centro](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)per i partner. Selezionare autenticazione a più fattori *& modello di applicazione protetta* come argomento.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>Ricerca per categorie ottenere informazioni tecniche per adottare un Framework del modello applicativo sicuro? 

Le opzioni di supporto tecnico per i prodotti Azure Active Directory sono disponibili tramite i vantaggi MPN. I partner con accesso a una sottoscrizione ASfP o PSfP attiva possono collaborare con l'account Manager associato (SAM/TAM) per comprendere meglio le opzioni disponibili.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Dove è possibile reperire altre informazioni sui problemi comuni tecnici? 

Informazioni sui problemi comuni tecnici sono disponibili [qui](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
