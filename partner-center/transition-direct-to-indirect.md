---
title: Passa direttamente alla fattura partner a rivenditori indiretti
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sul modo in cui un partner del programma CSP può usare il centro per i partner per la transizione dal partner Direct-Bill al rivenditore indiretto.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795866"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="d3dc9-103">Transizione da partner CSP (Cloud Solution Provider) con fatturazione diretta a rivenditore CSP indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="d3dc9-104">**Si applica a:**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-104">**Applies to:**</span></span>
- <span data-ttu-id="d3dc9-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d3dc9-105">Partner Center</span></span>

<span data-ttu-id="d3dc9-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-106">**Appropriate roles**</span></span>

- <span data-ttu-id="d3dc9-107">Tutti i partner CSP con fatturazione diretta</span><span class="sxs-lookup"><span data-stu-id="d3dc9-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="d3dc9-108">Questo articolo è destinato ai partner di fatturazione diretta che hanno deciso di passare a rivenditori indiretti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="d3dc9-109">Tuttavia, anche se non si è ancora preso una decisione esplicita per la registrazione come rivenditore indiretto, i partner diretti della fatturazione che non soddisfano i nuovi [requisiti](direct-partner-new-requirements.md) per il programma per la fatturazione diretta di CSP saranno informati da Microsoft quando le relative [funzionalità di fatturazione diretta saranno limitate](restricted-direct-bill-capabilities.md).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="d3dc9-110">Al 2021 gennaio verrà aggiunto un nuovo requisito di ricavi.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="d3dc9-111">I partner iscritti come partner di fatturazione diretta dovranno avere effettuato transazioni per almeno USD $300K in un programma Cloud Solution Provider ricavi a un livello di conto globale del partner nei 12 mesi precedenti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="d3dc9-112">Sarà possibile eseguire la registrazione al programma indirect Reseller usando il tenant di fatturazione diretta esistente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="d3dc9-113">Introduzione</span><span class="sxs-lookup"><span data-stu-id="d3dc9-113">Get started</span></span>

1. <span data-ttu-id="d3dc9-114">Verificare che il profilo partner nel centro per i partner e l'ID MPN siano aggiornati.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="d3dc9-115">Accedere al centro per i partner come amministratore globale per il tenant di fatturazione diretta che si sta passando al rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Overview":::

3. <span data-ttu-id="d3dc9-117">Esaminare i dettagli del partner nel modulo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Iscriviti ora":::

4. <span data-ttu-id="d3dc9-119">Selezionare Registrati ora.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-119">Select Enroll now.</span></span> <span data-ttu-id="d3dc9-120">L'azienda del rivenditore indiretto userà lo stesso tenant di AAD usato per l'azienda diretta.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d3dc9-121">Inizialmente, questa nuova funzionalità di transizione sarà disponibile per i partner la cui data dell'anniversario ricorre da settembre a dicembre.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="d3dc9-122">Se non si ha una data di anniversario tra settembre e dicembre, non sarà possibile visualizzare la funzionalità in questo momento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="d3dc9-123">I partner la cui data dell'anniversario è successiva a dicembre 2018 riceveranno una notifica in un secondo momento, quando la funzionalità sarà abilitata anche per loro.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="d3dc9-124">Quando la registrazione è approvata, accedere di nuovo a partner Center.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d3dc9-125">Mentre l'approvazione è in genere immediata, possono essere importati fino a cinque giorni lavorativi.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="d3dc9-126">Una volta approvata, si riceverà una notifica per l'indirizzo di posta elettronica specificato in contatto principale nel modulo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="d3dc9-127">È anche possibile controllare lo stato di registrazione in **Impostazioni**  >  **partner impostazioni partner**  >  **profilo** > informazioni sul programma.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="d3dc9-128">Nella pagina **Panoramica** viene visualizzato il contratto di rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="d3dc9-129">Seleziona **Accetta e continua** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-129">Select **Accept and continue** .</span></span> <span data-ttu-id="d3dc9-130">Questa azione Abilita le funzionalità dei rivenditori indiretti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="d3dc9-131">Dopo aver accettato il contratto di rivenditore indiretto, si noti che il profilo partner identifica l'utente **come fattura** diretta e rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Contratto rivenditore indiretto":::

