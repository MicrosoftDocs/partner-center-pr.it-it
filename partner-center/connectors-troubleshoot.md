---
title: Risoluzione dei problemi relativi ai connettori di co-selling
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle risposte alle domande comuni sull'uso dei connettori di co-selling. Leggere queste domande frequenti su come risolvere i problemi relativi ai connettori di co-selling.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284214"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="2d2a2-104">Risoluzione dei problemi relativi ai connettori di co-selling</span><span class="sxs-lookup"><span data-stu-id="2d2a2-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="2d2a2-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-105">**Applies to**</span></span>

- <span data-ttu-id="2d2a2-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="2d2a2-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="2d2a2-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="2d2a2-107">Salesforce CRM</span></span>

<span data-ttu-id="2d2a2-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-108">**Appropriate roles**</span></span>

- <span data-ttu-id="2d2a2-109">Amministratore delle segnalazioni</span><span class="sxs-lookup"><span data-stu-id="2d2a2-109">Referrals admin</span></span>
- <span data-ttu-id="2d2a2-110">Amministratore di sistema o a personalizzatore di sistema in CRM</span><span class="sxs-lookup"><span data-stu-id="2d2a2-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="2d2a2-111">Domande e risposte sui prerequisiti</span><span class="sxs-lookup"><span data-stu-id="2d2a2-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="2d2a2-112">È possibile usare una soluzione connettori per le segnalazioni di co-selling di valutazione per l'ambiente?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="2d2a2-113">Se si è nell'ambiente di test/staging, è possibile optare per la soluzione di valutazione.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="2d2a2-114">La versione a pagamento dei connettori è disponibile in AppSource a US$ 15/mese.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="2d2a2-115">Con la connessione a pagamento si riceveranno 10.000 chiamate API al giorno.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="2d2a2-116">I connettori sono wrapper sulle API di riferimento Partner Center di riferimento.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="2d2a2-117">Ogni volta che le  soluzioni  connettore vengono eseguite per un evento di creazione o aggiornamento sulle opportunità Partner Center o sul lato CRM, viene eseguita una chiamata API.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="2d2a2-118">Quale ruolo è necessario per creare sezioni nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="2d2a2-119">Gli utenti amministratori di sistema o personalizzatori di sistema possono applicare modifiche a tutti gli utenti.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="2d2a2-120">Tutti gli utenti dell'app, tuttavia, possono personalizzare il sistema e persino condividere alcune personalizzazioni con altri utenti.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="2d2a2-121">I venditori di partner hanno bisogno di ruoli speciali per lavorare Partner Center?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="2d2a2-122">Ai venditori partner deve essere assegnato il ruolo "Amministratore delle segnalazioni".</span><span class="sxs-lookup"><span data-stu-id="2d2a2-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="2d2a2-123">Per altre informazioni, vedere Panoramica [delle autorizzazioni](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="2d2a2-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="2d2a2-124">Quali campi devono essere impostati per primi nell'ambiente CRM?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="2d2a2-125">• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trova nell'ambiente CRM in modo accurato.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="2d2a2-126">• Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="2d2a2-127">Quali prerequisiti sono necessari per la creazione Power Automate'ambiente?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="2d2a2-128">Per usare l'Power Automate virtuale, è necessario:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="2d2a2-129">È Power Automate una licenza.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="2d2a2-130">È necessario almeno 1 GB di spazio di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="2d2a2-131">È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione connettori Salesforce?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="2d2a2-132">La soluzione Salesforce Connector è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="2d2a2-133">La soluzione non richiede un'istanza di Dynamics 365 o una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="2d2a2-134">Durante l'installazione della soluzione Salesforce, potrebbe essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="2d2a2-135">È necessario selezionare l'ambiente.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-135">You need to select that environment.</span></span> <span data-ttu-id="2d2a2-136">Inoltre, se viene visualizzato l'errore "Non è stato possibile trovare un'organizzazione dynamics 365 connessa all'utente connesso", sarà necessario creare un nuovo ambiente per il connettore.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="2d2a2-137">Domande e risposte sulla configurazione</span><span class="sxs-lookup"><span data-stu-id="2d2a2-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="2d2a2-138">Cosa è necessario fare se si verifica l'errore seguente durante l'attivazione dei flussi in Power Automate piattaforma?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="2d2a2-139">Errore: Richiesta a Azure Resource Manager non riuscita con errore: '{"error":{"code":"WorkflowTriggerNotFound","message":"Impossibile trovare il trigger 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual'."}}'.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="2d2a2-140">Seguire questa procedura per la risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="2d2a2-141">Eliminare la connessione CDS e quindi ricreare le connessioni CDS.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="2d2a2-142">Attivare e disattivare il flusso figlio</span><span class="sxs-lookup"><span data-stu-id="2d2a2-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="2d2a2-143">Eliminare la soluzione e reinstallarla.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="2d2a2-144">Cosa è necessario fare se si verifica l'errore "Accesso" durante l'aggiunta di un connettore Partner Center in Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

