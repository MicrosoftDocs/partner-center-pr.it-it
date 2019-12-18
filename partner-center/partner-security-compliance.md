---
title: Stato dei requisiti di sicurezza per i partner | Centro per i partner
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri i nuovi requisiti obbligatori che consentono di aumentare la sicurezza per gli advisor, i fornitori del pannello di controllo e i partner del programma Cloud Solution Provider.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, autenticazione a più fattori, modello di applicazione sicura, sicurezza
ms.localizationpriority: high
ms.openlocfilehash: 32b185452e8287678e6ae010b435e127bfcf54aa
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005010"
---
# <a name="partner-security-requirements-status"></a>Stato dei requisiti di sicurezza per i partner

**Si applica a**

- Tutti i partner nell'ambito del programma Cloud Solution Provider
  - Fatturazione diretta
  - Provider indiretto
  - Rivenditore indiretto
- Tutti i fornitori del pannello di controllo
- Tutti gli advisor

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente amministratore
-   Amministratore fatturazione
-   Amministratore dei partner MPN

Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti. Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli. Questo è il motivo per cui è necessario che tutti gli utenti nell'ecosistema agiscano e si assicurino di disporre di protezioni di sicurezza appropriate. Per garantire la sicurezza di partner e clienti, viene introdotto un set di requisiti di sicurezza obbligatori per gli advisor, i fornitori del pannello di controllo e i partner che partecipano al programma Cloud Solution Provider.

Dal 1° agosto 2019 tutti i partner sono tenuti a implementare l'autenticazione a più fattori per tutti gli utenti, inclusi gli account di servizio, nel tenant partner. Per informazioni più dettagliate sui nuovi criteri di sicurezza, vedi [Requisiti di sicurezza per i partner](partner-security-requirements.md).

L'obiettivo è che ogni utente sia sottoposto a un test MFA per ogni singola autenticazione. Questo risultato può essere ottenuto in uno dei modi seguenti:

