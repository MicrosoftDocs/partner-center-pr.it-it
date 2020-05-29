---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Dynamics 365 CRM
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 87b1d27fa2f42eeba3b0f8308648536c0686911e
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145135"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="95945-103">Co-selling Connector per Dynamics 365 CRM-Panoramica</span><span class="sxs-lookup"><span data-stu-id="95945-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="95945-104">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="95945-104">Appropriate roles</span></span>

- <span data-ttu-id="95945-105">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="95945-105">Referrals admin</span></span>
- <span data-ttu-id="95945-106">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="95945-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="95945-107">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="95945-108">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="95945-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="95945-109">Usare i connettori di co-selling, per creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare/rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="95945-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="95945-110">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="95945-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="95945-111">È possibile eseguire tutti i riferimenti all'interno del CRM scelto, anziché nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="95945-112">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="95945-113">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="95945-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="95945-114">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="95945-114">**Topics**</span></span>   |<span data-ttu-id="95945-115">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="95945-115">**Details**</span></span>   |<span data-ttu-id="95945-116">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="95945-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="95945-117">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="95945-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="95945-118">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="95945-118">You need a valid MPN ID</span></span>|<span data-ttu-id="95945-119">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="95945-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="95945-120">Coselling pronto</span><span class="sxs-lookup"><span data-stu-id="95945-120">Cosell ready</span></span>|<span data-ttu-id="95945-121">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="95945-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="95945-122">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="95945-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="95945-123">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="95945-123">Partner Center account</span></span>|<span data-ttu-id="95945-124">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="95945-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="95945-125">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="95945-126">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="95945-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="95945-127">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="95945-127">Partner Center user roles</span></span>|<span data-ttu-id="95945-128">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="95945-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="95945-129">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="95945-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="95945-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="95945-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="95945-131">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="95945-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="95945-132">Assegnare i ruoli in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="95945-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="95945-133">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="95945-133">Power Automate Flow Account</span></span>|<span data-ttu-id="95945-134">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="95945-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="95945-135">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="95945-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="95945-136">Installare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 (soluzione Power automatici)</span><span class="sxs-lookup"><span data-stu-id="95945-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="95945-137">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="95945-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="95945-138">In questo passaggio vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="95945-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="95945-139">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="95945-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="95945-140">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="95945-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="95945-141">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="95945-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Apri AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="95945-143">Cercare i **connettori dei riferimenti del centro per i partner per Dynamics 365** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="95945-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="95945-144">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="95945-144">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="95945-145">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="95945-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="95945-146">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="95945-146">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="95945-147">Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="95945-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="95945-148">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="95945-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="95945-149">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="95945-150">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="95945-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="95945-151">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="95945-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="95945-152">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Dynamics 365** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="95945-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="95945-153">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="95945-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="95945-154">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="95945-154">The following Power Automate flows and entities are available:</span></span>

