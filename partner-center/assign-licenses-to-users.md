---
title: Gestire gli utenti per gli account dei clienti
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gestire gli utenti per i clienti in Partner Center: creare account utente, aggiungere o rimuovere licenze utente, reimpostare le password ed eliminare o ripristinare gli account utente.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149894"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gestire utenti e licenze utente per gli account dei clienti 

**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente amministratore


È possibile creare ed eliminare nuovi utenti nell'account di un cliente. È anche possibile ripristinare uno o più account utente eliminati in precedenza entro 30 giorni dall'eliminazione. Verranno ripristinate anche le assegnazioni di sottoscrizioni precedenti dell'utente (supponendo che le allocazioni precedenti siano disponibili).

Quando si acquistano nuove sottoscrizioni per un cliente, il cliente deve fornire un elenco di tutti gli utenti che necessitano di account, le relative autorizzazioni utente e i servizi necessari per ogni utente.  

>[!NOTE]
>La **sezione Utenti e** licenze della scheda **Cliente** mostra tutti gli utenti creati nel tenant di un cliente specifico, inclusi gli utenti che hanno licenze acquistate da un altro partner CSP o da un altro canale di acquisto.

È possibile [assegnare sottoscrizioni a più utenti](bulk-license-provisioning-for-multiple-users.md) contemporaneamente importando i nomi usando un file di foglio di calcolo csv compatibile con [Excel.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Creare account utente per un cliente

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Nel menu del cliente selezionare **Utenti e licenze.**

4. Per ogni utente aggiunto, selezionare **Aggiungi sottoscrizione** e quindi immettere le informazioni, incluse le autorizzazioni e le licenze. **Salvare** le modifiche.

5. Assicurati di registrare il nome utente e una password temporanea da inviare all'utente.

6. Se si aggiungono più utenti uno alla volta, usare **Aggiungi un altro utente**.

7. È anche possibile aggiungere più utenti contemporaneamente [importando un file](adding-multiple-users-to-a-customer-account.md)di foglio di calcolo csv compatibile con Excel. È possibile attendere il completamento dell'intero set prima di inviare tramite posta elettronica o stampare i nomi e le password dalla schermata di conferma.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Aggiungere o rimuovere licenze utente per un cliente

I passaggi seguenti si applicano all'aggiunta o alla rimozione di licenze utente per i prodotti Microsoft. Per aggiungere o rimuovere licenze utente per sottoscrizioni SaaS basate su licenza nel marketplace commerciale, vedere Aggiungere o rimuovere licenze [per una sottoscrizione SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Nel menu del cliente selezionare **Utenti e licenze.**

4. Seleziona uno o più utenti nell'elenco. Se, ad esempio, il cliente ha appena acquistato nuove licenze e si vuole assegnarle a persone che non le hanno ancora, è possibile usare l'opzione Filtra utenti **per...** per trovare il gruppo giusto.

5. Seleziona **Gestisci licenze**. Apportare le modifiche e quindi **salvare**.

> [!NOTE]
> Per [Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Reimpostare la password di un utente per un cliente

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Nel menu del cliente selezionare **Utenti e licenze.** Scegliere l'utente dall'elenco.

4. Nella parte inferiore della schermata fai clic su **Reimposta password**. 

5. Invia la nuova password temporanea all'utente.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Eliminare account utente per un cliente

1. Dal menu **Partner Center** selezionare **Clienti.** Scegliere il cliente dall'elenco.

2. Nel menu del cliente selezionare **Utenti e licenze.** Scegliere l'utente dall'elenco.

3. Nella parte inferiore della schermata selezionare **Elimina account utente**.

Se è necessario ripristinare questo account, è possibile trovarlo nella scheda **Utenti** eliminati dell'elenco **Utenti e licenze del** cliente. Il ripristino di un utente eliminato è di 30 giorni.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Ripristinare account utente eliminati

1. Dal menu **Partner Center** selezionare **Clienti** e quindi scegliere il cliente dall'elenco.

2. Selezionare **Utenti e licenze.**

3. Selezionare la **scheda Utenti eliminati (** ). Dovrebbe leggere **(1)** o superiore quando sono presenti utenti eliminati che possono essere ripristinati.

4. Seleziona una o più caselle di controllo degli utenti eliminati e quindi seleziona **Ripristina**.

    Tutti gli account utente selezionati verranno nuovamente visualizzati nella pagina **Utenti e licenze**.

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare o revocare licenze a più utenti](bulk-license-provisioning-for-multiple-users.md)

- [Creare più utenti per l'account di un cliente](adding-multiple-users-to-a-customer-account.md)