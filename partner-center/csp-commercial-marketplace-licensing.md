---
title: Gestire le licenze nelle offerte del marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come configurare e gestire le licenze per le offerte del marketplace commerciale ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284873"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="550ca-103">Gestire le licenze nelle offerte del marketplace</span><span class="sxs-lookup"><span data-stu-id="550ca-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="550ca-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="550ca-104">**Appropriate roles**</span></span>

- <span data-ttu-id="550ca-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="550ca-105">Global admin</span></span>
- <span data-ttu-id="550ca-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="550ca-106">Account admin</span></span>

<span data-ttu-id="550ca-107">Questo articolo illustra come configurare un'offerta in Partner Center, renderla disponibile in Microsoft AppSource e quindi gestire le licenze per tale offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="550ca-108">Le funzionalità di questo articolo sono attualmente disponibili in anteprima pubblica.</span><span class="sxs-lookup"><span data-stu-id="550ca-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="550ca-109">Prima di iniziare</span><span class="sxs-lookup"><span data-stu-id="550ca-109">Before you begin</span></span>

<span data-ttu-id="550ca-110">Prima di iniziare questo processo, è consigliabile acquisire familiarità con le informazioni seguenti.</span><span class="sxs-lookup"><span data-stu-id="550ca-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="550ca-111">Esaminare la documentazione Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="550ca-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="550ca-112">Gli articoli seguenti contengono informazioni che è necessario conoscere prima di continuare.</span><span class="sxs-lookup"><span data-stu-id="550ca-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="550ca-113">Creare un'offerta Dynamics 365 for Customer Engagement & PowerApps</span><span class="sxs-lookup"><span data-stu-id="550ca-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="550ca-114">Creare un account del marketplace commerciale in Partner Center</span><span class="sxs-lookup"><span data-stu-id="550ca-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="550ca-115">Creare l'ID offerta</span><span class="sxs-lookup"><span data-stu-id="550ca-115">Create your Offer ID</span></span>

<span data-ttu-id="550ca-116">Nelle procedure seguenti verrà richiesto di immettere un ID offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="550ca-117">A questo punto, è opportuno creare un ID offerta appropriato, tenendo presente quanto segue:</span><span class="sxs-lookup"><span data-stu-id="550ca-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="550ca-118">Questo ID è visibile ai clienti nell'indirizzo Web per l'offerta del marketplace e nei modelli di Azure Resource Manager, se applicabile.</span><span class="sxs-lookup"><span data-stu-id="550ca-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="550ca-119">L'ID offerta combinato con l'ID editore deve avere una lunghezza inferiore a 40 caratteri.</span><span class="sxs-lookup"><span data-stu-id="550ca-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="550ca-120">Usare solo lettere minuscole e numeri.</span><span class="sxs-lookup"><span data-stu-id="550ca-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="550ca-121">L'ID offerta può includere trattini e caratteri di sottolineatura, ma non spazi.</span><span class="sxs-lookup"><span data-stu-id="550ca-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="550ca-122">Ad esempio, se l'ID editore è testpublisherid e si immette test-offer-1, l'indirizzo Web dell'offerta sarà https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="550ca-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="550ca-123">Questo ID non può essere modificato dopo aver selezionato **Crea.**</span><span class="sxs-lookup"><span data-stu-id="550ca-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="550ca-124">Creare l'alias dell'offerta</span><span class="sxs-lookup"><span data-stu-id="550ca-124">Create your Offer alias</span></span>

<span data-ttu-id="550ca-125">L'alias dell'offerta è il nome usato per l'offerta in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="550ca-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="550ca-126">È anche necessario un alias dell'offerta appropriato che segua le linee guida seguenti:</span><span class="sxs-lookup"><span data-stu-id="550ca-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="550ca-127">Questo nome non viene usato nel marketplace ed è diverso dal nome dell'offerta e da altri valori visualizzati ai clienti.</span><span class="sxs-lookup"><span data-stu-id="550ca-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="550ca-128">Questo nome non può essere modificato dopo aver selezionato Crea.</span><span class="sxs-lookup"><span data-stu-id="550ca-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="550ca-129">Creare l'offerta</span><span class="sxs-lookup"><span data-stu-id="550ca-129">Create your offer</span></span>

