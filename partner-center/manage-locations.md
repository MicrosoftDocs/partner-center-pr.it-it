---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005914"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="9b78d-103">Gestire i percorsi degli account MPN e aggiungere (eliminare) un percorso</span><span class="sxs-lookup"><span data-stu-id="9b78d-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="9b78d-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="9b78d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9b78d-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="9b78d-105">Global admin</span></span>
- <span data-ttu-id="9b78d-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="9b78d-106">Account admin</span></span>

<span data-ttu-id="9b78d-107">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="9b78d-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="9b78d-108">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="9b78d-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="9b78d-109">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="9b78d-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="9b78d-110">Di seguito è riportato uno scenario tipico:</span><span class="sxs-lookup"><span data-stu-id="9b78d-110">The following is a typical scenario:</span></span>

<span data-ttu-id="9b78d-111">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="9b78d-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="9b78d-112">Si tratta della sede legale dell'azienda e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="9b78d-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="9b78d-113">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="9b78d-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="9b78d-114">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="9b78d-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="9b78d-115">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="9b78d-116">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="9b78d-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="9b78d-117">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="9b78d-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="9b78d-119">Prerequisiti per l'aggiunta di un nuovo account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="9b78d-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="9b78d-120">Per aggiungere un nuovo account aziendale CSP, iniziare assicurandosi di aver soddisfatto i prerequisiti.</span><span class="sxs-lookup"><span data-stu-id="9b78d-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="9b78d-121">È necessario disporre di un ID MPN della località nel paese in cui si desidera eseguire l'attività di CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="9b78d-122">Per creare un nuovo percorso MPN, vedere "aggiungere un percorso MPN" di seguito.</span><span class="sxs-lookup"><span data-stu-id="9b78d-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="9b78d-123">Per creare una nuova registrazione del rivenditore indiretto CSP, vedere usare i [provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="9b78d-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="9b78d-124">Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** account CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="9b78d-125">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="9b78d-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="9b78d-126">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="9b78d-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="9b78d-127">Se vuoi iscriverti come partner Direct fattura, leggi [i requisiti per la fatturazione diretta dei partner](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="9b78d-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="9b78d-128">Visualizza le località MPN</span><span class="sxs-lookup"><span data-stu-id="9b78d-128">View your MPN locations</span></span>

1. <span data-ttu-id="9b78d-129">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home) del centro per i partner con le credenziali dell'account MPN.</span><span class="sxs-lookup"><span data-stu-id="9b78d-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="9b78d-130">(Le credenziali MPN potrebbero essere diverse da quelle del CSP)</span><span class="sxs-lookup"><span data-stu-id="9b78d-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="9b78d-131">Nell'icona **Impostazioni** selezionare **Impostazioni account**, **profilo organizzazione**, **legale**.</span><span class="sxs-lookup"><span data-stu-id="9b78d-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="9b78d-132">Nella scheda **partner** verificare che non sia presente un messaggio di errore banner che chiede di correggere i percorsi migrati da PMC.</span><span class="sxs-lookup"><span data-stu-id="9b78d-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="9b78d-133">Se è presente, seguire le istruzioni e correggere tali percorsi.</span><span class="sxs-lookup"><span data-stu-id="9b78d-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="9b78d-134">Se non è presente un messaggio di errore, da  **Impostazioni** selezionare  **Impostazioni account**, **profilo organizzazione**, **identificatori**.</span><span class="sxs-lookup"><span data-stu-id="9b78d-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="9b78d-135">Trovare l'ID MPN con il tipo "location" corrispondente al paese di questo account CSP e usarlo per eseguire la ricerca sotto e completare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="9b78d-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="9b78d-136">Se non è possibile trovare l'ID MPN della località che corrisponde all'account CSP da usare, è possibile aggiungere un nuovo percorso che creerà un nuovo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="9b78d-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="9b78d-137">Vedere **aggiungere un percorso MPN di** seguito.</span><span class="sxs-lookup"><span data-stu-id="9b78d-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="9b78d-138">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="9b78d-138">Add an MPN location</span></span>

1. <span data-ttu-id="9b78d-139">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9b78d-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="9b78d-140">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="9b78d-141">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="9b78d-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="9b78d-142">Nell' **icona Impostazioni** selezionare le impostazioni dell' **account** e quindi selezionare **profilo organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="9b78d-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="9b78d-143">Selezionare **Legal** , quindi nella scheda **partner** Selezionare **percorsi aziendali** e fare clic su **Aggiungi un percorso.**</span><span class="sxs-lookup"><span data-stu-id="9b78d-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="9b78d-144">Specificare i dettagli richiesti, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="9b78d-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="9b78d-145">Fare clic su **Aggiungi percorso**.</span><span class="sxs-lookup"><span data-stu-id="9b78d-145">Click **Add location**.</span></span> <span data-ttu-id="9b78d-146">Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungi una nuova attività legale":::

> [!NOTE]
> <span data-ttu-id="9b78d-148">Una volta aggiunta una località nel centro per i partner, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="9b78d-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="9b78d-149">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9b78d-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="9b78d-150">Elimina un percorso</span><span class="sxs-lookup"><span data-stu-id="9b78d-150">Delete a location</span></span>

<span data-ttu-id="9b78d-151">Per eliminare una località dall'account, è necessario contattare il [supporto tecnico del partner](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="9b78d-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="9b78d-152">Assicurarsi di comprendere l'effetto di questa azione.</span><span class="sxs-lookup"><span data-stu-id="9b78d-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="9b78d-153">Non è possibile recuperare i percorsi eliminati e qualsiasi elemento associato a tale ID MPN specifico non verrà più riconosciuto o attivo per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="9b78d-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="9b78d-154">Modificare il paese dell'account globale del partner</span><span class="sxs-lookup"><span data-stu-id="9b78d-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="9b78d-155">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="9b78d-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="9b78d-156">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="9b78d-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="9b78d-157">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="9b78d-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="9b78d-158">Nella scheda **partner** passare a **percorsi aziendali** e controllare l'elenco delle località per assicurarsi che la località desiderata come entità legale sia elencata.</span><span class="sxs-lookup"><span data-stu-id="9b78d-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="9b78d-159">Per aggiungere un percorso, fare clic su **Aggiungi un percorso** e, in uscita, fornire i dettagli necessari, tra cui il nome dell'azienda, l'indirizzo e il contatto principale per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="9b78d-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="9b78d-160">Selezionare **cambia il paese** accanto all'elenco a discesa **paese/area geografica** e seguire i passaggi.</span><span class="sxs-lookup"><span data-stu-id="9b78d-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Informazioni legali sui dati del profilo aziendale":::

5. <span data-ttu-id="9b78d-162">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="9b78d-162">Click **Save**.</span></span>

6. <span data-ttu-id="9b78d-163">Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.</span><span class="sxs-lookup"><span data-stu-id="9b78d-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="9b78d-164">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="9b78d-164">Next steps</span></span>

- <span data-ttu-id="9b78d-165">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="9b78d-165">Learn about the [verification process](verification-responses.md).</span></span>
