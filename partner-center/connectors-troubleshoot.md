---
title: Risoluzione dei problemi relativi ai connettori di co-selling
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle risposte alle domande comuni sull'uso dei connettori di co-selling. Leggere le domande frequenti su come risolvere i problemi di co-selling.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354543"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="4f946-104">Risoluzione dei problemi relativi ai connettori di co-selling</span><span class="sxs-lookup"><span data-stu-id="4f946-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="4f946-105">**Si applica a:**</span><span class="sxs-lookup"><span data-stu-id="4f946-105">**Applies to:**</span></span>

- <span data-ttu-id="4f946-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="4f946-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="4f946-107">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="4f946-107">Salesforce CRM</span></span>

<span data-ttu-id="4f946-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="4f946-108">**Appropriate roles**</span></span>

- <span data-ttu-id="4f946-109">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="4f946-109">Referrals admin</span></span>
- <span data-ttu-id="4f946-110">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="4f946-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="4f946-111">Domande e risposte sui prerequisiti</span><span class="sxs-lookup"><span data-stu-id="4f946-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="4f946-112">È possibile usare una soluzione di valutazione per la co-selling dei connettori per l'ambiente?</span><span class="sxs-lookup"><span data-stu-id="4f946-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="4f946-113">Se si utilizza l'ambiente di test/gestione temporanea, è possibile optare per la soluzione di valutazione.</span><span class="sxs-lookup"><span data-stu-id="4f946-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="4f946-114">La versione a pagamento dei connettori è disponibile in AppSource a 15 dollari al mese.</span><span class="sxs-lookup"><span data-stu-id="4f946-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="4f946-115">Con la connessione a pagamento, si otterranno 10.000 chiamate API al giorno.</span><span class="sxs-lookup"><span data-stu-id="4f946-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="4f946-116">I connettori sono wrapper oltre alle API di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="4f946-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="4f946-117">Ogni volta che le soluzioni del connettore vengono eseguite per un evento di **creazione** o **aggiornamento** in caso di opportunità in un centro per i partner o sul lato CRM, viene eseguita una chiamata API.</span><span class="sxs-lookup"><span data-stu-id="4f946-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="4f946-118">Quale ruolo è necessario per creare sezioni nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="4f946-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="4f946-119">Gli utenti che sono amministratori di sistema o personalizzatori di sistema possono applicare modifiche a tutti.</span><span class="sxs-lookup"><span data-stu-id="4f946-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="4f946-120">Tutti gli utenti dell'app, tuttavia, possono personalizzare il sistema e persino condividere alcune delle loro personalizzazioni con altri utenti.</span><span class="sxs-lookup"><span data-stu-id="4f946-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="4f946-121">I venditori partner hanno bisogno di ruoli speciali per lavorare al centro per i partner?</span><span class="sxs-lookup"><span data-stu-id="4f946-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="4f946-122">Ai venditori partner deve essere assegnato il ruolo di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="4f946-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="4f946-123">Per ulteriori informazioni, fare riferimento a [Cenni preliminari sulle autorizzazioni) (Create-User-Accounts-and-set-permissions).</span><span class="sxs-lookup"><span data-stu-id="4f946-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="4f946-124">Quali campi devono essere impostati per primi nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="4f946-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="4f946-125">• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trovi in un ambiente CRM in modo accurato.</span><span class="sxs-lookup"><span data-stu-id="4f946-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="4f946-126">• Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="4f946-127">Quali prerequisiti sono necessari per la creazione dell'ambiente di Power Automatic?</span><span class="sxs-lookup"><span data-stu-id="4f946-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="4f946-128">Per usare l'ambiente Power automatizzate, è necessario quanto segue:</span><span class="sxs-lookup"><span data-stu-id="4f946-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="4f946-129">È necessaria una licenza di Power automatici.</span><span class="sxs-lookup"><span data-stu-id="4f946-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="4f946-130">È necessario almeno 1 GB di spazio di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="4f946-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="4f946-131">È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione connettori Salesforce?</span><span class="sxs-lookup"><span data-stu-id="4f946-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="4f946-132">La soluzione del connettore Salesforce è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="4f946-133">Per la soluzione non è necessario disporre di un'istanza di Dynamics 365 o di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="4f946-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="4f946-134">Durante l'installazione della soluzione Salesforce, può essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda.</span><span class="sxs-lookup"><span data-stu-id="4f946-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="4f946-135">È necessario selezionare l'ambiente.</span><span class="sxs-lookup"><span data-stu-id="4f946-135">You need to select that environment.</span></span> <span data-ttu-id="4f946-136">Inoltre, se si riceve l'errore "non è stato possibile trovare un'organizzazione Dynamics 365 connessa all'utente connesso", sarà necessario creare un nuovo ambiente per il connettore.</span><span class="sxs-lookup"><span data-stu-id="4f946-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="4f946-137">Domande e risposte sulla configurazione</span><span class="sxs-lookup"><span data-stu-id="4f946-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="4f946-138">Cosa si deve fare se si affronta l'errore seguente durante l'attivazione dei flussi nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="4f946-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="4f946-139">Errore: la richiesta di Azure Resource Manager non è riuscita con errore:' {"Error": {"code": "WorkflowTriggerNotFound", "message": "Impossibile trovare il trigger ' manual ' del flusso di lavoro."}}'.</span><span class="sxs-lookup"><span data-stu-id="4f946-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="4f946-140">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="4f946-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="4f946-141">Eliminare la connessione CDS e quindi ricreare le connessioni CDS.</span><span class="sxs-lookup"><span data-stu-id="4f946-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="4f946-142">Attivare e disattivare il flusso figlio</span><span class="sxs-lookup"><span data-stu-id="4f946-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="4f946-143">Eliminare la soluzione e reinstallare la soluzione.</span><span class="sxs-lookup"><span data-stu-id="4f946-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="4f946-144">Cosa si deve fare se si affronta l'errore di "accesso" durante l'aggiunta di un connettore del centro per i partner nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="4f946-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

