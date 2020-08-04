---
title: Personalizzare l'esperienza predefinita di un dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Prima di consegnare il nuovo dispositivo di un cliente, è possibile usare i profili di Windows Autopilot per personalizzare o preconfigurare l'esperienza predefinita del dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a59b0c25b8f5203942e73b549d5ffb9d65d90c36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527657"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="c1469-103">Usare i profili di Windows Autopilot nei nuovi dispositivi per personalizzare l'esperienza predefinita di un cliente</span><span class="sxs-lookup"><span data-stu-id="c1469-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="c1469-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="c1469-104">**Applies to**</span></span>

- <span data-ttu-id="c1469-105">CSP Direct-fatturazione partner, provider indiretti e rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="c1469-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="c1469-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="c1469-106">**Appropriate roles**</span></span>

- <span data-ttu-id="c1469-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="c1469-107">Admin agent</span></span>
- <span data-ttu-id="c1469-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c1469-108">Global admin</span></span>
- <span data-ttu-id="c1469-109">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="c1469-109">Sales agent</span></span>
- <span data-ttu-id="c1469-110">Amministratore gestione utenti</span><span class="sxs-lookup"><span data-stu-id="c1469-110">User management admin</span></span>

<span data-ttu-id="c1469-111">Se si gestiscono i dispositivi dei clienti, potrebbe essere necessario personalizzare l'esperienza predefinita per gli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="c1469-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="c1469-112">È possibile preconfigurare nuovi dispositivi con i profili di Windows Autopilot prima di consegnare i dispositivi ai clienti e applicare nuovi profili ai dispositivi che i clienti hanno già acquistato.</span><span class="sxs-lookup"><span data-stu-id="c1469-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="c1469-113">Si noti che gli OEM hanno iniziato ad includere un'etichetta di spedizione all'esterno della casella dispositivo Autopilot che mostra l' **ID del codice Product Key (pkID)** del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1469-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="c1469-114">Questo codice a barre leggibile e unidimensionale fornisce ai partner downstream un modo per registrare i dispositivi per Autopilot senza dover sottoporre a unboxing i dispositivi e raccogliere l'ID del dispositivo in modo alternativo.</span><span class="sxs-lookup"><span data-stu-id="c1469-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="c1469-115">Questo articolo illustra come creare e applicare i profili di Autopilot ai dispositivi nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1469-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="c1469-116">Se non si ha già familiarità con Autopilot, rivedere le informazioni contenute in questi articoli:</span><span class="sxs-lookup"><span data-stu-id="c1469-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="c1469-117">Panoramica di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1469-117">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="c1469-118">Guida di riferimento per la distribuzione di Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1469-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="c1469-119">Panoramica</span><span class="sxs-lookup"><span data-stu-id="c1469-119">Overview</span></span>

