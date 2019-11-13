---
title: Promandamento dell'autenticazione a più fattori per il tenant partner | Centro per i partner
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Dettagli sull'uso dell'autenticazione a più fattori per i requisiti di sicurezza del tenant partner
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 9241e7fd7f9812e2c456eac70065e185a9cf8d61
ms.sourcegitcommit: 0f14e29540c6814f01395924223b495cc5299954
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/13/2019
ms.locfileid: "73983345"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Imposizione di multi-factor authentication per il tenant partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti gli advisor

Questi partner saranno tenuti a completare la verifica dell'autenticazione a più fattori per le aree seguenti:

- [Dashboard del centro](#partner-center-dashboard) per i partner (con destinazione H1 CY2020)
- [API del centro](#partner-center-api) per i partner (con destinazione H1 CY2020)
- [Amministrazione delegata partner](#partner-delegated-administration) (a partire dal 18 novembre 2019)

Lo scopo di questa funzionalità è aiutare i partner a proteggere l'accesso alle risorse dei clienti da eventuali compromessi.

## <a name="partner-center-dashboard"></a>Dashboard del centro per i partner
Alcune pagine nel dashboard del centro per i partner verranno protette con autenticazione a più fattori, tra cui:

* Tutte le pagine nella scheda **Customers (clienti** ).
* Tutte le pagine nella scheda **supporto > richieste del cliente** .

Se si tenta di accedere a una di queste pagine e la verifica dell'autenticazione a più fattori non è stata completata in precedenza, sarà necessario eseguire questa operazione.

I tipi di utente seguenti sono autorizzati ad accedere a queste pagine protette da multi-factor authentication e pertanto sono interessate da questa funzionalità, tra cui:

* Agenti di amministrazione
* Agenti di vendita
* Agenti helpdesk

Per illustrare il funzionamento di questo, considerare i due esempi seguenti.

**Esempio 1: il partner ha implementato Azure AD autenticazione a più fattori**
1.  Jane funziona per CSP contoso. Contoso ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant partner Contoso usando Azure AD autenticazione a più fattori.
2.  Dalla propria workstation Jane avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del centro per i partner, che non è protetta con l'autenticazione a più fattori. Il centro per i partner reindirizza Jane a Azure AD per l'accesso.
3.  A causa della configurazione esistente di Azure AD autenticazione a più fattori di Contoso, Jane è necessario per completare la verifica dell'autenticazione a più fattori. Al completamento dell'accesso e della verifica dell'autenticazione a più fattori, Jane viene reindirizzato alla pagina di panoramica del dashboard del centro per i partner.
4.  Jane tenta di accedere a una delle pagine protette con autenticazione a più fattori nel centro per i partner. Poiché Jane ha già completato la verifica dell'autenticazione a più fattori durante l'accesso in precedenza, Jane può accedere alla pagina protetta da multi-factor authentication senza dover eseguire di nuovo la verifica dell'autenticazione a più fattori.

**Esempio 2: l'autenticazione a più fattori di terze parti è stata implementata dal partner**
1. Trent funziona per CSP Wingtip. Wingtip ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant del partner Wingtip usando l'autenticazione a più fattori di terze parti integrata con Azure AD tramite la Federazione delle identità.
2. Dalla sua workstation, Trent avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del centro per i partner, che non è protetta con l'autenticazione a più fattori. Il centro per i partner reindirizza Justin a Azure AD per l'accesso.
3. Poiché in Wingtip è stata impostata la Federazione delle identità, Azure AD reindirizza Trent al provider di identità federato per completare la verifica dell'accesso e dell'autenticazione a più fattori. Al completamento dell'accesso e della verifica dell'autenticazione a più fattori, Trent viene reindirizzato a Azure AD e quindi alla pagina di panoramica del dashboard del centro per i partner.
4. Justin tenta di accedere a una delle pagine protette con autenticazione a più fattori nel centro per i partner. Poiché Trent ha già completato la verifica dell'autenticazione a più fattori durante l'accesso in precedenza, Trent può accedere alla pagina protetta da multi-factor authentication senza che sia necessario eseguire nuovamente la verifica dell'autenticazione a più fattori.

**Esempio 3: il partner non ha implementato multi-factor authentication**
1. Giorgio lavora per CSP fabrikam. Fabrikam non ha implementato l'autenticazione a più fattori per tutti gli utenti del tenant partner Fabrikam.
2. Dalla sua workstation Giorgio avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del centro per i partner, che non è protetta con l'autenticazione a più fattori. Il centro per i partner reindirizza Giorgio a Azure AD per l'accesso.
3. Poiché Fabrikam non ha implementato l'autenticazione a più fattori, per completare la verifica dell'autenticazione a più fattori, Al completamento dell'accesso, Giorgio viene reindirizzato alla pagina di panoramica del dashboard del centro per i partner.
4. Giorgio tenta di accedere a una delle pagine protette con autenticazione a più fattori nel centro per i partner. Dal momento che John non ha completato la verifica dell'autenticazione a più fattori, il centro per i partner reindirizza Giorgio a Azure AD per completare la verifica dell'autenticazione Poiché questa è la prima volta che Giorgio è necessario per completare l'autenticazione a più fattori, John è anche richiesto di effettuare la registrazione per l'autenticazione a più fattori usando Microsoft Authenticator app. Al termine della registrazione dell'autenticazione a più fattori e della verifica dell'autenticazione a più fattori, Giorgio può accedere alla pagina protetta da AMF.

## <a name="partner-center-api"></a>API del centro per i partner

L'API del centro per i partner supporta sia l'autenticazione solo app che l'autenticazione dell'app e dell'utente. Quando si usa l'autenticazione app + User, il centro per i partner richiede la verifica dell'autenticazione a più fattori. In particolare, quando un'applicazione partner vuole inviare una richiesta API al centro per i partner, deve includere un token di accesso nell'intestazione dell'autorizzazione della richiesta. Quando il centro per i partner riceve una richiesta API con un token di accesso ottenuto usando l'autenticazione dell'utente e dell'app, l'API del centro per i partner verificherà la presenza *del valore di autenticazione a più fattori* nell'attestazione di riferimento al metodo di *autenticazione (AMR)* . È possibile usare un decodificatore JWT per verificare se un token di accesso contiene il valore AMR (Authentication method Reference) previsto o meno:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Se il valore è presente, il centro per i partner conclude che la verifica dell'autenticazione a più fattori è stata completata ed elabora la richiesta dell'API. Se il valore non è presente, l'API del centro per i partner rifiuterà la richiesta con la risposta seguente:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>Amministrazione delegata partner

### <a name="using-service-portals"></a>Uso di portali di servizio

Gli account partner, inclusi gli agenti di amministrazione e gli agenti helpdesk, possono usare i propri privilegi amministrativi delegati del partner per gestire le risorse dei clienti tramite i portali di Microsoft Online Services, l'interfaccia della riga di comando (CLI) e le API (usando l'autenticazione app + User).

Quando si accede ai portali di Microsoft Online Services usando i privilegi amministrativi delegati del partner per gestire le risorse dei clienti, molti di questi portali richiedono che l'account del partner esegua l'autenticazione interattiva, con il cliente Azure Active Directory tenant impostato come contesto di autenticazione: l'account partner è necessario per accedere al tenant del cliente.

Quando Azure Active Directory riceve tali richieste di autenticazione, richiede l'account del partner per completare la verifica dell'autenticazione a più fattori. Esistono due possibili esperienze utente, a seconda che l'account partner sia un'identità gestita o federata:

- Se l'account partner è un'identità **gestita** , Azure Active Directory chiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è registrato per l'autenticazione a più fattori con Azure Active Directory prima, all'utente verrà richiesto di completare prima la [registrazione](#mfa-registration-experience) dell'autenticazione a più fattori.

- Se l'account partner è un'identità **federata** , l'esperienza dipende dal modo in cui l'amministratore partner ha configurato la federazione in Azure Active Directory. Quando si configura la Federazione in Azure Active Directory, l'amministratore partner può indicare a Azure Active Directory se il provider di identità federato supporta o meno l'autenticazione a più fattori. In tal caso, Azure Active Directory reindirizza l'utente al provider di identità federato per completare la verifica dell'autenticazione a più fattori. In caso contrario, Azure Active Directory chiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è registrato per l'autenticazione a più fattori con Azure Active Directory prima, all'utente verrà richiesto di completare prima la [registrazione](#mfa-registration-experience) dell'autenticazione a più fattori.

L'esperienza complessiva è molto simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato [Azure ad criterio di base-](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)autenticazione a più fattori per gli amministratori, che richiede tutti gli account con diritti amministrativi per accedere al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti di amministrazione e gli agenti helpdesk. A scopo di test, i partner possono abilitare i criteri di autenticazione a più fattori [per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) nel tenant del cliente, quindi provare a usare i privilegi di amministrazione delegata del partner per accedere al tenant del cliente.

> [!NOTE]
> Non tutti i portali dei servizi online Microsoft richiedono account partner per accedere al tenant del cliente durante l'accesso alle risorse dei clienti usando privilegi amministrativi delegati dal partner. Ma richiedono solo che gli account partner accedano al tenant partner. Un esempio è l'interfaccia di amministrazione di Exchange. Nel corso del tempo, si prevede che questi portali necessitino degli account partner per accedere al tenant del cliente quando si usano i privilegi amministrativi delegati del partner.

### <a name="using-service-apis"></a>Uso delle API del servizio
Alcune API di Microsoft Online Services (ad esempio Azure Resource Manager, Azure AD Graph, Microsoft Graph e così via) supportano partner che usano privilegi amministrativi delegati dai partner per gestire le risorse dei clienti a livello di codice. Per sfruttare i privilegi amministrativi delegati del partner con queste API, l'applicazione partner deve includere un token di accesso nell'intestazione di autorizzazione della richiesta API, in cui il token di accesso viene ottenuto con un account utente partner per l'autenticazione con Azure AD, con il Customer Azure AD impostato come contesto di autenticazione. È necessario che l'applicazione partner disponga di un account utente partner per accedere al tenant del cliente.

Quando Azure AD riceve, ad esempio la richiesta di autenticazione, Azure AD richiederà l'account utente partner per completare la verifica dell'autenticazione a più fattori. Se l'account utente del partner non è stato registrato per l'autenticazione a più fattori in precedenza, all'account utente verrà richiesto di completare prima la registrazione a più fattori.

Questa funzionalità interessa tutte le applicazioni partner integrate con queste API utilizzando privilegi amministrativi delegati dai partner. Per garantire che le applicazioni partner possano continuare a usare queste API senza interruzioni:

- Il partner deve evitare di usare un metodo di autenticazione utente non interattivo con Azure AD per ottenere il token di accesso. Quando si usa un metodo di autenticazione utente non interattivo come il [flusso della password](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure ad non sarà in grado di richiedere all'utente di completare la verifica dell'autenticazione a più fattori. Il partner deve passare all'uso di un metodo di autenticazione utente interattivo, ad esempio il [flusso OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) .
- Durante il metodo di autenticazione utente interattiva, il partner deve usare un account utente partner già abilitato per l'autenticazione a più fattori. In alternativa, quando richiesto dal Azure AD, il partner può completare la registrazione dell'autenticazione a più fattori e la verifica dell'autenticazione a più fattori durante l'accesso.
- Questo è molto simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato [Azure ad criterio di base-](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)autenticazione a più fattori per gli amministratori, che richiede a tutti gli account utente con diritti amministrativi di accedere al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti di amministrazione e gli agenti helpdesk. A scopo di test, i partner possono abilitare i criteri di autenticazione a più fattori [per gli amministratori](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) nel tenant del cliente, quindi provare a usare i privilegi di amministrazione delegata del partner per accedere a livello di codice al tenant del cliente.

### <a name="mfa-registration-experience"></a>Esperienza di registrazione con autenticazione a più fattori
Durante la verifica dell'autenticazione a più fattori, se l'account partner non è stato registrato per l'autenticazione a più fattori prima di, Azure AD chiederà all'utente di completare prima la registrazione

![Passaggio 1 della registrazione dell'autenticazione a più fattori](images/MfaRegistration1.png)

Dopo aver fatto clic su **Avanti**, all'utente verrà richiesto di scegliere da un elenco di metodi di verifica, ad esempio telefono, SMS e app di autenticazione.

![Passaggio 2 della registrazione dell'autenticazione a più fattori](images/MfaRegistration2.png)

Una volta completata la registrazione, l'utente dovrà completare la verifica dell'autenticazione a più fattori in base alla verifica scelta dall'utente.



## <a name="request-for-technical-exception"></a>Richiesta di eccezione tecnica

I partner possono applicare un'eccezione tecnica per evitare la verifica dell'autenticazione a più fattori se riscontrano problemi tecnici con i Microsoft Online Services e non esistono soluzioni o soluzioni attuabili. Prima di procedere, consultare le sezioni seguenti:

 - [Elenco dei problemi comuni segnalati dai partner](#list-of-common-issues-reported-by-partners)
 - [Come inviare una richiesta di eccezione tecnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Elenco dei problemi comuni segnalati dai partner
Prima di applicare un'eccezione tecnica, esaminare l'elenco dei problemi comuni segnalati da altri partner per comprendere se sono motivi validi per le eccezioni tecniche.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: il partner necessita di più tempo per implementare l'autenticazione a più fattori per gli agenti partner
Un partner non è stato avviato o è ancora in fase di implementazione dell'autenticazione a più fattori per gli agenti partner che richiedono l'accesso ai portali di Microsoft Online Services mediante privilegi di amministrazione delegata del partner per gestire le risorse del cliente. Il partner necessita di più tempo per completare l'implementazione dell'autenticazione a più fattori. Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: No. Il partner deve pianificare l'implementazione dell'autenticazione a più fattori per gli utenti, in modo da evitare rotture.

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per i propri agenti partner, gli agenti partner possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministrazione delegata del partner purché possano completare la registrazione dell'autenticazione a più fattori Quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'autenticazione a più fattori.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: il partner non ha implementato l'autenticazione a più fattori per gli account utente che non usano privilegi amministrativi delegati
Un partner ha alcuni utenti dei tenant partner che non necessitano dell'accesso ai portali di Microsoft Online Services per gestire le risorse dei clienti usando i privilegi di amministrazione delegata del partner. Il partner è in fase di implementazione dell'autenticazione a più fattori per questi utenti e richiede più tempo per il completamento. Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministrazione delegata del partner per gestire le risorse dei clienti, non dovranno accedere al tenant del cliente. Non saranno interessati dalla Azure AD che richiede la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: il partner non ha implementato l'autenticazione a più fattori per gli account del servizio utente
Un partner ha alcuni account utente nei tenant partner usati dai dispositivi come account del servizio. Si tratta in genere di account con privilegi limitati che non richiedono Access partner Center né i portali di Microsoft Online Services per gestire le risorse dei clienti mediante privilegi di amministrazione delegata del partner. Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministrazione delegata del partner per gestire le risorse dei clienti, non dovranno accedere al tenant del cliente. Non saranno interessati dalla Azure AD che richiede la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: il partner non può implementare l'autenticazione a più fattori con l'app MS Authenticator
Un partner ha criteri di "pulizia" che non consentono ai dipendenti di portare i dispositivi mobili personali nell'area di lavoro. Senza accedere ai dispositivi mobili personali, i dipendenti non possono installare l'app MS Authenticator, che è l'unica verifica dell'autenticazione a più fattori supportata dai criteri di base Azure AD. Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: No, non è un motivo valido per un'eccezione tecnica. Il partner deve prendere in considerazione le alternative seguenti, in modo che i dipendenti possano comunque completare la verifica dell'autenticazione a più fattori quando accedono al centro
- Oltre all'app MS Authenticator, è possibile usare i criteri di Azure AD Baseline anche con l'app di autenticazione compatibile di terze parti, che può essere supportata da computer Windows che eseguono Microsoft Windows.
- Il partner può inoltre iscriversi a soluzioni di autenticazione a più fattori Azure AD Premium o di terze parti (compatibili con Azure AD) che possono fornire metodi di verifica aggiuntivi.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: il partner non può implementare l'autenticazione a più fattori a causa dell'uso di protocolli di autenticazione legacy
Un partner ha alcuni agenti partner che usano ancora protocolli di autenticazione legacy, che non sono compatibili con l'autenticazione A più fattori. Ad esempio, gli utenti usano ancora Outlook 2010, basato sui protocolli di autenticazione legacy. L'abilitazione dell'autenticazione a più fattori per questi agenti partner interferirà con i protocolli di autenticazione legacy.

**Risposta**: No, non è un motivo valido per un'eccezione tecnica. I partner sono vivamente invitati a uscire dall'uso di protocolli di autenticazione legacy a causa di potenziali implicazioni sulla sicurezza, perché questi protocolli non possono essere protetti con la verifica dell'autenticazione a più fattori e sono molto più vulnerabili alla compromissione delle credenziali. Se non è possibile evitare l'uso di protocolli di autenticazione legacy, i partner devono prendere in considerazione l'iscrizione a Azure AD Premium, che supporta l'uso delle password dell'applicazione. Le password dell'applicazione sono password di sistema generate una sola volta, che in genere sono più solide delle password generate dall'uomo. Usando le password dell'applicazione, i partner possono implementare l'autenticazione a più fattori per gli utenti, eseguendo il fallback alle password dell'applicazione solo per i protocolli di autenticazione legacy.

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per i propri agenti partner, gli agenti partner possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministrazione delegata del partner purché possano completare la registrazione dell'autenticazione a più fattori Quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'autenticazione a più fattori.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>Problema 6: il partner USA PowerShell di Exchange Online che non supporta l'autenticazione a più fattori
Un partner sta usando Exchange Online PowerShell con privilegi di amministrazione delegata del partner per gestire il servizio Exchange Online per conto dei clienti. PowerShell per Exchange Online non supporta l'autenticazione a più fattori. Se il partner implementa l'autenticazione a più fattori per gli utenti, questi utenti non saranno più in grado di accedere a Exchange Online PowerShell. Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: Sì, questo può essere considerato un motivo valido per un'eccezione tecnica. Il [modulo di PowerShell di Exchange Online esistente che supporta l'amministrazione delegata del partner](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) non richiede che l'utente partner abbia accesso al tenant del cliente e pertanto non è interessato da Azure ad che richiedono la verifica dell'autenticazione a più fattori. Tuttavia, non è compatibile con l'autenticazione a più fattori. Il team di Microsoft Exchange Online sta sviluppando un nuovo modulo di PowerShell che supporta i privilegi di amministrazione delegata partner e l'autenticazione a più fattori. Fino a quando non è disponibile il nuovo modulo PowerShell, i partner non possono implementare l'autenticazione a più fattori per gli utenti che devono usare il modulo di PowerShell esistente. Se si verificano problemi durante l'accesso ad altri Microsoft Online Services a causa di Azure AD richiedendo la verifica dell'autenticazione a più fattori durante l'accesso tra tenant, i partner possono richiedere un'eccezione tecnica per disattivare la verifica dell'autenticazione a più fattori.

> [!NOTE]
> Anche se il partner non è in grado di implementare l'autenticazione a più fattori per gli utenti che richiedono l'accesso al modulo di PowerShell per Exchange Online, questi utenti possono comunque accedere ai Microsoft Online Services per gestire le risorse dei clienti usando i privilegi di amministrazione delegata possono completare la registrazione dell'autenticazione a più fattori e la verifica dell'autenticazione a più fattori quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'utente per l'autenticazione a più fattori e pertanto non influisce sull'accesso al modulo PowerShell di Exchange Online

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>Problema 7: il partner ha implementato l'autenticazione a più fattori di terze parti che non viene riconosciuta da Azure AD
Un partner ha implementato l'autenticazione a più fattori per gli utenti usando una soluzione multi-factor authentication di terze parti Tuttavia, il partner non è in grado di configurare correttamente la soluzione multi-factor authentication di terze parti per inoltrare al Azure AD che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione Si tratta di un motivo valido per un'eccezione tecnica?

**Risposta**: Sì, questo può essere considerato un motivo valido per un'eccezione tecnica. Prima Azure AD di inviare una richiesta di eccezione tecnica, verificare con il provider di soluzioni multi-factor authentication di terze parti che la soluzione multi-factor authentication non può essere configurata in modo da trasmettere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*) per indicare che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione dell'utente. Quando si invia una richiesta di eccezione tecnica, fornire i dettagli della soluzione di autenticazione a più fattori di terze parti usata e indicare il metodo di integrazione (ad esempio, tramite la Federazione delle identità o l'uso di Azure AD controllo personalizzato).

### <a name="how-to-submit-a-request-for-technical-exception"></a>Come inviare una richiesta di eccezione tecnica

Per inviare una richiesta di eccezione tecnica:

1. Accedere al centro per i partner come amministratore globale o agente di amministrazione.
2. Per creare una nuova richiesta di servizio partner, passare a **supporto** > **richieste di supporto partner** e fare clic su **nuova richiesta**.
4. Nell'argomento autenticazione a più fattori **e modello di applicazione protetta** seleziona **Invia una richiesta di eccezione tecnica** come tipo di problema.
6. Specificare i dettagli richiesti per inviare una richiesta di servizio per eccezione tecnica e fare clic su **Invia**.

Microsoft può richiedere fino a 3 giorni lavorativi per fornire una risposta alla richiesta di eccezione tecnica.
