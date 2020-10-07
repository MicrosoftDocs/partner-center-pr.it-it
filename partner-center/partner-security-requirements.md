---
title: Requisiti di sicurezza dei partner
ms.topic: article
ms.date: 10/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introduce i requisiti dei partner per abilitare l'autenticazione a più fattori (MFA) e adottare il framework del modello di applicazione sicura.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 361a36adf40af67769a9a24ba1c485f2ad95b98c
ms.sourcegitcommit: 8a4a3de728532533276a88b1fd40c82b7a4ebb15
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/06/2020
ms.locfileid: "91763344"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Requisiti di sicurezza per partner che usano il Centro per i partner o le API del Centro per i partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti i fornitori del pannello di controllo
- Tutti gli advisor

**Utenti appropriati**

- Tutti gli utenti abilitati, inclusi gli utenti guest

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti nell'ecosistema agiscano e si assicurino che vengano adottate le protezioni di sicurezza appropriate. Per la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori di pannelli di controllo e i partner che partecipano al programma Cloud Solution Provider.

## <a name="overview"></a>Panoramica

I partner sono tenuti a imporre l'autenticazione a più fattori per tutti gli account utente esistenti nel tenant partner. Le condizioni associate ai requisiti di sicurezza dei partner sono state aggiunte al Contratto Microsoft Partner. Per quanto riguarda gli advisor, saranno in vigore gli stessi requisiti contrattuali.

I partner che non implementano i requisiti di sicurezza obbligatori non potranno eseguire transazioni nel programma Cloud Solution Provider o gestire i tenant dei clienti usando i diritti di amministratore con delega quando verranno imposti tali requisiti. Inoltre, i partner che non implementano i requisiti di sicurezza possono mettere a rischio la loro partecipazione ai programmi.  

Per la tua protezione e quella dei tuoi clienti, è opportuno che i partner intraprendano immediatamente le azioni seguenti:  

1. **Abilitare Multi-Factor Authentication (MFA) per tutti gli account utente inclusi nel tenant partner**. A tutti gli account utente inclusi nei tenant dei partner deve essere richiesta la verifica tramite autenticazione a più fattori al momento di accedere ai servizi cloud commerciali Microsoft o per eseguire transazioni in Cloud Solution Provider tramite il Centro per i partner o le API.

2. **Adottare il framework del modello di applicazione sicura**. Adottare il framework del modello di applicazione sicura. Tutti i partner che si integrano con l'API del Centro per i partner devono adottare tale framework per qualsiasi app e applicazione del modello di autenticazione utente.

    > [!IMPORTANT]
    > È consigliabile che i partner implementino il modello di applicazione sicura per l'integrazione con un'API Microsoft come Azure Resource Manager o Microsoft Graph oppure per l'uso dell'automazione, ad esempio tramite PowerShell con credenziali utente, per evitare interruzioni quando viene imposta l'autenticazione a più fattori.

L'abilitazione di Multi-Factor Authentication (MFA) e l'adozione del framework del modello di applicazione sicura consentiranno di proteggere l'infrastruttura e salvaguardare i dati del cliente da potenziali rischi per la sicurezza, ad esempio mediante l'identificazione di un furto o di altri eventi illeciti.  

## <a name="actions-that-you-need-to-take"></a>Azioni da intraprendere

Per adeguarti ai requisiti di sicurezza dei partner, devi imporre l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. È possibile procedere in uno dei modi seguenti:

