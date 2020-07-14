---
title: Connettore di co-selling per Salesforce CRM Partner Center
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con Salesforce CRM
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 0a22587f5b555281cae6f557acfc2695ba92727e
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302378"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="dba9e-103">Connettore di co-selling per CRM Salesforce - Panoramica</span><span class="sxs-lookup"><span data-stu-id="dba9e-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="dba9e-104">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="dba9e-104">Appropriate roles</span></span>

- <span data-ttu-id="dba9e-105">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="dba9e-105">Referrals admin</span></span>
- <span data-ttu-id="dba9e-106">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="dba9e-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="dba9e-107">Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="dba9e-108">Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="dba9e-109">Utilizzando i connettori di co-selling, è possibile creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare o rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura.</span><span class="sxs-lookup"><span data-stu-id="dba9e-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="dba9e-110">È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="dba9e-111">È possibile eseguire tutte le attività di riferimento quando si lavora all'interno del CRM scelto piuttosto che nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="dba9e-112">La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="dba9e-113">Prima di installare-prerequisiti</span><span class="sxs-lookup"><span data-stu-id="dba9e-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="dba9e-114">**Argomenti**</span><span class="sxs-lookup"><span data-stu-id="dba9e-114">**Topics**</span></span>   |<span data-ttu-id="dba9e-115">**Dettagli**</span><span class="sxs-lookup"><span data-stu-id="dba9e-115">**Details**</span></span>   |<span data-ttu-id="dba9e-116">**Collegamenti**</span><span class="sxs-lookup"><span data-stu-id="dba9e-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="dba9e-117">ID Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="dba9e-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="dba9e-118">È necessario un ID MPN valido</span><span class="sxs-lookup"><span data-stu-id="dba9e-118">You need a valid MPN ID</span></span>|<span data-ttu-id="dba9e-119">Per aggiungere [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="dba9e-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="dba9e-120">Co-selling pronto</span><span class="sxs-lookup"><span data-stu-id="dba9e-120">Co-sell ready</span></span>|<span data-ttu-id="dba9e-121">La soluzione IP/servizi deve essere pronta per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="dba9e-122">Vendi con Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="dba9e-123">Account del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-123">Partner Center account</span></span>|<span data-ttu-id="dba9e-124">L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="dba9e-125">Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="dba9e-126">Gestire l'account</span><span class="sxs-lookup"><span data-stu-id="dba9e-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="dba9e-127">Ruoli utente del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-127">Partner Center user roles</span></span>|<span data-ttu-id="dba9e-128">Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti</span><span class="sxs-lookup"><span data-stu-id="dba9e-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="dba9e-129">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="dba9e-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="dba9e-130">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="dba9e-130">Salesforce CRM</span></span>|<span data-ttu-id="dba9e-131">Il ruolo utente CRM è amministratore sistema o sistema verbi</span><span class="sxs-lookup"><span data-stu-id="dba9e-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="dba9e-132">Assegnare ruoli in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="dba9e-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="dba9e-133">Power automatizzare l'account di flusso</span><span class="sxs-lookup"><span data-stu-id="dba9e-133">Power Automate Flow Account</span></span>|<span data-ttu-id="dba9e-134">Un account di [Power automatici](https://flow.microsoft.com) attivo per l'amministratore del sistema CRM o verbi di sistema.</span><span class="sxs-lookup"><span data-stu-id="dba9e-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="dba9e-135">L'utente deve accedere a [Power Automate](https://flow.microsoft.com) almeno una volta prima dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="dba9e-136">Installare la sincronizzazione dei riferimenti del centro per i partner per Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="dba9e-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="dba9e-137">Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="dba9e-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="dba9e-138">Vengono visualizzate le istanze di CRM disponibili.</span><span class="sxs-lookup"><span data-stu-id="dba9e-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="dba9e-139">Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.</span><span class="sxs-lookup"><span data-stu-id="dba9e-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="dba9e-140">Selezionare **soluzioni** sulla barra di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="dba9e-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="dba9e-141">Fare clic sul collegamento **Apri AppSource** nel menu in alto.</span><span class="sxs-lookup"><span data-stu-id="dba9e-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. <span data-ttu-id="dba9e-143">Cercare **connettori per i riferimenti del centro per i partner per Salesforce** nella schermata popup.</span><span class="sxs-lookup"><span data-stu-id="dba9e-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="dba9e-145">Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="dba9e-146">Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente Salesforce CRM per installare l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="dba9e-147">Accettare i termini e le condizioni.</span><span class="sxs-lookup"><span data-stu-id="dba9e-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="DISPONGONO disponibili":::

