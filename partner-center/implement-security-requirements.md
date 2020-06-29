---
title: Implementare i requisiti di sicurezza per i partner
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come implementare i requisiti di sicurezza necessari per gli utenti
author: LauraBrenner
ms.author: labrenne
keywords: sicurezza
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133266"
---
# <a name="implement-the-partner-security-requirements"></a>Implementare i requisiti di sicurezza per i partner

**Ruoli appropriati**

- Amministratore globale

Sicurezza e privacy di clienti e partner costituiscono le priorità principali di Microsoft. Continuano infatti a perpetrarsi in misura crescente attacchi alla sicurezza sempre più sofisticati, soprattutto correlati a eventi di compromissione dell'identità. Poiché i controlli preventivi svolgono un ruolo fondamentale in una strategia di difesa complessiva volta a contrastare gli attacchi alla sicurezza, per contribuire alla protezione di partner e clienti si inizierà ad applicare un set di requisiti di sicurezza obbligatori.

In questa esercitazione comprenderai meglio i requisiti di sicurezza per i partner, come soddisfarli e l'effetto sugli utenti nella directory del partner.

Tutti i partner che partecipano al programma Cloud Solution Provider, i fornitori del pannello di controllo e i partner Advisor devono applicare l'autenticazione a più fattori per ogni utente nel relativo tenant del partner. A tale scopo, è possibile abilitare due [criteri di base di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). I criteri di base sono un set di criteri predefiniti che consentono di proteggere le organizzazioni da molti attacchi comuni. Questi attacchi comuni possono includere password spraying, riproduzione e phishing. I criteri di protezione di base sono disponibili in tutte le edizioni di Azure Active Directory. A seguito dell'aumento degli attacchi basati sull'identità registrato negli ultimi anni, Microsoft li renderà presto disponibili a tutti gli utenti.

Le procedure riportate di seguito descrivono il processo di abilitazione dei due criteri di base necessari:

- **Richiedere l'autenticazione a più fattori per gli amministratori** Se si abilita il criterio Richiedere l'autenticazione a più fattori per gli amministratori, gli utenti nei ruoli di amministratore dovranno eseguire la registrazione all'autenticazione a più fattori usando l'app Authenticator. Al termine della registrazione all'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.

- **Protezione dell'utente finale** Protezione dell'utente finale è un criterio di base dell'autenticazione a più fattori basato sul rischio che protegge tutti gli utenti di una directory. Per abilitare questo criterio è necessario che tutti gli utenti eseguano la registrazione all'autenticazione a più fattori usando l'app Authenticator. Gli utenti possono ignorare la richiesta di registrazione dell'autenticazione a più fattori per 14 giorni, dopo i quali verrà impedito l'accesso fino al momento di registrarsi all'autenticazione a più fattori. Al termine della registrazione all'autenticazione a più fattori, agli utenti verrà richiesto di eseguire l'autenticazione a più fattori solo durante i tentativi di accesso rischioso. Gli account utente compromessi vengono bloccati finché la password non viene reimpostata e gli eventi di rischio sono stati risolti.

Dopo l'abilitazione di questi criteri, ogni utente potrà usare l'autenticazione a più fattori di Azure senza costi aggiuntivi. Se usi una soluzione di terze parti, devi applicare l'autenticazione a più fattori per ogni utente per l'accesso ai servizi del cloud commerciale Microsoft.

>[!NOTE]
>Poiché l'autenticazione a più fattori verrà applicata per tutti gli utenti nella directory del partner, ci saranno ripercussioni su un'eventuale automazione o integrazione che usa le credenziali utente. Per far fronte a tali ripercussioni, dovrai modificare il modo in cui l'automazione o l'integrazione si connette ai servizi del cloud commerciale Microsoft. Se il servizio a cui ti connetti supporta l'autenticazione basata su token, è consigliabile implementare il [framework modello di applicazione sicura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Passaggio 1: Bloccare tutti i protocolli di autenticazione legacy esistenti