- Implementazione delle [impostazioni predefinite per la sicurezza Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Acquisto di Azure Active Directory Premium per ogni account utente. Per altre informazioni, vedere [Pianificazione di una distribuzione di Azure Multi-Factor Authentication basata sul cloud](/azure/active-directory/authentication/howto-mfa-getstarted).

- Uso di una soluzione di terze parti per implementare l'autenticazione a più fattori per ogni account utente esistente nel tenant partner. Per assicurarsi che la soluzione fornisca le informazioni previste, vedere [come verranno implementati i requisiti di sicurezza](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Anche se l'autenticazione a più fattori non è richiesta contrattualmente per un cloud sovrano (21Vianet, Governo degli Stati Uniti e Germania), è consigliabile adottare questi requisiti di sicurezza.

## <a name="security-defaults"></a>Impostazioni predefinite per la sicurezza

Il criterio delle impostazioni predefinite per la sicurezza è una delle [opzioni](#actions-that-you-need-to-take) che i partner possono scegliere per implementare l'autenticazione a più fattori per i requisiti di sicurezza in base alle specifiche esigenze aziendali. Viene offerto un livello di sicurezza di case, abilitato senza costi aggiuntivi. Prima di abilitare le impostazioni predefinite per la sicurezza, esamina come abilitare l'autenticazione a più fattori per l'organizzazione con Azure AD e analizza le seguenti considerazioni chiave.

- I criteri di base saranno mantenuti ancora per un paio di mesi e deprecati per la fine di febbraio 2020.

- I partner che hanno già adottato i criteri di base devono agire per passare alle impostazioni predefinite per la sicurezza.

- Le impostazioni predefinite per la sicurezza sostituiscono a livello di disponibilità generale i criteri di base di anteprima. Dopo aver abilitato le impostazioni predefinite per la sicurezza, un partner non potrà più abilitare i criteri di base.

- Con le impostazioni predefinite per la sicurezza, tutti i criteri saranno abilitati contemporaneamente.

- Per i partner che usano l'[accesso condizionale](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), le [impostazioni predefinite per la sicurezza non sono disponibili](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Per il momento, il blocco dell'autenticazione legacy non verrà applicato ai partner. Tuttavia, poiché la maggior parte degli eventi correlati a identità compromesse proviene da tentativi di accesso con autenticazione legacy, i partner sono invitati a uscire dai protocolli meno recenti.

- L'account di sincronizzazione di Azure AD Connect è escluso dalle impostazioni predefinite per la sicurezza.

- Per informazioni dettagliate, leggi [Abilitare Multi-Factor Authentication per l'organizzazione](/azure/active-directory/authentication/concept-mfa-get-started) e [Impostazioni predefinite per la sicurezza Azure Active Directory](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Le impostazioni predefinite per la sicurezza Azure AD sono l'evoluzione dei criteri di protezione di base semplificati. Se hai già abilitato i criteri di protezione di base, è consigliabile abilitare le impostazioni predefinite per la sicurezza.

Per passare dai criteri di base alle impostazioni predefinite per la sicurezza, leggi [Che cosa sono le impostazioni predefinite della sicurezza?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Considerazioni

Poiché questi requisiti si applicano a tutti gli account utente inclusi nel tenant partner, devi considerare diversi aspetti per garantire una distribuzione senza problemi, inclusa l'identificazione degli account utente in Azure Active Directory che non possono eseguire l'autenticazione a più fattori, nonché delle applicazioni e dei dispositivi usati dall'organizzazione che non supportano l'autenticazione moderna.

Prima di eseguire qualsiasi azione, è consigliabile identificare gli elementi seguenti:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Si hanno applicazioni o dispositivi che non supportano l'uso dell'autenticazione moderna?

Quando imponi l'autenticazione a più fattori, i protocolli per l'uso dell'autenticazione legacy, ad esempio IMAP, POP3, SMTP e così via, verranno bloccati perché non supportano l'autenticazione a più fattori. Per ovviare a questa limitazione, puoi usare una funzionalità nota come [password dell'app](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) per assicurarti che l'applicazione o il dispositivo possa eseguire comunque l'autenticazione. Esaminare le considerazioni per l'uso delle password dell'app [qui](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) documentate per determinare se è possibile usarle nell'ambiente in uso.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Sono presenti utenti che usano Office 365 fornito dalle licenze associate al tenant partner?

Prima di implementare qualsiasi soluzione, è consigliabile determinare quale versione di Microsoft Office viene usata dagli utenti del tenant partner. È possibile che gli utenti riscontrino problemi di connettività con applicazioni come Outlook. Prima di implementare l'autenticazione a più fattori, è importante assicurarsi che sia in uso Outlook 2013 SP1 o versione successiva e che nell'organizzazione sia abilitata l'autenticazione moderna. Per altre informazioni, vedere [Abilitare l'autenticazione moderna in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Per abilitare l'autenticazione moderna in tutti i dispositivi che eseguono Windows, su cui è installato Microsoft Office 2013, sarà necessario creare due chiavi del registro di sistema. Vedere [Abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Esistono criteri che impediscono agli utenti di usare i propri dispositivi mobili durante il lavoro?

È importante identificare qualsiasi criterio aziendale che impedisca ai dipendenti di usare dispositivi mobili durante l'orario di lavoro perché questo potrà influenzare la soluzione di autenticazione a più fattori implementata. Esistono soluzioni, ad esempio quella fornita tramite l'implementazione delle [impostazioni predefinite per la sicurezza Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), che consentono di eseguire la verifica solo con l'uso di un'app di autenticazione. Se l'organizzazione dispone di un criterio che impedisce l'uso dei dispositivi mobili, è necessario prendere in considerazione una delle opzioni seguenti:

- Distribuire un'applicazione TOTP (con password monouso con limiti di tempo) che può essere eseguita in un sistema sicuro

- Implementare una soluzione di terze parti per l'autenticazione a più fattori per ogni account utente esistente nel tenant partner che offre l'opzione di verifica più appropriata

- Acquistare licenze [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) per gli utenti interessati

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Quale automazione o integrazione è disponibile per usare le credenziali utente e garantire l'autenticazione?

Poiché il requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nella directory del partner, verrà usata l'automazione o l'integrazione che sfrutta le credenziali utente per l'autenticazione. È quindi importante identificare gli account usati in queste situazioni. Vedere l'elenco seguente di applicazioni o servizi di esempio da prendere in considerazione:

- Pannello di controllo usato per effettuare il provisioning delle risorse per conto dei clienti

- Integrazione con qualsiasi piattaforma usata per la fatturazione (in relazione al programma CSP) e supporto dei clienti

- Script di PowerShell che usano i moduli AZ, AzureRM, Azure AD, MS online e così via

L'elenco precedente non è completo. È quindi importante eseguire una valutazione completa di qualsiasi applicazione o servizio nel proprio ambiente che sfrutti le credenziali utente per l'autenticazione. Per far fronte al requisito di autenticazione a più fattori, è necessario, dove possibile, implementare le indicazioni nel [framework del modello di applicazione sicura](/partner-center/develop/enable-secure-app-model).

## <a name="accessing-your-environment"></a>Accesso all'ambiente

Per comprendere meglio cosa o chi esegue l'autenticazione senza che venga richiesta l'autenticazione a più fattori, è consigliabile verificare l'attività di accesso. Tramite Azure Active Directory Premium puoi sfruttare i vantaggi offerti dal report sull'accesso. Per altre informazioni, vedi [Report dell'attività di accesso nel portale di Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Se non hai Azure Active Directory Premium o stai cercando di ottenerlo tramite PowerShell, dovrai usare il cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) del modulo [PowerShell per il Centro per i partner](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Come verranno implementati i requisiti

I requisiti di sicurezza dei partner verranno implementati da Azure Active Directory e, a sua volta, dal Centro per i partner, mediante il controllo della presenza dell'attestazione che stabilisce che la verifica dell'autenticazione a più fattori è stata eseguita. A partire dal 18 novembre 2019, Microsoft attiverà misure di sicurezza aggiuntive (indicate in precedenza come "imposizione tecnica") per i tenant dei partner. 

Con l'attivazione, agli utenti nel tenant partner verrà richiesto di completare la verifica tramite autenticazione a più fattori quando eseguono operazioni in modalità AOBO (Admin On Behalf Of, Amministratore per conto terzi). Microsoft continuerà a estendere l'ambito delle misure di sicurezza ad altri scenari e ruoli utente, inviando in anticipo una comunicazione ai partner. Per altre informazioni, fai riferimento a questo documento che verrà aggiornato spesso. I partner che non hanno soddisfatto i requisiti devono implementare queste misure non appena possibile per evitare interruzioni dell'attività. 

Se usi Azure Multi-Factor Authentication o le impostazioni predefinite per la sicurezza Azure AD, non devi intraprendere altre azioni.

Quando si usa una soluzione di autenticazione a più fattori di terze parti, è possibile che l'attestazione di autenticazione a più fattori non venga rilasciata. Se l'attestazione non è presente, Azure Active Directory non sarà in grado di stabilire se la richiesta di autenticazione è stata verificata dall'autenticazione a più fattori. Per informazioni su come verificare il rilascio dell'attestazione prevista da parte della soluzione, leggi [Test dei requisiti di sicurezza per i partner](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Se la soluzione di terze parti non rilascia l'attestazione prevista, sarà necessario interagire con il fornitore che ha sviluppato la soluzione per individuare le azioni da intraprendere.

## <a name="resources-and-support"></a>Risorse e supporto

Per il supporto e il codice di esempio, vedi le risorse seguenti:

- [Community del gruppo di linee guida per la sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): Community del gruppo di linee guida per la sicurezza del Centro per i partner: si tratta di una community online in cui è possibile ottenere informazioni sugli eventi imminenti e porre qualsiasi domanda.
- [Esempi .NET del Centro per i partner](https://github.com/microsoft/partner-center-dotnet-samples): questo repository GitHub contiene esempi, sviluppati con .NET, che dimostreranno come implementare il framework del modello di applicazione sicura.
- [Esempi Java del Centro per i partner](https://github.com/microsoft/partner-center-java-samples): questo repository GitHub contiene esempi, sviluppati con Java, che mostreranno come implementare il framework del modello di applicazione sicura.
- [Multi-Factor Authentication di PowerShell per il Centro per i partner](/powershell/partnercenter/multi-factor-auth): si tratta di un articolo che fornisce informazioni dettagliate su come implementare il framework del modello di applicazione sicura usando PowerShell.