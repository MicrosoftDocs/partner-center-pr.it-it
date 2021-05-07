---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702893"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="247e4-103">Gestire le posizioni dell'account MPN e aggiungere (eliminare) una località</span><span class="sxs-lookup"><span data-stu-id="247e4-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="247e4-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="247e4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="247e4-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="247e4-105">Global admin</span></span>
- <span data-ttu-id="247e4-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="247e4-106">Account admin</span></span>

<span data-ttu-id="247e4-107">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="247e4-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="247e4-108">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="247e4-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="247e4-109">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="247e4-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="247e4-110">Lo scenario seguente è tipico:</span><span class="sxs-lookup"><span data-stu-id="247e4-110">The following scenario is typical:</span></span>

<span data-ttu-id="247e4-111">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="247e4-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="247e4-112">Il PGA è l'azienda legale registrata e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="247e4-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="247e4-113">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="247e4-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="247e4-114">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="247e4-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="247e4-115">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="247e4-116">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="247e4-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="247e4-117">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="247e4-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="247e4-119">Prerequisiti per aggiungere un nuovo account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="247e4-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="247e4-120">Per aggiungere un nuovo account aziendale CSP, iniziare verificando di aver soddisfatto i prerequisiti.</span><span class="sxs-lookup"><span data-stu-id="247e4-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="247e4-121">È necessario avere un ID MPN della posizione nel paese in cui si vuole eseguire l'attività CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="247e4-122">Per creare una nuova posizione MPN, leggere "Aggiungere una posizione MPN" di seguito.</span><span class="sxs-lookup"><span data-stu-id="247e4-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="247e4-123">Per creare una nuova registrazione CSP Indirect Reseller, vedere [Usare i provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="247e4-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="247e4-124">Ricordarsi di accedere con le **nuove** credenziali per il **nuovo** account CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="247e4-125">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="247e4-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="247e4-126">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="247e4-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="247e4-127">Per registrarsi come partner con fatturazione diretta, vedere [Requisiti per i partner con fatturazione diretta](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="247e4-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="247e4-128">Visualizzare e aggiornare le località MPN</span><span class="sxs-lookup"><span data-stu-id="247e4-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="247e4-129">Accedere al dashboard Partner Center [con](https://partner.microsoft.com/dashboard/home) le credenziali dell'account MPN.</span><span class="sxs-lookup"><span data-stu-id="247e4-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="247e4-130">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="247e4-131">**Dall'icona Impostazioni** selezionare **Impostazioni account,** **Profilo organizzazione,** **Note legali.**</span><span class="sxs-lookup"><span data-stu-id="247e4-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="247e4-132">Nella scheda **Partner** verificare che non sia presente un messaggio di errore banner in cui viene chiesto di correggere i percorsi migrati da PMC.</span><span class="sxs-lookup"><span data-stu-id="247e4-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="247e4-133">Se le posizioni non sono state configurate correttamente in PMC e non sono ancora state aggiornate al PC, è necessario aggiornare tali posizioni.</span><span class="sxs-lookup"><span data-stu-id="247e4-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap mostra come aggiornare la posizione.":::
 
4.  <span data-ttu-id="247e4-135">Nella schermata **Review PMC locations (Verifica posizioni PMC)** selezionare Update **(Aggiorna).**</span><span class="sxs-lookup"><span data-stu-id="247e4-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="247e4-136">Aggiornare i campi seguenti:</span><span class="sxs-lookup"><span data-stu-id="247e4-136">Update the following fields:</span></span>

