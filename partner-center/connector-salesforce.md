---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b96be195788ccc8b82aafd0bddb90dd34a672f9
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422447"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="900ee-103">Connettore di co-selling per CRM Salesforce - Panoramica</span><span class="sxs-lookup"><span data-stu-id="900ee-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="900ee-104">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="900ee-104">Appropriate roles</span></span>

- <span data-ttu-id="900ee-105">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="900ee-105">Referrals admin</span></span>
- <span data-ttu-id="900ee-106">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="900ee-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="900ee-107">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="900ee-108">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="900ee-109">Utilizzando i connettori di co-selling, è possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="900ee-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="900ee-110">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="900ee-111">È possibile eseguire tutte le attività di riferimento quando si lavora all'interno del CRM scelto piuttosto che nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="900ee-112">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="900ee-113">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="900ee-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="900ee-114">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="900ee-114">**Topics**</span></span>   |<span data-ttu-id="900ee-115">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="900ee-115">**Details**</span></span>   |<span data-ttu-id="900ee-116">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="900ee-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="900ee-117">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="900ee-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="900ee-118">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="900ee-118">You need a valid MPN ID</span></span>|<span data-ttu-id="900ee-119">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="900ee-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="900ee-120">Co-selling pronto</span><span class="sxs-lookup"><span data-stu-id="900ee-120">Co-sell ready</span></span>|<span data-ttu-id="900ee-121">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="900ee-122">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="900ee-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="900ee-123">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="900ee-123">Partner Center account</span></span>|<span data-ttu-id="900ee-124">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="900ee-125">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="900ee-126">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="900ee-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="900ee-127">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="900ee-127">Partner Center user roles</span></span>|<span data-ttu-id="900ee-128">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="900ee-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="900ee-129">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="900ee-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="900ee-130">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="900ee-130">Salesforce CRM</span></span>|<span data-ttu-id="900ee-131">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="900ee-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="900ee-132">Assegnare ruoli in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="900ee-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="900ee-133">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="900ee-133">Power Automate Flow Account</span></span>|<span data-ttu-id="900ee-134">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="900ee-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="900ee-135">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="900ee-136">Installazione del pacchetto Salesforce per i campi personalizzati Microsoft</span><span class="sxs-lookup"><span data-stu-id="900ee-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="900ee-137">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve identificare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="900ee-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="900ee-138">Questa delimitazione offre ai team dei venditori partner la possibilità di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="900ee-139">In Salesforce attivare le **Note** e aggiungerle all'elenco relativo alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="900ee-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="900ee-140">Riferimento</span><span class="sxs-lookup"><span data-stu-id="900ee-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="900ee-141">Attivare i **Team opportunity** attenendosi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="900ee-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="900ee-142">Nel programma di installazione utilizzare la casella **ricerca rapida** per individuare le impostazioni del team di opportunità.</span><span class="sxs-lookup"><span data-stu-id="900ee-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="900ee-143">Definire le impostazioni in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="900ee-143">Define the settings as needed.</span></span>
[<span data-ttu-id="900ee-144">Riferimento</span><span class="sxs-lookup"><span data-stu-id="900ee-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="900ee-145">In Salesforce installare i campi e gli oggetti personalizzati usando il programma di installazione del pacchetto riportato di seguito.</span><span class="sxs-lookup"><span data-stu-id="900ee-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="900ee-146">Per installare il pacchetto in qualsiasi azienda, fare clic [qui](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) :</span><span class="sxs-lookup"><span data-stu-id="900ee-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="900ee-147">Nota: se si esegue l'installazione in un ambiente sandbox, è necessario sostituire la parte iniziale dell'URL con http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="900ee-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="900ee-148">In Salesforce aggiungere soluzioni Microsoft all'elenco relativo alle **opportunità** .</span><span class="sxs-lookup"><span data-stu-id="900ee-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="900ee-149">Una volta aggiunto, fare clic sull'icona della **chiave** e aggiornare le proprietà</span><span class="sxs-lookup"><span data-stu-id="900ee-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="900ee-150">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="900ee-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="900ee-151">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="900ee-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="900ee-152">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="900ee-153">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="900ee-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="900ee-154">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="900ee-155">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="900ee-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="900ee-156">Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="900ee-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="900ee-157">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="900ee-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="900ee-158">Vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="900ee-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="900ee-159">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="900ee-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="900ee-160">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="900ee-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="900ee-161">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="900ee-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. <span data-ttu-id="900ee-163">Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="900ee-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="900ee-165">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="900ee-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="900ee-166">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="900ee-167">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="900ee-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="DISPONGONO disponibili":::

8. <span data-ttu-id="900ee-169">Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="900ee-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="900ee-170">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="900ee-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="900ee-171">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="900ee-172">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="900ee-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="900ee-173">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="900ee-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="900ee-174">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="900ee-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="900ee-175">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="900ee-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="900ee-176">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="900ee-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flussi di Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="900ee-178">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="900ee-178">Configure the solution</span></span>

1. <span data-ttu-id="900ee-179">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="900ee-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="900ee-180">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="900ee-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="900ee-181">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="900ee-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="900ee-182">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="900ee-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="900ee-183">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="900ee-183">Partner Center Events</span></span>
    - <span data-ttu-id="900ee-184">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="900ee-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="900ee-185">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="900ee-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="900ee-186">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="900ee-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Creare la connessione":::

- <span data-ttu-id="900ee-188">Cercare i riferimenti per il centro per i partner (anteprima) nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="900ee-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="900ee-189">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="900ee-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="900ee-190">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="900ee-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="900ee-191">Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="900ee-192">Una volta aggiunte tutte le connessioni, nell'ambiente verranno visualizzate le connessioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="900ee-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Osservare le connessioni":::

### <a name="edit-the-connections"></a><span data-ttu-id="900ee-194">Modificare le connessioni</span><span class="sxs-lookup"><span data-stu-id="900ee-194">Edit the connections</span></span>

1. <span data-ttu-id="900ee-195">Tornare alla pagina soluzioni e selezionare **soluzione predefinita**.</span><span class="sxs-lookup"><span data-stu-id="900ee-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="900ee-196">Selezionare **riferimento alla connessione (anteprima)** facendo clic su **tutto**.</span><span class="sxs-lookup"><span data-stu-id="900ee-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inizio modifica connettore":::

2. <span data-ttu-id="900ee-198">Modificare ognuna delle connessioni una alla volta selezionando l'icona a tre punti.</span><span class="sxs-lookup"><span data-stu-id="900ee-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="900ee-199">Aggiungere le connessioni pertinenti.</span><span class="sxs-lookup"><span data-stu-id="900ee-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modificare i connettori":::

3. <span data-ttu-id="900ee-201">Attivare i flussi nella sequenza seguente:</span><span class="sxs-lookup"><span data-stu-id="900ee-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="900ee-202">Registrazione webhook del centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="900ee-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="900ee-203">Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="900ee-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="900ee-204">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="900ee-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="900ee-205">Da partner Center a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="900ee-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="900ee-206">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="900ee-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="900ee-207">Opportunità di Salesforce per il centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="900ee-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="900ee-208">Salesforce Microsoft Solutions to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="900ee-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="900ee-209">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="900ee-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="900ee-210">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="900ee-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="900ee-211">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="900ee-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="900ee-212">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="900ee-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="900ee-213">Aggiungere le connessioni per l'utente del centro per i partner (a.) con le credenziali di amministratore di riferimento (b.) eventi del centro per i partner come indicato di seguito</span><span class="sxs-lookup"><span data-stu-id="900ee-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="900ee-215">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="900ee-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="900ee-217">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="900ee-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="900ee-218">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="900ee-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="900ee-219">Selezionare **centro per i partner per Salesforce CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="900ee-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="900ee-220">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="900ee-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="900ee-221">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="900ee-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="900ee-223">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="900ee-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="900ee-224">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="900ee-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="900ee-225">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="900ee-225">Enter the following details:</span></span>

    1. <span data-ttu-id="900ee-226">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="900ee-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="900ee-227">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="900ee-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="900ee-228">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="900ee-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="900ee-229">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="900ee-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="900ee-230">Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.</span><span class="sxs-lookup"><span data-stu-id="900ee-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="900ee-231">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="900ee-231">Customize synchronization steps</span></span>

<span data-ttu-id="900ee-232">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="900ee-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="900ee-233">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="900ee-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="900ee-234">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="900ee-235">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="900ee-236">Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="900ee-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="900ee-237">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="900ee-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="900ee-238">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="900ee-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="900ee-239">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="900ee-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="900ee-240">Selezionare Centro per i partner per Salesforce CRM (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="900ee-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="900ee-241">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="900ee-242">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="900ee-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="900ee-243">Per personalizzare i mapping dei campi CRM per creare eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="900ee-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="900ee-244">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="900ee-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="900ee-245">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="900ee-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="900ee-246">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="900ee-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="900ee-247">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="900ee-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="900ee-248">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="900ee-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="900ee-249">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="900ee-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="900ee-250">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="900ee-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="900ee-251">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="900ee-252">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="900ee-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="900ee-253">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="900ee-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="900ee-254">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="900ee-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="900ee-255">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="900ee-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="900ee-256">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="900ee-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="900ee-257">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="900ee-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="900ee-258">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="900ee-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="900ee-259">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="900ee-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="900ee-260">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="900ee-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="900ee-261">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="900ee-261">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="900ee-262">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Salesforce CRM e il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-262">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="900ee-263">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="900ee-263">Pre-requisites</span></span>

<span data-ttu-id="900ee-264">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="900ee-264">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="900ee-265">Questa identificazione consente ai team dei venditori di decidere quali riferimenti desiderano condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="900ee-265">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="900ee-266">Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-266">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="900ee-267">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="900ee-267">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="900ee-268">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="900ee-268">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="900ee-269">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="900ee-269">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="900ee-270">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="900ee-270">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="900ee-271">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="900ee-271">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="900ee-272">**Come è possibile eseguire la Guida Microsoft**per informazioni su come richiedere Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="900ee-272">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="900ee-273">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="900ee-273">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="900ee-274">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="900ee-274">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="900ee-275">SCENARI</span><span class="sxs-lookup"><span data-stu-id="900ee-275">SCENARIOS:</span></span>

1. <span data-ttu-id="900ee-276">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="900ee-276">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="900ee-277">Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-277">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="900ee-278">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="900ee-278">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce":::

   3. <span data-ttu-id="900ee-280">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="900ee-280">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="900ee-281">"Sincronizza con il centro per i partner": Sì</span><span class="sxs-lookup"><span data-stu-id="900ee-281">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="900ee-282">"Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="900ee-282">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="900ee-283">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="900ee-283">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="900ee-284">Dopo aver impostato l'opzione opportunity  **Sync with partner Center** su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-284">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="900ee-285">I riferimenti verranno sincronizzati con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-285">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="900ee-286">Quando l'opzione "Sincronizza con il centro per i partner" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-286">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="900ee-287">Le opportunità che vengono sincronizzate correttamente con partner Center verranno identificate con ✔ icona in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-287">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="900ee-288">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="900ee-288">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="900ee-289">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="900ee-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="900ee-290">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="900ee-290">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="900ee-291">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="900ee-291">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="900ee-292">Accedere all'ambiente Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-292">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="900ee-293">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="900ee-293">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="900ee-294">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="900ee-294">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata di opportunità di Salesforce":::

    6. <span data-ttu-id="900ee-296">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="900ee-296">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="900ee-297">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="900ee-297">Next steps</span></span>

- [<span data-ttu-id="900ee-298">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="900ee-298">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="900ee-299">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="900ee-299">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="900ee-300">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="900ee-300">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)