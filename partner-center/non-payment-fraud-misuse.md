---
title: Gestire insoluti, frodi o uso improprio
description: Informazioni sui vari rischi coinvolti nelle transazioni online e sulle procedure consigliate per gestire e mitigare tali rischi in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818661"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Gestione di mancato pagamento, frode o uso improprio nel Centro per i partner

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente di amministrazione | Amministratore fatturazione

L'utente è responsabile finanziariamente degli acquisti fraudolenti da parte dei clienti e/o del non pagamento dei servizi acquistati. Pertanto, è consigliabile mettere in atto controlli di prevenzione e rilevamento dei rischi *di prevenzione delle frodi.*

Per evitare e/o risolvere attività fraudolente o uso improprio, è importante comprendere i potenziali rischi e sviluppare criteri e procedure che possono ridurre l'esposizione.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Applicazione dei criteri di utilizzo accettabili di Microsoft

Se Microsoft rileva attività di partner o clienti che confermano o sospettano di violare i criteri per l'uso accettabile, verranno esecutori i passaggi di imposizione. Il cliente potrebbe essere immediatamente sospeso. Si verrà informati delle azioni di imposizione o aggiornato in base alle richieste da Parte di Microsoft.

## <a name="abuse-of-service-risks"></a>Uso improprio dei rischi del servizio

**L'uso improprio** dei rischi del servizio implica che i clienti che usano servizi cloud violano i criteri di utilizzo accettabili di Microsoft.

### <a name="examples-of-abuse-of-service"></a>Esempi di uso improprio del servizio

Esempi di queste violazioni dei criteri di utilizzo accettabili di Microsoft possono includere:

- Spamming
- Hacking
- Attacchi Distributed Denial of Service (DDoS)
- Mining Disamina
- Distribuzione di malware
- Rivendita di sottoscrizioni pirata

## <a name="theft-of-service-risks"></a>Furto di rischi del servizio

**Il furto di rischi del** servizio indica i clienti che non hanno intenzione di pagare per i servizi utilizzati. Questo furto può comportare l'uso di strumenti di pagamento rubati, fornendo informazioni di fatturazione false e/o l'impostazione predefinita sui saldi in sospeso.

### <a name="examples-of-service-theft"></a>Esempi di furto di servizi

Esempi di questi rischi per le transazioni online possono includere:

- Transazioni che non si verificano di persona ("transazioni con carta di credito non presente")
- Identità rappresentate in modo errepresente
- Servizi di cui è stato effettuato il provisioning e usati prima della ricezione del pagamento iniziale
- Mercati emergenti e/o aree ad alto rischio per le frodi online
- Automatizzare la creazione e l'acquisto di account da parte di attori malinti

## <a name="managing-online-risk"></a>Gestione dei rischi online

È possibile usare le raccomandazioni seguenti per sviluppare criteri e procedure per ridurre l'esposizione ai rischi delle transazioni online nel ciclo di vita delle relazioni con i clienti.

### <a name="onboarding-new-customers"></a>Onboarding di nuovi clienti

I suggerimenti per ridurre i rischi online durante l'onboarding di nuovi clienti includono:

- Stabilire relazioni personali con i clienti quando possibile (ad esempio, contattare i clienti per telefono).
- Verificare le credenziali e il background dei clienti tramite metodi migliori, ad esempio usando uffici di credito o agenzie di report commerciali.
- Usare l'autenticazione a più fattori (ad esempio la verifica SMS) durante l'iscrizione per ridurre al minimo l'esposizione alla creazione e all'acquisto di account robotici.
- Gestire e tenere traccia delle identità usando i servizi (ad esempio i servizi di identità digitali).
- Valutare la solidità finanziaria dei clienti tramite rigorosi sistemi di rilevamento delle frodi con carta di credito.
- Stabilire criteri di raccolta non crittografati. Descrizione dettagliata del processo di raccolta e del momento in cui l'accesso alle sottoscrizioni sarà influenzata dal non pagamento. È possibile disabilitare l'accesso [o sospendere le sottoscrizioni di un cliente](create-a-new-subscription.md#suspend-a-subscription) per il non pagamento.

### <a name="managing-customer-accounts"></a>Gestione degli account cliente

I suggerimenti per la gestione degli account dei clienti dopo l'acquisto includono:

- Implementare un processo per ricevere, rivedere, agire e rispondere rapidamente alle notifiche Microsoft.
- Collaborare con i clienti per comprendere le esigenze aziendali di utilizzo del cloud e impostare soglie di monitoraggio appropriate. Ad esempio, è possibile impostare [un budget di spesa mensile di Azure](set-an-azure-spending-budget-for-your-customers.md) Partner Center. Questa conoscenza consente di monitorare l'utilizzo dei clienti durante il mese e di ricevere una notifica quando i clienti sono vicini al budget.
- Monitorare regolarmente [i log attività dei clienti](activity-logs.md) per rilevare tempestivamente le frodi.
- Intraprendere un'azione rapida quando vengono rilevate attività sospette.
- Evitare di concedere ai clienti l'accesso amministrativo completo alle sottoscrizioni senza prima implementare i controlli di mitigazione dei rischi.

### <a name="managing-customer-billing"></a>Gestione della fatturazione dei clienti

I suggerimenti per la gestione della fatturazione dei clienti dopo l'acquisto includono:

- Richiedere pagamenti anticipati prima delle transazioni iniziali e della fatturazione.
- Non accettare strumenti di pagamento ad alto rischio, ad esempio carte prepagato o carte con valore archiviato.
- Monitorare i pagamenti dei clienti e i crediti degli account obsoleti. Applicare in modo aggressivo processi di dunazione standardizzati per i pagamenti in ritardo o il non pagamento.

Per strategie più dettagliate per la mitigazione dei rischi online, vedere la Guida [alla gestione dei rischi delle transazioni online.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
