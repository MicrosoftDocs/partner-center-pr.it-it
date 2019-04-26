---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: article
ms.date: 03/15/2019
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: migrazione dei clienti, provisioning, account tenant, consolidamento dei tenant
ms.localizationpriority: medium
ms.openlocfilehash: c2226fea4523b5f34a2cb1b5fcfcde88048dda82
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134780"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="ce7d0-104">Consolidamento dei tenant per l'autorizzazione regionale per CSP</span><span class="sxs-lookup"><span data-stu-id="ce7d0-104">CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="ce7d0-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="ce7d0-105">**Applies to**</span></span>

-  <span data-ttu-id="ce7d0-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ce7d0-106">Partner Center</span></span>
-  <span data-ttu-id="ce7d0-107">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="ce7d0-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="ce7d0-108">\[Alcune informazioni si riferiscono al prodotto non definitivo che può essere modificato sostanzialmente prima del rilascio in commercio.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="ce7d0-109">Microsoft non rilascia alcuna garanzia, espressa o implicita, relativamente alle informazioni fornite di seguito.\]</span><span class="sxs-lookup"><span data-stu-id="ce7d0-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="ce7d0-110">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="ce7d0-111">**Nota** Devi conoscere tutte le sottoscrizioni e il numero di postazioni per i tuoi clienti di cui è stato eseguito il provisioning dagli account per la transizione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="ce7d0-112">Nell'ambito del processo di migrazione, dovrai eseguire nuovamente il provisioning degli stessi esatti abbonamenti con lo stesso numero di postazioni nel nuovo account CSP centralizzato.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="ce7d0-113">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="ce7d0-114">Il consolidamento dei tenant è una scelta del partner.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="ce7d0-115">Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="ce7d0-116">Tieni presente che potrebbe essere richiesto anche l'intervento dei clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-116">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="ce7d0-117">Prepararsi per la migrazione</span><span class="sxs-lookup"><span data-stu-id="ce7d0-117">Prepare for migration</span></span>


-   <span data-ttu-id="ce7d0-118">Accedi per i **Centro per i Partner** con il **dedicata alla transizione** account (esistente) (quello passerà) e prendere nota di tutti i clienti e tutti i servizi di provisioning per i clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-118">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![elenco dei clienti regionali](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="ce7d0-120">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="ce7d0-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="ce7d0-121">Accedi per i **Centro per i Partner** con il **dedicata alla transizione** (nuovo) dell'account (quello che stanno passando a) e passare all'elenco di clienti dal **clienti**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-121">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="ce7d0-122">Seleziona Clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-122">Select Customers.</span></span>

3.  <span data-ttu-id="ce7d0-123">Fai cli su **Richiedi una relazione come rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="ce7d0-124">Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="ce7d0-125">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="ce7d0-126">**Azione del cliente:** Assicurarsi che ogni cliente active che si vuole eseguire la migrazione visita questo URL.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="ce7d0-127">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="ce7d0-128">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="ce7d0-129">Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="ce7d0-130">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="ce7d0-131">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo l'invio del contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="ce7d0-132">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="ce7d0-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="ce7d0-133">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="ce7d0-134">Dal **Centro per i Partner** selezionate **clienti**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-134">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="ce7d0-135">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="ce7d0-136">Fai clic su **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="ce7d0-137">Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="ce7d0-138">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![elenco di clienti](images/regionalcustomer2.png)

6.  <span data-ttu-id="ce7d0-140">Fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-140">Click **Submit.**</span></span>

<span data-ttu-id="ce7d0-141">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ce7d0-142">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="ce7d0-143">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ce7d0-144">**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ce7d0-145">Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="ce7d0-146">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="ce7d0-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="ce7d0-147">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="ce7d0-148">Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="ce7d0-149">Accedi per il **Centro per i Partner** con il **in fase di transizione da** CSP di account e passare all'elenco di clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-149">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="ce7d0-150">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="ce7d0-151">Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[! **Nota**]<span data-ttu-id="ce7d0-152"> sospensione della sottoscrizione assicura provochi una fatturazione non si verifica.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-152"> Suspending the subscription ensures double billing does not occur.</span></span>



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="ce7d0-153">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="ce7d0-154">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-154">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="ce7d0-155">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="ce7d0-156">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="ce7d0-156">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="ce7d0-157">Nota che non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP in base all'uso di Azure come nel caso delle sottoscrizioni CSP di Office 365.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-157">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="ce7d0-158">Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-158">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="ce7d0-159">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-159">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="ce7d0-160">Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-160">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="ce7d0-161">I partner comunicano a Microsoft gli account dei clienti con sottoscrizioni di Azure pronti per la migrazione e forniscono i nomi dell'azienda dei clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-161">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="ce7d0-162">Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-162">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="ce7d0-163">Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-163">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="ce7d0-164">Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-164">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[! **Nota**]<span data-ttu-id="ce7d0-165"> la disabilitazione di sottoscrizioni per il cliente non modifica l'aspetto del cliente nell'elenco di clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-165"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="ce7d0-166">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="ce7d0-167">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="ce7d0-168">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="ce7d0-169">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="ce7d0-170">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-170">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="ce7d0-171">Note</span><span class="sxs-lookup"><span data-stu-id="ce7d0-171">Notes</span></span>

-   <span data-ttu-id="ce7d0-172">Disabilitare la sottoscrizione dall'account CSP di **origine della transizione** non influisce sul servizio del cliente finale, a condizione che il provisioning del servizio sia stato eseguito dall'account CSP di **destinazione della transizione** prima della disabilitazione.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="ce7d0-173">Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="ce7d0-174">Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-174">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="ce7d0-175">**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-175">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ce7d0-176">Microsoft non supporterà le richieste di accrediti causate da eventuali sovrapposizioni nella fatturazione dovute alla mancata sospensione delle sottoscrizioni nell'**origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-176">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="ce7d0-177">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="ce7d0-177">Simplify migration using Export</span></span>

<span data-ttu-id="ce7d0-178">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="ce7d0-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="ce7d0-179">Fare clic su **clienti** nel centro per i Partner per visualizzare l'elenco di clienti in una struttura esistente.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-179">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="ce7d0-180">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-180">Open the desired customer name.</span></span>

3.  <span data-ttu-id="ce7d0-181">Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-181">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="ce7d0-182">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="ce7d0-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="ce7d0-183">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="ce7d0-183">API registration</span></span>

<span data-ttu-id="ce7d0-184">Per altre informazioni sulla registrazione dell'API, [vedi questa pagina](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="ce7d0-184">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








