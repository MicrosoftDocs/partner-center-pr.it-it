---
title: Requisiti di sicurezza per i partner | Centro per i partner
ms.topic: article
ms.date: 08/05/2019
description: Informazioni sui requisiti di sicurezza per advisor e partner che partecipano al programma Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 40f5ac3e1481c0b630fc7e22e680409b1ca80926
ms.sourcegitcommit: a5d5bd83e20649e9f02d2d82d682f87bb28a0265
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/09/2019
ms.locfileid: "68912634"
---
# <a name="partner-security-requirements"></a>Requisiti di sicurezza per i partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti i fornitori del pannello di controllo
- Tutti gli advisor

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti gli utenti nell'ecosistema agiscano e si assicurino di disporre di protezioni di sicurezza appropriate. Per garantire la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori del pannello di controllo e i partner che partecipano al programma Cloud Solution Provider.

A partire dal 1° agosto 2019 tutti i partner devono applicare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account del servizio, nel tenant partner.

> [!NOTE]
> È fortemente consigliabile che tutti i partner che effettuino transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) agiscano e adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, non è necessario che questi partner soddisfino i nuovi requisiti di sicurezza con decorrenza a partire dal 1° agosto 2019. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

Le condizioni associate ai requisiti di sicurezza dei partner sono state aggiunte alla [Guida al programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100). A partire dal 1° agosto 2019 tutti i partner che partecipano al programma Cloud Solution Provider dovranno attenersi a tali condizioni. In riferimento agli advisor, saranno in vigore gli stessi requisiti contrattuali.

I partner che non implementano i requisiti di sicurezza obbligatori non potranno eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti di amministratore delegato quando verranno applicati tali requisiti. È in corso il processo di identificazione di una data di applicazione tecnica per i requisiti. I partner riceveranno una notifica con tale data e informazioni dettagliate.

## <a name="what-actions-do-i-need-to-take"></a>Azioni da eseguire.

Considerati i privilegi elevati della condizione di partner, dobbiamo garantire che ogni utente disponga di una richiesta di autenticazione a più fattori per ogni singola autenticazione. Questa operazione può essere eseguita in uno dei modi seguenti

- Implementazione di Azure AD Premium e verifica che l'autenticazione a più fattori venga applicata per ogni utente
- Implementazione dei [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementazione di una soluzione di terze parti e verifica che l'autenticazione a più fattori venga applicata per ogni utente

> [!IMPORTANT]
> Dopo aver applicato questi requisiti a livello tecnico, ogni singola autenticazione deve avere una richiesta di autenticazione a più fattori in attesa di verifica. Non sarà possibile usare alcuna funzionalità di accesso condizionale per evitare di autenticarsi tramite l'autenticazione a più fattori quando si accede ai servizi cloud commerciali Microsoft.

### <a name="considerations"></a>Considerazioni

Poiché questi requisiti si applicano a tutti gli utenti, inclusi gli account del servizio, nel tenant partner, è necessario tenere presenti diverse considerazioni per garantire una distribuzione uniforme. Queste considerazioni includono l'identificazione degli utenti in Azure AD che non possono eseguire l'autenticazione a più fattori, nonché le applicazioni e i dispositivi usati dall'organizzazione che non supportano l'autenticazione moderna.

Prima di eseguire qualsiasi azione, è consigliabile identificare gli elementi seguenti

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>Si dispone di un'applicazione o di un dispositivo che non supporta l'uso dell'autenticazione a più fattori durante l'autenticazione?

Quando si applica l'autenticazione legacy a più fattori, l'uso di protocolli, ad esempio, IMAP, POP3, SMTP e così via, sarà bloccato perché questi protocolli non supportano l'autenticazione a più fattori. Per risolvere questa limitazione, è possibile usare una funzionalità nota come [password dell'app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) per assicurarsi che l'applicazione o il dispositivo possa ancora eseguire l'autenticazione. Esaminare le considerazioni per l'uso delle password dell'app [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) documentate per determinare se è possibile usarle nell'ambiente in uso.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Sono presenti utenti che usano Office 365 fornito dalle licenze associate al tenant partner?