<span data-ttu-id="2d2a2-146">Seguire questo passaggio per la risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="2d2a2-147">Usare le credenziali Partner Center per accedere all'ambiente di flusso una sola volta (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="2d2a2-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="2d2a2-148">Cosa fare se viene visualizzato l'errore seguente durante l'attivazione del flusso Partner Center flusso da crm a CRM in Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede aggiornamenti":::

<span data-ttu-id="2d2a2-150">Seguire questa procedura di risoluzione dei problemi:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="2d2a2-151">Attivare prima i due flussi figlio seguenti prima di attivare il flusso Partner Center flusso verso CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="2d2a2-152">Partner Center a CRM - Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="2d2a2-153">Partner Center microsoft co-selling referral updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="2d2a2-154">Cosa è necessario fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="2d2a2-155">Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="2d2a2-156">Se la finestra di dialogo per aggiungere connessioni non si apre automaticamente durante la modifica del flusso, è possibile modificare ognuno dei passaggi e dei passaggi secondari dei flussi singolarmente.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="2d2a2-157">Selezionare ogni flusso e modificarlo singolarmente.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="2d2a2-158">Espandere tutti i passaggi nel flusso</span><span class="sxs-lookup"><span data-stu-id="2d2a2-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passaggi che necessitano di connessioni":::

- <span data-ttu-id="2d2a2-160">Selezionare i passaggi in cui viene visualizzata un'icona di avviso che chiede di associare le connessioni e aggiungere le connessioni.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modificare il flusso passo dopo passo":::


5. <span data-ttu-id="2d2a2-162">Cosa fare se i flussi della soluzione Co-selling Referrals Connectors non si attivano?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="2d2a2-163">A.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-163">A.</span></span> <span data-ttu-id="2d2a2-164">In Power Automate, è necessario modificare i flussi nell'ordine seguente e aggiornarli per usare le connessioni corrette:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="2d2a2-165">Partner Center Webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-166">Creare una segnalazione di co-selling - Salesforce per Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-167">Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-168">Partner Center a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-169">Da Salesforce a Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-170">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="2d2a2-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="2d2a2-172">B.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-172">B.</span></span> <span data-ttu-id="2d2a2-173">Per ogni flusso selezionare **l'opzione Esegui solo utenti.**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="2d2a2-174">Selezionare **Usa connessione** anziché Fornito **dall'utente di sola esecuzione.**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Per attivare un flusso":::


