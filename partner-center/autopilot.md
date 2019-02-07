---
title: Personalizzare l'esperienza out-of-box di un dispositivo con i profili di Windows Autopilot | Centro per i partner
description: Preconfigurare esperienza out-of-box di un dispositivo con i profili Autopilot.
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot windows, autopilot microsoft, distribuzione automatica, configurazione guidata, schermate di accesso, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062279"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="009f3-104">Personalizzare l'esperienza out-of-box di un dispositivo con i profili di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="009f3-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="009f3-105">Si applica a</span><span class="sxs-lookup"><span data-stu-id="009f3-105">Applies to</span></span>**

- <span data-ttu-id="009f3-106">I partner direct-fattura CSP, i provider indiretti e i rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="009f3-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="009f3-107">Se si gestiscono i dispositivi dei clienti, devi personalizzare l'esperienza di out-of-box (OOBE) per gli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="009f3-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="009f3-108">Puoi pre-configurare nuovi dispositivi con i profili di Windows Autopilot prima della consegna i dispositivi per i clienti e applicare i profili di nuovo ai dispositivi i clienti hanno già acquistato.</span><span class="sxs-lookup"><span data-stu-id="009f3-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="009f3-109">Questo articolo spiega come creare e applicare i profili Autopilot ai dispositivi nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="009f3-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="009f3-110">Se non sei già familiarità con Autopilot, controlla le informazioni in questi articoli:</span><span class="sxs-lookup"><span data-stu-id="009f3-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="009f3-111">Panoramica di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="009f3-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="009f3-112">Guida di riferimento di distribuzione AutoPilot</span><span class="sxs-lookup"><span data-stu-id="009f3-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="009f3-113">Panoramica</span><span class="sxs-lookup"><span data-stu-id="009f3-113">Overview</span></span>

