---
title: Usare i webhook per ottenere gli eventi di modifica delle risorse
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare le API webhook del centro per i partner per apprendere quando si verificano le modifiche delle risorse dei riferimenti per Dynamics 365 CRM o Salesforce CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2335c06d9c410d44ed5f444574d9bc8fb3e48fc0
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434020"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="f3d4a-103">Usare le API webhook per registrare gli eventi di modifica delle risorse per Dynamics 365 CRM e Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f3d4a-103">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f3d4a-104">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="f3d4a-104">Appropriate roles</span></span>

- <span data-ttu-id="f3d4a-105">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="f3d4a-105">Referrals admin</span></span>
- <span data-ttu-id="f3d4a-106">System Admin o System verbi per Dynamics 365 CRM o Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="f3d4a-106">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="f3d4a-107">Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-107">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f3d4a-108">Questi eventi di modifica vengono inviati all'URL come post HTTP.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-108">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="f3d4a-109">Questo argomento illustra le API webhook per Dynamics 365 CRM e Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-109">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="f3d4a-110">Configurare il webhook</span><span class="sxs-lookup"><span data-stu-id="f3d4a-110">Configure the webhook</span></span>

1. <span data-ttu-id="f3d4a-111">Per registrare l'URL, selezionare il flusso di registrazione del webhook per il centro per i **partner (anteprima di insider Preview)** .</span><span class="sxs-lookup"><span data-stu-id="f3d4a-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="f3d4a-112">Aggiungi connessioni per (a) Utente del centro per i partner con credenziali di amministratore di riferimento (b) Eventi del centro per i partner evidenziati di seguito</span><span class="sxs-lookup"><span data-stu-id="f3d4a-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="f3d4a-114">Quando si effettuano questi aggiornamenti, viene visualizzato</span><span class="sxs-lookup"><span data-stu-id="f3d4a-114">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="f3d4a-116">Salvare le modifiche e selezionare **attiva**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-116">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="f3d4a-117">Per consentire ai webhook del centro per i partner di restare in ascolto delle modifiche agli eventi negli oggetti di riferimento di co-selling/indipendenti IP nel centro per i partner e nei sistemi CRM, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="f3d4a-118">Selezionare **centro per i partner per Dynamics 365 (insider Preview)** o **Partner Center a Salesforce (insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="f3d4a-119">Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="f3d4a-120">Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copia l'URL":::

8. <span data-ttu-id="f3d4a-122">Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="f3d4a-123">Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="f3d4a-124">Immettere i dettagli seguenti:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-124">Enter the following details:</span></span>

    1. <span data-ttu-id="f3d4a-125">**Endpoint trigger http**: URL copiato dal passaggio precedente</span><span class="sxs-lookup"><span data-stu-id="f3d4a-125">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="f3d4a-126">**Eventi da registrare**: "riferimento-creato" e "riferimento-aggiornato"</span><span class="sxs-lookup"><span data-stu-id="f3d4a-126">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="f3d4a-127">Sovrascrivi gli **endpoint del trigger esistenti se presenti**: Sì (sovrascrive gli endpoint esistenti).</span><span class="sxs-lookup"><span data-stu-id="f3d4a-127">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="f3d4a-128">Il webhook può ora restare in ascolto delle modifiche (creazione e aggiornamento degli eventi).</span><span class="sxs-lookup"><span data-stu-id="f3d4a-128">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="f3d4a-129">Selezionare **Esegui** , quindi fare clic su **fine.**</span><span class="sxs-lookup"><span data-stu-id="f3d4a-129">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f3d4a-130">Personalizzare i passaggi di sincronizzazione</span><span class="sxs-lookup"><span data-stu-id="f3d4a-130">Customize synchronization steps</span></span>