<span data-ttu-id="2d2a2-176">C.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-176">C.</span></span> <span data-ttu-id="2d2a2-177">Attivare i flussi indicati di seguito:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="2d2a2-178">Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="2d2a2-179">Da Salesforce a Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="2d2a2-180">D.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-180">D.</span></span> <span data-ttu-id="2d2a2-181">Attivare tutti i flussi rimanenti.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="2d2a2-182">E.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-182">E.</span></span> <span data-ttu-id="2d2a2-183">In flow Partner Center Webhook Registration (Registrazione webhook) **selezionare Run (Esegui).**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="2d2a2-184">Specificare **l'URL HTTP** della prima azione nel **flusso Partner Center a Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="2d2a2-185">Selezionare tutte e quattro le opzioni **in Eventi da registrare** e selezionare **Sì** per Sovrascrivi.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="2d2a2-186">Domande e risposte su Esecuzione/Manutenzione</span><span class="sxs-lookup"><span data-stu-id="2d2a2-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="2d2a2-187">Come risolvere gli errori durante l'Power Automate del flusso?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="2d2a2-188">Per assicurarsi che i flussi Power Automate siano eseguiti come previsto e per risolvere gli errori durante l'esecuzione, vedere [Correggere gli errori di flusso.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="2d2a2-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="2d2a2-189">Cosa devi fare se vedi segnalazioni non sincronizzate correttamente nell'ambiente Partner Center o CRM?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="2d2a2-190">Per determinare lo stato della sincronizzazione dei riferimenti, selezionare **Controlla.**</span><span class="sxs-lookup"><span data-stu-id="2d2a2-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Come sincronizzare le segnalazioni":::

<span data-ttu-id="2d2a2-192">Assicurarsi che siano soddisfatte le condizioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="2d2a2-193">L'ID soluzione viene fornito come parte dell'opportunità.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="2d2a2-194">È necessario un codice paese di due lettere.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-194">Two letter country code is required.</span></span>

- <span data-ttu-id="2d2a2-195">Quando si seleziona l'assistenza di Microsoft per l'opportunità, sono necessarie le informazioni di contatto del cliente.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="2d2a2-196">Come assicurarsi che una segnalazione verrà sincronizzata bidirezionale?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="2d2a2-197">Eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-197">Do the following steps:</span></span>

- <span data-ttu-id="2d2a2-198">I venditori partner devono assicurarsi di aver abilitato l'opzione **Sincronizza con** Partner Center nella sezione CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Assicurarsi di aver abilitato Synch":::

- <span data-ttu-id="2d2a2-200">I venditori devono fornire ricavi e data di chiusura quando qualificano un lead.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="2d2a2-201">Se l'ID CRM  viene  specificato nella fase di creazione o aggiornamento dell'opportunità di co-selling, ma un'opportunità lead con tale ID non viene trovata in CRM, l'aggiornamento o la creazione verranno ignorati.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="2d2a2-202">Assicurarsi che il campo della valuta di riferimento sia configurato nell'ambiente Salesforce.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="2d2a2-203">Cosa fare se il connettore viene disconnesso e si perde una sincronizzazione delle segnalazioni?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="2d2a2-204">Di seguito sono riportate alcune opzioni che è possibile provare:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="2d2a2-205">Controllare se il nome utente o la password sono scaduti per l Partner Center utente con ruoli di amministratore di riferimento.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="2d2a2-206">È possibile passare all'opportunità non sincronizzata, eseguire un aggiornamento secondario e osservare se la segnalazione è sincronizzata.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="2d2a2-207">Se i flussi sono stati eseguiti e non riusciti, selezionare il flusso e inviare nuovamente l'esecuzione che ha avuto esito negativo.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="2d2a2-208">Cosa è necessario fare quando si ottengono errori di accesso negato?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="2d2a2-209">Assicurarsi che esistano i ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="2d2a2-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="2d2a2-210">Ruolo di amministratore delle segnalazioni per Partner Center venditore</span><span class="sxs-lookup"><span data-stu-id="2d2a2-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="2d2a2-211">Ruolo Amministratore di sistema o Asonalizzazione sistema nell'istanza di CRM</span><span class="sxs-lookup"><span data-stu-id="2d2a2-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="2d2a2-212">Assicurarsi che l'Power Automate dell'account flusso di lavoro accerta https://flow.microsoft.com almeno una volta in anticipo</span><span class="sxs-lookup"><span data-stu-id="2d2a2-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="2d2a2-213">Se viene visualizzato il **codice paese dell'account cliente** mancante durante la creazione di un'opportunità di co-selling, cosa è necessario fare?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="2d2a2-214">Sarà necessario aggiungere il codice ISO di due lettere del paese all'account cliente in CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="2d2a2-215">Cosa fare se viene visualizzato l'errore che indica che **l'ID** soluzione è necessario durante la creazione di un'opportunità di co-selling?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="2d2a2-216">Per creare una segnalazione di co-selling, è necessaria una soluzione pronta per il co-selling Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="2d2a2-217">Cosa è necessario fare quando si visualizzano opportunità di co-selling create in Partner Center che non sono sincronizzate con CRM anche se non sono presenti errori di flusso?</span><span class="sxs-lookup"><span data-stu-id="2d2a2-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="2d2a2-218">Eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="2d2a2-218">Do the following:</span></span>

- <span data-ttu-id="2d2a2-219">Dopo aver creato una nuova trattativa di co-selling in Partner Center, verificare se il flusso Partner Center a Dynamics 365 viene richiamato (potrebbe essere richiamato più volte).</span><span class="sxs-lookup"><span data-stu-id="2d2a2-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="2d2a2-220">Se il flusso viene richiamato, controllare tutti i flussi richiamati e identificare l'esecuzione del flusso che aggiornerà crm.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="2d2a2-221">È possibile seguire le azioni e verificare se il sistema CRM è stato aggiornato o se si è verificato un problema.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="2d2a2-222">Selezionare **New deal (Nuova** trattativa) Partner Center per verificare se viene popolata con l'ID CRM.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="2d2a2-223">Assicurarsi che la trattativa non sia stata accidentalmente chiusa come **Vinta** o **Persa** in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2d2a2-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2d2a2-224">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="2d2a2-224">Next steps</span></span>

- [<span data-ttu-id="2d2a2-225">Gestire lead</span><span class="sxs-lookup"><span data-stu-id="2d2a2-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="2d2a2-226">Gestire opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="2d2a2-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
