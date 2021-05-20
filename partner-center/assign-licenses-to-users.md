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
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="040b5-103">Gestire utenti e licenze utente per gli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="040b5-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="040b5-104">**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="040b5-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="040b5-105">È possibile creare ed eliminare nuovi utenti nell'account di un cliente.</span><span class="sxs-lookup"><span data-stu-id="040b5-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="040b5-106">È anche possibile ripristinare uno o più account utente eliminati in precedenza entro 30 giorni dall'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="040b5-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="040b5-107">Verranno ripristinate anche le assegnazioni di sottoscrizioni precedenti dell'utente (supponendo che le allocazioni precedenti siano disponibili).</span><span class="sxs-lookup"><span data-stu-id="040b5-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="040b5-108">Quando si acquistano nuove sottoscrizioni per un cliente, il cliente deve fornire un elenco di tutti gli utenti che necessitano di account, le relative autorizzazioni utente e i servizi necessari per ogni utente.</span><span class="sxs-lookup"><span data-stu-id="040b5-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="040b5-109">La **sezione Utenti e** licenze della scheda **Cliente** mostra tutti gli utenti creati nel tenant di un cliente specifico, inclusi gli utenti che hanno licenze acquistate da un altro partner CSP o da un altro canale di acquisto.</span><span class="sxs-lookup"><span data-stu-id="040b5-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="040b5-110">È possibile [assegnare sottoscrizioni a più utenti](bulk-license-provisioning-for-multiple-users.md) contemporaneamente importando i nomi usando un file di foglio di calcolo csv compatibile con [Excel.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="040b5-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="040b5-111">Creare account utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="040b5-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="040b5-112">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="040b5-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="040b5-113">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="040b5-114">Nel menu del cliente selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="040b5-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="040b5-115">Per ogni utente aggiunto, selezionare **Aggiungi sottoscrizione** e quindi immettere le informazioni, incluse le autorizzazioni e le licenze.</span><span class="sxs-lookup"><span data-stu-id="040b5-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="040b5-116">**Salvare** le modifiche.</span><span class="sxs-lookup"><span data-stu-id="040b5-116">**Save** your changes.</span></span>

5. <span data-ttu-id="040b5-117">Assicurati di registrare il nome utente e una password temporanea da inviare all'utente.</span><span class="sxs-lookup"><span data-stu-id="040b5-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="040b5-118">Se si aggiungono più utenti uno alla volta, usare **Aggiungi un altro utente**.</span><span class="sxs-lookup"><span data-stu-id="040b5-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="040b5-119">È anche possibile aggiungere più utenti contemporaneamente [importando un file](adding-multiple-users-to-a-customer-account.md)di foglio di calcolo csv compatibile con Excel.</span><span class="sxs-lookup"><span data-stu-id="040b5-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="040b5-120">È possibile attendere il completamento dell'intero set prima di inviare tramite posta elettronica o stampare i nomi e le password dalla schermata di conferma.</span><span class="sxs-lookup"><span data-stu-id="040b5-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="040b5-121">Aggiungere o rimuovere licenze utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="040b5-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="040b5-122">I passaggi seguenti si applicano all'aggiunta o alla rimozione di licenze utente per i prodotti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="040b5-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="040b5-123">Per aggiungere o rimuovere licenze utente per sottoscrizioni SaaS basate su licenza nel marketplace commerciale, vedere Aggiungere o rimuovere licenze [per una sottoscrizione SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="040b5-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="040b5-124">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="040b5-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="040b5-125">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="040b5-126">Nel menu del cliente selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="040b5-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="040b5-127">Seleziona uno o più utenti nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-127">Choose one or more users from the list.</span></span> <span data-ttu-id="040b5-128">Se, ad esempio, il cliente ha appena acquistato nuove licenze e si vuole assegnarle a persone che non le hanno ancora, è possibile usare l'opzione Filtra utenti **per...** per trovare il gruppo giusto.</span><span class="sxs-lookup"><span data-stu-id="040b5-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="040b5-129">Seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="040b5-129">Select **Manage licenses**.</span></span> <span data-ttu-id="040b5-130">Apportare le modifiche e quindi **salvare**.</span><span class="sxs-lookup"><span data-stu-id="040b5-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="040b5-131">Per [Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto.</span><span class="sxs-lookup"><span data-stu-id="040b5-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="040b5-132">Reimpostare la password di un utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="040b5-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="040b5-133">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="040b5-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="040b5-134">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="040b5-135">Nel menu del cliente selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="040b5-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="040b5-136">Scegliere l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="040b5-137">Nella parte inferiore della schermata fai clic su **Reimposta password**.</span><span class="sxs-lookup"><span data-stu-id="040b5-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="040b5-138">Invia la nuova password temporanea all'utente.</span><span class="sxs-lookup"><span data-stu-id="040b5-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="040b5-139">Eliminare account utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="040b5-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="040b5-140">Dal menu **Partner Center** selezionare **Clienti.**</span><span class="sxs-lookup"><span data-stu-id="040b5-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="040b5-141">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="040b5-142">Nel menu del cliente selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="040b5-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="040b5-143">Scegliere l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="040b5-144">Nella parte inferiore della schermata selezionare **Elimina account utente**.</span><span class="sxs-lookup"><span data-stu-id="040b5-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="040b5-145">Se è necessario ripristinare questo account, è possibile trovarlo nella scheda **Utenti** eliminati dell'elenco **Utenti e licenze del** cliente.</span><span class="sxs-lookup"><span data-stu-id="040b5-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="040b5-146">Il ripristino di un utente eliminato è di 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="040b5-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="040b5-147">Ripristinare account utente eliminati</span><span class="sxs-lookup"><span data-stu-id="040b5-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="040b5-148">Dal menu **Partner Center** selezionare **Clienti** e quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="040b5-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="040b5-149">Selezionare **Utenti e licenze.**</span><span class="sxs-lookup"><span data-stu-id="040b5-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="040b5-150">Selezionare la **scheda Utenti eliminati (** ). Dovrebbe leggere **(1)** o superiore quando sono presenti utenti eliminati che possono essere ripristinati.</span><span class="sxs-lookup"><span data-stu-id="040b5-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="040b5-151">Seleziona una o più caselle di controllo degli utenti eliminati e quindi seleziona **Ripristina**.</span><span class="sxs-lookup"><span data-stu-id="040b5-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="040b5-152">Tutti gli account utente selezionati verranno nuovamente visualizzati nella pagina **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="040b5-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="040b5-153">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="040b5-153">Next steps</span></span>

- [<span data-ttu-id="040b5-154">Assegnare o revocare licenze a più utenti</span><span class="sxs-lookup"><span data-stu-id="040b5-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="040b5-155">Creare più utenti per l'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="040b5-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)