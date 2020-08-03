---
title: Creare un'associazione cliente tramite il modello CPOR
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Creare le associazioni dei clienti tramite il modello CPOR (Claiming partner of record). Consente di gestire le vendite, l'utilizzo & gli incentivi per i clienti Microsoft 365 e Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 47f4912e33eb1a2bb3e7c5a1c734d7cc5d3e5f33
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468348"
---
# <a name="create-a-customer-association-via-the-cpor-model--use-for-microsoft-365-and-dynamics-365-customers"></a><span data-ttu-id="a5a17-104">Creare un'associazione cliente tramite il modello CPOR: usare per i clienti Microsoft 365 e Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a5a17-104">Create a customer association via the CPOR model – use for Microsoft 365 and Dynamics 365 customers</span></span>

<span data-ttu-id="a5a17-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="a5a17-105">**Applies to**</span></span>

- <span data-ttu-id="a5a17-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="a5a17-106">Partner Center</span></span>

<span data-ttu-id="a5a17-107">Il 1 ° ottobre 2019, Microsoft ha iniziato a usare il modello CPOR (Claiming partner of record) per gestire le associazioni con i clienti Microsoft 365 e Dynamics 365 per quanto concerne i clienti di Internet Services Advisory (OSA) sell, Online Services Usage (OSU)-Microsoft 365 e OSU-Business Application incentives.</span><span class="sxs-lookup"><span data-stu-id="a5a17-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