> [!IMPORTANT]
> <span data-ttu-id="d3dc9-133">Una volta eseguita la registrazione come rivenditore indiretto tramite la nuova funzionalità, non è possibile eseguire il rollback a un tenant diretto di sola fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="d3dc9-134">Assicurati di prendere in considerazione tutte le tue esigenze aziendali prima eseguire la registrazione come rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="d3dc9-135">Durante la transizione da diretto a rivenditore indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="d3dc9-136">Durante questa fase, si continuerà a gestire le esigenze di sottoscrizione dirette dei clienti, incluso il processo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="d3dc9-137">È anche possibile iniziare ad accettare i clienti dal provider indiretto e operare come rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Sei una fattura diretta e un rivenditore indiretto":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="d3dc9-139">Trovare un provider indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-139">Find an indirect provider</span></span>

<span data-ttu-id="d3dc9-140">Dopo la registrazione, nel NAV di sinistra verrà visualizzato un collegamento a provider indiretti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="d3dc9-141">I rivenditori indiretti stabiliscono una relazione con un provider indiretto che può gestire la fatturazione, acquistare prodotti per i clienti e supportare l'infrastruttura.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="d3dc9-142">Il supporto e i servizi offerti variano a seconda del provider indiretto scelto. Valutare pertanto i provider presenti nella propria zona per individuare quelli che soddisfano meglio le proprie esigenze.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="d3dc9-143">In genere, la maggior parte dei provider:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-143">Generally, most providers will:</span></span>

- <span data-ttu-id="d3dc9-144">Fornisce al rivenditore assistenza e formazione tecnica</span><span class="sxs-lookup"><span data-stu-id="d3dc9-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="d3dc9-145">Aiuta il rivenditore a commercializzare prodotti e servizi</span><span class="sxs-lookup"><span data-stu-id="d3dc9-145">Help you market your products and services</span></span>
- <span data-ttu-id="d3dc9-146">Gestione delle condizioni di credito e di finanziamento</span><span class="sxs-lookup"><span data-stu-id="d3dc9-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="d3dc9-147">Eseguire una ricerca nell'elenco dei [provider Microsoft indiretti](https://partnercenter.microsoft.com/partner/find-a-provider)ufficiali.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="d3dc9-148">Altre informazioni, leggere  [partner con provider indiretti](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="d3dc9-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="d3dc9-149">Accetta un invito a una partnership dal provider indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="d3dc9-150">Quando si trova un provider indiretto per collaborare con, stabilire una relazione con il provider indiretto nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="d3dc9-151">Il provider indiretto selezionato invierà all'utente un collegamento di invito tramite posta elettronica che consentirà di passare all'invito nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="d3dc9-152">Assicurarsi che l'amministratore globale acceda al centro per i partner e segua il collegamento all'invito.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="d3dc9-153">Quando si accetta l'invito, il nome del provider verrà visualizzato nell'elenco provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="d3dc9-154">Acquisisci nuovi clienti come rivenditore indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="d3dc9-155">È necessario che l'utente e il provider indiretto dispongano di relazioni rivenditore con i clienti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="d3dc9-156">Queste relazioni dei rivenditori consentono di gestire le sottoscrizioni e i servizi di un cliente per loro conto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="d3dc9-157">Per acquisire un nuovo cliente che disponga di un tenant di Azure AD esistente, è possibile invitare il cliente a stabilire una relazione di rivenditore con l'utente e il provider nello stesso momento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="d3dc9-158">Per creare un invito al rivenditore indiretto:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="d3dc9-159">Selezionare **provider indiretti** dal navigatore a sinistra del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="d3dc9-160">Selezionare **Invita nuovi clienti** per invitare il cliente a stabilire contemporaneamente una relazione come rivenditore con l'utente e il provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="d3dc9-161">Il provider deve avere una relazione di rivenditore con il cliente, in modo che possa inviare ordini per conto del cliente quando il cliente desidera acquistare nuove sottoscrizioni o aggiungere nuove licenze alle sottoscrizioni esistenti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="d3dc9-162">Nella pagina successiva esaminare la bozza del messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="d3dc9-163">È possibile aprire il messaggio bozza in un messaggio di posta elettronica oppure copiarlo negli Appunti e incollarlo in un messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="d3dc9-164">Modificare il testo del messaggio di posta elettronica per indicare gli elementi necessari, ma assicurarsi di includere il collegamento in quanto è personalizzato per connettere il cliente direttamente al proprio account e al proprio account del provider.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="d3dc9-165">Al termine selezionare **Done** (Fine).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-165">Then select **Done** .</span></span>