<span data-ttu-id="550ca-130">Il primo passaggio del processo di gestione delle licenze consiste nel creare l'offerta del marketplace commerciale.</span><span class="sxs-lookup"><span data-stu-id="550ca-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="550ca-131">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="550ca-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="550ca-132">Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**</span><span class="sxs-lookup"><span data-stu-id="550ca-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="550ca-133">Nella parte superiore della pagina Panoramica selezionare Nuova offerta **e** quindi **Dynamics 365 for Customer Engagement & PowerApps.**</span><span class="sxs-lookup"><span data-stu-id="550ca-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="550ca-134">Immettere **l'ID offerta** e **l'alias** dell'offerta creati in precedenza.</span><span class="sxs-lookup"><span data-stu-id="550ca-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="550ca-135">Selezionare **Crea** per generare l'offerta e continuare.</span><span class="sxs-lookup"><span data-stu-id="550ca-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="550ca-136">Scegliere le opzioni di licenza.</span><span class="sxs-lookup"><span data-stu-id="550ca-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="550ca-137">Per abilitare la gestione delle licenze per l'offerta, selezionare Abilita gestione licenze **app tramite Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="550ca-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="550ca-138">Si tratta di un'impostazione una sola volta e non è possibile modificarla dopo la pubblicazione dell'offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="550ca-139">È anche possibile abilitare i clienti per eseguire le funzionalità di base dell'app senza una licenza ed eseguire le funzionalità Premium dopo aver acquistato una licenza.</span><span class="sxs-lookup"><span data-stu-id="550ca-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="550ca-140">A tale scopo, selezionare **Consenti ai clienti di installare l'app anche se le licenze non sono assegnate.**</span><span class="sxs-lookup"><span data-stu-id="550ca-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="550ca-141">Se non si vuole che la gestione delle licenze dell'offerta sia abilitata, selezionare Scarica adesso **(gratuito),** Versione di valutazione gratuita o **Contattami.**</span><span class="sxs-lookup"><span data-stu-id="550ca-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="550ca-142">Creare il piano</span><span class="sxs-lookup"><span data-stu-id="550ca-142">Create your plan</span></span>