8. <span data-ttu-id="dba9e-149">Si viene quindi reindirizzati alla pagina **Gestisci soluzioni** .</span><span class="sxs-lookup"><span data-stu-id="dba9e-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="dba9e-150">Passare a "centro per i partner" usando i pulsanti freccia nella parte inferiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="dba9e-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="dba9e-151">L' **installazione pianificata** verrà visualizzata accanto alla soluzione di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="dba9e-152">L'installazione può richiedere 10-15 minuti.</span><span class="sxs-lookup"><span data-stu-id="dba9e-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="dba9e-153">Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra.</span><span class="sxs-lookup"><span data-stu-id="dba9e-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="dba9e-154">Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Salesforce** è disponibile nell'elenco soluzioni.</span><span class="sxs-lookup"><span data-stu-id="dba9e-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="dba9e-155">Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="dba9e-156">Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:</span><span class="sxs-lookup"><span data-stu-id="dba9e-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Flussi di Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="dba9e-158">Procedura consigliata: testare prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="dba9e-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="dba9e-159">Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.</span><span class="sxs-lookup"><span data-stu-id="dba9e-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="dba9e-160">Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="dba9e-161">Creare una copia della soluzione ed eseguire la configurazione e Power automatizzare le personalizzazioni dei flussi nell'ambiente di gestione temporanea.</span><span class="sxs-lookup"><span data-stu-id="dba9e-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="dba9e-162">Testare la soluzione in un'istanza di staging/CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="dba9e-163">In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="dba9e-164">Configurare la soluzione</span><span class="sxs-lookup"><span data-stu-id="dba9e-164">Configure the solution</span></span>

1. <span data-ttu-id="dba9e-165">Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="dba9e-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="dba9e-166">Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.</span><span class="sxs-lookup"><span data-stu-id="dba9e-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="dba9e-167">Sarà necessario creare connessioni che associano i tre account utente:</span><span class="sxs-lookup"><span data-stu-id="dba9e-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="dba9e-168">Utente del centro per i partner con credenziali di amministratore per i riferimenti</span><span class="sxs-lookup"><span data-stu-id="dba9e-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="dba9e-169">Eventi del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-169">Partner Center Events</span></span>
   - <span data-ttu-id="dba9e-170">L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="dba9e-171">Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="dba9e-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="dba9e-172">Creare una connessione facendo clic su **Crea una connessione**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Creare la connessione":::

   3. <span data-ttu-id="dba9e-174">Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.</span><span class="sxs-lookup"><span data-stu-id="dba9e-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="dba9e-175">Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="dba9e-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="dba9e-176">Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="dba9e-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="dba9e-177">Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="dba9e-178">Per associare i flussi di automazione dell'alimentazione con le connessioni, modificare ognuno dei flussi di automazione dell'alimentazione per connettersi a Common Data Service e ai riferimenti del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="dba9e-179">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="dba9e-179">Save the changes.</span></span>

5. <span data-ttu-id="dba9e-180">**Attivare** i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="dba9e-181">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="dba9e-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="dba9e-182">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="dba9e-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="dba9e-183">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="dba9e-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="dba9e-184">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="dba9e-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="dba9e-185">Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito</span><span class="sxs-lookup"><span data-stu-id="dba9e-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="dba9e-187">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="dba9e-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="dba9e-189">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="dba9e-190">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="dba9e-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="dba9e-191">Selezionare **centro per i partner per Salesforce CRM (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="dba9e-192">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="dba9e-193">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="dba9e-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="dba9e-195">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="dba9e-196">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="dba9e-197">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="dba9e-197">Enter the following details:</span></span>

    1. <span data-ttu-id="dba9e-198">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="dba9e-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="dba9e-199">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="dba9e-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="dba9e-200">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="dba9e-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="dba9e-201">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="dba9e-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="dba9e-202">Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.</span><span class="sxs-lookup"><span data-stu-id="dba9e-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="dba9e-203">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="dba9e-203">Customize synchronization steps</span></span>

