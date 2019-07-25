---
title: Domande frequenti sui requisiti di sicurezza dei partner | Centro per i partner
ms.topic: article
ms.date: 07/18/2019
description: Domande frequenti sui requisiti di sicurezza dei partner
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, provider di soluzioni cloud, programma Cloud Solution Provider, CSP, fornitore del pannello di controllo, CPV, multi-factor authentication, autenticazione a più fattori, modello di applicazione sicura, modello di applicazione sicura, sicurezza
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315550"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Domande frequenti sui requisiti di sicurezza dei partner

Questo articolo contiene alcune domande frequenti sui requisiti di [sicurezza dei partner](partner-security-requirements.md). [Qui](http://assetsprod.microsoft.com/security-requirements-faq.pdf)è possibile trovare un elenco completo delle domande frequenti.

## <a name="conditional-access"></a>Accesso condizionale

### <a name="can-conditional-access-be-used"></a>È possibile usare l'accesso condizionale?

Sì, è possibile usare l'accesso condizionale per applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner. Tuttavia, data la natura altamente privilegiata di essere un partner, è necessario assicurarsi che ogni utente abbia una richiesta di autenticazione a più fattori per ogni singola autenticazione. Ciò significa che non sarà possibile sfruttare la funzionalità di accesso condizionale che elude il requisito per l'autenticazione a più fattori.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>I clienti sono soggetti ai requisiti di sicurezza dei partner?

No, non è necessario applicare l'autenticazione a più fattori per ogni utente nei tenant Azure AD del cliente. Tuttavia, si consiglia di collaborare con ogni cliente per determinare il modo migliore per proteggere gli utenti.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>È possibile usare le password delle app con i criteri di protezione di base?

Sì, è possibile usare le [password dell'app](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) . Esaminare le considerazioni per l'uso delle password di app documentate [qui](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) per determinare se sono supportate in base alle esigenze.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>È possibile escludere qualsiasi utente da questo requisito? 

No, per ogni utente, inclusi gli account del servizio, nel tenant partner verrà richiesto di eseguire l'autenticazione con l'autenticazione a più fattori.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>I requisiti di sicurezza dei partner si applicano alla sandbox di integrazione?

Sì, i requisiti di sicurezza del partner si applicano alla sandbox di integrazione. Ciò significa che sarà necessario implementare la soluzione di autenticazione a più fattori appropriata per gli utenti nel tenant sandbox di integrazione. È consigliabile implementare i criteri di protezione di base per fornire l'autenticazione a più fattori.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Ricerca per categorie configurare un account di accesso di emergenza (Break Glass)?

È stata considerata una procedura consigliata creare uno o due account di accesso di emergenza per impedire che il tenant Azure AD venga bloccato inavvertitamente. Per quanto riguarda i requisiti di sicurezza dei partner, è necessario che ogni utente esegua l'autenticazione con multi-factor authentication. Questo significa che sarà necessario modificare la definizione di un account di accesso di emergenza. Potrebbe trattarsi di un account che sfrutta una soluzione di terze parti per l'autenticazione a più fattori.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>In che modo gli utenti Guest saranno interessati dai requisiti di sicurezza dei partner?

Gli utenti Guest dovranno eseguire l'autenticazione con l'autenticazione a più fattori quando accedono alle risorse nel tenant partner. I requisiti di sicurezza dei partner non avranno alcun effetto sull'accesso delle risorse al tenant da parte dell'utente Guest.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Se si usa una soluzione di terze parti è Active Directory è necessario Servizio federativo (ADFS)? 

No, non è necessario disporre di Active Directory Servizio federativo (ADFS) se si utilizza una soluzione di terze parti. Si consiglia di collaborare con il fornitore della soluzione per determinare quali sono i requisiti per la soluzione.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>È necessario abilitare i criteri di protezione di base?

No, non è necessario abilitare i criteri di protezione di base. L'unico requisito è quello di applicare l'autenticazione a più fattori per ogni utente, inclusi gli account del servizio, nel tenant partner.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>Quali opzioni di verifica vengono fornite tramite l'implementazione dei criteri di protezione di base? 

Per quanto riguarda la versione di multi-factor authentication disponibile tramite l'implementazione dei criteri di protezione di base, l'unica opzione di verifica disponibile è un'app di autenticazione. L'utilizzo di una telefonata e di un messaggio di SMS è considerato meno sicuro. Quindi, queste opzioni non sono disponibili tramite questa versione di autenticazione a più fattori.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>L'account del servizio usato da Azure AD Connect sarà influenzato dai requisiti di sicurezza dei partner?

No, l'account del servizio usato da Azure AD Connect non verrà influenzato dai requisiti di sicurezza dei partner. Se si verifica un problema con Azure AD Connect come risultato dell'applicazione dell'autenticazione a più fattori, aprire una richiesta di supporto tecnico con il supporto tecnico Microsoft.
