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
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276825"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="d39fb-103">Gestire le posizioni dell'account MPN e aggiungere (eliminare) una località</span><span class="sxs-lookup"><span data-stu-id="d39fb-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="d39fb-104">**Ruoli appropriati:** Amministratore globale | Amministratore dell'account</span><span class="sxs-lookup"><span data-stu-id="d39fb-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="d39fb-105">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="d39fb-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="d39fb-106">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="d39fb-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="d39fb-107">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="d39fb-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="d39fb-108">Lo scenario seguente è tipico:</span><span class="sxs-lookup"><span data-stu-id="d39fb-108">The following scenario is typical:</span></span>

<span data-ttu-id="d39fb-109">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="d39fb-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="d39fb-110">Il PGA è l'azienda legale registrata e il relativo ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="d39fb-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="d39fb-111">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="d39fb-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="d39fb-112">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="d39fb-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="d39fb-113">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="d39fb-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="d39fb-114">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="d39fb-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="d39fb-115">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="d39fb-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle posizioni MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="d39fb-117">Prerequisiti per aggiungere un nuovo account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="d39fb-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="d39fb-118">Per aggiungere un nuovo account aziendale CSP, assicurarsi di aver soddisfatto i prerequisiti.</span><span class="sxs-lookup"><span data-stu-id="d39fb-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="d39fb-119">È necessario avere un ID MPN della località nel paese in cui si vuole eseguire l'attività CSP.</span><span class="sxs-lookup"><span data-stu-id="d39fb-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="d39fb-120">Per creare una nuova posizione MPN, vedere "Aggiungere una posizione MPN" di seguito.</span><span class="sxs-lookup"><span data-stu-id="d39fb-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="d39fb-121">Per creare una nuova CSP Indirect Reseller, vedere [Usare i provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="d39fb-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="d39fb-122">Ricordarsi di accedere con le **nuove** credenziali per il **nuovo** account CSP.</span><span class="sxs-lookup"><span data-stu-id="d39fb-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="d39fb-123">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="d39fb-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="d39fb-124">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="d39fb-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="d39fb-125">Se si vuole eseguire la registrazione come partner direct bill, leggere [Requisiti per i partner direct bill](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="d39fb-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="d39fb-126">Visualizzare e aggiornare le posizioni MPN</span><span class="sxs-lookup"><span data-stu-id="d39fb-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="d39fb-127">Accedere al dashboard Partner Center [con](https://partner.microsoft.com/dashboard/home) le credenziali dell'account MPN.</span><span class="sxs-lookup"><span data-stu-id="d39fb-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="d39fb-128">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP.</span><span class="sxs-lookup"><span data-stu-id="d39fb-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="d39fb-129">**Dall'icona Impostazioni** selezionare **Impostazioni account**, **Profilo organizzazione**, **Legale**.</span><span class="sxs-lookup"><span data-stu-id="d39fb-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="d39fb-130">Nella scheda **Partner** verificare che non sia presente un messaggio di errore banner in cui viene chiesto di correggere i percorsi migrati da PMC.</span><span class="sxs-lookup"><span data-stu-id="d39fb-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="d39fb-131">Se le località non sono state configurate correttamente in PMC e non sono ancora state transizione al PC, è necessario aggiornare tali posizioni.</span><span class="sxs-lookup"><span data-stu-id="d39fb-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap mostra come aggiornare la posizione.":::
 
4.  <span data-ttu-id="d39fb-133">Nella schermata **Rivedi posizioni PMC** selezionare **Aggiorna**.</span><span class="sxs-lookup"><span data-stu-id="d39fb-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="d39fb-134">Aggiornare i campi seguenti:</span><span class="sxs-lookup"><span data-stu-id="d39fb-134">Update the following fields:</span></span>

