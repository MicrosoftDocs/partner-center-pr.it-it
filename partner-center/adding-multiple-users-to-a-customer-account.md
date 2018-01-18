---
title: "Creare più utenti per l'account di un cliente | Centro per i partner"
description: "Puoi aggiungere più utenti contemporaneamente all'account di un cliente caricando un file di dati con valori delimitati da virgole (CSV) nel Centro per i partner."
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: "caricamento in blocco, aggiungere più utenti all'account di un cliente, aggiungere gli utenti di un cliente, caricamento in blocco degli utenti di un cliente, account del cliente, utenti del cliente, utenti"
ms.openlocfilehash: b360ced878973cde19b1a6aa8470ac4218ea6773
ms.sourcegitcommit: e01a63d8b778668c560bc821275ddfcb0a6d4881
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2017
---
# <a name="add-multiple-users-to-a-customer-account"></a>Aggiungere più utenti all'account di un cliente

**Si applica a**

-  Centro per i partner

Puoi aggiungere più utenti contemporaneamente all'account di un cliente caricando un file di dati con valori delimitati da virgole (CSV) nel Centro per i partner. Puoi scaricare un file di dati di esempio dal Centro per i partner e quindi modificarlo per i tuoi scopi oppure puoi creare un nuovo file di dati usando il modello di dati definito di seguito.

## <a href="" id="creatingtheimportcsvfile"></a>Requisiti per i file di dati


Per aggiungere più utenti all'account di un cliente con il processo di caricamento in blocco, dovrai soddisfare i requisiti seguenti:

-   Devi avere le autorizzazioni di amministratore globale per l'account del cliente;
-   Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;
-   Puoi caricare fino a 100 record alla volta. Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.
-   Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.
-   Immetti solo i dati descritti di seguito. La presenza di dati estranei causerà l'esito negativo del caricamento.

Immetti i dati seguenti nel file di dati:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nome colonna** | **Descrizione**                                                              | **Limitazione**                             |
| Nome      | Nome dell'utente (campo facoltativo)                                           | Limite di 50 caratteri                         |
| Cognome       | Cognome dell'utente (campo facoltativo)                                            | Limite di 50 caratteri                         |
| Nome visualizzato    | Nome visualizzato nel Centro per i partner (campo obbligatorio)                            | Limite di 50 caratteri                         |
| E-mail           | Indirizzo e-mail aziendale dell'utente presso l'azienda del cliente (campo obbligatorio)           | Ogni utente deve avere un indirizzo e-mail univoco |
| Aggiornamento stato   | Usato per indicare se il nuovo record utente è stato o meno creato correttamente | \*\*Lasciare vuoto\*\*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Per creare più account utente

<a href="" id="creatingtheaccounts"></a>
1.  Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo.
2.  Nel menu **Dashboard** seleziona **Clienti** e quindi scegli un cliente nell'elenco.
3.  Seleziona **Carica utenti**.
4.  In **Carica informazioni utenti** seleziona **Sfoglia**.
5.  Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.
6.  Seleziona **Convalida**.

    **Nota** La maggior parte degli errori di creazione di account sono causati da problemi del file di dati, tra cui informazioni mancanti, indirizzi e-mail non validi o duplicati o troppi record nel file.

     

7.  Dopo la convalida del file da parte del Centro per i partner, seleziona la **Posizione** geografica per i nuovi utenti.
8.  Seleziona **Salva**.
9.  Scarica le informazioni sulle password temporanee per gli utenti.

**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

Il Centro per i partner assegna automaticamente le autorizzazioni **può usare licenze e servizi** ai nuovi utenti.

 

 



