---
title: Requisiti di sicurezza dei partner
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Presenta i requisiti di sicurezza dei partner per abilitare l'autenticazione a più fattori (MFA) e adottare il framework del modello di applicazione sicura.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087060"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Requisiti di sicurezza per l'uso del Centro per i partner o delle API del Centro per i partner

**Ruoli appropriati**

- Tutti gli utenti del Centro per i partner

Questo articolo illustra i requisiti di sicurezza obbligatori per gli advisor, i fornitori di pannelli di controllo e i partner che partecipano al programma Cloud Solution Provider, nonché le opzioni di autenticazione e altri aspetti correlati alla sicurezza. Le misure di sicurezza e la protezione della privacy sono alcune delle nostre priorità principali. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti nell'ecosistema agiscano e si assicurino che vengano adottate le protezioni di sicurezza appropriate.

## <a name="mandatory-security-requirements"></a>Requisiti di sicurezza obbligatori

I partner che non implementano i requisiti di sicurezza obbligatori non saranno in grado di eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti amministrativi delegati. Inoltre, i partner che non implementano i requisiti di sicurezza possono mettere a rischio la loro partecipazione ai programmi. Le condizioni associate ai requisiti di sicurezza dei partner sono state aggiunte al Contratto Microsoft Partner. Per quanto riguarda gli advisor, saranno in vigore gli stessi requisiti contrattuali.

Per la tua protezione e quella dei tuoi clienti, è opportuno che i partner intraprendano immediatamente le azioni seguenti:  

1. **Abilitare l'autenticazione a più fattori (MFA) per tutti gli account utente inclusi nel tenant partner**. È necessario applicare l'autenticazione a più fattori per tutti gli account utente inclusi nel tenant o nei tenant partner. Agli utenti deve essere richiesta la verifica tramite autenticazione a più fattori al momento di accedere ai servizi cloud commerciali Microsoft o per eseguire transazioni in Cloud Solution Provider tramite il Centro per i partner o le API.

2. **Adottare il framework del modello di applicazione sicura**. Tutti i partner che integrano le API del Centro per i partner devono adottare il [framework del modello di applicazione sicura](/partner-center/develop/enable-secure-app-model) per qualsiasi app e applicazione del modello di autenticazione utente.

    > [!IMPORTANT]
    > È consigliabile che i partner implementino il modello di applicazione sicura per l'integrazione con un'API Microsoft come Azure Resource Manager o Microsoft Graph oppure per l'uso dell'automazione, ad esempio tramite PowerShell con credenziali utente, per evitare interruzioni quando viene imposta l'autenticazione a più fattori.

Questi requisiti di sicurezza consentiranno di proteggere l'infrastruttura e salvaguardare i dati dei clienti da potenziali rischi per la sicurezza, ad esempio con l'identificazione di furti o altri eventi illeciti.  

## <a name="implementing-multi-factor-authentication"></a>Implementazione dell'autenticazione a più fattori

Per la conformità ai requisiti di sicurezza dei partner, è necessario implementare e applicare l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. È possibile procedere in uno dei modi seguenti:

