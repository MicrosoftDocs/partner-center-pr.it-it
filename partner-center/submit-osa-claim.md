---
title: Creare un'associazione cliente
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Creare le associazioni dei clienti con il modello claiming partner of record (CPOR). Consente di gestire le vendite, l'utilizzo e gli incentivi per i clienti Microsoft 365 & Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92174994"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="84bb0-104">Associazioni dei clienti tramite il modello CPOR (partner di record) per Microsoft 365 e Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="84bb0-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="84bb0-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="84bb0-105">**Applies to**</span></span>

- <span data-ttu-id="84bb0-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="84bb0-106">Partner Center</span></span>

<span data-ttu-id="84bb0-107">**Ruoli appropriati:**</span><span class="sxs-lookup"><span data-stu-id="84bb0-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="84bb0-108">Amministratore degli incentivi</span><span class="sxs-lookup"><span data-stu-id="84bb0-108">Incentives admin</span></span>

<span data-ttu-id="84bb0-109">Il 1 ° ottobre 2019, Microsoft ha iniziato a usare il modello CPOR (Claiming partner of record) per gestire le associazioni con i clienti Microsoft 365 e Dynamics 365 per quanto concerne i clienti di Online Services Advisory (OSA) sell, Online Services Usage (OSU)-Microsoft 365 e OSU-Business Application incentives.</span><span class="sxs-lookup"><span data-stu-id="84bb0-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="84bb0-110">Le attestazioni relative all'associazione clienti (CPOR) si applicano solo ai programmi Online Services Advisory (OSA) sell, Online Services Usage (OSU)-Microsoft 365 e OSU-Business Application incentive.</span><span class="sxs-lookup"><span data-stu-id="84bb0-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="84bb0-111">Se si invia un'attestazione co-op per un altro programma, ad esempio Cloud Solution Provider, Managed Reseller, hosting o Surface, fare riferimento al processo di attestazioni co-op descritto qui.</span><span class="sxs-lookup"><span data-stu-id="84bb0-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="84bb0-112">Quando si invia l'attestazione, Microsoft la convalida.</span><span class="sxs-lookup"><span data-stu-id="84bb0-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="84bb0-113">A questo punto, è possibile che vengano richieste altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="84bb0-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="84bb0-114">Verrà inoltre inviata una notifica al cliente della richiesta di associazione.</span><span class="sxs-lookup"><span data-stu-id="84bb0-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="84bb0-115">I clienti hanno cinque giorni lavorativi per rifiutare esplicitamente. Se non si rifiutano esplicitamente, l'associazione a questo tenant e carico di lavoro specifici sarà ufficiale.</span><span class="sxs-lookup"><span data-stu-id="84bb0-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="84bb0-116">A questo punto sarà possibile accedere ai dati di utilizzo del cliente.</span><span class="sxs-lookup"><span data-stu-id="84bb0-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="84bb0-117">Per completare un'attestazione, sono necessarie le informazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="84bb0-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="84bb0-118">**ID MPN** per l'entità che rilascia l'attestazione</span><span class="sxs-lookup"><span data-stu-id="84bb0-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="84bb0-119">Il **nome di dominio** del cliente [trova questo](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="84bb0-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="84bb0-120">**ID directory** o **ID tenant** [Find this](find-domain-name.md) del cliente</span><span class="sxs-lookup"><span data-stu-id="84bb0-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="84bb0-121">**Area della soluzione**, ad esempio Business Applications o Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="84bb0-121">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="84bb0-122">L' **attività** eseguita e il tipo di attestazione che si desidera effettuare, ad esempio pre-vendite, utilizzo o associazione dei ricavi</span><span class="sxs-lookup"><span data-stu-id="84bb0-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="84bb0-123">Il nome del **contatto**, il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="84bb0-123">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="84bb0-124">Per Dynamics 365, è anche necessario fornire il nome del **contatto tecnico** , il titolo e l'indirizzo di posta elettronica del cliente</span><span class="sxs-lookup"><span data-stu-id="84bb0-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="84bb0-125">**Nome del contatto** e indirizzo di posta elettronica dell'azienda</span><span class="sxs-lookup"><span data-stu-id="84bb0-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="84bb0-126">Verrà creato un **nome** per questa attestazione</span><span class="sxs-lookup"><span data-stu-id="84bb0-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="84bb0-127">Il **prodotto** o i carichi di lavoro che si sta reclamando</span><span class="sxs-lookup"><span data-stu-id="84bb0-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="84bb0-128">**Proof of Execution (PoE)**, ad esempio un rendiconto di lavoro firmato dal cliente.</span><span class="sxs-lookup"><span data-stu-id="84bb0-128">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="84bb0-129">È anche possibile scaricare un modello PoE da usare.</span><span class="sxs-lookup"><span data-stu-id="84bb0-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="84bb0-130">Per i partner che rivendicano solo l'associazione dei ricavi: **nome del venditore della soluzione Dynamics**, **nome del cliente**e **nome della soluzione o del prodotto ISV**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-130">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="84bb0-131">È inoltre necessario comprendere i punti seguenti:</span><span class="sxs-lookup"><span data-stu-id="84bb0-131">You should also understand the following points:</span></span>

