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
ms.openlocfilehash: 813d24c12501edc7b633d3e10b5174d02ed881d1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/07/2020
ms.locfileid: "82907994"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="15bc3-105">Istruzioni per il consolidamento dei tenant di autorizzazione regionale CSP</span><span class="sxs-lookup"><span data-stu-id="15bc3-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="15bc3-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="15bc3-106">**Applies to**</span></span>

-  <span data-ttu-id="15bc3-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="15bc3-107">Partner Center</span></span>
-  <span data-ttu-id="15bc3-108">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="15bc3-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="15bc3-109">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="15bc3-109">**Appropriate roles**</span></span>

- <span data-ttu-id="15bc3-110">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="15bc3-110">Global admin</span></span>
- <span data-ttu-id="15bc3-111">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="15bc3-111">Admin agent</span></span>

<span data-ttu-id="15bc3-112">\[Alcune informazioni si riferiscono al prodotto pre-rilasciato che può essere modificato in modo sostanziale prima del rilascio commerciale.</span><span class="sxs-lookup"><span data-stu-id="15bc3-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="15bc3-113">Microsoft non offre alcuna garanzia, esplicita o implicita, riguardo alle informazioni fornite in questo documento.\]</span><span class="sxs-lookup"><span data-stu-id="15bc3-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="15bc3-114">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="15bc3-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="15bc3-115">**Nota**  È necessario essere a conoscenza di tutte le sottoscrizioni e dei conteggi delle postazioni per i clienti sottoposti a provisioning dagli account di transizione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-115">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="15bc3-116">Verrà eseguito nuovamente il provisioning di tali sottoscrizioni esatte con lo stesso numero di postazioni del nuovo account CSP centrale come parte del processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="15bc3-117">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="15bc3-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="15bc3-118">Il consolidamento dei tenant è una scelta del partner.</span><span class="sxs-lookup"><span data-stu-id="15bc3-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="15bc3-119">Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="15bc3-120">Si noti che potrebbe essere necessaria anche l'azione del cliente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-120">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="15bc3-121">Preparare la migrazione</span><span class="sxs-lookup"><span data-stu-id="15bc3-121">Prepare for migration</span></span>


-   <span data-ttu-id="15bc3-122">Accedere al centro per i **partner** con l'account di **transizione** (esistente) (quello che si vuole usare per la transizione) e prendere nota di tutti i clienti e tutti i servizi di cui è stato eseguito il provisioning per tali clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-122">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![elenco dei clienti regionali](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="15bc3-124">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="15bc3-124">Migrate customer accounts</span></span>


1.  <span data-ttu-id="15bc3-125">Accedere al centro per i **partner** con l'account di **transizione** (nuovo) (quello in cui si sta effettuando la transizione) e passare all'elenco Customers (clienti) dai **clienti**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="15bc3-126">Seleziona Clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-126">Select Customers.</span></span>

3.  <span data-ttu-id="15bc3-127">Fai cli su **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="15bc3-128">Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="15bc3-129">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="15bc3-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="15bc3-130">**Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL.</span><span class="sxs-lookup"><span data-stu-id="15bc3-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="15bc3-131">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="15bc3-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="15bc3-132">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="15bc3-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="15bc3-133">Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="15bc3-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="15bc3-134">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="15bc3-135">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo che hanno inviato il contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="15bc3-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="15bc3-136">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="15bc3-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="15bc3-137">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="15bc3-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="15bc3-138">Dal centro per i **partner** selezionare **Customers**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-138">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="15bc3-139">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-139">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="15bc3-140">Fare clic su **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-140">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="15bc3-141">Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo.</span><span class="sxs-lookup"><span data-stu-id="15bc3-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="15bc3-142">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![elenco dei clienti](images/regionalcustomer2.png)

6.  <span data-ttu-id="15bc3-144">Fare clic su **Invia.**</span><span class="sxs-lookup"><span data-stu-id="15bc3-144">Click **Submit.**</span></span>

<span data-ttu-id="15bc3-145">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="15bc3-146">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="15bc3-147">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="15bc3-148">**Nota**  I partner devono sospendere le sottoscrizioni in **fase di transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all' **account del tenant partner nel** centro per assicurarsi che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-148">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="15bc3-149">Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="15bc3-150">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="15bc3-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="15bc3-151">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="15bc3-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="15bc3-152">Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="15bc3-153">Accedere al centro per i **partner** con l'account di **transizione da** CSP e passare all'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="15bc3-154">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="15bc3-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="15bc3-155">Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[! **Nota**]<span data-ttu-id="15bc3-156"> La sospensione della sottoscrizione garantisce che non si verifichi la doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-156"> Suspending the subscription ensures double billing does not occur.</span></span>

~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="15bc3-157">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="15bc3-158">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-158">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="15bc3-159">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="15bc3-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="15bc3-160">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="15bc3-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="15bc3-161">Azure, le sottoscrizioni CSP basate sull'utilizzo non devono essere migrate manualmente come nel caso delle sottoscrizioni di Office 365 CSP.</span><span class="sxs-lookup"><span data-stu-id="15bc3-161">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="15bc3-162">Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-162">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="15bc3-163">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-163">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="15bc3-164">Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-164">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="15bc3-165">I partner notificano a Microsoft quali account cliente che dispongono di sottoscrizioni di Azure sono pronti per la migrazione e forniscono i nomi delle società dei clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-165">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>
3.  <span data-ttu-id="15bc3-166">Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-166">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="15bc3-167">Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-167">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="15bc3-168">Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-168">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[! **Nota**]<span data-ttu-id="15bc3-169"> La disabilitazione delle sottoscrizioni del cliente non comporta la modifica dell'aspetto del cliente nell'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-169"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="15bc3-170">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="15bc3-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="15bc3-171">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="15bc3-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="15bc3-172">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="15bc3-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="15bc3-173">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="15bc3-174">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="15bc3-174">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="15bc3-175">Note</span><span class="sxs-lookup"><span data-stu-id="15bc3-175">Notes</span></span>

-   <span data-ttu-id="15bc3-176">La disabilitazione della sottoscrizione dalla **transizione dall'** account CSP non influisca sul servizio del cliente finale purché sia stato effettuato il provisioning del servizio dall'account **di transizione a** CSP prima di disabilitare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

-   <span data-ttu-id="15bc3-177">Le sottoscrizioni non possono essere utilizzate dal cliente e non generano addebiti quando vengono sospese o annullate.</span><span class="sxs-lookup"><span data-stu-id="15bc3-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

-   <span data-ttu-id="15bc3-178">Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="15bc3-178">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="15bc3-179">**Nota**  I partner devono sospendere le sottoscrizioni per la **transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all'account del tenant partner nel centro per i partner per garantire che non si **verifichi la doppia** fatturazione.</span><span class="sxs-lookup"><span data-stu-id="15bc3-179">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="15bc3-180">Microsoft non supporterà le richieste di crediti dovute a eventuali sovrapposizioni nella fatturazione che si verificano se non si imposta correttamente la **transizione dalle** sottoscrizioni a sospesa.</span><span class="sxs-lookup"><span data-stu-id="15bc3-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="15bc3-181">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="15bc3-181">Simplify migration using Export</span></span>

<span data-ttu-id="15bc3-182">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="15bc3-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="15bc3-183">Fare clic su **clienti** nel centro per i partner per visualizzare l'elenco dei clienti nella struttura esistente.</span><span class="sxs-lookup"><span data-stu-id="15bc3-183">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="15bc3-184">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="15bc3-184">Open the desired customer name.</span></span>

3.  <span data-ttu-id="15bc3-185">Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="15bc3-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="15bc3-186">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="15bc3-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="15bc3-187">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="15bc3-187">API registration</span></span>

<span data-ttu-id="15bc3-188">Per altre informazioni sulla registrazione dell'API, [vedi questa pagina](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="15bc3-188">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








