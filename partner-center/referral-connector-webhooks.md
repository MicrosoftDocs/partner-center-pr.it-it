---
title: Usare i webhook per ottenere gli eventi di modifica delle risorse
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare le API webhook per scoprire quando si verificano modifiche alle risorse dei riferimenti
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: riferimenti, API webhook, eventi di modifica delle risorse
ms.localizationpriority: medium
ms.openlocfilehash: 4e1eb2e9bd8ceb4f8c4bf43684305504c8594e5c
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145085"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b9463-104">Usare le API webhook per registrare gli eventi di modifica delle risorse</span><span class="sxs-lookup"><span data-stu-id="b9463-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="b9463-105">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="b9463-105">Appropriate roles</span></span>

- <span data-ttu-id="b9463-106">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="b9463-106">Referrals admin</span></span>
- <span data-ttu-id="b9463-107">System Admin o System verbi per Dynamics 365 CRM o Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b9463-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="b9463-108">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="b9463-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b9463-109">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="b9463-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="b9463-110">Questo argomento illustra le API webhook per Dynamics 365 CRM e Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="b9463-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="b9463-111">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="b9463-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b9463-112">Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito</span><span class="sxs-lookup"><span data-stu-id="b9463-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Trigger](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="b9463-114">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="b9463-114">When you make these updates, you will see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="b9463-116">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="b9463-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="b9463-117">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi negli oggetti di riferimento di co-selling/indipendenti IP nel centro per i partner e nei sistemi CRM, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="b9463-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="b9463-118">Selezionare **centro per i partner per Dynamics 365 (insider Preview)** o **Partner Center a Salesforce (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="b9463-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="b9463-119">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="b9463-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b9463-120">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="b9463-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copia l'URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="b9463-122">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="b9463-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b9463-123">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="b9463-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="b9463-124">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="b9463-124">Enter the following details:</span></span> 

    <span data-ttu-id="b9463-125">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-125">a.</span></span> <span data-ttu-id="b9463-126">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="b9463-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="b9463-127">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-127">b.</span></span> <span data-ttu-id="b9463-128">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="b9463-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="b9463-129">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-129">c.</span></span> <span data-ttu-id="b9463-130">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="b9463-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="b9463-131">Il webhook può ora restare in ascolto delle modifiche (creazione e aggiornamento degli eventi).</span><span class="sxs-lookup"><span data-stu-id="b9463-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="b9463-132">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="b9463-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="b9463-133">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="b9463-133">Customize synchronization steps</span></span>

<span data-ttu-id="b9463-134">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="b9463-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b9463-135">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="b9463-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b9463-136">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="b9463-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b9463-137">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="b9463-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b9463-138">Sono disponibili i mapping del centro per i partner Microsoft per CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="b9463-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b9463-139">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="b9463-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b9463-140">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="b9463-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b9463-141">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="b9463-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="b9463-142">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-142">a.</span></span> <span data-ttu-id="b9463-143">Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="b9463-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="b9463-144">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-144">b.</span></span> <span data-ttu-id="b9463-145">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="b9463-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="b9463-146">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-146">c.</span></span> <span data-ttu-id="b9463-147">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="b9463-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b9463-148">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b9463-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b9463-149">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="b9463-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b9463-150">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b9463-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="b9463-151">d.</span><span class="sxs-lookup"><span data-stu-id="b9463-151">d.</span></span> <span data-ttu-id="b9463-152">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="b9463-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="b9463-153">e.</span><span class="sxs-lookup"><span data-stu-id="b9463-153">e.</span></span> <span data-ttu-id="b9463-154">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b9463-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b9463-155">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b9463-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="b9463-156">f.</span><span class="sxs-lookup"><span data-stu-id="b9463-156">f.</span></span> <span data-ttu-id="b9463-157">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="b9463-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="b9463-158">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="b9463-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="b9463-159">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-159">a.</span></span> <span data-ttu-id="b9463-160">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="b9463-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="b9463-161">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-161">b.</span></span> <span data-ttu-id="b9463-162">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="b9463-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="b9463-163">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-163">c.</span></span> <span data-ttu-id="b9463-164">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="b9463-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="b9463-165">d.</span><span class="sxs-lookup"><span data-stu-id="b9463-165">d.</span></span> <span data-ttu-id="b9463-166">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="b9463-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="b9463-167">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b9463-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b9463-168">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="b9463-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="b9463-169">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-169">a.</span></span> <span data-ttu-id="b9463-170">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="b9463-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="b9463-171">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-171">b.</span></span> <span data-ttu-id="b9463-172">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="b9463-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="b9463-173">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-173">c.</span></span> <span data-ttu-id="b9463-174">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="b9463-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="b9463-175">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="b9463-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b9463-176">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="b9463-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="b9463-177">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile eseguire il test per la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 o Salesforce e centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b9463-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b9463-178">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="b9463-178">Pre-requisites</span></span>

