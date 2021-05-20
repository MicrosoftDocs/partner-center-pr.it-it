---
title: Personalizzare l'esperienza di un dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Prima di distribuire il nuovo dispositivo di un cliente, è possibile usare i profili Windows Autopilot per personalizzare o pre-configurare l'esperienza predefinita del dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149826"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="34a28-103">Usare i profili di Windows Autopilot nei nuovi dispositivi per personalizzare l'esperienza predefinita di un cliente</span><span class="sxs-lookup"><span data-stu-id="34a28-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="34a28-104">**Ruoli appropriati:** amministrazione dell'agente | Amministratore globale | Agente di vendita | Amministratore di gestione utenti</span><span class="sxs-lookup"><span data-stu-id="34a28-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="34a28-105">Se si gestiscono i dispositivi dei clienti, potrebbe essere necessario personalizzare l'esperienza predefinita (OOBE) per gli utenti del cliente.</span><span class="sxs-lookup"><span data-stu-id="34a28-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="34a28-106">È possibile pre-configurare nuovi dispositivi con Windows Autopilot prima di recapitare i dispositivi ai clienti e applicare nuovi profili ai dispositivi che i clienti hanno già acquistato.</span><span class="sxs-lookup"><span data-stu-id="34a28-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="34a28-107">Si noti che gli OEM hanno iniziato a includere un'etichetta di spedizione all'esterno della casella del dispositivo Autopilot che mostra l'ID del codice **Product Key (PKID) del dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="34a28-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="34a28-108">Questo codice a barre leggibile unidimensionale offre ai partner downstream un modo per registrare i dispositivi per Autopilot senza dover disappiare i dispositivi e raccogliere l'ID dispositivo con mezzi alternativi.</span><span class="sxs-lookup"><span data-stu-id="34a28-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="34a28-109">Questo articolo illustra come creare e applicare profili Autopilot ai dispositivi in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34a28-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="34a28-110">Se non si ha già familiarità con Autopilot, vedere le informazioni in questi articoli:</span><span class="sxs-lookup"><span data-stu-id="34a28-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="34a28-111">Panoramica di Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="34a28-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="34a28-112">Guida di riferimento alla distribuzione di Autopilot</span><span class="sxs-lookup"><span data-stu-id="34a28-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="34a28-113">Panoramica</span><span class="sxs-lookup"><span data-stu-id="34a28-113">Overview</span></span>

