---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare le segnalazioni Partner Center con Salesforce CRM. I venditori possono quindi eseguire il co-selling con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276978"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="20d4a-104">Connettore di co-selling per CRM Salesforce - Panoramica</span><span class="sxs-lookup"><span data-stu-id="20d4a-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="20d4a-105">**Ruoli appropriati:** amministratore delle segnalazioni | Amministratore di sistema o a personalizzatore di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="20d4a-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="20d4a-106">Partner Center connettore di co-selling consente ai venditori di co-selling con Microsoft dall'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="20d4a-107">Non sarà necessario eseguire il training per usare le Partner Center per gestire le trattative di co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="20d4a-108">Usando i connettori di co-selling, puoi creare una nuova segnalazione di co-selling per coinvolgere un venditore Microsoft, ricevere segnalazioni dal venditore Microsoft, accettare/rifiutare le segnalazioni, modificare i dati delle trattative, ad esempio il valore della trattativa e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="20d4a-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="20d4a-109">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft su queste trattative di co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="20d4a-110">È possibile eseguire tutte le segnalazioni mentre si lavora all'interno del sistema CRM preferito anziché in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20d4a-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="20d4a-111">La soluzione è basata su Microsoft Power Automate e usa Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="20d4a-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="20d4a-112">Prima di installare : prerequisiti</span><span class="sxs-lookup"><span data-stu-id="20d4a-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="20d4a-113">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="20d4a-113">**Topics**</span></span>   |<span data-ttu-id="20d4a-114">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="20d4a-114">**Details**</span></span>   |<span data-ttu-id="20d4a-115">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="20d4a-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="20d4a-116">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="20d4a-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="20d4a-117">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="20d4a-117">You need a valid MPN ID</span></span>|<span data-ttu-id="20d4a-118">Per partecipare [a MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="20d4a-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="20d4a-119">Pronto per il co-selling</span><span class="sxs-lookup"><span data-stu-id="20d4a-119">Co-sell ready</span></span>|<span data-ttu-id="20d4a-120">La soluzione IP/Servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="20d4a-121">Vendere con Microsoft</span><span class="sxs-lookup"><span data-stu-id="20d4a-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="20d4a-122">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="20d4a-122">Partner Center account</span></span>|<span data-ttu-id="20d4a-123">L'ID MPN associato al tenant Partner Center deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="20d4a-124">Verificare che sia possibile visualizzare le segnalazioni di co-selling Partner Center portale prima di distribuire i connettori.</span><span class="sxs-lookup"><span data-stu-id="20d4a-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="20d4a-125">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="20d4a-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="20d4a-126">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="20d4a-126">Partner Center user roles</span></span>|<span data-ttu-id="20d4a-127">Il dipendente che installerà e userà i connettori deve essere un amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="20d4a-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="20d4a-128">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="20d4a-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="20d4a-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20d4a-129">Salesforce CRM</span></span>|<span data-ttu-id="20d4a-130">Il ruolo utente CRM è Amministratore di sistema o A personalizzatore sistema</span><span class="sxs-lookup"><span data-stu-id="20d4a-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="20d4a-131">Assegnare ruoli in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20d4a-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="20d4a-132">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="20d4a-132">Power Automate Flow Account</span></span>|<span data-ttu-id="20d4a-133">Un account [di Power Automate](https://flow.microsoft.com) per l'amministratore di sistema CRM o l'asonalizzazione del sistema.</span><span class="sxs-lookup"><span data-stu-id="20d4a-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="20d4a-134">Tale utente deve accedere [al](https://flow.microsoft.com) Power Automate almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="20d4a-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="20d4a-135">Installazione del pacchetto Salesforce per i campi personalizzati Microsoft</span><span class="sxs-lookup"><span data-stu-id="20d4a-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="20d4a-136">Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve identificare chiaramente i campi di segnalazione specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20d4a-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="20d4a-137">Questa delimitazione offre ai team venditori dei partner la possibilità di decidere quali segnalazioni condividere con Microsoft per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="20d4a-138">In Salesforce attivare Note **e** aggiungerlo all'elenco correlato alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="20d4a-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="20d4a-139">Riferimento</span><span class="sxs-lookup"><span data-stu-id="20d4a-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="20d4a-140">Attivare **i team opportunity** seguendo questa procedura:</span><span class="sxs-lookup"><span data-stu-id="20d4a-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="20d4a-141">In Configurazione usare la casella **Ricerca rapida per** individuare Opportunity Team Settings (Impostazioni team opportunità).</span><span class="sxs-lookup"><span data-stu-id="20d4a-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="20d4a-142">Definire le impostazioni in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="20d4a-142">Define the settings as needed.</span></span>
[<span data-ttu-id="20d4a-143">Riferimento</span><span class="sxs-lookup"><span data-stu-id="20d4a-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="20d4a-144">In Salesforce installare campi e oggetti personalizzati usando il programma [di installazione del pacchetto](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="20d4a-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="20d4a-145">Usare questa opzione per installare il pacchetto in qualsiasi società.</span><span class="sxs-lookup"><span data-stu-id="20d4a-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="20d4a-146">Se si sta installando in una sandbox, è necessario sostituire la parte iniziale dell'URL con http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="20d4a-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="20d4a-147">In Salesforce aggiungere Soluzioni Microsoft **all'elenco Correlato** alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="20d4a-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="20d4a-148">Dopo l'aggiunta, selezionare **l'icona della chiave inglese** e aggiornare le proprietà</span><span class="sxs-lookup"><span data-stu-id="20d4a-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="20d4a-149">Procedura consigliata: eseguire il test prima di iniziare a essere live</span><span class="sxs-lookup"><span data-stu-id="20d4a-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="20d4a-150">Prima di installare, configurare e personalizzare la soluzione Power Automate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza crm di staging.</span><span class="sxs-lookup"><span data-stu-id="20d4a-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="20d4a-151">Installare la soluzione Microsoft Power Automate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="20d4a-152">Creare una copia della soluzione ed eseguire la configurazione e Power Automate le personalizzazioni del flusso nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="20d4a-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="20d4a-153">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="20d4a-154">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="20d4a-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="20d4a-155">Installare la Partner Center delle segnalazioni per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20d4a-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="20d4a-156">Passare a [Power Automate](https://flow.microsoft.com) e selezionare **Ambienti nell'angolo** superiore destro.</span><span class="sxs-lookup"><span data-stu-id="20d4a-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="20d4a-157">Verranno mostrate le istanze crm disponibili.</span><span class="sxs-lookup"><span data-stu-id="20d4a-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="20d4a-158">Selezionare l'istanza di CRM appropriata nell'elenco a discesa nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="20d4a-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="20d4a-159">Selezionare **Soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="20d4a-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="20d4a-160">Selezionare il **collegamento Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="20d4a-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Aprire AppSource.":::

5. <span data-ttu-id="20d4a-162">Cercare Partner Center **Referrals Connectors for Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="20d4a-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="20d4a-164">Selezionare il **pulsante Scarica adesso** e quindi **Continua.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="20d4a-165">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="20d4a-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="20d4a-166">Accettare termini e condizioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CrmS disponibile.":::

8. <span data-ttu-id="20d4a-168">Si verrà quindi indirizzati alla **pagina Gestisci le** soluzioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="20d4a-169">Passare a "Partner Center segnalazioni" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="20d4a-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="20d4a-170">**L'installazione** pianificata dovrebbe essere visualizzata Partner Center soluzione Segnalazioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="20d4a-171">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="20d4a-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="20d4a-172">Al termine dell'installazione, tornare [all'Power Automate](https://flow.microsoft.com) e selezionare **Soluzioni nell'area** di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="20d4a-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="20d4a-173">Si noti **che Partner Center delle segnalazioni per Salesforce** è disponibile nell'elenco Soluzioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="20d4a-174">Selezionare **Partner Center referrals Synchronization for Salesforce (Sincronizzazione delle segnalazioni per Salesforce).**</span><span class="sxs-lookup"><span data-stu-id="20d4a-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="20d4a-175">Sono disponibili Power Automate seguenti flussi ed entità:</span><span class="sxs-lookup"><span data-stu-id="20d4a-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flussi di Salesforce.":::



## <a name="configure-the-solution"></a><span data-ttu-id="20d4a-177">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="20d4a-177">Configure the solution</span></span>

1. <span data-ttu-id="20d4a-178">Dopo aver installato la soluzione nell'istanza di CRM, tornare [a Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="20d4a-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="20d4a-179">**Nell'elenco a** discesa Ambienti nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la Power Automate soluzione.</span><span class="sxs-lookup"><span data-stu-id="20d4a-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="20d4a-180">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="20d4a-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="20d4a-181">Partner Center utente con le credenziali di amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="20d4a-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="20d4a-182">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="20d4a-182">Partner Center Events</span></span>
    - <span data-ttu-id="20d4a-183">Amministratore CRM con i Power Automate nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="20d4a-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="20d4a-184">Selezionare **Connessioni** dalla barra di spostamento a sinistra e selezionare la soluzione "segnalazioni Partner Center" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="20d4a-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="20d4a-185">Creare una connessione facendo clic **su Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Creare una connessione.":::

- <span data-ttu-id="20d4a-187">Cercare Partner Center segnalazioni (anteprima) nella barra di ricerca nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="20d4a-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="20d4a-188">Creare una connessione per l'Partner Center utente con il ruolo credenziali di amministratore delle segnalazioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="20d4a-189">Creare quindi una connessione Partner Center eventi per l'utente Partner Center con le credenziali di amministratore delle segnalazioni.</span><span class="sxs-lookup"><span data-stu-id="20d4a-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="20d4a-190">Creare una connessione per Salesforce per l'utente amministratore di CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="20d4a-191">Dopo aver aggiunto tutte le connessioni, nell'ambiente dovrebbero essere presenti le connessioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="20d4a-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Osservare le connessioni.":::

### <a name="edit-the-connections"></a><span data-ttu-id="20d4a-193">Modificare le connessioni</span><span class="sxs-lookup"><span data-stu-id="20d4a-193">Edit the connections</span></span>

1. <span data-ttu-id="20d4a-194">Tornare alla pagina Soluzioni e selezionare **Soluzione predefinita.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="20d4a-195">Selezionare **Riferimento alla connessione (anteprima)** facendo clic su **Tutti**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniziare la modifica del connettore.":::

2. <span data-ttu-id="20d4a-197">Modificare ognuna delle connessioni singolarmente selezionando l'icona con i tre puntini.</span><span class="sxs-lookup"><span data-stu-id="20d4a-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="20d4a-198">Aggiungere le connessioni pertinenti.</span><span class="sxs-lookup"><span data-stu-id="20d4a-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modificare i connettori.":::

3. <span data-ttu-id="20d4a-200">Attivare i flussi nella sequenza seguente:</span><span class="sxs-lookup"><span data-stu-id="20d4a-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="20d4a-201">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-202">Creare una segnalazione di co-selling - Salesforce per Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-203">Partner Center microsoft co-selling referral updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-204">Partner Center a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-205">Da Salesforce a Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-206">Opportunità di salesforce per Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="20d4a-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="20d4a-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="20d4a-208">Usare le API webhook per la registrazione per gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="20d4a-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="20d4a-209">Le PARTNER CENTER Webhook consentono di registrarsi per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="20d4a-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="20d4a-210">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="20d4a-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="20d4a-211">Per registrare l'URL, **selezionare Partner Center webhook registration (Insider Preview) Power Automate** flusso.</span><span class="sxs-lookup"><span data-stu-id="20d4a-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="20d4a-212">Aggiungere connessioni per (a.) Partner Center utente con credenziali di amministratore delle segnalazioni (b.) Partner Center eventi come evidenziato di seguito</span><span class="sxs-lookup"><span data-stu-id="20d4a-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Grilletto.":::

3. <span data-ttu-id="20d4a-214">Quando si apportano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="20d4a-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook.":::

4. <span data-ttu-id="20d4a-216">Salvare le modifiche e selezionare **Attiva**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="20d4a-217">Per abilitare Partner Center webhook per l'ascolto delle modifiche degli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="20d4a-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="20d4a-218">Selezionare **Partner Center a Salesforce CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="20d4a-219">Selezionare **l'icona** Modifica e selezionare **Quando viene ricevuta una richiesta HTTP.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="20d4a-220">Selezionare **l'icona** Copia per copiare l'URL HTTP POST specificato.</span><span class="sxs-lookup"><span data-stu-id="20d4a-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiare l'URL.":::

8. <span data-ttu-id="20d4a-222">Selezionare ora il flusso di Partner Center webhook (Insider Preview) Power Automate e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="20d4a-223">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e selezionare **Continua.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="20d4a-224">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="20d4a-224">Enter the following details:</span></span>

    1. <span data-ttu-id="20d4a-225">**Endpoint trigger HTTP:** URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="20d4a-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="20d4a-226">**Eventi da registrare:**"referral-created" e "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="20d4a-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="20d4a-227">**Sovrascrivi gli endpoint del trigger esistenti se presenti:** Sì (in questo modo vengono sovrascritti tutti gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="20d4a-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="20d4a-228">Selezionare **Esegui** e quindi **Fare clic su Fine.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="20d4a-229">Il webhook può ora restare in ascolto degli eventi di creazione e aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="20d4a-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="20d4a-230">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="20d4a-230">Customize synchronization steps</span></span>

<span data-ttu-id="20d4a-231">Quando le segnalazioni di co-selling vengono sincronizzate tra Partner Center e il sistema CRM, i campi sincronizzati Partner Center PC sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="20d4a-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="20d4a-232">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="20d4a-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="20d4a-233">È possibile personalizzare i Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="20d4a-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="20d4a-234">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="20d4a-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="20d4a-235">Vengono forniti mapping da Microsoft Partner Center a CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="20d4a-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="20d4a-236">È possibile personalizzare più passaggi di Power Automate flusso di lavoro in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="20d4a-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="20d4a-237">Di seguito sono riportati esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="20d4a-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="20d4a-238">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel Partner Center alla sincronizzazione delle segnalazioni di CRM:</span><span class="sxs-lookup"><span data-stu-id="20d4a-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="20d4a-239">Selezionare Partner Center a Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="20d4a-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="20d4a-240">Selezionare **Modifica** per modificare o personalizzare il flusso Power Automate dati.</span><span class="sxs-lookup"><span data-stu-id="20d4a-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="20d4a-241">Selezionare **(Ambito) Sincronizzare il lead o l'opportunità.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="20d4a-242">Per personalizzare i mapping dei campi CRM per la creazione di eventi, selezionare Se si tratta di una **nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="20d4a-243">Selezionare il passaggio secondario **in caso affermativa** e quindi espandere **Creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="20d4a-244">È possibile modificare i mapping in questa sezione usando la Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="20d4a-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="20d4a-245">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare il passaggio "(Ambito) Sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="20d4a-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="20d4a-246">Selezionare **Se si tratta di un aggiornamento di un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="20d4a-247">Selezionare il passaggio secondario **in caso affermativa** e quindi espandere Se la differenza tra gli oggetti opportunità in Partner Center **e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="20d4a-248">Selezionare **Se sì seguito** da Aggiorna opportunità **esistente**</span><span class="sxs-lookup"><span data-stu-id="20d4a-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="20d4a-249">Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="20d4a-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="20d4a-250">Selezionare **Modifica**  per modificare o personalizzare il flusso Power Automate dati.</span><span class="sxs-lookup"><span data-stu-id="20d4a-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="20d4a-251">Selezionare **(Ambito) Sincronizzare l'opportunità.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="20d4a-252">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per gli eventi di aggiornamento, selezionare Se esiste una differenza tra gli oggetti lead **in Partner Center e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="20d4a-253">Selezionare il passaggio secondario **in caso affermativa,** quindi espandere il passaggio **Aggiornare una segnalazione con i dati dell'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="20d4a-254">È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="20d4a-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="20d4a-255">Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="20d4a-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="20d4a-256">Selezionare **Modifica**  per modificare o personalizzare il flusso Power Automate dati.</span><span class="sxs-lookup"><span data-stu-id="20d4a-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="20d4a-257">Selezionare **(Ambito) Sincronizzazione delle segnalazioni.**</span><span class="sxs-lookup"><span data-stu-id="20d4a-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="20d4a-258">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea segnalazione Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="20d4a-259">È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="20d4a-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="20d4a-260">Sincronizzazione delle segnalazioni di co-selling bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="20d4a-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="20d4a-261">Dopo aver installato, configurato e personalizzato la soluzione Power Automate, è possibile testare la sincronizzazione delle segnalazioni di co-selling tra Salesforce CRM e Partner Center.</span><span class="sxs-lookup"><span data-stu-id="20d4a-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="20d4a-262">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="20d4a-262">Pre-requisites</span></span>

<span data-ttu-id="20d4a-263">Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve delimitare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20d4a-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="20d4a-264">Questa identificazione offre ai team venditori la possibilità di decidere quali segnalazioni condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="20d4a-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="20d4a-265">Un set di campi personalizzati è disponibile come parte dell'entità opportunità Partner Center di sincronizzazione delle **segnalazioni** per la soluzione Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="20d4a-266">Un utente amministratore di CRM dovrà creare una sezione CRM separata con i **campi** personalizzati Opportunità.</span><span class="sxs-lookup"><span data-stu-id="20d4a-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="20d4a-267">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="20d4a-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="20d4a-268">**Sincronizza con Partner Center**: indica se sincronizzare l'opportunità con Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="20d4a-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="20d4a-269">**Identificatore di riferimento:** campo dell'identificatore di sola lettura per la segnalazione Partner Center Microsoft</span><span class="sxs-lookup"><span data-stu-id="20d4a-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="20d4a-270">**Collegamento alla segnalazione:** collegamento di sola lettura alla segnalazione in Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="20d4a-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="20d4a-271">**Come può essere utile Microsoft:** Guida necessaria a Microsoft per la segnalazione</span><span class="sxs-lookup"><span data-stu-id="20d4a-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="20d4a-272">**Products**: elenco di prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="20d4a-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="20d4a-273">**Audit:** un'istanza di sola audit trail per la sincronizzazione con Partner Center segnalazioni</span><span class="sxs-lookup"><span data-stu-id="20d4a-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="20d4a-274">Scenari:</span><span class="sxs-lookup"><span data-stu-id="20d4a-274">SCENARIOS:</span></span>

1. <span data-ttu-id="20d4a-275">Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in CRM e sincronizzata in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="20d4a-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="20d4a-276">Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella **sezione Opportunità** di CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="20d4a-277">Assicurarsi che la sezione seguente sia presente quando si crea una "Nuova opportunità" nell'ambiente Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="20d4a-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce.":::

   3. <span data-ttu-id="20d4a-279">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="20d4a-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="20d4a-280">"Sync with Partner Center": Sì</span><span class="sxs-lookup"><span data-stu-id="20d4a-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="20d4a-281">"Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="20d4a-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="20d4a-282">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="20d4a-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="20d4a-283">Dopo aver impostato l'opzione Sincronizza  **con Partner Center** su Sì **,** attendere 10 minuti, accedere all'account Partner Center utente.</span><span class="sxs-lookup"><span data-stu-id="20d4a-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="20d4a-284">Le segnalazioni verranno sincronizzate con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="20d4a-285">Quando l'opzione "Sincronizza con Partner Center" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account Partner Center personale.</span><span class="sxs-lookup"><span data-stu-id="20d4a-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="20d4a-286">Le opportunità sincronizzate correttamente con Partner Center verranno identificate con ✔icon in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="20d4a-287">Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in Microsoft Partner Center sincronizzata nell'ambiente Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="20d4a-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="20d4a-288">Accedere al dashboard [Partner Center.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="20d4a-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="20d4a-289">Selezionare **Segnalazioni** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="20d4a-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="20d4a-290">Creare una nuova segnalazione di co-selling da Partner Center facendo clic sull'opzione "New deal".</span><span class="sxs-lookup"><span data-stu-id="20d4a-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="20d4a-291">Accedere all'ambiente Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="20d4a-292">Passare a **Apri opportunità**.</span><span class="sxs-lookup"><span data-stu-id="20d4a-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="20d4a-293">La segnalazione creata in Microsoft Partner Center è ora sincronizzata in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="20d4a-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata opportunità di Salesforce.":::

    6. <span data-ttu-id="20d4a-295">Quando si seleziona una segnalazione sincronizzata, i dettagli della visualizzazione scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="20d4a-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20d4a-296">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="20d4a-296">Next steps</span></span>

- [<span data-ttu-id="20d4a-297">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="20d4a-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="20d4a-298">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="20d4a-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="20d4a-299">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="20d4a-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
