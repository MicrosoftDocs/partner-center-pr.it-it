---
title: Personalizzare l'esperienza predefinita di un dispositivo con i profili di Windows Autopilot | Centro per i partner
description: Preconfigurare l'esperienza predefinita di un dispositivo con i profili Autopilot.
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, distribuzione Zero-Touch, OOBE, schermate di accesso, predefinite
ms.localizationpriority: medium
ms.openlocfilehash: 213ed9e45e0109eaa88d7575249272ba403dfcfd
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708748"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="2c7f8-104">Personalizzare l'esperienza predefinita di un dispositivo con i profili di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="2c7f8-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="2c7f8-105">**Applies to**</span></span>

- <span data-ttu-id="2c7f8-106">CSP Direct-fatturazione partner, provider indiretti e rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="2c7f8-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="2c7f8-107">Se si gestiscono i dispositivi dei clienti, potrebbe essere necessario personalizzare l'esperienza predefinita per gli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="2c7f8-108">È possibile preconfigurare nuovi dispositivi con i profili di Windows Autopilot prima di consegnare i dispositivi ai clienti e applicare nuovi profili ai dispositivi che i clienti hanno già acquistato.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="2c7f8-109">Si noti che gli OEM hanno iniziato ad includere un'etichetta di spedizione all'esterno della casella dispositivo Autopilot che mostra l' **ID del codice Product Key (pkID)** del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-109">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device’s **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="2c7f8-110">Questo codice a barre leggibile e unidimensionale fornisce ai partner downstream un modo per registrare i dispositivi per Autopilot senza dover sottoporre a unboxing i dispositivi e raccogliere l'ID del dispositivo in modo alternativo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-110">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="2c7f8-111">Questo articolo illustra come creare e applicare i profili di Autopilot ai dispositivi nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-111">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="2c7f8-112">Se non si ha già familiarità con Autopilot, rivedere le informazioni contenute in questi articoli:</span><span class="sxs-lookup"><span data-stu-id="2c7f8-112">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="2c7f8-113">Panoramica di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-113">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="2c7f8-114">Guida di riferimento per la distribuzione di Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-114">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="2c7f8-115">Panoramica</span><span class="sxs-lookup"><span data-stu-id="2c7f8-115">Overview</span></span>

