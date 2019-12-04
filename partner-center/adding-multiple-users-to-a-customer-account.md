---
title: Creare più utenti per l'account di un cliente | Centro per i partner
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere più utenti all'account di un cliente contemporaneamente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: caricamento in blocco, aggiungere più utenti all'account di un cliente, aggiungere gli utenti di un cliente, caricamento in blocco degli utenti di un cliente, account del cliente, utenti del cliente, utenti
ms.localizationpriority: medium
ms.openlocfilehash: 2195d23074a3e7c397b5f557fd3bed9ec0cc518e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721990"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Aggiungere più utenti all'account di un cliente

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

È possibile aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner. È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.

## <a href="" id="creatingtheimportcsvfile"></a>Requisiti per i file di dati

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
| E-mail           | Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo e-mail univoco |
| Aggiornamento stato   | Usato per indicare se il nuovo record utente è stato o meno creato correttamente | \*\*lasciare vuoti\*\*                        |

### <a href="" id="createmultipleuseraccounts"></a>Per creare più account utente

<a href="" id="creatingtheaccounts"></a>

1. Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo.

2. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.

3. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

4. Selezionare la scheda **utenti e licenze** del cliente, quindi selezionare **carica utenti**.

5. In **Carica informazioni utenti** seleziona **Sfoglia**.

6. Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.

7. Seleziona **Convalida**.

    **Si noti**  la maggior parte degli errori di creazione dell'account sono causati da problemi relativi a file di dati, ad esempio informazioni mancanti, indirizzi di posta elettronica non validi o duplicati oppure troppi record nel file.

8. Dopo che il centro per i partner ha convalidato il file, selezionare la **posizione** geografica per i nuovi utenti.
9. Seleziona **Salva**.
10. Scarica le informazioni sulle password temporanee per gli utenti.

**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

10. Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni **può usare licenze e servizi**. 

 

 



