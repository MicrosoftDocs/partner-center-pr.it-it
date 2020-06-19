---
title: Aggiungere più utenti per un account cliente
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere più utenti all'account di un cliente in una sola volta. Caricare un file di dati nel centro per i partner usando il formato di file con valori delimitati da virgole (CSV).
author: LauraBrenner
ms.author: labrenne
keywords: caricamento bulk, aggiunta di più utenti a un account cliente, aggiunta degli utenti del cliente, caricamento bulk degli utenti del cliente, account cliente, utenti cliente, utenti
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 09bb83b82cf1db78a54af9bab98a5cbdaa00c0d9
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991083"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a>Aggiungere più utenti a un account cliente: caricare un file di dati nel centro per i partner

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

È possibile aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner. È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisiti per i file di dati

Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:

- Devi avere le autorizzazioni di amministratore globale per l'account del cliente;
- Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;
- Puoi caricare fino a 100 record alla volta. Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.
- Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.
- Immetti solo i dati descritti di seguito. La presenza di dati estranei causerà l'esito negativo del caricamento.

Immetti i dati seguenti nel file di dati:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nome colonna** | **Descrizione**                                                              | **Limitazione**                             |
| Nome      | Nome dell'utente (campo facoltativo)                                           | Limite di 50 caratteri                         |
| Cognome       | Cognome dell'utente (campo facoltativo)                                            | Limite di 50 caratteri                         |
| Nome visualizzato    | Nome visualizzato nel centro per i partner (campo obbligatorio)                            | Limite di 50 caratteri                         |
| Email           | Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo di posta elettronica univoco |
| Aggiornamento dello stato   | Usato per indicare se il nuovo record utente è stato o meno creato correttamente | \*\*Lascia vuoto\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>Per creare più account utente

<a href="" id="creatingtheaccounts"></a>

1. Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo.

2. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

3. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

4. Selezionare la scheda **utenti e licenze** del cliente, quindi selezionare **carica utenti**.

5. In **Carica informazioni utenti** seleziona **Sfoglia**.

6. Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.

7. Selezionare **Convalida**.

    **Nota**    La maggior parte degli errori di creazione dell'account è causata da problemi relativi ai file di dati, tra cui informazioni mancanti, indirizzi di posta elettronica non validi o duplicati o troppi record nel file.

8. Dopo che il centro per i partner ha convalidato il file, selezionare la **posizione** geografica per i nuovi utenti.
9. Selezionare **Salva**.
10. Scaricare le informazioni sulla password temporanea per gli utenti.

**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

10. Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni di **che possono usare licenze e servizi** . 

 

 



