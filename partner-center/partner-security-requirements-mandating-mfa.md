---
title: Imposizione dell'autenticazione a più fattori per il tenant partner
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descrive come l'imposizione dell'autenticazione a più fattori per i tenant del partner consente di proteggere l'accesso alle risorse dei clienti. Sono inclusi scenari di esempio.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b1b02967209ba36088b0c7bb7487428ab08b8a37
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152580"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Imposizione dell'autenticazione a più fattori per il tenant partner

**Ruoli appropriati:** Agente di amministrazione | Agente di vendita | Supporto dell'agente | Gestione della fatturazione | Amministratore globale

Questo articolo fornisce esempi dettagliati e istruzioni per l'imposizione dell'autenticazione a più fattori (MFA) nel Centro per i partner. Questa funzionalità consente ai partner di proteggere l'accesso alle risorse dei clienti da violazioni delle credenziali. I partner sono tenuti ad applicare l'autenticazione a più fattori per tutti gli account utente esistenti nel tenant partner, inclusi gli utenti guest. Agli utenti verrà imposto di completare la verifica dell'autenticazione a più fattori per le aree seguenti:

- [Dashboard Centro per i partner](#partner-center-dashboard)
- [API del Centro per i partner](#partner-center-api)
- [Amministrazione con delega del partner](#partner-delegated-administration)

Tra le nostre priorità principali vi è una maggiore e costante tutela della sicurezza e della privacy e continuiamo ad aiutare i partner a proteggere i loro clienti e tenant. Per essere conformi, tutti i partner che partecipano al programma Cloud Solution Provider (CSP), i fornitori di pannelli di controllo (CPV) e gli advisor devono implementare i [requisiti di sicurezza dei partner](partner-security-requirements.md).

Per aiutare i partner a proteggere clienti e attività da furti di identità e accessi non autorizzati, sono state attivate misure di sicurezza aggiuntive per i tenant partner che richiedono e verificano l'autenticazione a più fattori. 

## <a name="partner-center-dashboard"></a>Dashboard del Centro per i partner

Alcune pagine nel dashboard del Centro per i partner verranno protette con l'autenticazione a più fattori, tra cui:

- Tutte le pagine incluse nella scheda **Clienti**, ad esempio tutte le pagine a cui è possibile accedere tramite l'URL seguente: https://partner.microsoft.com/commerce/*
- Tutte le pagine incluse nella scheda **Supporto > Richieste clienti**, ad esempio la pagina a cui è possibile accedere da https://partner.microsoft.com/dashboard/support/csp/customers/*
- Pagina di fatturazione

La tabella seguente mostra i tipi di utente autorizzati ad accedere alle pagine protette dall'autenticazione a più fattori e quindi interessati da questa funzionalità.


| Pagine protette dall'autenticazione a più fattori       | Agenti amministratore      |  Agenti di vendita     |   Agenti help desk     | Amministratore globale      |  Amministratore fatturazione     | 
|---    |---    |---    |---    |---    |---    |
| Tutte le pagine nella scheda Clienti      |   x    |    x   |  x     |       |       |
| Tutte le pagine nella scheda Supporto > Richieste clienti     | x      |       |    x   |       |       |
| Pagina di fatturazione     |   x    |       |       |    x   |   x    |

Se tenti di accedere a una di queste pagine senza aver prima completato la verifica dell'autenticazione a più fattori, ti verrà richiesto di eseguire questa operazione. Per altre pagine del Centro per i partner, ad esempio la pagina Panoramica o Stato di integrità dei servizi, non è necessaria l'autenticazione a più fattori.

## <a name="verification-examples"></a>Esempi di verifica

Per illustrare il funzionamento della verifica nel dashboard Centro per i partner, prendere in considerazione gli esempi seguenti.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Esempio 1: il partner ha implementato la soluzione di autenticazione a più fattori di Azure AD

1. Raffaella lavora per il Cloud Solution Provider Contoso. Contoso ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant partner Contoso usando l'autenticazione a più fattori di Azure Active Directory (Azure AD).

2. Raffaella avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Raffaella ad Azure AD per l'accesso.

3. A causa della configurazione esistente dell'autenticazione a più fattori di Azure AD per Contoso, Raffaella deve completare la verifica dell'autenticazione a più fattori. Al termine della verifica dell'accesso e dell'autenticazione a più fattori, Jane viene reindirizzata alla pagina Partner Center panoramica del dashboard.

4. Raffaella tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Poiché Raffaella ha già completato la verifica dell'autenticazione a più fattori durante l'accesso, può accedere alla pagina protetta dall'autenticazione a più fattori senza dover eseguire di nuovo la verifica.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Esempio 2: il partner ha implementato una soluzione di autenticazione a più fattori di terze parti con la federazione delle identità

1. Lorenzo lavora per il Cloud Solution Provider Wingtip. Wingtip ha implementato l'autenticazione a più fattori per tutti gli utenti nel tenant del partner Wingtip usando una soluzione di terze parti, integrata con Azure AD tramite la federazione delle identità.

2. Lorenzo avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Lorenzo ad Azure AD per l'accesso.

3. Poiché in Wingtip è stata impostata la federazione delle identità, Azure AD reindirizza Lorenzo al provider di identità federato per completare l'accesso e la verifica dell'autenticazione a più fattori. Al termine della verifica dell'accesso e dell'autenticazione a più fattori, Viene reindirizzato a Azure AD e quindi alla pagina Partner Center panoramica del dashboard.

4. Lorenzo tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Poiché Lorenzo ha già completato la verifica dell'autenticazione a più fattori durante l'accesso, può accedere alla pagina protetta dall'autenticazione a più fattori senza dover eseguire di nuovo la verifica.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Esempio 3: il partner non ha implementato una soluzione di autenticazione a più fattori

1. Davide lavora per il Cloud Solution Provider Fabrikam. Fabrikam non ha implementato una soluzione di autenticazione a più fattori per gli utenti del tenant del partner Fabrikam.

2. Davide avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard del Centro per i partner, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Davide ad Azure AD per l'accesso.

3. Poiché Fabrikam non ha implementato l'autenticazione a più fattori, a Davide non viene richiesto di completare la verifica dell'autenticazione a più fattori. Al completamento dell'accesso, John viene reindirizzato alla Partner Center panoramica del dashboard.

4. Davide tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Dal momento che Davide non ha completato la verifica dell'autenticazione a più fattori, il Centro per i partner reindirizza Davide ad Azure AD per completare la verifica dell'autenticazione a più fattori. Poiché questa è la prima volta che a Davide viene richiesto di completare l'autenticazione a più fattori, deve effettuare anche la [registrazione per l'autenticazione a più fattori](#mfa-registration-experience). Al termine della registrazione e della verifica dell'autenticazione a più fattori, Davide può accedere alla pagina protetta dall'autenticazione a più fattori.

5. Un altro giorno prima che Fabrikam implementi l'autenticazione a più fattori per tutti gli utenti, Davide avvia una nuova sessione del browser e passa alla pagina di panoramica del dashboard Partner Center, che non è protetta dall'autenticazione a più fattori. Partner Center reindirizza Davide ad Azure AD per l'accesso senza la richiesta dell'autenticazione a più fattori. 

6. Davide tenta di accedere a una delle pagine protette con l'autenticazione a più fattori nel Centro per i partner. Dal momento che Davide non ha completato la verifica dell'autenticazione a più fattori, il Centro per i partner reindirizza Davide ad Azure AD per completare la verifica dell'autenticazione a più fattori. Poiché Davide ha effettuato la registrazione dell'autenticazione a più fattori, questa volta gli viene chiesto solo di eseguire la verifica dell'autenticazione a più fattori.

> [!NOTE]
>Azione: gli amministratori della società hanno [tre opzioni](partner-security-requirements.md#implementing-multi-factor-authentication) per l'implementazione dell'autenticazione a più fattori.

## <a name="partner-center-api"></a>API del Centro per i partner

L'API del Centro per i partner supporta sia l'autenticazione basata solo su app che l'autenticazione app+utente. 

Quando si usa l'autenticazione app+utente, il Centro per i partner richiede la verifica dell'autenticazione a più fattori. In particolare, quando un'applicazione partner vuole inviare una richiesta API al Centro per i partner, deve includere un token di accesso nell'intestazione dell'autorizzazione della richiesta. 

> [!NOTE]
>Il [modello di applicazione sicura](/partner-center/develop/enable-secure-app-model) è un framework scalabile per l'autenticazione dei partner CSP e dei CPV attraverso l'architettura dell'autenticazione a più fattori di Microsoft Azure quando si chiamano le API del Centro per i partner. È necessario implementare questo framework prima di abilitare l'autenticazione a più fattori nel tenant. 

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

Quando App-Only viene usata l'autenticazione a più fattori, le API che supportano App-Only'autenticazione a più fattori funzionano continuamente senza richiedere l'autenticazione a più fattori.

## <a name="partner-delegated-administration"></a>Amministrazione con delega del partner

Gli account partner, inclusi gli agenti amministratore e gli agenti help desk, possono usare i propri privilegi di amministratore con delega del partner per gestire le risorse dei clienti tramite i portali di Microsoft Online Services, l'interfaccia della riga di comando e le API (usando l'autenticazione app+utente).

### <a name="using-service-portals"></a>Uso dei portali di servizio

Quando si accede ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner (AOBO, Admin On Behalf Of) per gestire le risorse dei clienti, molti di questi portali richiedono che l'account partner esegua l'autenticazione interattiva, con il tenant Azure AD del cliente impostato come contesto di autenticazione (l'account partner deve accedere al tenant del cliente).

Quando Azure AD riceve tali richieste di autenticazione, richiede all'account partner di completare la verifica dell'autenticazione a più fattori. Esistono due possibili esperienze utente, a seconda che l'account partner sia un'identità gestita o federata:

- Se l'account partner è un'identità **gestita**, Azure AD chiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è stato registrato in precedenza per l'autenticazione a più fattori con Azure AD, all'utente verrà chiesto di [completare prima la registrazione per l'autenticazione a più fattori](#mfa-registration-experience).

- Se l'account partner è un'identità **federata**, l'esperienza dipende dalla modalità con cui l'amministratore partner ha configurato la federazione in Azure AD. Quando si configura la federazione in Azure AD, l'amministratore partner può indicare ad Azure AD se il provider di identità federato supporta o meno l'autenticazione a più fattori. In caso positivo, Azure AD reindirizza l'utente al provider di identità federato per completare la verifica dell'autenticazione a più fattori. In caso contrario, Azure AD richiederà direttamente all'utente di completare la verifica dell'autenticazione a più fattori. Se l'account partner non è stato registrato in precedenza per l'autenticazione a più fattori con Azure AD, all'utente verrà chiesto di [completare prima la registrazione per l'autenticazione a più fattori](#mfa-registration-experience).

L'esperienza complessiva è simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato le [impostazioni predefinite per la sicurezza di Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), che richiedono che tutti gli account con diritti amministrativi accedano al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti amministratore e gli agenti help desk. A scopo di test, i partner possono abilitare le [impostazioni predefinite per la sicurezza di Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) nel tenant del cliente e quindi provare a usare i privilegi di amministratore con delega del partner per accedere al tenant del cliente.

> [!NOTE]
> Non tutti i portali di Microsoft Online Services richiedono che gli account partner accedano al tenant del cliente in caso di accesso alle risorse dei clienti tramite i privilegi di amministratore con delega del partner. Richiedono invece che gli account partner accedano al tenant del partner. Un esempio è l'interfaccia di amministrazione di Exchange. Si prevede che questi portali necessitino degli account partner per accedere al tenant del cliente quando usano i privilegi di amministratore con delega del partner.

### <a name="using-service-apis"></a>Uso delle API del servizio

Alcune API di Microsoft Online Services, ad esempio Azure Resource Manager, Azure AD Graph, Microsoft Graph e così via, supportano i partner tramite i privilegi di amministratore con delega del partner per gestire le risorse del cliente a livello di codice. Per usare i privilegi di amministratore con delega partner con queste API, l'applicazione partner deve includere un token di accesso nell'intestazione di autorizzazione della richiesta API, in cui il token di accesso viene ottenuto con un account utente partner per l'autenticazione con Azure AD, con il Azure AD del cliente impostato come contesto di autenticazione. L'applicazione del partner deve avere le informazioni di accesso di un account utente partner al tenant del cliente.

Quando Azure AD riceve tali richieste di autenticazione, richiede all'account utente partner di completare la verifica dell'autenticazione a più fattori. Se l'account utente partner non è stato registrato in precedenza per l'autenticazione a più fattori, all'account utente verrà richiesto di completare innanzitutto la registrazione a più fattori.

Questa funzionalità interessa tutte le applicazioni partner integrate con queste API che usano i privilegi di amministratore con delega del partner. Per garantire che le applicazioni partner possano continuare a usare queste API senza interruzioni:

- Il partner deve evitare di usare un metodo di autenticazione utente non interattivo con Azure AD per ottenere il token di accesso. Se si usa un metodo di autenticazione utente non interattivo, ad esempio il [flusso della password](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure AD non sarà in grado di richiedere all'utente di completare la verifica dell'autenticazione a più fattori. Il partner deve invece passare all'uso di un metodo di autenticazione utente interattivo, ad esempio il [flusso di OpenID Connect](/azure/active-directory/develop/v1-protocols-openid-connect-code).

- Durante il metodo di autenticazione utente interattivo, il partner deve usare un account utente partner già abilitato per l'autenticazione a più fattori. In alternativa, quando richiesto da Azure AD, il partner può completare la registrazione e la verifica dell'autenticazione a più fattori durante l'accesso.

- L'esperienza è simile allo scenario in cui un tenant del cliente finale ha implementato l'autenticazione a più fattori per gli amministratori. Ad esempio, il tenant del cliente ha abilitato le [impostazioni predefinite per la sicurezza di Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), che richiedono che tutti gli account utente con diritti amministrativi accedano al tenant del cliente con la verifica dell'autenticazione a più fattori, inclusi gli agenti amministratore e gli agenti help desk. A scopo di test, i partner possono abilitare le [impostazioni predefinite per la sicurezza di Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) nel tenant del cliente e quindi provare a usare i privilegi di amministratore con delega del partner per accedere al tenant del cliente a livello di codice.

### <a name="mfa-registration-experience"></a>Esperienza di registrazione con l'autenticazione a più fattori

Durante la verifica dell'autenticazione a più fattori, se l'account utente partner non è stato registrato in precedenza per l'autenticazione a più fattori, Azure AD richiede all'utente di completare innanzitutto la registrazione a più fattori:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Registrazione all'autenticazione a più fattori - Passaggio 1":::

Dopo aver selezionato **Avanti**, l'utente dovrà scegliere un metodo di verifica da un elenco.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Registrazione all'autenticazione a più fattori - Passaggio 2":::

Al termine della registrazione, l'utente dovrà completare la verifica dell'autenticazione a più fattori in base al metodo scelto dall'utente.
 
## <a name="list-of-common-issues"></a>Elenco di problemi comuni

Prima di richiedere un'[eccezione tecnica](#how-to-submit-a-request-for-technical-exception) rispetto al requisito di autenticazione a più fattori, esaminare l'elenco dei problemi comuni segnalati da altri partner per stabilire se la richiesta è valida.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: il partner necessita di più tempo per implementare l'autenticazione a più fattori per gli agenti del partner
Un partner non ha avviato o è ancora in fase di implementazione dell'autenticazione a più fattori per gli agenti del partner che richiedono l'accesso ai portali di Microsoft Online Services mediante privilegi di amministratore con delega del partner per gestire le risorse del cliente. Il partner necessita di più tempo per completare l'implementazione dell'autenticazione a più fattori. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Il partner deve pianificare l'implementazione dell'autenticazione a più fattori per gli utenti, in modo da evitare interruzioni.

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per gli agenti del partner, questi ultimi possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner purché possano completare la registrazione e la verifica dell'autenticazione a più fattori quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'utente per l'autenticazione a più fattori.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: il partner non ha implementato l'autenticazione a più fattori per gli account utente che non usano i privilegi di amministratore con delega
Un partner ha alcuni utenti nei tenant del partner che non richiedono l'accesso ai portali di Microsoft Online Services per gestire le risorse del cliente tramite i privilegi di amministratore con delega del partner. Il partner è in fase di implementazione dell'autenticazione a più fattori per questi utenti e necessita di più tempo per il completamento dell'operazione. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministratore con delega del partner per gestire le risorse del cliente, non verrà loro richiesto di accedere al tenant del cliente. Non saranno interessati dalla richiesta di Azure AD di eseguire la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: il partner non ha implementato l'autenticazione a più fattori per gli account del servizio utente
Un partner dispone di alcuni account utente nei tenant del partner, usati dai dispositivi come account del servizio. Si tratta di account con privilegi bassi che non richiedono l'accesso Partner Center portali di Microsoft Online Services per gestire le risorse dei clienti usando i privilegi di amministrazione delegata dei partner. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: No. Poiché questi account utente non usano i privilegi di amministratore con delega del partner per gestire le risorse del cliente, non verrà loro richiesto di accedere al tenant del cliente. Non saranno interessati dalla richiesta di Azure AD di eseguire la verifica dell'autenticazione a più fattori durante l'accesso al tenant del cliente.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: il partner non può implementare l'autenticazione a più fattori con l'app Microsoft Authenticator
Un partner adotta la "politica della scrivania pulita", che non consente ai dipendenti di portare i dispositivi mobili personali nell'area di lavoro. Senza accesso ai dispositivi mobili personali, i dipendenti non possono installare l'app Microsoft Authenticator, che è l'unica verifica dell'autenticazione a più fattori supportata dalle impostazioni predefinite per la sicurezza di Azure AD. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: no, non è un motivo valido per un'eccezione tecnica. Il partner deve prendere in considerazione le alternative seguenti, in modo che i dipendenti possano comunque completare la verifica dell'autenticazione a più fattori quando accedono al Centro per i partner:
- Il partner può anche iscriversi ad Azure AD Premium o a soluzioni di autenticazione a più fattori di terze parti (compatibili con Azure AD) che possono fornire metodi di verifica aggiuntivi.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: il partner non può implementare l'autenticazione a più fattori a causa di protocolli di autenticazione legacy
Un partner ha alcuni agenti del partner che usano ancora protocolli di autenticazione legacy, che non sono compatibili con l'autenticazione a più fattori. Ad esempio, gli utenti usano ancora Outlook 2010 che si basa sui protocolli di autenticazione legacy. L'abilitazione dell'autenticazione a più fattori per questi agenti del partner interferirà con i protocolli di autenticazione legacy.

**Risposta**: no, non è un motivo valido per un'eccezione tecnica. I partner sono vivamente invitati a evitare l'uso di protocolli di autenticazione legacy a causa di potenziali implicazioni sulla sicurezza, poiché questi protocolli non possono essere protetti con la verifica dell'autenticazione a più fattori e sono maggiormente soggetti alla violazione delle credenziali. Se non è possibile evitare l'uso di protocolli di autenticazione legacy, i partner devono prendere in considerazione l'opportunità di iscriversi ad Azure AD Premium, che supporta l'uso delle password dell'applicazione. Le password dell'applicazione sono password di sistema generate una sola volta e sono solitamente più sicure delle password generate dagli utenti. Usando le password dell'applicazione, i partner possono implementare l'autenticazione a più fattori per gli utenti, facendo affidamento alle password dell'applicazione solo per i protocolli di autenticazione legacy.

Leggi il post su [autenticazione di base ed Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) per conoscere gli ultimi sviluppi relativi al supporto dell'autenticazione legacy per Outlook e segui il [blog del team Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) per ricevere le prossime notizie. 

> [!NOTE]
> Anche se il partner non ha implementato l'autenticazione a più fattori per gli agenti del partner, questi ultimi possono comunque accedere ai portali di Microsoft Online Services usando i privilegi di amministratore con delega del partner purché possano completare la registrazione e la verifica dell'autenticazione a più fattori quando richiesto durante l'accesso al tenant del cliente. Il completamento della registrazione dell'autenticazione a più fattori non abilita automaticamente l'utente per l'autenticazione a più fattori.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problema 6: il partner ha implementato una soluzione di autenticazione a più fattori di terze parti non riconosciuta da Azure AD
Un partner ha implementato l'autenticazione a più fattori per gli utenti usando una soluzione di terze parti. Il partner non è tuttavia in grado di configurare correttamente la soluzione di autenticazione a più fattori di terze parti in modo da indicare ad Azure AD che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione dell'utente. Questo problema rappresenta un motivo valido per un'eccezione tecnica?

**Risposta**: sì, il problema può essere considerato un motivo valido per un'eccezione tecnica. Prima di inviare una richiesta di eccezione tecnica, verifica con il provider della soluzione di autenticazione a più fattori di terze parti che tale soluzione non possa essere configurata in modo da trasmettere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*) ad Azure AD per indicare che la verifica dell'autenticazione a più fattori è stata completata durante l'autenticazione dell'utente. Quando invii una richiesta di eccezione tecnica, devi fornire i dettagli della soluzione di autenticazione a più fattori di terze parti usata e indicare il metodo di integrazione, ad esempio tramite la federazione delle identità o l'uso di Controllo personalizzato di Azure AD. Nella richiesta di eccezione tecnica devi inoltre fornire le informazioni seguenti come documenti di supporto:

- Configurazioni dell'autenticazione a più fattori di terze parti.

- Risultato del [test dei requisiti di sicurezza dei partner](/powershell/partnercenter/test-partner-security-requirements) eseguito dall'account abilitato all'autenticazione a più fattori di terze parti.

- Ordine di acquisto della soluzione di autenticazione a più fattori di terze parti che stai usando o prevedi di usare.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Come inviare una richiesta per un'eccezione tecnica

I partner possono applicare un'eccezione tecnica per eliminare la verifica dell'autenticazione a più fattori se si riscontrano problemi tecnici con Microsoft Online Services e non sono presenti alternative o soluzioni praticabili. Prima di procedere, esaminare l'[elenco dei problemi comuni](#list-of-common-issues) nella sezione precedente.

Per inviare una richiesta per un'eccezione tecnica:

1. Accedere a Partner Center come amministratore globale o agente amministratore.

2. Creare una nuova richiesta di servizio partner passando **a** Richieste di supporto partner  >  **e** selezionando **Nuova richiesta.**

3. Cercare **MFA - Richiesta di eccezione** nella casella di ricerca. oppure selezionare **CSP** da Categoria, quindi selezionare **Account, Onboarding,** Accesso da argomento, quindi selezionare **MFA - Richiesta** di eccezione nell'argomento secondario, quindi selezionare **il passaggio successivo.**

4. Specificare i dettagli richiesti per inviare una richiesta di servizio per l'eccezione tecnica e selezionare **Invia**.

Microsoft può impiegare fino a tre giorni lavorativi per fornire una risposta a una richiesta relativa a un'eccezione tecnica.

## <a name="next-steps"></a>Passaggi successivi

 - [Stato dei requisiti di sicurezza per i partner](partner-security-compliance.md)