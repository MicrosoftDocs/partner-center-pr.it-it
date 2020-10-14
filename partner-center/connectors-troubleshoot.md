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
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031264"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="49756-104">Risoluzione dei problemi relativi ai connettori di co-selling</span><span class="sxs-lookup"><span data-stu-id="49756-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="49756-105">**Si applica a:**</span><span class="sxs-lookup"><span data-stu-id="49756-105">**Applies to:**</span></span>

- <span data-ttu-id="49756-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="49756-106">Partner Center</span></span>
- <span data-ttu-id="49756-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="49756-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="49756-108">CRM Salesforce</span><span class="sxs-lookup"><span data-stu-id="49756-108">Salesforce CRM</span></span>

<span data-ttu-id="49756-109">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="49756-109">**Appropriate roles**</span></span>

- <span data-ttu-id="49756-110">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="49756-110">Referrals admin</span></span>
- <span data-ttu-id="49756-111">Amministratore di sistema o verbi di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="49756-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="49756-112">Domande e risposte sui prerequisiti</span><span class="sxs-lookup"><span data-stu-id="49756-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="49756-113">È possibile usare una soluzione di valutazione per la co-selling dei connettori per l'ambiente?</span><span class="sxs-lookup"><span data-stu-id="49756-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="49756-114">Se si utilizza l'ambiente di test/gestione temporanea, è possibile optare per la soluzione di valutazione.</span><span class="sxs-lookup"><span data-stu-id="49756-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="49756-115">La versione a pagamento dei connettori è disponibile in AppSource a 15 dollari al mese.</span><span class="sxs-lookup"><span data-stu-id="49756-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="49756-116">Con la connessione a pagamento, si otterranno 10.000 chiamate API al giorno.</span><span class="sxs-lookup"><span data-stu-id="49756-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="49756-117">I connettori sono wrapper oltre alle API di riferimento del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="49756-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="49756-118">Ogni volta che le soluzioni del connettore vengono eseguite per un evento di **creazione** o **aggiornamento** in caso di opportunità in un centro per i partner o sul lato CRM, viene eseguita una chiamata API.</span><span class="sxs-lookup"><span data-stu-id="49756-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="49756-119">Quale ruolo è necessario per creare sezioni nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="49756-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="49756-120">Gli utenti che sono amministratori di sistema o personalizzatori di sistema possono applicare modifiche a tutti.</span><span class="sxs-lookup"><span data-stu-id="49756-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="49756-121">Tutti gli utenti dell'app, tuttavia, possono personalizzare il sistema e persino condividere alcune delle loro personalizzazioni con altri utenti.</span><span class="sxs-lookup"><span data-stu-id="49756-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="49756-122">I venditori partner hanno bisogno di ruoli speciali per lavorare al centro per i partner?</span><span class="sxs-lookup"><span data-stu-id="49756-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="49756-123">Ai venditori partner deve essere assegnato il ruolo di amministratore dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="49756-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="49756-124">Per ulteriori informazioni, fare riferimento a [Cenni preliminari sulle autorizzazioni) (Create-User-Accounts-and-set-permissions).</span><span class="sxs-lookup"><span data-stu-id="49756-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="49756-125">Quali campi devono essere impostati per primi nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="49756-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="49756-126">• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trovi in un ambiente CRM in modo accurato.</span><span class="sxs-lookup"><span data-stu-id="49756-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="49756-127">• Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="49756-128">Quali prerequisiti sono necessari per la creazione dell'ambiente di Power Automatic?</span><span class="sxs-lookup"><span data-stu-id="49756-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="49756-129">Per usare l'ambiente Power automatizzate, è necessario quanto segue:</span><span class="sxs-lookup"><span data-stu-id="49756-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="49756-130">È necessaria una licenza di Power automatici.</span><span class="sxs-lookup"><span data-stu-id="49756-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="49756-131">È necessario almeno 1 GB di spazio di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="49756-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="49756-132">È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione connettori Salesforce?</span><span class="sxs-lookup"><span data-stu-id="49756-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="49756-133">La soluzione del connettore Salesforce è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="49756-134">Per la soluzione non è necessario disporre di un'istanza di Dynamics 365 o di una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="49756-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="49756-135">Durante l'installazione della soluzione Salesforce, può essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda.</span><span class="sxs-lookup"><span data-stu-id="49756-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="49756-136">È necessario selezionare l'ambiente.</span><span class="sxs-lookup"><span data-stu-id="49756-136">You need to select that environment.</span></span> <span data-ttu-id="49756-137">Inoltre, se si riceve l'errore "non è stato possibile trovare un'organizzazione Dynamics 365 connessa all'utente connesso", sarà necessario creare un nuovo ambiente per il connettore.</span><span class="sxs-lookup"><span data-stu-id="49756-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="49756-138">Domande e risposte sulla configurazione</span><span class="sxs-lookup"><span data-stu-id="49756-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="49756-139">Cosa si deve fare se si affronta l'errore seguente durante l'attivazione dei flussi nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="49756-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="49756-140">Errore: la richiesta di Azure Resource Manager non è riuscita con errore:' {"Error": {"code": "WorkflowTriggerNotFound", "message": "Impossibile trovare il trigger ' manual ' del flusso di lavoro."}}'.</span><span class="sxs-lookup"><span data-stu-id="49756-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="49756-141">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="49756-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="49756-142">Eliminare la connessione CDS e quindi ricreare le connessioni CDS.</span><span class="sxs-lookup"><span data-stu-id="49756-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="49756-143">Attivare e disattivare il flusso figlio</span><span class="sxs-lookup"><span data-stu-id="49756-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="49756-144">Eliminare la soluzione e reinstallare la soluzione.</span><span class="sxs-lookup"><span data-stu-id="49756-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="49756-145">Cosa si deve fare se si affronta l'errore di "accesso" durante l'aggiunta di un connettore del centro per i partner nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="49756-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

