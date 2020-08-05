---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account cliente e delle sottoscrizioni dei clienti.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 4e6d98069822df9a6310335ffd8b1ab08dc61ccb
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545652"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="345fe-104">Istruzioni per il consolidamento dei tenant per l'autorizzazione regionale per CSP</span><span class="sxs-lookup"><span data-stu-id="345fe-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="345fe-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="345fe-105">**Applies to**</span></span>

-  <span data-ttu-id="345fe-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="345fe-106">Partner Center</span></span>
-  <span data-ttu-id="345fe-107">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="345fe-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="345fe-108">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="345fe-108">**Appropriate roles**</span></span>

- <span data-ttu-id="345fe-109">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="345fe-109">Global admin</span></span>
- <span data-ttu-id="345fe-110">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="345fe-110">Admin agent</span></span>

<span data-ttu-id="345fe-111">\[Alcune informazioni si riferiscono al prodotto pre-rilasciato che può essere modificato in modo sostanziale prima del rilascio commerciale.</span><span class="sxs-lookup"><span data-stu-id="345fe-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="345fe-112">Microsoft non offre alcuna garanzia, esplicita o implicita, relativamente alle informazioni fornite.\]</span><span class="sxs-lookup"><span data-stu-id="345fe-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="345fe-113">È possibile consolidare i tenant per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="345fe-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="345fe-114">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="345fe-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="345fe-115">È necessario essere a conoscenza di tutte le sottoscrizioni di cui è stato effettuato il provisioning e dei conteggi delle licenze per ogni cliente nell'account da cui si esegue la transizione.</span><span class="sxs-lookup"><span data-stu-id="345fe-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="345fe-116">Verrà eseguito nuovamente il provisioning di tali sottoscrizioni esatte con gli stessi conteggi delle licenze nel nuovo account CSP centrale come parte del processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="345fe-117">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="345fe-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="345fe-118">Al termine del consolidamento, non è possibile ripristinare lo stato precedente del tenant.</span><span class="sxs-lookup"><span data-stu-id="345fe-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="345fe-119">Potrebbe essere necessaria anche l'azione del cliente.</span><span class="sxs-lookup"><span data-stu-id="345fe-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="345fe-120">Preparare la migrazione</span><span class="sxs-lookup"><span data-stu-id="345fe-120">Prepare for migration</span></span>

- <span data-ttu-id="345fe-121">Accedere al centro per i **partner** usando l'account di **transizione** (quello che si passerà al nuovo account) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="345fe-122">Disconnettersi da questo account.</span><span class="sxs-lookup"><span data-stu-id="345fe-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="345fe-123">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="345fe-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="345fe-124">Accedere al centro per i **partner** con l'account di **transizione** (nuovo) (quello in cui si sta effettuando la transizione dei clienti).</span><span class="sxs-lookup"><span data-stu-id="345fe-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="345fe-125">Selezionare **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="345fe-125">Select **Customers**.</span></span>

3. <span data-ttu-id="345fe-126">Fai cli su **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="345fe-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="345fe-127">Viene visualizzato un messaggio di posta elettronica predefinito da inviare ai clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="345fe-128">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="345fe-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="345fe-129">**Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL.</span><span class="sxs-lookup"><span data-stu-id="345fe-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="345fe-130">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="345fe-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="345fe-131">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="345fe-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="345fe-132">Dopo l'accesso, all'amministratore globale per l' **account del cliente** viene richiesto di inviare un contratto che fornisce privilegi amministrativi delegati al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="345fe-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="345fe-133">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="345fe-134">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo che hanno inviato il contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="345fe-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="345fe-135">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="345fe-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="345fe-136">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="345fe-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="345fe-137">Dal **centro** per i partner selezionare **Customers**.</span><span class="sxs-lookup"><span data-stu-id="345fe-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="345fe-138">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="345fe-139">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="345fe-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="345fe-140">Aggiungere al catalogo le sottoscrizioni e i conteggi delle licenze corretti.</span><span class="sxs-lookup"><span data-stu-id="345fe-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="345fe-141">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="345fe-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco dei clienti":::

6. <span data-ttu-id="345fe-143">Fare clic su **Invia.**</span><span class="sxs-lookup"><span data-stu-id="345fe-143">Click **Submit.**</span></span>

   <span data-ttu-id="345fe-144">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="345fe-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="345fe-145">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="345fe-146">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="345fe-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="345fe-147">I partner devono sospendere le sottoscrizioni in **fase di transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all' **account del tenant partner nel** centro per assicurarsi che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="345fe-148">Le richieste di supporto verranno negate per i crediti a causa di sovrapposizioni nella fatturazione che si verificano quando non si disabilita correttamente la **transizione dalle** sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="345fe-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="345fe-149">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="345fe-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="345fe-150">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="345fe-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="345fe-151">Non è necessario disabilitare manualmente le sottoscrizioni di Azure perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="345fe-152">Accedere al centro per i **partner** con l'account di **transizione da** CSP e passare all'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="345fe-153">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="345fe-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="345fe-154">Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="345fe-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="345fe-155">La sospensione della sottoscrizione garantisce che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="345fe-156">La sottoscrizione Mostra **sospesa** nell'elenco delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="345fe-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="345fe-157">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="345fe-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="345fe-158">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="345fe-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="345fe-159">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="345fe-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="345fe-160">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="345fe-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="345fe-161">A differenza delle sottoscrizioni di Office 365 CSP, non è necessario eseguire la migrazione manuale delle sottoscrizioni CSP basate sull'utilizzo di Azure.</span><span class="sxs-lookup"><span data-stu-id="345fe-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="345fe-162">Il supporto Microsoft Azure eseguirà la migrazione delle sottoscrizioni di Azure, nonché di tutti i servizi o le risorse distribuiti dalla **transizione dagli account del** rivenditore CSP all' **account del rivenditore** CSP.</span><span class="sxs-lookup"><span data-stu-id="345fe-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="345fe-163">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="345fe-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="345fe-164">Assicurarsi che gli account cliente che disporranno di sottoscrizioni di Azure migrati abbiano accettato il contratto da associare alla nuova **transizione all'** account CSP.</span><span class="sxs-lookup"><span data-stu-id="345fe-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="345fe-165">Si invierà una notifica a Microsoft di quali account cliente sono pronti per la migrazione e si specificano i nomi delle società dei clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="345fe-166">Microsoft esegue la migrazione delle sottoscrizioni basate sull'utilizzo di Azure e invia una notifica al termine della migrazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="345fe-167">È necessario verificare che la sottoscrizione di Azure nell'ambito dell'account reseller del rivenditore **di** CSP sia ora contrassegnata come **sospesa** nel centro per i partner nella sezione sottoscrizioni clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="345fe-168">Verificare che la sottoscrizione di Azure in **transizione all'** account rivenditore CSP Ora visualizzi lo stato **attivo** nel centro per i partner nella sezione sottoscrizioni clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="345fe-169">La disabilitazione delle sottoscrizioni del cliente non comporta la modifica dell'aspetto del cliente nell'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="345fe-170">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="345fe-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="345fe-171">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="345fe-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="345fe-172">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="345fe-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="345fe-173">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="345fe-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="345fe-174">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="345fe-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="345fe-175">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="345fe-175">Additional information</span></span>

- <span data-ttu-id="345fe-176">La disabilitazione della sottoscrizione dalla **transizione dall'** account CSP non influisca sul servizio del cliente finale purché sia stato effettuato il provisioning del servizio dall'account **di transizione a** CSP prima di disabilitare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="345fe-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="345fe-177">Le sottoscrizioni non possono essere utilizzate dal cliente e non generano addebiti quando vengono sospese o annullate.</span><span class="sxs-lookup"><span data-stu-id="345fe-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="345fe-178">Attualmente non è possibile rimuovere completamente un cliente dall'elenco dei **clienti** .</span><span class="sxs-lookup"><span data-stu-id="345fe-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="345fe-179">I partner devono sospendere le sottoscrizioni per la **transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui vengono passate le sottoscrizioni e configurate in fase di **transizione a** account per assicurarsi che la doppia fatturazione non venga eseguita.</span><span class="sxs-lookup"><span data-stu-id="345fe-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="345fe-180">Microsoft non supporterà le richieste di crediti dovute a eventuali sovrapposizioni nella fatturazione che si verificano se non si imposta correttamente la **transizione dalle** sottoscrizioni a sospesa.</span><span class="sxs-lookup"><span data-stu-id="345fe-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="345fe-181">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="345fe-181">Simplify migration using Export</span></span>

<span data-ttu-id="345fe-182">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="345fe-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="345fe-183">Fare clic su **clienti** nel centro per i partner per visualizzare l'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="345fe-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="345fe-184">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="345fe-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="345fe-185">Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="345fe-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="345fe-186">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="345fe-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="345fe-187">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="345fe-187">API registration</span></span>

<span data-ttu-id="345fe-188">Per altre informazioni sulla registrazione dell'API, vedere [configurare l'accesso all'API nel centro per i partner](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="345fe-188">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="next-steps"></a><span data-ttu-id="345fe-189">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="345fe-189">Next steps</span></span>

- [<span data-ttu-id="345fe-190">Configurazione e gestione degli account cliente per i partner rivenditori nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="345fe-190">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)
