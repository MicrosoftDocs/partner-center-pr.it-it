---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account cliente e delle sottoscrizioni dei clienti.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: migrare i clienti, il provisioning, l'account tenant, il consolidamento dei tenant
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: c2667bf19f73dfb2498cd6f706bd97b595f67a31
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679068"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="e6ca4-105">Istruzioni per il consolidamento dei tenant di autorizzazione regionale CSP</span><span class="sxs-lookup"><span data-stu-id="e6ca4-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="e6ca4-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="e6ca4-106">**Applies to**</span></span>

-  <span data-ttu-id="e6ca4-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="e6ca4-107">Partner Center</span></span>
-  <span data-ttu-id="e6ca4-108">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e6ca4-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e6ca4-109">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="e6ca4-109">**Appropriate roles**</span></span>

- <span data-ttu-id="e6ca4-110">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="e6ca4-110">Global admin</span></span>
- <span data-ttu-id="e6ca4-111">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="e6ca4-111">Admin agent</span></span>

<span data-ttu-id="e6ca4-112">\[Alcune informazioni si riferiscono al prodotto pre-rilasciato che può essere modificato in modo sostanziale prima del rilascio commerciale.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="e6ca4-113">Microsoft non offre alcuna garanzia, espressa o implicita, relativamente alle informazioni fornite in questo articolo.\]</span><span class="sxs-lookup"><span data-stu-id="e6ca4-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="e6ca4-114">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="e6ca4-115">È necessario essere a conoscenza di tutte le sottoscrizioni e dei conteggi delle postazioni per i clienti sottoposti a provisioning dagli account di transizione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-115">You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="e6ca4-116">Verrà eseguito nuovamente il provisioning di tali sottoscrizioni esatte con lo stesso numero di postazioni del nuovo account CSP centrale come parte del processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="e6ca4-117">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="e6ca4-118">Il consolidamento dei tenant è una scelta del partner.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="e6ca4-119">Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="e6ca4-120">Potrebbe essere necessaria anche l'azione del cliente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-120">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="e6ca4-121">Preparare la migrazione</span><span class="sxs-lookup"><span data-stu-id="e6ca4-121">Prepare for migration</span></span>

- <span data-ttu-id="e6ca4-122">Accedere al centro per i **partner** con l'account di **transizione** (esistente) (quello che si eseguirà la transizione) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-122">Sign in to **Partner Center**  with the **Transitioning** (existing) account (the one you will transition) and review of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="elenco dei clienti regionali":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="e6ca4-124">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="e6ca4-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="e6ca4-125">Accedere al centro per i **partner** con l'account di **transizione** (nuovo) (quello in cui si sta effettuando la transizione) e passare all'elenco Customers (clienti) dai **clienti**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="e6ca4-126">Selezionare Clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-126">Select Customers.</span></span>

3. <span data-ttu-id="e6ca4-127">Fai cli su **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="e6ca4-128">Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="e6ca4-129">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="e6ca4-130">**Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="e6ca4-131">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="e6ca4-132">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="e6ca4-133">Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="e6ca4-134">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="e6ca4-135">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo che hanno inviato il contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="e6ca4-136">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="e6ca4-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="e6ca4-137">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="e6ca4-138">Dal **centro** per i partner selezionare **Customers**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-138">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="e6ca4-139">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="e6ca4-140">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-140">Select **Add subscription**.</span></span>

5. <span data-ttu-id="e6ca4-141">Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="e6ca4-142">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco dei clienti":::

6. <span data-ttu-id="e6ca4-144">Fare clic su **Invia.**</span><span class="sxs-lookup"><span data-stu-id="e6ca4-144">Click **Submit.**</span></span>

   <span data-ttu-id="e6ca4-145">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="e6ca4-146">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="e6ca4-147">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="e6ca4-148">I partner devono sospendere le sottoscrizioni in **fase di transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all' **account del tenant partner nel** centro per assicurarsi che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="e6ca4-149">Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="e6ca4-150">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="e6ca4-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="e6ca4-151">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="e6ca4-152">Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="e6ca4-153">Accedere al centro per i **partner** con l'account di **transizione da** CSP e passare all'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="e6ca4-154">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="e6ca4-155">Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="e6ca4-156">La sospensione della sottoscrizione garantisce che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="e6ca4-157">La sottoscrizione è indicata con lo stato **Sospeso** nell'elenco delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="e6ca4-158">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="e6ca4-159">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="e6ca4-160">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="e6ca4-161">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="e6ca4-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="e6ca4-162">Azure, le sottoscrizioni CSP basate sull'utilizzo non devono essere migrate manualmente come nel caso delle sottoscrizioni di Office 365 CSP.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="e6ca4-163">Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="e6ca4-164">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="e6ca4-165">Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="e6ca4-166">I partner notificano a Microsoft quali account cliente che dispongono di sottoscrizioni di Azure sono pronti per la migrazione e forniscono i nomi delle società dei clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="e6ca4-167">Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="e6ca4-168">Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="e6ca4-169">Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="e6ca4-170">La disabilitazione delle sottoscrizioni del cliente non comporta la modifica dell'aspetto del cliente nell'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="e6ca4-171">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="e6ca4-172">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="e6ca4-173">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="e6ca4-174">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="e6ca4-175">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-175">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="e6ca4-176">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="e6ca4-176">Additional information</span></span>

- <span data-ttu-id="e6ca4-177">La disabilitazione della sottoscrizione dalla **transizione dall'** account CSP non influisca sul servizio del cliente finale purché sia stato effettuato il provisioning del servizio dall'account **di transizione a** CSP prima di disabilitare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="e6ca4-178">Le sottoscrizioni non possono essere utilizzate dal cliente e non generano addebiti quando vengono sospese o annullate.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="e6ca4-179">Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

    >[!Note]
    > <span data-ttu-id="e6ca4-180">I partner devono sospendere le sottoscrizioni per la **transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all'account del tenant partner nel centro per i partner per garantire che non si **verifichi la doppia** fatturazione.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="e6ca4-181">Microsoft non supporterà le richieste di crediti dovute a eventuali sovrapposizioni nella fatturazione che si verificano se non si imposta correttamente la **transizione dalle** sottoscrizioni a sospesa.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="e6ca4-182">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="e6ca4-182">Simplify migration using Export</span></span>

<span data-ttu-id="e6ca4-183">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="e6ca4-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="e6ca4-184">Fare clic su **clienti** nel centro per i partner per visualizzare l'elenco dei clienti nella struttura esistente.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="e6ca4-185">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="e6ca4-186">Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="e6ca4-187">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="e6ca4-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="e6ca4-188">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="e6ca4-188">API registration</span></span>

<span data-ttu-id="e6ca4-189">Per altre informazioni sulla registrazione dell'API, vedere [configurare l'accesso all'API nel centro per i partner](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="e6ca4-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