- <span data-ttu-id="247e4-137">**Campo Nome:** assicurarsi che il nome della località aziendale sia corretto.</span><span class="sxs-lookup"><span data-stu-id="247e4-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="247e4-138">Se viene visualizzato un errore duplicato, provare a cambiare, ad esempio, da Contoso a Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="247e4-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="247e4-139">**Campo Persona giuridica:** assicurarsi di aver scelto la persona giuridica a cui è associata la località</span><span class="sxs-lookup"><span data-stu-id="247e4-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="247e4-140">**Riga indirizzo 1 & 2 campi**: assicurarsi che l'indirizzo sia corretto</span><span class="sxs-lookup"><span data-stu-id="247e4-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="247e4-141">**City & State/Province :** assicurarsi che la combinazione tra la città e lo stato/provincia sia corretta.</span><span class="sxs-lookup"><span data-stu-id="247e4-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="247e4-142">In alcuni paesi verrà applicato il menu a discesa per la scelta dello stato/provincia e in altri paesi il campo dovrà essere inserito manualmente.</span><span class="sxs-lookup"><span data-stu-id="247e4-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="247e4-143">**Campo CAP:** assicurarsi che il campo CAP sia corrispondente al paese, all'area geografica, alla città o all'indirizzo indicato.</span><span class="sxs-lookup"><span data-stu-id="247e4-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="247e4-144">**Campi** relativi alle informazioni di contatto primarie: assicurarsi che i campi nome e cognome siano compilati e che l'indirizzo di posta elettronica indicato sia un indirizzo di posta elettronica dell'lavoro e non personale (ad esempio, , e così @outlook.com @live.com via).</span><span class="sxs-lookup"><span data-stu-id="247e4-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="247e4-145">**Campo Numero di telefono:** assicurarsi che il numero di telefono NON includa caratteri speciali, spazi o codice paese.</span><span class="sxs-lookup"><span data-stu-id="247e4-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="247e4-146">Il valore immesso nel campo Numero di telefono conterrà sempre un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="247e4-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="247e4-147">Se non viene visualizzato un messaggio di errore, in  **Impostazioni** selezionare  **Impostazioni account**, **Profilo organizzazione**, **Identificatori**.</span><span class="sxs-lookup"><span data-stu-id="247e4-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="247e4-148">Trovare l'ID MPN con tipo "Location" corrispondente al paese di questo account CSP e usarlo per completare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="247e4-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="247e4-149">Se non è possibile trovare l'ID MPN della posizione corrispondente all'account CSP che si vuole usare, è possibile aggiungere una nuova posizione, che creerà un nuovo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="247e4-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="247e4-150">Vedere **Aggiungere un percorso MPN di** seguito.</span><span class="sxs-lookup"><span data-stu-id="247e4-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="247e4-151">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="247e4-151">Add an MPN location</span></span>

1. <span data-ttu-id="247e4-152">Accedere usando l'account MPN in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="247e4-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="247e4-153">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="247e4-154">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="247e4-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="247e4-155">**Dall'icona Impostazioni** selezionare Impostazioni **account e** quindi Profilo **organizzazione.**</span><span class="sxs-lookup"><span data-stu-id="247e4-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="247e4-156">Selezionare **Legale** e quindi nella **scheda Partner** selezionare Località aziendali e **fare** clic su Aggiungi **una località.**</span><span class="sxs-lookup"><span data-stu-id="247e4-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="247e4-157">Specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si vuole aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="247e4-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="247e4-158">Fare clic **su Aggiungi percorso**.</span><span class="sxs-lookup"><span data-stu-id="247e4-158">Click **Add location**.</span></span> <span data-ttu-id="247e4-159">Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungere una nuova azienda legale":::

> [!NOTE]
> <span data-ttu-id="247e4-161">Dopo aver aggiunto un percorso in Partner Center, non è possibile rimuoverlo.</span><span class="sxs-lookup"><span data-stu-id="247e4-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="247e4-162">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="247e4-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="247e4-163">Aggiungere l'ID del numero di registrazione</span><span class="sxs-lookup"><span data-stu-id="247e4-163">Add the registration number ID</span></span>

