---
title: Aggiungere più utenti per un account cliente
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere più utenti all'account di un cliente in una sola volta. Caricare un file di dati nel centro per i partner usando il formato di file con valori delimitati da virgole (CSV).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436310"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="226b3-104">Aggiungere più utenti a un account cliente: caricare un file di dati nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="226b3-104">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="226b3-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="226b3-105">**Applies to**</span></span>

- <span data-ttu-id="226b3-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="226b3-106">Partner Center</span></span>

<span data-ttu-id="226b3-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="226b3-107">**Appropriate roles**</span></span>

- <span data-ttu-id="226b3-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="226b3-108">Global admin</span></span>

<span data-ttu-id="226b3-109">È possibile aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="226b3-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="226b3-110">È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="226b3-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="226b3-111">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="226b3-111">Data file requirements</span></span>

<span data-ttu-id="226b3-112">Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="226b3-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="226b3-113">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="226b3-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="226b3-114">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="226b3-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="226b3-115">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="226b3-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="226b3-116">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="226b3-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="226b3-117">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="226b3-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="226b3-118">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="226b3-118">Enter only the data described below.</span></span> <span data-ttu-id="226b3-119">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="226b3-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="226b3-120">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="226b3-120">Enter the following data in the data file:</span></span>

| <span data-ttu-id="226b3-121">**Nome colonna**</span><span class="sxs-lookup"><span data-stu-id="226b3-121">**Column name**</span></span> | <span data-ttu-id="226b3-122">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="226b3-122">**Description**</span></span>  | <span data-ttu-id="226b3-123">**Limitazione**</span><span class="sxs-lookup"><span data-stu-id="226b3-123">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="226b3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="226b3-124">First name</span></span>  | <span data-ttu-id="226b3-125">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="226b3-125">User's first name (optional field)</span></span>  | <span data-ttu-id="226b3-126">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="226b3-126">50-character limit</span></span>  |
| <span data-ttu-id="226b3-127">Cognome</span><span class="sxs-lookup"><span data-stu-id="226b3-127">Last name</span></span>  | <span data-ttu-id="226b3-128">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="226b3-128">User's last name (optional field)</span></span>  | <span data-ttu-id="226b3-129">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="226b3-129">50-character limit</span></span>  |
| <span data-ttu-id="226b3-130">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="226b3-130">Display name</span></span>    | <span data-ttu-id="226b3-131">Nome visualizzato nel centro per i partner (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="226b3-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="226b3-132">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="226b3-132">50-character limit</span></span>                         |
| <span data-ttu-id="226b3-133">E-mail</span><span class="sxs-lookup"><span data-stu-id="226b3-133">Email</span></span>   | <span data-ttu-id="226b3-134">Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="226b3-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="226b3-135">Ogni utente deve avere un indirizzo di posta elettronica univoco</span><span class="sxs-lookup"><span data-stu-id="226b3-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="226b3-136">Aggiornamento dello stato</span><span class="sxs-lookup"><span data-stu-id="226b3-136">Status update</span></span>   | <span data-ttu-id="226b3-137">Usato per indicare se il nuovo record utente è stato o meno creato correttamente</span><span class="sxs-lookup"><span data-stu-id="226b3-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="226b3-138">\*\*Lascia vuoto\*\*</span><span class="sxs-lookup"><span data-stu-id="226b3-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="226b3-139">Per creare più account utente</span><span class="sxs-lookup"><span data-stu-id="226b3-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="226b3-140">Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra.</span><span class="sxs-lookup"><span data-stu-id="226b3-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="226b3-141">Salva il file in modo da poterlo visualizzare in un passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="226b3-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="226b3-142">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="226b3-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="226b3-143">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="226b3-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="226b3-144">Selezionare la scheda **utenti e licenze** del cliente, quindi selezionare **carica utenti**.</span><span class="sxs-lookup"><span data-stu-id="226b3-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="226b3-145">In **Carica informazioni utenti** seleziona **Sfoglia**.</span><span class="sxs-lookup"><span data-stu-id="226b3-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="226b3-146">Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.</span><span class="sxs-lookup"><span data-stu-id="226b3-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="226b3-147">Selezionare **Convalida**.</span><span class="sxs-lookup"><span data-stu-id="226b3-147">Select **Validate**.</span></span>

    <span data-ttu-id="226b3-148">**Nota**    La maggior parte degli errori di creazione dell'account è causata da problemi relativi ai file di dati, tra cui informazioni mancanti, indirizzi di posta elettronica non validi o duplicati o troppi record nel file.</span><span class="sxs-lookup"><span data-stu-id="226b3-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="226b3-149">Dopo che il centro per i partner ha convalidato il file, selezionare la **posizione** geografica per i nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="226b3-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="226b3-150">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="226b3-150">Select **Save**.</span></span>
10. <span data-ttu-id="226b3-151">Scaricare le informazioni sulla password temporanea per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="226b3-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="226b3-152">**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito.</span><span class="sxs-lookup"><span data-stu-id="226b3-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="226b3-153">I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.</span><span class="sxs-lookup"><span data-stu-id="226b3-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="226b3-154">Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni di **che possono usare licenze e servizi** .</span><span class="sxs-lookup"><span data-stu-id="226b3-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