<span data-ttu-id="4f946-146">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="4f946-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="4f946-147">Usare le credenziali del centro per i partner per accedere all'ambiente Microsoft Flow una volta (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="4f946-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="4f946-148">Cosa è necessario fare se viene visualizzato l'errore seguente quando si attiva il centro per i partner al flusso di CRM nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="4f946-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede aggiornamenti":::

<span data-ttu-id="4f946-150">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="4f946-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="4f946-151">Attivare i seguenti due flussi figlio prima di attivare il centro per i partner al flusso CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="4f946-152">Centro per i partner per CRM-Helper (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="4f946-153">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a CRM (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="4f946-154">Cosa fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?</span><span class="sxs-lookup"><span data-stu-id="4f946-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="4f946-155">Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.</span><span class="sxs-lookup"><span data-stu-id="4f946-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="4f946-156">Se la finestra di dialogo per l'aggiunta di connessioni non viene aperta automaticamente durante la modifica del flusso, è possibile modificare singolarmente i passaggi e i passaggi secondari dei flussi.</span><span class="sxs-lookup"><span data-stu-id="4f946-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="4f946-157">Selezionare ogni flusso e modificarli singolarmente.</span><span class="sxs-lookup"><span data-stu-id="4f946-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="4f946-158">Espandi tutti i passaggi nel flusso</span><span class="sxs-lookup"><span data-stu-id="4f946-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passaggi che richiedono connessioni":::

- <span data-ttu-id="4f946-160">Selezionare i passaggi in cui viene visualizzata un'icona di avviso che richiede di associare le connessioni e di aggiungere connessioni.</span><span class="sxs-lookup"><span data-stu-id="4f946-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modificare il flusso passo per passo":::