- Implementazione di Azure AD Premium per fare in modo che l'autenticazione MFA venga applicata per ogni utente
- Implementazione delle [impostazioni predefinite per la sicurezza Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementazione di una soluzione di terze parti in modo che l'autenticazione MFA venga applicata per ogni utente

## <a name="partner-security-requirements-status"></a>Stato dei requisiti di sicurezza per i partner

Questo report può essere utile per verificare lo stato dei requisiti di sicurezza poiché consente di individuare i punti deboli. Il rilevamento viene aggiornato regolarmente.

>[!NOTE]
>Il report sullo stato dei requisiti di sicurezza per i partner è supportato solo nel Centro per i partner. Non è disponibile in Microsoft Cloud for US Government o Microsoft Cloud Germania. È fortemente consigliabile che tutti i partner che effettuano transazioni attraverso un cloud sovrano (21Vianet, governo statunitense e Germania) adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, non è necessario che questi partner soddisfino i nuovi requisiti di sicurezza con decorrenza a partire dal 1° agosto 2019. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

Ogni volta che i tuoi dipendenti accedono al Centro per i partner per lavorare oppure, tramite le API, ricevono o inviano dati attraverso il Centro per i partner, il loro stato di sicurezza viene testato e monitorato. Sono incluse nel rilevamento dello stato di sicurezza anche le tue applicazioni e tutte le applicazioni del fornitore del pannello di controllo. Lo stato visualizzato è relativo ai sette giorni precedenti.

## <a name="multi-factor-authentication-mfa-report"></a>Report sull'autenticazione a più fattori ("MFA")

Il report MFA del Centro per i partner offre informazioni dettagliate sull'implementazione dell'autenticazione MFA per partner fornendo due metriche basate sulle attività del Centro per i partner:

**Verifica MFA completata dagli utenti**

Questa metrica è correlata alle attività nel dashboard del Centro per i partner. Misura la percentuale di operazioni eseguite dagli utenti che hanno completato la verifica MFA. Ad esempio:

- Contoso è un partner CSP con due agenti di amministrazione, Jane e John.
- Il primo giorno Jane ha eseguito l'accesso al dashboard del Centro per i partner senza verifica MFA e ha effettuato tre operazioni.
- Il secondo giorno John ha eseguito l'accesso al dashboard del Centro per i partner senza verifica MFA e ha effettuato cinque operazioni.
- Il terzo giorno Jane ha eseguito l'accesso al dashboard del Centro per i partner con verifica MFA e ha effettuato due operazioni.
- Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.
- Delle dieci operazioni effettuate nella finestra di sette giorni, sue sono state effettuate dall'utente con verifica MFA. Di conseguenza, la metrica indica il 20%.

**Autenticazione app+utente**

Questa metrica è correlata all'uso di richieste API del Centro per i partner effettuate con l'autenticazione app+utente. Misura la percentuale di richieste API effettuate usando un token di accesso con attestazione MFA. Ad esempio:

- Fabrikam è un partner CSP che dispone di un'applicazione CSP che usa una combinazione di autenticazione app+utente e di metodi di autenticazione basati solo su app.
- Il primo giorno l'applicazione ha effettuato tre richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente senza verifica MFA.
- Il secondo giorno l'applicazione ha effettuato cinque richieste API supportate da un token di accesso ottenuto usando l'autenticazione basata solo su app.
- Il terzo giorno l'applicazione ha effettuato due richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente con verifica MFA.
- Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.
- Le cinque richieste API nel secondo giorno supportate da un token di accesso ottenuto tramite l'autenticazione basata solo su app vengono omesse dalla metrica perché non usano le credenziali utente. Delle cinque operazioni rimanenti, due sono state supportate da un token di accesso ottenuto con la verifica MFA. Di conseguenza, la metrica indica il 40%.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Come procedere se le metriche nel report MFA non sono pari al 100%

È possibile che le metriche nel report MFA del Centro per i partner non siano pari al 100% per i partner che hanno implementato l'autenticazione MFA. Per capire perché, di seguito sono riportati alcuni fattori di cui tenere conto.

> [!NOTE]
> Dovrai collaborare con una persona dell'organizzazione che abbia familiarità con la gestione delle identità e l'implementazione dell'autenticazione MFA per il tenant partner.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Hai implementato l'autenticazione MFA per il tenant partner?

In caso negativo, devi prima effettuare questa operazione. Per informazioni dettagliate su come implementare l'autenticazione MFA, vedi l'articolo [Requisiti di sicurezza per i partner](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Hai completato l'implementazione dell'autenticazione MFA solo di recente?

Le metriche vengono calcolate su base giornaliera e prendono in considerazione le operazioni eseguite negli ultimi sette giorni. Se hai completato l'implementazione dell'autenticazione per il tenant partner solo di recente, è possibile che le metriche non siano pari al 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Alcuni account utente sono stati esclusi dall'implementazione dell'autenticazione MFA?

Verifica se l'implementazione dell'autenticazione MFA corrente copre tutti gli account utente o solo alcuni. Alcune soluzioni MFA sono basate su criteri e supportano l'esclusione degli utenti, mentre altre potrebbero richiedere l'abilitazione esplicita dell'autenticazione MFA in base ai singoli utenti. Verifica di non aver escluso alcun utente dall'implementazione MFA corrente. Eventuali account utente esclusi che eseguono l'accesso al Centro per i partner per eseguire un'attività correlata a CSP possono causare il mancato raggiungimento del 100% nelle metriche.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>L'autenticazione MFA è necessaria solo se vengono soddisfatte determinate condizioni?

Verifica se l'implementazione corrente applica l'autenticazione MFA solo in condizioni specifiche. Alcune soluzioni MFA presentano caratteristiche di flessibilità e consentono di applicare l'autenticazione MFA solo quando vengono soddisfatte determinate condizioni, ad esempio un utente che accede da un dispositivo o da una posizione sconosciuta. Un utente che è abilitato per l'autenticazione MFA, ma non è tenuto a completare la verifica MFA quando accede al Centro per i partner, può causare il mancato raggiungimento del 100% nelle metriche.

>[!NOTE]
>Per i partner che hanno implementato l'autenticazione MFA usando le impostazioni predefinite per la sicurezza Azure AD, è importante tenere presente che per gli account utente non di tipo amministratore verrà imposta l'autenticazione a più fattori in base al rischio. Agli utenti verrà chiesto di eseguire l'autenticazione MFA solo durante tentativi di accesso a rischio (ad esempio per l'accesso da una località diversa). Inoltre, gli utenti dispongono di un periodo massimo di 14 giorni per la registrazione per l'autenticazione MFA. Agli utenti che non hanno completato la registrazione MFA non verrà richiesta la verifica MFA durante il periodo di 14 giorni. È previsto pertanto che le metriche non siano pari al 100% per i partner che hanno implementato l'autenticazione MFA usando le impostazioni predefinite per la sicurezza Azure AD.

### <a name="are-you-using-3rd-party-mfa-solution"></a>Usi una soluzione MFA di terze parti?

Se usi una soluzione MFA di terze parti, verifica come integrarla con Azure AD. In generale, sono disponibili due metodi, tra cui la federazione e i controlli personalizzati:

* **Federazione delle identità**: quando riceve una richiesta di autenticazione, Azure AD reindirizza l'utente al provider di identità federato per l'autenticazione. Al completamento dell'autenticazione, il provider di identità federato reindirizza di nuovo l'utente ad Azure AD insieme a un token SAML. Affinché Azure AD riconosca che l'utente ha completato la verifica MFA durante l'autenticazione al provider di identità federato, il token SAML deve includere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*). Controlla se il provider di identità federato supporta il rilascio di tale attestazione. In tal caso, verifica che il provider di identità federato sia stato configurato per questa operazione. Se l'attestazione non è presente, Azure AD (e quindi il Centro per i partner) non saprà che l'utente ha completato la verifica MFA con il conseguente mancato raggiungimento del 100% nella metrica.

* **Controllo personalizzato**: non è possibile usare Controllo personalizzato di Azure AD per determinare se un utente ha completato la verifica MFA tramite una soluzione MFA di terze parti. Di conseguenza, tutti gli utenti che hanno completato la verifica MFA tramite un controllo personalizzato verranno sempre considerati da Azure AD e, a sua volta, dal Centro per i partner come utenti che non hanno completato la verifica MFA. Se possibile, è consigliabile passare all'uso della Federazione delle identità anziché di un controllo personalizzato durante l'integrazione con Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identificare gli utenti che hanno effettuato l'accesso al Centro per i partner senza MFA

Può essere utile identificare gli utenti che accedono al Centro per i partner senza verifica MFA e verificarli a fronte della tua implementazione MFA corrente. Per verificare se un utente ha completato o meno la verifica MFA, puoi usare il [report con le informazioni di accesso Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins). Il report con le informazioni di accesso Azure AD è attualmente disponibile solo per i partner che hanno sottoscritto Azure AD Premium o qualsiasi SKU O365 che includa Azure AD Premium, ad esempio EMS.

**Per altre informazioni**

- [Community del gruppo di linee guida per la sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisiti di sicurezza del Centro per i partner](partner-security-requirements.md)
- [Domande frequenti sui requisiti di sicurezza del Centro per i partner](partner-security-requirements-faq.md)
