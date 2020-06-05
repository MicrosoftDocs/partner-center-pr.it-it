---
title: Imposizione MFA per il tenant partner
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descrive come l'imposizione dell'autenticazione a più fattori per i tenant del partner consente di proteggere l'accesso alle risorse dei clienti. Sono inclusi scenari di esempio.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9454e9410e4110fdf3542bde3696d8447d4c90d0
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998307"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Imposizione dell'autenticazione a più fattori per il tenant del partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti gli advisor

**Ruoli interessati**

- Agente amministratore
- Agente di vendita
- Agente di supporto tecnico
- Amministratore fatturazione
- Amministratore globale

Questa funzionalità consente ai partner di proteggere l'accesso alle risorse dei clienti da violazioni delle credenziali.
I partner sono tenuti ad applicare l'autenticazione a più fattori (MFA) per tutti gli account utente presenti nel loro tenant del partner, inclusi gli utenti guest. Con questa funzionalità, ai ruoli di partner verrà imposto di eseguire la verifica dell'autenticazione a più fattori per le aree seguenti:

- [Dashboard del Centro per i partner](#partner-center-dashboard) (a partire dal 1° maggio 2020)
- [API del Centro per i partner](#partner-center-api) (a partire dal 1° maggio 2020)
- [Amministrazione con delega del partner](#partner-delegated-administration)

Tra le nostre priorità principali vi è una maggiore e costante tutela della sicurezza e della privacy e continuiamo ad aiutare i partner a proteggere i loro clienti e tenant. Per essere conformi, tutti i partner che partecipano al programma Cloud Solution Provider (CSP), i fornitori di pannelli di controllo (CPV) e gli Advisor devono implementare i [requisiti di sicurezza dei partner](partner-security-requirements.md).

Microsoft ha avviato l'attivazione di misure di sicurezza aggiuntive per i tenant del partner. L'attivazione delle misure di sicurezza consente ai partner di proteggere i loro tenant e clienti imponendo la verifica dell'autenticazione a più fattori (MFA) per evitare accessi non autorizzati.

Abbiamo completato l'attivazione delle funzionalità di amministrazione con delega del partner per tutti i tenant del partner. Per proteggere ulteriormente partner e clienti, a partire dal 1° maggio 2020 avvieremo l'attivazione delle transazioni del Centro per i partner in CSP, aiutando i partner a proteggere le loro attività e i clienti da eventi imprevisti correlati al furto di identità.

Questa documentazione fornisce ai partner esperienza dettagliata e indicazioni per l'attivazione delle misure di sicurezza.

## <a name="partner-center-dashboard"></a>Dashboard del Centro per i partner

Alcune pagine nel dashboard del Centro per i partner verranno protette con l'autenticazione a più fattori, tra cui:

* Tutte le pagine incluse nella scheda **Clienti**, ad esempio tutte le pagine a cui è possibile accedere tramite l'URL seguente: https://partner.microsoft.com/commerce/*
* Tutte le pagine incluse nella scheda **Supporto > Richieste clienti**, ad esempio la pagina a cui è possibile accedere da https://partner.microsoft.com/dashboard/support/csp/customers/*
* Pagina di fatturazione

Se tenti di accedere a una di queste pagine senza aver prima completato la verifica dell'autenticazione a più fattori, ti verrà richiesto di eseguire questa operazione.

> [!NOTE]
> Altre pagine di Partner Center, ad esempio la pagina Panoramica o Stato di integrità dei servizi, non saranno protette dall'autenticazione a più fattori.

I tipi di utente seguenti sono autorizzati ad accedere a queste pagine protette dall'autenticazione a più fattori e sono quindi interessati da questa funzionalità.


| Pagine protette dall'autenticazione a più fattori       | Agenti amministratore      |  Agenti di vendita     |   Agenti help desk     | Amministratore globale      |  Amministratore fatturazione     | 
|---    |---    |---    |---    |---    |---    |
| Tutte le pagine nella scheda Clienti      |   x    |    x   |  x     |       |       |
| Tutte le pagine nella scheda Supporto > Richieste clienti     | x      |       |    x   |       |       |
| Pagina di fatturazione     |   x    |       |       |    x   |   x    |

**Esempi**

Per illustrare il funzionamento della verifica, prendi in considerazione i due esempi seguenti.

**Esempio 1: il partner ha implementato la soluzione di autenticazione a più fattori di Azure AD**
1.    Raffaella lavora per il Cloud Solution Provider Contoso. Contoso ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant del partner Contoso usando l'autenticazione a più fattori di Azure Active Directory (Azure AD).
2.    Raffaella avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Raffaella ad Azure AD per l'accesso.
3.    A causa della configurazione esistente dell'autenticazione a più fattori di Azure AD per Contoso, Raffaella deve completare la verifica dell'autenticazione a più fattori. Al completamento dell'accesso e della verifica dell'autenticazione a più fattori, Raffaella viene reindirizzata alla pagina di panoramica del dashboard Partner Center.
4.    Raffaella tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Poiché Raffaella ha già completato la verifica dell'autenticazione a più fattori durante l'accesso, può accedere alla pagina protetta dall'autenticazione a più fattori senza dover eseguire di nuovo la verifica.

**Esempio 2: il partner ha implementato una soluzione di autenticazione a più fattori di terze parti con la federazione delle identità**
1. Lorenzo lavora per il Cloud Solution Provider Wingtip. Wingtip ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant del partner Wingtip usando una soluzione di terze parti, integrata con Azure AD tramite la federazione delle identità.
2. Lorenzo avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Lorenzo ad Azure AD per l'accesso.
3. Poiché in Wingtip è stata impostata la federazione delle identità, Azure AD reindirizza Lorenzo al provider di identità federato per completare l'accesso e la verifica dell'autenticazione a più fattori. Al completamento dell'accesso e della verifica dell'autenticazione a più fattori, Lorenzo viene reindirizzato ad Azure AD e quindi alla pagina di panoramica del dashboard Partner Center.
4. Lorenzo tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Poiché Lorenzo ha già completato la verifica dell'autenticazione a più fattori durante l'accesso, può accedere alla pagina protetta dall'autenticazione a più fattori senza dover eseguire di nuovo la verifica.

**Esempio 3: il partner non ha implementato una soluzione di autenticazione a più fattori**
1. Davide lavora per il Cloud Solution Provider Fabrikam. Fabrikam non ha implementato una soluzione di autenticazione a più fattori per gli utenti del tenant del partner Fabrikam.
2. Davide avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Davide ad Azure AD per l'accesso.
3. Poiché Fabrikam non ha implementato l'autenticazione a più fattori, a Davide non viene richiesto di completare la verifica dell'autenticazione a più fattori. Al completamento dell'accesso, Davide viene reindirizzato alla pagina di panoramica del dashboard Partner Center.
4. Davide tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Dal momento che Davide non ha completato la verifica dell'autenticazione a più fattori, il Centro per i partner reindirizza Davide ad Azure AD per completare la verifica dell'autenticazione a più fattori. Poiché questa è la prima volta che a Davide viene richiesto di completare l'autenticazione a più fattori, deve effettuare anche la [registrazione per l'autenticazione a più fattori](#mfa-registration-experience). Al termine della registrazione e della verifica dell'autenticazione a più fattori, Davide può accedere alla pagina protetta dall'autenticazione a più fattori.
5. Un altro giorno prima che Fabrikam implementi l'autenticazione a più fattori per tutti gli utenti, Davide avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard Partner Center, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Davide ad Azure AD per l'accesso senza la richiesta dell'autenticazione a più fattori. 
6. Davide tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Dal momento che Davide non ha completato la verifica dell'autenticazione a più fattori, il Centro per i partner reindirizza Davide ad Azure AD per completare la verifica dell'autenticazione a più fattori. Poiché Davide ha effettuato la registrazione dell'autenticazione a più fattori, questa volta gli viene chiesto solo di eseguire la verifica dell'autenticazione a più fattori.

> [!NOTE]
>Azione: L'amministratore aziendale deve ora implementare l'autenticazione a più fattori tramite una delle [opzioni](partner-security-requirements.md#actions-that-you-need-to-take) suggerite da Partner Center.

## <a name="partner-center-api"></a>API del Centro per i partner

L'API del Centro per i partner supporta sia l'autenticazione basata solo su app che l'autenticazione app+utente. 

Quando si usa l'autenticazione app+utente, il Centro per i partner richiede la verifica dell'autenticazione a più fattori. In particolare, quando un'applicazione partner vuole inviare una richiesta API al Centro per i partner, deve includere un token di accesso nell'intestazione dell'autorizzazione della richiesta. 

> [!NOTE]
>Il [modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) è un framework sicuro e scalabile per l'autenticazione dei partner CSP e dei CPV attraverso l'architettura dell'autenticazione a più fattori di Microsoft Azure quando si chiama l'API di Partner Center. Devi implementare questo modello prima di abilitare l'autenticazione a più fattori nel tenant. 

Quando Partner Center riceve una richiesta API con un token di accesso ottenuto usando l'autenticazione app+utente, l'API di Partner Center verificherà la presenza del valore dell'*autenticazione a più fattori* nell'attestazione *Authentication Method Reference (AMR)* . Puoi usare un decodificatore JWT per verificare se un token di accesso contiene il valore di Authentication Method Reference previsto o meno:

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
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Se il valore è presente, il Centro per i partner conclude che la verifica dell'autenticazione a più fattori è stata completata ed elabora la richiesta dell'API. Se il valore non è presente, l'API del Centro per i partner rifiuterà la richiesta con la risposta seguente:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Quando viene usata l'autenticazione basata solo su app, le API che supportano questo tipo di autenticazione funzioneranno continuamente senza richiedere l'autenticazione a più fattori.

## <a name="partner-delegated-administration"></a>Amministrazione con delega del partner

### <a name="using-service-portals"></a>Uso dei portali di servizio

Gli account partner, inclusi gli agenti amministratore e gli agenti help desk, possono usare i propri privilegi di amministratore con delega del partner per gestire le risorse dei clienti tramite i portali di Microsoft Online Services, l'interfaccia della riga di comando e le API (usando l'autenticazione app+utente).

Quando si accede ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner (AOBO, Admin On Behalf Of) per gestire le risorse dei clienti, molti di questi portali richiedono che l'account partner esegua l'autenticazione interattiva, con il tenant Azure Active Directory del cliente impostato come contesto di autenticazione (l'account partner deve accedere al tenant del cliente).

Quando Azure Active Directory riceve tali richieste di autenticazione, richiede all'account partner di completare la verifica dell'autenticazione a più fattori. Esistono due possibili esperienze utente, a seconda che l'account partner sia un'identità gestita o federata:

- Se l'account partner è un'identità **gestita**, Azure Active Directory chiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è stato registrato in precedenza per l'autenticazione a più fattori con Azure Active Directory, all'utente verrà richiesto di [completare innanzitutto la registrazione dell'autenticazione a più fattori](#mfa-registration-experience).

- Se l'account partner è un'identità **federata**, l'esperienza dipende dalla modalità in cui l'amministratore partner ha configurato la federazione in Azure Active Directory. Quando si configura la federazione in Azure Active Directory, l'amministratore partner può indicare ad Azure Active Directory se il provider di identità federato supporta o meno l'autenticazione a più fattori. In tal caso, Azure Active Directory reindirizza l'utente al provider di identità federato per completare la verifica dell'autenticazione a più fattori. In caso contrario, Azure Active Directory chiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è stato registrato in precedenza per l'autenticazione a più fattori con Azure Active Directory, all'utente verrà richiesto di [completare innanzitutto la registrazione dell'autenticazione a più fattori](#mfa-registration-experience).

L'esperienza complessiva è simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato le [impostazioni predefinite per la sicurezza di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), che richiedono che tutti gli account con diritti amministrativi accedano al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti amministratore e gli agenti help desk. A scopo di test, i partner possono abilitare le [impostazioni predefinite per la sicurezza di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) nel tenant del cliente e quindi provare a usare i privilegi di amministratore con delega del partner per accedere al tenant del cliente.

> [!NOTE]
> Non tutti i portali di Microsoft Online Services richiedono che gli account partner accedano al tenant del cliente in caso di accesso alle risorse dei clienti tramite i privilegi di amministratore con delega del partner. Richiedono invece che gli account partner accedano al tenant del partner. Un esempio è l'interfaccia di amministrazione di Exchange. Si prevede che questi portali necessitino degli account partner per accedere al tenant del cliente quando usano i privilegi di amministratore con delega del partner.

### <a name="using-service-apis"></a>Uso delle API del servizio
Alcune API di Microsoft Online Services, ad esempio Azure Resource Manager, Azure AD Graph, Microsoft Graph e così via, supportano i partner tramite i privilegi di amministratore con delega del partner per gestire le risorse del cliente a livello di codice. Per sfruttare i vantaggi dei privilegi di amministratore con delega del partner con queste API, l'applicazione partner deve includere un token di accesso nell'intestazione di autorizzazione della richiesta API, in cui il token di accesso si ottiene con l'autenticazione di un account utente del partner con Azure AD, con il cliente Azure AD impostato come contesto di autenticazione. L'applicazione del partner deve avere le informazioni di accesso di un account utente partner al tenant del cliente.

Quando Azure AD riceve tali richieste di autenticazione, richiede all'account utente partner di completare la verifica dell'autenticazione a più fattori. Se l'account utente partner non è stato registrato in precedenza per l'autenticazione a più fattori, all'account utente verrà richiesto di completare innanzitutto la registrazione a più fattori.

Questa funzionalità interessa tutte le applicazioni partner integrate con queste API che usano i privilegi di amministratore con delega del partner. Per garantire che le applicazioni partner possano continuare a usare queste API senza interruzioni:

- Il partner deve evitare di usare un metodo di autenticazione utente non interattivo con Azure AD per ottenere il token di accesso. Se si usa un metodo di autenticazione utente non interattivo, ad esempio il [flusso della password](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure AD non sarà in grado di richiedere all'utente di completare la verifica dell'autenticazione a più fattori. Il partner deve invece passare all'uso di un metodo di autenticazione utente interattivo, ad esempio il [flusso di OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code).
- Durante il metodo di autenticazione utente interattivo, il partner deve usare un account utente partner già abilitato per l'autenticazione a più fattori. In alternativa, quando richiesto da Azure AD, il partner può completare la registrazione e la verifica dell'autenticazione a più fattori durante l'accesso.
- L'esperienza è simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato le [impostazioni predefinite per la sicurezza di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), che richiedono che tutti gli account utente con diritti amministrativi accedano al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti amministratore e gli agenti help desk. A scopo di test, i partner possono abilitare le [impostazioni predefinite per la sicurezza di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) nel tenant del cliente e quindi provare a usare i privilegi di amministratore con delega del partner per accedere al tenant del cliente a livello di codice.

### <a name="mfa-registration-experience"></a>Esperienza di registrazione con l'autenticazione a più fattori
Durante la verifica dell'autenticazione a più fattori, se l'account utente partner non è stato registrato in precedenza per l'autenticazione a più fattori, Azure AD richiede all'utente di completare innanzitutto la registrazione a più fattori:

![Registrazione all'autenticazione a più fattori - Passaggio 1](images/MfaRegistration1.png)

Dopo aver selezionato **Avanti**, l'utente dovrà scegliere un metodo di verifica da un elenco.

![Registrazione all'autenticazione a più fattori - Passaggio 2](images/MfaRegistration2.png)

Al termine della registrazione, l'utente dovrà completare la verifica dell'autenticazione a più fattori in base al metodo scelto dall'utente.



## <a name="request-for-technical-exception"></a>Richiesta per un'eccezione tecnica

I partner possono applicare un'eccezione tecnica per eliminare la verifica dell'autenticazione a più fattori se si riscontrano problemi tecnici con Microsoft Online Services e non sono presenti alternative o soluzioni praticabili. Prima di procedere, esamina le sezioni seguenti:

 - [Elenco dei problemi comuni segnalati dai partner](#list-of-common-issues-reported-by-partners)
 - [Come inviare una richiesta per un'eccezione tecnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Elenco di problemi comuni segnalati dai partner
Prima di applicare un'eccezione tecnica, esamina l'elenco dei problemi comuni segnalati da altri partner per comprendere se rappresentano motivi validi per un'eccezione tecnica.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: il partner necessita di più tempo per implementare l'autenticazione a più fattori per gli agenti del partner
Un partner non ha avviato o è ancora in fase di implementazione dell'autenticazione a più fattori per gli agenti del partner che richiedono l'accesso ai portali di Microsoft Online Services mediante privilegi di amministratore con delega del partner per gestire le risorse del cliente. Il partner necessita di più tempo per completare l'implementazione dell'autenticazione a più fattori. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Il partner deve pianificare l'implementazione dell'autenticazione a più fattori per gli utenti, in modo da evitare interruzioni.

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per gli agenti del partner, questi ultimi possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner purché possano completare la registrazione e la verifica dell'autenticazione a più fattori quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'utente per l'autenticazione a più fattori.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: il partner non ha implementato l'autenticazione a più fattori per gli account utente che non usano i privilegi di amministratore con delega
Un partner ha alcuni utenti nei tenant del partner che non richiedono l'accesso ai portali di Microsoft Online Services per gestire le risorse del cliente tramite i privilegi di amministratore con delega del partner. Il partner è in fase di implementazione dell'autenticazione a più fattori per questi utenti e necessita di più tempo per il completamento dell'operazione. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministratore con delega del partner per gestire le risorse del cliente, non verrà loro richiesto di accedere al tenant del cliente. Non saranno interessati dalla richiesta di Azure AD di eseguire la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: il partner non ha implementato l'autenticazione a più fattori per gli account del servizio utente
Un partner dispone di alcuni account utente nei tenant del partner, usati dai dispositivi come account del servizio. Si tratta di account con privilegi ridotti che non richiedono l'accesso al Centro per i partner o ai portali di Microsoft Online Services per gestire le risorse del cliente tramite i privilegi di amministratore con delega del partner. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministratore con delega del partner per gestire le risorse del cliente, non verrà loro richiesto di accedere al tenant del cliente. Non saranno interessati dalla richiesta di Azure AD di eseguire la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: il partner non può implementare l'autenticazione a più fattori con l'app Microsoft Authenticator
Un partner adotta la "politica della scrivania pulita", che non consente ai dipendenti di portare i dispositivi mobili personali nell'area di lavoro. Senza accesso ai dispositivi mobili personali, i dipendenti non possono installare l'app Microsoft Authenticator, che è l'unica verifica dell'autenticazione a più fattori supportata dalle impostazioni predefinite per la sicurezza di Azure AD. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: no, non è un motivo valido per un'eccezione tecnica. Il partner deve prendere in considerazione le alternative seguenti, in modo che i dipendenti possano comunque completare la verifica dell'autenticazione a più fattori quando accedono al Centro per i partner:
- Il partner può anche iscriversi ad Azure AD Premium o a soluzioni di autenticazione a più fattori di terze parti (compatibili con Azure AD) che possono fornire metodi di verifica aggiuntivi.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: il partner non può implementare l'autenticazione a più fattori a causa di protocolli di autenticazione legacy
Un partner ha alcuni agenti del partner che usano ancora protocolli di autenticazione legacy, che non sono compatibili con l'autenticazione a più fattori. Ad esempio, gli utenti usano ancora Outlook 2010 che si basa sui protocolli di autenticazione legacy. L'abilitazione dell'autenticazione a più fattori per questi agenti del partner interferirà con i protocolli di autenticazione legacy.

**Risposta**: no, non è un motivo valido per un'eccezione tecnica. I partner sono vivamente invitati a evitare l'uso di protocolli di autenticazione legacy a causa di potenziali implicazioni sulla sicurezza, poiché questi protocolli non possono essere protetti con la verifica dell'autenticazione a più fattori e sono maggiormente soggetti alla violazione delle credenziali. Se non è possibile evitare l'uso di protocolli di autenticazione legacy, i partner devono prendere in considerazione l'opportunità di iscriversi ad Azure AD Premium, che supporta l'uso delle password dell'applicazione. Le password dell'applicazione sono password di sistema generate una sola volta e sono solitamente più sicure delle password generate dagli utenti. Usando le password dell'applicazione, i partner possono implementare l'autenticazione a più fattori per gli utenti, facendo affidamento alle password dell'applicazione solo per i protocolli di autenticazione legacy.

Leggi il post su [autenticazione di base ed Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) per conoscere gli ultimi sviluppi relativi al supporto dell'autenticazione legacy per Outlook e segui il [blog del team Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) per ricevere le prossime notizie. 

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per gli agenti del partner, questi ultimi possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner purché possano completare la registrazione e la verifica dell'autenticazione a più fattori quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'utente per l'autenticazione a più fattori.

#### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problema 6: il partner ha implementato una soluzione di autenticazione a più fattori di terze parti non riconosciuta da Azure AD
Un partner ha implementato l'autenticazione a più fattori per gli utenti usando una soluzione di terze parti. Il partner non è tuttavia in grado di configurare correttamente la soluzione di autenticazione a più fattori di terze parti in modo da indicare ad Azure AD che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione dell'utente. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: sì, il problema può essere considerato un motivo valido per un'eccezione tecnica. Prima di inviare una richiesta di eccezione tecnica, verifica con il provider della soluzione di autenticazione a più fattori di terze parti che tale soluzione non possa essere configurata in modo da trasmettere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*) ad Azure AD per indicare che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione dell'utente. Quando invii una richiesta di eccezione tecnica, devi fornire i dettagli della soluzione di autenticazione a più fattori di terze parti usata e indicare il metodo di integrazione, ad esempio tramite la federazione delle identità o l'uso di Controllo personalizzato di Azure AD. Nella richiesta di eccezione tecnica devi inoltre fornire le informazioni seguenti come documenti di supporto:
* Configurazioni dell'autenticazione a più fattori di terze parti. 
* Risultato del [test dei requisiti di sicurezza dei partner](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) eseguito dall'account abilitato all'autenticazione a più fattori di terze parti.
* Ordine di acquisto della soluzione di autenticazione a più fattori di terze parti che stai usando o prevedi di usare.


### <a name="how-to-submit-a-request-for-technical-exception"></a>Come inviare una richiesta per un'eccezione tecnica

Per inviare una richiesta per un'eccezione tecnica:

1. Accedere al Centro per i partner come amministratore globale o agente amministratore.
2. Per creare una nuova richiesta di servizio del partner, passa a **Supporto** > **Richieste di supporto per i partner** e seleziona **Nuova richiesta**.
3. Cerca **MFA - Request for exception** (Autenticazione a più fattori - Richiesta di eccezione) nella casella di ricerca. In alternativa, seleziona **CSP** da Categoria, quindi **Accounts, Onboarding, Access** (Account, onboarding, accesso) da Argomento, **MFA - Request for exception** (Autenticazione a più fattori - Richiesta di eccezione) dall'argomento secondario e infine **Passaggio successivo**.
4. Specifica i dettagli richiesti per inviare una richiesta di servizio per un'eccezione tecnica e fai clic su **Invia**.

Microsoft può richiedere fino a tre giorni lavorativi per fornire una risposta alla richiesta per un'eccezione tecnica.