- <span data-ttu-id="d39fb-135">**Campo Nome:** assicurarsi che il nome della sede aziendale sia corretto.</span><span class="sxs-lookup"><span data-stu-id="d39fb-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="d39fb-136">Se viene visualizzato un errore duplicato, provare a cambiare, ad esempio, da Contoso a Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="d39fb-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="d39fb-137">**Campo Persona giuridica:** assicurarsi di aver scelto la persona giuridica a cui è associata la località</span><span class="sxs-lookup"><span data-stu-id="d39fb-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="d39fb-138">**Riga dell'indirizzo 1 & 2 campi**: assicurarsi che l'indirizzo sia corretto</span><span class="sxs-lookup"><span data-stu-id="d39fb-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="d39fb-139">**City & State/Province :** assicurarsi che la combinazione tra la città e lo stato/provincia sia corretta.</span><span class="sxs-lookup"><span data-stu-id="d39fb-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="d39fb-140">In alcuni paesi verrà applicato il menu a discesa per la scelta dello stato/provincia e in altri paesi il campo dovrà essere inserito manualmente.</span><span class="sxs-lookup"><span data-stu-id="d39fb-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="d39fb-141">**Campo CAP:** assicurarsi che il campo CAP sia corrispondente al paese, all'area geografica, alla città o all'indirizzo indicato.</span><span class="sxs-lookup"><span data-stu-id="d39fb-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="d39fb-142">**Campi** relativi alle informazioni di contatto primarie: assicurarsi che i campi nome e cognome siano compilati e che l'indirizzo di posta elettronica indicato sia un indirizzo di posta elettronica dell'lavoro e non personale (ad esempio, , e così @outlook.com @live.com via).</span><span class="sxs-lookup"><span data-stu-id="d39fb-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="d39fb-143">**Campo Numero di telefono:** assicurarsi che il numero di telefono NON includa caratteri speciali, spazi o codice paese.</span><span class="sxs-lookup"><span data-stu-id="d39fb-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="d39fb-144">Il valore immesso nel campo Numero di telefono conterrà sempre un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="d39fb-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="d39fb-145">Se non viene visualizzato un messaggio di errore, in  **Impostazioni** selezionare  **Impostazioni account**, **Profilo organizzazione**, **Identificatori**.</span><span class="sxs-lookup"><span data-stu-id="d39fb-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="d39fb-146">Trovare l'ID MPN con tipo "Location" corrispondente al paese di questo account CSP e usarlo per completare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="d39fb-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="d39fb-147">Se non è possibile trovare l'ID MPN della posizione corrispondente all'account CSP che si vuole usare, è possibile aggiungere una nuova posizione, che creerà un nuovo ID MPN.</span><span class="sxs-lookup"><span data-stu-id="d39fb-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="d39fb-148">Vedere **Aggiungere un percorso MPN di** seguito.</span><span class="sxs-lookup"><span data-stu-id="d39fb-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="d39fb-149">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="d39fb-149">Add an MPN location</span></span>

1. <span data-ttu-id="d39fb-150">Accedere usando l'account MPN in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d39fb-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="d39fb-151">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP. L'account MPN deve avere privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="d39fb-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="d39fb-152">**Dall'icona Impostazioni** selezionare Impostazioni **account e** quindi Profilo **organizzazione.**</span><span class="sxs-lookup"><span data-stu-id="d39fb-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="d39fb-153">Selezionare **Legale** e quindi nella **scheda Partner** selezionare Località aziendali **e** quindi Aggiungi **una località.**</span><span class="sxs-lookup"><span data-stu-id="d39fb-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="d39fb-154">Specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto, per la località che si vuole aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="d39fb-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="d39fb-155">Selezionare **Aggiungi percorso**.</span><span class="sxs-lookup"><span data-stu-id="d39fb-155">Select **Add location**.</span></span> <span data-ttu-id="d39fb-156">Verrà creato un nuovo ID MPN per la nuova posizione che è possibile usare per le transazioni e gli incentivi CSP.</span><span class="sxs-lookup"><span data-stu-id="d39fb-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungere una nuova attività legale.":::

> [!NOTE]
> <span data-ttu-id="d39fb-158">Dopo aver aggiunto una posizione in Partner Center, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="d39fb-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="d39fb-159">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d39fb-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="d39fb-160">Aggiungere l'ID del numero di registrazione</span><span class="sxs-lookup"><span data-stu-id="d39fb-160">Add the registration number ID</span></span>

