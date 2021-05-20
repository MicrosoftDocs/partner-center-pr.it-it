---
title: Aggiungere più utenti per un account cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per aggiungere più utenti all'account di un cliente, caricare un file di dati Partner Center usando il formato di file con valori delimitati da virgole (csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150472"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="095bb-103">Caricare un file CSV di utenti nell'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="095bb-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="095bb-104">**Ruoli appropriati:** Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="095bb-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="095bb-105">Aggiungere contemporaneamente più utenti all'account di un cliente caricando un file di dati nel formato di file con valori delimitati da virgole (csv) nel Partner Center.</span><span class="sxs-lookup"><span data-stu-id="095bb-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="095bb-106">Creare il file degli utenti dei clienti e caricarlo nell'account del cliente</span><span class="sxs-lookup"><span data-stu-id="095bb-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="095bb-107">Crea un file di dati con valori delimitati da virgole (CSV) con i dati descritti sopra.</span><span class="sxs-lookup"><span data-stu-id="095bb-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="095bb-108">Salva il file in modo da poterlo visualizzare in un passaggio successivo.</span><span class="sxs-lookup"><span data-stu-id="095bb-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="095bb-109">Vedere [Campi per il file CSV per importare più utenti per un account cliente.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="095bb-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="095bb-110">Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="095bb-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="095bb-111">Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="095bb-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="095bb-112">Selezionare la scheda Utenti e licenze **del** cliente e quindi **selezionare Carica utenti**.</span><span class="sxs-lookup"><span data-stu-id="095bb-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="095bb-113">In **Carica informazioni utenti** seleziona **Sfoglia**.</span><span class="sxs-lookup"><span data-stu-id="095bb-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="095bb-114">Nel selettore di file seleziona il file di dati e quindi seleziona **Apri**.</span><span class="sxs-lookup"><span data-stu-id="095bb-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="095bb-115">Selezionare **Convalida**.</span><span class="sxs-lookup"><span data-stu-id="095bb-115">Select **Validate**.</span></span>

    <span data-ttu-id="095bb-116">**Nota**  La maggior parte degli errori di creazione dell'account è causata da problemi del file di dati, tra cui informazioni mancanti, indirizzi di posta elettronica in formato non valido o duplicati o troppi record nel file.</span><span class="sxs-lookup"><span data-stu-id="095bb-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="095bb-117">Dopo aver Partner Center convalidare il file, selezionare la località **geografica** per i nuovi utenti.</span><span class="sxs-lookup"><span data-stu-id="095bb-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="095bb-118">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="095bb-118">Select **Save**.</span></span>
10. <span data-ttu-id="095bb-119">Scaricare le informazioni sulla password temporanea per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="095bb-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="095bb-120">Assicurarsi di scaricare il file con le password temporanee ora perché non sarà possibile eseguire questa operazione in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="095bb-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="095bb-121">I nuovi utenti devono accedere all'account nuovo usando la password temporanea per i nuovi account.</span><span class="sxs-lookup"><span data-stu-id="095bb-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="095bb-122">Ai nuovi utenti vengono assegnate automaticamente le autorizzazioni **di Può usare licenze e servizi**.</span><span class="sxs-lookup"><span data-stu-id="095bb-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="095bb-123">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="095bb-123">Next steps</span></span>

- [<span data-ttu-id="095bb-124">Concedere ai clienti l'autorizzazione Partner Center acquistare i propri prodotti o servizi</span><span class="sxs-lookup"><span data-stu-id="095bb-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