<span data-ttu-id="dba9e-204">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="dba9e-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="dba9e-205">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="dba9e-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="dba9e-206">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="dba9e-207">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="dba9e-208">Sono disponibili i centri partner Microsoft per i mapping CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="dba9e-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="dba9e-209">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="dba9e-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="dba9e-210">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="dba9e-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="dba9e-211">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="dba9e-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="dba9e-212">Selezionare Centro per i partner per Salesforce CRM (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="dba9e-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="dba9e-213">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="dba9e-214">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="dba9e-215">Per personalizzare i mapping dei campi CRM per creare eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="dba9e-216">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="dba9e-217">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="dba9e-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="dba9e-218">Per personalizzare i mapping dei campi CRM per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="dba9e-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="dba9e-219">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="dba9e-220">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="dba9e-221">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="dba9e-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="dba9e-222">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="dba9e-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="dba9e-223">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="dba9e-224">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="dba9e-225">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="dba9e-226">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="dba9e-227">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="dba9e-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="dba9e-228">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="dba9e-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="dba9e-229">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="dba9e-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="dba9e-230">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="dba9e-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="dba9e-231">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="dba9e-232">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="dba9e-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="dba9e-233">Creare una sezione separata nel layout delle opportunità di Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="dba9e-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="dba9e-234">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dba9e-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="dba9e-235">In questo modo, i team dei venditori possono decidere quali riferimenti condividere con Microsoft per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="dba9e-236">Un set di campi personalizzati è disponibile nell'ambito della sincronizzazione dei riferimenti del centro per i partner per **Salesforce CRM.**</span><span class="sxs-lookup"><span data-stu-id="dba9e-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="dba9e-237">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="dba9e-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="dba9e-238">L'utente amministratore di Salesforce CRM dovrà creare una sezione CRM separata.</span><span class="sxs-lookup"><span data-stu-id="dba9e-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="dba9e-239">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="dba9e-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="dba9e-240">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="dba9e-241">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="dba9e-242">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="dba9e-243">**Come può essere utile Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="dba9e-243">**How can Microsoft help?**</span></span> <span data-ttu-id="dba9e-244">Guida richiesta da Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="dba9e-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="dba9e-245">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="dba9e-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="dba9e-246">**Controllo**: audit trail di sola lettura per la sincronizzazione con il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="dba9e-247">Configurare campi e relazioni</span><span class="sxs-lookup"><span data-stu-id="dba9e-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="dba9e-248">Accedere all'account di Salesforce e passare a **opportunità**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="dba9e-249">Fare clic sulle opzioni **installazione** e **modifica oggetto** per aggiungere i campi necessari.</span><span class="sxs-lookup"><span data-stu-id="dba9e-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="dba9e-250">Selezionare i **campi & le relazioni** dal percorso di spostamento a sinistra</span><span class="sxs-lookup"><span data-stu-id="dba9e-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="dba9e-252">Aggiungere i campi seguenti nei **campi &** tabella delle relazioni:</span><span class="sxs-lookup"><span data-stu-id="dba9e-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="dba9e-253">**Etichetta campo**</span><span class="sxs-lookup"><span data-stu-id="dba9e-253">**Field label**</span></span>   |<span data-ttu-id="dba9e-254">**Nome campo**</span><span class="sxs-lookup"><span data-stu-id="dba9e-254">**Field name**</span></span>|<span data-ttu-id="dba9e-255">**Tipo di dati**</span><span class="sxs-lookup"><span data-stu-id="dba9e-255">**Data type**</span></span>|<span data-ttu-id="dba9e-256">**Indicizzata**</span><span class="sxs-lookup"><span data-stu-id="dba9e-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="dba9e-257">Audit</span><span class="sxs-lookup"><span data-stu-id="dba9e-257">Audit</span></span>| <span data-ttu-id="dba9e-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="dba9e-258">Audit__c</span></span>|<span data-ttu-id="dba9e-259">Area di testo lungo (100.000) (riga visibile 4)</span><span class="sxs-lookup"><span data-stu-id="dba9e-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="dba9e-260">Come può essere utile Microsoft?</span><span class="sxs-lookup"><span data-stu-id="dba9e-260">How can Microsoft help?</span></span>|<span data-ttu-id="dba9e-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="dba9e-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="dba9e-262">Picklist</span><span class="sxs-lookup"><span data-stu-id="dba9e-262">Picklist\*</span></span>|
   |<span data-ttu-id="dba9e-263">Prodotti</span><span class="sxs-lookup"><span data-stu-id="dba9e-263">Products</span></span>|<span data-ttu-id="dba9e-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="dba9e-264">Products_c</span></span>|<span data-ttu-id="dba9e-265">testo (255)</span><span class="sxs-lookup"><span data-stu-id="dba9e-265">text (255)</span></span>||
   |<span data-ttu-id="dba9e-266">Referral</span><span class="sxs-lookup"><span data-stu-id="dba9e-266">Referral</span></span> | <span data-ttu-id="dba9e-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="dba9e-267">Referral_Identfier_c</span></span>|<span data-ttu-id="dba9e-268">Testo (100) (ID esterno)</span><span class="sxs-lookup"><span data-stu-id="dba9e-268">Text(100)(External ID)</span></span>|<span data-ttu-id="dba9e-269">sì</span><span class="sxs-lookup"><span data-stu-id="dba9e-269">yes</span></span>|
   |<span data-ttu-id="dba9e-270">Collegamento di riferimento</span><span class="sxs-lookup"><span data-stu-id="dba9e-270">Referral Link</span></span>| <span data-ttu-id="dba9e-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="dba9e-271">Referral_Link_c_</span></span>|<span data-ttu-id="dba9e-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="dba9e-272">URL(255)</span></span>||
   |<span data-ttu-id="dba9e-273">Sincronizza con il centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-273">Sync with Partner Center</span></span>|<span data-ttu-id="dba9e-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="dba9e-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="dba9e-275">CheckBox (impostazione predefinita deselezionata)</span><span class="sxs-lookup"><span data-stu-id="dba9e-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="dba9e-276">\* Valori elenco a discesa:</span><span class="sxs-lookup"><span data-stu-id="dba9e-276">\*Picklist values:</span></span>

   - <span data-ttu-id="dba9e-277">Proposta di valore specifico del carico di lavoro</span><span class="sxs-lookup"><span data-stu-id="dba9e-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="dba9e-278">Architettura tecnica del cliente</span><span class="sxs-lookup"><span data-stu-id="dba9e-278">Customer technical architecture</span></span>
   - <span data-ttu-id="dba9e-279">Modello di prova o demo</span><span class="sxs-lookup"><span data-stu-id="dba9e-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="dba9e-280">Virgolette o licenze</span><span class="sxs-lookup"><span data-stu-id="dba9e-280">Quotes or licensing</span></span>
   - <span data-ttu-id="dba9e-281">Successo del cliente dopo vendite</span><span class="sxs-lookup"><span data-stu-id="dba9e-281">Post sales customer success</span></span>
   - <span data-ttu-id="dba9e-282">Generale o altro</span><span class="sxs-lookup"><span data-stu-id="dba9e-282">General or other</span></span>

5. <span data-ttu-id="dba9e-283">I campi vengono creati in **campi & relazioni**</span><span class="sxs-lookup"><span data-stu-id="dba9e-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Campi creati":::

6. <span data-ttu-id="dba9e-285">Nel layout opportunity creare una sezione separata con i campi elencati sopra.</span><span class="sxs-lookup"><span data-stu-id="dba9e-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="dba9e-286">Questa sezione dovrebbe essere disponibile per i venditori nel layout opportunità</span><span class="sxs-lookup"><span data-stu-id="dba9e-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Layout di campi del centro per i partner":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="dba9e-288">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="dba9e-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="dba9e-289">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Salesforce CRM e il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="dba9e-290">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="dba9e-290">Pre-requisites</span></span>

<span data-ttu-id="dba9e-291">Per sincronizzare i riferimenti tra il centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dba9e-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="dba9e-292">Questa identificazione consente ai team dei venditori di decidere quali riferimenti desiderano condividere con Microsoft per la co-selling.</span><span class="sxs-lookup"><span data-stu-id="dba9e-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="dba9e-293">Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="dba9e-294">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="dba9e-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="dba9e-295">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="dba9e-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="dba9e-296">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="dba9e-297">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="dba9e-298">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="dba9e-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="dba9e-299">**Come è possibile eseguire la Guida Microsoft**per informazioni su come richiedere Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="dba9e-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="dba9e-300">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="dba9e-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="dba9e-301">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="dba9e-302">SCENARI</span><span class="sxs-lookup"><span data-stu-id="dba9e-302">SCENARIOS:</span></span>

1. <span data-ttu-id="dba9e-303">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="dba9e-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="dba9e-304">Accedere all'ambiente Salesforce CRM con l'utente che ha visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="dba9e-305">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="dba9e-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Ambiente Salesforce":::

   3. <span data-ttu-id="dba9e-307">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="dba9e-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="dba9e-308">"Sincronizza con il centro per i partner": Sì</span><span class="sxs-lookup"><span data-stu-id="dba9e-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="dba9e-309">"Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="dba9e-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="dba9e-310">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="dba9e-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="dba9e-311">Dopo aver impostato l'opzione opportunity **Sync with partner Center** su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="dba9e-312">I riferimenti verranno sincronizzati con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="dba9e-313">Quando l'opzione "Sincronizza con il centro per i partner" è impostata su "Sì", se si aggiorna l'opportunità in Salesforce CRM, le modifiche verranno sincronizzate con l'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="dba9e-314">Le opportunità che vengono sincronizzate correttamente con partner Center verranno identificate con ✔ icona in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="dba9e-315">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="dba9e-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="dba9e-316">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="dba9e-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="dba9e-317">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="dba9e-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="dba9e-318">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="dba9e-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="dba9e-319">Accedere all'ambiente Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="dba9e-320">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="dba9e-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="dba9e-321">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="dba9e-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Schermata di opportunità di Salesforce":::

    6. <span data-ttu-id="dba9e-323">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="dba9e-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dba9e-324">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="dba9e-324">Next steps</span></span>

- [<span data-ttu-id="dba9e-325">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="dba9e-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="dba9e-326">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="dba9e-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="dba9e-327">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="dba9e-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="dba9e-328">Webhook del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="dba9e-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)