<span data-ttu-id="d39fb-161">Se si è un provider indiretto, un partner di fatturazione diretta o un rivenditore indiretto e si stanno facendo affari con clienti nuovi o esistenti nei paesi seguenti, è necessario fornire i numeri ID di registrazione per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="d39fb-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="d39fb-162">Se il paese in cui si stanno facendo affari non è elencato di seguito, l'ID registrazione è facoltativo.</span><span class="sxs-lookup"><span data-stu-id="d39fb-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="d39fb-163">Armenia</span><span class="sxs-lookup"><span data-stu-id="d39fb-163">Armenia</span></span> 
- <span data-ttu-id="d39fb-164">Azerbaigian</span><span class="sxs-lookup"><span data-stu-id="d39fb-164">Azerbaijan</span></span> 
- <span data-ttu-id="d39fb-165">Bielorussia</span><span class="sxs-lookup"><span data-stu-id="d39fb-165">Belarus</span></span> 
- <span data-ttu-id="d39fb-166">Brasile</span><span class="sxs-lookup"><span data-stu-id="d39fb-166">Brazil</span></span> 
- <span data-ttu-id="d39fb-167">Ungheria</span><span class="sxs-lookup"><span data-stu-id="d39fb-167">Hungary</span></span> 
- <span data-ttu-id="d39fb-168">India</span><span class="sxs-lookup"><span data-stu-id="d39fb-168">India</span></span> 
- <span data-ttu-id="d39fb-169">Iraq</span><span class="sxs-lookup"><span data-stu-id="d39fb-169">Iraq</span></span> 
- <span data-ttu-id="d39fb-170">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="d39fb-170">Kazakhstan</span></span> 
- <span data-ttu-id="d39fb-171">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="d39fb-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="d39fb-172">Moldova</span><span class="sxs-lookup"><span data-stu-id="d39fb-172">Moldova</span></span> 
- <span data-ttu-id="d39fb-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="d39fb-173">Myanmar</span></span> 
- <span data-ttu-id="d39fb-174">Polonia</span><span class="sxs-lookup"><span data-stu-id="d39fb-174">Poland</span></span> 
- <span data-ttu-id="d39fb-175">Russia</span><span class="sxs-lookup"><span data-stu-id="d39fb-175">Russia</span></span> 
- <span data-ttu-id="d39fb-176">Arabia Saudita</span><span class="sxs-lookup"><span data-stu-id="d39fb-176">Saudi Arabia</span></span> 
- <span data-ttu-id="d39fb-177">Sudafrica</span><span class="sxs-lookup"><span data-stu-id="d39fb-177">South Africa</span></span> 
- <span data-ttu-id="d39fb-178">Sud Sudan</span><span class="sxs-lookup"><span data-stu-id="d39fb-178">South Sudan</span></span>  
- <span data-ttu-id="d39fb-179">Tagikistan</span><span class="sxs-lookup"><span data-stu-id="d39fb-179">Tajikistan</span></span> 
- <span data-ttu-id="d39fb-180">Thailandia</span><span class="sxs-lookup"><span data-stu-id="d39fb-180">Thailand</span></span>
- <span data-ttu-id="d39fb-181">Turchia</span><span class="sxs-lookup"><span data-stu-id="d39fb-181">Turkey</span></span> 
- <span data-ttu-id="d39fb-182">Ucraina</span><span class="sxs-lookup"><span data-stu-id="d39fb-182">Ukraine</span></span> 
- <span data-ttu-id="d39fb-183">Emirati Arabi Uniti</span><span class="sxs-lookup"><span data-stu-id="d39fb-183">United Arab Emirates</span></span> 
- <span data-ttu-id="d39fb-184">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="d39fb-184">Uzbekistan</span></span> 
- <span data-ttu-id="d39fb-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="d39fb-185">Venezuela</span></span>
- <span data-ttu-id="d39fb-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="d39fb-186">Vietnam</span></span> 


<span data-ttu-id="d39fb-187">Per altre informazioni, vedere Informazioni [sul numero ID registrazione](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="d39fb-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="d39fb-188">Eliminare una località</span><span class="sxs-lookup"><span data-stu-id="d39fb-188">Delete a location</span></span>

<span data-ttu-id="d39fb-189">Per eliminare una località dall'account, è necessario contattare il [supporto tecnico per i partner.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="d39fb-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="d39fb-190">Assicurarsi di comprendere l'impatto di questa azione.</span><span class="sxs-lookup"><span data-stu-id="d39fb-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="d39fb-191">Le posizioni eliminate non possono essere recuperate e tutto ciò che è associato a tale ID MPN specifico non verrà più riconosciuto o sarà attivo per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="d39fb-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="d39fb-192">Cambiare il paese dell'account globale del partner</span><span class="sxs-lookup"><span data-stu-id="d39fb-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="d39fb-193">Accedere usando l'account MPN in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d39fb-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="d39fb-194">Le credenziali MPN potrebbero essere diverse dalle credenziali CSP. L'account MPN deve avere privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="d39fb-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="d39fb-195">Nella scheda **Partner** passare a **Località** aziendali e controllare l'elenco delle località per assicurarsi che sia elencata la località desiderata come persona giuridica.</span><span class="sxs-lookup"><span data-stu-id="d39fb-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="d39fb-196">Per aggiungere una località, fare clic su Aggiungi una località e, nel riquadro a comparsa, specificare i dettagli necessari, inclusi il nome dell'azienda, l'indirizzo e il contatto primario per la località che si vuole aggiungere all'azienda.</span><span class="sxs-lookup"><span data-stu-id="d39fb-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="d39fb-197">Selezionare **Cambia paese accanto** all'elenco a discesa **Paese/area** geografica e seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="d39fb-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="I dati del profilo aziendale legale sono in uscita.":::

5. <span data-ttu-id="d39fb-199">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="d39fb-199">Select **Save**.</span></span>

6. <span data-ttu-id="d39fb-200">Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.</span><span class="sxs-lookup"><span data-stu-id="d39fb-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="d39fb-201">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d39fb-201">Next steps</span></span>

- <span data-ttu-id="d39fb-202">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="d39fb-202">Learn about the [verification process](verification-responses.md).</span></span>
