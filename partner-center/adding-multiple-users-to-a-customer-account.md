---
title: Creare più utenti per l'account di un cliente | Centro per i partner
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere più utenti all'account di un cliente contemporaneamente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: jasonwhowell
ms.author: jasonh
keywords: caricamento in blocco, aggiungere più utenti all'account di un cliente, aggiungere gli utenti di un cliente, caricamento in blocco degli utenti di un cliente, account del cliente, utenti del cliente, utenti
ms.localizationpriority: medium
ms.openlocfilehash: 499aff67d18b0d8f9fbaf098fecbab2d888d9ac7
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390370"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="9a13d-104">Aggiungere più utenti all'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="9a13d-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="9a13d-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="9a13d-105">**Applies to**</span></span>

- <span data-ttu-id="9a13d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="9a13d-106">Partner Center</span></span>

<span data-ttu-id="9a13d-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="9a13d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="9a13d-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9a13d-108">Global admin</span></span>

<span data-ttu-id="9a13d-109">È possibile aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9a13d-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="9a13d-110">È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="9a13d-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="9a13d-111">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="9a13d-111">Data file requirements</span></span>

<span data-ttu-id="9a13d-112">Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="9a13d-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="9a13d-113">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="9a13d-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="9a13d-114">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="9a13d-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="9a13d-115">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="9a13d-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="9a13d-116">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="9a13d-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="9a13d-117">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="9a13d-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="9a13d-118">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="9a13d-118">Enter only the data described below.</span></span> <span data-ttu-id="9a13d-119">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="9a13d-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="9a13d-120">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="9a13d-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="9a13d-121">**Nome colonna**</span><span class="sxs-lookup"><span data-stu-id="9a13d-121">**Column name**</span></span> | <span data-ttu-id="9a13d-122">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="9a13d-122">**Description**</span></span>                                                              | <span data-ttu-id="9a13d-123">**Limitazione**</span><span class="sxs-lookup"><span data-stu-id="9a13d-123">**Limitation**</span></span>                             |
| <span data-ttu-id="9a13d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9a13d-124">First name</span></span>      | <span data-ttu-id="9a13d-125">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="9a13d-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="9a13d-126">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="9a13d-126">50-character limit</span></span>                         |
| <span data-ttu-id="9a13d-127">Cognome</span><span class="sxs-lookup"><span data-stu-id="9a13d-127">Last name</span></span>       | <span data-ttu-id="9a13d-128">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="9a13d-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="9a13d-129">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="9a13d-129">50-character limit</span></span>                         |
| <span data-ttu-id="9a13d-130">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="9a13d-130">Display name</span></span>    | <span data-ttu-id="9a13d-131">Nome visualizzato nel centro per i partner (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="9a13d-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="9a13d-132">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="9a13d-132">50-character limit</span></span>                         |
| <span data-ttu-id="9a13d-133">Posta elettronica</span><span class="sxs-lookup"><span data-stu-id="9a13d-133">Email</span></span>           | <span data-ttu-id="9a13d-134">Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="9a13d-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="9a13d-135">Ogni utente deve avere un indirizzo e-mail univoco</span><span class="sxs-lookup"><span data-stu-id="9a13d-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="9a13d-136">Aggiornamento stato</span><span class="sxs-lookup"><span data-stu-id="9a13d-136">Status update</span></span>   | <span data-ttu-id="9a13d-137">Usato per indicare se il nuovo record utente è stato o meno creato correttamente</span><span class="sxs-lookup"><span data-stu-id="9a13d-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="9a13d-138">\*\*lasciare vuoti\*\*</span><span class="sxs-lookup"><span data-stu-id="9a13d-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="9a13d-139">Per creare più account utente</span><span class="sxs-lookup"><span data-stu-id="9a13d-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="9a13d-140">Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra.</span><span class="sxs-lookup"><span data-stu-id="9a13d-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="9a13d-141">Salva il file in modo da poterlo visualizzare in un passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="9a13d-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="9a13d-142">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9a13d-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="9a13d-143">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="9a13d-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="9a13d-144">Selezionare la scheda **utenti e licenze** del cliente, quindi selezionare **carica utenti**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="9a13d-145">In **Carica informazioni utenti** seleziona **Sfoglia**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="9a13d-146">Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="9a13d-147">Seleziona **Convalida**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-147">Select **Validate**.</span></span>

    <span data-ttu-id="9a13d-148">**Si noti**  la maggior parte degli errori di creazione dell'account sono causati da problemi relativi a file di dati, ad esempio informazioni mancanti, indirizzi di posta elettronica non validi o duplicati oppure troppi record nel file.</span><span class="sxs-lookup"><span data-stu-id="9a13d-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="9a13d-149">Dopo che il centro per i partner ha convalidato il file, selezionare la **posizione** geografica per i nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="9a13d-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="9a13d-150">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-150">Select **Save**.</span></span>
10. <span data-ttu-id="9a13d-151">Scarica le informazioni sulle password temporanee per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="9a13d-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="9a13d-152">**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito.</span><span class="sxs-lookup"><span data-stu-id="9a13d-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="9a13d-153">I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.</span><span class="sxs-lookup"><span data-stu-id="9a13d-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="9a13d-154">Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni **può usare licenze e servizi**.</span><span class="sxs-lookup"><span data-stu-id="9a13d-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



