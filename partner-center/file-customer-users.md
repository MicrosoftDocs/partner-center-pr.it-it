---
title: Campi per il file CSV per importare più utenti per un account cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti a un account cliente, creare un file con estensione csv con valori delimitati da virgole con i campi appropriati.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150982"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="c4849-103">Aggiungere più utenti a un account cliente creando un file CSV</span><span class="sxs-lookup"><span data-stu-id="c4849-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="c4849-104">**Ruoli appropriati**: Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c4849-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c4849-105">Aggiungere contemporaneamente più utenti all'account di un cliente caricando un file di dati nel formato di file con valori delimitati da virgole (csv) nel Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c4849-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="c4849-106">È possibile scaricare un file di dati di esempio dal Partner Center e quindi modificarlo per l'uso oppure creare un nuovo file di dati usando il modello di dati definito di seguito.</span><span class="sxs-lookup"><span data-stu-id="c4849-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="c4849-107">Requisiti per i file di dati</span><span class="sxs-lookup"><span data-stu-id="c4849-107">Data file requirements</span></span>

<span data-ttu-id="c4849-108">Per aggiungere più utenti all'account di un cliente usando il processo di caricamento bulk, è necessario soddisfare i requisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="c4849-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="c4849-109">Devi avere le autorizzazioni di amministratore globale per l'account del cliente;</span><span class="sxs-lookup"><span data-stu-id="c4849-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="c4849-110">Ogni utente deve avere un indirizzo e-mail univoco, aggiunto ai domini di e-mail del cliente;</span><span class="sxs-lookup"><span data-stu-id="c4849-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="c4849-111">Puoi caricare fino a 100 record alla volta.</span><span class="sxs-lookup"><span data-stu-id="c4849-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="c4849-112">Se hai bisogno di aggiungere più di 100 utenti, crea e carica ulteriori file di dati.</span><span class="sxs-lookup"><span data-stu-id="c4849-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="c4849-113">Tutti gli utenti devono trovarsi nella stessa **Posizione** geografica.</span><span class="sxs-lookup"><span data-stu-id="c4849-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="c4849-114">Immetti solo i dati descritti di seguito.</span><span class="sxs-lookup"><span data-stu-id="c4849-114">Enter only the data described below.</span></span> <span data-ttu-id="c4849-115">La presenza di dati estranei causerà l'esito negativo del caricamento.</span><span class="sxs-lookup"><span data-stu-id="c4849-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="c4849-116">Immetti i dati seguenti nel file di dati:</span><span class="sxs-lookup"><span data-stu-id="c4849-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="c4849-117">**Nome colonna**</span><span class="sxs-lookup"><span data-stu-id="c4849-117">**Column name**</span></span> | <span data-ttu-id="c4849-118">**Descrizione**</span><span class="sxs-lookup"><span data-stu-id="c4849-118">**Description**</span></span>  | <span data-ttu-id="c4849-119">**Limitazione**</span><span class="sxs-lookup"><span data-stu-id="c4849-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="c4849-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c4849-120">First name</span></span>  | <span data-ttu-id="c4849-121">Nome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="c4849-121">User's first name (optional field)</span></span>  | <span data-ttu-id="c4849-122">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="c4849-122">50-character limit</span></span>  |
| <span data-ttu-id="c4849-123">Cognome</span><span class="sxs-lookup"><span data-stu-id="c4849-123">Last name</span></span>  | <span data-ttu-id="c4849-124">Cognome dell'utente (campo facoltativo)</span><span class="sxs-lookup"><span data-stu-id="c4849-124">User's last name (optional field)</span></span>  | <span data-ttu-id="c4849-125">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="c4849-125">50-character limit</span></span>  |
| <span data-ttu-id="c4849-126">Nome visualizzato</span><span class="sxs-lookup"><span data-stu-id="c4849-126">Display name</span></span>    | <span data-ttu-id="c4849-127">Nome visualizzato nella Partner Center (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="c4849-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="c4849-128">Limite di 50 caratteri</span><span class="sxs-lookup"><span data-stu-id="c4849-128">50-character limit</span></span>                         |
| <span data-ttu-id="c4849-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="c4849-129">Email</span></span>   | <span data-ttu-id="c4849-130">Indirizzo di posta elettronica aziendale dell'utente presso la società del cliente (campo obbligatorio)</span><span class="sxs-lookup"><span data-stu-id="c4849-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="c4849-131">Ogni utente deve avere un indirizzo di posta elettronica univoco</span><span class="sxs-lookup"><span data-stu-id="c4849-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="c4849-132">Aggiornamento dello stato</span><span class="sxs-lookup"><span data-stu-id="c4849-132">Status update</span></span>   | <span data-ttu-id="c4849-133">Usato per indicare se il nuovo record utente è stato creato correttamente</span><span class="sxs-lookup"><span data-stu-id="c4849-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="c4849-134">\*\*Lasciare vuoto\*\*</span><span class="sxs-lookup"><span data-stu-id="c4849-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="c4849-135">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c4849-135">Next steps</span></span>

- [<span data-ttu-id="c4849-136">Come aggiungere più utenti per un cliente</span><span class="sxs-lookup"><span data-stu-id="c4849-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)