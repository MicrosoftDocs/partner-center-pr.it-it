---
title: Creare un'associazione cliente tramite il modello CPOR
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Creare le associazioni dei clienti tramite il modello CPOR (Claiming partner of record). Consente di gestire le vendite, l'utilizzo & gli incentivi per i clienti Microsoft 365 e Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
keywords: attestazioni per incentivi, attestazioni co-op, fondi co-op, OSU, OSA, ISV, associazione di ricavi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ded3850ea03626cd25571746cc9aa32231bd14bc
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265062"
---
# <a name="create-a-customer-association-via-the-cpor-model--use-for-microsoft-365-and-dynamics-365-customers"></a><span data-ttu-id="769ce-105">Creare un'associazione cliente tramite il modello CPOR: usare per i clienti Microsoft 365 e Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="769ce-105">Create a customer association via the CPOR model – use for Microsoft 365 and Dynamics 365 customers</span></span>

<span data-ttu-id="769ce-106">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="769ce-106">**Applies to**</span></span>

- <span data-ttu-id="769ce-107">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="769ce-107">Partner Center</span></span>

<span data-ttu-id="769ce-108">Il 1 ° ottobre 2019, Microsoft ha iniziato a usare il modello CPOR (Claiming partner of record) per gestire le associazioni con i clienti Microsoft 365 e Dynamics 365 per quanto concerne i clienti di Internet Services Advisory (OSA) sell, Online Services Usage (OSU)-Microsoft 365 e OSU-Business Application incentives.</span><span class="sxs-lookup"><span data-stu-id="769ce-108">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

<span data-ttu-id="769ce-109">Quando si invia l'attestazione, Microsoft la convalida.</span><span class="sxs-lookup"><span data-stu-id="769ce-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="769ce-110">A questo punto, è possibile che vengano richieste altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="769ce-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="769ce-111">Verrà inoltre inviata una notifica al cliente della richiesta di associazione.</span><span class="sxs-lookup"><span data-stu-id="769ce-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="769ce-112">I clienti hanno cinque giorni lavorativi per rifiutare esplicitamente. Se non si rifiutano esplicitamente, l'associazione a questo tenant e carico di lavoro specifici sarà ufficiale.</span><span class="sxs-lookup"><span data-stu-id="769ce-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="769ce-113">A questo punto sarà possibile accedere ai dati di utilizzo del cliente.</span><span class="sxs-lookup"><span data-stu-id="769ce-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="769ce-114">Per completare un'attestazione, sono necessarie le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="769ce-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="769ce-115">**ID MPN** per l'entità che rilascia l'attestazione</span><span class="sxs-lookup"><span data-stu-id="769ce-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="769ce-116">Il **nome di dominio** del cliente [trova questo](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span><span class="sxs-lookup"><span data-stu-id="769ce-116">Customer's **domain name** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="769ce-117">**ID directory** o **ID tenant** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name) del cliente</span><span class="sxs-lookup"><span data-stu-id="769ce-117">Customer's **Directory ID** or **Tenant ID** [Find this](https://docs.microsoft.com/partner-center/find-customer-domain-name)</span></span>

- <span data-ttu-id="769ce-118">**Area della soluzione**, ad esempio Business Applications o Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="769ce-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="769ce-119">L' **attività** eseguita e il tipo di attestazione che si desidera effettuare, ad esempio pre-vendite, utilizzo o associazione dei ricavi</span><span class="sxs-lookup"><span data-stu-id="769ce-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="769ce-120">Il nome del **contatto**, il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="769ce-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="769ce-121">Per Dynamics 365, è anche necessario fornire il nome del **contatto tecnico** , il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="769ce-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="769ce-122">**Nome del contatto** e indirizzo di posta elettronica dell'azienda</span><span class="sxs-lookup"><span data-stu-id="769ce-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="769ce-123">Verrà creato un **nome** per questa attestazione</span><span class="sxs-lookup"><span data-stu-id="769ce-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="769ce-124">Il **prodotto** o i carichi di lavoro che si sta reclamando</span><span class="sxs-lookup"><span data-stu-id="769ce-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="769ce-125">**Proof of Execution (PoE)**, ad esempio un rendiconto di lavoro firmato dal cliente.</span><span class="sxs-lookup"><span data-stu-id="769ce-125">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="769ce-126">È anche possibile scaricare un modello POE da usare.</span><span class="sxs-lookup"><span data-stu-id="769ce-126">You can also download a POE template to use.</span></span>

- <span data-ttu-id="769ce-127">Per i partner che rivendicano solo l'associazione dei ricavi: **nome del venditore della soluzione Dynamics**, **nome del cliente**e **nome della soluzione o del prodotto ISV**.</span><span class="sxs-lookup"><span data-stu-id="769ce-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="769ce-128">È inoltre necessario comprendere i punti seguenti:</span><span class="sxs-lookup"><span data-stu-id="769ce-128">You should also understand the following points:</span></span>

