---
title: Requisiti di sicurezza dei partner | Centro per i partner
ms.topic: article
ms.date: 06/25/2019
description: Informazioni sui requisiti di sicurezza per i consulenti e partner la partecipazione al programma Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Provider di soluzioni Cloud di programma, CSP, fornitore del Pannello di controllo, CPV, multi-factor authentication, MFA, proteggere il modello di applicazione, modello di app protette, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 8f513b96619819cd6ba892625e47731170d22130
ms.sourcegitcommit: de88bb4cd994f1a106a5d02242261042958d4300
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2019
ms.locfileid: "67549531"
---
# <a name="partner-security-requirements"></a>Requisiti di sicurezza di partner

**Si applica a**

- Tutti i partner del programma Cloud Solution Provider
  - Bill diretto
  - Provider indiretti
  - Rivenditore indiretto
- Tutti i fornitori di Pannello di controllo
- Tutti i consulenti

Sicurezza e privacy dei clienti e partner sono le attività più importanti per Microsoft. Si continua a visualizzare un numero crescente di più sofisticati attacchi alla sicurezza, riguardanti principalmente le identità compromesse. Come controlli preventivi svolgono un ruolo fondamentale in una strategia globale di difesa per contrastare attacchi alla sicurezza, si inizierà l'applicazione di un set di requisiti di sicurezza obbligatori per proteggere i clienti e partner.

> [!NOTE]
> È consigliabile che tutti i partner vincolante tramite (21Vianet, US Government e Germania) con cloud sovrano agiscano e adottano immediatamente questi nuovi requisiti di sicurezza. Tuttavia, questi partner non sono richiesti per soddisfare i nuovi requisiti di sicurezza efficaci 1 agosto 2019. Microsoft invierà altri dettagli riguardanti l'imposizione di questi requisiti di sicurezza per cloud sovrani in futuro.

## <a name="overview-of-the-requirements"></a>Panoramica dei requisiti

Tutti i partner che fanno parte il programma Cloud Solution Provider, i fornitori di Pannello di controllo e partner di Advisor sono necessari per applicare multi-Factor Authentication (MFA) per ogni utente, inclusi gli account del servizio, i tenant del partner. Questa operazione può essere eseguita abilitando due [i criteri di base di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). I criteri di base sono un set di criteri predefiniti che consentono di proteggere da attacchi comuni molte organizzazioni. Questi attacchi comuni possono includere phishing, riproduzione e spray password. I criteri di base sono disponibili in tutte le edizioni di Azure Active Directory. Microsoft sta rendendo questi criteri di protezione della linea di base disponibili per tutti gli utenti per consentire ai clienti e partner di implementare procedure di sicurezza di alto livello in.

I criteri di due della linea di base che devono essere abilitati sono descritti nella tabella seguente.

|**Criterio**| |
|-----|-----|
|**Richiedere l'autenticazione MFA per gli amministratori**|Abilita autenticazione a più fattori richiedono per criteri di gruppo admins, verrà richiesto agli utenti nei ruoli di amministratore di effettuare la registrazione per MFA usando l'App Authenticator. Dopo aver completata la registrazione MFA, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta Accedi.|
|**Protezione dell'utente finale**|Protezione dell'utente finale è un criterio della linea di base MFA basato sul rischio che protegge tutti gli utenti in una directory. Abilita questo criterio richiede tutti gli utenti di effettuare la registrazione per MFA usando l'App Authenticator. Gli utenti possono ignorare la richiesta di registrazione MFA per 14 giorni, dopodiché verranno bloccati dall'accesso fino a quando non si registrano per MFA. Una volta registrato per MFA, verranno richiesto agli utenti per MFA solo durante i tentativi di accesso rischiosi. Account utente compromessi vengono bloccate finché non viene reimpostata la password e gli eventi di rischio sono stati ignorati.|

Quando questi criteri sono abilitati, ogni utente sarà in grado di usare Azure MFA senza costi aggiuntivi. Se si usa una soluzione di terze parti, quindi è necessario imporre l'autenticazione MFA per ogni utente quando si accede a servizi cloud commerciale Microsoft.

