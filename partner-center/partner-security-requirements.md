---
title: Requisiti di sicurezza dei partner | Centro per i partner
ms.topic: article
ms.date: 07/18/2019
description: Informazioni sui requisiti di sicurezza per gli Advisor e i partner che partecipano al programma Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provider di soluzioni cloud, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, multi-factor authentication, autenticazione a più fattori, modello di applicazione sicura, modello di applicazione sicura, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 0ce8a8dd5a58d1647c8d9e53dec0d0bbf7fe6592
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/18/2019
ms.locfileid: "68313929"
---
# <a name="partner-security-requirements"></a>Requisiti di sicurezza dei partner

**Si applica a**

- Tutti i partner nel programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti i fornitori del pannello di controllo
- Tutti gli Advisor

Sono tra le priorità più importanti le misure di sicurezza e la protezione della privacy. Sappiamo che la migliore difesa è la prevenzione e che siamo soliti come il nostro collegamento più debole. Questo è il motivo per cui è necessario che tutti gli utenti nell'ecosistema agiscano e garantiscano che siano disponibili protezioni di sicurezza appropriate. Per contribuire alla protezione di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli Advisor, i fornitori del pannello di controllo e i partner che partecipano al programma Cloud Solution Provider.

A partire dal 1 ° agosto 2019 tutti i partner devono applicare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account del servizio, nel tenant partner.

> [!NOTE]
> Si consiglia vivamente che tutti i partner che trasformano attraverso un cloud sovrano (21Vianet, US Government e Germania) agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, questi partner non devono soddisfare i nuovi requisiti di sicurezza a partire dall'1 agosto 2019. Microsoft fornirà ulteriori dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

I termini associati ai requisiti di sicurezza dei partner sono stati aggiunti alla [Guida del programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100). A partire dal 1 ° agosto 2019 tutti i partner che partecipano al programma Cloud Solution Provider devono essere conformi alle condizioni. In relazione agli Advisor, saranno presenti gli stessi requisiti contrattuali.

I partner che non implementano i requisiti di sicurezza obbligatori non saranno in grado di eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti sfruttando i diritti di amministratore delegato, una volta applicati tali requisiti. È in corso il processo di creazione di una data di applicazione tecnica per i requisiti e invierà una notifica ai partner della data con informazioni dettagliate.

## <a name="what-actions-do-i-need-to-take"></a>Quali azioni è necessario eseguire?

Data la natura altamente privilegiata di essere un partner, dobbiamo garantire che ogni utente abbia una richiesta di autenticazione a più fattori per ogni singola autenticazione. Questa operazione può essere eseguita in uno dei modi seguenti:

- Implementazione di Azure AD Premium e assicurare che l'autenticazione a più fattori venga applicata per ogni utente
- Implementazione dei [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementazione di una soluzione di terze parti e assicurare l'applicazione dell'autenticazione a più fattori per ogni utente

> [!IMPORTANT]
> Una volta che questi requisiti vengono applicati tecnicamente ogni singola autenticazione deve avere una richiesta di autenticazione a più fattori. Non sarà possibile usare alcuna funzionalità di accesso condizionale per evitare l'autenticazione con l'autenticazione a più fattori quando si accede ai servizi cloud commerciali Microsoft.

### <a name="considerations"></a>Considerazioni

Poiché questi requisiti si applicano a tutti gli utenti, inclusi gli account del servizio, nel tenant partner, è necessario tenere presenti diverse considerazioni per garantire una distribuzione uniforme. Queste considerazioni includono l'identificazione degli utenti in Azure AD che non possono eseguire l'autenticazione a più fattori, nonché le applicazioni e i dispositivi usati dall'organizzazione che non supportano l'autenticazione moderna.

Prima di eseguire qualsiasi azione, è consigliabile identificare gli elementi seguenti

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Si dispone di un'applicazione o di un dispositivo che non supporta l'utilizzo dell'autenticazione a più fattori durante l'autenticazione?

Quando si applica l'autenticazione legacy a più fattori, usare protocolli quali IMAP, POP3, SMTP e così via verranno bloccati perché questi protocolli non supportano l'autenticazione a più fattori. Per risolvere questa limitazione, è possibile usare una funzionalità nota come [password di app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) per assicurarsi che l'applicazione o il dispositivo possa ancora eseguire l'autenticazione. Esaminare le considerazioni per l'uso delle password di app documentate [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) per determinare se è possibile usarle nell'ambiente in uso.

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Esistono criteri che impediscono agli utenti di usare i propri dispositivi mobili durante il lavoro?

È importante identificare qualsiasi criterio aziendale che impedisce ai dipendenti di usare i dispositivi mobili mentre funziona perché influenzerà la soluzione multi-factor authentication implementata. Sono disponibili soluzioni di autenticazione a più fattori, ad esempio quella fornita tramite l'implementazione dei [criteri di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), che consentono solo l'uso di un'app di autenticazione per la verifica. Nel caso in cui l'organizzazione abbia un criterio che impedisca l'uso dei dispositivi mobili, è necessario esaminare l'acquisto [Azure ad Premium](https://azure.microsoft.com/pricing/details/active-directory/) per gli utenti interessati oppure è possibile implementare una soluzione di terze parti che fornisca la verifica più appropriata opzione.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quale automazione o integrazione si ha per sfruttare le credenziali utente per l'autenticazione?

Poiché il requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nella directory del partner, l'automazione o l'integrazione che sfrutta le credenziali utente per l'autenticazione avrà un effetto. È quindi importante identificare gli account usati in queste situazioni. Di seguito è riportato un elenco di esempi di applicazioni o servizi che devono essere considerati

- Pannello di controllo usato per il provisioning delle risorse per conto dei clienti
- Integrazione con qualsiasi piattaforma utilizzata per la fatturazione (in relazione al programma CSP) e supporto dei clienti
- Script di PowerShell che utilizzano i moduli AZ, AzureRM, Azure AD, MS online e così via

L'elenco precedente non è completo. Pertanto, è importante eseguire una valutazione completa di qualsiasi applicazione o servizio nel proprio ambiente che sfrutti le credenziali utente per l'autenticazione. Per quanto riguarda il requisito per l'autenticazione a più fattori, è necessario implementare le linee guida nel [Framework del modello applicativo sicuro](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) laddove possibile. Di seguito sono riportate risorse aggiuntive che consentono di comprendere in che modo è possibile implementare il Framework del modello applicativo sicuro

- [Esempi .NET del centro](https://github.com/microsoft/partner-center-dotnet-samples) per i partner: questo repository GitHub contiene esempi, sviluppati con .NET, che dimostreranno come implementare il Framework del modello applicazione protetta.
- [Esempi di Java](https://github.com/microsoft/partner-center-java-samples) per il centro per i partner: questo repository GitHub contiene esempi, sviluppati con Java, che dimostreranno come è possibile implementare il Framework del modello applicativo protetto.
- [Centro per i partner PowerShell-modello di applicazione sicura](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) : questo è un articolo che fornisce informazioni dettagliate su come implementare il Framework del modello di applicazione protetta usando PowerShell.
- [Community del gruppo di linee guida sulla sicurezza del centro](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) per i partner: si tratta di una community online in cui è possibile ottenere informazioni sugli eventi imminenti e porre qualsiasi domanda.

### <a name="enforcing-mfa-for-all-users"></a>Applicazione dell'autenticazione a più fattori per tutti gli utenti

Questa sezione illustra come è possibile usare i [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) per applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner. Se si prevede di usare Azure AD Premium, seguire i passaggi descritti [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Una soluzione di terze parti, compatibile con Azure AD, può essere usata per applicare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account del servizio. Per informazioni dettagliate sulla modalità di implementazione della soluzione, vedere la documentazione del fornitore.

I criteri di protezione di base sono un set di criteri predefiniti che consentono di proteggere le organizzazioni da molti attacchi comuni. Questi attacchi comuni possono includere spray, riproduzione e phishing delle password. I criteri di protezione di base sono disponibili in tutte le edizioni di Azure Active Directory. Microsoft sta rendendo disponibili i criteri di protezione di base a tutti per consentire a clienti e partner di implementare procedure di sicurezza ottimali.

I due criteri di protezione di base che devono essere abilitati sono descritti nella tabella seguente.

|**Criterio**| |
|-----|-----|
|**Richiedi autenticazione a più fattori per gli amministratori**|Se si Abilita il criterio Richiedi autenticazione a più fattori per gli amministratori, gli utenti nei ruoli di amministratore dovranno eseguire la registrazione per l'autenticazione a più fattori usando l'app Authenticator. Al termine della registrazione dell'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.|
|**Protezione dell'utente finale**|La protezione degli utenti finali è un criterio di protezione dell'autenticazione a più fattori basato sul rischio che protegge tutti gli utenti di una directory. Per abilitare questo criterio è necessario che tutti gli utenti eseguano la registrazione per l'autenticazione a più fattori usando l'app Authenticator Gli utenti possono ignorare la richiesta di registrazione dell'autenticazione a più fattori per 14 giorni, dopo i quali verrà impedito l'accesso fino alla registrazione per l'autenticazione a più fattori. Una volta registrati per l'autenticazione a più fattori, agli utenti verrà richiesto di eseguire l'autenticazione a più fattori solo durante i tentativi di accesso rischioso. Gli account utente compromessi vengono bloccati finché la password non viene reimpostata e gli eventi di rischio sono stati rilasciati.|

Quando questi criteri sono abilitati, ogni utente sarà in grado di usare l'autenticazione a più fattori di Azure con l'app Authenticator per la verifica senza costi aggiuntivi.

#### <a name="configure-self-service-password-reset"></a>Configurare la reimpostazione della password self-service

La reimpostazione della password self-service (SSPR) è una funzionalità Azure Active Directory che consente agli utenti di reimpostare le password senza dover contattare il team di supporto. Prima di usare il servizio, gli utenti devono registrarsi per la reimpostazione della password self-service o essere registrati. Durante la registrazione, l'utente sceglie uno o più metodi di autenticazione abilitati dall'organizzazione.

Quando il criterio di protezione della linea di base per la [protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) è abilitato, gli account utente compromessi vengono bloccati finché la password non viene reimpostata e gli eventi di rischio sono stati rilasciati. Considerato questo, è consigliabile che ogni utente, che è un amministratore globale, esegua le operazioni seguenti per eseguire la registrazione per SSPR, in modo che non vengano bloccati.

1. Passare alla [pagina di installazione di SSPR](https://aka.ms/ssprsetup)
2. Immettere il nome utente e la password
3. Configurare almeno una delle opzioni di verifica che verranno usate per verificare chi si sta reimpostando la password.  

Quando un account è stato compromesso, un amministratore deve intervenire per ripristinare l'accesso per l'utente interessato. Per informazioni dettagliate sul processo di sblocco dell'utente, vedere la [procedura per sbloccare un utente](#recovering-compromised-accounts) .

#### <a name="require-mfa-for-admins"></a>Richiedi autenticazione a più fattori per gli amministratori

Per i criteri di base Richiedi autenticazione a più fattori *per gli amministratori* è necessaria l'autenticazione a più fattori per i ruoli della directory seguenti, considerati come i ruoli Azure Active Directory più privilegiati:

- Amministratore globale
- Amministratore di SharePoint
- Amministratore di Exchange
- Amministratore di accesso condizionale
- Amministratore della sicurezza
- Amministratore helpdesk/amministratore password
- Amministratore fatturazione
- Amministratore utenti

Quando si Abilita il criterio Richiedi autenticazione a più fattori per gli amministratori, verranno richiesti i nove ruoli di amministratore precedenti per la registrazione per l'autenticazione a più fattori tramite l'app Authenticator. Una volta completata la registrazione dell'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.

Se l'organizzazione dispone di questi account in uso negli script o nel codice, è consigliabile sostituirli con [identità gestite](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Per abilitare questo criterio e proteggere gli amministratori:

1. Accedere al **portale di Azure** come amministratore globale, amministratore della sicurezza o amministratore dell'accesso condizionale.
2. Passare a **Azure Active Directory** > **accesso condizionale**.
3. Nell'elenco dei criteri selezionare **criteri di base: Richiedere l'autenticazione a più**fattori per gli amministratori.
4. Impostare **Abilita criterio** per **usare immediatamente i criteri**.
5. Fare clic su **Salva**.

> [!WARNING]
> Prima di abilitare questo criterio, verificare che gli utenti non utilizzino protocolli di autenticazione legacy. Tramite l'implementazione di questa autenticazione legacy del criterio verrà bloccato.

> [!IMPORTANT]
> Si è verificato un problema noto che influisca sulla possibilità di connettersi a Exchange Online PowerShell usando i privilegi amministrativi delegati. Vedere il problema noto di [Exchange Online PowerShell](#exchange-online-powershell) prima di abilitare questo criterio se si usa questo modulo di PowerShell.

#### <a name="end-user-protection"></a>Protezione dell'utente finale

I criteri di base per la protezione dell'utente finale proteggono tutti gli utenti di una directory. Per abilitare questo criterio, tutti gli utenti possono registrarsi per l'autenticazione a più fattori di Azure entro 14 giorni. Una volta effettuata la registrazione, agli utenti verrà richiesto di eseguire l'autenticazione a più fattori solo durante i tentativi di accesso rischioso. Gli account utente compromessi vengono bloccati fino alla reimpostazione della password e al rischio.

Criteri di **base dei criteri: La protezione** dell'utente finale è preconfigurata e verrà visualizzata nella parte superiore quando si passa al pannello accesso condizionale in portale di Azure.

Per abilitare questo criterio e proteggere gli utenti:

1. Accedere al **portale di Azure** come amministratore globale, amministratore della sicurezza o amministratore dell'accesso condizionale.
2. Passare a **Azure Active Directory** > **accesso condizionale**.
3. Nell'elenco dei criteri selezionare **criteri di base: Protezione dell'utente finale (anteprima**).
4. Impostare **Abilita criterio** per **usare immediatamente i criteri**.
5. Fare clic su **Salva**.

> [!WARNING]
> Prima di abilitare questo criterio, verificare che gli utenti non utilizzino protocolli di autenticazione legacy. Tramite l'implementazione di questa autenticazione legacy del criterio verrà bloccato.

> [!IMPORTANT]
> Si sono verificati problemi noti che influiscano sulla possibilità di connettersi a Exchange Online PowerShell usando privilegi amministrativi delegati. Vedere il problema noto di [Exchange Online PowerShell](#exchange-online-powershell) prima di abilitare questo criterio se si usa questo modulo di PowerShell.

## <a name="common-issues"></a>Problemi comuni

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Dopo aver abilitato i criteri di base, è possibile che l'automazione o l'integrazione stia riscontrando un'eccezione simile alla seguente:

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Il motivo di questa eccezione è che si esegue l'autenticazione usando le credenziali utente ed è ora necessaria l'autenticazione a più fattori. Per risolvere questa eccezione, sarà necessario usare un token di accesso per l'autenticazione. Per ulteriori informazioni, vedere la [Guida del modello di applicazione protetta](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) .

>[!IMPORTANT]
>La maggior parte delle API moderne e dei moduli di PowerShell supporta la possibilità di usare un token di accesso per l'autenticazione. Tuttavia, esistono alcuni che attualmente non supportano questa funzionalità. Se è necessario contribuire a determinare se l'API o il modulo di PowerShell che si sta tentando di utilizzare supporta l'utilizzo di un token di accesso per l'autenticazione, pubblicare un messaggio nella community del [gruppo di linee guida sulla sicurezza del centro](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) per i partner.

#### <a name="aadsts700082"></a>AADSTS700082

Una volta implementato il Framework del modello applicazione protetta, è possibile che venga visualizzata l'eccezione seguente 90 giorni dopo la generazione del token di aggiornamento iniziale.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Per quanto riguarda Azure Active Directory la durata massima di un token di aggiornamento è di 90 giorni. Per risolvere questo errore, è necessario generare e archiviare in modo sicuro un nuovo token di aggiornamento. Si noti che è possibile aggiornare il token di aggiornamento a livello di codice perché, a ogni richiesta Azure Active Directory per un token di accesso, viene restituito un nuovo token di aggiornamento. È possibile implementare la logica appropriata per aggiornare il token di aggiornamento archiviato in modo sicuro prima della scadenza.

Per ulteriori informazioni, vedere la [durata dei token configurabile in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) .

### <a name="recovering-compromised-accounts"></a>Ripristino di account compromessi

Per garantire la protezione dei clienti, il servizio di credenziali perse trova le coppie nome utente/password disponibili pubblicamente. Se corrispondono a uno degli utenti, Microsoft contribuisce a proteggere immediatamente l'account. Gli utenti identificati con una credenziale persa vengono confermati compromessi. A questi utenti verrà impedito l'accesso fino alla reimpostazione della password.

Gli utenti assegnati a una licenza Azure AD Premium possono ripristinare l'accesso tramite la reimpostazione della password self-service (SSPR) se la funzionalità è abilitata nella propria directory. Gli utenti senza una licenza Premium che viene bloccata devono contattare un amministratore per eseguire una reimpostazione manuale della password e ignorare l'evento di rischio utente contrassegnato.

#### <a name="steps-to-unblock-a-user"></a>Passaggi per sbloccare un utente

Verificare che l'utente sia stato bloccato dal criterio esaminando i log di accesso dell'utente.

1. Un amministratore deve accedere al **portale di Azure** e passare a **Azure Active Directory** > **utenti** > fare clic sul nome dell'utente e passare ad accessi.
2. Per avviare la reimpostazione della password per un utente bloccato, un amministratore deve passare a **Azure Active Directory** > **utenti contrassegnati per il rischio**
3. Fare clic sull'utente il cui account è bloccato per visualizzare le informazioni sull'attività di accesso recente dell'utente.
4. Fare clic su Reimposta password per assegnare una password temporanea che deve essere modificata al successivo accesso.
5. Fare clic su Ignora tutti gli eventi per reimpostare il Punteggio di rischio dell'utente.

L'utente può ora accedere, reimpostare la password e accedere all'applicazione.

## <a name="known-issues"></a>Problemi noti

### <a name="exchange-online-powershell"></a>PowerShell per Exchange Online

Quando l'autenticazione a più fattori è abilitata, i partner non saranno in grado di usare i propri privilegi amministrativi delegati con Exchange Online PowerShell per eseguire azioni contro i clienti. Per altre informazioni su questa limitazione, vedere [connettersi a Exchange Online PowerShell usando l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) .

## <a name="resources-and-support"></a>Risorse e supporto

Attraverso la [community del gruppo di linee guida per la sicurezza di partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) è possibile trovare risorse aggiuntive e ottenere informazioni sugli eventi imminenti, ad esempio le ore di ufficio tecnico. Per ulteriori informazioni sui requisiti, vedere il documento [domande frequenti](http://assetsprod.microsoft.com/security-requirements-faq.pdf) .