- <span data-ttu-id="84bb0-132">Se si dispone di Microsoft 365 clienti esistenti, sarà necessario riassociarli a quelli per i quali si desidera continuare a ottenere incentivi OSU utilizzando questo processo.</span><span class="sxs-lookup"><span data-stu-id="84bb0-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="84bb0-133">Se si dispone di associazioni esistenti con i clienti di Dynamics 365 o Power BI, queste associazioni rimarranno valide fino alla scadenza delle sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="84bb0-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="84bb0-134">Un cliente può avere più partner, ma ogni carico di lavoro (per OSU-Microsoft 365) o una sottoscrizione (per le applicazioni OSA-Sell e OSU-Business) può essere associato solo a un partner.</span><span class="sxs-lookup"><span data-stu-id="84bb0-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="84bb0-135">Creare un'associazione cliente</span><span class="sxs-lookup"><span data-stu-id="84bb0-135">Create a customer association</span></span>

1. <span data-ttu-id="84bb0-136">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="84bb0-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="84bb0-137">Selezionare la scheda **incentivi** , fare clic su **Panoramica**e quindi selezionare **associazioni clienti**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-137">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="84bb0-138">Nella parte superiore della pagina associazioni clienti selezionare **+ associazione clienti**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-138">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="84bb0-139">Selezionare l'**ID MPN** della località partner da associare al cliente, quindi aggiungere il nome di dominio e l'ID directory del cliente.</span><span class="sxs-lookup"><span data-stu-id="84bb0-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="84bb0-140">Trova</span><span class="sxs-lookup"><span data-stu-id="84bb0-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="84bb0-141">Selezionare **Continua**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-141">Select **Continue**.</span></span>

6. <span data-ttu-id="84bb0-142">Selezionare l' **area** e l' **attività**della soluzione.</span><span class="sxs-lookup"><span data-stu-id="84bb0-142">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="84bb0-143">Se si seleziona Business Applications, selezionare **utilizzo e/o pre-vendite**o **associazione ricavi**, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-143">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="84bb0-144">Se si seleziona Associazione ricavi, verranno richieste informazioni leggermente diverse da quelle elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="84bb0-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="84bb0-145">Immettere le informazioni appropriate nella pagina **associa cliente** , quindi selezionare **Crea attestazione**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="84bb0-146">Selezionare il prodotto o i prodotti associati a questa associazione cliente, quindi selezionare **continua**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-146">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="84bb0-147">Completare le informazioni di contatto del cliente e le informazioni di contatto della società.</span><span class="sxs-lookup"><span data-stu-id="84bb0-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="84bb0-148">Tutti i campi sono obbligatori.</span><span class="sxs-lookup"><span data-stu-id="84bb0-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="84bb0-149">Se il prodotto è Dynamics 365 e il prodotto scelto ha più sottoscrizioni per questo particolare cliente, sarà necessario immettere anche l'ID sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="84bb0-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="84bb0-150">Fornire la prova di esecuzione (PoE).</span><span class="sxs-lookup"><span data-stu-id="84bb0-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="84bb0-151">È possibile trascinarla nella casella, passare alla propria documentazione di supporto o usare un modello selezionando **Scarica modello**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="84bb0-152">Aggiungere e salvare i commenti se lo si desidera, quindi selezionare **Invia attestazione**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-152">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="84bb0-153">Invieremo un messaggio di posta elettronica al cliente per richiedere l'approvazione dell'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="84bb0-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="84bb0-154">Una volta inviata l'associazione del cliente, non è possibile modificarla.</span><span class="sxs-lookup"><span data-stu-id="84bb0-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="84bb0-155">Lo stato dell'associazione del cliente viene visualizzato nel campo **stato**.</span><span class="sxs-lookup"><span data-stu-id="84bb0-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="84bb0-156">Selezionare **Cronologia** per visualizzare la cronologia di un'associazione del cliente.</span><span class="sxs-lookup"><span data-stu-id="84bb0-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="84bb0-157">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="84bb0-157">Next steps</span></span>

- [<span data-ttu-id="84bb0-158">Gestire le associazioni del cliente</span><span class="sxs-lookup"><span data-stu-id="84bb0-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)