---
title: Aggiungere più utenti per un account cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti all'account di un cliente, caricare un file di dati Partner Center usando il formato di file con valori delimitati da virgole (csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150472"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Caricare un file CSV di utenti nell'account di un cliente


**Ruoli appropriati:** Amministratore globale

Aggiungere contemporaneamente più utenti all'account di un cliente caricando un file di dati nel formato di file con valori delimitati da virgole (csv) nel Partner Center. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Creare il file degli utenti dei clienti e caricarlo nell'account del cliente

1. Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra. Salva il file in modo da poterlo visualizzare in un passaggio successivo. Vedere [Campi per il file CSV per importare più utenti per un account cliente.](file-customer-users.md) 

2. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

3. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

4. Selezionare la scheda Utenti e licenze **del** cliente e quindi **selezionare Carica utenti**.

5. In **Carica informazioni utenti** seleziona **Sfoglia**.

6. Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.

7. Selezionare **Convalida**.

    **Nota**  La maggior parte degli errori di creazione dell'account è causata da problemi del file di dati, tra cui informazioni mancanti, indirizzi di posta elettronica in formato non valido o duplicati o troppi record nel file.

8. Dopo aver Partner Center convalidare il file, selezionare la località **geografica** per i nuovi utenti.
9. Selezionare **Salva**.
10. Scaricare le informazioni sulla password temporanea per gli utenti.

    >[!IMPORTANT]
    > Assicurarsi di scaricare il file con le password temporanee ora perché non sarà possibile eseguire questa operazione in un secondo momento. I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.

11. Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni **di Può usare licenze e servizi**. 

## <a name="next-steps"></a>Passaggi successivi

- [Concedere ai clienti l'autorizzazione Partner Center acquistare i propri prodotti o servizi](give-customers-permission.md)
