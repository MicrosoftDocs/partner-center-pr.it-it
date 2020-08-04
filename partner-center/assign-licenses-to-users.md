---
title: Gestire gli utenti negli account cliente
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come creare gli account utente per un cliente, aggiungere o rimuovere licenze utente, reimpostare le password utente, eliminare gli account utente o ripristinarli.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527677"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a>Attività di gestione degli utenti per gli account cliente nel centro per i partner

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore gestione utenti
- Agente amministratore
- Agente di vendita
- Agente di supporto tecnico

È possibile creare ed eliminare nuovi utenti nell'account di un cliente. È anche possibile ripristinare uno o più account utente eliminati in precedenza entro 30 giorni dall'eliminazione. Verranno ripristinate anche le assegnazioni di sottoscrizioni precedenti dell'utente (supponendo che le allocazioni precedenti siano disponibili).

Quando si acquistano nuove sottoscrizioni per un cliente, il cliente deve fornire un elenco di tutti gli utenti che necessitano di account, le relative autorizzazioni utente e i servizi necessari per ogni utente.  

È possibile [assegnare sottoscrizioni a più utenti](bulk-license-provisioning-for-multiple-users.md) contemporaneamente importando i nomi usando un [file foglio di calcolo con estensione CSV compatibile con Excel](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Creare account utente per un cliente

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).

4. Per ogni utente aggiunto, selezionare **Aggiungi sottoscrizione**, quindi compilare le informazioni, incluse le autorizzazioni e le licenze. **Salvare** le modifiche.

5. Assicurati di registrare il nome utente e una password temporanea da inviare all'utente.

6. Se si aggiungono più utenti uno alla volta, usare **Aggiungi un altro utente**.

7. È anche possibile aggiungere contemporaneamente più utenti [importando un file foglio di calcolo CSV compatibile con Excel](adding-multiple-users-to-a-customer-account.md). È possibile attendere fino a quando non viene completato l'intero set prima di inviare tramite posta elettronica o stampare i nomi e le password dalla schermata di conferma.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Aggiungere o rimuovere licenze utente per un cliente

I passaggi seguenti riguardano l'aggiunta o la rimozione di licenze utente per i prodotti Microsoft. Per aggiungere o rimuovere le licenze utente per le sottoscrizioni SaaS basate su licenza nel Marketplace commerciale, vedere [aggiungere o rimuovere licenze per una sottoscrizione Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).

4. Seleziona uno o più utenti nell'elenco. Ad esempio, se il cliente ha appena acquistato nuove licenze e vuoi assegnarle agli utenti che ancora non le hanno, puoi usare l'opzione **Filtra utenti in base a** per trovare il gruppo corretto.

5. Seleziona **Gestisci licenze**. Apporta le modifiche e quindi fai clic su **Salva**.

> [!NOTE]
> Per i [prodotti Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Reimpostare la password di un utente per un cliente

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3.  Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze). Scegliere l'utente dall'elenco.

4.  Nella parte inferiore della schermata fai clic su **Reimposta password**. 

5.  Invia la nuova password temporanea all'utente.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Eliminare account utente per un cliente

1.  Scegliere **clienti**dal menu **centro partner** . Scegliere il cliente dall'elenco.

2.  Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze). Scegliere l'utente dall'elenco.

3.  Nella parte inferiore della schermata selezionare **Elimina account utente**.

Se è necessario ripristinare l'account, è possibile trovarlo nella scheda **utenti eliminati** dell'elenco **utenti e licenze** del cliente. Sono disponibili 30 giorni per ripristinare un utente eliminato.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Ripristinare account utente eliminati

1.  Dal menu **centro** per i partner selezionare **Customers**, quindi scegliere il cliente dall'elenco.

2.  Selezionare **utenti e licenze**.

3.  Selezionare la scheda **utenti eliminati ()** . Deve leggere **(1)** o versione successiva quando sono presenti utenti eliminati che possono essere ripristinati.

4.  Seleziona una o più caselle di controllo degli utenti eliminati e quindi seleziona **Ripristina**.

    Tutti gli account utente selezionati verranno nuovamente visualizzati nella pagina **Utenti e licenze**.

## <a name="related-topics"></a>Argomenti correlati


[Assegnare o revocare licenze a più utenti](bulk-license-provisioning-for-multiple-users.md)

[Creare più utenti per l'account di un cliente](adding-multiple-users-to-a-customer-account.md)