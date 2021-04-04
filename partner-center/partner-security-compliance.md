---
title: Report di stato dei requisiti di sicurezza
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come verificare la conformità ai requisiti di sicurezza con il report di stato dei requisiti di sicurezza e il report di autenticazione a più fattori del Centro per i partner
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086550"
---
# <a name="security-requirements-status-report"></a>Report di stato dei requisiti di sicurezza

**Ruoli appropriati**
- Amministratore CPV
- Amministratore globale

Questo articolo descrive il report di stato dei requisiti di sicurezza disponibile nel Centro per i partner. Questo report fornisce le metriche sulla conformità ai [requisiti di sicurezza dei partner](partner-security-requirements.md) per multi-factor authentication per gli utenti nel tenant partner.

Per accedere a questo report nel centro per i [partner](https://partner.microsoft.com/dashboard), passare a **Impostazioni**  >  **account impostazioni** di  >  **sicurezza stato dei requisiti**. Il report viene aggiornato ogni giorno e riflette i dati di accesso degli ultimi sette giorni.

>[!NOTE]
>Il report di stato dei requisiti di sicurezza è supportato solo nel Centro per i partner. Non è disponibile in Microsoft Cloud for US Government o Microsoft Cloud Germania. È consigliabile che tutti i partner che effettuano transazioni attraverso un cloud sovrano (US Government e Germania) adottino immediatamente questi nuovi requisiti di sicurezza. Tuttavia, non è necessario che questi partner soddisfino ora i nuovi requisiti di sicurezza. Microsoft fornirà altri dettagli sull'applicazione di questi requisiti di sicurezza per i cloud sovrani in futuro.

## <a name="security-status-metrics"></a>Metriche relative allo stato della sicurezza

Il report di stato dei requisiti di sicurezza offre informazioni dettagliate sull'implementazione dell'autenticazione a più fattori e fornisce metriche per la configurazione dell'autenticazione a più fattori e attività del Centro per i partner per i tenant partner. Le sezioni seguenti illustrano queste metriche in modo più dettagliato.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Configurazione dell'autenticazione a più fattori in un tenant partner

La metrica **Percentage of enabled user accounts with MFA enforced using options listed here:** (Percentuale di account utenti abilitati con autenticazione a più fattori applicata usando le opzioni qui elencate) mostra la percentuale di account utente abilitati nel tenant partner ai quali è applicata l'autenticazione a più fattori. Per ottenere la conformità, è possibile usare una di queste [opzioni di autenticazione a più fattori](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Questi dati vengono acquisiti e segnalati su base giornaliera. Ad esempio:

- Contoso è un partner CSP con 110 account utente nel tenant, 10 dei quali sono disabilitati. 
- A 90 dei 100 account utente rimanenti viene applicata l'autenticazione MFA usando le [opzioni MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) specificate. Di conseguenza, la metrica indica il 90%. 

### <a name="partner-center-requests-with-mfa"></a>Richieste del Centro per i partner con autenticazione a più fattori

Ogni volta che i tuoi dipendenti accedono al Centro per i partner per lavorare oppure, tramite le API, ricevono o inviano dati attraverso il Centro per i partner, il loro stato di sicurezza viene testato e monitorato. Sono incluse nel rilevamento dello stato di sicurezza anche le applicazioni in uso e tutte le applicazioni del fornitore del pannello di controllo. Questi dati vengono visualizzati nelle metriche disponibili in **Percentage of requests to Partner Center with MFA** (Percentuale di richieste inviate al Centro per i partner con autenticazione a più fattori) e riflettono lo stato degli ultimi sette giorni.

#### <a name="dashboard-mfa-verification"></a>Verifica dell'autenticazione a più fattori del dashboard

La metrica **Through Partner Center portal** (Tramite il portale del Centro per i partner) è correlata alle attività all'interno del dashboard Centro per i partner. Misura la percentuale di operazioni eseguite dagli utenti che hanno completato la verifica MFA. Ad esempio:

- Contoso è un partner CSP con due agenti di amministrazione, Jane e John.
- Il primo giorno Jane ha eseguito l'accesso al dashboard Partner Center senza verifica MFA e ha effettuato tre operazioni.
- Il secondo giorno John ha eseguito l'accesso al dashboard Partner Center senza verifica MFA e ha effettuato cinque operazioni.
- Il terzo giorno Jane ha eseguito l'accesso al dashboard Partner Center con verifica MFA e ha effettuato due operazioni.
- Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.
- Le 10 operazioni eseguite nella finestra di sette giorni, due sono state effettuate dall'utente con verifica dell'autenticazione a più fattori. Di conseguenza, la metrica indica il 20%.

Usa il file **Richieste portale senza MFA** per sapere quale utente ha eseguito l'accesso al dashboard Partner Center senza avere la verifica MFA e l'ora dell'ultima visita durante la finestra di reporting.

#### <a name="appuser-mfa-verification"></a>Verifica dell'autenticazione a più fattori app+utente

La metrica **Through API or SDK** (Tramite API o SDK) è correlata all'autenticazione app+utente eseguita tramite le richieste delle API del Centro per i partner. Misura la percentuale di richieste API effettuate usando un token di accesso con attestazione MFA. Ad esempio:

- Fabrikam è un partner CSP che dispone di un'applicazione CSP che usa una combinazione di autenticazione app+utente e di metodi di autenticazione basati solo su app.
- Il primo giorno l'applicazione ha effettuato tre richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente senza verifica dell'autenticazione a più fattori.
- Il secondo giorno l'applicazione ha effettuato cinque richieste API supportate da un token di accesso ottenuto usando l'autenticazione basata solo su app.
- Il terzo giorno l'applicazione ha effettuato due richieste API supportate da un token di accesso ottenuto tramite il metodo di autenticazione app+utente con verifica MFA.
- Nei restanti quattro giorni non è stata effettuata alcuna operazione dagli agenti.
- Le cinque richieste API nel secondo giorno, supportate da un token di accesso ottenuto tramite l'autenticazione basata solo su app, vengono omesse dalla metrica perché non usano le credenziali utente. Delle cinque operazioni rimanenti, due sono state supportate da un token di accesso ottenuto con la verifica dell'autenticazione a più fattori. Di conseguenza, la metrica indica il 40%.

Se vuoi sapere quali sono le attività app+utente che determinano il non 100% di questa metrica, usa i file seguenti:

- **Riepilogo richieste API** per conoscere lo stato generale dell'autenticazione MFA per singola applicazione.
- **Tutte le richieste API** per conoscere i dettagli di ogni richiesta API eseguita dagli utenti del tenant. Il risultato è limitato a un numero massimo pari a 10.000 richieste più recenti per una migliore esperienza di download.

## <a name="actions-for-mfa-status-below-100"></a>Azioni in caso di stato dell'autenticazione a più fattori inferiore al 100%

È possibile che alcuni partner che hanno implementato l'autenticazione a più fattori visualizzino metriche di report inferiori al 100%. Per capire perché, di seguito sono riportati alcuni fattori di cui tenere conto.

> [!NOTE]
> Dovrai collaborare con una persona dell'organizzazione che abbia familiarità con la gestione delle identità e l'implementazione dell'autenticazione MFA per il tenant partner.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Autenticazione a più fattori implementata per il tenant partner

È necessario implementare l'autenticazione a più fattori per il tenant partner per raggiungere la conformità. Per informazioni dettagliate su come implementare l'autenticazione a più fattori, vedere [Requisiti di sicurezza per l'uso del Centro per i partner o delle API del Centro per i partner](partner-security-requirements.md).

>[!NOTE]
> Le metriche dell'autenticazione a più fattori vengono calcolate su base giornaliera e prendono in considerazione le operazioni eseguite negli ultimi sette giorni. Se l'implementazione dell'autenticazione a più fattori per il tenant partner è stata completata solo di recente, è possibile che le metriche non indichino ancora un valore pari al 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Verificare l'autenticazione a più fattori per tutti gli account utente

Verifica se l'implementazione dell'autenticazione MFA corrente copre tutti gli account utente o solo alcuni. Alcune soluzioni di autenticazione a più fattori sono basate su criteri e supportano l'esclusione degli utenti, mentre altre potrebbero richiedere l'abilitazione esplicita dell'autenticazione a più fattori in base ai singoli utenti. Verifica di non aver escluso alcun utente dall'implementazione MFA corrente. Eventuali account utente esclusi che eseguono l'accesso al Centro per i partner per eseguire un'attività correlata a CSP, CPV o un advisor possono causare il mancato raggiungimento del 100% nelle metriche.

### <a name="review-your-mfa-conditions"></a>Esaminare le condizioni dell'autenticazione a più fattori

Verifica se l'implementazione corrente applica l'autenticazione MFA solo in condizioni specifiche. Alcune soluzioni MFA presentano caratteristiche di flessibilità e consentono di applicare l'autenticazione MFA solo quando vengono soddisfatte determinate condizioni, ad esempio un utente che accede da un dispositivo o da una posizione sconosciuta. Un utente che è abilitato per l'autenticazione MFA, ma non è tenuto a completare la verifica MFA quando accede al Centro per i partner, può causare il mancato raggiungimento del 100% nelle metriche.

>[!NOTE]
>Per i partner che hanno implementato l'autenticazione MFA usando le impostazioni predefinite per la sicurezza Azure AD, è importante tenere presente che per gli account utente non di tipo amministratore verrà imposta l'autenticazione a più fattori in base al rischio. Agli utenti verrà chiesto di eseguire l'autenticazione a più fattori solo durante tentativi di accesso a rischio (ad esempio per l'accesso da una località diversa). Inoltre, gli utenti dispongono di un periodo massimo di 14 giorni per la registrazione per l'autenticazione MFA. Agli utenti che non hanno completato la registrazione MFA non verrà richiesta la verifica MFA durante il periodo di 14 giorni. È previsto pertanto che le metriche non siano pari al 100% per i partner che hanno implementato l'autenticazione MFA usando le impostazioni predefinite per la sicurezza Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Esaminare le configurazioni dell'autenticazione a più fattori di terze parti

Se usi una soluzione MFA di terze parti, verifica come è integrata con Azure AD. In generale, sono disponibili due metodi, tra cui la federazione e i controlli personalizzati:

* **Federazione delle identità**: quando riceve una richiesta di autenticazione, Azure AD reindirizza l'utente al provider di identità federato per l'autenticazione. Al completamento dell'autenticazione, il provider di identità federato reindirizza di nuovo l'utente ad Azure AD insieme a un token SAML. Affinché Azure AD riconosca che l'utente ha completato la verifica MFA durante l'autenticazione al provider di identità federato, il token SAML deve includere l'attestazione *authenticationmethodsreferences* (con valore *multipleauthn*). Controlla se il provider di identità federato supporta il rilascio di tale attestazione. In tal caso, verifica che il provider di identità federato sia stato configurato per questa operazione. Se l'attestazione non è presente, Azure AD (e quindi Partner Center) non saprà che l'utente ha completato la verifica MFA e l'assenza dell'attestazione può determinare il mancato raggiungimento del 100% nella metrica.

* **Controllo personalizzato**: non è possibile usare Controllo personalizzato di Azure AD per determinare se un utente ha completato la verifica MFA tramite una soluzione MFA di terze parti. Di conseguenza, tutti gli utenti che hanno completato la verifica MFA tramite un controllo personalizzato verranno sempre considerati da Azure AD e, a sua volta, dal Centro per i partner come utenti che non hanno completato la verifica MFA. Se possibile, è consigliabile passare all'uso della Federazione delle identità anziché di un controllo personalizzato durante l'integrazione con Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identificare gli utenti che hanno eseguito l'accesso al Centro per i partner senza autenticazione a più fattori

Può essere utile identificare gli utenti che accedono al Centro per i partner senza verifica MFA e verificarli a fronte della tua implementazione MFA corrente. Per verificare se un utente ha completato o meno la verifica MFA, puoi usare il [report con le informazioni di accesso Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins). Il report con le informazioni di accesso Azure AD è attualmente disponibile solo per i partner che hanno sottoscritto Azure AD Premium o qualsiasi SKU O365 che includa Azure AD Premium, ad esempio EMS.

## <a name="next-steps"></a>Passaggi successivi

- [Community del gruppo di linee guida per la sicurezza del Centro per i partner](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisiti di sicurezza del Centro per i partner](partner-security-requirements.md)
- [Domande frequenti sui requisiti di sicurezza del Centro per i partner](partner-security-requirements-faq.md)
