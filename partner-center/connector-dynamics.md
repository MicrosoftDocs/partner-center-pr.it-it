---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con il connettore di co-selling per Dynamics 365 CRM. I venditori possono quindi co-vendere con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556362"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="a2619-104">Co-selling Connector per Dynamics 365 CRM-Panoramica</span><span class="sxs-lookup"><span data-stu-id="a2619-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="a2619-105">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="a2619-105">Appropriate roles</span></span>

- <span data-ttu-id="a2619-106">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="a2619-106">Referrals admin</span></span>
- <span data-ttu-id="a2619-107">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="a2619-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="a2619-108">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="a2619-109">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="a2619-110">Usare i connettori di co-selling, per creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare/rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="a2619-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="a2619-111">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="a2619-112">È possibile eseguire tutti i riferimenti all'interno del CRM scelto, anziché nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="a2619-113">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="a2619-114">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="a2619-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="a2619-115">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="a2619-115">**Topics**</span></span>   |<span data-ttu-id="a2619-116">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="a2619-116">**Details**</span></span>   |<span data-ttu-id="a2619-117">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="a2619-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="a2619-118">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="a2619-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="a2619-119">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="a2619-119">You need a valid MPN ID</span></span>|<span data-ttu-id="a2619-120">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="a2619-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="a2619-121">Coselling pronto</span><span class="sxs-lookup"><span data-stu-id="a2619-121">Cosell ready</span></span>|<span data-ttu-id="a2619-122">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="a2619-123">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2619-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="a2619-124">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2619-124">Partner Center account</span></span>|<span data-ttu-id="a2619-125">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="a2619-126">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="a2619-127">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="a2619-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="a2619-128">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2619-128">Partner Center user roles</span></span>|<span data-ttu-id="a2619-129">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="a2619-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="a2619-130">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="a2619-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="a2619-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="a2619-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="a2619-132">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="a2619-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="a2619-133">Assegnare i ruoli in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2619-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="a2619-134">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="a2619-134">Power Automate Flow Account</span></span>|<span data-ttu-id="a2619-135">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="a2619-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="a2619-136">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="a2619-137">Installare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 (soluzione Power automatici)</span><span class="sxs-lookup"><span data-stu-id="a2619-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="a2619-138">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="a2619-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="a2619-139">In questo passaggio vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="a2619-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="a2619-140">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="a2619-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="a2619-141">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="a2619-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="a2619-142">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="a2619-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. <span data-ttu-id="a2619-144">Cercare i **connettori dei riferimenti del centro per i partner per Dynamics 365** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="a2619-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="a2619-145">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="a2619-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="a2619-146">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="a2619-147">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="a2619-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="a2619-148">Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="a2619-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="a2619-149">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="a2619-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="a2619-150">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="a2619-151">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="a2619-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="a2619-152">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="a2619-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="a2619-153">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Dynamics 365** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="a2619-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="a2619-154">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="a2619-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="a2619-155">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="a2619-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="DISPONGONO disponibili":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="a2619-157">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="a2619-157">Best practice: test before you go live</span></span>

<span data-ttu-id="a2619-158">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="a2619-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="a2619-159">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="a2619-160">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="a2619-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="a2619-161">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="a2619-162">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="a2619-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="a2619-163">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="a2619-163">Configure the solution</span></span>

1. <span data-ttu-id="a2619-164">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="a2619-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="a2619-165">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="a2619-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="a2619-166">È necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="a2619-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="a2619-167">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="a2619-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="a2619-168">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2619-168">Partner Center Events</span></span>

   - <span data-ttu-id="a2619-169">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="a2619-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="a2619-170">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="a2619-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="a2619-171">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="a2619-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Creare la connessione":::

      3. <span data-ttu-id="a2619-173">Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="a2619-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="a2619-174">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="a2619-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="a2619-175">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="a2619-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="a2619-176">Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="a2619-177">Una volta aggiunte tutte le connessioni, nell'ambiente verranno visualizzate le connessioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a2619-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Connessioni":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="a2619-179">Modificare le connessioni</span><span class="sxs-lookup"><span data-stu-id="a2619-179">Edit the connections</span></span>

