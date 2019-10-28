---
title: Requisiti di sicurezza per i partner | Centro per i partner
ms.topic: article
ms.date: 10/11/2019
description: Informazioni sui requisiti di sicurezza per advisor e partner che partecipano al programma Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.openlocfilehash: b09588387d3b4f0f3f726a700245999c89755199
ms.sourcegitcommit: 9dd6f1ee0ebc132442126340c9df8cf7e3e1d3ad
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/16/2019
ms.locfileid: "72425199"
---
# <a name="partner-security-requirements"></a>Requisiti di sicurezza per i partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti i fornitori del pannello di controllo
- Tutti gli advisor

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti gli utenti nell'ecosistema agiscano e si assicurino di disporre di protezioni di sicurezza appropriate. Per la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori di pannelli di controllo e i partner che partecipano al programma Cloud Solution Provider.

## <a name="overview"></a>Panoramica

Dal 1° agosto 2019 tutti i partner sono tenuti a implementare l'autenticazione a più fattori per tutti gli account utente esistenti nel tenant partner. Le condizioni associate ai requisiti di sicurezza dei partner sono state aggiunte alla [Guida al programma Cloud Solution Provider](https://go.microsoft.com/fwlink/p/?LinkId=617100). In riferimento agli advisor, saranno in vigore gli stessi requisiti contrattuali.

> [!NOTE]
> È consigliabile che tutti i partner che effettuano transazioni attraverso un cloud sovrano (21Vianet, amministrazione degli Stati Uniti e Germania) si adoperino immediatamente per adottare questi requisiti di sicurezza. I partner, tuttavia, non sono obbligati a soddisfare i requisiti di sicurezza in vigore dal 1° agosto 2019. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

I partner che non implementano i requisiti di sicurezza obbligatori non potranno eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti di amministratore delegato quando verranno applicati tali requisiti.

## <a name="actions-that-you-need-to-take"></a>Azioni da intraprendere

Per adeguarsi ai requisiti di sicurezza dei partner, è necessario implementare l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. A tal fine, è possibile procedere in uno dei modi seguenti:

- Implementazione dei criteri di protezione di base [Richiedi autenticazione a più fattori per gli amministratori ](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [Protezione dell'utente finale](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) da Azure Active Directory senza costi aggiuntivi.
- Acquisto di Azure Active Directory Premium per ogni account utente. Per altre informazioni, vedere [Pianificazione di una distribuzione di Azure Multi-Factor Authentication basata sul cloud](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).
- Uso di una soluzione di terze parti per implementare l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. Per altri dettagli utili per assicurarsi che la soluzione fornisca le informazioni previste, vedere [come verranno implementati i requisiti di sicurezza](#how-the-requirements-will-be-enforced).

### <a name="consideration"></a>Considerazione

Poiché questi requisiti si applicano a tutti gli account utente esistenti nel tenant partner, per una distribuzione senza problemi è necessario considerare diversi aspetti. È ad esempio necessario identificare gli account utente di Azure Active Directory che non possono eseguire l'autenticazione a più fattori, nonché le applicazioni e i dispositivi usati dall'organizzazione che non supportano l'autenticazione moderna.

Prima di eseguire qualsiasi azione, è consigliabile identificare gli elementi seguenti

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Si hanno applicazioni o dispositivi che non supportano l'uso dell'autenticazione moderna?

Quando si implementa l'autenticazione a più fattori, i protocolli per l'uso dell'autenticazione legacy, ad esempio IMAP, POP3, SMTP e così via, verranno bloccati perché non supportano l'autenticazione a più fattori. Per risolvere questa limitazione, è possibile usare una funzionalità nota come [password dell'app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) per assicurarsi che l'applicazione o il dispositivo possa ancora eseguire l'autenticazione. Esaminare le considerazioni per l'uso delle password dell'app [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) documentate per determinare se è possibile usarle nell'ambiente in uso.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Sono presenti utenti che usano Office 365 fornito dalle licenze associate al tenant partner?

Prima di implementare qualsiasi soluzione, è consigliabile determinare quale versione di Microsoft Office viene usata dagli utenti del tenant partner. Esaminare il [piano di autenticazione a più fattori per le distribuzioni di Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) prima di intraprendere qualsiasi azione. È possibile che gli utenti riscontrino problemi di connettività con applicazioni come Outlook. Prima di implementare l'autenticazione a più fattori, è importante assicurarsi che sia in uso Outlook 2013 SP1 o versione successiva e che nell'organizzazione sia abilitata l'autenticazione moderna. Per altre informazioni, vedere [Abilitare l'autenticazione moderna in Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Per abilitare l'autenticazione moderna in tutti i dispositivi che eseguono Windows, su cui è installato Microsoft Office 2013, sarà necessario creare due chiavi del registro di sistema. Vedere [Abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Esistono criteri che impediscono agli utenti di usare i propri dispositivi mobili durante il lavoro?

È importante identificare qualsiasi criterio aziendale che impedisca ai dipendenti di usare dispositivi mobili durante l'orario di lavoro perché questo potrà influenzare la soluzione di autenticazione a più fattori implementata. Esistono soluzioni, ad esempio quella fornita tramite l'implementazione di [criteri di protezione di base](/azure/active-directory/conditional-access/concept-baseline-protection), che consentono di eseguire la verifica solo con l'uso di un'app di autenticazione. Nel caso in cui l'organizzazione disponga di un criterio che impedisce l'uso dei dispositivi mobili, è necessario prendere in considerazione una delle opzioni seguenti

- Distribuire un'applicazione TOTP (con password monouso con limiti di tempo) che può essere eseguita in un sistema sicuro
- Implementare una soluzione di terze parti per l'autenticazione a più fattori per ogni account utente esistente nel tenant partner che offre l'opzione di verifica più appropriata
- Acquistare licenze [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) per gli utenti interessati

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>Quale automazione o integrazione è disponibile per usare le credenziali utente e garantire l'autenticazione?

Poiché il requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nella directory del partner, verrà usata l'automazione o l'integrazione che sfrutta le credenziali utente per l'autenticazione. È quindi importante identificare gli account usati in queste situazioni. Di seguito è riportato un elenco di esempi di applicazioni o servizi che devono essere presi in considerazione

- Pannello di controllo usato per effettuare il provisioning delle risorse per conto dei clienti
- Integrazione con qualsiasi piattaforma usata per la fatturazione (in relazione al programma CSP) e supporto dei clienti
- Script di PowerShell che usano i moduli AZ, AzureRM, Azure AD, MS online e così via

L'elenco precedente non è completo. È quindi importante eseguire una valutazione completa di qualsiasi applicazione o servizio nel proprio ambiente che sfrutti le credenziali utente per l'autenticazione. Per far fronte al requisito di autenticazione a più fattori, è necessario, dove possibile, implementare le indicazioni nel [framework del modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="accessing-your-environment"></a>Accesso all'ambiente

Per comprendere meglio cosa o chi esegue l'autenticazione senza che venga richiesta l'autenticazione a più fattori, è consigliabile eseguire query sui log di controllo di Azure Active Directory. Questa operazione può essere eseguita usando il modulo [Azure PowerShell ](https://docs.microsoft.com/powershell/azure/overview) e lo script seguente. Verrà generato un report che fornisce informazioni dettagliate sui tentativi di autenticazione che si sono verificati nel giorno precedente per i quali non è stata richiesta l'autenticazione a più fattori.

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

$report | Where-Object {$_.mfaRequired -eq $false -and $_.loginSucceeded -eq $true} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Dopo aver eseguito lo script precedente, i dettagli saranno disponibili nel file report.csv. Conterrà un elenco di tentativi di autenticazione che si sono verificati nell'ultimo giorno in cui all'utente è stata richiesta l'autenticazione a più fattori. Sarà necessario esaminare ogni voce per determinare se questo è il comportamento previsto e agire se necessario.

![Report di valutazione](images/security/assessment-report.png)

## <a name="how-the-requirements-will-be-enforced"></a>Come verranno implementati i requisiti

I requisiti di sicurezza dei partner verranno implementati da Azure Active Directory e, a sua volta, dal Centro per i partner, mediante il controllo della presenza dell'attestazione che stabilisce che la verifica dell'autenticazione a più fattori è stata eseguita. Se si usano i criteri di protezione di base o Azure Multi-Factor Authentication, non è necessario intraprendere altre azioni.

Quando si usa una soluzione di autenticazione a più fattori di terze parti, è possibile che l'attestazione di autenticazione a più fattori non venga rilasciata. Se l'attestazione non è presente, Azure Active Directory non sarà in grado di stabilire se la richiesta di autenticazione è stata verificata dall'autenticazione a più fattori. Per informazioni su come verificare il rilascio dell'attestazione prevista da parte della soluzione, vedere [Test dei requisiti di sicurezza per i partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements).

> [!IMPORTANT]
> Se la soluzione di terze parti non rilascia l'attestazione prevista, sarà necessario interagire con il fornitore che ha sviluppato la soluzione per individuare le azioni da intraprendere.

## <a name="resources-and-support"></a>Risorse e supporto

Di seguito sono elencate le risorse che possono fornire supporto e codice di esempio:

- [Community del gruppo per la guida alla sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): si tratta di una community online in cui è possibile ottenere informazioni sugli eventi imminenti e porre qualsiasi domanda.
- [Esempi .NET del Centro per i partner](https://github.com/microsoft/partner-center-dotnet-samples): questo repository GitHub contiene esempi, sviluppati con .NET, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [Esempi Java del Centro per i partner](https://github.com/microsoft/partner-center-java-samples): questo repository GitHub contiene esempi, sviluppati con Java, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [PowerShell per il Centro per i partner - Autenticazione a più fattori](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth): si tratta di un articolo che fornisce informazioni dettagliate su come implementare il framework del modello di applicazione sicura usando PowerShell.
