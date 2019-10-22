---
title: Domande frequenti sui requisiti di sicurezza per i partner | Centro per i partner
ms.topic: article
ms.date: 09/27/2019
description: Domande frequenti sui requisiti di sicurezza per i partner
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.openlocfilehash: e9471ae8dd0e478540e30a879d010ffb0c1f1bc0
ms.sourcegitcommit: c388fae97437b727edeb0de3712bd2822010ecd6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/30/2019
ms.locfileid: "71678298"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Domande frequenti sui requisiti di sicurezza per i partner

Questo articolo contiene alcune domande frequenti sui [requisiti di sicurezza per i partner](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisiti di sicurezza per i partner

### <a name="what-are-the-new-partner-security-requirements"></a>Quali sono i nuovi requisiti di sicurezza per i partner?

Per la protezione dei partner Microsoft e dei rispettivi clienti, è opportuno che i partner intraprendano immediatamente le azioni seguenti:  

1. **Abilitare Multi-Factor Authentication (MFA) per tutti gli utenti inclusi nei tenant dei partner**. Tutti gli utenti inclusi nei tenant dei partner devono usare Multi-Factor Authentication (MFA) per accedere ai servizi cloud commerciali Microsoft o per eseguire transazioni in CSP tramite API o il Centro per i partner. Con l'abilitazione dei criteri di protezione di base, MFA è disponibile gratuitamente per tutti gli utenti inclusi nei tenant dei partner.

2. **Adottare il framework del modello di applicazione sicura**. Tutti i partner che eseguono l'integrazione usando un'API Microsoft, quale Azure Resource Manager, Microsoft Graph o l'API del Centro per i partner, devono adottare il framework del modello di applicazione sicura per evitare problemi di integrazione quando sono abilitati i criteri di base.

L'abilitazione di Multi-Factor Authentication e l'adozione del framework del modello di applicazione sicura consentono infatti di proteggere l'infrastruttura e salvaguardare i dati dei clienti da potenziali rischi per la sicurezza, come l'identificazione di un furto o di altri eventi illeciti.  

### <a name="which-partners-need-to-meet-the-requirements"></a>Quali partner devono soddisfare i requisiti?

Questi requisiti devono essere soddisfatti dai gruppi di partner seguenti:

- Tutte le organizzazioni partner che partecipano al programma Cloud Solution Provider (CSP) ed effettuano le transazioni usando i servizi cloud commerciali Microsoft
  - Partner con fatturazione diretta
  - Provider indiretti
  - Rivenditori indiretti
- Tutti i fornitori del pannello di controllo
- Tutti i partner del programma Advisor  

Tutti i partner che effettuano le transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) non sono più tenuti a soddisfare i nuovi requisiti di sicurezza a partire dal 1° agosto. Ciononostante, è fortemente consigliabile che tutti i partner che usano un cloud sovrano agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

### <a name="what-are-the-key-timelines-and-milestones"></a>Quali sono le tempistiche e le attività cardine?

Le condizioni associate a questi requisiti di sicurezza verranno immediatamente aggiunte alla [Guida al programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100). Questi requisiti di sicurezza devono essere stati implementati a partire dal 1° agosto 2019 conformemente alla partecipazione del partner al programma CSP.

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>Cosa succede se non intraprendo alcuna azione?

I partner che non soddisfano questi obblighi e requisiti di sicurezza non potranno effettuare transazioni nell'ambito del programma Cloud Solution Provider o gestire i tenant dei clienti usando diritti di amministratore delegato quando vengono applicati questi requisiti. È in corso il processo di identificazione di una data di applicazione per i requisiti. I partner riceveranno una notifica con tale data e informazioni dettagliate.

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>Cosa succede se l'autenticazione MFA non è stata implementata entro il 1° agosto 2019, come definito dai nuovi requisiti per la sicurezza?

Dal 1° agosto 2019 sono entrate in vigore le condizioni associate a questi requisiti di sicurezza nella [Guida al programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100). Per rispettare queste condizioni e proteggere la propria azienda, tutti i partner che partecipano al programma CSP devono quindi soddisfare i requisiti. I partner che non rispettano queste procedure di sicurezza possono perdere la facoltà di effettuare transazioni nel programma CSP o gestire i tenant dei clienti sfruttando i diritti di amministratore delegato dal momento in cui viene eseguita l'applicazione tecnica dei requisiti di sicurezza per i partner. Viene stabilita una data di applicazione di cui vengono tempestivamente informati i partner.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Perché Microsoft applica questi nuovi requisiti?

