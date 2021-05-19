---
title: Informazioni Partner Center fatturazione
ms.topic: article
ms.date: 05/18/2020
description: Comprendere i campi nel file della fattura per Partner Center fatturazione. Sono inclusi i campi e le definizioni per tutti i campi della fattura e i campi di addebito una sola volta.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146613"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informazioni Partner Center campi della fattura di fatturazione

**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Amministratore fatturazione | Agente del supporto help desk

È possibile usare le tabelle seguenti per comprendere i campi nei file Partner Center fattura.

## <a name="invoice-file-fields"></a>Campi del file della fattura

I campi seguenti vengono visualizzati nei file della fattura.

| Campo | Definizione |
| ----- | ---------- |
| US FEIN | Numero di identificazione del datore di lavoro federale (FEIN). Questo è il numero Stati Uniti'identificatore fiscale federale. |
| Numero cliente | Numero del cliente. |
| Indirizzo di fatturazione | Indirizzo a cui inviare la fattura. È possibile modificare il nome e l'indirizzo della società nel Partner Center di fatturazione. |
| Addebiti basati su licenza | Addebiti mensili o annuali per le licenze basate sull'utilizzo acquistate, fatturate prima del servizio. Questo numero è la somma di tutti gli addebiti nella colonna **Subtotal** (colonna **T**) nel file di riconciliazione basato su licenza. |
| Addebiti in base all'utilizzo | Utilizzo di Azure. Sono inclusi nuovi servizi o applicazioni abilitati e usati durante il periodo di fatturazione. Questo numero è la somma di tutti gli addebiti nella colonna **PretaxCharges** (colonna **Z**) nel file di riconciliazione basato sull'utilizzo. |
| Sconti | Sconto che il cliente riceve dal prezzo normale della sottoscrizione. Questo numero viene visualizzato come importo *fisso,* non come prezzo per unità o licenza. |
| Credits | Crediti o rettifiche per le modifiche apportate alle sottoscrizioni (ad esempio, aumenti o diminuzioni delle licenze). |
| Subtotale | Totale prima delle imposte e degli addebiti e crediti escludono le imposte. |
| Imposta | L'imposta totale per gli addebiti correnti, come totale nella **sezione Dettagli** a partire dalla pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti nella colonna **TaxAmount** (colonna **AA)** nel file di riconciliazione basato sull'utilizzo e nella colonna **Tax** (colonna **U**) nel file di riconciliazione basato su licenza. |
| Altri crediti | Crediti escludono le imposte. |
| Addebiti correnti totali | Importo dovuto nella valuta di fatturazione per il periodo di fatturazione. Questi addebiti sono dovuti entro la data di scadenza del pagamento. |
| Istruzioni per il pagamento | Descrizione di come pagare la fattura, in base all'area. *Assicurarsi sempre di includere il numero di fattura quando si effettua un pagamento.* |
| N. fattura | Numero della fattura. |
| Periodo di fatturazione | Periodo mensile che ha inizio alla data della fattura. Questo è il periodo durante il quale i servizi basati sull'utilizzo vengono utilizzati e i servizi basati su licenza vengono riconciliati per eventuali modifiche al credito o modifiche nel numero di licenze. |
| Data fattura | Data di fatturazione o data dell'anniversario in cui la fattura viene generata ogni mese. |
| Condizioni di pagamento | Termine di pagamento. Per gli acquisti una sola volta, saranno sempre 60 giorni. |
| Data scadenza pagamento | Data entro la quale il pagamento deve essere ricevuto. |
| Ordine d'acquisto del cliente | Ordine del numero di acquisto. |
| Servizio clienti | Indirizzo del sito Web in cui è possibile accedere al servizio clienti. |
| Destinatario servizio | Indirizzo in cui viene usato il servizio. Si tratta dell'indirizzo legale dell'azienda associato al controllo dell'azienda. |

## <a name="one-time-charges-fields"></a>Campi degli addebiti una sola volta

I campi seguenti si applicano solo **agli addebiti una sola** volta Partner Center:

| Campo | Definizione |
| ----- | ---------- |
| Data | Data di acquisto. |
| Descrizione | Nome prodotto. |
| Quantity | Numero di prodotti (ad esempio prenotazioni) acquistati. |
| Prezzo unitario | Prezzo per prodotto (ad esempio una prenotazione). |
| Sconti | Eventuali sconti applicabili. |
| Importo pre-imposta | Subtotale degli acquisti prima delle imposte. |
| Iva | Importo relativo alle imposte. |
| Totale | Importo totale da pagare. |
