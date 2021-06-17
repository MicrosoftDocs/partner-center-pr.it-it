---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account dei clienti e delle sottoscrizioni dei clienti.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276876"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="d6df9-104">Istruzioni per il consolidamento dei tenant per l'autorizzazione regionale per CSP</span><span class="sxs-lookup"><span data-stu-id="d6df9-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="d6df9-105">**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d6df9-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d6df9-106">**Ruoli appropriati:** amministratore globale | Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="d6df9-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="d6df9-107">\[Alcune informazioni riguardano un prodotto pre-rilasciato che può essere modificato sostanzialmente prima del rilascio in commercio.</span><span class="sxs-lookup"><span data-stu-id="d6df9-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="d6df9-108">Microsoft non riconosce alcuna garanzia, espressa o implicita, in merito alle informazioni qui fornite.\]</span><span class="sxs-lookup"><span data-stu-id="d6df9-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="d6df9-109">È possibile consolidare i tenant per l'azienda.</span><span class="sxs-lookup"><span data-stu-id="d6df9-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="d6df9-110">Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.</span><span class="sxs-lookup"><span data-stu-id="d6df9-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="d6df9-111">È necessario conoscere tutti i conteggi delle sottoscrizioni e delle licenze di cui è stato effettuato il provisioning per ogni cliente nell'account da cui si esegue la transizione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="d6df9-112">Nell'ambito del processo di migrazione, verrà nuovamente provisioning delle stesse sottoscrizioni esatte con gli stessi conteggi delle licenze nel nuovo account CSP centrale.</span><span class="sxs-lookup"><span data-stu-id="d6df9-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="d6df9-113">Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.</span><span class="sxs-lookup"><span data-stu-id="d6df9-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="d6df9-114">Al termine del consolidamento, non è possibile ripristinare lo stato precedente del tenant.</span><span class="sxs-lookup"><span data-stu-id="d6df9-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="d6df9-115">Potrebbe essere necessaria anche l'azione del cliente.</span><span class="sxs-lookup"><span data-stu-id="d6df9-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="d6df9-116">Preparare la migrazione</span><span class="sxs-lookup"><span data-stu-id="d6df9-116">Prepare for migration</span></span>

- <span data-ttu-id="d6df9-117">Accedere a **Partner Center** l'account  di transizione (quello di cui si eseguirà la transizione al nuovo account) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="d6df9-118">Disconnettersi da questo account.</span><span class="sxs-lookup"><span data-stu-id="d6df9-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="d6df9-119">Eseguire la migrazione degli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="d6df9-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="d6df9-120">Accedere al **Partner Center**  con l'account **Transitioning** (nuovo) (quello in cui si sta effettuando la transizione dei clienti).</span><span class="sxs-lookup"><span data-stu-id="d6df9-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="d6df9-121">Seleziona **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-121">Select **Customers**.</span></span>

3. <span data-ttu-id="d6df9-122">Selezionare **Richiedi una relazione come rivenditore.**</span><span class="sxs-lookup"><span data-stu-id="d6df9-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="d6df9-123">Viene visualizzato un messaggio di posta elettronica predefinito da inviare ai clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="d6df9-124">Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d6df9-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="d6df9-125">**Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL.</span><span class="sxs-lookup"><span data-stu-id="d6df9-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="d6df9-126">All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="d6df9-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="d6df9-127">Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.</span><span class="sxs-lookup"><span data-stu-id="d6df9-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="d6df9-128">Dopo l'accesso, all'amministratore globale per **l'account** cliente viene richiesto di inviare un contratto che concede privilegi di amministratore delegato al nuovo account CSP.</span><span class="sxs-lookup"><span data-stu-id="d6df9-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="d6df9-129">Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="d6df9-130">I clienti verranno visualizzati nell'elenco dei clienti del partner dopo aver inviato il contratto, uno alla volta.</span><span class="sxs-lookup"><span data-stu-id="d6df9-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="d6df9-131">Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure</span><span class="sxs-lookup"><span data-stu-id="d6df9-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="d6df9-132">Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.</span><span class="sxs-lookup"><span data-stu-id="d6df9-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="d6df9-133">In **Partner Center** selezionare **Clienti.**</span><span class="sxs-lookup"><span data-stu-id="d6df9-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="d6df9-134">Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="d6df9-135">Selezionare **Aggiungi sottoscrizione**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="d6df9-136">Aggiungere le sottoscrizioni e i conteggi delle licenze corretti dal catalogo.</span><span class="sxs-lookup"><span data-stu-id="d6df9-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="d6df9-137">Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco di clienti.":::

6. <span data-ttu-id="d6df9-139">Selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="d6df9-139">Select **Submit.**</span></span>

   <span data-ttu-id="d6df9-140">I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="d6df9-141">Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="d6df9-142">Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="d6df9-143">I partner devono  sospendere le sottoscrizioni nell'account del tenant partner di transizione Partner Center stesso giorno  in cui tali sottoscrizioni vengono transizione e impostate nell'account del tenant partner di transizione nel Partner Center per garantire che non si verifichi una doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="d6df9-144">Le richieste di supporto verranno negate per i crediti a causa di eventuali sovrapposizioni nella fatturazione dovute alla disabilitazione non corretta delle sottoscrizioni di **transizione dalle** sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="d6df9-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="d6df9-145">Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione</span><span class="sxs-lookup"><span data-stu-id="d6df9-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="d6df9-146">La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future.</span><span class="sxs-lookup"><span data-stu-id="d6df9-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="d6df9-147">Non è necessario disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="d6df9-148">Accedere al portale di **Partner Center** con l'account **Transitioning From** CSP (Transizione da CSP) e passare all'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="d6df9-149">Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.</span><span class="sxs-lookup"><span data-stu-id="d6df9-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="d6df9-150">Impostare la sottoscrizione su **sospeso** e quindi selezionare **Invia.**</span><span class="sxs-lookup"><span data-stu-id="d6df9-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="d6df9-151">La sospensione della sottoscrizione garantisce che non si verifichi una doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="d6df9-152">La sottoscrizione viene visualizzata **come sospesa** nell'elenco delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="d6df9-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="d6df9-153">Ripeti questi passaggi per tutte le sottoscrizioni per il cliente.</span><span class="sxs-lookup"><span data-stu-id="d6df9-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="d6df9-154">Verifica che per tutte sia indicato lo stato **Sospeso**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="d6df9-155">Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="d6df9-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="d6df9-156">Migrazione di sottoscrizioni in base all'uso di Azure</span><span class="sxs-lookup"><span data-stu-id="d6df9-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="d6df9-157">A differenza delle sottoscrizioni CSP di Office 365, non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP basate sull'utilizzo di Azure.</span><span class="sxs-lookup"><span data-stu-id="d6df9-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="d6df9-158">Microsoft Azure supporto tecnico eseguirà la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuite dagli account rivenditore **CSP** all'account del rivenditore **di** transizione a CSP.</span><span class="sxs-lookup"><span data-stu-id="d6df9-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="d6df9-159">Non ci saranno interruzioni del servizio per il cliente durante la transizione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="d6df9-160">Assicurarsi che gli account dei clienti di cui verrà eseguita la migrazione delle sottoscrizioni di Azure abbia accettato il contratto da associare al nuovo account di transizione **a** CSP.</span><span class="sxs-lookup"><span data-stu-id="d6df9-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="d6df9-161">Si invierà una notifica a Microsoft degli account dei clienti pronti per la migrazione e si forniranno i nomi delle società del cliente.</span><span class="sxs-lookup"><span data-stu-id="d6df9-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="d6df9-162">Microsoft esegue la migrazione delle sottoscrizioni basate sull'utilizzo di Azure e invia una notifica al termine della migrazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="d6df9-163">È necessario verificare che la sottoscrizione di Azure nell'account  del rivenditore **Transitioning From** CSP (Transizione da rivenditore CSP) sia ora contrassegnata come sospesa Partner Center nella sezione sottoscrizioni dei clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="d6df9-164">Verificare che la sottoscrizione di Azure nell'account del rivenditore **Di** transizione a CSP ora mostra lo stato attivo **Partner Center** nella sezione sottoscrizioni dei clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="d6df9-165">La disabilitazione delle sottoscrizioni del cliente non modifica l'aspetto del cliente nell'elenco Clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="d6df9-166">Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="d6df9-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="d6df9-167">I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.</span><span class="sxs-lookup"><span data-stu-id="d6df9-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="d6df9-168">Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**.</span><span class="sxs-lookup"><span data-stu-id="d6df9-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="d6df9-169">Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="d6df9-170">Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.</span><span class="sxs-lookup"><span data-stu-id="d6df9-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="d6df9-171">Informazioni aggiuntive</span><span class="sxs-lookup"><span data-stu-id="d6df9-171">Additional information</span></span>

- <span data-ttu-id="d6df9-172">La disabilitazione della sottoscrizione dall'account **CSP** di transizione non influisce sul servizio del cliente finale, purché sia stato effettuato il provisioning del servizio dall'account di transizione a **CSP** prima di disabilitare la sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="d6df9-173">Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.</span><span class="sxs-lookup"><span data-stu-id="d6df9-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="d6df9-174">Attualmente non è possibile rimuovere completamente un cliente **dall'elenco Clienti.**</span><span class="sxs-lookup"><span data-stu-id="d6df9-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="d6df9-175">I partner devono sospendere le sottoscrizioni nell'account **del** tenant partner di transizione da Partner Center stesso giorno in cui tali sottoscrizioni vengono impostate e impostate nell'account  di transizione a per garantire che non si verifichi una doppia fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d6df9-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="d6df9-176">Microsoft non supporterà le richieste di crediti a causa di  eventuali sovrapposizioni nella fatturazione dovute all'impostazione non corretta delle sottoscrizioni di transizione da a sospeso.</span><span class="sxs-lookup"><span data-stu-id="d6df9-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="d6df9-177">Semplificare la migrazione con l'esportazione</span><span class="sxs-lookup"><span data-stu-id="d6df9-177">Simplify migration using Export</span></span>

<span data-ttu-id="d6df9-178">La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:</span><span class="sxs-lookup"><span data-stu-id="d6df9-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="d6df9-179">Selezionare **Clienti** nella Partner Center per visualizzare l'elenco dei clienti.</span><span class="sxs-lookup"><span data-stu-id="d6df9-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="d6df9-180">Apri il nome del cliente desiderato.</span><span class="sxs-lookup"><span data-stu-id="d6df9-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="d6df9-181">Nella pagina **Sottoscrizioni** selezionare Esporta **sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.</span><span class="sxs-lookup"><span data-stu-id="d6df9-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="d6df9-182">Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.</span><span class="sxs-lookup"><span data-stu-id="d6df9-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="d6df9-183">Registrazione dell'API</span><span class="sxs-lookup"><span data-stu-id="d6df9-183">API registration</span></span>

<span data-ttu-id="d6df9-184">Per altre informazioni sulla registrazione dell'API, vedere [Configurare l'accesso all'API in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="d6df9-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d6df9-185">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d6df9-185">Next steps</span></span>

- [<span data-ttu-id="d6df9-186">Cloud Solution Provider mercati e valute regionali del programma in cui è possibile vendere offerte CSP</span><span class="sxs-lookup"><span data-stu-id="d6df9-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