<span data-ttu-id="550ca-143">In questi passaggi si definiranno il piano o i piani da abilitare per l'offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="550ca-144">Nel menu di spostamento a sinistra selezionare **Panoramica del piano** e quindi Selezionare Crea nuovo **piano.**</span><span class="sxs-lookup"><span data-stu-id="550ca-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="550ca-145">Immettere un **ID piano** e un **nome di** piano e quindi selezionare **Crea**.</span><span class="sxs-lookup"><span data-stu-id="550ca-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="550ca-146">Nella pagina **Elenco piani** immettere la descrizione **del piano.**</span><span class="sxs-lookup"><span data-stu-id="550ca-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="550ca-147">Per salvare la descrizione e completare in un secondo momento, **selezionare Salva bozza.**</span><span class="sxs-lookup"><span data-stu-id="550ca-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="550ca-148">Al termine, selezionare Rivedi **e pubblica**.</span><span class="sxs-lookup"><span data-stu-id="550ca-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="550ca-149">Le informazioni sul piano verranno ora visualizzate nel appsource.microsoft.com nell'inserzione dell'offerta (sezione piani).</span><span class="sxs-lookup"><span data-stu-id="550ca-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="550ca-150">Dopo aver creato tutti i piani per questa offerta, è necessario copiare l'ID servizio di ogni piano.</span><span class="sxs-lookup"><span data-stu-id="550ca-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="550ca-151">Selezionare **Panoramica del** piano nella parte superiore della pagina Elenco piani.</span><span class="sxs-lookup"><span data-stu-id="550ca-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="550ca-152">Copiare l'ID servizio per ogni piano in una posizione sicura.</span><span class="sxs-lookup"><span data-stu-id="550ca-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="550ca-153">Aggiungere GLI ID servizio alla soluzione</span><span class="sxs-lookup"><span data-stu-id="550ca-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="550ca-154">Il passaggio successivo consiste nell'aggiornare la soluzione aggiungendo gli ID servizio per ogni piano appena copiato.</span><span class="sxs-lookup"><span data-stu-id="550ca-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="550ca-155">Per indicazioni, vedere [Creare un pacchetto AppSource per la soluzione.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="550ca-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="550ca-156">Caricare il pacchetto e pubblicare l'offerta</span><span class="sxs-lookup"><span data-stu-id="550ca-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="550ca-157">Nel riquadro di spostamento a sinistra selezionare **Marketplace commerciale** e quindi Selezionare **Configurazione tecnica.**</span><span class="sxs-lookup"><span data-stu-id="550ca-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="550ca-158">In **Base License Model (Modello di licenza** di base) selezionare User **(Utente).**</span><span class="sxs-lookup"><span data-stu-id="550ca-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="550ca-159">In **Crm Package (Pacchetto CRM)** immettere l'URL del percorso del pacchetto.</span><span class="sxs-lookup"><span data-stu-id="550ca-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="550ca-160">Usare le altre schede nel riquadro di spostamento a sinistra per immettere eventuali altre informazioni necessarie.</span><span class="sxs-lookup"><span data-stu-id="550ca-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="550ca-161">Al termine, selezionare Rivedi **e pubblica.**</span><span class="sxs-lookup"><span data-stu-id="550ca-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="550ca-162">Dopo aver pubblicato l'offerta, verranno esaminate e verificate le informazioni.</span><span class="sxs-lookup"><span data-stu-id="550ca-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="550ca-163">In caso di problemi con questo processo, l'utente verrà avvisato.</span><span class="sxs-lookup"><span data-stu-id="550ca-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="550ca-164">Dopo aver risolto tutti i problemi, si otterrà una notifica che indica che l'offerta è disponibile in AppSource.</span><span class="sxs-lookup"><span data-stu-id="550ca-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="550ca-165">A questo punto è possibile renderlo live.</span><span class="sxs-lookup"><span data-stu-id="550ca-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="550ca-166">Rendere l'offerta live in Partner Center</span><span class="sxs-lookup"><span data-stu-id="550ca-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="550ca-167">La procedura seguente illustra il processo per rendere l'offerta live in AppSource.</span><span class="sxs-lookup"><span data-stu-id="550ca-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="550ca-168">Per altre informazioni su questo processo, vedere [Introduzione alle opzioni di elenco.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="550ca-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="550ca-169">Dopo aver pubblicato l'offerta, la pubblicazione dell'offerta sarà di 4-6 ore.</span><span class="sxs-lookup"><span data-stu-id="550ca-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="550ca-170">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="550ca-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="550ca-171">Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**</span><span class="sxs-lookup"><span data-stu-id="550ca-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="550ca-172">Nella **pagina Panoramica** trovare l'offerta che si sta cercando.</span><span class="sxs-lookup"><span data-stu-id="550ca-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="550ca-173">Lo stato delle offerte pronte per la pubblicazione sarà **Anteprima.**</span><span class="sxs-lookup"><span data-stu-id="550ca-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="550ca-174">Selezionare l'offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-174">Select the offer.</span></span>
4. <span data-ttu-id="550ca-175">Nella pagina **Panoramica dell'offerta** selezionare **Vai al live.**</span><span class="sxs-lookup"><span data-stu-id="550ca-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="550ca-176">L'offerta sarà live in 4-6 ore.</span><span class="sxs-lookup"><span data-stu-id="550ca-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="550ca-177">Per visualizzare la presentazione dell'offerta in AppSource, selezionare il **collegamento AppSource** nella parte inferiore della **pagina panoramica dell'offerta.**</span><span class="sxs-lookup"><span data-stu-id="550ca-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="550ca-178">**Per le offerte abilitate** per le licenze: se l'offerta richiede un controllo della licenza, gli utenti potranno immettere un lead solo facendo clic su **Contattami,** in modo da poter comunicare con loro.</span><span class="sxs-lookup"><span data-stu-id="550ca-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="550ca-179">**Per le offerte abilitate** per le licenze con l'opzione di installazione  gratuita: se l'offerta non richiede un controllo della licenza, gli utenti amministratori visualizzano un pulsante Scarica adesso oltre a **Contattami.**</span><span class="sxs-lookup"><span data-stu-id="550ca-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="550ca-180">Gli utenti che vogliono provare l'opzione di installazione gratuita dovrebbero fare clic su Scarica **adesso,** che li porterà a installare l'offerta Power Platform Admin Center.</span><span class="sxs-lookup"><span data-stu-id="550ca-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="550ca-181">Gli utenti possono comunque usare **Contattami** se hanno domande o se vogliono eseguire l'aggiornamento a un piano a pagamento.</span><span class="sxs-lookup"><span data-stu-id="550ca-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="550ca-182">Registrare l'offerta ISV Connect in DealReg</span><span class="sxs-lookup"><span data-stu-id="550ca-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="550ca-183">Il passaggio successivo consiste nel registrare l'accordo.</span><span class="sxs-lookup"><span data-stu-id="550ca-183">The next step is to register your deal.</span></span> <span data-ttu-id="550ca-184">A tale scopo, vedere [Registrare le offerte.](https://docs.microsoft.com/partner-center/register-deals)</span><span class="sxs-lookup"><span data-stu-id="550ca-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="550ca-185">Invitare il cliente</span><span class="sxs-lookup"><span data-stu-id="550ca-185">Invite the customer</span></span>