Prima di abilitare i criteri di protezione Richiedere l'autenticazione a più fattori per gli amministratori e Protezione dell'utente finale, verificare che gli utenti non usino protocolli di autenticazione legacy. Vedi l'articolo [Procedura: Bloccare l'autenticazione legacy ad Azure AD con l'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) per avere altre informazioni.

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Passaggio 2: Abilitare il criterio di base Richiedere l'autenticazione a più fattori per gli amministratori

Il criterio di base Richiedere l'autenticazione a più fattori per gli amministratori rende obbligatoria l'autenticazione a più fattori per i ruoli di directory seguenti, considerati i più privilegiati tra i ruoli Azure AD:

- Amministratore globale
- Amministratore di SharePoint
- Amministratori di Exchange
- Amministratore di accesso condizionale
- Amministratore della protezione
- Amministratore del supporto tecnico/Amministratore delle password
- Amministratore fatturazione
- Amministratore degli utenti

Se si abilita il criterio Richiedere l'autenticazione a più fattori per gli amministratori, i 9 ruoli di amministratore precedenti dovranno eseguire la registrazione all'autenticazione a più fattori usando l'app Authenticator. Al termine della registrazione all'autenticazione a più fattori, gli amministratori dovranno eseguire l'autenticazione a più fattori ogni volta che accedono.

Se l'organizzazione dispone di questi account in uso negli script o nel codice, è consigliabile sostituirli con  [identità gestite](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Per abilitare questo criterio e proteggere gli amministratori:

1. Accedere al  **portale di Azure** come amministratore globale, amministratore della protezione o amministratore dell'accesso condizionale. 

2. Passare a **Accesso condizionale** di  > **Azure Active Directory**.

3. Nell'elenco dei criteri selezionare **Criteri di base: Richiedere l'autenticazione a più fattori per gli amministratori**.

4. Impostare **Abilita criterio** su **Usa i criteri immediatamente**.

5. Selezionare  **Salva**.

Dopo aver abilitato questo criterio, agli utenti nei ruoli di amministratore precedenti verrà chiesto di eseguire l'accesso per specificare informazioni di sicurezza aggiuntive e configurare l'app per dispositivi mobili. Al completamento di tali operazioni, gli utenti potranno accedere al servizio cloud appropriato.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Passaggio 3: Abilitare il criterio di base Protezione dell'utente finale

I criteri di base per la protezione dell'utente finale proteggono tutti gli utenti di una directory. Per abilitare questo criterio è necessario che tutti gli utenti eseguano la registrazione all'autenticazione a più fattori di Azure entro 14 giorni. Dopo la registrazione, agli utenti verrà richiesta l'autenticazione a più fattori solo durante i tentativi di accesso rischiosi. Questo comportamento cambierà per i tenant dei partner in futuro. Gli account utente compromessi vengono bloccati fino alla reimpostazione della password e alla rimozione del rischio.

Criterio di base dei criteri: Il criterio Protezione dell'utente finale risulterà preconfigurato e verrà mostrato in alto quando si accederà al pannello dell'accesso condizionale nel portale di Azure.

Per abilitare questo criterio e proteggere gli utenti:

1. Accedere al  **portale di Azure** come amministratore globale, amministratore della protezione o amministratore dell'accesso condizionale. 

2. Passare a **Accesso condizionale** di  > **Azure Active Directory**.

3. Nell'elenco dei criteri selezionare **Criteri di base: protezione dell'utente finale (anteprima)** .

4. Impostare **Abilita criterio** su **Usa i criteri immediatamente**.

5. Selezionare  **Salva**.

Dopo aver abilitato questo criterio, a tutti gli utenti verrà chiesto di eseguire l'accesso per specificare informazioni di sicurezza aggiuntive e configurare l'app per dispositivi mobili. Al completamento di tali operazioni, gli utenti potranno accedere al servizio cloud appropriato.

>[!NOTE]
>Finché non vengono applicati i requisiti di sicurezza per i partner, agli utenti non coperti dal criterio di base Richiedere l'autenticazione a più fattori per gli amministratori verrà richiesta solo l'autenticazione a più fattori basata sul rischio.