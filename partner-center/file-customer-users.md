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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441422"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Aggiungere più utenti a un account cliente creando un file CSV

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
| Aggiornamento dello stato   | Utilizzato per indicare se il nuovo record utente è stato creato correttamente | \*\*Lascia vuoto\*\*                        |

## <a name="next-steps"></a>Passaggi successivi

- [Come aggiungere più utenti per un cliente](adding-multiple-users-to-a-customer-account.md)