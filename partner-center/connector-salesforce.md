---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Salesforce CRM. I venditori possono quindi co-vendere con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 68b8bdf7a88c1ca8d063cf3198fc49bf87552edb
ms.sourcegitcommit: de2ac2eea26426ae8f962d29ab50b68850318ce6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/07/2021
ms.locfileid: "97960952"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="d9ee0-104">Connettore di co-selling per CRM Salesforce - Panoramica</span><span class="sxs-lookup"><span data-stu-id="d9ee0-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="d9ee0-105">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="d9ee0-105">Appropriate roles</span></span>

- <span data-ttu-id="d9ee0-106">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="d9ee0-106">Referrals admin</span></span>
- <span data-ttu-id="d9ee0-107">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="d9ee0-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="d9ee0-108">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="d9ee0-109">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="d9ee0-110">Utilizzando i connettori di co-selling, è possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="d9ee0-111">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="d9ee0-112">È possibile eseguire tutte le attività di riferimento quando si lavora all'interno del CRM scelto piuttosto che nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="d9ee0-113">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="d9ee0-114">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="d9ee0-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="d9ee0-115">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-115">**Topics**</span></span>   |<span data-ttu-id="d9ee0-116">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-116">**Details**</span></span>   |<span data-ttu-id="d9ee0-117">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="d9ee0-118">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="d9ee0-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="d9ee0-119">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="d9ee0-119">You need a valid MPN ID</span></span>|<span data-ttu-id="d9ee0-120">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="d9ee0-121">Co-selling pronto</span><span class="sxs-lookup"><span data-stu-id="d9ee0-121">Co-sell ready</span></span>|<span data-ttu-id="d9ee0-122">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="d9ee0-123">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="d9ee0-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="d9ee0-124">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9ee0-124">Partner Center account</span></span>|<span data-ttu-id="d9ee0-125">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="d9ee0-126">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="d9ee0-127">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="d9ee0-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="d9ee0-128">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9ee0-128">Partner Center user roles</span></span>|<span data-ttu-id="d9ee0-129">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="d9ee0-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="d9ee0-130">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="d9ee0-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="d9ee0-131">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="d9ee0-131">Salesforce CRM</span></span>|<span data-ttu-id="d9ee0-132">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="d9ee0-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="d9ee0-133">Assegnare ruoli in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="d9ee0-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="d9ee0-134">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="d9ee0-134">Power Automate Flow Account</span></span>|<span data-ttu-id="d9ee0-135">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="d9ee0-136">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="d9ee0-137">Installazione del pacchetto Salesforce per i campi personalizzati Microsoft</span><span class="sxs-lookup"><span data-stu-id="d9ee0-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="d9ee0-138">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve identificare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="d9ee0-139">Questa delimitazione offre ai team dei venditori partner la possibilità di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="d9ee0-140">In Salesforce attivare le **Note** e aggiungerle all'elenco relativo alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="d9ee0-141">Riferimento</span><span class="sxs-lookup"><span data-stu-id="d9ee0-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="d9ee0-142">Attivare i **Team opportunity** attenendosi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="d9ee0-143">Nel programma di installazione utilizzare la casella **ricerca rapida** per individuare le impostazioni del team di opportunità.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="d9ee0-144">Definire le impostazioni in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-144">Define the settings as needed.</span></span>
[<span data-ttu-id="d9ee0-145">Riferimento</span><span class="sxs-lookup"><span data-stu-id="d9ee0-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="d9ee0-146">In Salesforce installare i campi e gli oggetti personalizzati usando il programma di installazione del pacchetto riportato di seguito.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="d9ee0-147">Per installare il pacchetto in qualsiasi azienda, fare clic [qui](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) .</span><span class="sxs-lookup"><span data-stu-id="d9ee0-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) to install the package into any company.</span></span>


<span data-ttu-id="d9ee0-148">Nota: se si esegue l'installazione in un ambiente sandbox, è necessario sostituire la parte iniziale dell'URL con http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="d9ee0-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="d9ee0-149">In Salesforce aggiungere soluzioni Microsoft all'elenco relativo alle **opportunità** .</span><span class="sxs-lookup"><span data-stu-id="d9ee0-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="d9ee0-150">Una volta aggiunto, fare clic sull'icona della **chiave** e aggiornare le proprietà</span><span class="sxs-lookup"><span data-stu-id="d9ee0-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="d9ee0-151">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="d9ee0-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="d9ee0-152">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="d9ee0-153">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="d9ee0-154">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="d9ee0-155">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="d9ee0-156">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="d9ee0-157">Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="d9ee0-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="d9ee0-158">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="d9ee0-159">Vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="d9ee0-160">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="d9ee0-161">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="d9ee0-162">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. <span data-ttu-id="d9ee0-164">Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="d9ee0-166">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="d9ee0-167">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="d9ee0-168">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="DISPONGONO disponibili":::

8. <span data-ttu-id="d9ee0-170">Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="d9ee0-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="d9ee0-171">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="d9ee0-172">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="d9ee0-173">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="d9ee0-174">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="d9ee0-175">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="d9ee0-176">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="d9ee0-177">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flussi di Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="d9ee0-179">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="d9ee0-179">Configure the solution</span></span>

1. <span data-ttu-id="d9ee0-180">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="d9ee0-181">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="d9ee0-182">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="d9ee0-183">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="d9ee0-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="d9ee0-184">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9ee0-184">Partner Center Events</span></span>
    - <span data-ttu-id="d9ee0-185">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="d9ee0-186">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="d9ee0-187">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Creare la connessione":::

