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
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="4a687-105">Aggiungere più utenti a un account cliente: caricare un file di dati nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="4a687-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="4a687-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="4a687-106">**Applies to**</span></span>

- <span data-ttu-id="4a687-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="4a687-107">Partner Center</span></span>

<span data-ttu-id="4a687-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="4a687-108">**Appropriate roles**</span></span>

- <span data-ttu-id="4a687-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="4a687-109">Global admin</span></span>

<span data-ttu-id="4a687-110">È possibile aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="4a687-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="4a687-111">È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="4a687-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="4a687-112">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="4a687-112">Data file requirements</span></span>

<span data-ttu-id="4a687-113">Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="4a687-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="4a687-114">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="4a687-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="4a687-115">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="4a687-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="4a687-116">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="4a687-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="4a687-117">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="4a687-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="4a687-118">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="4a687-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="4a687-119">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="4a687-119">Enter only the data described below.</span></span> <span data-ttu-id="4a687-120">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="4a687-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="4a687-121">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="4a687-121">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="4a687-122">**Nome colonna**</span><span class="sxs-lookup"><span data-stu-id="4a687-122">**Column name**</span></span> | <span data-ttu-id="4a687-123">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="4a687-123">**Description**</span></span>                                                              | <span data-ttu-id="4a687-124">**Limitazione**</span><span class="sxs-lookup"><span data-stu-id="4a687-124">**Limitation**</span></span>                             |
| <span data-ttu-id="4a687-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4a687-125">First name</span></span>      | <span data-ttu-id="4a687-126">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="4a687-126">User's first name (optional field)</span></span>                                           | <span data-ttu-id="4a687-127">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="4a687-127">50-character limit</span></span>                         |
| <span data-ttu-id="4a687-128">Cognome</span><span class="sxs-lookup"><span data-stu-id="4a687-128">Last name</span></span>       | <span data-ttu-id="4a687-129">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="4a687-129">User's last name (optional field)</span></span>                                            | <span data-ttu-id="4a687-130">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="4a687-130">50-character limit</span></span>                         |
| <span data-ttu-id="4a687-131">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="4a687-131">Display name</span></span>    | <span data-ttu-id="4a687-132">Nome visualizzato nel centro per i partner (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="4a687-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="4a687-133">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="4a687-133">50-character limit</span></span>                         |
| <span data-ttu-id="4a687-134">Email</span><span class="sxs-lookup"><span data-stu-id="4a687-134">Email</span></span>           | <span data-ttu-id="4a687-135">Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="4a687-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="4a687-136">Ogni utente deve avere un indirizzo di posta elettronica univoco</span><span class="sxs-lookup"><span data-stu-id="4a687-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="4a687-137">Aggiornamento dello stato</span><span class="sxs-lookup"><span data-stu-id="4a687-137">Status update</span></span>   | <span data-ttu-id="4a687-138">Usato per indicare se il nuovo record utente è stato o meno creato correttamente</span><span class="sxs-lookup"><span data-stu-id="4a687-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="4a687-139">\*\*Lascia vuoto\*\*</span><span class="sxs-lookup"><span data-stu-id="4a687-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="4a687-140">Per creare più account utente</span><span class="sxs-lookup"><span data-stu-id="4a687-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="4a687-141">Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra.</span><span class="sxs-lookup"><span data-stu-id="4a687-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="4a687-142">Salva il file in modo da poterlo visualizzare in un passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="4a687-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="4a687-143">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="4a687-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="4a687-144">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="4a687-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="4a687-145">Selezionare la scheda **utenti e licenze** del cliente, quindi selezionare **carica utenti**.</span><span class="sxs-lookup"><span data-stu-id="4a687-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="4a687-146">In **Carica informazioni utenti** seleziona **Sfoglia**.</span><span class="sxs-lookup"><span data-stu-id="4a687-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="4a687-147">Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.</span><span class="sxs-lookup"><span data-stu-id="4a687-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="4a687-148">Selezionare **Convalida**.</span><span class="sxs-lookup"><span data-stu-id="4a687-148">Select **Validate**.</span></span>

    <span data-ttu-id="4a687-149">**Nota**    La maggior parte degli errori di creazione dell'account è causata da problemi relativi ai file di dati, tra cui informazioni mancanti, indirizzi di posta elettronica non validi o duplicati o troppi record nel file.</span><span class="sxs-lookup"><span data-stu-id="4a687-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="4a687-150">Dopo che il centro per i partner ha convalidato il file, selezionare la **posizione** geografica per i nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="4a687-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="4a687-151">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="4a687-151">Select **Save**.</span></span>
10. <span data-ttu-id="4a687-152">Scaricare le informazioni sulla password temporanea per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="4a687-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="4a687-153">**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito.</span><span class="sxs-lookup"><span data-stu-id="4a687-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="4a687-154">I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.</span><span class="sxs-lookup"><span data-stu-id="4a687-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="4a687-155">Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni di **che possono usare licenze e servizi** .</span><span class="sxs-lookup"><span data-stu-id="4a687-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