Prima di implementare qualsiasi soluzione, è consigliabile determinare perché la versione di Microsoft Office viene usata dagli utenti nel tenant partner. Esaminare il [piano di autenticazione a più fattori per le distribuzioni di Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) prima di intraprendere qualsiasi azione. È possibile che gli utenti riscontrino problemi di connettività con applicazioni come Outlook. Prima di applicare l'autenticazione a più fattori, è importante assicurarsi che sia in uso Outlook 2013 SP1 o versione successiva e che nell'organizzazione sia abilitata l'autenticazione moderna. Per altre informazioni, vedere [Abilitare l'autenticazione moderna in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Per abilitare l'autenticazione moderna in tutti i dispositivi che eseguono Windows, su cui è installato Microsoft Office 2013, sarà necessario creare due chiavi del registro di sistema. Vedere [Abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Se gli utenti sono stati abilitati per l'autenticazione a più fattori di Azure AD e i loro dispositivi che eseguono Office 2013 non sono abilitati per l'autenticazione moderna, dovranno usare le password dell'app in tali dispositivi. Per altre informazioni sulle password dell'app e su quando, dove e come usarle, vedere: [Password dell'app con Azure Multi-Factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Esistono criteri che impediscono agli utenti di usare i propri dispositivi mobili durante il lavoro?

È importante identificare qualsiasi criterio aziendale che impedisce ai dipendenti di usare i dispositivi mobili a lavoro perché influenzerà la soluzione di autenticazione a più fattori implementata. Sono disponibili soluzioni di autenticazione a più fattori, ad esempio quella offerta tramite l'implementazione dei [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), che consentono solo l'uso di un'app di autenticazione per la verifica. Nel caso in cui l'organizzazione disponga di un criterio che impedisce l'uso dei dispositivi mobili, è necessario prendere in considerazione una delle opzioni seguenti

- Distribuire un'applicazione TOTP (con password monouso con limiti di tempo) che può essere eseguita in un sistema sicuro
- Implementare una soluzione di terze parti che applichi l'autenticazione a più fattori per ogni utente nel tenant partner che offre l'opzione di verifica più appropriata
- Acquistare licenze [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) per gli utenti interessati

Il supporto per l'uso delle chiavi di sicurezza di FIDO si trova nella guida ai criteri di protezione di base. Dopo aver aggiunto il supporto, sarà possibile sfruttare le chiavi di sicurezza di FIDO per il secondo fattore di autenticazione. Fino a quel momento si è limitati all'uso dell'app Authenticator.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quale automazione o integrazione è disponibile per usare le credenziali utente e garantire l'autenticazione?

Poiché il requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nella directory del partner, verrà usata l'automazione o l'integrazione che sfrutta le credenziali utente per l'autenticazione. È quindi importante identificare gli account usati in queste situazioni. Di seguito è riportato un elenco di esempi di applicazioni o servizi che devono essere presi in considerazione

- Pannello di controllo usato per effettuare il provisioning delle risorse per conto dei clienti
- Integrazione con qualsiasi piattaforma usata per la fatturazione (in relazione al programma CSP) e supporto dei clienti
- Script di PowerShell che usano i moduli AZ, AzureRM, Azure AD, MS online e così via

L'elenco precedente non è completo. È quindi importante eseguire una valutazione completa di qualsiasi applicazione o servizio nel proprio ambiente che sfrutti le credenziali utente per l'autenticazione. Per quanto riguarda il requisito per l'autenticazione a più fattori, è necessario implementare le linee guida nel [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) dove possibile. Di seguito sono riportate risorse aggiuntive che consentono di comprendere in che modo è possibile implementare il framework del modello di applicazione sicura