- <span data-ttu-id="769ce-129">Se si dispone di Microsoft 365 clienti esistenti, sarà necessario riassociarli a quelli per i quali si desidera continuare a ottenere incentivi OSU utilizzando questo processo.</span><span class="sxs-lookup"><span data-stu-id="769ce-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="769ce-130">Se si dispone di associazioni esistenti con i clienti di Dynamics 365 o Power BI, queste associazioni rimarranno valide fino alla scadenza delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="769ce-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="769ce-131">Un cliente può avere più partner, ma ogni carico di lavoro (per OSU-Microsoft 365) o per la sottoscrizione (per OSA-sell e OSU-Business Applications) può essere associato solo a un partner.</span><span class="sxs-lookup"><span data-stu-id="769ce-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="769ce-132">Creare un'associazione cliente</span><span class="sxs-lookup"><span data-stu-id="769ce-132">Create a customer association</span></span>

1. <span data-ttu-id="769ce-133">Nel dashboard del centro per i partner, in **incentivi**selezionare **Panoramica**, quindi selezionare **associazioni clienti**.</span><span class="sxs-lookup"><span data-stu-id="769ce-133">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2. <span data-ttu-id="769ce-134">Nella parte superiore della pagina associazioni clienti selezionare **+ associazione clienti**.</span><span class="sxs-lookup"><span data-stu-id="769ce-134">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3. <span data-ttu-id="769ce-135">Selezionare l' **ID MPN** della località partner da associare al cliente, quindi aggiungere il nome di dominio e l'ID directory del cliente.</span><span class="sxs-lookup"><span data-stu-id="769ce-135">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="769ce-136">Dove si trovano?</span><span class="sxs-lookup"><span data-stu-id="769ce-136">Where are these?</span></span>](https://docs.microsoft.com/partner-center/find-customer-domain-name)

4. <span data-ttu-id="769ce-137">Selezionare **Continua**.</span><span class="sxs-lookup"><span data-stu-id="769ce-137">Select **Continue**.</span></span>

5. <span data-ttu-id="769ce-138">Selezionare l' **area** e l' **attività**della soluzione.</span><span class="sxs-lookup"><span data-stu-id="769ce-138">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="769ce-139">Se si seleziona Business Applications, selezionare **utilizzo e/o pre-vendite**o **associazione ricavi**, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="769ce-139">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

   ><span data-ttu-id="769ce-140">Se si seleziona l'associazione di ricavi, verranno richieste informazioni leggermente diverse da quelle elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="769ce-140">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

6. <span data-ttu-id="769ce-141">Immettere le informazioni appropriate nella pagina **associa cliente** , quindi selezionare **Crea attestazione**.</span><span class="sxs-lookup"><span data-stu-id="769ce-141">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

7. <span data-ttu-id="769ce-142">Selezionare il prodotto o i prodotti associati a questa associazione cliente, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="769ce-142">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

8. <span data-ttu-id="769ce-143">Completare le informazioni di contatto del cliente e le informazioni di contatto della società.</span><span class="sxs-lookup"><span data-stu-id="769ce-143">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="769ce-144">Tutti i campi sono obbligatori.</span><span class="sxs-lookup"><span data-stu-id="769ce-144">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="769ce-145">Se il prodotto è Dynamics 365 e il prodotto scelto ha più sottoscrizioni per questo particolare cliente, sarà necessario immettere anche l'ID sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="769ce-145">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

9. <span data-ttu-id="769ce-146">Fornire la prova di esecuzione (POE).</span><span class="sxs-lookup"><span data-stu-id="769ce-146">Supply your proof of execution (POE).</span></span> <span data-ttu-id="769ce-147">È possibile trascinarlo nella casella, passare alla documentazione di supporto o usare un modello selezionando **Scarica modello**.</span><span class="sxs-lookup"><span data-stu-id="769ce-147">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

10. <span data-ttu-id="769ce-148">Aggiungere e salvare i commenti se lo si desidera, quindi selezionare **Invia attestazione**.</span><span class="sxs-lookup"><span data-stu-id="769ce-148">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="769ce-149">Invieremo un messaggio di posta elettronica al cliente per richiedere l'approvazione dell'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="769ce-149">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="769ce-150">Una volta inviata l'associazione del cliente, non è possibile modificarla.</span><span class="sxs-lookup"><span data-stu-id="769ce-150">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="769ce-151">Lo stato dell'associazione del cliente viene visualizzato nel campo **stato** .</span><span class="sxs-lookup"><span data-stu-id="769ce-151">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="769ce-152">Selezionare **cronologia** per visualizzare la cronologia di un'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="769ce-152">Select **History** to view the history of a customer association.</span></span>