5. <span data-ttu-id="d3dc9-166">Dopo che il cliente ha autorizzato te e il provider a diventare i suoi Reseller of Record, avrai le autorizzazioni di amministratore necessarie per gestire sottoscrizioni, licenze e utenti per conto del cliente e il provider indiretto potrà inviare ordini per conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="d3dc9-167">Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandi il record del cliente selezionando la freccia verso il basso accanto al nome.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="d3dc9-168">Diversamente dai partner Direct Bill, i rivenditori indiretti non possono creare tenant Azure AD per i nuovi clienti nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="d3dc9-169">Il provider creerà il tenant e verrà specificato come rivenditore indiretto per questo cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="d3dc9-170">Ciò garantisce che il cliente venga visualizzato nell'elenco dei clienti nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="d3dc9-171">Non sarà possibile utilizzare la funzionalità di fatturazione diretta per creare acquisti per i clienti acquisiti come rivenditori indiretti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="d3dc9-172">Gestione dei clienti Direct fattura e dei clienti indiretti del rivenditore</span><span class="sxs-lookup"><span data-stu-id="d3dc9-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="d3dc9-173">È possibile gestire in modo diverso i clienti Direct fattura e i clienti indiretti del rivenditore.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="d3dc9-174">Fatturazione diretta dei clienti (operazioni che non verranno eseguite come rivenditore indiretto)</span><span class="sxs-lookup"><span data-stu-id="d3dc9-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="d3dc9-175">Creare ordini per i prodotti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-175">Create orders for products</span></span>
- <span data-ttu-id="d3dc9-176">Gestire le prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="d3dc9-176">Manage Azure reservations</span></span>
- <span data-ttu-id="d3dc9-177">Gestire la cronologia degli ordini</span><span class="sxs-lookup"><span data-stu-id="d3dc9-177">Manage their order history</span></span>
- <span data-ttu-id="d3dc9-178">Acquistare software</span><span class="sxs-lookup"><span data-stu-id="d3dc9-178">Purchase software</span></span>
- <span data-ttu-id="d3dc9-179">Fatturazione diretta dei clienti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="d3dc9-180">Clienti rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-180">Indirect reseller customers</span></span>

- <span data-ttu-id="d3dc9-181">Il provider indiretto Ordina i prodotti per i clienti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="d3dc9-182">Gestione delle licenze e degli utenti dei clienti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="d3dc9-183">Gestire i rinnovi delle sottoscrizioni</span><span class="sxs-lookup"><span data-stu-id="d3dc9-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="d3dc9-184">Per identificare i clienti acquisiti come partner per la fatturazione diretta</span><span class="sxs-lookup"><span data-stu-id="d3dc9-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="d3dc9-185">Selezione **clienti**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-185">Select **Customers**</span></span>