<span data-ttu-id="a5a17-108">Quando si invia l'attestazione, Microsoft la convalida.</span><span class="sxs-lookup"><span data-stu-id="a5a17-108">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="a5a17-109">A questo punto, è possibile che vengano richieste altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="a5a17-109">We may ask you for more information at this point.</span></span> <span data-ttu-id="a5a17-110">Verrà inoltre inviata una notifica al cliente della richiesta di associazione.</span><span class="sxs-lookup"><span data-stu-id="a5a17-110">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="a5a17-111">I clienti hanno cinque giorni lavorativi per rifiutare esplicitamente. Se non si rifiutano esplicitamente, l'associazione a questo tenant e carico di lavoro specifici sarà ufficiale.</span><span class="sxs-lookup"><span data-stu-id="a5a17-111">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="a5a17-112">A questo punto sarà possibile accedere ai dati di utilizzo del cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a17-112">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="a5a17-113">Per completare un'attestazione, sono necessarie le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a5a17-113">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="a5a17-114">**ID MPN** per l'entità che rilascia l'attestazione</span><span class="sxs-lookup"><span data-stu-id="a5a17-114">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="a5a17-115">Il **nome di dominio** del cliente [trova questo](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="a5a17-115">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="a5a17-116">**ID directory** o **ID tenant** [Find this](find-domain-name.md) del cliente</span><span class="sxs-lookup"><span data-stu-id="a5a17-116">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="a5a17-117">**Area della soluzione**, ad esempio Business Applications o Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a5a17-117">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="a5a17-118">L' **attività** eseguita e il tipo di attestazione che si desidera effettuare, ad esempio pre-vendite, utilizzo o associazione dei ricavi</span><span class="sxs-lookup"><span data-stu-id="a5a17-118">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="a5a17-119">Il nome del **contatto**, il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="a5a17-119">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="a5a17-120">Per Dynamics 365, è anche necessario fornire il nome del **contatto tecnico** , il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="a5a17-120">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="a5a17-121">**Nome del contatto** e indirizzo di posta elettronica dell'azienda</span><span class="sxs-lookup"><span data-stu-id="a5a17-121">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="a5a17-122">Verrà creato un **nome** per questa attestazione</span><span class="sxs-lookup"><span data-stu-id="a5a17-122">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="a5a17-123">Il **prodotto** o i carichi di lavoro che si sta reclamando</span><span class="sxs-lookup"><span data-stu-id="a5a17-123">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="a5a17-124">**Proof of Execution (PoE)**, ad esempio un rendiconto di lavoro firmato dal cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a17-124">**Proof of execution (POE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="a5a17-125">È anche possibile scaricare un modello POE da usare.</span><span class="sxs-lookup"><span data-stu-id="a5a17-125">You can also download a POE template to use.</span></span>

- <span data-ttu-id="a5a17-126">Per i partner che rivendicano solo l'associazione dei ricavi: **nome del venditore della soluzione Dynamics**, **nome del cliente**e **nome della soluzione o del prodotto ISV**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-126">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="a5a17-127">È inoltre necessario comprendere i punti seguenti:</span><span class="sxs-lookup"><span data-stu-id="a5a17-127">You should also understand the following points:</span></span>

- <span data-ttu-id="a5a17-128">Se si dispone di Microsoft 365 clienti esistenti, sarà necessario riassociarli a quelli per i quali si desidera continuare a ottenere incentivi OSU utilizzando questo processo.</span><span class="sxs-lookup"><span data-stu-id="a5a17-128">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="a5a17-129">Se si dispone di associazioni esistenti con i clienti di Dynamics 365 o Power BI, queste associazioni rimarranno valide fino alla scadenza delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="a5a17-129">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="a5a17-130">Un cliente può avere più partner, ma ogni carico di lavoro (per OSU-Microsoft 365) o per la sottoscrizione (per OSA-sell e OSU-Business Applications) può essere associato solo a un partner.</span><span class="sxs-lookup"><span data-stu-id="a5a17-130">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="a5a17-131">Creare un'associazione cliente</span><span class="sxs-lookup"><span data-stu-id="a5a17-131">Create a customer association</span></span>

1. <span data-ttu-id="a5a17-132">Nel dashboard del centro per i partner, in **incentivi**selezionare **Panoramica**, quindi selezionare **associazioni clienti**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-132">In the Partner Center dashboard, under **Incentives**, select **Overview**, and then select **Customer associations**.</span></span> 

2. <span data-ttu-id="a5a17-133">Nella parte superiore della pagina associazioni clienti selezionare **+ associazione clienti**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-133">At the top of the Customer associations page, select **+ Customer association**.</span></span>

3. <span data-ttu-id="a5a17-134">Selezionare l' **ID MPN** della località partner da associare al cliente, quindi aggiungere il nome di dominio e l'ID directory del cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a17-134">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="a5a17-135">Trova</span><span class="sxs-lookup"><span data-stu-id="a5a17-135">Find this</span></span>](find-domain-name.md)

4. <span data-ttu-id="a5a17-136">Seleziona **Continua**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-136">Select **Continue**.</span></span>

5. <span data-ttu-id="a5a17-137">Selezionare l' **area** e l' **attività**della soluzione.</span><span class="sxs-lookup"><span data-stu-id="a5a17-137">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="a5a17-138">Se si seleziona Business Applications, selezionare **utilizzo e/o pre-vendite**o **associazione ricavi**, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-138">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 

   ><span data-ttu-id="a5a17-139">Se si seleziona l'associazione di ricavi, verranno richieste informazioni leggermente diverse da quelle elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="a5a17-139">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

6. <span data-ttu-id="a5a17-140">Immettere le informazioni appropriate nella pagina **associa cliente** , quindi selezionare **Crea attestazione**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-140">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

7. <span data-ttu-id="a5a17-141">Selezionare il prodotto o i prodotti associati a questa associazione cliente, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-141">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

8. <span data-ttu-id="a5a17-142">Completare le informazioni di contatto del cliente e le informazioni di contatto della società.</span><span class="sxs-lookup"><span data-stu-id="a5a17-142">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="a5a17-143">Tutti i campi sono obbligatori.</span><span class="sxs-lookup"><span data-stu-id="a5a17-143">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="a5a17-144">Se il prodotto è Dynamics 365 e il prodotto scelto ha più sottoscrizioni per questo particolare cliente, sarà necessario immettere anche l'ID sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="a5a17-144">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

9. <span data-ttu-id="a5a17-145">Fornire la prova di esecuzione (POE).</span><span class="sxs-lookup"><span data-stu-id="a5a17-145">Supply your proof of execution (POE).</span></span> <span data-ttu-id="a5a17-146">È possibile trascinarlo nella casella, passare alla documentazione di supporto o usare un modello selezionando **Scarica modello**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-146">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

10. <span data-ttu-id="a5a17-147">Aggiungere e salvare i commenti se lo si desidera, quindi selezionare **Invia attestazione**.</span><span class="sxs-lookup"><span data-stu-id="a5a17-147">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="a5a17-148">Invieremo un messaggio di posta elettronica al cliente per richiedere l'approvazione dell'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a17-148">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="a5a17-149">Una volta inviata l'associazione del cliente, non è possibile modificarla.</span><span class="sxs-lookup"><span data-stu-id="a5a17-149">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="a5a17-150">Lo stato dell'associazione del cliente viene visualizzato nel campo **stato** .</span><span class="sxs-lookup"><span data-stu-id="a5a17-150">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="a5a17-151">Selezionare **cronologia** per visualizzare la cronologia di un'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a17-151">Select **History** to view the history of a customer association.</span></span>