- [Esempi .NET del Centro per i partner](https://github.com/microsoft/partner-center-dotnet-samples): questo repository GitHub contiene esempi, sviluppati con .NET, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [Esempi Java del Centro per i partner](https://github.com/microsoft/partner-center-java-samples): questo repository GitHub contiene esempi, sviluppati con Java, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [PowerShell per Centro per i partner - Modello di applicazione sicura](https://docs.microsoft.com/powershell/partnercenter/secure-app-model): si tratta di un articolo che fornisce informazioni dettagliate su come implementare il framework del modello di applicazione sicura usando PowerShell.
- [Community del gruppo per la guida alla sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): si tratta di una community online in cui è possibile ottenere informazioni sugli eventi imminenti e porre qualsiasi domanda.

### <a name="enforcing-mfa-for-all-users"></a>Applicazione dell'autenticazione a più fattori per tutti gli utenti

Questa sezione illustra come è possibile usare i [criteri di protezione di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) per applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner. Se si prevede di usare Azure AD Premium, seguire i passaggi descritti [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Una soluzione di terze parti, compatibile con Azure AD, può essere usata per applicare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account del servizio. Per informazioni dettagliate sulla modalità di implementazione della soluzione, vedere la documentazione del fornitore.

I criteri di protezione di base sono un set di criteri predefiniti che consentono di proteggere le organizzazioni da molti attacchi comuni. Questi attacchi comuni possono includere password spraying, riproduzione e phishing. I criteri di protezione di base sono disponibili in tutte le edizioni di Azure Active Directory. Microsoft sta rendendo disponibili i criteri di protezione di base a tutti per consentire a clienti e partner di implementare procedure di sicurezza ottimali.

I due criteri di protezione di base che devono essere abilitati sono descritti nella tabella seguente.

|**Criterio**| |
|-----|-----|
|**Richiedere l'autenticazione a più fattori per gli amministratori**|Se si abilita il criterio Richiedere l'autenticazione a più fattori per gli amministratori, gli utenti nei ruoli di amministratore dovranno eseguire la registrazione all'autenticazione a più fattori usando l'app Authenticator. Al termine della registrazione all'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.|
|**Protezione dell'utente finale**|La protezione dell'utente finale è un criterio di protezione di base dell'autenticazione a più fattori basato sul rischio che protegge tutti gli utenti di una directory. Per abilitare questo criterio è necessario che tutti gli utenti eseguano la registrazione all'autenticazione a più fattori usando l'app Authenticator. Gli utenti possono ignorare la richiesta di registrazione dell'autenticazione a più fattori per 14 giorni, dopo i quali verrà impedito l'accesso fino al momento di registrarsi all'autenticazione a più fattori. Al termine della registrazione all'autenticazione a più fattori, agli utenti verrà richiesto di eseguire l'autenticazione a più fattori solo durante i tentativi di accesso rischioso. Gli account utente compromessi vengono bloccati finché la password non viene reimpostata e gli eventi di rischio sono stati risolti.|

Quando questi criteri sono abilitati, ogni utente sarà in grado di usare l'autenticazione a più fattori di Azure con l'app Authenticator a scopo di verifica senza costi aggiuntivi.

#### <a name="configure-self-service-password-reset"></a>Configurare la reimpostazione della password self-service

La reimpostazione della password self-service (SSPR) è una funzionalità di Azure Active Directory che consente agli utenti di reimpostare le password senza dover contattare il team di supporto. Prima di usare il servizio, gli utenti devono essere registrati o registrarsi alla reimpostazione della password self-service. Durante la registrazione, l'utente sceglie uno o più metodi di autenticazione abilitati dall'organizzazione.

Quando il criterio di protezione di base della [protezione dell'utente finale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) è abilitato, gli account utente compromessi vengono bloccati finché la password non viene reimpostata e gli eventi di rischio sono stati risolti. Considerato questo, è consigliabile che ogni utente, che è un amministratore globale, esegua le operazioni seguenti per registrarsi alla SSPR, in modo da non venire bloccato.

1. Passare alla [pagina di installazione di SSPR](https://aka.ms/ssprsetup)
2. Immettere il nome utente e la password
3. Configurare almeno una delle opzioni di verifica che verranno usate per individuare chi sta reimpostando la password.  

Quando un account è stato compromesso, l'amministratore deve intervenire per ripristinare l'accesso all'utente interessato. Per informazioni dettagliate sul processo di sblocco dell'utente, vedere la [procedura per sbloccare un utente](#recovering-compromised-accounts).

#### <a name="require-mfa-for-admins"></a>Richiedere l'autenticazione a più fattori per gli amministratori

Per il criterio di base *Richiedere l'autenticazione a più fattori per gli amministratori* è necessaria l'autenticazione a più fattori per i ruoli della directory seguenti, considerati come i ruoli Azure Active Directory più privilegiati:

- Amministratore globale
- Amministratore di SharePoint
- Amministratori di Exchange
- Amministratore di accesso condizionale
- Amministratore della protezione
- Amministratore helpdesk/amministratore password
- Amministratore fatturazione
- Amministratore degli utenti

Se si abilita il criterio Richiedere l'autenticazione a più fattori per gli amministratori, i 9 ruoli di amministratore precedenti dovranno eseguire la registrazione all'autenticazione a più fattori usando l'app Authenticator. Al termine della registrazione all'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.

Se l'organizzazione dispone di questi account in uso negli script o nel codice, è consigliabile sostituirli con  [identità gestite](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Per abilitare questo criterio e proteggere gli amministratori:

1. Accedere al  **portale di Azure** come amministratore globale, amministratore della protezione o amministratore dell'accesso condizionale. 
2. Passare a **Accesso condizionale** di  > **Azure Active Directory**.
3. Nell'elenco dei criteri selezionare **Criteri di base: Richiedere l'autenticazione a più fattori per gli amministratori**.
4. Impostare **Abilita criterio** su **Usa i criteri immediatamente**.
5. Fare  **clic** su Salva.

> [!WARNING]
> Prima di abilitare questo criterio, verificare che gli utenti non usino protocolli di autenticazione legacy. Tramite l'implementazione di questo criterio, l'autenticazione legacy verrà bloccata.

> [!IMPORTANT]
> Si è verificato un problema noto che influisce sulla possibilità di connettersi a PowerShell per Exchange Online usando i privilegi amministrativi delegati. Vedere il problema noto di [PowerShell per Exchange Online](#exchange-online-powershell) prima di abilitare questo criterio se si usa questo modulo di PowerShell.

#### <a name="end-user-protection"></a>Protezione dell'utente finale

I criteri di base per la protezione dell'utente finale proteggono tutti gli utenti di una directory. Per abilitare questo criterio è necessario che tutti gli utenti eseguano la registrazione all'autenticazione a più fattori di Azure entro 14 giorni. Al termine della registrazione, agli utenti verrà richiesto di eseguire l'autenticazione a più fattori solo durante i tentativi di accesso rischioso. Gli account utente compromessi vengono bloccati fino alla reimpostazione della password e alla rimozione del rischio.

Il criterio di **Criteri di base: protezione dell'utente finale** è preconfigurata e verrà visualizzata nella parte superiore passando al pannello dell'Accesso condizionale nel portale di Azure.

Per abilitare questo criterio e proteggere gli utenti:

1. Accedere al  **portale di Azure** come amministratore globale, amministratore della protezione o amministratore dell'accesso condizionale. 
2. Passare a **Accesso condizionale** di  > **Azure Active Directory**.
3. Nell'elenco dei criteri selezionare **Criteri di base: protezione dell'utente finale (anteprima)** .
4. Impostare **Abilita criterio** su **Usa i criteri immediatamente**.
5. Fare  **clic** su Salva.

> [!WARNING]
> Prima di abilitare questo criterio, verificare che gli utenti non usino protocolli di autenticazione legacy. Tramite l'implementazione di questo criterio, l'autenticazione legacy verrà bloccata.

> [!IMPORTANT]
> Si è verificato un problema noto che influisce sulla possibilità di connettersi a PowerShell per Exchange Online usando i privilegi amministrativi delegati. Vedere il problema noto di [PowerShell per Exchange Online](#exchange-online-powershell) prima di abilitare questo criterio se si usa questo modulo di PowerShell.

## <a name="assessing-your-environment"></a>Valutazione dell'ambiente

Tramite uno dei requisiti di sicurezza del partner attuali, è necessario applicare l'autenticazione a più fattori per ogni utente nel tenant partner. Poiché questo requisito può essere soddisfatto tramite una serie di metodi diversi, può risultare difficile valutare se sono necessarie azioni aggiuntive. È possibile usare strumenti come i log di controllo di Azure Active Directory e [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score) per valutare se sono necessarie azioni aggiuntive per proteggere il tenant con l'autenticazione a più fattori. Microsoft sta lavorando a un'esperienza nel Centro per i partner per fornire un rapido controllo della conformità ai requisiti di autenticazione a più fattori e del modello di applicazione sicura.

Microsoft Secure Score offre visualizzazioni affidabili, l'integrazione con altri prodotti Microsoft, il confronto del punteggio con altre società, il filtraggio per categoria e molto altro ancora. Con questo strumento è possibile completare le azioni di miglioramento della protezione all'interno dell'organizzazione e tenere traccia della cronologia del punteggio. Il punteggio può inoltre riflettere il momento in cui le soluzioni di terze parti hanno risolto le azioni di miglioramento consigliate.

![Microsoft Secure Score](images/security/secure-score.png)

> [!NOTE]
> Le azioni che è possibile eseguire per migliorare Microsoft Secure Score possono richiedere fino a 24 ore per essere riflesse nel punteggio.

Microsoft Secure Score presenterà solo una rappresentazione numerica del comportamento di sicurezza. Per comprendere meglio cosa o chi esegue l'autenticazione senza che venga richiesta l'autenticazione a più fattori, è consigliabile eseguire una query sui log di controllo di Azure Active Directory. Questa operazione può essere eseguita usando il modulo [Azure PowerShell ](https://docs.microsoft.com/powershell/azure/overview) e lo script seguente. Verrà generato un report che fornisce informazioni sui tentativi di autenticazione rilevati nel giorno precedente che non sono stati verificati per l'autenticazione a più fattori.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Dopo aver eseguito lo script precedente, i dettagli saranno disponibili nel file report.csv. Conterrà un elenco di tentativi di autenticazione che si sono verificati nell'ultimo giorno in cui all'utente è stata richiesta l'autenticazione a più fattori. Sarà necessario esaminare ogni voce per determinare se questo è il comportamento previsto e agire se necessario.

![Report di valutazione](images/security/assessment-report.png)

## <a name="common-issues"></a>Problemi comuni

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Dopo aver abilitato i criteri di base, è possibile che l'automazione o l'integrazione stia riscontrando un'eccezione simile alla seguente

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Il motivo di questa eccezione è che si esegue l'autenticazione usando le credenziali utente ed è ora necessaria l'autenticazione a più fattori. Per risolvere questa eccezione, sarà necessario usare un token di accesso per l'autenticazione. Per altre informazioni, vedere la [Guida del modello di applicazione sicura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

>[!IMPORTANT]
>La maggior parte delle API e dei moduli di PowerShell moderni supporta la possibilità di usare un token di accesso per l'autenticazione. Tuttavia, ne esistono alcuni che attualmente non supportano questa funzionalità. Per determinare se l'API o il modulo di PowerShell che si sta tentando di usare supporta l'uso di un token di accesso per l'autenticazione, pubblicare un messaggio nella community del [gruppo per la guida alla sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

#### <a name="aadsts700082"></a>AADSTS700082

Dopo aver implementato il framework del modello di applicazione sicura, è possibile che venga visualizzata l'eccezione seguente 90 giorni dopo la generazione del token di aggiornamento iniziale

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Per quanto riguarda Azure Active Directory la durata massima di un token di aggiornamento è di 90 giorni. Per risolvere questo errore, è necessario generare e archiviare in modo sicuro un nuovo token di aggiornamento. Si noti che è possibile aggiornare il token di aggiornamento a livello di codice perché, a ogni richiesta a Azure Active Directory per un token di accesso, viene restituito un nuovo token di aggiornamento. È possibile implementare la logica appropriata per aggiornare il token di aggiornamento archiviato in modo sicuro prima della scadenza.

Per altre informazioni, vedere le [Durate dei token configurabile in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

### <a name="recovering-compromised-accounts"></a>Ripristino di un account compromesso

Per garantire la protezione dei clienti, il servizio di credenziali perse di Microsoft rileva le coppie nome utente/password disponibili pubblicamente. Se corrispondono a uno degli utenti, Microsoft contribuisce a proteggere immediatamente l'account. Gli utenti identificati con una credenziale persa vengono confermati come compromessi. A questi utenti verrà impedito l'accesso fino alla reimpostazione della password.

Gli utenti assegnati a una licenza Azure AD Premium possono ripristinare l'accesso tramite la reimpostazione della password self-service (SSPR) se la funzionalità è abilitata nella propria directory. Gli utenti senza una licenza Premium che viene bloccata devono contattare un amministratore per eseguire una reimpostazione manuale della password e ignorare l'evento di rischio dell'utente contrassegnato.

#### <a name="steps-to-unblock-a-user"></a>Procedura per sbloccare un utente

Verificare che l'utente sia stato bloccato dal criterio esaminando i log di accesso dell'utente.

1. Un amministratore deve accedere al **portale di Azure** e passare a **Azure Active Directory** > **Utenti** > fare clic sul nome dell'utente e passare alle informazioni di accesso.
2. Per avviare la reimpostazione della password per un utente bloccato, un amministratore deve passare a **Azure Active Directory** > **Utenti contrassegnati per il rischio**
3. Fare clic sull'utente il cui account è bloccato per visualizzare le informazioni sull'attività di accesso recente dell'utente.
4. Fare clic su Reimposta password per assegnare una password temporanea che deve essere modificata all'accesso successivo.
5. Fare clic su Ignora tutti gli eventi per reimpostare il punteggio di rischio dell'utente.

L'utente può ora accedere, reimpostare la password e accedere all'applicazione.

## <a name="known-issues"></a>Problemi noti

### <a name="exchange-online-powershell"></a>PowerShell per Exchange Online

Quando l'autenticazione a più fattori è applicata, i partner non saranno in grado di usare i propri privilegi amministrativi delegati con PowerShell per Exchange Online per eseguire azioni nei confronti dei clienti. Per altre informazioni su questa limitazione, vedere [Connettersi a PowerShell per Exchange Online usando l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).

Per ovviare a questa limitazione, è possibile creare un nuovo account e non usarlo mai per eseguire un'autenticazione interattiva. È consigliabile usare [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) per creare il nuovo account ed eseguire la configurazione iniziale. Il PowerShell seguente può essere usato per creare e configurare l'account

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

Alla successiva connessione a Exchange Online tramite PowerShell usare questo account, che funzionerà come previsto.

> [!IMPORTANT]
> Quando l'autenticazione a più fattori è applicata, i partner saranno in grado di usare in futuro i propri privilegi amministrativi delegati con PowerShell per Exchange Online per eseguire azioni nei confronti dei clienti. Fino a quel momento, è consigliabile usare questa soluzione.

## <a name="resources-and-support"></a>Risorse e supporto

Attraverso la [community del gruppo per la guida alla sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) è possibile trovare risorse aggiuntive e ottenere informazioni sugli eventi imminenti, ad esempio l'orario di apertura dell'ufficio tecnico. Per altre informazioni sui requisiti, vedere il documento sulle [domande frequenti](partner-security-requirements-faq.md).