<span data-ttu-id="247e4-164">Se si è un provider indiretto, un partner con fatturazione diretta o un rivenditore indiretto e si collabora con clienti nuovi o esistenti nei paesi seguenti, è necessario fornire i numeri ID di registrazione per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="247e4-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="247e4-165">Se il paese in cui si sta effettuando la società non è elencato di seguito, l'ID registrazione è facoltativo.</span><span class="sxs-lookup"><span data-stu-id="247e4-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="247e4-166">Armenia</span><span class="sxs-lookup"><span data-stu-id="247e4-166">Armenia</span></span> 
- <span data-ttu-id="247e4-167">Azerbaigian</span><span class="sxs-lookup"><span data-stu-id="247e4-167">Azerbaijan</span></span> 
- <span data-ttu-id="247e4-168">Bielorussia</span><span class="sxs-lookup"><span data-stu-id="247e4-168">Belarus</span></span> 
- <span data-ttu-id="247e4-169">Brasile</span><span class="sxs-lookup"><span data-stu-id="247e4-169">Brazil</span></span> 
- <span data-ttu-id="247e4-170">Ungheria</span><span class="sxs-lookup"><span data-stu-id="247e4-170">Hungary</span></span> 
- <span data-ttu-id="247e4-171">India</span><span class="sxs-lookup"><span data-stu-id="247e4-171">India</span></span> 
- <span data-ttu-id="247e4-172">Iraq</span><span class="sxs-lookup"><span data-stu-id="247e4-172">Iraq</span></span> 
- <span data-ttu-id="247e4-173">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="247e4-173">Kazakhstan</span></span> 
- <span data-ttu-id="247e4-174">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="247e4-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="247e4-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="247e4-175">Moldova</span></span> 
- <span data-ttu-id="247e4-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="247e4-176">Myanmar</span></span> 
- <span data-ttu-id="247e4-177">Polonia</span><span class="sxs-lookup"><span data-stu-id="247e4-177">Poland</span></span> 
- <span data-ttu-id="247e4-178">Russia</span><span class="sxs-lookup"><span data-stu-id="247e4-178">Russia</span></span> 
- <span data-ttu-id="247e4-179">Arabia Saudita</span><span class="sxs-lookup"><span data-stu-id="247e4-179">Saudi Arabia</span></span> 
- <span data-ttu-id="247e4-180">Sudafrica</span><span class="sxs-lookup"><span data-stu-id="247e4-180">South Africa</span></span> 
- <span data-ttu-id="247e4-181">Sud Sudan</span><span class="sxs-lookup"><span data-stu-id="247e4-181">South Sudan</span></span>  
- <span data-ttu-id="247e4-182">Tagikistan</span><span class="sxs-lookup"><span data-stu-id="247e4-182">Tajikistan</span></span> 
- <span data-ttu-id="247e4-183">Thailandia</span><span class="sxs-lookup"><span data-stu-id="247e4-183">Thailand</span></span>
- <span data-ttu-id="247e4-184">Turchia</span><span class="sxs-lookup"><span data-stu-id="247e4-184">Turkey</span></span> 
- <span data-ttu-id="247e4-185">Ucraina</span><span class="sxs-lookup"><span data-stu-id="247e4-185">Ukraine</span></span> 
- <span data-ttu-id="247e4-186">Emirati Arabi Uniti</span><span class="sxs-lookup"><span data-stu-id="247e4-186">United Arab Emirates</span></span> 
- <span data-ttu-id="247e4-187">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="247e4-187">Uzbekistan</span></span> 
- <span data-ttu-id="247e4-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="247e4-188">Venezuela</span></span>
- <span data-ttu-id="247e4-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="247e4-189">Vietnam</span></span> 


<span data-ttu-id="247e4-190">Per altre informazioni, vedere Informazioni [sul numero ID registrazione](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="247e4-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="247e4-191">Eliminare una località</span><span class="sxs-lookup"><span data-stu-id="247e4-191">Delete a location</span></span>

<span data-ttu-id="247e4-192">Per eliminare una località dall'account, è necessario contattare il [supporto per i partner.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="247e4-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="247e4-193">Assicurarsi di comprendere l'impatto di questa azione.</span><span class="sxs-lookup"><span data-stu-id="247e4-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="247e4-194">Le posizioni eliminate non possono essere recuperate e qualsiasi elemento associato a tale ID MPN specifico non verrà più riconosciuto o sarà attivo per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="247e4-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="247e4-195">Cambiare il paese dell'account globale del partner</span><span class="sxs-lookup"><span data-stu-id="247e4-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="247e4-196">Accedere con l'account MPN Partner Center.</span><span class="sxs-lookup"><span data-stu-id="247e4-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="247e4-197">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP.</span><span class="sxs-lookup"><span data-stu-id="247e4-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="247e4-198">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="247e4-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="247e4-199">Nella scheda **Partner** passare a **Località aziendali** e controllare l'elenco delle località per assicurarsi che sia elencata la località desiderata come persona legale.</span><span class="sxs-lookup"><span data-stu-id="247e4-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="247e4-200">Per aggiungere una località, fare clic su Aggiungi una località e, nel riquadro a comparsa, specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto principale per la località che si vuole aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="247e4-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="247e4-201">Selezionare **Cambia paese accanto** all'elenco a discesa **Paese/area** geografica e seguire la procedura.</span><span class="sxs-lookup"><span data-stu-id="247e4-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Riquadro a comparsa dei dati del profilo di business legale":::

5. <span data-ttu-id="247e4-203">Fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="247e4-203">Click **Save**.</span></span>

6. <span data-ttu-id="247e4-204">Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.</span><span class="sxs-lookup"><span data-stu-id="247e4-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="247e4-205">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="247e4-205">Next steps</span></span>

- <span data-ttu-id="247e4-206">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="247e4-206">Learn about the [verification process](verification-responses.md).</span></span>