- <span data-ttu-id="d9ee0-189">Cercare i riferimenti per il centro per i partner (anteprima) nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="d9ee0-190">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="d9ee0-191">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="d9ee0-192">Creare una connessione per Salesforce per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="d9ee0-193">Una volta aggiunte tutte le connessioni, nell'ambiente verranno visualizzate le connessioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Osservare le connessioni":::

### <a name="edit-the-connections"></a><span data-ttu-id="d9ee0-195">Modificare le connessioni</span><span class="sxs-lookup"><span data-stu-id="d9ee0-195">Edit the connections</span></span>

1. <span data-ttu-id="d9ee0-196">Tornare alla pagina soluzioni e selezionare **soluzione predefinita**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="d9ee0-197">Selezionare **riferimento alla connessione (anteprima)** facendo clic su **tutto**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inizio modifica connettore":::

2. <span data-ttu-id="d9ee0-199">Modificare ognuna delle connessioni una alla volta selezionando l'icona a tre punti.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="d9ee0-200">Aggiungere le connessioni pertinenti.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modificare i connettori":::

3. <span data-ttu-id="d9ee0-202">Attivare i flussi nella sequenza seguente:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="d9ee0-203">Registrazione webhook del centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-204">Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-205">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-206">Da partner Center a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-207">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-208">Opportunità di Salesforce per il centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d9ee0-209">Salesforce Microsoft Solutions to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d9ee0-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="d9ee0-210">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="d9ee0-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="d9ee0-211">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="d9ee0-212">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="d9ee0-213">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="d9ee0-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="d9ee0-214">Aggiungere le connessioni per l'utente del centro per i partner (a.) con le credenziali di amministratore di riferimento (b.) eventi del centro per i partner come indicato di seguito</span><span class="sxs-lookup"><span data-stu-id="d9ee0-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="d9ee0-216">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="d9ee0-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="d9ee0-218">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="d9ee0-219">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="d9ee0-220">Selezionare **centro per i partner per Salesforce CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="d9ee0-221">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="d9ee0-222">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="d9ee0-224">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="d9ee0-225">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="d9ee0-226">Immettere le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-226">Enter the following details:</span></span>

    1. <span data-ttu-id="d9ee0-227">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="d9ee0-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="d9ee0-228">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="d9ee0-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="d9ee0-229">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="d9ee0-230">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="d9ee0-231">Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="d9ee0-232">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="d9ee0-232">Customize synchronization steps</span></span>

<span data-ttu-id="d9ee0-233">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="d9ee0-234">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="d9ee0-235">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="d9ee0-236">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="d9ee0-237">Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="d9ee0-238">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="d9ee0-239">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="d9ee0-240">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="d9ee0-241">Selezionare Centro per i partner per Salesforce CRM (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="d9ee0-242">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="d9ee0-243">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="d9ee0-244">Per personalizzare i mapping dei campi CRM per creare eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="d9ee0-245">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="d9ee0-246">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="d9ee0-247">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="d9ee0-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="d9ee0-248">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="d9ee0-249">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="d9ee0-250">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="d9ee0-251">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="d9ee0-252">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="d9ee0-253">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="d9ee0-254">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="d9ee0-255">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="d9ee0-256">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="d9ee0-257">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="d9ee0-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="d9ee0-258">Selezionare **modifica**  per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="d9ee0-259">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="d9ee0-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="d9ee0-260">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="d9ee0-261">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="d9ee0-262">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="d9ee0-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="d9ee0-263">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Salesforce CRM e il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="d9ee0-264">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="d9ee0-264">Pre-requisites</span></span>

<span data-ttu-id="d9ee0-265">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="d9ee0-266">Questa identificazione consente ai team dei venditori di decidere quali riferimenti desiderano condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="d9ee0-267">Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="d9ee0-268">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="d9ee0-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="d9ee0-269">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="d9ee0-270">**Sincronizzare con il centro** per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="d9ee0-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="d9ee0-271">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="d9ee0-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="d9ee0-272">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="d9ee0-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="d9ee0-273">**Come è possibile eseguire la Guida Microsoft** per informazioni su come richiedere Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="d9ee0-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="d9ee0-274">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="d9ee0-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="d9ee0-275">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9ee0-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="d9ee0-276">SCENARI</span><span class="sxs-lookup"><span data-stu-id="d9ee0-276">SCENARIOS:</span></span>

1. <span data-ttu-id="d9ee0-277">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="d9ee0-278">Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="d9ee0-279">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="d9ee0-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce":::

   3. <span data-ttu-id="d9ee0-281">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="d9ee0-282">"Sincronizza con il centro per i partner": Sì</span><span class="sxs-lookup"><span data-stu-id="d9ee0-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="d9ee0-283">"Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="d9ee0-284">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="d9ee0-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="d9ee0-285">Dopo aver impostato l'opzione opportunity  **Sync with partner Center** su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="d9ee0-286">I riferimenti verranno sincronizzati con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="d9ee0-287">Quando l'opzione "Sincronizza con il centro per i partner" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="d9ee0-288">Le opportunità che vengono sincronizzate correttamente con partner Center verranno identificate con ✔ icona in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="d9ee0-289">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="d9ee0-290">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="d9ee0-291">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="d9ee0-292">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="d9ee0-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="d9ee0-293">Accedere all'ambiente Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="d9ee0-294">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="d9ee0-295">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata di opportunità di Salesforce":::

    6. <span data-ttu-id="d9ee0-297">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d9ee0-298">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d9ee0-298">Next steps</span></span>

- [<span data-ttu-id="d9ee0-299">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="d9ee0-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="d9ee0-300">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="d9ee0-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="d9ee0-301">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9ee0-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