<span data-ttu-id="49756-147">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="49756-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="49756-148">Usare le credenziali del centro per i partner per accedere all'ambiente Microsoft Flow una volta (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="49756-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="49756-149">Cosa è necessario fare se viene visualizzato l'errore seguente quando si attiva il centro per i partner al flusso di CRM nella piattaforma Power automatizzate?</span><span class="sxs-lookup"><span data-stu-id="49756-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede l'accesso":::

<span data-ttu-id="49756-151">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="49756-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="49756-152">Attivare i seguenti due flussi figlio prima di attivare il centro per i partner al flusso CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="49756-153">Centro per i partner per CRM-Helper (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="49756-154">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a CRM (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="49756-155">Cosa fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?</span><span class="sxs-lookup"><span data-stu-id="49756-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="49756-156">Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.</span><span class="sxs-lookup"><span data-stu-id="49756-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="49756-157">Se la finestra di dialogo per l'aggiunta di connessioni non viene aperta automaticamente durante la modifica del flusso, è possibile modificare singolarmente i passaggi e i passaggi secondari dei flussi.</span><span class="sxs-lookup"><span data-stu-id="49756-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="49756-158">Selezionare ogni flusso e modificarli singolarmente.</span><span class="sxs-lookup"><span data-stu-id="49756-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="49756-159">Espandi tutti i passaggi nel flusso</span><span class="sxs-lookup"><span data-stu-id="49756-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Messaggio di errore che richiede l'accesso":::

- <span data-ttu-id="49756-161">Selezionare i passaggi in cui viene visualizzata un'icona di avviso che richiede di associare le connessioni e di aggiungere connessioni.</span><span class="sxs-lookup"><span data-stu-id="49756-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Messaggio di errore che richiede l'accesso":::


5. <span data-ttu-id="49756-163">Cosa si deve fare se i flussi della soluzione per la co-selling dei connettori per i riferimenti non vengono attivati?</span><span class="sxs-lookup"><span data-stu-id="49756-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="49756-164">R.</span><span class="sxs-lookup"><span data-stu-id="49756-164">A.</span></span> <span data-ttu-id="49756-165">In Power automatizzate, sarà necessario modificare i flussi nell'ordine seguente e aggiornarli in modo da usare le connessioni corrette:</span><span class="sxs-lookup"><span data-stu-id="49756-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="49756-166">Registrazione webhook del centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="49756-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="49756-167">Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="49756-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49756-168">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="49756-169">Da partner Center a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="49756-170">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="49756-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49756-171">Opportunità di Salesforce per il centro per i partner (anteprima Insider)</span><span class="sxs-lookup"><span data-stu-id="49756-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49756-172">Salesforce Microsoft Solutions to partner Center (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="49756-173">B.</span><span class="sxs-lookup"><span data-stu-id="49756-173">B.</span></span> <span data-ttu-id="49756-174">Per ogni flusso, selezionare l'opzione **Esegui solo utenti** .</span><span class="sxs-lookup"><span data-stu-id="49756-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="49756-175">Selezionare **Usa connessione** anziché **fornita dall'utente di sola esecuzione**.</span><span class="sxs-lookup"><span data-stu-id="49756-175">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Messaggio di errore che richiede l'accesso":::


