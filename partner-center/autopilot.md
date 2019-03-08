---
title: Personalizzare l'esperienza out-of-box del dispositivo con i profili di Autopilot di Windows | Centro per i partner
description: Preconfigurare esperienza out-of-box del dispositivo con i profili di Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot di windows, autopilot microsoft, distribuzione zero touch, la configurazione guidata, le schermate di accesso, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586914"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="9042a-104">Personalizzare l'esperienza out-of-box del dispositivo con i profili Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="9042a-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="9042a-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="9042a-105">**Applies to**</span></span>

- <span data-ttu-id="9042a-106">I partner CSP diretti fattura e i provider indiretti i rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="9042a-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="9042a-107">Se si gestiscono i dispositivi dei clienti, si potrebbe essere necessario personalizzare l'esperienza di out-of-box (OOBE) per gli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="9042a-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="9042a-108">È possibile preconfigurare nuovi dispositivi con profili di Autopilot di Windows prima di recapitare i dispositivi per i clienti e si applicano nuovi profili nei dispositivi, i clienti hanno già acquistato.</span><span class="sxs-lookup"><span data-stu-id="9042a-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="9042a-109">Questo articolo illustra come creare e applicare i profili di Autopilot per i dispositivi nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="9042a-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="9042a-110">Se non si ha già familiarità con Autopilot, consultare le informazioni contenute in questi articoli:</span><span class="sxs-lookup"><span data-stu-id="9042a-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="9042a-111">Panoramica di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="9042a-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="9042a-112">Guida di riferimento di distribuzione AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9042a-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="9042a-113">Panoramica</span><span class="sxs-lookup"><span data-stu-id="9042a-113">Overview</span></span>