<span data-ttu-id="b9463-179">Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM o nel centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b9463-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b9463-180">In questo modo, i team dei venditori possono decidere quali riferimenti condividere con Microsoft per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="b9463-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b9463-181">Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b9463-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="b9463-182">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="b9463-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b9463-183">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="b9463-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b9463-184">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="b9463-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b9463-185">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="b9463-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b9463-186">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="b9463-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b9463-187">In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="b9463-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b9463-188">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="b9463-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b9463-189">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b9463-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b9463-190">SCENARI</span><span class="sxs-lookup"><span data-stu-id="b9463-190">SCENARIOS:</span></span>

1. <span data-ttu-id="b9463-191">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="b9463-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="b9463-192">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-192">a.</span></span> <span data-ttu-id="b9463-193">Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="b9463-193">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="b9463-194">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-194">b.</span></span> <span data-ttu-id="b9463-195">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b9463-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Opportunità](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="b9463-197">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-197">c.</span></span> <span data-ttu-id="b9463-198">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="b9463-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="b9463-199">"Sincronizza con il centro per i partner": Sì</span><span class="sxs-lookup"><span data-stu-id="b9463-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="b9463-200">"Come può essere utile Microsoft?": selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="b9463-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![Selezioni della Guida](images/cosellconnectors/help.png)

    - <span data-ttu-id="b9463-202">Prodotti: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="b9463-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="b9463-203">d.</span><span class="sxs-lookup"><span data-stu-id="b9463-203">d.</span></span> <span data-ttu-id="b9463-204">Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b9463-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b9463-205">I riferimenti verranno sincronizzati con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b9463-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="b9463-206">e.</span><span class="sxs-lookup"><span data-stu-id="b9463-206">e.</span></span> <span data-ttu-id="b9463-207">Di conseguenza, per un'opportunità con l'opzione "Sincronizza con il centro per i partner" impostata su "Sì", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b9463-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="b9463-208">f.</span><span class="sxs-lookup"><span data-stu-id="b9463-208">f.</span></span> <span data-ttu-id="b9463-209">Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="b9463-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="b9463-210">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="b9463-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="b9463-211">a.</span><span class="sxs-lookup"><span data-stu-id="b9463-211">a.</span></span> <span data-ttu-id="b9463-212">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="b9463-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="b9463-213">b.</span><span class="sxs-lookup"><span data-stu-id="b9463-213">b.</span></span> <span data-ttu-id="b9463-214">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="b9463-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="b9463-215">c.</span><span class="sxs-lookup"><span data-stu-id="b9463-215">c.</span></span> <span data-ttu-id="b9463-216">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="b9463-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="b9463-217">d.</span><span class="sxs-lookup"><span data-stu-id="b9463-217">d.</span></span> <span data-ttu-id="b9463-218">Accedere al proprio ambiente Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="b9463-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="b9463-219">e.</span><span class="sxs-lookup"><span data-stu-id="b9463-219">e.</span></span> <span data-ttu-id="b9463-220">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="b9463-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b9463-221">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="b9463-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="b9463-222">f.</span><span class="sxs-lookup"><span data-stu-id="b9463-222">f.</span></span> <span data-ttu-id="b9463-223">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="b9463-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="b9463-224">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b9463-224">Next steps</span></span>

- [<span data-ttu-id="b9463-225">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="b9463-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="b9463-226">Eventi webhook del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="b9463-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="b9463-227">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="b9463-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b9463-228">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="b9463-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
