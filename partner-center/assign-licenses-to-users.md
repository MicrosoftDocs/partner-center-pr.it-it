---
title: Gestire gli utenti per gli account cliente
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gestire gli utenti per i clienti nel centro per i partner: creare account utente, aggiungere o rimuovere licenze utente, reimpostare le password ed eliminare o ripristinare gli account utente.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756088"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="3e172-103">Gestire utenti e licenze utente per gli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="3e172-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="3e172-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="3e172-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3e172-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="3e172-105">Global admin</span></span>
- <span data-ttu-id="3e172-106">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="3e172-106">User management admin</span></span>
- <span data-ttu-id="3e172-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="3e172-107">Admin agent</span></span>


<span data-ttu-id="3e172-108">È possibile creare ed eliminare nuovi utenti nell'account di un cliente.</span><span class="sxs-lookup"><span data-stu-id="3e172-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="3e172-109">È anche possibile ripristinare uno o più account utente eliminati in precedenza entro 30 giorni dall'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="3e172-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="3e172-110">Verranno ripristinate anche le assegnazioni di sottoscrizioni precedenti dell'utente (supponendo che le allocazioni precedenti siano disponibili).</span><span class="sxs-lookup"><span data-stu-id="3e172-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="3e172-111">Quando si acquistano nuove sottoscrizioni per un cliente, il cliente deve fornire un elenco di tutti gli utenti che necessitano di account, le relative autorizzazioni utente e i servizi necessari per ogni utente.</span><span class="sxs-lookup"><span data-stu-id="3e172-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="3e172-112">La sezione **utenti e licenze** della scheda **cliente** Mostra tutti gli utenti creati nel tenant di un cliente specifico, inclusi gli utenti con licenze acquistate da un altro partner CSP o da un altro canale di acquisto.</span><span class="sxs-lookup"><span data-stu-id="3e172-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="3e172-113">È possibile [assegnare sottoscrizioni a più utenti](bulk-license-provisioning-for-multiple-users.md) contemporaneamente importando i nomi usando un [file foglio di calcolo con estensione CSV compatibile con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="3e172-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="3e172-114">Creare account utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="3e172-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="3e172-115">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="3e172-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3e172-116">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3e172-117">Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).</span><span class="sxs-lookup"><span data-stu-id="3e172-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3e172-118">Per ogni utente aggiunto, selezionare **Aggiungi sottoscrizione**, quindi compilare le informazioni, incluse le autorizzazioni e le licenze.</span><span class="sxs-lookup"><span data-stu-id="3e172-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="3e172-119">**Salvare** le modifiche.</span><span class="sxs-lookup"><span data-stu-id="3e172-119">**Save** your changes.</span></span>

5. <span data-ttu-id="3e172-120">Assicurati di registrare il nome utente e una password temporanea da inviare all'utente.</span><span class="sxs-lookup"><span data-stu-id="3e172-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="3e172-121">Se si aggiungono più utenti uno alla volta, usare **Aggiungi un altro utente**.</span><span class="sxs-lookup"><span data-stu-id="3e172-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="3e172-122">È anche possibile aggiungere contemporaneamente più utenti [importando un file foglio di calcolo CSV compatibile con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="3e172-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="3e172-123">È possibile attendere fino a quando non viene completato l'intero set prima di inviare tramite posta elettronica o stampare i nomi e le password dalla schermata di conferma.</span><span class="sxs-lookup"><span data-stu-id="3e172-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="3e172-124">Aggiungere o rimuovere licenze utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="3e172-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="3e172-125">I passaggi seguenti riguardano l'aggiunta o la rimozione di licenze utente per i prodotti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3e172-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="3e172-126">Per aggiungere o rimuovere le licenze utente per le sottoscrizioni SaaS basate su licenza nel Marketplace commerciale, vedere [aggiungere o rimuovere licenze per una sottoscrizione Saas](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="3e172-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="3e172-127">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="3e172-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3e172-128">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3e172-129">Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).</span><span class="sxs-lookup"><span data-stu-id="3e172-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3e172-130">Seleziona uno o più utenti nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-130">Choose one or more users from the list.</span></span> <span data-ttu-id="3e172-131">Ad esempio, se il cliente ha appena acquistato nuove licenze e vuoi assegnarle agli utenti che ancora non le hanno, puoi usare l'opzione **Filtra utenti in base a** per trovare il gruppo corretto.</span><span class="sxs-lookup"><span data-stu-id="3e172-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="3e172-132">Seleziona **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="3e172-132">Select **Manage licenses**.</span></span> <span data-ttu-id="3e172-133">Apporta le modifiche e quindi fai clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="3e172-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="3e172-134">Per i [prodotti Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto.</span><span class="sxs-lookup"><span data-stu-id="3e172-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="3e172-135">Reimpostare la password di un utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="3e172-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="3e172-136">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="3e172-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3e172-137">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3e172-138">Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).</span><span class="sxs-lookup"><span data-stu-id="3e172-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3e172-139">Scegliere l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="3e172-140">Nella parte inferiore della schermata fai clic su **Reimposta password**.</span><span class="sxs-lookup"><span data-stu-id="3e172-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="3e172-141">Invia la nuova password temporanea all'utente.</span><span class="sxs-lookup"><span data-stu-id="3e172-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="3e172-142">Eliminare account utente per un cliente</span><span class="sxs-lookup"><span data-stu-id="3e172-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="3e172-143">Scegliere **clienti** dal menu **centro partner** .</span><span class="sxs-lookup"><span data-stu-id="3e172-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3e172-144">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="3e172-145">Nel menu del cliente seleziona **Users and licenses** (Utenti e licenze).</span><span class="sxs-lookup"><span data-stu-id="3e172-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3e172-146">Scegliere l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="3e172-147">Nella parte inferiore della schermata selezionare **Elimina account utente**.</span><span class="sxs-lookup"><span data-stu-id="3e172-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="3e172-148">Se è necessario ripristinare l'account, è possibile trovarlo nella scheda **utenti eliminati** dell'elenco **utenti e licenze** del cliente.</span><span class="sxs-lookup"><span data-stu-id="3e172-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="3e172-149">Sono disponibili 30 giorni per ripristinare un utente eliminato.</span><span class="sxs-lookup"><span data-stu-id="3e172-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="3e172-150">Ripristinare account utente eliminati</span><span class="sxs-lookup"><span data-stu-id="3e172-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="3e172-151">Dal menu **centro** per i partner selezionare **Customers**, quindi scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="3e172-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="3e172-152">Selezionare **utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="3e172-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="3e172-153">Selezionare la scheda **utenti eliminati ()** . Deve leggere **(1)** o versione successiva quando sono presenti utenti eliminati che possono essere ripristinati.</span><span class="sxs-lookup"><span data-stu-id="3e172-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="3e172-154">Seleziona una o più caselle di controllo degli utenti eliminati e quindi seleziona **Ripristina**.</span><span class="sxs-lookup"><span data-stu-id="3e172-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="3e172-155">Tutti gli account utente selezionati verranno nuovamente visualizzati nella pagina **Utenti e licenze**.</span><span class="sxs-lookup"><span data-stu-id="3e172-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3e172-156">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="3e172-156">Next steps</span></span>

- [<span data-ttu-id="3e172-157">Assegnare o revocare licenze a più utenti</span><span class="sxs-lookup"><span data-stu-id="3e172-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="3e172-158">Creare più utenti per l'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="3e172-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)