<span data-ttu-id="9042a-114">Con la funzionalità di Windows Autopilot nel centro per i Partner, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti.</span><span class="sxs-lookup"><span data-stu-id="9042a-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="9042a-115">Le impostazioni del profilo sono state disponibili al momento che della pubblicazione dell'articolo:</span><span class="sxs-lookup"><span data-stu-id="9042a-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="9042a-116">Ignorare le impostazioni di privacy.</span><span class="sxs-lookup"><span data-stu-id="9042a-116">Skip privacy settings.</span></span> <span data-ttu-id="9042a-117">Questa impostazione del profilo di Autopilot facoltativa consente alle organizzazioni di non porre sulle impostazioni di privacy durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="9042a-118">Disabilitare la creazione dell'account amministratore locale nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9042a-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="9042a-119">Le organizzazioni possono decidere se l'utente di configurazione del dispositivo deve avere accesso come amministratore, una volta completato il processo.</span><span class="sxs-lookup"><span data-stu-id="9042a-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="9042a-120">Configurare automaticamente i dispositivi per lavoro o dell'istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="9042a-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="9042a-121">Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati lavoro o dell'istituto di istruzione, i dispositivi in modo che durante il processo di configurazione guidata non verrà chiesto di questa domanda.</span><span class="sxs-lookup"><span data-stu-id="9042a-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="9042a-122">Ignorare Cortana, OneDrive e OEM pagine di configurazione di registrazione.</span><span class="sxs-lookup"><span data-stu-id="9042a-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="9042a-123">Tutti i dispositivi registrati con Autopilot ignorerà automaticamente queste pagine durante il processo di out-of-box configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="9042a-124">Ignorare il contratto di licenza utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="9042a-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="9042a-125">A partire da Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina Contratto di licenza presentata durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="9042a-126">Visualizzare [licenziamento condizioni di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da considerare su come ignorare la pagina Contratto di licenza Windows durante l'installazione.</span><span class="sxs-lookup"><span data-stu-id="9042a-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="9042a-127">Si applicano le autorizzazioni di gestione profilo e dispositivo e le limitazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="9042a-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="9042a-128">I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti con cui hanno relazioni reseller, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.</span><span class="sxs-lookup"><span data-stu-id="9042a-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="9042a-129">È possibile gestire i dispositivi esistenti per i clienti che sono state aggiunte dall'utente o da un altro partner CSP.</span><span class="sxs-lookup"><span data-stu-id="9042a-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="9042a-130">Non è possibile gestire i dispositivi che del cliente è caricata in Microsoft Store per le aziende o il portale di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9042a-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="9042a-131">Creare e gestire i profili di Autopilot nel centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="9042a-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="9042a-132">Nel centro per i Partner, è possibile creare profili di distribuzione Windows Autopilot e applicarle ai dispositivi.</span><span class="sxs-lookup"><span data-stu-id="9042a-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="9042a-133">Solo gli agenti di amministrazione è possono creare e applicare i profili.</span><span class="sxs-lookup"><span data-stu-id="9042a-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="9042a-134">Creare un nuovo profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="9042a-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="9042a-135">Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente crei il profilo di Autopilot per.</span><span class="sxs-lookup"><span data-stu-id="9042a-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="9042a-136">Nella pagina dei dettagli del cliente, selezionare **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9042a-137">Sotto **profili Windows Autopilot** selezionate **aggiungere nuovo profilo**.</span><span class="sxs-lookup"><span data-stu-id="9042a-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="9042a-138">Immettere nome e una descrizione del profilo e quindi configurare le impostazioni di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="9042a-139">Scegliere tra:</span><span class="sxs-lookup"><span data-stu-id="9042a-139">Choose from:</span></span>  

   - <span data-ttu-id="9042a-140">Ignorare le impostazioni di privacy nel programma di installazione</span><span class="sxs-lookup"><span data-stu-id="9042a-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="9042a-141">Disabilitare l'account amministratore locale durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="9042a-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="9042a-142">Ignorare automaticamente le pagine durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="9042a-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="9042a-143">(Include *automaticamente seleziona il programma di installazione per l'azienda o dell'istituto di istruzione* e *pagine di configurazione di registrazione OEM, OneDrive e Skip Cortana*)</span><span class="sxs-lookup"><span data-stu-id="9042a-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="9042a-144">Ignorare il contratto di licenza utente finale (EULA)</span><span class="sxs-lookup"><span data-stu-id="9042a-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="9042a-145">Visualizzare [licenziamento condizioni di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da considerare su come ignorare la pagina Contratto di licenza Windows durante l'installazione.</span><span class="sxs-lookup"><span data-stu-id="9042a-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="9042a-146">Al termine seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="9042a-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="9042a-147">Applicare un profilo di Autopilot per i dispositivi dei clienti</span><span class="sxs-lookup"><span data-stu-id="9042a-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="9042a-148">Le istruzioni seguenti presuppongono che i dispositivi del cliente è già stato aggiunto al centro per i Partner e che sia possibile accedere proprio elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="9042a-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="9042a-149">Se è già stato aggiunto i dispositivi del cliente, seguire le istruzioni in [aggiungere i dispositivi a un account del cliente](#add-devices-to-a-customers-account) e quindi seguire la procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="9042a-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="9042a-150">Dopo aver creato un profilo di Autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="9042a-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="9042a-151">Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente creato per il profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="9042a-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9042a-152">Nella pagina dei dettagli del cliente, selezionare **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9042a-153">Sotto **applicare i profili nei dispositivi** selezionare i dispositivi o gruppi di dispositivi che si desidera aggiungere i profili e quindi selezionare **applicare profilo**.</span><span class="sxs-lookup"><span data-stu-id="9042a-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="9042a-154">Il profilo appena applicati viene visualizzato nei **profilo** colonna.</span><span class="sxs-lookup"><span data-stu-id="9042a-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="9042a-155">Attenersi alla procedura seguente per verificare che il profilo verrà applicato correttamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9042a-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="9042a-156">a.</span><span class="sxs-lookup"><span data-stu-id="9042a-156">a.</span></span>  <span data-ttu-id="9042a-157">Connettere un dispositivo alla rete e attivarlo.</span><span class="sxs-lookup"><span data-stu-id="9042a-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="9042a-158">b.</span><span class="sxs-lookup"><span data-stu-id="9042a-158">b.</span></span>  <span data-ttu-id="9042a-159">Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="9042a-160">c.</span><span class="sxs-lookup"><span data-stu-id="9042a-160">c.</span></span>  <span data-ttu-id="9042a-161">Quando si arresta il processo di configurazione guidata, reimpostare il dispositivo per le impostazioni predefinite per prepararlo per un nuovo utente.</span><span class="sxs-lookup"><span data-stu-id="9042a-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="9042a-162">Rimuovere un profilo di Autopilot da dispositivo del cliente</span><span class="sxs-lookup"><span data-stu-id="9042a-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="9042a-163">Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente creato per il profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="9042a-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9042a-164">Nella pagina dei dettagli del cliente, selezionare **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9042a-165">Sotto **applicare i profili nei dispositivi** selezionare i dispositivi che si desidera rimuovere il profilo e quindi selezionare **rimuovere il profilo**.</span><span class="sxs-lookup"><span data-stu-id="9042a-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="9042a-166">Rimozione di un profilo da un dispositivo non elimina il profilo dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="9042a-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="9042a-167">Se si desidera eliminare un profilo, seguire le istruzioni in [Update o delete un profilo di Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="9042a-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="9042a-168">Aggiornare o eliminare un profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="9042a-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="9042a-169">Se un cliente vuole modificare l'esperienza di out-of-box dopo che è stato spedito i loro dispositivi, è possibile modificare il profilo nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="9042a-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="9042a-170">Quando il dispositivo del cliente si connette a internet, verrà scaricato la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="9042a-171">Inoltre, ogni volta che un cliente consente di ripristinare un dispositivo per le impostazioni predefinite, il dispositivo nuovamente scaricherà l'ultima versione del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="9042a-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="9042a-172">Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente che si desidera modificare un profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="9042a-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="9042a-173">Nella pagina dei dettagli del cliente, selezionare **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9042a-174">Sotto **profili Windows Autopilot** selezionare il profilo è necessario aggiornare.</span><span class="sxs-lookup"><span data-stu-id="9042a-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="9042a-175">Apportare le modifiche necessarie e quindi selezionare **Submit**.</span><span class="sxs-lookup"><span data-stu-id="9042a-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="9042a-176">Per eliminare questo profilo, selezionare **eliminare il profilo** dall'angolo superiore destro della pagina.</span><span class="sxs-lookup"><span data-stu-id="9042a-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="9042a-177">Aggiungere i dispositivi a un account del cliente</span><span class="sxs-lookup"><span data-stu-id="9042a-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="9042a-178">Gli agenti di vendita e amministratore possono aggiungere dispositivi all'account del cliente.</span><span class="sxs-lookup"><span data-stu-id="9042a-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="9042a-179">Prima di poter applicare i profili di Autopilot personalizzati per i dispositivi dei clienti, è necessario essere in grado di accedere all'elenco dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="9042a-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="9042a-180">Se si prevede di usare il nome OEM, numero di serie e combinazione di modello, tenere presente queste limitazioni:</span><span class="sxs-lookup"><span data-stu-id="9042a-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="9042a-181">Questa tupla funziona solo per i dispositivi più recenti (4 k gli hash, ad esempio) e non è supportata per gli hash 128b (RS2 e dispositivi precedenti).</span><span class="sxs-lookup"><span data-stu-id="9042a-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="9042a-182">La registrazione di tupla viene fatta distinzione tra maiuscole e minuscole, in modo che i dati nel file devono corrispondere ai nomi di produttore e modello ***esattamente*** fornito dal provider OEM (provider hardware).</span><span class="sxs-lookup"><span data-stu-id="9042a-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="9042a-183">Seguire le istruzioni seguenti per aggiungere i dispositivi per conto del cliente nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="9042a-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="9042a-184">Selezionare **clienti** dal centro per i Partner menu e quindi selezionare il cliente con i dispositivi da gestire.</span><span class="sxs-lookup"><span data-stu-id="9042a-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="9042a-185">Nella pagina dei dettagli del cliente, selezionare **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9042a-186">Sotto **applicare i profili nei dispositivi** selezionate **aggiungere dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="9042a-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="9042a-187">Immettere un nome per l'elenco dei dispositivi e quindi selezionare **esplorare** per caricare l'elenco del cliente (nel formato di file con estensione csv) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9042a-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9042a-188">Dovrebbe avere inviato questo file con estensione csv con l'acquisto di dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9042a-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="9042a-189">Se non è stato ricevuto un file con estensione csv, è possibile creare uno manualmente seguendo la procedura descritta in [aggiunta di dispositivi a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="9042a-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="9042a-190">Caricare il file con estensione csv e quindi selezionare **salvare**.</span><span class="sxs-lookup"><span data-stu-id="9042a-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="9042a-191">Se viene visualizzato un messaggio di errore durante il tentativo di caricare il file con estensione csv, controllare il formato del file.</span><span class="sxs-lookup"><span data-stu-id="9042a-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="9042a-192">È possibile usare solo l'hash hardware o il nome OEM, il numero di serie e modello (in tale ordine delle colonne) o l'ID prodotto Windows.</span><span class="sxs-lookup"><span data-stu-id="9042a-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="9042a-193">È anche possibile usare il file CSV di esempio fornito dal collegamento accanto a **aggiungere i dispositivi** per creare un elenco dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="9042a-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="9042a-194">Licenziamento condizioni di licenza di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="9042a-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="9042a-195">INFORMAZIONI IMPORTANTI</span><span class="sxs-lookup"><span data-stu-id="9042a-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="9042a-196">Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti.</span><span class="sxs-lookup"><span data-stu-id="9042a-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="9042a-197">Se autorizzato a eseguire questa operazione dal cliente, è possibile eliminare o nascondere alcune schermate di configurazione che normalmente vengono presentate all'utente durante la configurazione di Windows, tra cui la schermata di accettazione di condizioni di licenza (End User License Agreement).</span><span class="sxs-lookup"><span data-stu-id="9042a-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="9042a-198">Tramite questa funzione, si accetta che l'eliminazione o nascondere tutte le schermate che sono progettate per offrire agli utenti con avviso o l'accettazione di mezzi di termini di avere ottenuto il consenso sufficiente e l'autorizzazione dal cliente per nascondere i termini e, per conto di il cliente (se un'organizzazione o un singolo utente come nel caso può essere), fornire il consenso a eventuali comunicazioni e accettare le condizioni applicabili al cliente.</span><span class="sxs-lookup"><span data-stu-id="9042a-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="9042a-199">Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento.</span><span class="sxs-lookup"><span data-stu-id="9042a-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="9042a-200">Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.</span><span class="sxs-lookup"><span data-stu-id="9042a-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>