<span data-ttu-id="34a28-114">Con la Windows Autopilot funzionalità in Partner Center, è possibile creare profili personalizzati da applicare ai dispositivi dei clienti.</span><span class="sxs-lookup"><span data-stu-id="34a28-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="34a28-115">Al momento della pubblicazione di questo articolo erano disponibili le impostazioni del profilo seguenti:</span><span class="sxs-lookup"><span data-stu-id="34a28-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="34a28-116">Ignorare le impostazioni di privacy.</span><span class="sxs-lookup"><span data-stu-id="34a28-116">Skip privacy settings.</span></span> <span data-ttu-id="34a28-117">Questa impostazione del profilo Autopilot facoltativa consente alle organizzazioni di non chiedere informazioni sulle impostazioni di privacy durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="34a28-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="34a28-118">Disabilitare la creazione dell'account amministratore locale nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34a28-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="34a28-119">Le organizzazioni possono decidere se l'utente che configura il dispositivo deve avere accesso come amministratore al termine del processo.</span><span class="sxs-lookup"><span data-stu-id="34a28-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="34a28-120">Configurare automaticamente il dispositivo per l'istituto di istruzione o l'istituto di istruzione.</span><span class="sxs-lookup"><span data-stu-id="34a28-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="34a28-121">Tutti i dispositivi registrati con Autopilot verranno automaticamente considerati dispositivi aziendali o dell'istituto di istruzione, quindi questa domanda non verrà posta durante il processo di configurazione.</span><span class="sxs-lookup"><span data-stu-id="34a28-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="34a28-122">Ignorare le pagine di configurazione della registrazione di Cortana, OneDrive e OEM.</span><span class="sxs-lookup"><span data-stu-id="34a28-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="34a28-123">Tutti i dispositivi registrati con Autopilot ignorano automaticamente queste pagine durante il processo di configurazione della configurazione automatica.</span><span class="sxs-lookup"><span data-stu-id="34a28-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="34a28-124">Ignorare il Contratto di licenza con l'utente finale .</span><span class="sxs-lookup"><span data-stu-id="34a28-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="34a28-125">A partire Windows 10 versione 1709, le organizzazioni possono decidere di ignorare la pagina EULA presentata durante il processo di configurazione.</span><span class="sxs-lookup"><span data-stu-id="34a28-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="34a28-126">Per informazioni importanti su come ignorare la pagina [EULA durante](#windows-autopilot-eula-dismissal) l'installazione di Windows, vedere Windows Autopilot chiusura dell'EULA di seguito.</span><span class="sxs-lookup"><span data-stu-id="34a28-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="34a28-127">Si applicano le limitazioni e le autorizzazioni seguenti di gestione dei profili e dei dispositivi:</span><span class="sxs-lookup"><span data-stu-id="34a28-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="34a28-128">I partner CSP possono continuare a gestire i profili di Autopilot per i clienti esistenti di cui sono rivenditori, anche se i clienti hanno rimosso i privilegi di amministrazione delegata del partner.</span><span class="sxs-lookup"><span data-stu-id="34a28-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="34a28-129">È possibile gestire i dispositivi esistenti per i clienti aggiunti.</span><span class="sxs-lookup"><span data-stu-id="34a28-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="34a28-130">Non è possibile gestire i dispositivi caricati dal cliente in Microsoft Store per le aziende o nel portale di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="34a28-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="34a28-131">Creare e gestire profili Autopilot in Partner Center</span><span class="sxs-lookup"><span data-stu-id="34a28-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="34a28-132">In Partner Center, è possibile creare Windows Autopilot di distribuzione e applicarli ai dispositivi.</span><span class="sxs-lookup"><span data-stu-id="34a28-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="34a28-133">Solo gli agenti amministratore possono creare e applicare profili.</span><span class="sxs-lookup"><span data-stu-id="34a28-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="34a28-134">Creare un nuovo profilo Autopilot</span><span class="sxs-lookup"><span data-stu-id="34a28-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="34a28-135">Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui si sta creando il profilo Autopilot.</span><span class="sxs-lookup"><span data-stu-id="34a28-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="34a28-136">Nella pagina dei dettagli del cliente selezionare **Dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="34a28-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="34a28-137">In **Windows Autopilot profili selezionare** Aggiungi nuovo **profilo**.</span><span class="sxs-lookup"><span data-stu-id="34a28-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="34a28-138">Immettere il nome e la descrizione del profilo e quindi configurare le impostazioni di Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="34a28-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="34a28-139">Scegliere tra:</span><span class="sxs-lookup"><span data-stu-id="34a28-139">Choose from:</span></span>  

   - <span data-ttu-id="34a28-140">Ignorare le impostazioni di privacy nella configurazione</span><span class="sxs-lookup"><span data-stu-id="34a28-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="34a28-141">Disabilitare l'account amministratore locale durante l'installazione</span><span class="sxs-lookup"><span data-stu-id="34a28-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="34a28-142">Ignorare automaticamente le pagine nella configurazione</span><span class="sxs-lookup"><span data-stu-id="34a28-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="34a28-143">(Include *la selezione automatica della configurazione per l'ambiente di lavoro o dell'istituto di* istruzione e ignora le pagine di configurazione della registrazione di *Cortana, OneDrive e OEM)*</span><span class="sxs-lookup"><span data-stu-id="34a28-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="34a28-144">Ignorare il contratto di licenza con l'utente finale (EULA)</span><span class="sxs-lookup"><span data-stu-id="34a28-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="34a28-145">Per informazioni importanti su come ignorare la pagina [EULA durante](#windows-autopilot-eula-dismissal) l'installazione di Windows, vedere Windows Autopilot chiusura dell'EULA di seguito.</span><span class="sxs-lookup"><span data-stu-id="34a28-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="34a28-146">Al **termine, selezionare** Invia.</span><span class="sxs-lookup"><span data-stu-id="34a28-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="34a28-147">Applicare un profilo Autopilot ai dispositivi dei clienti</span><span class="sxs-lookup"><span data-stu-id="34a28-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="34a28-148">Le istruzioni seguenti presuppongono che i dispositivi del cliente siano già stati aggiunti a Partner Center e che sia possibile accedere al relativo elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="34a28-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="34a28-149">Se i dispositivi del cliente non sono ancora stati aggiunti, seguire le istruzioni riportate in Aggiungere dispositivi [all'account](#add-devices-to-a-customers-account) di un cliente e quindi seguire questa procedura.</span><span class="sxs-lookup"><span data-stu-id="34a28-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="34a28-150">Dopo aver creato un profilo autopilot per un cliente, è possibile applicarlo ai dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="34a28-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="34a28-151">Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui è stato creato il profilo autopilot.</span><span class="sxs-lookup"><span data-stu-id="34a28-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="34a28-152">Nella pagina dei dettagli del cliente selezionare **Dispositivi.**</span><span class="sxs-lookup"><span data-stu-id="34a28-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="34a28-153">In **Applica profili ai dispositivi** selezionare i dispositivi o i gruppi di dispositivi a cui si vogliono aggiungere profili e quindi selezionare Applica **profilo.**</span><span class="sxs-lookup"><span data-stu-id="34a28-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="34a28-154">Il profilo appena applicato viene visualizzato nella **colonna** Profilo.</span><span class="sxs-lookup"><span data-stu-id="34a28-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="34a28-155">Seguire questa procedura per verificare che il profilo verrà applicato correttamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34a28-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="34a28-156">a.</span><span class="sxs-lookup"><span data-stu-id="34a28-156">a.</span></span>  <span data-ttu-id="34a28-157">Connettere un dispositivo alla rete e attivarlo.</span><span class="sxs-lookup"><span data-stu-id="34a28-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="34a28-158">b.</span><span class="sxs-lookup"><span data-stu-id="34a28-158">b.</span></span>  <span data-ttu-id="34a28-159">Verificare che vengano visualizzate le eventuali schermate appropriate della Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="34a28-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="34a28-160">c.</span><span class="sxs-lookup"><span data-stu-id="34a28-160">c.</span></span>  <span data-ttu-id="34a28-161">Quando il processo di Configurazione guidata si arresta, ripristinare le impostazioni predefinite del dispositivo per prepararlo per un nuovo utente.</span><span class="sxs-lookup"><span data-stu-id="34a28-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="34a28-162">Rimuovere un profilo di Autopilot dal dispositivo di un cliente</span><span class="sxs-lookup"><span data-stu-id="34a28-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="34a28-163">Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente per cui è stato creato il profilo autopilot.</span><span class="sxs-lookup"><span data-stu-id="34a28-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="34a28-164">Nella pagina dei dettagli del cliente selezionare **Dispositivi.**</span><span class="sxs-lookup"><span data-stu-id="34a28-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="34a28-165">In **Applica profili ai dispositivi** selezionare i dispositivi da cui si vuole rimuovere il profilo e quindi selezionare Rimuovi **profilo.**</span><span class="sxs-lookup"><span data-stu-id="34a28-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="34a28-166">La rimozione di un profilo da un dispositivo non elimina il profilo dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="34a28-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="34a28-167">Se si vuole eliminare un profilo, seguire le istruzioni in [Aggiornare o eliminare un profilo di Autopilot.](#update-or-delete-an-autopilot-profile)</span><span class="sxs-lookup"><span data-stu-id="34a28-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="34a28-168">Aggiornare o eliminare un profilo di Autopilot</span><span class="sxs-lookup"><span data-stu-id="34a28-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="34a28-169">Se un cliente vuole modificare l'esperienza predefinita dopo aver inviato i dispositivi, è possibile modificare il profilo in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34a28-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="34a28-170">Quando il dispositivo del cliente si connette a Internet, scarica la versione più recente del profilo durante il processo di Configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="34a28-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="34a28-171">Inoltre, ogni volta che un cliente ripristina le impostazioni predefinite predefinite di un dispositivo, il dispositivo scaricherà di nuovo la versione più recente del profilo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="34a28-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="34a28-172">Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente che vuole modificare un profilo autopilot.</span><span class="sxs-lookup"><span data-stu-id="34a28-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="34a28-173">Nella pagina dei dettagli del cliente selezionare **Dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="34a28-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="34a28-174">In **Windows Autopilot profili** selezionare il profilo da aggiornare.</span><span class="sxs-lookup"><span data-stu-id="34a28-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="34a28-175">Apportare le modifiche necessarie e quindi selezionare **Invia**.</span><span class="sxs-lookup"><span data-stu-id="34a28-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="34a28-176">Per eliminare questo profilo, selezionare **Elimina profilo** nell'angolo superiore destro della pagina.</span><span class="sxs-lookup"><span data-stu-id="34a28-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="34a28-177">Aggiungere dispositivi all'account di un cliente</span><span class="sxs-lookup"><span data-stu-id="34a28-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="34a28-178">Gli agenti di vendita e gli agenti di amministrazione possono aggiungere dispositivi all'account di un cliente.</span><span class="sxs-lookup"><span data-stu-id="34a28-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="34a28-179">Prima di poter applicare profili Autopilot personalizzati ai dispositivi dei clienti, è necessario poter accedere all'elenco dei dispositivi del cliente.</span><span class="sxs-lookup"><span data-stu-id="34a28-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="34a28-180">Se si prevede di usare la combinazione di nome, numero di serie e modello OEM, tenere presenti queste limitazioni:</span><span class="sxs-lookup"><span data-stu-id="34a28-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="34a28-181">Questa tupla funziona solo per i dispositivi più nuovi (hash 4k, ad esempio) e non è supportata per gli hash da 128b (RS2 e dispositivi precedenti).</span><span class="sxs-lookup"><span data-stu-id="34a28-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="34a28-182">La registrazione della tupla fa distinzione tra maiuscole e  minuscole, quindi i dati nel file devono corrispondere ai nomi del modello e del produttore esattamente come fornito dal provider OEM (provider hardware).</span><span class="sxs-lookup"><span data-stu-id="34a28-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="34a28-183">Seguire le istruzioni seguenti per aggiungere dispositivi all'account di un cliente in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="34a28-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="34a28-184">Selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente di cui si vuole gestire i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="34a28-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="34a28-185">Nella pagina dei dettagli del cliente selezionare **Dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="34a28-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="34a28-186">In **Applica profili ai dispositivi** selezionare Aggiungi **dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="34a28-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="34a28-187">Immettere un nome per l'elenco di dispositivi e quindi selezionare Sfoglia per caricare l'elenco del cliente (in formato di file CSV) in Partner Center. </span><span class="sxs-lookup"><span data-stu-id="34a28-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="34a28-188">Questo file CSV dovrebbe essere stato ricevuto con l'acquisto del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34a28-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="34a28-189">Se non si riceve un file CSV, è possibile crearne uno manualmente seguendo la procedura [descritta](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)in Aggiunta di dispositivi a Windows Autopilot .</span><span class="sxs-lookup"><span data-stu-id="34a28-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="34a28-190">Caricare il file CSV e quindi selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="34a28-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="34a28-191">Se si riceve un messaggio di errore mentre si tenta di caricare il file CSV, controllare il formato del file.</span><span class="sxs-lookup"><span data-stu-id="34a28-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="34a28-192">È possibile usare solo l'hash hardware oppure il nome OEM, il numero di serie e il modello (nell'ordine di tale colonna) o l'ID del prodotto Windows.</span><span class="sxs-lookup"><span data-stu-id="34a28-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="34a28-193">È anche possibile usare il file CSV di esempio fornito dal collegamento accanto ad **Aggiungi dispositivi** per creare un elenco di dispositivi.</span><span class="sxs-lookup"><span data-stu-id="34a28-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="34a28-194">Il file CSV dovrebbe essere simile al seguente:</span><span class="sxs-lookup"><span data-stu-id="34a28-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="34a28-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span><span class="sxs-lookup"><span data-stu-id="34a28-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="34a28-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="34a28-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="34a28-197">Per "Nome produttore" e "Modello di dispositivo" viene fatto distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="34a28-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="34a28-198">Se non si conosce il valore da inserire per Nome produttore e Modello di dispositivo, è possibile eseguire questa operazione nel dispositivo per raccogliere i valori corretti:</span><span class="sxs-lookup"><span data-stu-id="34a28-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="34a28-199">Windows Autopilot EULA dismissal</span><span class="sxs-lookup"><span data-stu-id="34a28-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="34a28-200">INFORMAZIONI IMPORTANTI</span><span class="sxs-lookup"><span data-stu-id="34a28-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="34a28-201">Windows Autopilot consente di configurare installazioni personalizzate di Windows nei dispositivi gestiti per i clienti.</span><span class="sxs-lookup"><span data-stu-id="34a28-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="34a28-202">Se autorizzato dal cliente, è possibile eliminare o nascondere determinate schermate di configurazione che vengono normalmente presentate agli utenti durante la configurazione di Windows, inclusa la schermata di accettazione del contratto di licenza con l'utente finale.</span><span class="sxs-lookup"><span data-stu-id="34a28-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="34a28-203">Usando questa funzione, l'utente accetta di eliminare o nascondere eventuali schermate progettate per fornire agli utenti la comunicazione o l'accettazione delle condizioni significa che il cliente ha ottenuto un consenso e un'autorizzazione sufficienti per nascondere le condizioni e che, per conto del cliente (che possa trattarsi di un'organizzazione o di un singolo utente), acconsentire a eventuali comunicazioni e accettare le condizioni applicabili al cliente.</span><span class="sxs-lookup"><span data-stu-id="34a28-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="34a28-204">Ciò include il contratto ai termini e alle condizioni della licenza o all'avviso che verrebbe presentato all'utente se non fosse stato eliminato o nascosto con questo strumento.</span><span class="sxs-lookup"><span data-stu-id="34a28-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="34a28-205">Il cliente non può usare il software Windows su tali dispositivi se il cliente non ha acquistato in modo valido una licenza per il software da Microsoft o dai suoi distributori con licenza.</span><span class="sxs-lookup"><span data-stu-id="34a28-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>