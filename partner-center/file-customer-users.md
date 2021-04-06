---
title: Campi per il file con estensione CSV per l'importazione di più utenti per un account cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti a un account cliente, creare un file con valori delimitati da virgole (CSV) con campi appropriati.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441422"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="f7ac9-103">Aggiungere più utenti a un account cliente creando un file CSV</span><span class="sxs-lookup"><span data-stu-id="f7ac9-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="f7ac9-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="f7ac9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f7ac9-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="f7ac9-105">Global admin</span></span>

<span data-ttu-id="f7ac9-106">Aggiungere contemporaneamente più utenti all'account di un cliente, caricando un file di dati nel formato di file con valori delimitati da virgole (CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="f7ac9-107">È possibile scaricare un file di dati di esempio dal centro per i partner e quindi modificarlo per l'uso, oppure è possibile creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="f7ac9-108">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="f7ac9-108">Data file requirements</span></span>

<span data-ttu-id="f7ac9-109">Per aggiungere più utenti a un account del cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="f7ac9-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="f7ac9-110">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="f7ac9-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="f7ac9-111">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="f7ac9-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="f7ac9-112">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="f7ac9-113">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="f7ac9-114">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="f7ac9-115">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-115">Enter only the data described below.</span></span> <span data-ttu-id="f7ac9-116">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="f7ac9-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="f7ac9-117">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="f7ac9-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="f7ac9-118">**Nome colonna**</span><span class="sxs-lookup"><span data-stu-id="f7ac9-118">**Column name**</span></span> | <span data-ttu-id="f7ac9-119">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="f7ac9-119">**Description**</span></span>  | <span data-ttu-id="f7ac9-120">**Limitazione**</span><span class="sxs-lookup"><span data-stu-id="f7ac9-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="f7ac9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f7ac9-121">First name</span></span>  | <span data-ttu-id="f7ac9-122">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="f7ac9-122">User's first name (optional field)</span></span>  | <span data-ttu-id="f7ac9-123">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="f7ac9-123">50-character limit</span></span>  |
| <span data-ttu-id="f7ac9-124">Cognome</span><span class="sxs-lookup"><span data-stu-id="f7ac9-124">Last name</span></span>  | <span data-ttu-id="f7ac9-125">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="f7ac9-125">User's last name (optional field)</span></span>  | <span data-ttu-id="f7ac9-126">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="f7ac9-126">50-character limit</span></span>  |
| <span data-ttu-id="f7ac9-127">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="f7ac9-127">Display name</span></span>    | <span data-ttu-id="f7ac9-128">Nome visualizzato nel centro per i partner (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="f7ac9-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="f7ac9-129">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="f7ac9-129">50-character limit</span></span>                         |
| <span data-ttu-id="f7ac9-130">E-mail</span><span class="sxs-lookup"><span data-stu-id="f7ac9-130">Email</span></span>   | <span data-ttu-id="f7ac9-131">Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="f7ac9-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="f7ac9-132">Ogni utente deve avere un indirizzo di posta elettronica univoco</span><span class="sxs-lookup"><span data-stu-id="f7ac9-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="f7ac9-133">Aggiornamento dello stato</span><span class="sxs-lookup"><span data-stu-id="f7ac9-133">Status update</span></span>   | <span data-ttu-id="f7ac9-134">Utilizzato per indicare se il nuovo record utente è stato creato correttamente</span><span class="sxs-lookup"><span data-stu-id="f7ac9-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="f7ac9-135">\*\*Lascia vuoto\*\*</span><span class="sxs-lookup"><span data-stu-id="f7ac9-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="f7ac9-136">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="f7ac9-136">Next steps</span></span>

- [<span data-ttu-id="f7ac9-137">Come aggiungere più utenti per un cliente</span><span class="sxs-lookup"><span data-stu-id="f7ac9-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)