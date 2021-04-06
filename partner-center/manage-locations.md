---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441329"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="1c3d5-103">Gestire i percorsi degli account MPN e aggiungere (eliminare) un percorso</span><span class="sxs-lookup"><span data-stu-id="1c3d5-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="1c3d5-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="1c3d5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1c3d5-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="1c3d5-105">Global admin</span></span>
- <span data-ttu-id="1c3d5-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="1c3d5-106">Account admin</span></span>

<span data-ttu-id="1c3d5-107">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="1c3d5-108">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="1c3d5-109">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="1c3d5-110">Lo scenario seguente è tipico:</span><span class="sxs-lookup"><span data-stu-id="1c3d5-110">The following scenario is typical:</span></span>

<span data-ttu-id="1c3d5-111">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="1c3d5-112">Il PGA è il proprio business legale registrato e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="1c3d5-113">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="1c3d5-114">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="1c3d5-115">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="1c3d5-116">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="1c3d5-117">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="1c3d5-119">Prerequisiti per l'aggiunta di un nuovo account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="1c3d5-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="1c3d5-120">Per aggiungere un nuovo account aziendale CSP, iniziare assicurandosi di aver soddisfatto i prerequisiti.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="1c3d5-121">È necessario disporre di un ID MPN della località nel paese in cui si desidera eseguire l'attività di CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="1c3d5-122">Per creare un nuovo percorso MPN, vedere "aggiungere un percorso MPN" di seguito.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="1c3d5-123">Per creare una nuova registrazione del rivenditore indiretto CSP, vedere usare i [provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="1c3d5-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="1c3d5-124">Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** account CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="1c3d5-125">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="1c3d5-126">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="1c3d5-127">Se vuoi iscriverti come partner Direct fattura, leggi [i requisiti per la fatturazione diretta dei partner](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="1c3d5-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="1c3d5-128">Visualizza le località MPN</span><span class="sxs-lookup"><span data-stu-id="1c3d5-128">View your MPN locations</span></span>

1. <span data-ttu-id="1c3d5-129">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home) del centro per i partner con le credenziali dell'account MPN.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="1c3d5-130">(Le credenziali MPN potrebbero essere diverse da quelle del CSP)</span><span class="sxs-lookup"><span data-stu-id="1c3d5-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="1c3d5-131">Nell'icona **Impostazioni** selezionare **Impostazioni account**, **profilo organizzazione**, **legale**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="1c3d5-132">Nella scheda **partner** verificare che non sia presente un messaggio di errore del banner che chiede di correggere i percorsi migrati da PMC.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="1c3d5-133">Se le località non sono state configurate correttamente in PMC e non sono ancora state passate a PC, è necessario aggiornare tali percorsi.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap Mostra come aggiornare il percorso.":::
 
4.  <span data-ttu-id="1c3d5-135">Nella schermata **Verifica percorsi di PMC** selezionare **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="1c3d5-136">Aggiornare i campi seguenti:</span><span class="sxs-lookup"><span data-stu-id="1c3d5-136">Update the following fields:</span></span>