Sicurezza e privacy di clienti e partner costituiscono la principale priorità di Microsoft. Continuano infatti a perpetrarsi attacchi alla sicurezza sempre più sofisticati, principalmente correlati a eventi imprevisti di compromissione dell'identità. Poiché i controlli preventivi svolgono un ruolo fondamentale in una strategia di difesa complessiva volta a contrastare gli attacchi alla sicurezza, per contribuire alla protezione di partner e clienti si inizierà ad applicare un set di requisiti di sicurezza obbligatori.

### <a name="does-this-apply-to-all-geographies"></a>Queste informazioni sono valide per tutte le aree geografiche?

Sì, queste informazioni fanno riferimento a tutte le aree geografiche? È fortemente consigliabile che tutti i partner che effettuino transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, non è necessario che questi partner soddisfino i nuovi requisiti di sicurezza con decorrenza a partire dal 1° agosto. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>È possibile ottenere un'esclusione per un account?

No, non è possibile escludere alcun account dal requisito di applicazione dell'autenticazione MFA. Considerati i privilegi elevati della condizione di partner, la [Guida al programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100) prevede che l'autenticazione MFA venga applicata a tutti gli account presenti nel tenant del partner.

## <a name="required-actions"></a>Azioni richieste

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Quali sono le azioni chiave che è necessario intraprendere per soddisfare i requisiti?

Tutti i partner del programma CSP (partner con fatturazione diretta, provider indiretto e rivenditore indiretto), gli Advisor e i fornitori di pannelli di controllo devono soddisfare i requisiti.