<span data-ttu-id="009f3-114">Con la funzionalità di Windows Autopilot nel centro per i Partner, puoi creare profili personalizzati da applicare ai dispositivi dei clienti.</span><span class="sxs-lookup"><span data-stu-id="009f3-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="009f3-115">Le seguenti impostazioni del profilo erano disponibili al momento della che pubblicazione di questo articolo:</span><span class="sxs-lookup"><span data-stu-id="009f3-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="009f3-116">Ignorare le impostazioni di privacy.</span><span class="sxs-lookup"><span data-stu-id="009f3-116">Skip privacy settings.</span></span> <span data-ttu-id="009f3-117">Questa impostazione facoltativa di profilo Autopilot consente alle organizzazioni di non chiedere informazioni sulle impostazioni di privacy durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="009f3-118">Disabilitare la creazione di un account amministratore locale nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="009f3-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="009f3-119">Le organizzazioni possono decidere se l'utente di configurare il dispositivo deve avere accesso come amministratore, una volta completato il processo.</span><span class="sxs-lookup"><span data-stu-id="009f3-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="009f3-120">Configura automaticamente dispositivo per l'azienda o all'istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="009f3-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="009f3-121">Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati aziendale o dell'istituto di istruzione dispositivi, in modo che questa domanda non verrà richiesto durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="009f3-122">Ignorare le pagine di configurazione registrazione OEM, OneDrive e Cortana.</span><span class="sxs-lookup"><span data-stu-id="009f3-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="009f3-123">Tutti i dispositivi registrati con Autopilot salterà automaticamente queste pagine durante il processo di out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="009f3-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="009f3-124">Ignora il contratto di licenza utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="009f3-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="009f3-125">A partire da Windows 10 versione 1709, le organizzazioni possono decidere di saltare la pagina di condizioni di licenza presentata durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="009f3-126">Vedi l' [interruzione dell'EULA di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da prendere in considerazione su ignorare la pagina di condizioni di licenza durante l'installazione di Windows.</span><span class="sxs-lookup"><span data-stu-id="009f3-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="009f3-127">Applicano le autorizzazioni di gestione di profilo e del dispositivo e limitazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="009f3-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="009f3-128">I partner CSP possono continuare a gestire i profili Autopilot per i clienti esistenti con cui hanno relazioni come rivenditore, anche se i clienti hanno rimosso i privilegi di privilegi di amministratore delegato del partner.</span><span class="sxs-lookup"><span data-stu-id="009f3-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="009f3-129">È possibile gestire i dispositivi esistenti per i clienti che sono stati aggiunti da te o da un altro partner CSP.</span><span class="sxs-lookup"><span data-stu-id="009f3-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="009f3-130">Non puoi gestire i dispositivi che caricati dal tuo cliente a Microsoft Store per le aziende o il portale di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="009f3-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="009f3-131">Creare e gestire i profili Autopilot nel centro per i Partner</span><span class="sxs-lookup"><span data-stu-id="009f3-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="009f3-132">Nel centro per i Partner, puoi creare profili di distribuzione Windows Autopilot e applicarli ai dispositivi.</span><span class="sxs-lookup"><span data-stu-id="009f3-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="009f3-133">Solo gli agenti amministratore possono creare e applicare i profili.</span><span class="sxs-lookup"><span data-stu-id="009f3-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="009f3-134">Creare un nuovo profilo Autopilot</span><span class="sxs-lookup"><span data-stu-id="009f3-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="009f3-135">Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che quando crei il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="009f3-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="009f3-136">Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="009f3-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="009f3-137">Selezionare **Aggiungi nuovo profilo** **Windows Autopilot profili** .</span><span class="sxs-lookup"><span data-stu-id="009f3-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="009f3-138">Immetti nome e una descrizione del profilo e quindi Configura le impostazioni di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="009f3-139">Scegliere tra:</span><span class="sxs-lookup"><span data-stu-id="009f3-139">Choose from:</span></span>  

   - <span data-ttu-id="009f3-140">Ignora impostazioni di privacy durante l'installazione</span><span class="sxs-lookup"><span data-stu-id="009f3-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="009f3-141">Disabilitare l'account amministratore locale durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="009f3-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="009f3-142">Ignorare automaticamente le pagine durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="009f3-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="009f3-143">(Include *Seleziona automaticamente la configurazione per l'azienda o all'istituto di istruzione* e *le pagine di configurazione registrazione OEM, OneDrive e Ignora Cortana*)</span><span class="sxs-lookup"><span data-stu-id="009f3-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="009f3-144">Ignora il contratto di licenza utente finale (EULA)</span><span class="sxs-lookup"><span data-stu-id="009f3-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="009f3-145">Vedi l' [interruzione dell'EULA di Windows Autopilot](#windows-autopilot-eula-dismissal) seguito per informazioni importanti da prendere in considerazione su ignorare la pagina di condizioni di licenza durante l'installazione di Windows.</span><span class="sxs-lookup"><span data-stu-id="009f3-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="009f3-146">Al termine seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="009f3-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="009f3-147">Applicare un profilo Autopilot ai dispositivi dei clienti</span><span class="sxs-lookup"><span data-stu-id="009f3-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="009f3-148">Le istruzioni seguenti presuppongono che hai già aggiunto i dispositivi del cliente nel centro per i Partner e che sia possibile accedere l'elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="009f3-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="009f3-149">Se non lo hai già aggiunto i dispositivi del cliente, segui le istruzioni in [dispositivi Aggiungi all'account del cliente](#add-devices-to-a-customers-account) e quindi seguire i passaggi seguenti.</span><span class="sxs-lookup"><span data-stu-id="009f3-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="009f3-150">Dopo aver creato un profilo Autopilot per un cliente, puoi applicare ai dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="009f3-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="009f3-151">Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="009f3-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="009f3-152">Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="009f3-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="009f3-153">Selezionare i dispositivi o gruppi di dispositivi che vuoi aggiungere i profili e quindi selezionare **Applica profilo** **Applica profili ai dispositivi** .</span><span class="sxs-lookup"><span data-stu-id="009f3-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="009f3-154">Il profilo che è stato applicato solo verrà visualizzato nella colonna **profilo** .</span><span class="sxs-lookup"><span data-stu-id="009f3-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="009f3-155">Segui i passaggi seguenti per verificare che il profilo verrà applicato correttamente nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="009f3-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="009f3-156">a.</span><span class="sxs-lookup"><span data-stu-id="009f3-156">a.</span></span>  <span data-ttu-id="009f3-157">Connettere un dispositivo alla rete e accendilo.</span><span class="sxs-lookup"><span data-stu-id="009f3-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="009f3-158">b.</span><span class="sxs-lookup"><span data-stu-id="009f3-158">b.</span></span>  <span data-ttu-id="009f3-159">Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="009f3-160">c.</span><span class="sxs-lookup"><span data-stu-id="009f3-160">c.</span></span>  <span data-ttu-id="009f3-161">Quando si interrompe il processo di configurazione guidata, reimpostare il dispositivo per impostazioni predefinite di fabbrica per prepararla per un nuovo utente.</span><span class="sxs-lookup"><span data-stu-id="009f3-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="009f3-162">Rimuovere un profilo Autopilot dal dispositivo del cliente</span><span class="sxs-lookup"><span data-stu-id="009f3-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="009f3-163">Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente per che è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="009f3-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="009f3-164">Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="009f3-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="009f3-165">Selezionare i dispositivi che vuoi rimuovere il profilo e quindi seleziona **rimuovere profilo** **Applica profili ai dispositivi** .</span><span class="sxs-lookup"><span data-stu-id="009f3-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="009f3-166">Rimozione di un profilo da un dispositivo non eliminare il profilo dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="009f3-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="009f3-167">Se si desidera eliminare un profilo, segui le istruzioni in [aggiornamento o eliminare un profilo Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="009f3-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="009f3-168">Aggiornare o eliminare un profilo Autopilot</span><span class="sxs-lookup"><span data-stu-id="009f3-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="009f3-169">Se un cliente desidera modificare l'esperienza out-of-box dopo che hai fornito i dispositivi su di essi, è possibile modificare il profilo nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="009f3-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="009f3-170">Quando il dispositivo del cliente si connette a internet, verranno scaricati la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="009f3-171">Inoltre, ogni volta che un cliente Ripristina impostazioni predefinite di fabbrica, un dispositivo il dispositivo verrà nuovamente scaricare la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="009f3-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="009f3-172">Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente che desidera modificare un profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="009f3-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="009f3-173">Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="009f3-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="009f3-174">Selezionare il profilo che è necessario aggiornare **i profili di Windows Autopilot** .</span><span class="sxs-lookup"><span data-stu-id="009f3-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="009f3-175">Apporta le modifiche necessarie e quindi seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="009f3-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="009f3-176">Per eliminare il profilo, seleziona **eliminare il profilo** nell'angolo superiore destro della pagina.</span><span class="sxs-lookup"><span data-stu-id="009f3-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="009f3-177">Aggiungere i dispositivi all'account del cliente</span><span class="sxs-lookup"><span data-stu-id="009f3-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="009f3-178">Gli agenti di vendita e agenti amministratore possono aggiungere i dispositivi per conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="009f3-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="009f3-179">Prima di poter applicare i profili Autopilot personalizzati per i dispositivi dei clienti, è necessario essere in grado di accedere all'elenco di dispositivo del cliente.</span><span class="sxs-lookup"><span data-stu-id="009f3-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="009f3-180">Se si prevede di usare il nome OEM, il numero di serie e combinazione di modello, tieni presente queste limitazioni:</span><span class="sxs-lookup"><span data-stu-id="009f3-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="009f3-181">Questa versione tupla funziona solo per i dispositivi più recente (4 k hash, ad esempio) e non è supportato per 128b hash (RS2 e dispositivi precedenti).</span><span class="sxs-lookup"><span data-stu-id="009f3-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="009f3-182">La registrazione tupla è tra maiuscole e minuscole, in modo che i dati nel file devono corrispondere il modello e produttore nomi ***esattamente*** come specificato dal provider di OEM (provider hardware).</span><span class="sxs-lookup"><span data-stu-id="009f3-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="009f3-183">Segui le istruzioni seguenti per aggiungere i dispositivi per conto del cliente nel centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="009f3-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="009f3-184">Seleziona **clienti** dal menu di Centro per i Partner e quindi seleziona il cliente di cui desideri gestire i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="009f3-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="009f3-185">Nella pagina dei dettagli del cliente, seleziona **i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="009f3-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="009f3-186">Selezionare **Aggiungi dispositivi** **Applica profili ai dispositivi** .</span><span class="sxs-lookup"><span data-stu-id="009f3-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="009f3-187">Immetti un nome per l'elenco dei dispositivi e quindi seleziona **Sfoglia** per caricare l'elenco del cliente (in formato di file con estensione csv) al centro per i Partner.</span><span class="sxs-lookup"><span data-stu-id="009f3-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="009f3-188">Dovrebbe aver ricevuto il file CSV con l'acquisto di dispositivo.</span><span class="sxs-lookup"><span data-stu-id="009f3-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="009f3-189">Se non ricevi un file con estensione csv, è possibile creare una personalizzata seguendo i passaggi descritti in [aggiunta i dispositivi Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="009f3-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="009f3-190">Caricare il file CSV e quindi seleziona **salvare**.</span><span class="sxs-lookup"><span data-stu-id="009f3-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="009f3-191">Se ricevi un messaggio di errore durante il tentativo di caricare il file con estensione csv, controlla il formato del file.</span><span class="sxs-lookup"><span data-stu-id="009f3-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="009f3-192">È possibile utilizzare, solo l'hash hardware o il nome dell'OEM, il numero di serie e modello (in questo ordine colonna) o l'ID prodotto Windows.</span><span class="sxs-lookup"><span data-stu-id="009f3-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="009f3-193">È inoltre possibile utilizzare il file CSV di esempio fornito dal collegamento accanto **Aggiungi dispositivi** per creare un elenco dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="009f3-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="009f3-194">Interruzione dell'EULA di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="009f3-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="009f3-195">INFORMAZIONI IMPORTANTI</span><span class="sxs-lookup"><span data-stu-id="009f3-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="009f3-196">Windows Autopilot consente di configurare le installazioni personalizzate di Windows nei dispositivi gestiti per i tuoi clienti.</span><span class="sxs-lookup"><span data-stu-id="009f3-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="009f3-197">Se disponi dell'autorizzazione per eseguire questa operazione dal cliente, puoi eliminare o nascondere alcune schermate di installazione che normalmente vengono visualizzate agli utenti durante la configurazione di Windows, tra cui lo schermo di accettazione del contratto di licenza (contratto di licenza utente finale).</span><span class="sxs-lookup"><span data-stu-id="009f3-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="009f3-198">Utilizzando questa funzione, accetti che eliminando o nascondendo le schermate progettate per fornire agli utenti avviso o l'accettazione delle condizioni indica di avere ricevuto il consenso sufficiente e l'autorizzazione dal cliente per nascondere i termini e che si, per conto di il cliente (se un'organizzazione o singolo utente nel caso potrebbe essere), gli avvisi e accettare le condizioni applicabili al cliente.</span><span class="sxs-lookup"><span data-stu-id="009f3-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="009f3-199">Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento.</span><span class="sxs-lookup"><span data-stu-id="009f3-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="009f3-200">Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.</span><span class="sxs-lookup"><span data-stu-id="009f3-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>