5. <span data-ttu-id="4f946-162">Cosa si deve fare se i flussi della soluzione per la co-selling dei connettori per i riferimenti non vengono attivati?</span><span class="sxs-lookup"><span data-stu-id="4f946-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="4f946-163">R.</span><span class="sxs-lookup"><span data-stu-id="4f946-163">A.</span></span> <span data-ttu-id="4f946-164">In Power automatizzate, sarà necessario modificare i flussi nell'ordine seguente e aggiornarli in modo da usare le connessioni corrette:</span><span class="sxs-lookup"><span data-stu-id="4f946-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="4f946-165">Registrazione webhook del centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="4f946-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="4f946-166">Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="4f946-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="4f946-167">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="4f946-168">Da partner Center a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="4f946-169">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="4f946-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="4f946-170">Opportunità di Salesforce per il centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="4f946-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="4f946-171">Salesforce Microsoft Solutions to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="4f946-172">B.</span><span class="sxs-lookup"><span data-stu-id="4f946-172">B.</span></span> <span data-ttu-id="4f946-173">Per ogni flusso, selezionare l'opzione **Esegui solo utenti** .</span><span class="sxs-lookup"><span data-stu-id="4f946-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="4f946-174">Selezionare **Usa connessione** anziché **fornita dall'utente di sola esecuzione**.</span><span class="sxs-lookup"><span data-stu-id="4f946-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Per attivare un flusso":::


