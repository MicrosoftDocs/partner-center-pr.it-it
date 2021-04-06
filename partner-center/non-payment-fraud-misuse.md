---
title: Gestire insoluti, frodi o uso improprio
description: Informazioni sui diversi rischi correlati alle transazioni online e sulle procedure consigliate per gestire e mitigare tali rischi nel centro per i partner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 9b3beef70052ad204327dd53c4aa9f477056bbcb
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441864"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gestione di mancato pagamento, frode o uso improprio nel Centro per i partner

Si applica a:

- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale
- Amministratore gestione utenti
- Agente amministratore
- Amministratore fatturazione

L'utente è responsabile finanziario per gli acquisti fraudolenti da clienti e/o clienti che non hanno effettuato il pagamento dei servizi acquistati. Pertanto, si *consiglia di adottare i controlli di mitigazione dei rischi di rilevamento e prevenzione delle frodi*.

Per evitare e/o risolvere le attività fraudolente o l'utilizzo improprio, è importante comprendere i potenziali rischi e sviluppare criteri e procedure che possono ridurre l'esposizione.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Imposizione dei criteri di utilizzo accettabili di Microsoft

Se Microsoft rileva l'attività del partner o del cliente confermata o sospetta viola i criteri di utilizzo accettabili, verranno eseguiti i passaggi per l'applicazione. Il cliente potrebbe essere immediatamente sospeso. Si riceverà una notifica sulle azioni di imposizione o sull'aggiornamento delle richieste da Microsoft.

## <a name="abuse-of-service-risks"></a>Abuso dei rischi di servizio

L' **abuso dei** rischi per i servizi indica che i clienti che usano servizi cloud violano i criteri di utilizzo accettabili di Microsoft.

### <a name="examples-of-abuse-of-service"></a>Esempi di abusi del servizio

Esempi di queste violazioni dei criteri di utilizzo accettabili di Microsoft possono includere:

- Spamming
- Hacking
- Attacchi Denial of Service (DDoS) distribuiti
- Data mining Bitcoin
- Distribuzione malware
- Rivendita di sottoscrizioni Pirate

## <a name="theft-of-service-risks"></a>Furto dei rischi di servizio

Il **furto di** rischi per i servizi indica ai clienti che non hanno intenzione di pagare per i servizi usati. Questo furto può comportare l'utilizzo di strumenti di pagamento rubati, l'invio di informazioni di fatturazione false e/o l'impostazione predefinita di saldi in attesa.

### <a name="examples-of-service-theft"></a>Esempi di furto del servizio

Esempi di questi rischi per le transazioni online possono includere:

- Transazioni che non si verificano in persona (transazioni con carta di credito non presenti)
- Identità non rappresentate
- Servizi sottoposti a provisioning e utilizzati prima della ricezione del pagamento iniziale
- Mercati emergenti e/o aree ad alto rischio per frode online
- Automatizzare la creazione e l'acquisto di account da attori malintenzionati

## <a name="managing-online-risk"></a>Gestione dei rischi online

È possibile utilizzare i seguenti suggerimenti per sviluppare criteri e procedure per ridurre l'esposizione ai rischi per le transazioni online nel ciclo di vita delle relazioni dei clienti.

### <a name="onboarding-new-customers"></a>Onboarding di nuovi clienti

Suggerimenti per ridurre i rischi online quando il caricamento di nuovi clienti include:

- Stabilire relazioni personali con i clienti, se possibile, ad esempio contattando i clienti per telefono.
- Verificare le credenziali e i retroscena dei clienti tramite metodi migliori, ad esempio l'uso di uffici di credito o agenzie di report commerciali commerciali.
- Usare l'autenticazione a più fattori, ad esempio la verifica tramite SMS, durante l'iscrizione per ridurre al minimo l'esposizione alla creazione e all'acquisto di account robotizzati.
- Gestire e tenere traccia delle identità usando i servizi, ad esempio i servizi di identità digitali.
- Valutare la forza finanziaria dei clienti tramite sistemi di rilevamento illeciti di carte di credito rigorosi.
- Definire un criterio Clear Collections. Consente di illustrare in dettaglio il processo di raccolta e quando l'accesso alle sottoscrizioni sarà influenzato da un mancato pagamento. È possibile disabilitare l'accesso o [sospendere le sottoscrizioni di un cliente per il](create-a-new-subscription.md#suspend-a-subscription) mancato pagamento.

### <a name="managing-customer-accounts"></a>Gestione degli account cliente

I suggerimenti per la gestione degli account cliente dopo l'acquisto includono:

- Implementare un processo per ricevere, rivedere, agire in modo rapido e rispondere alle notifiche Microsoft.
- Collaborare con i clienti per comprendere le esigenze aziendali di utilizzo del cloud e le impostazioni appropriate per le soglie di monitoraggio. Ad esempio, è possibile [impostare un budget mensile per la spesa di Azure](set-an-azure-spending-budget-for-your-customers.md) nel centro per i partner. Questa comprensione consente di monitorare l'utilizzo dei clienti durante il mese e di ricevere una notifica quando i clienti si avvicinano al budget.
- Monitora regolarmente i [log attività del cliente](activity-logs.md) per aiutare a rilevare tempestivamente le frodi.
- Eseguire un'azione rapida quando vengono rilevate attività sospette.
- Evitare di concedere ai clienti l'accesso amministrativo completo alle sottoscrizioni senza prima implementare i controlli di mitigazione dei rischi.

### <a name="managing-customer-billing"></a>Gestione della fatturazione dei clienti

I suggerimenti per la gestione della fatturazione del cliente dopo l'acquisto includono:

- Richiedere i prepagamenti prima delle transazioni e della fatturazione iniziali.
- Non accettare strumenti di pagamento ad alto rischio (ad esempio carte prepagate o schede con valori archiviati).
- Monitorare i pagamenti dei clienti e l'invecchiamento degli account. Applicare in modo aggressivo i processi di Dunning standardizzati per i pagamenti tardivi o il mancato pagamento.

Per strategie più dettagliate per attenuare i rischi online, vedere la guida alla gestione dei rischi per le [transazioni online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
