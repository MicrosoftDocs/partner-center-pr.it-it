---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925017"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="2c7f9-103">Gestire le sedi dell'account MPN e aggiungere una nuova sede</span><span class="sxs-lookup"><span data-stu-id="2c7f9-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="2c7f9-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="2c7f9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2c7f9-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="2c7f9-105">Global admin</span></span>
- <span data-ttu-id="2c7f9-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="2c7f9-106">Account admin</span></span>

<span data-ttu-id="2c7f9-107">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="2c7f9-108">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="2c7f9-109">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="2c7f9-110">Di seguito è riportato uno scenario tipico:</span><span class="sxs-lookup"><span data-stu-id="2c7f9-110">The following is a typical scenario:</span></span>

<span data-ttu-id="2c7f9-111">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="2c7f9-112">Si tratta della sede legale dell'azienda e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="2c7f9-113">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="2c7f9-114">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="2c7f9-115">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="2c7f9-116">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="2c7f9-117">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="2c7f9-119">Prerequisiti per l'aggiunta di un nuovo account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="2c7f9-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="2c7f9-120">Per aggiungere un nuovo account aziendale CSP, iniziare assicurandosi di aver soddisfatto i prerequisiti.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="2c7f9-121">È necessario disporre di un ID MPN della località nel paese in cui si desidera eseguire l'attività di CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="2c7f9-122">Per creare un nuovo percorso MPN, vedere "aggiungere un percorso MPN" di seguito.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="2c7f9-123">Per creare una nuova registrazione del rivenditore indiretto CSP, vedere usare i [provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="2c7f9-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="2c7f9-124">Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** account CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="2c7f9-125">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="2c7f9-126">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="2c7f9-127">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="2c7f9-127">Add an MPN location</span></span>

1. <span data-ttu-id="2c7f9-128">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="2c7f9-129">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="2c7f9-130">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="2c7f9-131">Nell' **icona Impostazioni** selezionare le impostazioni dell' **account** e quindi selezionare **profilo organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="2c7f9-132">Selezionare **Legal** , quindi nella scheda **partner** Selezionare **percorsi aziendali** e fare clic su **Aggiungi un percorso.**</span><span class="sxs-lookup"><span data-stu-id="2c7f9-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="2c7f9-133">Specificare i dettagli richiesti, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="2c7f9-134">Fare clic su **Aggiungi percorso**.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-134">Click **Add location**.</span></span> <span data-ttu-id="2c7f9-135">Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungi una nuova attività legale":::

> [!NOTE]
> <span data-ttu-id="2c7f9-137">dopo aver aggiunto una posizione nel Centro per i partner, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="2c7f9-138">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="2c7f9-139">Modificare il paese dell'account globale del partner</span><span class="sxs-lookup"><span data-stu-id="2c7f9-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="2c7f9-140">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="2c7f9-141">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="2c7f9-142">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="2c7f9-143">Nella scheda **partner** passare a **percorsi aziendali** e controllare l'elenco delle località per assicurarsi che la località desiderata come entità legale sia elencata.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="2c7f9-144">Per aggiungere un percorso, fare clic su **Aggiungi un percorso** e, in uscita, fornire i dettagli necessari, tra cui il nome dell'azienda, l'indirizzo e il contatto principale per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="2c7f9-145">Selezionare **cambia il paese** accanto all'elenco a discesa **paese/area geografica** e seguire i passaggi.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Informazioni legali sui dati del profilo aziendale":::

5. <span data-ttu-id="2c7f9-147">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-147">Click **Save**.</span></span>

6. <span data-ttu-id="2c7f9-148">Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.</span><span class="sxs-lookup"><span data-stu-id="2c7f9-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="2c7f9-149">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="2c7f9-149">Next steps</span></span>

- <span data-ttu-id="2c7f9-150">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="2c7f9-150">Learn about the [verification process](verification-responses.md).</span></span>