<span data-ttu-id="4f946-176">C.</span><span class="sxs-lookup"><span data-stu-id="4f946-176">C.</span></span> <span data-ttu-id="4f946-177">Attivare questi flussi indicati di seguito:</span><span class="sxs-lookup"><span data-stu-id="4f946-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="4f946-178">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="4f946-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="4f946-179">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="4f946-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="4f946-180">D.</span><span class="sxs-lookup"><span data-stu-id="4f946-180">D.</span></span> <span data-ttu-id="4f946-181">Attivare tutti i flussi rimanenti.</span><span class="sxs-lookup"><span data-stu-id="4f946-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="4f946-182">E.</span><span class="sxs-lookup"><span data-stu-id="4f946-182">E.</span></span> <span data-ttu-id="4f946-183">Nella registrazione del webhook del centro per i partner Microsoft Flow selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="4f946-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="4f946-184">Fornire l' **URL http** dalla prima azione nel **centro per i partner al flusso di Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="4f946-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="4f946-185">Selezionare tutte e quattro le opzioni in **eventi da registrare** e selezionare **Sì** per Sovrascrivi.</span><span class="sxs-lookup"><span data-stu-id="4f946-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="4f946-186">Domande e risposte su esecuzione/manutenzione</span><span class="sxs-lookup"><span data-stu-id="4f946-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="4f946-187">Come si risolvono i problemi in caso di errori durante l'esecuzione di Power automatizzare il flusso?</span><span class="sxs-lookup"><span data-stu-id="4f946-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="4f946-188">Per assicurarsi che i flussi vengano eseguiti come previsto e per risolvere gli errori durante l'esecuzione, vedere correggere gli [errori di flusso](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="4f946-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="4f946-189">Cosa è necessario fare se vengono visualizzati riferimenti che non sono sincronizzati correttamente nel centro per i partner o nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="4f946-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="4f946-190">Per determinare lo stato della sincronizzazione dei riferimenti, selezionare **controllo**.</span><span class="sxs-lookup"><span data-stu-id="4f946-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Come sincronizzare i riferimenti":::

<span data-ttu-id="4f946-192">Verificare che siano soddisfatte le condizioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="4f946-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="4f946-193">L'ID soluzione viene fornito come parte dell'opportunità.</span><span class="sxs-lookup"><span data-stu-id="4f946-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="4f946-194">Il codice paese a due lettere è obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="4f946-194">Two letter country code is required.</span></span>

- <span data-ttu-id="4f946-195">Quando la Guida di Microsoft è selezionata per l'opportunità, le informazioni di contatto del cliente sono obbligatorie.</span><span class="sxs-lookup"><span data-stu-id="4f946-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="4f946-196">Come verificare che il riferimento venga sincronizzato in modo bidirezionale?</span><span class="sxs-lookup"><span data-stu-id="4f946-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="4f946-197">Eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="4f946-197">Do the following steps:</span></span>

- <span data-ttu-id="4f946-198">Per i venditori partner è necessario assicurarsi di aver abilitato l'opzione **Sync with partner Center** nella sezione CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Assicurarsi di aver abilitato la sincronizzazione":::

- <span data-ttu-id="4f946-200">I venditori devono fornire i ricavi e la data di chiusura quando qualificano un responsabile.</span><span class="sxs-lookup"><span data-stu-id="4f946-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="4f946-201">Se l'ID CRM viene specificato nella fase di **creazione** o **aggiornamento** dell'opportunità di co-selling, ma non è stata trovata un'opportunità di lead con tale ID in CRM, Update o create verranno ignorate.</span><span class="sxs-lookup"><span data-stu-id="4f946-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="4f946-202">Verificare che il campo valuta referral sia configurato nell'ambiente Salesforce.</span><span class="sxs-lookup"><span data-stu-id="4f946-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="4f946-203">Cosa è necessario fare se il connettore viene disconnesso e non viene eseguita una sincronizzazione dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="4f946-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="4f946-204">Di seguito sono riportate alcune delle opzioni che è possibile provare:</span><span class="sxs-lookup"><span data-stu-id="4f946-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="4f946-205">Controllare se il nome utente o la password è scaduta per l'utente del centro per i partner con i ruoli di amministratore di riferimento.</span><span class="sxs-lookup"><span data-stu-id="4f946-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="4f946-206">È possibile passare all'opportunità non sincronizzata, effettuare un aggiornamento secondario e osservare se il riferimento è stato sincronizzato.</span><span class="sxs-lookup"><span data-stu-id="4f946-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="4f946-207">Se i flussi sono stati eseguiti e non riusciti, selezionare il flusso e inviare di nuovo l'esecuzione che ha avuto esito negativo.</span><span class="sxs-lookup"><span data-stu-id="4f946-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="4f946-208">Cosa si deve fare quando si ricevono errori di accesso negato?</span><span class="sxs-lookup"><span data-stu-id="4f946-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="4f946-209">Verificare che siano presenti i ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="4f946-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="4f946-210">Ruolo di amministratore di riferimento per il venditore del centro partner</span><span class="sxs-lookup"><span data-stu-id="4f946-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="4f946-211">Ruolo di amministratore di sistema o di sistema verbi nell'istanza di CRM</span><span class="sxs-lookup"><span data-stu-id="4f946-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="4f946-212">Assicurarsi che l'utente di Power automatizzare l'accesso https://flow.microsoft.com all'account di flusso almeno una volta in anticipo</span><span class="sxs-lookup"><span data-stu-id="4f946-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="4f946-213">Se si nota che il **codice paese dell'account del cliente** non è presente durante la creazione di un'opportunità di co-selling, cosa si deve fare?</span><span class="sxs-lookup"><span data-stu-id="4f946-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="4f946-214">È necessario aggiungere il codice di paese a due lettere ISO all'account del cliente in CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="4f946-215">Cosa è necessario fare se viene visualizzato l'errore relativo all' **ID della soluzione necessaria** per la creazione di un'opportunità di co-selling?</span><span class="sxs-lookup"><span data-stu-id="4f946-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="4f946-216">Per creare un riferimento di co-selling, è necessaria una soluzione di co-selling per Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4f946-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="4f946-217">Cosa si deve fare quando vengono visualizzate opportunità di co-selling create in Partner Center che non vengono sincronizzate con CRM anche se non sono presenti errori di flusso:</span><span class="sxs-lookup"><span data-stu-id="4f946-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="4f946-218">Eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="4f946-218">Do the following:</span></span>

- <span data-ttu-id="4f946-219">Dopo aver creato una nuova operazione di co-selling nel centro per i partner, verificare che venga richiamato il centro per i partner del flusso di Dynamics 365 (potrebbe essere richiamato più volte).</span><span class="sxs-lookup"><span data-stu-id="4f946-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="4f946-220">Se il flusso viene richiamato, controllare tutti i flussi richiamati e identificare l'esecuzione del flusso che aggiornerà il CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="4f946-221">È possibile seguire le azioni e verificare se il CRM è stato aggiornato o se si è verificato un problema.</span><span class="sxs-lookup"><span data-stu-id="4f946-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="4f946-222">Controllare *New Deal*\* nel centro per i partner per verificare se viene popolato con l'ID CRM.</span><span class="sxs-lookup"><span data-stu-id="4f946-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="4f946-223">Assicurarsi che l'operazione non sia chiusa accidentalmente come "Won" o "Lost" nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="4f946-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4f946-224">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="4f946-224">Next steps</span></span>

- [<span data-ttu-id="4f946-225">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="4f946-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="4f946-226">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="4f946-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
