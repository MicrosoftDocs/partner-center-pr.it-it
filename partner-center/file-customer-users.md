---
title: Campi per il file con estensione CSV per l'importazione di più utenti per un account cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti a un account cliente, creare un file con valori delimitati da virgole (CSV) con campi appropriati.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528181"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Aggiungere più utenti a un account cliente creando un file CSV

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

Aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner. È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisiti per i file di dati

Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:

- Devi avere le autorizzazioni di amministratore globale per l'account del cliente;
- Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;
- Puoi caricare fino a 100 record alla volta. Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.
- Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.
- Immetti solo i dati descritti di seguito. La presenza di dati estranei causerà l'esito negativo del caricamento.

Immetti i dati seguenti nel file di dati:

| **Nome colonna** | **Descrizione**  | **Limitazione**  |
|:-------- |:------  |:----- |
| Nome  | Nome dell'utente (campo facoltativo)  | Limite di 50 caratteri  |
| Cognome  | Cognome dell'utente (campo facoltativo)  | Limite di 50 caratteri  |
| Nome visualizzato    | Nome visualizzato nel centro per i partner (campo obbligatorio)                            | Limite di 50 caratteri                         |
| E-mail   | Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo di posta elettronica univoco |
| Aggiornamento dello stato   | Usato per indicare se il nuovo record utente è stato o meno creato correttamente | \*\*Lascia vuoto\*\*                        |

## <a name="next-steps"></a>Passaggi successivi

- [Come aggiungere più utenti per un cliente](adding-multiple-users-to-a-customer-account.md)