<span data-ttu-id="2c7f8-116">Con la funzionalità Windows Autopilot in centro per i partner, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-116">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="2c7f8-117">Al momento della pubblicazione di questo articolo sono disponibili le impostazioni di profilo seguenti:</span><span class="sxs-lookup"><span data-stu-id="2c7f8-117">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="2c7f8-118">Ignora le impostazioni di privacy.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-118">Skip privacy settings.</span></span> <span data-ttu-id="2c7f8-119">Questa impostazione facoltativa del profilo di Autopilot consente alle organizzazioni di non richiedere informazioni sulle impostazioni della privacy durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-119">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="2c7f8-120">Disabilitare la creazione dell'account amministratore locale nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-120">Disable local admin account creation on the device.</span></span> <span data-ttu-id="2c7f8-121">Le organizzazioni possono decidere se l'utente che configura il dispositivo deve avere l'accesso come amministratore al termine del processo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-121">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="2c7f8-122">Configurare automaticamente il dispositivo per l'ufficio o l'Istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-122">Automatically set up device for work or school.</span></span> <span data-ttu-id="2c7f8-123">Tutti i dispositivi registrati con Autopilot verranno considerati automaticamente dispositivi aziendali o dell'Istituto di istruzione, pertanto questa domanda non verrà richiesta durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-123">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="2c7f8-124">Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-124">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="2c7f8-125">Tutti i dispositivi registrati con Autopilot ignoreranno automaticamente queste pagine durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-125">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="2c7f8-126">Ignora il contratto di licenza con l'utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-126">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="2c7f8-127">A partire da Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina EULA visualizzata durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-127">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="2c7f8-128">Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="2c7f8-128">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="2c7f8-129">Si applicano le limitazioni e le autorizzazioni di gestione dei profili e dei dispositivi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2c7f8-129">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="2c7f8-130">I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti con le relazioni rivenditore, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-130">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="2c7f8-131">È possibile gestire i dispositivi esistenti per i clienti aggiunti.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-131">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="2c7f8-132">Non è possibile gestire i dispositivi caricati dal cliente in Microsoft Store for business o nel portale di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-132">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="2c7f8-133">Creare e gestire i profili di Autopilot nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2c7f8-133">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="2c7f8-134">Nel centro per i partner è possibile creare profili di distribuzione di Windows Autopilot e applicarli ai dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-134">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="2c7f8-135">Solo gli agenti amministratori possono creare e applicare profili.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-135">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="2c7f8-136">Crea un nuovo profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-136">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="2c7f8-137">Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente per il quale si sta creando il profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-137">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="2c7f8-138">Nella pagina dei dettagli del cliente selezionare Devices ( **dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-138">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2c7f8-139">In **profili di Windows Autopilot** selezionare **Aggiungi nuovo profilo**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-139">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="2c7f8-140">Immettere il nome e la descrizione del profilo e quindi configurare le impostazioni della configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-140">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="2c7f8-141">Scegliere tra:</span><span class="sxs-lookup"><span data-stu-id="2c7f8-141">Choose from:</span></span>  

   - <span data-ttu-id="2c7f8-142">Ignora le impostazioni di privacy nel programma di installazione</span><span class="sxs-lookup"><span data-stu-id="2c7f8-142">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="2c7f8-143">Disabilitare l'account amministratore locale durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="2c7f8-143">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="2c7f8-144">Ignorare automaticamente le pagine durante la configurazione</span><span class="sxs-lookup"><span data-stu-id="2c7f8-144">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="2c7f8-145">(Include *automaticamente seleziona configurazione per lavoro o scuola* e *Ignora le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM*)</span><span class="sxs-lookup"><span data-stu-id="2c7f8-145">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="2c7f8-146">Ignora il contratto di licenza con l'utente finale (EULA)</span><span class="sxs-lookup"><span data-stu-id="2c7f8-146">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="2c7f8-147">Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="2c7f8-147">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="2c7f8-148">Al termine seleziona **Invia**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-148">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="2c7f8-149">Applicare un profilo di Autopilot ai dispositivi dei clienti</span><span class="sxs-lookup"><span data-stu-id="2c7f8-149">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="2c7f8-150">Le istruzioni seguenti presuppongono che siano già stati aggiunti i dispositivi del cliente al centro per i partner e che sia possibile accedere all'elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-150">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="2c7f8-151">Se non sono stati ancora aggiunti i dispositivi del cliente, seguire le istruzioni riportate in [aggiungere dispositivi a un account del cliente](#add-devices-to-a-customers-account) e quindi seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-151">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="2c7f8-152">Dopo aver creato un profilo di Autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-152">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="2c7f8-153">Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-153">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2c7f8-154">Nella pagina dei dettagli del cliente selezionare Devices ( **dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-154">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2c7f8-155">In **applica profili ai dispositivi** selezionare i dispositivi o i gruppi di dispositivi a cui si vogliono aggiungere i profili e quindi selezionare **Applica profilo**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-155">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="2c7f8-156">Il profilo appena applicato viene visualizzato nella colonna **profilo** .</span><span class="sxs-lookup"><span data-stu-id="2c7f8-156">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="2c7f8-157">Attenersi alla procedura seguente per verificare che il profilo venga applicato correttamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-157">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="2c7f8-158">a.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-158">a.</span></span>  <span data-ttu-id="2c7f8-159">Connettere un dispositivo alla rete e attivarlo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-159">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="2c7f8-160">b.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-160">b.</span></span>  <span data-ttu-id="2c7f8-161">Verifica che siano visualizzate le eventuali schermate appropriate della Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-161">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="2c7f8-162">c.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-162">c.</span></span>  <span data-ttu-id="2c7f8-163">Quando il processo OOBE si interrompe, ripristinare le impostazioni predefinite del dispositivo per prepararlo per un nuovo utente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-163">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="2c7f8-164">Rimuovere un profilo di Autopilot dal dispositivo di un cliente</span><span class="sxs-lookup"><span data-stu-id="2c7f8-164">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="2c7f8-165">Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-165">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2c7f8-166">Nella pagina dei dettagli del cliente selezionare Devices ( **dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-166">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2c7f8-167">In **applica profili ai dispositivi** selezionare i dispositivi da cui si desidera rimuovere il profilo, quindi selezionare **Rimuovi profilo**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-167">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2c7f8-168">La rimozione di un profilo da un dispositivo non comporta l'eliminazione del profilo dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-168">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="2c7f8-169">Per eliminare un profilo, seguire le istruzioni riportate in [aggiornare o eliminare un profilo](#update-or-delete-an-autopilot-profile)di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-169">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="2c7f8-170">Aggiornare o eliminare un profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-170">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="2c7f8-171">Se un cliente vuole modificare l'esperienza predefinita dopo aver spedito i dispositivi, è possibile modificare il profilo nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-171">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="2c7f8-172">Quando il dispositivo del cliente si connette a Internet, verrà scaricata la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-172">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="2c7f8-173">Inoltre, ogni volta che un cliente Ripristina le impostazioni predefinite di un dispositivo, il dispositivo Scarica di nuovo la versione più recente del profilo durante il processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-173">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="2c7f8-174">Selezionare **Customers** dal menu centro per i partner e quindi selezionare il cliente che desidera modificare un profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-174">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="2c7f8-175">Nella pagina dei dettagli del cliente selezionare Devices ( **dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-175">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2c7f8-176">In **profili di Windows Autopilot** selezionare il profilo che si desidera aggiornare.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-176">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="2c7f8-177">Apportare le modifiche necessarie e quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-177">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="2c7f8-178">Per eliminare questo profilo, selezionare **Elimina profilo** nell'angolo superiore destro della pagina.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-178">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="2c7f8-179">Aggiungere dispositivi all'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="2c7f8-179">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="2c7f8-180">Gli agenti di vendita e gli agenti di amministrazione possono aggiungere dispositivi a un account del cliente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-180">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="2c7f8-181">Prima di poter applicare profili Autopilot personalizzati ai dispositivi dei clienti, è necessario essere in grado di accedere all'elenco di dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-181">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="2c7f8-182">Se si prevede di utilizzare il nome OEM, il numero di serie e la combinazione di modelli, tenere presente queste limitazioni:</span><span class="sxs-lookup"><span data-stu-id="2c7f8-182">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="2c7f8-183">Questa tupla funziona solo per i dispositivi più recenti (ad esempio, gli hash 4K) e non è supportata per gli hash 128B (RS2 e i dispositivi precedenti).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-183">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="2c7f8-184">Per la registrazione della tupla viene fatta distinzione tra maiuscole e minuscole, pertanto i dati nel file devono corrispondere ai nomi del modello e del produttore ***esattamente*** come fornito dal provider OEM (provider hardware).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-184">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="2c7f8-185">Seguire le istruzioni riportate di seguito per aggiungere i dispositivi all'account di un cliente nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-185">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="2c7f8-186">Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente di cui si vogliono gestire i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-186">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="2c7f8-187">Nella pagina dei dettagli del cliente selezionare Devices ( **dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-187">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2c7f8-188">In **applica profili ai dispositivi** selezionare **Aggiungi dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-188">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="2c7f8-189">Immettere un nome per l'elenco dei dispositivi e quindi selezionare **Sfoglia** per caricare l'elenco del cliente (in formato file CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-189">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2c7f8-190">Il file con estensione CSV è stato ricevuto con l'acquisto del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-190">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="2c7f8-191">Se non si riceve un file con estensione CSV, è possibile crearne uno seguendo i passaggi descritti in [aggiunta di dispositivi a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-191">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="2c7f8-192">Caricare il file con estensione CSV e quindi selezionare **Save (Salva**).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-192">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="2c7f8-193">Se viene ricevuto un messaggio di errore durante il tentativo di caricare il file CSV, controllare il formato del file.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-193">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="2c7f8-194">È possibile utilizzare solo l'hash hardware oppure il nome OEM, il numero di serie e il modello (nell'ordine di tale colonna) o l'ID del prodotto Windows.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-194">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="2c7f8-195">È anche possibile usare il file CSV di esempio fornito dal collegamento accanto a **Aggiungi dispositivi** per creare un elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-195">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="2c7f8-196">Dismissing EULA di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2c7f8-196">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="2c7f8-197">INFORMAZIONI IMPORTANTI</span><span class="sxs-lookup"><span data-stu-id="2c7f8-197">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="2c7f8-198">Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-198">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="2c7f8-199">Se il cliente è autorizzato a eseguire questa operazione, è possibile disattivare o nascondere alcune schermate di configurazione che in genere vengono presentate agli utenti durante la configurazione di Windows, inclusa la schermata di accettazione del contratto di licenza con l'utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="2c7f8-199">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="2c7f8-200">Utilizzando questa funzione, l'utente accetta che l'eliminazione o la disattivazione delle schermate progettate per fornire agli utenti la comunicazione o l'accettazione delle condizioni significa che l'utente ha ottenuto il consenso e l'autorizzazione sufficienti per nascondere i termini e che l'utente, per conto di il cliente (indipendentemente dal fatto che si tratti di un'organizzazione o di un singolo utente come caso), acconsente a qualsiasi comunicazione e accetti le condizioni applicabili al cliente.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-200">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="2c7f8-201">Ciò include il contratto per le condizioni della licenza o dell'avviso che potrebbero essere presentati all'utente se non è stato scelto di non visualizzare o di nascondere usando questo strumento.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-201">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="2c7f8-202">Il cliente non può utilizzare il software Windows su tali dispositivi se non ha acquisito validamente una licenza per il software da Microsoft o dai distributori autorizzati.</span><span class="sxs-lookup"><span data-stu-id="2c7f8-202">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
