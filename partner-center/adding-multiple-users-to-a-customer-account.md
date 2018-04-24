---
title: Creare più utenti per l'account di un cliente | Centro per i partner
description: Puoi aggiungere più utenti contemporaneamente all'account di un cliente caricando un file di dati con valori delimitati da virgole (CSV) nel Centro per i partner.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: caricamento in blocco, aggiungere più utenti all'account di un cliente, aggiungere gli utenti di un cliente, caricamento in blocco degli utenti di un cliente, account del cliente, utenti del cliente, utenti
ms.openlocfilehash: 2c695cd6c6e3b302d91730638358616ca3465188
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/08/2018
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="16c0b-104">Aggiungere più utenti all'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="16c0b-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="16c0b-105">Si applica a</span><span class="sxs-lookup"><span data-stu-id="16c0b-105">Applies to</span></span>**

-  <span data-ttu-id="16c0b-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="16c0b-106">Partner Center</span></span>

<span data-ttu-id="16c0b-107">Puoi aggiungere più utenti contemporaneamente all'account di un cliente caricando un file di dati con valori delimitati da virgole (CSV) nel dashboard del partner.</span><span class="sxs-lookup"><span data-stu-id="16c0b-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Dashboard.</span></span> <span data-ttu-id="16c0b-108">Puoi scaricare un file di dati di esempio dal dashboard del partner e quindi modificarlo per i tuoi scopi oppure puoi creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="16c0b-108">You can download a sample data file from the Partner Dashboard and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="16c0b-109">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="16c0b-109">Data file requirements</span></span>


<span data-ttu-id="16c0b-110">Per aggiungere più utenti all'account di un cliente con il processo di caricamento in blocco, dovrai soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="16c0b-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="16c0b-111">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="16c0b-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="16c0b-112">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="16c0b-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="16c0b-113">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="16c0b-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="16c0b-114">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="16c0b-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="16c0b-115">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="16c0b-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="16c0b-116">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="16c0b-116">Enter only the data described below.</span></span> <span data-ttu-id="16c0b-117">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="16c0b-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="16c0b-118">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="16c0b-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="16c0b-119">Nome colonna</span><span class="sxs-lookup"><span data-stu-id="16c0b-119">Column name</span></span>** | **<span data-ttu-id="16c0b-120">Descrizione</span><span class="sxs-lookup"><span data-stu-id="16c0b-120">Description</span></span>**                                                              | **<span data-ttu-id="16c0b-121">Limitazione</span><span class="sxs-lookup"><span data-stu-id="16c0b-121">Limitation</span></span>**                             |
| <span data-ttu-id="16c0b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="16c0b-122">First name</span></span>      | <span data-ttu-id="16c0b-123">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="16c0b-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="16c0b-124">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="16c0b-124">50-character limit</span></span>                         |
| <span data-ttu-id="16c0b-125">Cognome</span><span class="sxs-lookup"><span data-stu-id="16c0b-125">Last name</span></span>       | <span data-ttu-id="16c0b-126">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="16c0b-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="16c0b-127">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="16c0b-127">50-character limit</span></span>                         |
| <span data-ttu-id="16c0b-128">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="16c0b-128">Display name</span></span>    | <span data-ttu-id="16c0b-129">Nome visualizzato nel dashboard del partner (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="16c0b-129">Name displayed in the Partner Dashboard (required field)</span></span>                            | <span data-ttu-id="16c0b-130">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="16c0b-130">50-character limit</span></span>                         |
| <span data-ttu-id="16c0b-131">E-mail</span><span class="sxs-lookup"><span data-stu-id="16c0b-131">Email</span></span>           | <span data-ttu-id="16c0b-132">Indirizzo e-mail aziendale dell'utente presso l'azienda del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="16c0b-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="16c0b-133">Ogni utente deve avere un indirizzo e-mail univoco</span><span class="sxs-lookup"><span data-stu-id="16c0b-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="16c0b-134">Aggiornamento stato</span><span class="sxs-lookup"><span data-stu-id="16c0b-134">Status update</span></span>   | <span data-ttu-id="16c0b-135">Usato per indicare se il nuovo record utente è stato o meno creato correttamente</span><span class="sxs-lookup"><span data-stu-id="16c0b-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="16c0b-136">\*\*Lasciare vuoto\*\*</span><span class="sxs-lookup"><span data-stu-id="16c0b-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="16c0b-137">Per creare più account utente</span><span class="sxs-lookup"><span data-stu-id="16c0b-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="16c0b-138">Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra.</span><span class="sxs-lookup"><span data-stu-id="16c0b-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="16c0b-139">Salva il file in modo da poterlo visualizzare in un passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="16c0b-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="16c0b-140">Nel menu **Dashboard** seleziona **Clienti** e quindi scegli un cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="16c0b-140">From the **Dashboard** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="16c0b-141">Seleziona **Carica utenti**.</span><span class="sxs-lookup"><span data-stu-id="16c0b-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="16c0b-142">In **Carica informazioni utenti** seleziona **Sfoglia**.</span><span class="sxs-lookup"><span data-stu-id="16c0b-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="16c0b-143">Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.</span><span class="sxs-lookup"><span data-stu-id="16c0b-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="16c0b-144">Seleziona **Convalida**.</span><span class="sxs-lookup"><span data-stu-id="16c0b-144">Select **Validate**.</span></span>

    <span data-ttu-id="16c0b-145">**Nota** La maggior parte degli errori di creazione di account sono causati da problemi del file di dati, tra cui informazioni mancanti, indirizzi e-mail non validi o duplicati o troppi record nel file.</span><span class="sxs-lookup"><span data-stu-id="16c0b-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

     

7.  <span data-ttu-id="16c0b-146">Una volta convalidato il file nel dashboard del partner, seleziona la **Posizione** geografica per i nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="16c0b-146">After the Partner Dashboard validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="16c0b-147">Seleziona **Salva**.</span><span class="sxs-lookup"><span data-stu-id="16c0b-147">Select **Save**.</span></span>
9.  <span data-ttu-id="16c0b-148">Scarica le informazioni sulle password temporanee per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="16c0b-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="16c0b-149">**IMPORTANTE:** assicurati di scaricare il file con le password temporanee in questo momento, perché non potrai farlo in seguito.</span><span class="sxs-lookup"><span data-stu-id="16c0b-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="16c0b-150">I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.</span><span class="sxs-lookup"><span data-stu-id="16c0b-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

<span data-ttu-id="16c0b-151">Il dashboard del partner assegna automaticamente le autorizzazioni **può usare licenze e servizi** ai nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="16c0b-151">the Partner Dashboard automatically assigns permissions of **Can use licenses and services** to the new users.</span></span>

 

 



