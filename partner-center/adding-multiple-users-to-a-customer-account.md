---
title: Aggiungere più utenti per un account cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti a un account del cliente, caricare un file di dati nel centro per i partner usando il formato di file con valori delimitati da virgole (CSV).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535741"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Carica un file CSV di utenti nell'account di un cliente


**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

Aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Creare il file degli utenti del cliente e caricarlo nell'account del cliente

1. Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo. Per [importare più utenti per un account cliente, vedere campi per il file con estensione CSV](file-customer-users.md). 

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

    >[!IMPORTANT]
    > Assicurarsi di scaricare il file con le password temporanee perché non sarà possibile eseguire questa operazione in un secondo momento. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

11. Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni di **che possono usare licenze e servizi** . 

## <a name="next-steps"></a>Passaggi successivi

- [Concedere ai clienti l'autorizzazione per il centro per i partner per acquistare prodotti o servizi propri](give-customers-permission.md)
