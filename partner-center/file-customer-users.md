---
title: Campi per il file CSV per importare più utenti per un account cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti a un account cliente, creare un file con estensione csv con valori delimitati da virgole con i campi appropriati.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150982"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Aggiungere più utenti a un account cliente creando un file CSV

**Ruoli appropriati**: Amministratore globale

Aggiungere contemporaneamente più utenti all'account di un cliente caricando un file di dati nel formato di file con valori delimitati da virgole (csv) nel Partner Center. È possibile scaricare un file di dati di esempio dal Partner Center e quindi modificarlo per l'uso oppure creare un nuovo file di dati usando il modello di dati definito di seguito.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisiti per i file di dati

Per aggiungere più utenti all'account di un cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:

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
| Nome visualizzato    | Nome visualizzato nella Partner Center (campo obbligatorio)                            | Limite di 50 caratteri                         |
| E-mail   | Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo di posta elettronica univoco |
| Aggiornamento dello stato   | Usato per indicare se il nuovo record utente è stato creato correttamente | \*\*Lasciare vuoto\*\*                        |

## <a name="next-steps"></a>Passaggi successivi

- [Come aggiungere più utenti per un cliente](adding-multiple-users-to-a-customer-account.md)