1. <span data-ttu-id="a2619-180">Tornare alla pagina **soluzioni** e selezionare **soluzione predefinita**.</span><span class="sxs-lookup"><span data-stu-id="a2619-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="a2619-181">Selezionare **riferimento alla connessione (anteprima)** facendo clic su **tutto**.</span><span class="sxs-lookup"><span data-stu-id="a2619-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Connettere":::

2. <span data-ttu-id="a2619-183">Modificare ognuna delle connessioni una alla volta selezionando l'icona a tre punti.</span><span class="sxs-lookup"><span data-stu-id="a2619-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="a2619-184">Aggiungere le connessioni pertinenti.</span><span class="sxs-lookup"><span data-stu-id="a2619-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Connessioni elencate"::: 

3.  <span data-ttu-id="a2619-186">Attivare i flussi nella sequenza seguente:</span><span class="sxs-lookup"><span data-stu-id="a2619-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="a2619-187">Registrazione webhook del centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="a2619-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="a2619-188">Creazione di un riferimento di co-selling: Dynamics 365 al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="a2619-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a2619-189">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Dynamics 365 (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a2619-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="a2619-190">Da partner Center a Dynamics 365 (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a2619-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="a2619-191">Da Dynamics 365 al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="a2619-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a2619-192">Dynamics 365 opportunity to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a2619-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a2619-193">Dynamics 365 Microsoft Solutions to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="a2619-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="a2619-194">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="a2619-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="a2619-195">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="a2619-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="a2619-196">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="a2619-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="a2619-197">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="a2619-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="a2619-198">Aggiungere le connessioni per l'utente del centro per i partner (a.) con le credenziali di amministratore di riferimento (b.) eventi del centro per i partner come indicato di seguito</span><span class="sxs-lookup"><span data-stu-id="a2619-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="a2619-200">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="a2619-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="a2619-202">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="a2619-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="a2619-203">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="a2619-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="a2619-204">Selezionare **centro per i partner per Dynamics 365 (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="a2619-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="a2619-205">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="a2619-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="a2619-206">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="a2619-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="a2619-208">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="a2619-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="a2619-209">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="a2619-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="a2619-210">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="a2619-210">Enter the following details:</span></span>

    1. <span data-ttu-id="a2619-211">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="a2619-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="a2619-212">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="a2619-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="a2619-213">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="a2619-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="a2619-214">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="a2619-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="a2619-215">Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.</span><span class="sxs-lookup"><span data-stu-id="a2619-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="a2619-216">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="a2619-216">Customize synchronization steps</span></span>

<span data-ttu-id="a2619-217">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="a2619-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="a2619-218">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="a2619-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="a2619-219">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="a2619-220">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="a2619-221">Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="a2619-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="a2619-222">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="a2619-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="a2619-223">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="a2619-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="a2619-224">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="a2619-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="a2619-225">a.</span><span class="sxs-lookup"><span data-stu-id="a2619-225">a.</span></span> <span data-ttu-id="a2619-226">Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="a2619-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="a2619-227">b.</span><span class="sxs-lookup"><span data-stu-id="a2619-227">b.</span></span> <span data-ttu-id="a2619-228">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2619-229">c.</span><span class="sxs-lookup"><span data-stu-id="a2619-229">c.</span></span> <span data-ttu-id="a2619-230">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="a2619-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="a2619-231">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="a2619-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="a2619-232">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="a2619-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="a2619-233">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="a2619-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="a2619-234">d.</span><span class="sxs-lookup"><span data-stu-id="a2619-234">d.</span></span> <span data-ttu-id="a2619-235">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="a2619-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="a2619-236">e.</span><span class="sxs-lookup"><span data-stu-id="a2619-236">e.</span></span> <span data-ttu-id="a2619-237">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="a2619-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="a2619-238">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="a2619-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="a2619-239">f.</span><span class="sxs-lookup"><span data-stu-id="a2619-239">f.</span></span> <span data-ttu-id="a2619-240">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="a2619-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="a2619-241">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="a2619-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="a2619-242">a.</span><span class="sxs-lookup"><span data-stu-id="a2619-242">a.</span></span> <span data-ttu-id="a2619-243">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="a2619-244">b.</span><span class="sxs-lookup"><span data-stu-id="a2619-244">b.</span></span> <span data-ttu-id="a2619-245">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="a2619-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="a2619-246">c.</span><span class="sxs-lookup"><span data-stu-id="a2619-246">c.</span></span> <span data-ttu-id="a2619-247">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare **se c'è differenza tra gli oggetti lead in Partner Center e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="a2619-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="a2619-248">d.</span><span class="sxs-lookup"><span data-stu-id="a2619-248">d.</span></span> <span data-ttu-id="a2619-249">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="a2619-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="a2619-250">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="a2619-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="a2619-251">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="a2619-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="a2619-252">a.</span><span class="sxs-lookup"><span data-stu-id="a2619-252">a.</span></span> <span data-ttu-id="a2619-253">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="a2619-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="a2619-254">b.</span><span class="sxs-lookup"><span data-stu-id="a2619-254">b.</span></span> <span data-ttu-id="a2619-255">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="a2619-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="a2619-256">c.</span><span class="sxs-lookup"><span data-stu-id="a2619-256">c.</span></span> <span data-ttu-id="a2619-257">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="a2619-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="a2619-258">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="a2619-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="a2619-259">Sono state create due variabili di ambiente:</span><span class="sxs-lookup"><span data-stu-id="a2619-259">There are two environment variables created:</span></span>

- <span data-ttu-id="a2619-260">Segno di spunta: indica se è necessaria un'icona di segno di spunta oltre alle opportunità sincronizzate in modo bidirezionale tra il centro per i partner e Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="a2619-261">Sincronizza solo opportunità di co-selling: indica se si vuole sincronizzare solo le opportunità di co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="a2619-262">È possibile scegliere di modificare il valore predefinito per le variabili di ambiente.</span><span class="sxs-lookup"><span data-stu-id="a2619-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Casella di modifica per i valori predefiniti":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="a2619-264">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="a2619-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="a2619-265">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 e centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="a2619-266">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="a2619-266">Pre-requisites</span></span>

<span data-ttu-id="a2619-267">Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM, la soluzione Power automatizzate delimita chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a2619-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="a2619-268">Questa identificazione consente ai team dei venditori di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="a2619-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="a2619-269">Un set di campi personalizzati è disponibile come parte dell'entità **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="a2619-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="a2619-270">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="a2619-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="a2619-271">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="a2619-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="a2619-272">**Sincronizzare con il centro** per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2619-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="a2619-273">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2619-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="a2619-274">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="a2619-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="a2619-275">In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="a2619-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="a2619-276">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="a2619-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="a2619-277">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2619-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="a2619-278">Aggiornare il modulo opportunità in Dynamics 365 CRM per includere le soluzioni per il campo prodotti.</span><span class="sxs-lookup"><span data-stu-id="a2619-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Modulo opportunità":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="a2619-281">SCENARI</span><span class="sxs-lookup"><span data-stu-id="a2619-281">SCENARIOS:</span></span>

1. <span data-ttu-id="a2619-282">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="a2619-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="a2619-283">Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="a2619-284">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a2619-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sezione dell'opportunità di esempio che mostra le informazioni sul centro per i partner Microsoft in Dynamics 365.":::

   3. <span data-ttu-id="a2619-286">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="a2619-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="a2619-287">**Sincronizza con il centro per i partner**: Sì</span><span class="sxs-lookup"><span data-stu-id="a2619-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="a2619-288">**Come può essere utile Microsoft?**: selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a2619-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sezione dell'opportunità di esempio in Dynamics 365 che mostra le opzioni della Guida di Microsoft Partner Center accanto a un campo denominato come può essere utile Microsoft?":::

      - <span data-ttu-id="a2619-290">**Prodotti**: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="a2619-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="a2619-291">Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti e quindi accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="a2619-292">I riferimenti verranno sincronizzati con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2619-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="a2619-293">Analogamente, per un'opportunità con l'opzione "Sync with partner Center" impostata su "Yes", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="a2619-294">Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a2619-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="a2619-295">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="a2619-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="a2619-296">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="a2619-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="a2619-297">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="a2619-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="a2619-298">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="a2619-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="a2619-299">Accedere al proprio ambiente Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="a2619-300">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="a2619-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="a2619-301">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="a2619-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="a2619-302">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="a2619-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2619-303">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="a2619-303">Next steps</span></span>

- [<span data-ttu-id="a2619-304">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="a2619-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="a2619-305">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="a2619-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="a2619-306">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="a2619-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="a2619-307">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a2619-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)