- Implementare le [impostazioni predefinite per la sicurezza di Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Per altre informazioni, vedere la [sezione successiva](#security-defaults).

- Acquistare Azure Active Directory Premium per ogni account utente. Per altre informazioni, vedere [pianificare un Azure AD multi-factor authentication la distribuzione](/azure/active-directory/authentication/howto-mfa-getstarted).

- Usare una soluzione di terze parti per applicare l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. Per assicurarsi che la soluzione fornisca le informazioni previste, vedere [come verranno implementati i requisiti di sicurezza](#how-the-requirements-are-enforced).

> [!NOTE]
> Anche se l'autenticazione a più fattori non è richiesta contrattualmente per un cloud sovrano (US Government e Germania), è consigliabile adottare questi requisiti per la sicurezza.

### <a name="security-defaults"></a>Impostazioni predefinite per la sicurezza

Una delle opzioni che possono essere scelte dai partner per implementare i requisiti di autenticazione a più fattori è l'abilitazione delle impostazioni predefinite per la sicurezza in Azure AD. Le impostazioni predefinite per la sicurezza offrono un livello di sicurezza di base senza costi aggiuntivi. Prima di abilitare le impostazioni predefinite per la sicurezza, esaminare come abilitare l'autenticazione a più fattori per l'organizzazione con Azure AD e analizzare le considerazioni chiave seguenti.

- I partner che hanno già adottato i criteri di base devono agire per passare alle impostazioni predefinite per la sicurezza.

- Le impostazioni predefinite per la sicurezza sostituiscono a livello di disponibilità generale i criteri di base di anteprima. Dopo aver abilitato le impostazioni predefinite per la sicurezza, un partner non potrà più abilitare i criteri di base.

- Con le impostazioni predefinite per la sicurezza, tutti i criteri saranno abilitati contemporaneamente.

- Per i partner che usano l'[accesso condizionale](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), le [impostazioni predefinite per la sicurezza non sono disponibili](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Al momento non viene bloccata l'autenticazione legacy. Tuttavia, poiché la maggior parte degli eventi correlati a identità compromesse proviene dal tentativo di accesso con l'autenticazione legacy, i partner sono invitati a uscire da questi protocolli meno recenti.

- L'account di sincronizzazione di Azure AD Connect è escluso dalle impostazioni predefinite per la sicurezza.

Per informazioni dettagliate, vedere [Panoramica di Azure AD multi-factor authentication per l'organizzazione](/azure/active-directory/authentication/concept-mfa-get-started) e informazioni sulle [impostazioni predefinite](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)per la sicurezza.

> [!NOTE]
> Le impostazioni predefinite per la sicurezza Azure AD sono l'evoluzione dei criteri di protezione di base semplificati. Se sono già stati abilitati i criteri di protezione di base, è consigliabile abilitare le [impostazioni predefinite per la sicurezza](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Considerazioni sull'implementazione

Poiché questi requisiti si applicano a tutti gli account utente esistenti nel tenant partner, per una distribuzione senza problemi è necessario considerare diversi aspetti. Ad esempio, identificare gli account utente in Azure AD che non possono eseguire l'autenticazione a più fattori e le applicazioni e i dispositivi dell'organizzazione che non supportano l'autenticazione moderna.

Prima di eseguire qualsiasi azione, è consigliabile completare le convalide seguenti. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Si hanno applicazioni o dispositivi che non supportano l'uso dell'autenticazione moderna?

Quando si applica l'autenticazione a più fattori, l'autenticazione legacy usa protocolli quali IMAP, POP3, SMTP e altri vengono bloccati perché non supportano l'autenticazione a più fattori. Per ovviare a questa limitazione, è possibile usare la funzionalità [password dell'app](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) per assicurarsi che l'applicazione o il dispositivo possa eseguire comunque l'autenticazione. Esaminare le [considerazioni relative all'uso delle password dell'app](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) per stabilire se è possibile usarle nell'ambiente in uso.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Sono presenti utenti di Office 365 con licenze associate al tenant partner?

Prima di implementare qualsiasi soluzione, è consigliabile determinare quali versioni di Microsoft Office utenti nel tenant partner usano. È possibile che gli utenti riscontrino problemi di connettività con applicazioni come Outlook. Prima di applicare l'autenticazione a più fattori, è importante assicurarsi che sia in uso Outlook 2013 SP1 o versione successiva e che nell'organizzazione sia abilitata l'autenticazione moderna. Per altre informazioni, vedere [Abilitare l'autenticazione moderna in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Per abilitare l'autenticazione moderna nei dispositivi che eseguono Windows e in cui è installato Microsoft Office 2013, sarà necessario creare due chiavi del Registro di sistema. Vedere [Abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Esistono criteri che impediscono agli utenti di usare i propri dispositivi mobili durante il lavoro?

È importante identificare qualsiasi criterio aziendale che impedisce ai dipendenti di usare i dispositivi mobili a lavoro perché influenzerà la soluzione di autenticazione a più fattori implementata. Esistono soluzioni, ad esempio quella fornita tramite l'implementazione delle [impostazioni predefinite per la sicurezza Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), che consentono di eseguire la verifica solo con l'uso di un'app di autenticazione. Se l'organizzazione dispone di un criterio che impedisce l'uso dei dispositivi mobili, è necessario prendere in considerazione una delle opzioni seguenti:

- Distribuire un'applicazione TOTP (con password monouso con limiti di tempo) che può essere eseguita in un sistema sicuro.

- Implementare una soluzione di terze parti che applichi l'autenticazione a più fattori per ogni account utente esistente nel tenant partner che offre l'opzione di verifica più appropriata.

- Acquistare [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) licenze per gli utenti interessati.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Quale automazione o integrazione è disponibile per usare le credenziali utente e garantire l'autenticazione?

Poiché viene applicata l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nella directory dei partner, questo influirà sull'automazione o sull'integrazione che usa le credenziali utente per l'autenticazione. È quindi importante identificare gli account usati in queste situazioni. Vedere l'elenco seguente di applicazioni o servizi di esempio da prendere in considerazione:

- Pannello di controllo usato per effettuare il provisioning delle risorse per conto dei clienti

- Integrazione con qualsiasi piattaforma usata per la fatturazione (in relazione al programma CSP) e supporto dei clienti

- Script di PowerShell che usano AZ, AzureRM, Azure AD, MS online e altri moduli

L'elenco precedente non è completo. È quindi importante eseguire una valutazione completa di qualsiasi applicazione o servizio nell'ambiente che usa le credenziali utente per l'autenticazione. Per quanto riguarda il requisito per l'autenticazione a più fattori, è necessario implementare le linee guida nel [framework del modello di applicazione sicura](/partner-center/develop/enable-secure-app-model) dove possibile.

## <a name="accessing-your-environment"></a>Accesso all'ambiente

Per comprendere meglio cosa o chi esegue l'autenticazione senza che venga richiesta l'autenticazione a più fattori, è consigliabile verificare l'attività di accesso. Tramite Azure Active Directory Premium, è possibile usare il report di accesso. Per altre informazioni su questo argomento, vedere [report delle attività di accesso nel portale di Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Se non si ha Azure Active Directory Premium o si sta cercando un modo per ottenere questa attività di accesso tramite PowerShell, è necessario usare il cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) dal modulo di PowerShell per il centro per i [partner](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-are-enforced"></a>Come vengono applicati i requisiti

I requisiti di sicurezza dei partner vengono applicati da Azure AD e, a sua volta, dal Centro per i partner, mediante il controllo della presenza dell'attestazione che stabilisce che la verifica dell'autenticazione a più fattori è stata eseguita. A partire dal 18 novembre 2019, Microsoft ha attivato misure di sicurezza aggiuntive (indicate in precedenza come "applicazione tecnica") per i tenant partner.

Dopo l'attivazione, agli utenti del tenant partner è stato richiesto di completare la verifica dell'autenticazione a più fattori durante l'esecuzione delle operazioni in modalità AOBO (Admin On Behalf Of, Amministratore per conto terzi), accedendo al portale del Centro per i partner o chiamando le API del Centro per i partner. Per altre informazioni, vedere [Imposizione dell'autenticazione a più fattori per il tenant partner](partner-security-requirements-mandating-mfa.md). 

I partner che non hanno soddisfatto i requisiti devono implementare queste misure non appena possibile per evitare interruzioni dell'attività. Se si usa Azure Active Directory Multi-Factor Authentication o Azure AD impostazioni predefinite di sicurezza, non è necessario eseguire alcuna azione aggiuntiva.

Se si usa una soluzione di autenticazione a più fattori di terze parti, è possibile che l'attestazione dell'autenticazione a più fattori non venga rilasciata. Se l'attestazione non è presente, Azure AD non sarà in grado di stabilire se la richiesta di autenticazione è stata verificata dall'autenticazione a più fattori. Per informazioni su come verificare il rilascio dell'attestazione prevista da parte della soluzione, leggi [Test dei requisiti di sicurezza per i partner](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se la soluzione di terze parti non rilascia l'attestazione prevista, sarà necessario interagire con il fornitore che ha sviluppato la soluzione per individuare le azioni da intraprendere.

## <a name="resources-and-samples"></a>Risorse ed esempi

Per il supporto e il codice di esempio, vedi le risorse seguenti:

- [Community del gruppo di linee guida per la sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Community del gruppo di linee guida per la sicurezza del Centro per i partner: si tratta di una community online in cui è possibile ottenere informazioni sugli eventi imminenti e porre qualsiasi domanda.
- [Esempi .NET del Centro per i partner](https://github.com/microsoft/partner-center-dotnet-samples): questo repository GitHub contiene esempi, sviluppati con .NET, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [Esempi Java del Centro per i partner](https://github.com/microsoft/partner-center-java-samples): questo repository GitHub contiene esempi, sviluppati con Java, che mostreranno come implementare il framework del modello di applicazione sicura.
- [Multi-Factor Authentication di PowerShell per il Centro per i partner](/powershell/partnercenter/multi-factor-auth): si tratta di un articolo che fornisce informazioni dettagliate su come implementare il framework del modello di applicazione sicura usando PowerShell.

## <a name="next-steps"></a>Passaggi successivi

- [Imposizione dell'autenticazione a più fattori per il tenant del partner](partner-security-requirements-mandating-mfa.md)