- <span data-ttu-id="1c3d5-137">**Campo nome**: assicurarsi che il nome del percorso aziendale sia corretto.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="1c3d5-138">Se viene visualizzato un errore duplicato, provare a modificare da, ad esempio, contoso a contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="1c3d5-139">**Campo dell'entità legale**: assicurarsi di aver scelto l'entità legale a cui è associata la località</span><span class="sxs-lookup"><span data-stu-id="1c3d5-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="1c3d5-140">**Campi riga indirizzo 1 & 2**: assicurarsi che l'indirizzo sia corretto</span><span class="sxs-lookup"><span data-stu-id="1c3d5-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="1c3d5-141">**Campi provincia & stato/provincia**: assicurarsi che la combinazione tra la città e lo stato o la provincia sia corretta.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="1c3d5-142">In alcuni paesi viene applicato il menu a discesa per la scelta dello stato e della provincia e in altri paesi sarà necessario inserire manualmente tale campo.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="1c3d5-143">**Campo CAP**: assicurarsi che il campo CAP corrisponda al paese, all'area, alla città o all'indirizzo indicato.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="1c3d5-144">**Campi delle informazioni di contatto primarie**: assicurarsi che i campi nome e cognome siano compilati e che l'indirizzo di posta elettronica indicato sia un indirizzo di posta elettronica di lavoro e non uno personale, ad esempio,, e @outlook.com @live.com così via.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="1c3d5-145">**Campo numero di telefono**: assicurarsi che il numero di telefono non includa caratteri speciali, spazi o codici paese.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="1c3d5-146">Il valore immesso nel campo numero di telefono conterrà sempre un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="1c3d5-147">Se non è presente un messaggio di errore, da  **Impostazioni** selezionare  **Impostazioni account**, **profilo organizzazione**, **identificatori**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="1c3d5-148">Trovare l'ID MPN con il tipo "location" corrispondente al paese di questo account CSP e usarlo per completare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="1c3d5-149">Se non è possibile trovare l'ID MPN della località che corrisponde all'account CSP da usare, è possibile aggiungere un nuovo percorso che creerà un nuovo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="1c3d5-150">Vedere **aggiungere un percorso MPN di** seguito.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="1c3d5-151">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="1c3d5-151">Add an MPN location</span></span>

1. <span data-ttu-id="1c3d5-152">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="1c3d5-153">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="1c3d5-154">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="1c3d5-155">Nell' **icona Impostazioni** selezionare le impostazioni dell' **account** e quindi selezionare **profilo organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="1c3d5-156">Selezionare **Legal** , quindi nella scheda **partner** Selezionare **percorsi aziendali** e fare clic su **Aggiungi un percorso.**</span><span class="sxs-lookup"><span data-stu-id="1c3d5-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="1c3d5-157">Specificare i dettagli richiesti, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="1c3d5-158">Fare clic su **Aggiungi percorso**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-158">Click **Add location**.</span></span> <span data-ttu-id="1c3d5-159">Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungi una nuova attività legale":::

> [!NOTE]
> <span data-ttu-id="1c3d5-161">Una volta aggiunta una località nel centro per i partner, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="1c3d5-162">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="1c3d5-163">Elimina un percorso</span><span class="sxs-lookup"><span data-stu-id="1c3d5-163">Delete a location</span></span>

<span data-ttu-id="1c3d5-164">Per eliminare un percorso dall'account, sarà necessario contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="1c3d5-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="1c3d5-165">Assicurarsi di comprendere l'effetto di questa azione.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="1c3d5-166">Non è possibile recuperare i percorsi eliminati e qualsiasi elemento associato a tale ID MPN specifico non verrà più riconosciuto o attivo per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="1c3d5-167">Modificare il paese dell'account globale del partner</span><span class="sxs-lookup"><span data-stu-id="1c3d5-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="1c3d5-168">Accedere con l'account MPN nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="1c3d5-169">Le credenziali MPN potrebbero essere diverse da quelle del CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="1c3d5-170">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="1c3d5-171">Nella scheda **partner** passare a **percorsi aziendali** e controllare l'elenco delle località per assicurarsi che la località desiderata come entità legale sia elencata.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="1c3d5-172">Per aggiungere un percorso, fare clic su **Aggiungi un percorso** e, in uscita, fornire i dettagli necessari, tra cui il nome dell'azienda, l'indirizzo e il contatto principale per la località che si desidera aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="1c3d5-173">Selezionare **cambia il paese** accanto all'elenco a discesa **paese/area geografica** e seguire i passaggi.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Informazioni legali sui dati del profilo aziendale":::

5. <span data-ttu-id="1c3d5-175">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-175">Click **Save**.</span></span>

6. <span data-ttu-id="1c3d5-176">Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.</span><span class="sxs-lookup"><span data-stu-id="1c3d5-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="1c3d5-177">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="1c3d5-177">Next steps</span></span>

- <span data-ttu-id="1c3d5-178">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="1c3d5-178">Learn about the [verification process](verification-responses.md).</span></span>