<span data-ttu-id="c1469-120">Con la funzionalità Windows Autopilot in centro per i partner, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti.</span><span class="sxs-lookup"><span data-stu-id="c1469-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="c1469-121">Al momento della pubblicazione di questo articolo sono disponibili le impostazioni di profilo seguenti:</span><span class="sxs-lookup"><span data-stu-id="c1469-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="c1469-122">Ignora le impostazioni di privacy.</span><span class="sxs-lookup"><span data-stu-id="c1469-122">Skip privacy settings.</span></span> <span data-ttu-id="c1469-123">Questa impostazione facoltativa del profilo di Autopilot consente alle organizzazioni di non richiedere informazioni sulle impostazioni della privacy durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="c1469-124">Disabilitare la creazione dell'account amministratore locale nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1469-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="c1469-125">Le organizzazioni possono decidere se l'utente che configura il dispositivo deve avere l'accesso come amministratore al termine del processo.</span><span class="sxs-lookup"><span data-stu-id="c1469-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="c1469-126">Configurare automaticamente il dispositivo per l'ufficio o l'Istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="c1469-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="c1469-127">Tutti i dispositivi registrati con Autopilot verranno considerati automaticamente dispositivi aziendali o dell'Istituto di istruzione, pertanto questa domanda non verrà richiesta durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="c1469-128">Ignorare le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM.</span><span class="sxs-lookup"><span data-stu-id="c1469-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="c1469-129">Tutti i dispositivi registrati con Autopilot ignoreranno automaticamente queste pagine durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="c1469-130">Ignora il contratto di licenza con l'utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="c1469-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="c1469-131">A partire da Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina EULA visualizzata durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="c1469-132">Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="c1469-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="c1469-133">Si applicano le limitazioni e le autorizzazioni di gestione dei profili e dei dispositivi seguenti:</span><span class="sxs-lookup"><span data-stu-id="c1469-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="c1469-134">I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti con le relazioni rivenditore, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.</span><span class="sxs-lookup"><span data-stu-id="c1469-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="c1469-135">È possibile gestire i dispositivi esistenti per i clienti aggiunti.</span><span class="sxs-lookup"><span data-stu-id="c1469-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="c1469-136">Non è possibile gestire i dispositivi caricati dal cliente in Microsoft Store for business o nel portale di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c1469-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="c1469-137">Creare e gestire i profili di Autopilot nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="c1469-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="c1469-138">Nel centro per i partner è possibile creare profili di distribuzione di Windows Autopilot e applicarli ai dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c1469-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="c1469-139">Solo gli agenti amministratori possono creare e applicare profili.</span><span class="sxs-lookup"><span data-stu-id="c1469-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="c1469-140">Crea un nuovo profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1469-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="c1469-141">Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente per il quale si sta creando il profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="c1469-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="c1469-142">Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="c1469-142">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c1469-143">In **profili di Windows Autopilot** selezionare **Aggiungi nuovo profilo**.</span><span class="sxs-lookup"><span data-stu-id="c1469-143">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="c1469-144">Immettere il nome e la descrizione del profilo e quindi configurare le impostazioni della configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="c1469-145">Scegliere tra:</span><span class="sxs-lookup"><span data-stu-id="c1469-145">Choose from:</span></span>  

   - <span data-ttu-id="c1469-146">Ignora le impostazioni di privacy nel programma di installazione</span><span class="sxs-lookup"><span data-stu-id="c1469-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="c1469-147">Disabilitare l'account amministratore locale nel programma di installazione</span><span class="sxs-lookup"><span data-stu-id="c1469-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="c1469-148">Ignora automaticamente le pagine nel programma di installazione</span><span class="sxs-lookup"><span data-stu-id="c1469-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="c1469-149">(Include *automaticamente seleziona configurazione per lavoro o scuola* e *Ignora le pagine di configurazione per la registrazione di Cortana, OneDrive e OEM*)</span><span class="sxs-lookup"><span data-stu-id="c1469-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="c1469-150">Ignora il contratto di licenza con l'utente finale (EULA)</span><span class="sxs-lookup"><span data-stu-id="c1469-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="c1469-151">Per informazioni importanti su come ignorare la pagina di EULA durante l'installazione di Windows, vedere la pagina relativa al [contratto di licenza di Windows Autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="c1469-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="c1469-152">Al termine, selezionare **Invia** .</span><span class="sxs-lookup"><span data-stu-id="c1469-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="c1469-153">Applicare un profilo di Autopilot ai dispositivi dei clienti</span><span class="sxs-lookup"><span data-stu-id="c1469-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="c1469-154">Le istruzioni seguenti presuppongono che siano già stati aggiunti i dispositivi del cliente al centro per i partner e che sia possibile accedere all'elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c1469-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="c1469-155">Se non sono stati ancora aggiunti i dispositivi del cliente, seguire le istruzioni riportate in [aggiungere dispositivi a un account del cliente](#add-devices-to-a-customers-account) e quindi seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="c1469-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="c1469-156">Dopo aver creato un profilo di Autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="c1469-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="c1469-157">Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="c1469-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="c1469-158">Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="c1469-158">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c1469-159">In **applica profili ai dispositivi** selezionare i dispositivi o i gruppi di dispositivi a cui si vogliono aggiungere i profili e quindi selezionare **Applica profilo**.</span><span class="sxs-lookup"><span data-stu-id="c1469-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="c1469-160">Il profilo appena applicato viene visualizzato nella colonna **profilo** .</span><span class="sxs-lookup"><span data-stu-id="c1469-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="c1469-161">Attenersi alla procedura seguente per verificare che il profilo venga applicato correttamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1469-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="c1469-162">a.</span><span class="sxs-lookup"><span data-stu-id="c1469-162">a.</span></span>  <span data-ttu-id="c1469-163">Connettere un dispositivo alla rete e attivarlo.</span><span class="sxs-lookup"><span data-stu-id="c1469-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="c1469-164">b.</span><span class="sxs-lookup"><span data-stu-id="c1469-164">b.</span></span>  <span data-ttu-id="c1469-165">Verificare che vengano visualizzate le schermate OOBE appropriate, se presenti.</span><span class="sxs-lookup"><span data-stu-id="c1469-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="c1469-166">c.</span><span class="sxs-lookup"><span data-stu-id="c1469-166">c.</span></span>  <span data-ttu-id="c1469-167">Quando il processo OOBE si interrompe, ripristinare le impostazioni predefinite del dispositivo per prepararlo per un nuovo utente.</span><span class="sxs-lookup"><span data-stu-id="c1469-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="c1469-168">Rimuovere un profilo di Autopilot dal dispositivo di un cliente</span><span class="sxs-lookup"><span data-stu-id="c1469-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="c1469-169">Selezionare **Customers** dal menu centro partner e quindi selezionare il cliente per cui è stato creato il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="c1469-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="c1469-170">Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="c1469-170">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c1469-171">In **applica profili ai dispositivi** selezionare i dispositivi da cui si desidera rimuovere il profilo, quindi selezionare **Rimuovi profilo**.</span><span class="sxs-lookup"><span data-stu-id="c1469-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="c1469-172">La rimozione di un profilo da un dispositivo non comporta l'eliminazione del profilo dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c1469-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="c1469-173">Per eliminare un profilo, seguire le istruzioni riportate in [aggiornare o eliminare un profilo di Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="c1469-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="c1469-174">Aggiornare o eliminare un profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1469-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="c1469-175">Se un cliente vuole modificare l'esperienza predefinita dopo aver spedito i dispositivi, è possibile modificare il profilo nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1469-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="c1469-176">Quando il dispositivo del cliente si connette a Internet, verrà scaricata la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="c1469-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="c1469-177">Inoltre, ogni volta che un cliente Ripristina le impostazioni predefinite di un dispositivo, il dispositivo Scarica di nuovo la versione più recente del profilo durante il processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="c1469-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="c1469-178">Selezionare **Customers** dal menu centro per i partner e quindi selezionare il cliente che desidera modificare un profilo di Autopilot.</span><span class="sxs-lookup"><span data-stu-id="c1469-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="c1469-179">Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="c1469-179">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c1469-180">In **profili di Windows Autopilot** selezionare il profilo che si desidera aggiornare.</span><span class="sxs-lookup"><span data-stu-id="c1469-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="c1469-181">Apportare le modifiche necessarie e quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="c1469-181">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="c1469-182">Per eliminare questo profilo, selezionare **Elimina profilo** nell'angolo superiore destro della pagina.</span><span class="sxs-lookup"><span data-stu-id="c1469-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="c1469-183">Aggiungere dispositivi all'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="c1469-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="c1469-184">Gli agenti di vendita e gli agenti di amministrazione possono aggiungere dispositivi a un account del cliente.</span><span class="sxs-lookup"><span data-stu-id="c1469-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="c1469-185">Prima di poter applicare profili Autopilot personalizzati ai dispositivi dei clienti, è necessario essere in grado di accedere all'elenco di dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="c1469-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="c1469-186">Se si prevede di utilizzare il nome OEM, il numero di serie e la combinazione di modelli, tenere presente queste limitazioni:</span><span class="sxs-lookup"><span data-stu-id="c1469-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="c1469-187">Questa tupla funziona solo per i dispositivi più recenti (ad esempio, gli hash 4K) e non è supportata per gli hash 128B (RS2 e i dispositivi precedenti).</span><span class="sxs-lookup"><span data-stu-id="c1469-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="c1469-188">Per la registrazione della tupla viene fatta distinzione tra maiuscole e minuscole, pertanto i dati nel file devono corrispondere ai nomi del modello e del produttore ***esattamente*** come fornito dal provider OEM (provider hardware).</span><span class="sxs-lookup"><span data-stu-id="c1469-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="c1469-189">Seguire le istruzioni riportate di seguito per aggiungere i dispositivi all'account di un cliente nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1469-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="c1469-190">Selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente di cui si vogliono gestire i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c1469-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="c1469-191">Nella pagina dei dettagli del cliente selezionare **Devices (dispositivi**).</span><span class="sxs-lookup"><span data-stu-id="c1469-191">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="c1469-192">In **applica profili ai dispositivi** selezionare **Aggiungi dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="c1469-192">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="c1469-193">Immettere un nome per l'elenco dei dispositivi e quindi selezionare **Sfoglia** per caricare l'elenco del cliente (in formato file CSV) nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1469-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c1469-194">Il file con estensione CSV è stato ricevuto con l'acquisto del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1469-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="c1469-195">Se non si riceve un file con estensione CSV, è possibile crearne uno seguendo i passaggi descritti in [aggiunta di dispositivi a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="c1469-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="c1469-196">Caricare il file con estensione CSV e quindi selezionare **Save (Salva**).</span><span class="sxs-lookup"><span data-stu-id="c1469-196">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="c1469-197">Se viene ricevuto un messaggio di errore durante il tentativo di caricare il file CSV, controllare il formato del file.</span><span class="sxs-lookup"><span data-stu-id="c1469-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="c1469-198">È possibile utilizzare solo l'hash hardware oppure il nome OEM, il numero di serie e il modello (nell'ordine di tale colonna) o l'ID del prodotto Windows.</span><span class="sxs-lookup"><span data-stu-id="c1469-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="c1469-199">È anche possibile usare il file CSV di esempio fornito dal collegamento accanto a **Aggiungi dispositivi** per creare un elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="c1469-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="c1469-200">Il file CSV avrà un aspetto simile al seguente:</span><span class="sxs-lookup"><span data-stu-id="c1469-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="c1469-201">**Numero di serie del dispositivo, ID prodotto Windows, hash hardware, nome produttore, modello di dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c1469-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="c1469-202">**{serialNumber},,, Microsoft Corporation, Surface laptop**</span><span class="sxs-lookup"><span data-stu-id="c1469-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="c1469-203">"Nome produttore" e "modello di dispositivo" fanno distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="c1469-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="c1469-204">Se non si conosce il valore da inserire per il nome del produttore e il modello di dispositivo, è possibile eseguire questa operazione sul dispositivo per raccogliere i valori corretti:</span><span class="sxs-lookup"><span data-stu-id="c1469-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="c1469-205">Dismissing EULA di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="c1469-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="c1469-206">INFORMAZIONI IMPORTANTI</span><span class="sxs-lookup"><span data-stu-id="c1469-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="c1469-207">Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti.</span><span class="sxs-lookup"><span data-stu-id="c1469-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="c1469-208">Se il cliente è autorizzato a eseguire questa operazione, è possibile disattivare o nascondere alcune schermate di configurazione che in genere vengono presentate agli utenti durante la configurazione di Windows, inclusa la schermata di accettazione del contratto di licenza con l'utente finale (EULA).</span><span class="sxs-lookup"><span data-stu-id="c1469-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="c1469-209">Utilizzando questa funzione, l'utente accetta che l'eliminazione o la disattivazione di schermate progettate per fornire agli utenti la comunicazione o l'accettazione delle condizioni significa che il Licenziatario ha ottenuto il consenso e l'autorizzazione sufficienti per nascondere i termini e che l'utente, per conto del cliente (indipendentemente dal fatto che sia un'organizzazione o un singolo utente come il caso), acconsente a qualsiasi comunicazione e accetti le condizioni applicabili</span><span class="sxs-lookup"><span data-stu-id="c1469-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="c1469-210">Questo include il contratto con i termini e le condizioni della licenza o l'avviso che verrebbe presentato all'utente se non è stato eliminato o nascosto utilizzando questo strumento.</span><span class="sxs-lookup"><span data-stu-id="c1469-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="c1469-211">Il cliente non potrà utilizzare il software Windows su tali dispositivi se il cliente non ha acquistato in maniera valida una licenza per il software da Microsoft o dai suoi distributori autorizzati.</span><span class="sxs-lookup"><span data-stu-id="c1469-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
