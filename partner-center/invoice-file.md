---
title: Informazioni sulle fatture di fatturazione del centro per i partner
ms.topic: article
ms.date: 05/18/2020
description: Comprendere i campi del file di fattura per la fatturazione del centro per i partner. Sono inclusi campi e definizioni per tutti i campi della fattura e per i campi con addebito unico.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3e9eb392279c0a09b5e30395b38ab7030bfa87d4
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556294"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informazioni sui campi fattura del centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Amministratore fatturazione
- Agente di supporto tecnico

È possibile usare le tabelle seguenti per comprendere i campi nei file di fattura del centro per i partner.

## <a name="invoice-file-fields"></a>Campi del file di fattura

Nei file della fattura vengono visualizzati i campi seguenti.

| Campo | Definizione |
| ----- | ---------- |
| US FEIN | Il numero di identificazione del datore di lavoro federale (FEIN). Si tratta del Stati Uniti numero di identificatore dell'imposta federale. |
| Numero cliente | Numero del cliente. |
| Indirizzo di fatturazione | Indirizzo a cui inviare la fattura. È possibile modificare il nome e/o l'indirizzo della società nel profilo di fatturazione del centro per i partner. |
| Addebiti basati su licenza | Costi flat mensili o annuali per le licenze basate sull'utilizzo acquistate, fatturate prima del servizio. Questo numero corrisponde alla somma di tutti gli addebiti nella colonna del **Subtotale** (colonna **T**) nel file di riconciliazione basato sulle licenze. |
| Addebiti basati sull'utilizzo | Utilizzo di Azure. Sono inclusi i nuovi servizi o le applicazioni abilitati e usati durante il periodo di fatturazione. Questo numero corrisponde alla somma di tutti gli addebiti nella colonna **PretaxCharges** (colonna **Z**) nel file di riconciliazione basato sull'utilizzo. |
| Sconti | Lo sconto ricevuto dal cliente dal prezzo normale della sottoscrizione. Questo numero viene visualizzato come *importo Flat*, non come prezzo per unità o licenza. |
| Credits | Crediti o rettifiche per le modifiche apportate alle sottoscrizioni (ad esempio, aumenti o diminuzioni della licenza). |
| Subtotale | Totale prima delle imposte e addebiti e crediti fiscali esclusivi. |
| Imposta | Imposta totale per gli addebiti correnti, come totale nella sezione dei **Dettagli** a partire dalla pagina 2 della fattura. Questo numero corrisponde alla somma di tutti gli addebiti nella colonna **TaxAmount** (colonna **AA**) nel file di riconciliazione basato sull'utilizzo e nella colonna **Tax** (colonna **U**) nel file di riconciliazione basato su licenza. |
| Altri crediti | Crediti fiscali-esclusivi. |
| Addebiti correnti totali | Importo dovuto alla valuta di fatturazione per il periodo di fatturazione. Questi addebiti sono dovuti alla data di scadenza del pagamento. |
| Istruzioni per il pagamento | Descrizione di come pagare la fattura in base all'area geografica. *Quando si effettua un pagamento, assicurarsi sempre di includere il numero di fattura.* |
| N. fattura | Numero della fattura. |
| Periodo di fatturazione | Il periodo mensile che precede la data della fattura. Si tratta del periodo di tempo durante il quale vengono utilizzati i servizi basati sull'utilizzo e i servizi basati su licenze vengono riconciliati per eventuali rettifiche di credito o modifiche al numero di licenze. |
| Data fattura | Data di fatturazione o di anniversario in cui la fattura viene generata ogni mese. |
| Condizioni di pagamento | Termine del pagamento. Per gli acquisti monouso, questo sarà sempre di 60 giorni. |
| Data scadenza pagamento | Data in base alla quale deve essere ricevuto il pagamento. |
| Ordine d'acquisto del cliente | Ordine dei numeri di acquisto. |
| Servizio clienti | Indirizzo del sito Web a cui è possibile accedere al servizio clienti. |
| Destinatario servizio | Indirizzo in cui viene utilizzato il servizio. Si tratta dell'indirizzo aziendale legale associato al vagliatura aziendale. |

## <a name="one-time-charges-fields"></a>Campi di addebiti una sola volta

I campi seguenti si applicano solo agli **addebiti** monouso nel centro per i partner:

| Campo | Definizione |
| ----- | ---------- |
| Data | Data di acquisto. |
| Descrizione | Nome prodotto. |
| Quantità | Il numero di prodotti (ad esempio prenotazioni) acquistati. |
| Prezzo unitario | Prezzo per prodotto, ad esempio una prenotazione. |
| Sconti | Eventuali sconti applicabili. |
| Importo pre-imposta | Sub-Total degli acquisti prima delle imposte. |
| Imposta sulle vendite | Importo relativo alle imposte. |
| Totale | Importo totale da pagare. |
