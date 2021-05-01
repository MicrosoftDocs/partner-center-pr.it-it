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
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284384"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b1566-104">Connettore di co-selling per CRM Salesforce - Panoramica</span><span class="sxs-lookup"><span data-stu-id="b1566-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="b1566-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="b1566-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b1566-106">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="b1566-106">Referrals admin</span></span>
- <span data-ttu-id="b1566-107">Amministratore di sistema o a personalizzatore di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="b1566-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b1566-108">Partner Center connettore di co-selling consente ai venditori di co-selling con Microsoft dall'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b1566-109">Non sarà necessario eseguire il training per usare i Partner Center per gestire le trattative di co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b1566-110">Usando i connettori di co-selling, puoi creare una nuova segnalazione di co-selling per coinvolgere un venditore Microsoft, ricevere segnalazioni dal venditore Microsoft, accettare/rifiutare le segnalazioni, modificare i dati delle trattative, ad esempio il valore della trattativa e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="b1566-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b1566-111">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft su queste trattative di co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b1566-112">È possibile eseguire tutte le segnalazioni mentre si lavora all'interno del sistema CRM preferito anziché in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1566-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b1566-113">La soluzione è basata su Microsoft Power Automate e usa Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="b1566-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b1566-114">Prima di installare : prerequisiti</span><span class="sxs-lookup"><span data-stu-id="b1566-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b1566-115">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="b1566-115">**Topics**</span></span>   |<span data-ttu-id="b1566-116">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="b1566-116">**Details**</span></span>   |<span data-ttu-id="b1566-117">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="b1566-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b1566-118">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="b1566-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b1566-119">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="b1566-119">You need a valid MPN ID</span></span>|<span data-ttu-id="b1566-120">Per partecipare [a MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="b1566-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b1566-121">Pronto per il co-selling</span><span class="sxs-lookup"><span data-stu-id="b1566-121">Co-sell ready</span></span>|<span data-ttu-id="b1566-122">La soluzione IP/Servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b1566-123">Vendere con Microsoft</span><span class="sxs-lookup"><span data-stu-id="b1566-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b1566-124">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b1566-124">Partner Center account</span></span>|<span data-ttu-id="b1566-125">L'ID MPN associato al tenant Partner Center deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b1566-126">Verificare che sia possibile visualizzare le segnalazioni di co-selling Partner Center portale prima di distribuire i connettori.</span><span class="sxs-lookup"><span data-stu-id="b1566-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b1566-127">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="b1566-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b1566-128">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b1566-128">Partner Center user roles</span></span>|<span data-ttu-id="b1566-129">Il dipendente che installerà e userà i connettori deve essere un amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="b1566-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b1566-130">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="b1566-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b1566-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b1566-131">Salesforce CRM</span></span>|<span data-ttu-id="b1566-132">Il ruolo utente di CRM è Amministratore di sistema o A personalizzatore sistema</span><span class="sxs-lookup"><span data-stu-id="b1566-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b1566-133">Assegnare ruoli in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b1566-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="b1566-134">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="b1566-134">Power Automate Flow Account</span></span>|<span data-ttu-id="b1566-135">Un account [Power Automate](https://flow.microsoft.com) account per l'amministratore di sistema CRM o l'asonalizzazione del sistema.</span><span class="sxs-lookup"><span data-stu-id="b1566-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b1566-136">Tale utente deve accedere [a](https://flow.microsoft.com) Power Automate almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="b1566-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="b1566-137">Installazione del pacchetto Salesforce per i campi personalizzati Microsoft</span><span class="sxs-lookup"><span data-stu-id="b1566-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="b1566-138">Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve identificare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1566-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="b1566-139">Questa delimitazione offre ai team venditori partner la possibilità di decidere quali segnalazioni condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="b1566-140">In Salesforce attivare **Notes e** aggiungerlo all'elenco correlato alle opportunità.</span><span class="sxs-lookup"><span data-stu-id="b1566-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="b1566-141">Riferimento</span><span class="sxs-lookup"><span data-stu-id="b1566-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="b1566-142">Attivare **i team dell'opportunità** seguendo questa procedura:</span><span class="sxs-lookup"><span data-stu-id="b1566-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="b1566-143">Nel programma di installazione usare la **casella Ricerca rapida** per individuare Le impostazioni del team opportunità.</span><span class="sxs-lookup"><span data-stu-id="b1566-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="b1566-144">Definire le impostazioni in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="b1566-144">Define the settings as needed.</span></span>
[<span data-ttu-id="b1566-145">Riferimento</span><span class="sxs-lookup"><span data-stu-id="b1566-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="b1566-146">In Salesforce installare campi e oggetti personalizzati usando il programma [di installazione del pacchetto](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="b1566-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="b1566-147">Usare questa opzione per installare il pacchetto in qualsiasi azienda.</span><span class="sxs-lookup"><span data-stu-id="b1566-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="b1566-148">Se si installa in una sandbox, è necessario sostituire la parte iniziale dell'URL con http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="b1566-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="b1566-149">In Salesforce aggiungere Soluzioni Microsoft **all'elenco correlato** Opportunità.</span><span class="sxs-lookup"><span data-stu-id="b1566-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="b1566-150">Dopo l'aggiunta, selezionare **l'icona della chiave inglese** e aggiornare le proprietà</span><span class="sxs-lookup"><span data-stu-id="b1566-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b1566-151">Procedura consigliata: eseguire il test prima di iniziare a eseguire il test</span><span class="sxs-lookup"><span data-stu-id="b1566-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b1566-152">Prima di installare, configurare e personalizzare la soluzione Power Automate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza crm di staging.</span><span class="sxs-lookup"><span data-stu-id="b1566-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b1566-153">Installare la soluzione Microsoft Power Automate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b1566-154">Creare una copia della soluzione ed eseguire la configurazione e Power Automate del flusso nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="b1566-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b1566-155">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b1566-156">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="b1566-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b1566-157">Installare Partner Center delle segnalazioni per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b1566-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b1566-158">Passare a [Power Automate](https://flow.microsoft.com) e selezionare **Ambienti nell'angolo** superiore destro.</span><span class="sxs-lookup"><span data-stu-id="b1566-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b1566-159">Verranno mostrate le istanze crm disponibili.</span><span class="sxs-lookup"><span data-stu-id="b1566-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b1566-160">Selezionare l'istanza di CRM appropriata nell'elenco a discesa nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="b1566-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b1566-161">Selezionare **Soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="b1566-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b1566-162">Selezionare il **collegamento Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="b1566-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Aprire AppSource":::

5. <span data-ttu-id="b1566-164">Cercare Partner Center **Referrals Connectors for Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="b1566-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="b1566-166">Selezionare il **pulsante Scarica adesso** e quindi **Continua.**</span><span class="sxs-lookup"><span data-stu-id="b1566-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b1566-167">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="b1566-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b1566-168">Accettare termini e condizioni.</span><span class="sxs-lookup"><span data-stu-id="b1566-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibili":::

8. <span data-ttu-id="b1566-170">Si verrà quindi indirizzati alla **pagina Gestisci le** soluzioni.</span><span class="sxs-lookup"><span data-stu-id="b1566-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b1566-171">Passare a "Partner Center segnalazioni" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="b1566-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b1566-172">**L'installazione** pianificata dovrebbe essere visualizzata Partner Center soluzione Segnalazioni.</span><span class="sxs-lookup"><span data-stu-id="b1566-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b1566-173">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="b1566-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="b1566-174">Al termine dell'installazione, tornare a Power Automate [e](https://flow.microsoft.com) selezionare **Soluzioni nell'area** di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="b1566-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b1566-175">Si noti **Partner Center sincronizzazione delle segnalazioni per Salesforce** è disponibile nell'elenco Soluzioni.</span><span class="sxs-lookup"><span data-stu-id="b1566-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b1566-176">Selezionare **Partner Center Sincronizzazione delle segnalazioni per Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="b1566-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b1566-177">Sono disponibili Power Automate seguenti flussi ed entità:</span><span class="sxs-lookup"><span data-stu-id="b1566-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flussi di Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="b1566-179">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="b1566-179">Configure the solution</span></span>

1. <span data-ttu-id="b1566-180">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="b1566-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b1566-181">**Nell'elenco a** discesa Ambienti nell'angolo in alto a destra selezionare l'istanza di CRM in cui è stata installata Power Automate soluzione.</span><span class="sxs-lookup"><span data-stu-id="b1566-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="b1566-182">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="b1566-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="b1566-183">Partner Center utente con credenziali di amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="b1566-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="b1566-184">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b1566-184">Partner Center Events</span></span>
    - <span data-ttu-id="b1566-185">Amministratore di CRM con Power Automate flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="b1566-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="b1566-186">Selezionare **Connessioni** dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referral" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="b1566-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="b1566-187">Creare una connessione facendo clic **su Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="b1566-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Creare la connessione":::

- <span data-ttu-id="b1566-189">Cercare Partner Center segnalazioni (anteprima) nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="b1566-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="b1566-190">Creare una connessione per l'Partner Center utente con il ruolo credenziali dell'amministratore di Referrals.</span><span class="sxs-lookup"><span data-stu-id="b1566-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="b1566-191">Creare quindi una connessione Partner Center Eventi per l'utente Partner Center con le credenziali dell'amministratore di Referrals.</span><span class="sxs-lookup"><span data-stu-id="b1566-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="b1566-192">Creare una connessione per Salesforce per l'utente amministratore di CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="b1566-193">Dopo aver aggiunto tutte le connessioni, nell'ambiente dovrebbero essere presenti le connessioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="b1566-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Osservare le connessioni":::

### <a name="edit-the-connections"></a><span data-ttu-id="b1566-195">Modificare le connessioni</span><span class="sxs-lookup"><span data-stu-id="b1566-195">Edit the connections</span></span>

1. <span data-ttu-id="b1566-196">Tornare alla pagina Soluzioni e selezionare **Soluzione predefinita**.</span><span class="sxs-lookup"><span data-stu-id="b1566-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="b1566-197">Selezionare **Riferimento alla connessione (anteprima)** facendo clic su **Tutti**.</span><span class="sxs-lookup"><span data-stu-id="b1566-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Iniziare la modifica del connettore":::

2. <span data-ttu-id="b1566-199">Modificare ognuna delle connessioni singolarmente selezionando l'icona con i tre puntini.</span><span class="sxs-lookup"><span data-stu-id="b1566-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="b1566-200">Aggiungere le connessioni pertinenti.</span><span class="sxs-lookup"><span data-stu-id="b1566-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Modificare i connettori":::

3. <span data-ttu-id="b1566-202">Attivare i flussi nella sequenza seguente:</span><span class="sxs-lookup"><span data-stu-id="b1566-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="b1566-203">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b1566-204">Creare segnalazioni di co-selling - Salesforce per Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b1566-205">Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b1566-206">Partner Center a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b1566-207">Da Salesforce a Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b1566-208">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b1566-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b1566-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b1566-210">Usare le API webhook per la registrazione per gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="b1566-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b1566-211">Le PARTNER CENTER webhook consentono di registrarsi per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="b1566-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b1566-212">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="b1566-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b1566-213">Per registrare l'URL, **Partner Center registrazione webhook (Insider Preview)** Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b1566-214">Aggiungere connessioni per (a.) Partner Center utente con credenziali di amministratore delle segnalazioni (b.) Partner Center eventi, come evidenziato di seguito</span><span class="sxs-lookup"><span data-stu-id="b1566-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="b1566-216">Quando si apportano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="b1566-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="b1566-218">Salvare le modifiche e selezionare **Attiva.**</span><span class="sxs-lookup"><span data-stu-id="b1566-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="b1566-219">Per abilitare Partner Center webhook per l'ascolto delle modifiche degli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="b1566-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b1566-220">Selezionare **Partner Center a Salesforce CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="b1566-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b1566-221">Selezionare **l'icona** Modifica e selezionare **Quando viene ricevuta una richiesta HTTP.**</span><span class="sxs-lookup"><span data-stu-id="b1566-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b1566-222">Selezionare **l'icona** Copia per copiare l'URL HTTP POST specificato.</span><span class="sxs-lookup"><span data-stu-id="b1566-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="b1566-224">Selezionare ora il flusso di Partner Center webhook (Insider Preview) Power Automate e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="b1566-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b1566-225">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e selezionare **Continua.**</span><span class="sxs-lookup"><span data-stu-id="b1566-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="b1566-226">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="b1566-226">Enter the following details:</span></span>

    1. <span data-ttu-id="b1566-227">**Endpoint trigger HTTP:** URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="b1566-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="b1566-228">**Eventi da registrare:**"referral-created" e "referral-updated"</span><span class="sxs-lookup"><span data-stu-id="b1566-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="b1566-229">**Sovrascrivi gli endpoint del trigger esistenti se presenti:** Sì (in questo modo vengono sovrascritti tutti gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="b1566-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="b1566-230">Selezionare **Esegui** e quindi Fare **clic su Fine.**</span><span class="sxs-lookup"><span data-stu-id="b1566-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b1566-231">Il webhook può ora restare in ascolto degli eventi di creazione e aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="b1566-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b1566-232">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="b1566-232">Customize synchronization steps</span></span>

<span data-ttu-id="b1566-233">Quando le segnalazioni di co-selling vengono sincronizzate tra Partner Center e il sistema CRM, i campi sincronizzati Partner Center PC sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="b1566-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b1566-234">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="b1566-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b1566-235">È possibile personalizzare i Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b1566-236">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b1566-237">Vengono forniti mapping da Microsoft Partner Center a CRM, ma in base all'ambiente CRM è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="b1566-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b1566-238">È possibile personalizzare più passaggi di Power Automate flusso di lavoro in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="b1566-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b1566-239">Di seguito sono riportati esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="b1566-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b1566-240">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel Partner Center alla sincronizzazione delle segnalazioni di CRM:</span><span class="sxs-lookup"><span data-stu-id="b1566-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="b1566-241">Selezionare Partner Center a Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="b1566-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="b1566-242">Selezionare **Modifica** per modificare/personalizzare il Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="b1566-243">Selezionare **(Ambito) Sincronizzare il lead o l'opportunità.**</span><span class="sxs-lookup"><span data-stu-id="b1566-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b1566-244">Per personalizzare i mapping dei campi CRM per gli eventi di creazione, selezionare Se si tratta di **una nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b1566-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b1566-245">Selezionare il passaggio secondario **in caso affermativa** e quindi espandere **Creazione di una nuova opportunità in CRM.**</span><span class="sxs-lookup"><span data-stu-id="b1566-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b1566-246">È possibile modificare i mapping in questa sezione usando la Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b1566-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="b1566-247">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, selezionare il passaggio "(Ambito) Sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="b1566-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="b1566-248">Selezionare **Se si tratta di un aggiornamento di un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b1566-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b1566-249">Selezionare il sotto step **in caso affermativa** e quindi espandere **If difference between the opportunity objects in Partner Center and CRM (Differenza** tra gli oggetti opportunità in Partner Center CRM), quindi .</span><span class="sxs-lookup"><span data-stu-id="b1566-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="b1566-250">Selezionare **Se sì seguito** da Aggiorna opportunità **esistente**</span><span class="sxs-lookup"><span data-stu-id="b1566-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="b1566-251">Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="b1566-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="b1566-252">Selezionare **Modifica**  per modificare/personalizzare il Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b1566-253">Selezionare **(Ambito) Synchronize the opportunity (Sincronizza l'opportunità).**</span><span class="sxs-lookup"><span data-stu-id="b1566-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="b1566-254">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per gli eventi di aggiornamento, selezionare Se c'è differenza tra gli oggetti lead **in Partner Center e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b1566-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="b1566-255">Selezionare il passaggio secondario **in caso affermativa** e quindi espandere il passaggio **Aggiornare una segnalazione con i dati dell'opportunità.**</span><span class="sxs-lookup"><span data-stu-id="b1566-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="b1566-256">È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b1566-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b1566-257">Per personalizzare i campi per la sincronizzazione delle segnalazioni da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="b1566-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="b1566-258">Selezionare **Modifica**  per modificare/personalizzare il Power Automate flusso.</span><span class="sxs-lookup"><span data-stu-id="b1566-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b1566-259">Selezionare **(Ambito) Synchronizing Referrals (Sincronizzazione delle segnalazioni).**</span><span class="sxs-lookup"><span data-stu-id="b1566-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="b1566-260">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, **selezionare Create Microsoft Referral (Crea segnalazione Microsoft).**</span><span class="sxs-lookup"><span data-stu-id="b1566-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="b1566-261">È possibile modificare i mapping in questa sezione in base alla Guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b1566-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b1566-262">Sincronizzazione delle segnalazioni di co-selling bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="b1566-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b1566-263">Dopo aver installato, configurato e personalizzato la soluzione Power Automate, è possibile testare la sincronizzazione delle segnalazioni di co-selling tra Salesforce CRM e Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b1566-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b1566-264">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="b1566-264">Pre-requisites</span></span>

<span data-ttu-id="b1566-265">Per sincronizzare le segnalazioni tra Partner Center e Salesforce CRM, la soluzione Power Automate deve delimitare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1566-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b1566-266">Questa identificazione offre ai team venditori la possibilità di decidere quali segnalazioni condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="b1566-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b1566-267">Un set di campi personalizzati è disponibile come parte dell'entità opportunità Partner Center di sincronizzazione delle **segnalazioni** per la soluzione Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b1566-268">Un utente amministratore di CRM dovrà creare una sezione CRM separata con i **campi** personalizzati Opportunità.</span><span class="sxs-lookup"><span data-stu-id="b1566-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b1566-269">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="b1566-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b1566-270">**Sincronizza con Partner Center**: indica se sincronizzare l'opportunità con Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="b1566-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b1566-271">**Identificatore di riferimento:** campo dell'identificatore di sola lettura per la segnalazione Partner Center Microsoft</span><span class="sxs-lookup"><span data-stu-id="b1566-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b1566-272">**Collegamento alla segnalazione:** collegamento di sola lettura alla segnalazione in Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="b1566-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b1566-273">**Come può essere utile Microsoft:** Guida necessaria a Microsoft per la segnalazione</span><span class="sxs-lookup"><span data-stu-id="b1566-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b1566-274">**Products**: elenco di prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="b1566-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b1566-275">**Audit:** un'istanza di sola audit trail per la sincronizzazione con Partner Center segnalazioni</span><span class="sxs-lookup"><span data-stu-id="b1566-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b1566-276">Scenari:</span><span class="sxs-lookup"><span data-stu-id="b1566-276">SCENARIOS:</span></span>

1. <span data-ttu-id="b1566-277">Sincronizzazione delle segnalazioni quando la segnalazione viene creata o aggiornata in CRM e sincronizzata in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="b1566-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b1566-278">Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella **sezione Opportunità** di CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b1566-279">Assicurarsi che la sezione seguente sia presente quando si crea una "Nuova opportunità" nell'ambiente Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b1566-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce":::

   3. <span data-ttu-id="b1566-281">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="b1566-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="b1566-282">"Sincronizza con Partner Center": Sì</span><span class="sxs-lookup"><span data-stu-id="b1566-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="b1566-283">"How can Microsoft help?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="b1566-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="b1566-284">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="b1566-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="b1566-285">Dopo aver impostato l'opzione **Sincronizza con Partner Center** su Sì , attendere 10 minuti, accedere all'account Partner Center servizio. </span><span class="sxs-lookup"><span data-stu-id="b1566-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b1566-286">Le segnalazioni verranno sincronizzate con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="b1566-287">Quando l'opzione "Sincronizza con Partner Center" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account Partner Center personale.</span><span class="sxs-lookup"><span data-stu-id="b1566-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="b1566-288">Le opportunità sincronizzate correttamente con Partner Center verranno identificate con ✔icon in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b1566-289">Sincronizzazione dei riferimenti quando la segnalazione viene creata o aggiornata in Microsoft Partner Center sincronizzata nell'ambiente Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="b1566-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="b1566-290">Accedere al [dashboard Partner Center.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="b1566-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="b1566-291">Selezionare **Segnalazioni** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="b1566-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="b1566-292">Creare una nuova segnalazione di co-selling Partner Center facendo clic sull'opzione "Nuova trattativa".</span><span class="sxs-lookup"><span data-stu-id="b1566-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="b1566-293">Accedere all'ambiente Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="b1566-294">Passare a **Open Opportunities (Apri opportunità).**</span><span class="sxs-lookup"><span data-stu-id="b1566-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b1566-295">La segnalazione creata in Microsoft Partner Center è ora sincronizzata in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b1566-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata delle opportunità di Salesforce":::

    6. <span data-ttu-id="b1566-297">Quando si seleziona una segnalazione sincronizzata, i dettagli della visualizzazione scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="b1566-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b1566-298">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b1566-298">Next steps</span></span>

- [<span data-ttu-id="b1566-299">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="b1566-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b1566-300">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="b1566-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b1566-301">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b1566-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