<span data-ttu-id="49756-177">C.</span><span class="sxs-lookup"><span data-stu-id="49756-177">C.</span></span> <span data-ttu-id="49756-178">Attivare questi flussi indicati di seguito:</span><span class="sxs-lookup"><span data-stu-id="49756-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="49756-179">Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49756-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="49756-180">Da Salesforce al centro per i partner (anteprima di Insider)</span><span class="sxs-lookup"><span data-stu-id="49756-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="49756-181">D.</span><span class="sxs-lookup"><span data-stu-id="49756-181">D.</span></span> <span data-ttu-id="49756-182">Attivare tutti i flussi rimanenti.</span><span class="sxs-lookup"><span data-stu-id="49756-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="49756-183">E.</span><span class="sxs-lookup"><span data-stu-id="49756-183">E.</span></span> <span data-ttu-id="49756-184">Nella registrazione del webhook del centro per i partner Microsoft Flow selezionare **Esegui**.</span><span class="sxs-lookup"><span data-stu-id="49756-184">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="49756-185">Fornire l' **URL http** dalla prima azione nel **centro per i partner al flusso di Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="49756-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="49756-186">Selezionare tutte e quattro le opzioni in **eventi da registrare** e selezionare **Sì** per Sovrascrivi.</span><span class="sxs-lookup"><span data-stu-id="49756-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="49756-187">Domande e risposte su esecuzione/manutenzione</span><span class="sxs-lookup"><span data-stu-id="49756-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="49756-188">Come si risolvono i problemi in caso di errori durante l'esecuzione di Power automatizzare il flusso?</span><span class="sxs-lookup"><span data-stu-id="49756-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="49756-189">Per assicurarsi che i flussi vengano eseguiti come previsto e per risolvere gli errori durante l'esecuzione, vedere correggere gli [errori di flusso](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="49756-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="49756-190">Cosa è necessario fare se vengono visualizzati riferimenti che non sono sincronizzati correttamente nel centro per i partner o nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="49756-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="49756-191">Per determinare lo stato della sincronizzazione dei riferimenti, selezionare **controllo**.</span><span class="sxs-lookup"><span data-stu-id="49756-191">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Messaggio di errore che richiede l'accesso":::

<span data-ttu-id="49756-193">Verificare che siano soddisfatte le condizioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="49756-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="49756-194">L'ID soluzione viene fornito come parte dell'opportunità.</span><span class="sxs-lookup"><span data-stu-id="49756-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="49756-195">Il codice paese a due lettere è obbligatorio.</span><span class="sxs-lookup"><span data-stu-id="49756-195">Two letter country code is required.</span></span>

- <span data-ttu-id="49756-196">Quando la Guida di Microsoft è selezionata per l'opportunità, le informazioni di contatto del cliente sono obbligatorie.</span><span class="sxs-lookup"><span data-stu-id="49756-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="49756-197">Come verificare che il riferimento venga sincronizzato in modo bidirezionale?</span><span class="sxs-lookup"><span data-stu-id="49756-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="49756-198">Eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="49756-198">Do the following steps:</span></span>

- <span data-ttu-id="49756-199">Per i venditori partner è necessario assicurarsi di aver abilitato l'opzione **Sync with partner Center** nella sezione CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Messaggio di errore che richiede l'accesso":::

- <span data-ttu-id="49756-201">I venditori devono fornire i ricavi e la data di chiusura quando qualificano un responsabile.</span><span class="sxs-lookup"><span data-stu-id="49756-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="49756-202">Se l'ID CRM viene specificato nella fase di **creazione** o **aggiornamento** dell'opportunità di co-selling, ma non è stata trovata un'opportunità di lead con tale ID in CRM, Update o create verranno ignorate.</span><span class="sxs-lookup"><span data-stu-id="49756-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="49756-203">Verificare che il campo valuta referral sia configurato nell'ambiente Salesforce.</span><span class="sxs-lookup"><span data-stu-id="49756-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="49756-204">Cosa è necessario fare se il connettore viene disconnesso e non viene eseguita una sincronizzazione dei riferimenti.</span><span class="sxs-lookup"><span data-stu-id="49756-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="49756-205">Di seguito sono riportate alcune delle opzioni che è possibile provare:</span><span class="sxs-lookup"><span data-stu-id="49756-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="49756-206">Controllare se il nome utente o la password è scaduta per l'utente del centro per i partner con i ruoli di amministratore di riferimento.</span><span class="sxs-lookup"><span data-stu-id="49756-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="49756-207">È possibile passare all'opportunità non sincronizzata, effettuare un aggiornamento secondario e osservare se il riferimento è stato sincronizzato.</span><span class="sxs-lookup"><span data-stu-id="49756-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="49756-208">Se i flussi sono stati eseguiti e non riusciti, selezionare il flusso e inviare di nuovo l'esecuzione che ha avuto esito negativo.</span><span class="sxs-lookup"><span data-stu-id="49756-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="49756-209">Cosa si deve fare quando si ricevono errori di accesso negato?</span><span class="sxs-lookup"><span data-stu-id="49756-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="49756-210">Verificare che siano presenti i ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="49756-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="49756-211">Ruolo di amministratore di riferimento per il venditore del centro partner</span><span class="sxs-lookup"><span data-stu-id="49756-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="49756-212">Ruolo di amministratore di sistema o di sistema verbi nell'istanza di CRM</span><span class="sxs-lookup"><span data-stu-id="49756-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="49756-213">Assicurarsi che l'utente di Power automatizzare l'accesso https://flow.microsoft.com all'account di flusso almeno una volta in anticipo</span><span class="sxs-lookup"><span data-stu-id="49756-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="49756-214">Se si nota che il **codice paese dell'account del cliente** non è presente durante la creazione di un'opportunità di co-selling, cosa si deve fare?</span><span class="sxs-lookup"><span data-stu-id="49756-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="49756-215">È necessario aggiungere il codice di paese a due lettere ISO all'account del cliente in CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="49756-216">Cosa è necessario fare se viene visualizzato l'errore relativo all' **ID della soluzione necessaria** per la creazione di un'opportunità di co-selling?</span><span class="sxs-lookup"><span data-stu-id="49756-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="49756-217">Per creare un riferimento di co-selling, è necessaria una soluzione di co-selling per Microsoft.</span><span class="sxs-lookup"><span data-stu-id="49756-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="49756-218">Cosa si deve fare quando vengono visualizzate opportunità di co-selling create in Partner Center che non vengono sincronizzate con CRM anche se non sono presenti errori di flusso:</span><span class="sxs-lookup"><span data-stu-id="49756-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="49756-219">Eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="49756-219">Do the following:</span></span>

- <span data-ttu-id="49756-220">Dopo aver creato una nuova operazione di co-selling nel centro per i partner, verificare che venga richiamato il centro per i partner del flusso di Dynamics 365 (potrebbe essere richiamato più volte).</span><span class="sxs-lookup"><span data-stu-id="49756-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="49756-221">Se il flusso viene richiamato, controllare tutti i flussi richiamati e identificare l'esecuzione del flusso che aggiornerà il CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="49756-222">È possibile seguire le azioni e verificare se il CRM è stato aggiornato o se si è verificato un problema.</span><span class="sxs-lookup"><span data-stu-id="49756-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="49756-223">Controllare *New Deal*\* nel centro per i partner per verificare se viene popolato con l'ID CRM.</span><span class="sxs-lookup"><span data-stu-id="49756-223">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="49756-224">Assicurarsi che l'operazione non sia chiusa accidentalmente come "Won" o "Lost" nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="49756-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="49756-225">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="49756-225">Next steps</span></span>

- [<span data-ttu-id="49756-226">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="49756-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="49756-227">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="49756-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)