2. <span data-ttu-id="d3dc9-186">Selezionare un cliente per visualizzarne i dettagli</span><span class="sxs-lookup"><span data-stu-id="d3dc9-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="d3dc9-187">Se questo cliente è stato acquisito come partner Direct fattura, verranno visualizzate le opzioni per **aggiungere** o visualizzare i **prodotti** e verranno visualizzate le relative sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="d3dc9-188">Se il cliente ha una relazione di rivenditore indiretta, queste opzioni non saranno disponibili.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="d3dc9-189">Sposta i clienti diretti della fatturazione al provider indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="d3dc9-190">Il provider indiretto non può inviare ordini o trasferimenti di sottoscrizione esistenti per i clienti con fatturazione diretta esistente finché non hanno una relazione di rivenditore.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="d3dc9-191">Per stabilire la relazione del rivenditore tra il provider indiretto e il cliente di fatturazione diretta esistente, è possibile utilizzare uno dei metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="d3dc9-192">Estensione relazione rivenditore</span><span class="sxs-lookup"><span data-stu-id="d3dc9-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="d3dc9-193">Invia un invito del rivenditore indiretto al cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="d3dc9-194">Per una panoramica dettagliata del processo step-by-Step, vedere il documento relativo alla [transizione diretta a indiretta](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="d3dc9-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="d3dc9-195">Estensione relazione rivenditore</span><span class="sxs-lookup"><span data-stu-id="d3dc9-195">Reseller relationship extension</span></span>

<span data-ttu-id="d3dc9-196">È possibile utilizzare la funzionalità di estensione delle relazioni rivenditore per stabilire la relazione del rivenditore tra i clienti di fatturazione diretta esistenti e il provider indiretto tramite il dashboard del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="d3dc9-197">Prima di usare la funzionalità, tenere presente quanto segue:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="d3dc9-198">Questa funzionalità è disponibile solo per i partner Direct fattura che eseguono la transizione per diventare un rivenditore indiretto ha completato la [registrazione indiretta del rivenditore](#get-started).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="d3dc9-199">È possibile applicare questa funzionalità solo ai clienti con fatturazione diretta esistente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="d3dc9-200">Non è applicabile ai [clienti di rivenditori indiretti](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="d3dc9-201">È possibile selezionare solo un provider indiretto per il quale è stato [accettato un invito partner dal provider indiretto](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="d3dc9-202">Una copia delle informazioni fatturate per il cliente verrà resa disponibile al provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="d3dc9-203">Per accedere alle informazioni sulla fatturazione, accedere alla pagina dell'account del cliente nel dashboard del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d3dc9-204">Utilizzando la funzionalità di estensione Reseller Relationship, il cliente acconsente a condividere le informazioni fatturate per il cliente con il provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="d3dc9-205">Il provider indiretto non verrà fornito con [privilegi di amministrazione delegata](customers-revoke-admin-privileges.md) al tenant del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="d3dc9-206">Se il provider indiretto richiede privilegi di amministrazione delegata, è necessario inviare invece un invito al rivenditore indiretto al cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="d3dc9-207">Una volta stabilita la relazione Reseller, il provider indiretto verrà visualizzato come partner CSP per il cliente nella pagina Relazioni partner nell'interfaccia di [amministrazione di M365](https://admin.microsoft.com/AdminPortal/Home#/partners) e [Microsoft Store for business](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="d3dc9-208">Per evitare confusione e fraintendimenti, l'utente è obbligato dal contratto del partner per informare e ottenere il consenso del cliente Direct Bill prima di utilizzare la funzionalità di estensione delle relazioni per stabilire la relazione del rivenditore tra un cliente di fatturazione diretta esistente e un provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="d3dc9-209">Per usare questa funzionalità in un tenant del cliente esistente:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="d3dc9-210">Accedere al centro per i partner come **agente di amministrazione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="d3dc9-211">Nella **pagina clienti** selezionare un cliente esistente e fare clic sull'icona **collegamenti rapidi** per espandere la visualizzazione riepilogativa del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="d3dc9-212">In **provider/i indiretti** , fare clic **su Trasferisci cliente per un provider indiretto** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Trasferire il cliente a un provider indiretto":::

4. <span data-ttu-id="d3dc9-214">Nella finestra di dialogo popup selezionare il **provider indiretto** a cui si vuole associare il cliente per la relazione Reseller.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="d3dc9-215">Fare clic su **Salva e continua** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="d3dc9-216">Verificare che il provider indiretto selezionato venga visualizzato sotto **provider indiretti** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Provider indiretto elencato":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="d3dc9-218">Invia un invito del rivenditore indiretto al cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="d3dc9-219">Il provider indiretto non può inviare ordini per i clienti con fatturazione diretta esistente fino a quando non hanno una relazione di rivenditore.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="d3dc9-220">Per stabilire la relazione del rivenditore tra i clienti esistenti e il provider indiretto, invitare il cliente usando un invito al rivenditore indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="d3dc9-221">Selezionare **provider indiretti** dal navigatore a sinistra del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="d3dc9-222">Selezionare **Invita nuovi clienti** per invitare il cliente a stabilire contemporaneamente una relazione come rivenditore con l'utente e il provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="d3dc9-223">Il provider deve avere una relazione di rivenditore con il cliente, in modo che possa inviare ordini per conto del cliente quando il cliente desidera acquistare nuove sottoscrizioni o aggiungere nuove licenze alle sottoscrizioni esistenti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Invita nuovi clienti":::

3. <span data-ttu-id="d3dc9-225">Nella pagina successiva esaminare la bozza del messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="d3dc9-226">È possibile aprire il messaggio bozza in un messaggio di posta elettronica oppure copiarlo negli Appunti e incollarlo in un messaggio di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="d3dc9-227">Modificare il testo del messaggio di posta elettronica per indicare gli elementi necessari, ma assicurarsi di includere il collegamento in quanto è personalizzato per connettere il cliente direttamente al proprio account e al proprio account del provider.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="d3dc9-228">Al termine selezionare **Done** (Fine).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-228">Then select **Done** .</span></span>

5. <span data-ttu-id="d3dc9-229">Dopo che il cliente ha autorizzato te e il provider a diventare i suoi Reseller of Record, avrai le autorizzazioni di amministratore necessarie per gestire sottoscrizioni, licenze e utenti per conto del cliente e il provider indiretto potrà inviare ordini per conto del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="d3dc9-230">Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandi il record del cliente selezionando la freccia verso il basso accanto al nome.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="d3dc9-231">Accettazione del contratto clienti Microsoft</span><span class="sxs-lookup"><span data-stu-id="d3dc9-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="d3dc9-232">Microsoft Cloud contratto è valido fino al 31 gennaio 2020.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="d3dc9-233">Dopo tale data, tutti i clienti, esistenti e nuovi, devono firmare il nuovo contratto per i clienti [Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="d3dc9-234">Per la transizione dei clienti, se:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="d3dc9-235">**Il cliente non ha ancora accettato il contratto cliente Microsoft**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="d3dc9-236">Collaborare con il provider indiretto per chiedere al cliente di [accettare il contratto per i clienti Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="d3dc9-237">**Il cliente ha accettato il contratto per i clienti Microsoft attraverso l'interfaccia di amministrazione di Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="d3dc9-238">L'accettazione verrà mantenuta dopo che la relazione del rivenditore viene stabilita con il provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="d3dc9-239">Non è necessario eseguire alcuna operazione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="d3dc9-240">**Il cliente ha accettato il contratto per i clienti Microsoft tramite l'attestazione partner**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="d3dc9-241">L'accettazione non verrà mantenuta.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-241">The acceptance will not be retained.</span></span> <span data-ttu-id="d3dc9-242">Collaborare con il provider indiretto per [aggiornare l'accettazione del cliente nel centro per i partner](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="d3dc9-243">Trasferire le sottoscrizioni di fatturazione diretta esistenti al provider indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="d3dc9-244">In base al modello CSP indiretto, i rivenditori indiretti non hanno relazioni di fatturazione con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="d3dc9-245">Al contrario, i rivenditori indiretti ottengono le sottoscrizioni per i clienti tramite i provider indiretti.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="d3dc9-246">Durante la transizione da Direct Bill partner a Reseller indirect, è necessario trasferire le sottoscrizioni esistenti come partner Direct Bill al provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="d3dc9-247">A tale scopo, è possibile usare la funzionalità di trasferimento di sottoscrizioni autogestite nel dashboard del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="d3dc9-248">Prerequisiti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-248">Pre-requisites</span></span>

- <span data-ttu-id="d3dc9-249">Questa funzionalità è disponibile solo per i partner di transizione che hanno completato la registrazione indiretta dei rivenditori usando i tenant di Direct Bill partner esistenti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="d3dc9-250">Prima di trasferire le sottoscrizioni associate a un determinato cliente, il partner di transizione deve spostare il cliente a un provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="d3dc9-251">Il cliente deve avere [accettato il contratto per i clienti Microsoft attraverso il provider indiretto](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="d3dc9-252">Come passare allo stato rivenditore indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="d3dc9-253">La funzionalità è un processo in quattro passaggi, in cui:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="d3dc9-254">Il partner di transizione crea una richiesta di trasferimento della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="d3dc9-255">La richiesta contiene una o più sottoscrizioni esistenti associate allo stesso cliente ed è destinata a un provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="d3dc9-256">Il provider indiretto esamina e accetta (o rifiuta) la richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="d3dc9-257">Il provider indiretto verifica che la richiesta di trasferimento sia stata completata.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="d3dc9-258">Il partner di transizione verifica che la richiesta di trasferimento sia stata completata.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="d3dc9-259">Partner di transizione</span><span class="sxs-lookup"><span data-stu-id="d3dc9-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="d3dc9-260">È anche possibile usare il centro per i [partner API/SDK](/partner-center/develop/manage-customers) per trasferire le sottoscrizioni esistenti al provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="d3dc9-261">Ottenere l'idoneità al trasferimento degli abbonamenti di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="d3dc9-262">Creare il trasferimento di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="d3dc9-263">Ritirare il trasferimento di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="d3dc9-264">Accettare il trasferimento di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="d3dc9-265">Rifiutare il trasferimento di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="d3dc9-266">Ottenere i trasferimenti di un cliente</span><span class="sxs-lookup"><span data-stu-id="d3dc9-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="d3dc9-267">Ottenere i dettagli del trasferimento in base all'ID</span><span class="sxs-lookup"><span data-stu-id="d3dc9-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="d3dc9-268">Partner di transizione-creazione della richiesta di trasferimento</span><span class="sxs-lookup"><span data-stu-id="d3dc9-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="d3dc9-269">Per creare una richiesta di trasferimento come partner di transizione:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="d3dc9-270">Accedere al centro per i partner come **agente di amministrazione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="d3dc9-271">Nella pagina **clienti** selezionare il cliente desiderato e fare clic sull'icona collegamenti rapidi per espandere la visualizzazione riepilogativa del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="d3dc9-272">In **provider o provider indiretti** verificare che sia elencato il provider indiretto designato.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="d3dc9-273">Fare clic su **Visualizza sottoscrizioni** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="d3dc9-274">Nella pagina **sottoscrizioni** cercare trasferimento della **sottoscrizione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="d3dc9-275">In **trasferimento sottoscrizione** fare clic su **Richiedi trasferimento sottoscrizione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Richiedi trasferimento sottoscrizione":::

7. <span data-ttu-id="d3dc9-277">Nella finestra di dialogo richiesta di trasferimento selezionare una o più sottoscrizioni da trasferire.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Creazione della richiesta di trasferimento":::

8. <span data-ttu-id="d3dc9-279">Fare clic su **Crea** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-279">Click **Create** .</span></span>

9. <span data-ttu-id="d3dc9-280">Una richiesta di trasferimento di sottoscrizione attiva verrà visualizzata in **trasferimento sottoscrizione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Elenco richieste di trasferimento":::

10. <span data-ttu-id="d3dc9-282">Informare il provider indiretto che è stata creata una richiesta di trasferimento della sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="d3dc9-283">Provider indiretto-richiesta di trasferimento Accept</span><span class="sxs-lookup"><span data-stu-id="d3dc9-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="d3dc9-284">Per esaminare e accettare una richiesta di trasferimento come provider indiretto:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="d3dc9-285">Accedere al centro per i partner come agente di **Amministrazione** o **agente di vendita** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="d3dc9-286">Nella pagina **clienti** selezionare il cliente desiderato e fare clic sull'icona collegamenti rapidi per espandere la visualizzazione riepilogativa del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="d3dc9-287">In **rivenditori indiretti** verificare che sia elencato il partner di transizione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="d3dc9-288">Fare clic su **Visualizza sottoscrizioni** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="d3dc9-289">Nella pagina **sottoscrizioni** cercare trasferimento della **sottoscrizione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Visualizza la richiesta di trasferimento":::

6. <span data-ttu-id="d3dc9-291">In **trasferimento sottoscrizione** fare clic sulla richiesta di trasferimento da rivedere.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="d3dc9-292">Fare clic su **Accept** (o **Reject** ) in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Accetta richiesta di trasferimento":::

8. <span data-ttu-id="d3dc9-294">Attendere il completamento della richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="d3dc9-295">Provider indiretto: verifica della richiesta di trasferimento completata</span><span class="sxs-lookup"><span data-stu-id="d3dc9-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="d3dc9-296">Al termine della richiesta di trasferimento, verificare che le sottoscrizioni vengano visualizzate in **sottoscrizioni** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="d3dc9-297">Informare il partner di transizione.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="d3dc9-298">Partner di transizione: verifica della richiesta di trasferimento completata</span><span class="sxs-lookup"><span data-stu-id="d3dc9-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="d3dc9-299">Il partner di transizione deve eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="d3dc9-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="d3dc9-300">Accedere al centro per i partner come **agente di amministrazione** o agente di **vendita** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="d3dc9-301">Nella pagina **clienti** selezionare il cliente desiderato e fare clic sull'icona **collegamenti rapidi** per espandere la visualizzazione riepilogativa del cliente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="d3dc9-302">Fare clic su **Visualizza sottoscrizioni** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="d3dc9-303">Nella pagina **sottoscrizioni** cercare trasferimento della **sottoscrizione** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="d3dc9-304">Verificare che la richiesta di trasferimento sia contrassegnata come **completa** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="d3dc9-305">Verificare che le sottoscrizioni non vengano più visualizzate come attive nella pagina **sottoscrizioni** :</span><span class="sxs-lookup"><span data-stu-id="d3dc9-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="d3dc9-306">Se si tratta di una sottoscrizione di Azure (MS-AZR-0145P), non verrà più elencata.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="d3dc9-307">Se si tratta di una sottoscrizione basata su licenza (Office 365, Dynamics, Intune), questa verrà elencata con stato come **sospesa** .</span><span class="sxs-lookup"><span data-stu-id="d3dc9-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Sottoscrizione sospesa":::

### <a name="considerations"></a><span data-ttu-id="d3dc9-309">Considerazioni</span><span class="sxs-lookup"><span data-stu-id="d3dc9-309">Considerations</span></span>

- <span data-ttu-id="d3dc9-310">**L'ID sottoscrizione sarà diverso dopo il trasferimento.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="d3dc9-311">Se si tratta di una sottoscrizione di Azure (MS-AZR-0145P), inoltre, avrà un ID sottoscrizione di Azure, che viene mantenuto dal proprietario precedente, e verrà visualizzato nel portale di gestione di Azure.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="d3dc9-312">**Non è possibile fare riferimento alla stessa sottoscrizione da più richieste di trasferimento.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="d3dc9-313">Dopo aver creato una richiesta di trasferimento, che include una sottoscrizione esistente, non è possibile creare richieste di trasferimento aggiuntive, inclusa la stessa sottoscrizione, fino a quando non viene annullata la prima richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="d3dc9-314">**I componenti aggiuntivi per le sottoscrizioni basate su licenze devono essere trasferiti insieme alla sottoscrizione di base.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="d3dc9-315">Quando si crea una richiesta di trasferimento, se si seleziona una sottoscrizione esistente con uno o più componenti aggiuntivi, i componenti aggiuntivi verranno inclusi automaticamente nella richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="d3dc9-316">**Le modifiche al conteggio delle licenze in una sottoscrizione non verranno riflesse nella richiesta di trasferimento esistente.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="d3dc9-317">Dopo aver creato una richiesta di trasferimento che include una sottoscrizione esistente, è consigliabile evitare di aggiornare la quantità di licenze della sottoscrizione (o i relativi addons).</span><span class="sxs-lookup"><span data-stu-id="d3dc9-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="d3dc9-318">In tal caso, la nuova quantità non verrà riflessa nella richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="d3dc9-319">Quando il provider indiretto accetta la richiesta di trasferimento, la sottoscrizione risultante avrà la quantità precedente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="d3dc9-320">Se si desidera trasferire la nuova quantità al provider indiretto, è necessario annullare la richiesta di trasferimento esistente e ricrearne una nuova.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="d3dc9-321">**Non tutti gli acquisti possono essere trasferiti tramite il trasferimento di sottoscrizioni autogestite.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="d3dc9-322">Attualmente è possibile trasferire solo le sottoscrizioni O365 e le sottoscrizioni di Azure PAYG (MS-AZR-0145P) usando questa funzionalità.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="d3dc9-323">Non sono supportati altri acquisti, inclusi i piani di Azure, le istanze riservate di Azure, le sottoscrizioni basate su termini e le sottoscrizioni SaaS per Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="d3dc9-324">Verrà visualizzato un motivo per cui non è possibile trasferire una sottoscrizione nella pagina Invia richiesta di trasferimento.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="d3dc9-325">Per trasferire queste sottoscrizioni, sarà necessario [annullare la sottoscrizione esistente](create-a-new-subscription.md#suspend-or-cancel-a-subscription) e acquistare la nuova offerta per il cliente tramite il provider indiretto.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="d3dc9-326">**Non è possibile eseguire il test con l'ambiente sandbox.**</span><span class="sxs-lookup"><span data-stu-id="d3dc9-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="d3dc9-327">Registrazione per incentivi rivenditori indiretti</span><span class="sxs-lookup"><span data-stu-id="d3dc9-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="d3dc9-328">Dopo aver completato la registrazione come rivenditore indiretto sul tenant del partner Direct Bill esistente, si riceverà un invito a iscriversi per incentivare il rivenditore indiretto entro 30 giorni.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="d3dc9-329">L'invito è basato sull'account MPN partner attualmente associato al tenant del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="d3dc9-330">L'invito verrà inviato all'indirizzo di posta elettronica associato all'account MPN partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="d3dc9-331">È anche possibile iscriversi ai programmi Direct Bill Incentive con lo stesso tenant partner.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="d3dc9-332">È necessario gestire i programmi separatamente.</span><span class="sxs-lookup"><span data-stu-id="d3dc9-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d3dc9-333">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d3dc9-333">Next steps</span></span>

- [<span data-ttu-id="d3dc9-334">Altre informazioni su come diventare rivenditore indiretto</span><span class="sxs-lookup"><span data-stu-id="d3dc9-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="d3dc9-335">Nuovi requisiti dei partner diretti in CSP</span><span class="sxs-lookup"><span data-stu-id="d3dc9-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="d3dc9-336">Funzionalità di fatturazione diretta con restrizioni</span><span class="sxs-lookup"><span data-stu-id="d3dc9-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)