<span data-ttu-id="f3d4a-131">Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati qui.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-131">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="f3d4a-132">Spesso i sistemi CRM sono altamente personalizzati.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-132">Often CRM systems are highly customized.</span></span> <span data-ttu-id="f3d4a-133">È possibile personalizzare i flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-133">You can customize the Power Automate flows.</span></span> <span data-ttu-id="f3d4a-134">Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate nei passaggi dei flussi di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-134">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="f3d4a-135">Sono disponibili i mapping del centro per i partner Microsoft per CRM, ma in base all'ambiente CRM, è possibile scegliere di personalizzare ulteriormente i campi.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-135">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="f3d4a-136">È possibile personalizzare più passaggi di ognuno dei flussi di Power automatizzati in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-136">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="f3d4a-137">Di seguito sono riportati alcuni esempi di personalizzazioni disponibili:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-137">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="f3d4a-138">Per personalizzare i campi per gli eventi di creazione o aggiornamento nel centro per i partner per la sincronizzazione dei riferimenti CRM:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-138">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="f3d4a-139">Selezionare Centro per i partner per Dynamics 365 (insider Preview) o partner Center a Salesforce (insider Preview).</span><span class="sxs-lookup"><span data-stu-id="f3d4a-139">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="f3d4a-140">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-140">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="f3d4a-141">Selezionare **(ambito) sincronizzare il lead o l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-141">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="f3d4a-142">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per la creazione di eventi, selezionare **se è nuova opportunità condivisa, quindi**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-142">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="f3d4a-143">Selezionare il sottopassaggio **se sì** , quindi espandere **creazione di una nuova opportunità in CRM**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-143">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="f3d4a-144">È possibile modificare i mapping in questa sezione usando la guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-144">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="f3d4a-145">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, fare clic sul passaggio "(ambito) sincronizzare il lead o l'opportunità".</span><span class="sxs-lookup"><span data-stu-id="f3d4a-145">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="f3d4a-146">Selezionare **se è un aggiornamento a un'opportunità, quindi**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-146">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="f3d4a-147">Selezionare il sottopassaggio **se sì** , quindi espandere **if difference between the opportunity Objects in Partner Center and CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-147">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="f3d4a-148">Selezionare **se sì** seguito da **Aggiorna opportunità esistente**</span><span class="sxs-lookup"><span data-stu-id="f3d4a-148">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="f3d4a-149">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per gli eventi di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-149">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="f3d4a-150">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-150">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f3d4a-151">Selezionare **(ambito) sincronizzare l'opportunità**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-151">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="f3d4a-152">Per personalizzare i mapping dei campi CRM (in base alla guida per i mapping dei campi) per gli eventi di aggiornamento, selezionare **se esiste una differenza tra gli oggetti lead nel centro per i partner e CRM, quindi**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-152">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="f3d4a-153">Selezionare il sottopassaggio **se sì** , quindi espandere il passaggio **aggiornare un riferimento con i dati di opportunità**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-153">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="f3d4a-154">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-154">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="f3d4a-155">Per personalizzare i campi per la sincronizzazione dei riferimenti da CRM a PC per la creazione di eventi?</span><span class="sxs-lookup"><span data-stu-id="f3d4a-155">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="f3d4a-156">Selezionare **modifica** per modificare/personalizzare il flusso di automazione dell'alimentazione.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-156">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="f3d4a-157">Selezionare **(ambito) sincronizzare i riferimenti.**</span><span class="sxs-lookup"><span data-stu-id="f3d4a-157">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="f3d4a-158">Per personalizzare i mapping dei campi CRM (in base alla guida ai mapping dei campi) per la creazione di eventi, selezionare **Crea riferimento Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-158">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="f3d4a-159">È possibile modificare i mapping in questa sezione in base alla guida al mapping dei campi.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-159">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="f3d4a-160">Sincronizzazione del riferimento bidirezionale end-to-end</span><span class="sxs-lookup"><span data-stu-id="f3d4a-160">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="f3d4a-161">Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile eseguire il test per la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 o Salesforce e centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-161">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f3d4a-162">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="f3d4a-162">Pre-requisites</span></span>

<span data-ttu-id="f3d4a-163">Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM o nel centro per i partner e Salesforce CRM, la soluzione Power automatizzate deve demarcare chiaramente i campi di riferimento specifici di Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-163">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="f3d4a-164">In questo modo, i team dei venditori possono decidere quali riferimenti condividere con Microsoft per il co-selling.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-164">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f3d4a-165">Un set di campi personalizzati è disponibile come parte della sincronizzazione dei riferimenti del centro per i partner per l'entità di **opportunità** della soluzione Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-165">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="f3d4a-166">Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .</span><span class="sxs-lookup"><span data-stu-id="f3d4a-166">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f3d4a-167">I campi personalizzati seguenti devono far parte della sezione CRM:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-167">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f3d4a-168">**Sincronizzare con il centro**per i partner: se sincronizzare l'opportunità con il centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="f3d4a-168">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="f3d4a-169">**Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="f3d4a-169">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f3d4a-170">**Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft</span><span class="sxs-lookup"><span data-stu-id="f3d4a-170">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="f3d4a-171">In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento</span><span class="sxs-lookup"><span data-stu-id="f3d4a-171">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="f3d4a-172">**Prodotti**: elenco dei prodotti associati a questa opportunità</span><span class="sxs-lookup"><span data-stu-id="f3d4a-172">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="f3d4a-173">**Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="f3d4a-173">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="f3d4a-174">SCENARI</span><span class="sxs-lookup"><span data-stu-id="f3d4a-174">SCENARIOS:</span></span>

1. <span data-ttu-id="f3d4a-175">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-175">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f3d4a-176">Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-176">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f3d4a-177">Assicurarsi che la sezione seguente sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f3d4a-177">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Opportunità":::

   3. <span data-ttu-id="f3d4a-179">Per sincronizzare questa opportunità con Microsoft Partner Center, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-179">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="f3d4a-180">**Sincronizza con il centro per i partner**: Sì</span><span class="sxs-lookup"><span data-stu-id="f3d4a-180">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="f3d4a-181">**Come può essere utile Microsoft?**: selezionare una delle opzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-181">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Selezioni della Guida":::

      - <span data-ttu-id="f3d4a-183">**Prodotti**: ID soluzione del prodotto</span><span class="sxs-lookup"><span data-stu-id="f3d4a-183">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="f3d4a-184">Dopo aver creato l'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su **Sì**, attendere 10 minuti, accedere all'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-184">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="f3d4a-185">I riferimenti verranno sincronizzati con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-185">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="f3d4a-186">Di conseguenza, per un'opportunità con l'opzione "Sincronizza con il centro per i partner" impostata su "Sì", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-186">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="f3d4a-187">Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-187">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="f3d4a-188">Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="f3d4a-188">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="f3d4a-189">Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-189">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="f3d4a-190">Selezionare **riferimenti** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-190">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="f3d4a-191">Per creare un nuovo riferimento di co-selling dal centro per i partner, fare clic sull'opzione "nuovo affare".</span><span class="sxs-lookup"><span data-stu-id="f3d4a-191">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="f3d4a-192">Accedere al proprio ambiente Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-192">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="f3d4a-193">Passare a **Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-193">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f3d4a-194">Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-194">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="f3d4a-195">Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.</span><span class="sxs-lookup"><span data-stu-id="f3d4a-195">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f3d4a-196">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="f3d4a-196">Next steps</span></span>

- [<span data-ttu-id="f3d4a-197">Altre informazioni sulla piattaforma Microsoft Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="f3d4a-197">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="f3d4a-198">Eventi webhook del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="f3d4a-198">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="f3d4a-199">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="f3d4a-199">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f3d4a-200">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="f3d4a-200">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
