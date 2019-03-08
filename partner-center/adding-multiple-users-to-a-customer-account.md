---
title: Creare più utenti per l'account di un cliente | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: Puoi aggiungere più utenti contemporaneamente all'account di un cliente caricando un file di dati con valori delimitati da virgole (CSV) nel Centro per i partner.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: caricamento in blocco, aggiungere più utenti all'account di un cliente, aggiungere gli utenti di un cliente, caricamento in blocco degli utenti di un cliente, account del cliente, utenti del cliente, utenti
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584244"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Aggiungere più utenti all'account di un cliente

**Si applica a**

-  Centro per i partner

È possibile aggiungere più utenti all'account del cliente in una sola volta, caricando un file di dati nel formato di file delimitati da virgole (CSV) in Partner Center. È possibile scaricare un file di dati di esempio dal centro per i Partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati tramite il modello di dati definito di seguito.

## <a href="" id="creatingtheimportcsvfile"></a>Requisiti dei file di dati


Per aggiungere più utenti all'account di un cliente con il processo di caricamento in blocco, dovrai soddisfare i requisiti seguenti:

-   Devi avere le autorizzazioni di amministratore globale per l'account del cliente;
-   Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;
-   Puoi caricare fino a 100 record alla volta. Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.
-   Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.
-   Immetti solo i dati descritti di seguito. La presenza di dati estranei causerà l'esito negativo del caricamento.

Immetti i dati seguenti nel file di dati:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nome della colonna** | **Descrizione**                                                              | **Limitazione**                             |
| Nome      | Nome dell'utente (campo facoltativo)                                           | Limite di 50 caratteri                         |
| Cognome       | Cognome dell'utente (campo facoltativo)                                            | Limite di 50 caratteri                         |
| Nome visualizzato    | Nome visualizzato nel centro per i Partner (campo obbligatorio)                            | Limite di 50 caratteri                         |
| Posta elettronica           | Indirizzo e-mail aziendale dell'utente presso l'azienda del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo e-mail univoco |
| Aggiornamento stato   | Usato per indicare se il nuovo record utente è stato o meno creato correttamente | \*\*Lasciare vuoto\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Per creare più account utente

<a href="" id="creatingtheaccounts"></a>
1.  Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo.
2.  Dal **Centro per i Partner** dal menu **clienti**, quindi scegliere un cliente dall'elenco.
3.  Seleziona **Carica utenti**.
4.  In **Carica informazioni utenti** seleziona **Sfoglia**.
5.  Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.
6.  Seleziona **Convalida**.

    **Nota**  la maggior parte degli errori di creazione di account sono causati da problemi di file di dati, tra cui mancano informazioni, indirizzi di posta elettronica in formato non valido o duplicato o troppi record nel file.

7.  Dopo che il Partner Center ha convalidato il file, selezionare geografici **posizione** per i nuovi utenti.
8.  Seleziona **Salva**.
9.  Scarica le informazioni sulle password temporanee per gli utenti.

**IMPORTANTE:** Assicurarsi di scaricare il file con le password temporanee ora sarà possibile eseguire questa operazione in un secondo momento. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

10. Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni **può usare licenze e servizi**. 

 

 