> [!IMPORTANT]
> Poiché l'autenticazione a più fattori verranno applicati a tutti gli utenti della directory dei partner, ci sarà un impatto per qualsiasi automazione o l'integrazione che utilizza le credenziali dell'utente. Per risolvere tale impatto, dovrai modificare il modo in cui che l'automazione o l'integrazione si connette a servizi cloud commerciali di Microsoft. Se il servizio si è connessi supporta l'autenticazione basata su token, quindi è consigliabile implementare il [framework di modello di applicazione Secure](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="what-actions-do-i-need-to-take"></a>Quali azioni è necessario eseguire? 

Per garantire che gli utenti nel tenant del partner sono protette, è necessario imporre l'autenticazione MFA per ogni utente (inclusi gli account del servizio). Questa operazione può essere eseguita abilitando il [Richiedi autenticazione a più fattori per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) e [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) i criteri di base. Prima di abilitare questi criteri, è importante comprendere le attività e le modalità in cui questi influiscono qualsiasi componente di automazione o l'integrazione e gli utenti.

> [!NOTE]
> [I criteri di base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) continuerà a evolversi nel tempo. È consigliabile rivedere periodicamente la documentazione per ulteriori informazioni sull'evoluzione dei criteri.

### <a name="considerations"></a>Considerazioni

Poiché i requisiti di sicurezza si applicano a tutti gli utenti in una directory dei partner, è necessario apportare per garantire una regolare distribuzione diverse considerazioni. Queste considerazioni includono l'identificazione degli utenti in Azure Active Directory che non è possibile o non devono eseguire MFA, nonché applicazioni e client usati dall'organizzazione che non supportano l'autenticazione moderna.

#### <a name="self-service-password-reset"></a>Reimpostazione autonoma della password

La reimpostazione della password self-service (SSPR) è una funzionalità di Azure Active Directory che consente ai dipendenti di reimpostare le password senza dover contattare il personale IT. I dipendenti devono registrare per o essere registrati per la prima di usare il servizio di reimpostazione della password self-service. Durante la registrazione, il dipendente sceglie uno o più metodi di autenticazione abilitati dall'organizzazione.

SSPR consente ai dipendenti di essere sbloccati rapidamente e continuare a funzionare indipendentemente dalla loro posizione o l'ora del giorno. Consentendo agli utenti di sbloccare autonomamente, l'organizzazione può ridurre il tempo non produttivo ed elevati costi di assistenza per problemi più comuni correlati alle password.

Quando la [protezione degli utenti finali](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) della linea di base i criteri sono abilitati tutti gli account utente compromessi verranno bloccati fino a quando non viene reimpostata la password e gli eventi di rischio sono stati ignorati. Considerando questo è consigliabile che ogni utente, che è un amministratore globale, seguire questa procedura per registrare per SSPR

1. Individuare il [pagina di installazione di SSPR](https://aka.ms/ssprsetup)
2. Immettere il nome utente e password
3. Configurare almeno una delle opzioni verifiche che verranno usate per verificare l'identità dell'utente durante la reimpostazione della password.  

Quando è stato compromesso un account amministratore dovrà intervenire per ripristinare l'accesso per l'utente interessato. Vedere le [passaggi per sbloccare un utente](#recovering-compromised-accounts) per informazioni dettagliate sul processo per sbloccare l'utente.

#### <a name="legacy-protocols"></a>Protocolli legacy

Protocolli di autenticazione legacy (IMAP, SMTP, POP3, e così via) usati dai client di posta elettronica per effettuare richieste di autenticazione. Questi protocolli non supportano l'autenticazione a più fattori. La maggior parte dei rischi di compromissione di account sono causata da cattivi attori esegue gli attacchi contro i protocolli legacy, il tentativo di ignorare MFA. Per garantire che è richiesta la MFA quando accedono a un account in una directory di partner e cattivi attori non sono in grado di ignorare MFA, questi requisiti di sicurezza blocca tutte le richieste di autenticazione per i protocolli legacy.

### <a name="enabling-the-baseline-policies"></a>Abilitare i criteri di base

Vedere le [che implementa l'esercitazione di requisiti di sicurezza partner](tutorials/partner-security-requirements.yml) per un'esperienza guidata riguardanti l'implementazione di criteri di base.  

#### <a name="require-mfa-for-admins"></a>Richiedere l'autenticazione MFA per gli amministratori

Il *Richiedi autenticazione a più fattori per l'amministrazione* criterio di base richiede MFA per i seguenti ruoli di directory, considerati i ruoli di Azure Active Directory con più privilegi:

- Amministratore globale
- Amministratore di SharePoint
- Amministratore di Exchange
- Amministratore di accesso condizionale
- Amministratore della sicurezza
- Amministratore supporto tecnico o amministratore Password
- Amministratore fatturazione
- Amministratore utenti

Con l'abilitazione dell'autenticazione a più fattori richiedono per criteri di gruppo admins, i ruoli di nove amministratore precedente saranno necessario effettuare la registrazione per MFA usando l'App Authenticator. Dopo aver completata la registrazione MFA, gli amministratori dovranno eseguire autenticazione a più fattori ogni volta che accedi.

Se l'organizzazione dispone di questi account in uso nel codice o gli script, è consigliabile sostituirli con [gestito identità](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Per abilitare questo criterio e proteggere gli amministratori:

1. Accedi per il **portale di Azure** come un amministratore globale, amministratore della sicurezza o amministratore di accesso condizionale.
2. Passare a **Azure Active Directory** > **accesso condizionale**.
3. Nell'elenco dei criteri, selezionare **criterio di base: Richiedere l'autenticazione MFA per gli amministratori**.
4. Impostare **abilitare i criteri** al **Usa i criteri immediatamente**.
5. Fare clic su **salvare**.

    ![Richiedere l'autenticazione MFA per gli amministratori](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> Prima di abilitare questo criterio, assicurarsi che gli utenti non usano protocolli di autenticazione legacy. Vedere l'articolo [come: L'autenticazione legacy di blocco con Azure Active Directory con accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) per altre informazioni.

> [!IMPORTANT]
> È presente un problema noto, che influisce sulla possibilità di connettersi a Exchange Online PowerShell con privilegi di amministratore delegati. Vedere le [Exchange Online PowerShell](#exchange-online-powershell) noto problema prima di abilitare questo criterio se si usa questo modulo di PowerShell.

#### <a name="end-user-protection"></a>Protezione dell'utente finale

Il criterio di base di protezione degli utenti finali protegge tutti gli utenti in una directory. Abilita questo criterio richiede tutti gli utenti di registrarsi per Azure MFA entro 14 giorni. Una volta registrato, verranno richiesto agli utenti per MFA solo durante i tentativi di accesso rischiosi. Account utente compromessi vengono bloccate finché non reimpostare e rischio licenziamento password.

I criteri **criterio di base: Protezione dell'utente finale** è preconfigurata e verrà visualizzata nella parte superiore quando si passa al pannello di accesso condizionale nel portale di Azure.

Per abilitare questo criterio e proteggere gli utenti:

1. Accedi per il **portale di Azure** come un amministratore globale, amministratore della sicurezza o amministratore di accesso condizionale.
2. Passare a **Azure Active Directory** > **accesso condizionale**.
3. Nell'elenco dei criteri, selezionare **criterio di base: Protezione dell'utente finale (anteprima)** .
4. Impostare **abilitare i criteri** al **Usa i criteri immediatamente**.
5. Fare clic su **salvare**.

    ![Protezione dell'utente finale](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> Prima di abilitare questo criterio, assicurarsi che gli utenti non usano protocolli di autenticazione legacy. Vedere l'articolo [come: L'autenticazione legacy di blocco con Azure Active Directory con accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) per altre informazioni.

> [!IMPORTANT]
> È presente un problemi noti, che influisce sulla possibilità di connettersi a Exchange Online PowerShell con privilegi di amministratore delegati. Vedere le [Exchange Online PowerShell](#exchange-online-powershell) noto problema prima di abilitare questo criterio se si usa questo modulo di PowerShell.

## <a name="common-issues"></a>Problemi comuni

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Dopo aver abilitato i criteri di base, si noterà che l'automazione o l'integrazione sta riscontrando un'eccezione simile alla seguente

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

Il motivo di questa eccezione è che si esegue l'autenticazione usando le credenziali dell'utente e autenticazione a più fattori è ora obbligatorio. Per risolvere questa eccezione, è necessario usare un token di accesso per l'autenticazione. Vedere le [Guida per proteggere modello applicativo](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) per altre informazioni.

>[!IMPORTANT]
>I moduli di PowerShell e API più recenti supportano la possibilità di usare un token di accesso per l'autenticazione. Tuttavia, esistono alcune che attualmente non supportano questa funzionalità. Se è necessario determinare se il modulo di PowerShell o API che si desidera sfruttare supporta l'utilizzo di un token di accesso per l'autenticazione, quindi inviare un messaggio sul [gruppo di Partner Center sicurezza indicazioni](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) della community.

#### <a name="aadsts700082"></a>AADSTS700082

Dopo aver implementato il framework Secure modello applicativo è probabile si riceverà l'eccezione seguente 90 giorni dopo la generazione del token di aggiornamento iniziale

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Per quanto riguarda Azure Active Directory la durata massima per un aggiornamento di token è 90 giorni. Per risolvere questo errore, è necessario generare e archiviare in modo sicuro un nuovo token di aggiornamento. Si noti che è possibile aggiornare il token di aggiornamento a livello di codice perché, con ogni richiesta per Azure Active Directory per un token di accesso viene restituito un nuovo token di aggiornamento. È possibile implementare la logica appropriata per aggiornare il token di aggiornamento archiviato in modalità protetta prima della scadenza.

Visualizzare [durata dei token configurabili in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) per altre informazioni.

### <a name="recovering-compromised-accounts"></a>Il ripristino di account compromessi

Per proteggere i clienti, il servizio credenziali perse di Microsoft consente di trovare coppie di nome utente/password disponibile pubblicamente. Se uno dei nostri utenti corrispondono, contribuiamo alla protezione immediatamente tale account. Gli utenti identificati come avente una credenziale persa vengono confermati compromesso. Questi utenti non potranno accedere fino a quando non viene reimpostato la propria password.

Gli utenti assegnati una licenza di Azure AD Premium possono ripristinare l'accesso tramite la reimpostazione della password self-service (SSPR) se è abilitata la funzionalità nella propria directory. Gli utenti senza licenza premium che diventano bloccati devono contattare un amministratore per eseguire una reimpostazione manuale della password e chiudere l'evento di rischio utente contrassegnato.

#### <a name="steps-to-unblock-a-user"></a>Procedura per sbloccare un utente

Verificare che l'utente è stata bloccata dai criteri, esaminare i log di accesso dell'utente.

1. Un amministratore deve eseguire l'accesso per il **portale di Azure** e passare alla **Azure Active Directory** > **utenti** > fare clic sul nome dell'utente e passare agli accessi.
2. Per avviare la reimpostazione su un utente bloccato della password, un amministratore deve passare a **Azure Active Directory** > **utenti contrassegnati per il rischio**
3. Fare clic sull'utente il cui account viene bloccato per visualizzare informazioni sull'attività dell'utente recente accesso.
4. Fare clic su Reimposta Password per assegnare una password temporanea che deve essere modificata dall'account di accesso successivo.
5. Fare clic su Elimina tutti gli eventi per reimpostare il punteggio di rischio dell'utente.

L'utente può accedere a questo punto, reimpostare la password e accedere all'applicazione.

## <a name="known-issues"></a>Problemi noti

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Quando è abilitata MFA partner non sarà in grado di utilizzare i privilegi di amministratore delegati con Exchange Online PowerShell per eseguire azioni su ai clienti. Visualizzare [connettersi a Exchange Online PowerShell multi-factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) per altre informazioni su questa limitazione.

## <a name="resources-and-support"></a>Risorse e supporto

Tramite il [community di Partner Center sicurezza indicazioni gruppo](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) puoi verrà trovare risorse aggiuntive e informazioni sugli eventi imminenti, ad esempio orario di ufficio tecnici. Vedere le [domande frequenti](http://assetsprod.microsoft.com/security-requirements-faq.pdf) per altre informazioni sui requisiti.

### <a name="developers"></a>Sviluppatori

- [Abilitazione del modello applicativo sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Esempi di .NET Centro per i partner](https://github.com/microsoft/partner-center-dotnet-samples)
- [Esempi di Java Centro per i partner](https://github.com/microsoft/partner-center-java-samples)
- [PowerShell di Centro per i partner che implementa il modello di applicazione Secure](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