![DISPONGONO disponibili](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="95945-156">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="95945-156">Best practice: test before you go live</span></span>

<span data-ttu-id="95945-157">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="95945-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="95945-158">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="95945-159">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="95945-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="95945-160">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="95945-161">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="95945-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="95945-162">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="95945-162">Configure the solution</span></span>

1. <span data-ttu-id="95945-163">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="95945-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="95945-164">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="95945-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="95945-165">È necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="95945-165">You'll need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="95945-166">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="95945-166">Partner Center user with referrals admin credentials</span></span> 

- <span data-ttu-id="95945-167">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="95945-167">Partner Center Events</span></span>

- <span data-ttu-id="95945-168">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="95945-168">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="95945-169">a.</span><span class="sxs-lookup"><span data-stu-id="95945-169">a.</span></span> <span data-ttu-id="95945-170">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="95945-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="95945-171">b.</span><span class="sxs-lookup"><span data-stu-id="95945-171">b.</span></span> <span data-ttu-id="95945-172">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="95945-172">Create a connection by clicking **Create a connection**.</span></span>

    ![Creare la connessione](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="95945-174">c.</span><span class="sxs-lookup"><span data-stu-id="95945-174">c.</span></span> <span data-ttu-id="95945-175">Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="95945-175">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

    <span data-ttu-id="95945-176">d.</span><span class="sxs-lookup"><span data-stu-id="95945-176">d.</span></span> <span data-ttu-id="95945-177">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="95945-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="95945-178">e.</span><span class="sxs-lookup"><span data-stu-id="95945-178">e.</span></span> <span data-ttu-id="95945-179">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="95945-179">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

    <span data-ttu-id="95945-180">f.</span><span class="sxs-lookup"><span data-stu-id="95945-180">f.</span></span> <span data-ttu-id="95945-181">Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-181">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="95945-182">Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-182">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="95945-183">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="95945-183">Save the changes.</span></span>

5. <span data-ttu-id="95945-184">**Attivare** i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-184">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="95945-185">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="95945-185">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="95945-186">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="95945-186">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="95945-187">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="95945-187">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="95945-188">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="95945-188">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="95945-189">Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito</span><span class="sxs-lookup"><span data-stu-id="95945-189">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Trigger](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="95945-191">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="95945-191">When you make these updates, you'll see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="95945-193">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="95945-193">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="95945-194">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="95945-194">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="95945-195">Selezionare **centro per i partner per Dynamics 365 (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="95945-195">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="95945-196">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="95945-196">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="95945-197">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="95945-197">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copia l'URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="95945-199">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="95945-199">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="95945-200">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="95945-200">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="95945-201">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="95945-201">Enter the following details:</span></span> 

    <span data-ttu-id="95945-202">a.</span><span class="sxs-lookup"><span data-stu-id="95945-202">a.</span></span> <span data-ttu-id="95945-203">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="95945-203">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="95945-204">b.</span><span class="sxs-lookup"><span data-stu-id="95945-204">b.</span></span> <span data-ttu-id="95945-205">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="95945-205">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="95945-206">c.</span><span class="sxs-lookup"><span data-stu-id="95945-206">c.</span></span> <span data-ttu-id="95945-207">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="95945-207">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="95945-208">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="95945-208">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="95945-209">Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.</span><span class="sxs-lookup"><span data-stu-id="95945-209">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="95945-210">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="95945-210">Customize synchronization steps</span></span>

<span data-ttu-id="95945-211">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="95945-211">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="95945-212">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="95945-212">Often CRM systems are highly customized.</span></span> <span data-ttu-id="95945-213">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-213">You can customize the Power Automate flows.</span></span> <span data-ttu-id="95945-214">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-214">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="95945-215">Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="95945-215">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="95945-216">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="95945-216">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="95945-217">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="95945-217">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="95945-218">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="95945-218">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="95945-219">a.</span><span class="sxs-lookup"><span data-stu-id="95945-219">a.</span></span> <span data-ttu-id="95945-220">Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="95945-220">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="95945-221">b.</span><span class="sxs-lookup"><span data-stu-id="95945-221">b.</span></span> <span data-ttu-id="95945-222">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-222">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="95945-223">c.</span><span class="sxs-lookup"><span data-stu-id="95945-223">c.</span></span> <span data-ttu-id="95945-224">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="95945-224">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="95945-225">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="95945-225">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="95945-226">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="95945-226">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="95945-227">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="95945-227">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="95945-228">d.</span><span class="sxs-lookup"><span data-stu-id="95945-228">d.</span></span> <span data-ttu-id="95945-229">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="95945-229">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="95945-230">e.</span><span class="sxs-lookup"><span data-stu-id="95945-230">e.</span></span> <span data-ttu-id="95945-231">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="95945-231">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="95945-232">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="95945-232">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="95945-233">f.</span><span class="sxs-lookup"><span data-stu-id="95945-233">f.</span></span> <span data-ttu-id="95945-234">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="95945-234">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="95945-235">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="95945-235">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="95945-236">a.</span><span class="sxs-lookup"><span data-stu-id="95945-236">a.</span></span> <span data-ttu-id="95945-237">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-237">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="95945-238">b.</span><span class="sxs-lookup"><span data-stu-id="95945-238">b.</span></span> <span data-ttu-id="95945-239">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="95945-239">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="95945-240">c.</span><span class="sxs-lookup"><span data-stu-id="95945-240">c.</span></span> <span data-ttu-id="95945-241">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare **se c'è differenza tra gli oggetti lead in Partner Center e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="95945-241">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="95945-242">d.</span><span class="sxs-lookup"><span data-stu-id="95945-242">d.</span></span> <span data-ttu-id="95945-243">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="95945-243">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="95945-244">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="95945-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="95945-245">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="95945-245">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="95945-246">a.</span><span class="sxs-lookup"><span data-stu-id="95945-246">a.</span></span> <span data-ttu-id="95945-247">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="95945-247">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="95945-248">b.</span><span class="sxs-lookup"><span data-stu-id="95945-248">b.</span></span> <span data-ttu-id="95945-249">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="95945-249">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="95945-250">c.</span><span class="sxs-lookup"><span data-stu-id="95945-250">c.</span></span> <span data-ttu-id="95945-251">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="95945-251">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="95945-252">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="95945-252">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="95945-253">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="95945-253">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="95945-254">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 e centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-254">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="95945-255">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="95945-255">Pre-requisites</span></span>

<span data-ttu-id="95945-256">Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM, la soluzione Power automatizzate delimita chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="95945-256">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="95945-257">Questa identificazione consente ai team dei venditori di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="95945-257">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="95945-258">Un set di campi personalizzati è disponibile come parte dell'entità **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="95945-258">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="95945-259">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="95945-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="95945-260">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="95945-260">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="95945-261">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="95945-261">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="95945-262">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="95945-262">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="95945-263">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="95945-263">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="95945-264">In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="95945-264">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="95945-265">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="95945-265">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="95945-266">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="95945-266">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="95945-267">SCENARI</span><span class="sxs-lookup"><span data-stu-id="95945-267">SCENARIOS:</span></span>

1. <span data-ttu-id="95945-268">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="95945-268">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="95945-269">a.</span><span class="sxs-lookup"><span data-stu-id="95945-269">a.</span></span> <span data-ttu-id="95945-270">Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-270">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="95945-271">b.</span><span class="sxs-lookup"><span data-stu-id="95945-271">b.</span></span> <span data-ttu-id="95945-272">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="95945-272">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Opportunità](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="95945-274">c.</span><span class="sxs-lookup"><span data-stu-id="95945-274">c.</span></span> <span data-ttu-id="95945-275">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="95945-275">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="95945-276">**Sincronizza con il centro per i partner**: Sì</span><span class="sxs-lookup"><span data-stu-id="95945-276">**Sync with Partner Center**: Yes</span></span>

    - <span data-ttu-id="95945-277">**Come può essere utile Microsoft?**: selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="95945-277">**How can Microsoft help?**: Select from the following:</span></span>

    ![Selezioni della Guida](images/cosellconnectors/help.png)

    - <span data-ttu-id="95945-279">**Prodotti**: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="95945-279">**Products**: Solution IDs of the product</span></span>

    <span data-ttu-id="95945-280">d.</span><span class="sxs-lookup"><span data-stu-id="95945-280">d.</span></span> <span data-ttu-id="95945-281">Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti e quindi accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-281">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="95945-282">I riferimenti verranno sincronizzati con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="95945-282">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="95945-283">e.</span><span class="sxs-lookup"><span data-stu-id="95945-283">e.</span></span> <span data-ttu-id="95945-284">Analogamente, per un'opportunità con l'opzione "Sync with partner Center" impostata su "Yes", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-284">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="95945-285">f.</span><span class="sxs-lookup"><span data-stu-id="95945-285">f.</span></span> <span data-ttu-id="95945-286">Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="95945-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="95945-287">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="95945-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

    <span data-ttu-id="95945-288">a.</span><span class="sxs-lookup"><span data-stu-id="95945-288">a.</span></span> <span data-ttu-id="95945-289">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="95945-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="95945-290">b.</span><span class="sxs-lookup"><span data-stu-id="95945-290">b.</span></span> <span data-ttu-id="95945-291">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="95945-291">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="95945-292">c.</span><span class="sxs-lookup"><span data-stu-id="95945-292">c.</span></span> <span data-ttu-id="95945-293">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="95945-293">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="95945-294">d.</span><span class="sxs-lookup"><span data-stu-id="95945-294">d.</span></span> <span data-ttu-id="95945-295">Accedere al proprio ambiente Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-295">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="95945-296">e.</span><span class="sxs-lookup"><span data-stu-id="95945-296">e.</span></span> <span data-ttu-id="95945-297">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="95945-297">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="95945-298">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="95945-298">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="95945-299">f.</span><span class="sxs-lookup"><span data-stu-id="95945-299">f.</span></span> <span data-ttu-id="95945-300">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="95945-300">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="95945-301">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="95945-301">Next steps</span></span>

- [<span data-ttu-id="95945-302">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="95945-302">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="95945-303">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="95945-303">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="95945-304">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="95945-304">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="95945-305">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="95945-305">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)