1. **Applicazione di MFA a tutti gli utenti**

    Tutti i partner del programma CSP, gli Advisor e i fornitori di pannelli di controllo devono applicare l'autenticazione MFA a tutti gli utenti inclusi nel tenant del partner. Questa operazione può essere eseguita abilitando il criterio [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), i [criteri di base per la protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) ed eventuali altri criteri di base futuri. I vantaggi offerti dai criteri di base continueranno a evolversi per garantire che partner e clienti siano sempre protetti dalle minacce alla sicurezza in continua evoluzione. Per altre informazioni, consultare la [documentazione sui criteri di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    - Vedere [Criteri di base: Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) per informazioni dettagliate su come abilitare i criteri di base relativi alla richiesta di MFA per gli amministratori.
    - Vedere [Criteri di base: Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) per informazioni dettagliate su come abilitare i criteri di base per la protezione degli utenti finali.
    - Comprendere il concetto di [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Considerazioni aggiuntive:

    - I provider indiretti devono collaborare con rivenditori indiretti per poter eseguire l'onboarding nel Centro per i partner, qualora non lo abbiano già fatto, e incoraggiare i rivenditori a soddisfare i requisiti.
    - Azure MFA viene resa disponibile gratuitamente a tutti gli utenti inclusi nel tenant del partner tramite i criteri di base con l'[app Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) come unico metodo di verifica.
    - Se sono necessari altri metodi di verifica, ad esempio una telefonata o un SMS, è possibile ricorrere a metodi aggiuntivi tramite le SKU [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium).
    - Quando accedono ai servizi cloud commerciali Microsoft, i partner possono usare anche una soluzione MFA di terze parti per ogni account.

2. **Adottare il framework del modello di applicazione sicura**

    Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un errore correlato alla distribuzione della soluzione MFA. Le risorse seguenti offrono una panoramica e preziose indicazioni su come adottare il modello.

    - [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro per i partner: guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Se si usa un pannello di controllo, è necessario consultarsi con il fornitore in merito all'adozione del framework del modello di applicazione sicura.

    I fornitori di pannelli di controllo devono infatti eseguire l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro per i partner come fornitore di pannelli di controllo e avviare subito l'implementazione di questo requisito. Vedere [Centro per i partner: framework del modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). I fornitori di pannelli di controllo devono accettare e usare il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Che cos'è la Multi-Factor Authentication (MFA)?

MFA è un meccanismo di sicurezza che consente agli utenti di eseguire l'autenticazione tramite più di una procedura di sicurezza e convalida. In particolare, richiede due o più dei seguenti metodi di verifica:

- Un elemento noto, in genere una password
- Un oggetto fisico (un dispositivo attendibile non facilmente duplicabile, come un telefono)
- Una caratteristica personale (biometria)

### <a name="what-are-baseline-protection-policies"></a>Cosa sono i criteri di protezione di base?

I [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (attualmente in anteprima) sono un set di criteri predefiniti che consentono di proteggere le organizzazioni da molti attacchi comuni. Questi attacchi comuni possono includere password spraying, riproduzione e phishing. I criteri di protezione di base sono disponibili in tutte le edizioni di Azure Active Directory. A seguito dell'aumento degli attacchi basati sull'identità registrato negli ultimi anni, Microsoft li renderà presto disponibili a tutti gli utenti. Questi criteri sono stati sviluppati al fine di garantire che tutte le organizzazioni dispongano di un livello di sicurezza di base senza costi aggiuntivi.

> [!NOTE]
> I criteri di base Microsoft e le funzionalità correlate continueranno a evolversi per proteggere meglio partner e clienti dalle minacce alla sicurezza in continua evoluzione. È possibile anche che ai criteri di base vengano apportate alcune modifiche a livello di denominazione e tassonomia. Per consultare le informazioni più recenti, si consiglia di visitare direttamente le pagine dei criteri di base.

### <a name="what-baseline-policies-must-i-enable"></a>Quali criteri di base è necessario abilitare?

Se prevedi di usare i criteri di protezione di base correnti per fornire l'autenticazione MFA per ogni account incluso nel tenant del partner, devi abilitare i criteri di base [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). Questi criteri di protezione di base consentiranno di soddisfare gratuitamente il requisito relativo all'autenticazione MFA solo agli utenti inclusi nel tenant del partner che usano app Microsoft Authenticator tramite dispositivo mobile.

I [criteri di base Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) vengono usati per gli utenti amministratori nella directory dei partner, mentre i criteri di base [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) vengono applicati per proteggere gli utenti non amministratori nel tenant del partner. Per abilitare questi criteri, gli utenti dovranno effettuare la registrazione all'autenticazione MFA. Dopo aver effettuato la registrazione, verrà loro richiesta l'autenticazione MFA durante le procedure di accesso, in base a quanto definito dai singoli criteri. I vantaggi offerti dai criteri di base continueranno a evolversi per garantire che partner e clienti siano sempre protetti dalle minacce alla sicurezza in continua evoluzione. Per altre informazioni, consultare la [documentazione sui criteri di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Come è possibile abilitare i criteri Richiedi la MFA per gli amministratori?

I criteri di base Richiedi la MFA per gli amministratori possono essere abilitati tramite il portale di gestione di Azure. Vedere [Criteri di base: Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) per informazioni dettagliate su come abilitare i criteri di base.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Come è possibile abilitare i criteri Protezione dell'utente finale?

I criteri di base Protezione degli utenti finali possono essere abilitati tramite il portale di gestione di Azure. Vedere [Criteri di base: Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) per informazioni dettagliate su come abilitare questi criteri di base.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>I criteri di base verranno abilitati automaticamente?

No, per abilitare questi criteri, un utente membro del ruolo amministratore globale, amministratore della sicurezza o amministratore dell'accesso condizionale dovrà configurare i criteri su Usa i criteri immediatamente.

### <a name="what-is-the-cost-of-enabling-mfa"></a>Quanto costa abilitare l'autenticazione MFA?

Microsoft offre l'autenticazione MFA gratuitamente tramite l'implementazione dei criteri di base [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). L'unica opzione di verifica disponibile tramite questa versione di MFA è l'[app Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se si preferisce usare una telefonata o un SMS come opzione di verifica, sarà necessario acquistare una licenza di [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). In alternativa, è possibile usare una soluzione di terze parti per fornire l'autenticazione MFA a ogni utente incluso nel tenant del partner. In questo caso, è responsabilità del partner accertarsi che la soluzione MFA venga applicata e che siano rispettati tutti i requisiti.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Se si dispone già di una soluzione MFA, quali azioni è necessario eseguire?

Attraverso questi requisiti di sicurezza, agli utenti inclusi nel tenant di un partner sarà richiesto di eseguire l'autenticazione MFA quando accedono ai servizi cloud commerciali Microsoft. Per soddisfare questi requisiti, è possibile usare anche una soluzione di terze parti. Microsoft non fornisce più test di convalida ai provider di identità indipendenti per la compatibilità con Azure Active Directory. Se si vuole testare l'interoperabilità di un prodotto, consultare le [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Se usi una soluzione di terze parti, è importante verificare che rilasci l'attestazione con il riferimento al metodo di autenticazione (Authentication Method Reference, AMR) contenente il valore MFA. Per informazioni dettagliate su come verificare che la soluzione di terze parti rilasci l'attestazione prevista, vedi [Test dei requisiti di sicurezza per i partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>Quale metodo di verifica è possibile usare per eseguire l'autenticazione MFA?

Microsoft offre l'autenticazione MFA gratuitamente tramite l'implementazione dei criteri di base [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users). L'unica opzione di verifica disponibile tramite questa versione di MFA è l'[app Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Se si preferisce usare una telefonata o un SMS come opzione di verifica, sarà necessario acquistare una licenza di [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). In alternativa, è possibile usare una soluzione di terze parti per fornire l'autenticazione MFA a ogni utente incluso nel tenant del partner. In questo caso, è responsabilità del partner accertarsi che la soluzione MFA venga applicata e che siano rispettati tutti i requisiti.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Se vengono usati più tenant di partner per eseguire la transazione, e necessario implementare l'autenticazione MFA su tutti i tenant?

Sì, sarà necessario applicare l'autenticazione MFA a tutti i tenant di Azure Active Directory associati al programma CSP o al programma Advisor. Se si prevede di acquistare una licenza di Azure Active Directory Premium, sarà necessario acquistare una licenza per l'utente in ogni tenant di Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>È necessario che l'autenticazione MFA venga applicata a ogni utente incluso nel tenant del partner?*

I criteri di protezione di base [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) applicheranno l'autenticazione MFA a ogni utente incluso nel tenant del partner. Se si ricorre a questi criteri per fornire l'autenticazione MFA e si usa l'applicazione [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview), non sarà quindi necessario acquistare licenze aggiuntive. In caso contrario, sarà necessario acquistare una soluzione appropriata per fornire l'autenticazione MFA a ogni utente incluso nel tenant del partner.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Sono un partner con fatturazione diretta con Microsoft. Come devo procedere?

I partner Cloud Solution Provider con fatturazione diretta devono applicare l'autenticazione MFA per ogni utente incluso nel tenant del partner.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Sono un rivenditore indiretto ed eseguo le transazioni solo tramite un distributore. Devo comunque effettuare questa procedura?

Tutti i rivenditori indiretti sono tenuti ad applicare l'autenticazione MFA per ogni utente incluso nel tenant del partner. Questa azione deve essere eseguita dal rivenditore indiretto.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Se non viene usata l'API del Centro per i partner, è comunque necessario implementare l'autenticazione MFA?

Sì, questo requisito di sicurezza è valido per tutti gli utenti, inclusi gli utenti amministratori del partner e gli utenti finali inclusi in un tenant del partner.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Quali fornitori di terze parti offrono soluzioni MFA compatibili con Azure Active Directory?

Sono disponibili molte recensioni indipendenti di soluzioni MFA online, ad esempio [Gartner](https://www.gartner.com/en/webinars/3881781). Quando valutano fornitori e soluzioni MFA, i partner devono accertarsi che la soluzione scelta sia compatibile con Azure Active Directory.

Microsoft non fornisce più test di convalida ai provider di identità indipendenti per la compatibilità con Azure Active Directory. Se si vuole testare l'interoperabilità di un prodotto, consultare le [linee guida](https://www.microsoft.com/download/details.aspx?id=56843).

Per altre informazioni, vedere l'[Elenco di compatibilità della federazione di Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Come è possibile testare l'autenticazione MFA in una sandbox di integrazione?

I criteri di protezione di base [Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) dovrebbero essere già abilitati per il tenant della sandbox di integrazione. Tramite questi criteri, a ogni utente del tenant sarà richiesto di eseguire l'autenticazione tramite una soluzione MFA.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>L'abilitazione dell'autenticazione MFA influirà sulle modalità di interazione con il tenant dei clienti?

No. L'applicazione di questi requisiti di sicurezza non avrà alcun effetto sulle modalità di gestione dei clienti. Non verrà ad esempio annullata la possibilità di eseguire operazioni amministrative delegate.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Anche i clienti devono soddisfare i requisiti di sicurezza dei partner?

No, non è necessario applicare l'autenticazione MFA anche agli utenti inclusi nei tenant Azure AD dei clienti. Si consiglia tuttavia di collaborare con ogni cliente per determinare le procedure migliori per proteggere i rispettivi utenti.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>È possibile usare password di app con i criteri di protezione di base?

Sì, è possibile usare [password di app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords). Esaminare le considerazioni per l'uso delle password di app [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) documentate per determinare se sono supportate per l'uso desiderato.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>È possibile escludere un utente da questi requisiti?

No, l'autenticazione MFA è prevista per tutti gli utenti inclusi nel tenant del partner, inclusi gli account di servizio.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>I requisiti di sicurezza dei partner vengono applicati anche alla sandbox di integrazione?

Sì, i requisiti di sicurezza dei partner vengono applicati anche alla sandbox di integrazione. Questo significa che sarà necessario implementare la soluzione MFA appropriata per gli utenti inclusi nel tenant della sandbox di integrazione. È consigliabile implementare i criteri di protezione di base per fornire l'autenticazione MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Come è possibile configurare un account di accesso di emergenza (break glass)?

È consigliabile creare uno o due account di accesso di emergenza per impedire di essere inavvertitamente bloccati dal tenant di Azure AD. In merito ai requisiti di sicurezza dei partner, è necessario che ogni utente esegua l'autenticazione tramite Multi-Factor Authentication. Questo significa tuttavia che sarà necessario modificare la definizione di un account di accesso di emergenza. Potrebbe trattarsi, ad esempio, di un account che usa una soluzione di terze parti per l'autenticazione MFA.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>In che modo gli utenti guest saranno interessati dai requisiti di sicurezza dei partner?

Gli utenti guest dovranno eseguire l'autenticazione MFA quando accedono al tenant del partner. I requisiti di sicurezza dei partner non avranno invece alcuna conseguenza sugli utenti guest che accedono alle risorse nel tenant personale.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se si usa una soluzione di terze parti, è necessario Active Directory Federation Service (ADFS)?

No, se si una soluzione di terze parti, non è necessario avere Active Directory Federation Service (ADFS). Si consiglia di rivolgersi al fornitore della soluzione per determinare quali sono i requisiti per la soluzione.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>È necessario abilitare i criteri di protezione di base?

No, non è necessario abilitare i criteri di protezione di base. L'unico requisito è quello di applicare l'autenticazione MFA per ogni utente presente nel tenant del partner, inclusi gli account del servizio.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>È possibile usare l'accesso condizionale per soddisfare il requisito di autenticazione MFA?

Sì, è possibile usare l'accesso condizionale per applicare l'autenticazione MFA a ogni utente presente nel tenant del partner, inclusi gli account di servizio. Considerati i privilegi elevati della condizione di partner, è tuttavia necessario garantire che ogni utente disponga di una richiesta MFA per ogni singola autenticazione. Questo significa che non sarà possibile usare la funzionalità di accesso condizionale che elude la necessità di usare l'autenticazione MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quali opzioni di verifica vengono fornite tramite l'implementazione dei criteri di protezione di base?

Relativamente alla versione di Multi-Factor Authentication disponibile tramite l'implementazione dei criteri di protezione di base, l'unica opzione di verifica disponibile è un'app di autenticazione. Considerato meno sicuro, l'uso di una telefonata o di un SMS non è disponibile con questa versione di MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>L'account di servizio usato da Azure AD Connect sarà interessato dai requisiti di sicurezza dei partner?

No, l'account di servizio usato da Azure AD Connect non sarà interessato dai requisiti di sicurezza dei partner. Se si verifica un problema con Azure AD Connect in seguito all'applicazione dell'autenticazione MFA, aprire una richiesta di assistenza tecnica con il servizio di supporto tecnico Microsoft.

## <a name="secure-application-model"></a>Modello di applicazione sicura

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Chi deve adottare il modello di applicazione sicura per soddisfare i requisiti?

Microsoft sta introducendo un framework scalabile e sicuro per l'autenticazione dei partner Cloud Solution Provider (CSP) e dei fornitori di pannelli di controllo (CPV) che usano Multi-Factor Authentication. Per altre informazioni, vedere la [Guida del modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft.

### <a name="what-is-the-secure-application-model"></a>Che cos'è il modello di applicazione sicura?

Microsoft sta introducendo un framework scalabile e sicuro per l'autenticazione dei partner Cloud Solution Provider (CSP) e dei fornitori di pannelli di controllo (CPV) che usano Multi-Factor Authentication. Per altre informazioni, vedere la [Guida del modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>Come viene implementato il modello di applicazione sicura?

Tutti i partner che hanno sviluppato una procedura di integrazione personalizzata usando un'API (ad esempio Azure Resource Manager, Microsoft Graph, API del Centro per i partner e così via) o hanno implementato un'automazione personalizzata usando strumenti come PowerShell, dovranno adottare il [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) per eseguire l'integrazione con i servizi cloud Microsoft. In caso contrario, è possibile che si verifichi un errore correlato alla distribuzione della soluzione MFA. Le risorse seguenti offrono una panoramica e preziose indicazioni su come adottare il modello.

- [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Se si usa un pannello di controllo, è necessario consultarsi con il fornitore in merito all'adozione del framework del modello di applicazione sicura.

I fornitori di pannelli di controllo devono infatti eseguire l'[onboarding](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro per i partner come fornitore di pannelli di controllo e avviare subito l'implementazione di questo requisito. Vedere [Centro per i partner: framework del modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf). I fornitori di pannelli di controllo devono accettare e usare il consenso dei partner CSP anziché le credenziali ed eliminare tutte le credenziali dei partner CSP esistenti.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Chi sono i fornitori di pannelli di controllo (CPV)?

Un fornitore di pannelli di controllo è un fornitore di software indipendente che sviluppa app a disposizione dei partner CSP che eseguono l'integrazione con un'API del Centro per i partner. Un fornitore di pannelli di controllo non è un partner CSP con accesso diretto al dashboard o alle API del Centro per i partner. Una descrizione dettagliata è disponibile nell'articolo [Centro per i partner: Guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Il modello di applicazione sicura deve essere implementato solo per l'API/SDK del Centro per i partner?

Se sono abilitati entrambi i criteri di base *Richiedi la MFA per gli amministratori* e *Protezione dell'utente finale*, tutti gli utenti dovranno eseguire l'autenticazione MFA. Questo significa che sarà necessario implementare il modello di applicazione sicura per ogni API, interfaccia della riga di comando e modulo di PowerShell (ad esempio Azure, Azure AD, MS online, Centro per i partner e così via) che deve essere eseguito in modo non interattivo e si basa sull'uso delle credenziali utente per l'autenticazione.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Sono in uso strumenti di automazione come PowerShell. Come viene implementato il modello di applicazione sicura?

Se l'automazione è progettata per essere eseguita in modo non interattivo e si basa su credenziali utente per l'autenticazione, sarà necessario implementare il modello di applicazione sicura. Vedere [Modello di applicazione sicura | PowerShell per Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) per informazioni su come implementare questo framework.  Non tutti gli strumenti di automazione offrono la possibilità di eseguire l'autenticazione usando token di accesso. Per informazioni sulle modifiche che devono essere apportate, inviare un messaggio al gruppo [Linee guida per la sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Quali credenziali utente devono essere fornite dall'amministratore dell'applicazione durante l'esecuzione del processo di consenso?

Si consiglia di usare un account di servizio a cui sono assegnate autorizzazioni con privilegi minimi. In merito all'API del Centro per i partner, questo significa che è necessario usare un account a cui è assegnato il ruolo agente di vendita o agenti amministrativi.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Perché l'amministratore dell'applicazione non deve fornire credenziali di amministratore globale durante l'esecuzione del processo di consenso?

Per ridurre i rischi, è consigliabile usare identità con privilegi minimi e non un account con privilegi di amministratore globale, perché in questo modo verrebbero fornite più autorizzazioni di quelle richieste

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Com'è possibile per i partner CSP sapere se i rispettivi fornitori di pannelli di controllo (CPV) stanno lavorando all'implementare della soluzione?

I partner che usano una soluzione sviluppata da un fornitore di pannelli di controllo (CPV) per eseguire transazioni nel programma Cloud Solution Provider (CSP) sono tenuti a rivolgersi direttamente al fornitore.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Come può essere eseguita la registrazione dai fornitori di pannelli di controllo (CPV)?

Per registrarsi come fornitore di pannelli di controllo, attenersi alle linee guida riportate [qui](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Per ricevere il collegamento di registrazione, i fornitori di pannelli di controllo devono contattare [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) e specificare un dipendente Microsoft sponsor che abbia una relazione commerciale con il fornitore di pannelli di controllo o ne conosca il tipo di attività, ad esempio un Partner Development Manager (PDM).

Dopo aver eseguito la registrazione al Centro per i partner e aver registrato le applicazioni, sarà possibile accedere alle API del Centro per i partner. I nuovi fornitori di pannelli di controllo riceveranno invece informazioni sulla sandobox tramite una notifica del Centro per i partner. Dopo aver completato la registrazione come fornitore di pannelli di controllo Microsoft e aver accettato il contratto per CPV, è possibile:

1. Gestire un'applicazione multi-tenant (aggiungere applicazioni al portale di Azure, registrare e annullare la registrazione di applicazioni nel Centro per i partner). Nota: per ottenere l'autorizzazione per le API del Centro per i partner, i fornitori di pannelli di controllo devono registrare le proprie applicazioni nel Centro per i partner. La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner.
2. Visualizzare e gestire il profilo dei fornitori di pannelli di controllo.
3. Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo. L'unico ruolo che un fornitore di pannelli di controllo può avere è quello di amministratore globale.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Per i partner che usano il Partner Center SDK, l'SDK adotterà automaticamente il modello di applicazione sicura?

No, è necessario seguire le indicazioni fornite nella [guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>È possibile generare un token di aggiornamento per il modello di applicazione sicura con account in cui non è abilitata l'autenticazione MFA?

Sì, è possibile generare un token di aggiornamento anche con un account per il quale non è abilitata l'autenticazione MFA. Questa operazione, tuttavia, non dovrebbe essere eseguita perché tutti i token generati con un account che non usa l'autenticazione MFA non potranno accedere alle risorse a causa dei requisiti previsti per l'autenticazione MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>In che modo un'applicazione può ottenere un token di accesso se si abilita l'autenticazione MFA?

È necessario attenersi alla [guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf), che fornisce informazioni dettagliate su come eseguire questa operazione rispettando al tempo stesso i nuovi requisiti di sicurezza. È possibile trovare il codice di esempio .NET [qui](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) e il codice di esempio Java [qui](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>I fornitori di pannelli di controllo devono creare un'applicazione Azure AD nel tenant del CPV o nel tenant del partner CSP?

I fornitori di pannelli di controllo dovranno creare l'applicazione Azure Active Directory nel tenant associato alla rispettiva registrazione come fornitore di pannello di controllo.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>I partner CSP che usano l'autenticazione solo tramite app devono apportare modifiche?

L'autenticazione solo tramite app non è interessata perché le credenziali utente non vengono usate per richiedere un token di accesso. Se le credenziali utente vengono condivise, i fornitori di pannelli di controllo devono adottare il [framework del modello applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) ed eliminare eventuali credenziali di partner esistenti.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>I fornitori di pannelli di controllo possono sfruttare il metodo di autenticazione solo tramite app per ottenere i token di accesso?

No, i partner fornitori di pannelli di controllo non possono usare il metodo di autenticazione solo tramite app per richiedere token di accesso per conto del partner. Devono invece implementare il modello di applicazione sicura, che usa il metodo di autenticazione app + utente.

## <a name="enforcement"></a>Imposizione

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Uso una soluzione MFA di terze parti e vengo bloccato. Cosa devo fare?

Per verificare che l'account che accede alle risorse venga testato per l'autenticazione a più fattori, viene controllata l'attestazione [Authentication Method Reference](https://tools.ietf.org/html/rfc8176) per verificare che sia elencata l'autenticazione MFA. Alcune soluzioni di terze parti non rilasciano questa attestazione o non includono il valore MFA. Se l'attestazione non è presente o il valore MFA non è elencato, non esiste alcun modo per determinare se l'account autenticato è stato testato per l'autenticazione a più fattori. Dovrai collaborare con il fornitore della soluzione di terze parti per determinare quali azioni eseguire affinché la soluzione rilasci l'attestazione Authentication Method Reference.

Se non sei certo che la soluzione di terze parti rilasci l'attestazione prevista, vedi [Test dei requisiti di sicurezza per i partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0).

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA mi impedisce di supportare i miei clienti usando Amministra per conto terzi. Come posso procedere?

L'applicazione tecnica dei requisiti di sicurezza per i partner verificherà se l'account autenticato è stato testato per l'autenticazione a più fattori. Se l'account non è stato sottoposto a questa verifica, verrai reindirizzato alla pagina di accesso e ti verrà chiesto di eseguire di nuovo l'autenticazione. Se il tuo dominio non è federato, dopo l'autenticazione ti verrà chiesto di configurare l'autenticazione a più fattori. Al termine, potrai gestire i clienti usando Amministra per conto terzi. Se invece il tuo dominio è federato, dovrai assicurarti che l'account venga testato per l'autenticazione a più fattori.

## <a name="key-resources"></a>Risorse principali

### <a name="how-to-get-started"></a>Operazioni preliminari

- [Requisiti di sicurezza per i partner: guida dettagliata](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Indirizzare eventuali domande e commenti a questo [gruppo di linee guida per la sicurezza del Centro per i partner](https://aka.ms/MPCSecurityGuidance).
- Partecipare ai prossimi webinar per i partner. Consultare le [risorse e la pianificazione dettagliata qui](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-enabling-mfa"></a>Risorse per abilitare l'autenticazione MFA

- Comprendere il concetto di [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Vedere [Criteri di base: Richiedi la MFA per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) per informazioni dettagliate su come abilitare i criteri di base relativi alla richiesta di MFA per gli amministratori.
- Vedere [Criteri di base: Protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) per informazioni dettagliate su come abilitare i criteri di base per la protezione degli utenti finali.

### <a name="resources-for-adopting-secure-application-model"></a>Risorse per l'adozione di un modello di applicazione sicura

- [Panoramica del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro per i partner: guida al modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partner aderenti al programma CSP: codice di esempio .NET per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partner aderenti al programma CSP: codice di esempio Java per l'abilitazione del modello di applicazione sicura](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento di autenticazione del Centro per i partner](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento Multi-Factor Authentication di PowerShell per il Centro per i partner](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Supporto

### <a name="where-can-i-get-support"></a>Dove è possibile richiedere il supporto tecnico?

Per le risorse di supporto a cui è possibile ricorrere per soddisfare i requisiti di sicurezza, se si dispone del supporto avanzato per i partner (ASfP), contattare il servizio Gestione account servizio; se invece si dispone del supporto tecnico Premier per i partner (PSfP), contattare il servizio Gestione account servizio o il Technical Account Manager.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>Come è possibile ottenere assistenza per l'abilitazione dei criteri di base?

- Per ottenere informazioni più dettagliate su come implementare i requisiti di sicurezza, i partner possono sfruttare le ore di consulenza previste dai vantaggi MPN.
- Le opzioni di supporto tecnico di prodotto per Azure Active Directory sono disponibili tramite i vantaggi MPN. I partner con accesso a un contratto ASfP o PSfP attivo possono collaborare con il rispettivo Account Manager (SAM/TAM) per comprendere meglio le opzioni disponibili.
- È possibile accedere al supporto per l'implementazione dei criteri di base con il Centro per i partner tramite la [richiesta di servizio del Centro per i partner](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Selezionare *MFA e modello di applicazione sicura* come argomento.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Come è possibile ottenere assistenza e informazioni tecniche per l'adozione del framework del modello di applicazione sicura?

Le opzioni di supporto tecnico di prodotto per Azure Active Directory sono disponibili tramite i vantaggi MPN. I partner con accesso a una sottoscrizione ASfP o PSfP attiva possono collaborare con il rispettivo Account Manager (SAM/TAM) per comprendere meglio le opzioni disponibili.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>Come è possibile contattare il supporto se si perde l'accesso al Centro per i partner?

Passa a [Supporto Microsoft Partner](https://partner.microsoft.com/support) e quindi scegli **Show all support options** (Mostra tutte le opzioni di supporto). Visualizzerai le opzioni disponibili per contattare il supporto per i partner Microsoft. Le opzioni includono un numero di telefono per chiamare il supporto e un'opzione per chattare con il supporto. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>Dove è possibile trovare altre informazioni sui problemi tecnici più comuni?

Informazioni sui problemi tecnici sono comuni disponibili [qui.](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)