<span data-ttu-id="550ca-186">Usare la procedura seguente per invitare il cliente a partecipare all'offerta.</span><span class="sxs-lookup"><span data-stu-id="550ca-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="550ca-187">Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="550ca-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="550ca-188">Nel menu di spostamento a sinistra selezionare **Marketplace commerciale/Panoramica.**</span><span class="sxs-lookup"><span data-stu-id="550ca-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="550ca-189">Filtrare **le offerte** inviate, selezionare la scheda **In** corso e quindi selezionare l'offerta desiderata.</span><span class="sxs-lookup"><span data-stu-id="550ca-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="550ca-190">Nella pagina di panoramica per questa operazione selezionare **Gestisci licenze**.</span><span class="sxs-lookup"><span data-stu-id="550ca-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="550ca-191">Nella finestra **Gestisci licenze** selezionare il cliente nell'elenco a discesa **Dettagli** cliente.</span><span class="sxs-lookup"><span data-stu-id="550ca-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="550ca-192">Se la relazione con il cliente non esiste ancora, selezionare **+Invita un nuovo cliente a acconsentire.**</span><span class="sxs-lookup"><span data-stu-id="550ca-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="550ca-193">Copiare il collegamento visualizzato.</span><span class="sxs-lookup"><span data-stu-id="550ca-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="550ca-194">Inviare questo collegamento tramite posta elettronica all'amministratore della fatturazione o all'amministratore globale del cliente e fare in modo che usi questo collegamento per accedere admin.microsoft.com e accettare e autorizzare la relazione che si sta stabilendo.</span><span class="sxs-lookup"><span data-stu-id="550ca-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="550ca-195">La relazione non verrà stabilita fino a quando il cliente non esegue questo passaggio.</span><span class="sxs-lookup"><span data-stu-id="550ca-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="550ca-196">Attivare, gestire e rimuovere le licenze</span><span class="sxs-lookup"><span data-stu-id="550ca-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="550ca-197">Dopo aver stabilito il cliente, è possibile iniziare ad aggiungere piani dall'offerta e assegnare licenze a ogni piano.</span><span class="sxs-lookup"><span data-stu-id="550ca-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="550ca-198">Nella finestra Gestisci licenze per questa trattativa selezionare **+Aggiungi un piano.**</span><span class="sxs-lookup"><span data-stu-id="550ca-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="550ca-199">Completare **i campi Piani per questa soluzione** e Numero **di** licenze e quindi selezionare **Aggiorna licenze.**</span><span class="sxs-lookup"><span data-stu-id="550ca-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="550ca-200">Le licenze saranno disponibili a livello admin.microsoft.com che i clienti possono gestire e assegnare ai dipendenti.</span><span class="sxs-lookup"><span data-stu-id="550ca-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="550ca-201">Per modificare il numero di licenze per un piano esistente, immettere il nuovo numero nel campo **Numero** di licenze e quindi selezionare **Aggiorna licenze.**</span><span class="sxs-lookup"><span data-stu-id="550ca-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="550ca-202">Per disattivare o rimuovere le licenze per una trattativa, selezionare l'icona del cestino nel **campo Azioni** e quindi selezionare **Aggiorna licenze.**</span><span class="sxs-lookup"><span data-stu-id="550ca-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>