---
title: Aggiungere Servizi condivisi per partner di Azure
description: Usare Servizi condivisi per partner di Azure per acquistare sottoscrizioni di Azure per uso personale e avere un metodo uniforme per l'acquisto, il rilevamento e la gestione di Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: ffec50d53b50bdb6aa2690f1dfcc1bc7312cc3cb
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277301"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="230c6-103">Aggiungere Servizi condivisi per partner di Azure in modo che i partner possano acquistare sottoscrizioni di Azure per uso personale</span><span class="sxs-lookup"><span data-stu-id="230c6-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="230c6-104">**Ruoli appropriati:** Amministratore globale | Agente amministratore | Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="230c6-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="230c6-105">Azure - Servizi condivisi/Carico di lavoro interno è un nuovo tipo di offerta per i partner aderenti al programma CSP che consente di acquistare sottoscrizioni di Azure per uso proprio.</span><span class="sxs-lookup"><span data-stu-id="230c6-105">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="230c6-106">Consente ai partner di usare un metodo uniforme per l'acquisto, il rilevamento e la gestione di Azure, oltre alla possibilità di consolidare i contratti di licenza e rivendita di Azure con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="230c6-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="230c6-107">Con Servizi condivisi per partner di Azure, i partner hanno ora la stessa flessibilità di usare le sottoscrizioni di Azure in CSP come nei programmi Microsoft Contratto Enterprise e Web Direct, aprendo scenari come la creazione di ambienti di sviluppo e test, la distribuzione di carichi di lavoro interni e l'hosting di servizi condivisi o applicazioni multi-tenant.</span><span class="sxs-lookup"><span data-stu-id="230c6-107">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="230c6-108">Creare il tenant dei servizi condivisi</span><span class="sxs-lookup"><span data-stu-id="230c6-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="230c6-109">Passare a **Impostazioni**  >  **Impostazioni Account Servizi**  >  **condivisi**.</span><span class="sxs-lookup"><span data-stu-id="230c6-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Impostazioni dell'account > servizi condivisi":::

2. <span data-ttu-id="230c6-111">Se non si dispone già di un tenant di servizi condivisi, fare clic **su Crea servizi condivisi**.</span><span class="sxs-lookup"><span data-stu-id="230c6-111">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Creare servizi condivisi.":::

3. <span data-ttu-id="230c6-113">Verrà creato un tenant di servizi condivisi e verrà acquistata Azure CSP di servizi condivisi da usare per le risorse condivise e il carico di lavoro interno.</span><span class="sxs-lookup"><span data-stu-id="230c6-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Creare il tenant e acquistare la sottoscrizione.":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="230c6-115">Informazioni sull'Azure - Servizi condivisi/Carico di lavoro interno offerta</span><span class="sxs-lookup"><span data-stu-id="230c6-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="230c6-116">La Azure - Servizi condivisi/Carico di lavoro interno è un nuovo tipo di offerta di Azure in CSP accessibile tramite Partner Center che i partner ottengono per il proprio uso di Azure.</span><span class="sxs-lookup"><span data-stu-id="230c6-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="230c6-117">Servizi condivisi per partner di Azure le sottoscrizioni sono idonee e possono essere usate per acquistare le richieste pull.</span><span class="sxs-lookup"><span data-stu-id="230c6-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="230c6-118">L Azure - Servizi condivisi/Carico di lavoro interno'offerta può essere applicata solo al tenant dei servizi condivisi.</span><span class="sxs-lookup"><span data-stu-id="230c6-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="230c6-119">L'uso principale per la Azure - Servizi condivisi/Carico di lavoro interno è in modo che sia possibile usare Azure per scopi di sviluppo personalizzati.</span><span class="sxs-lookup"><span data-stu-id="230c6-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="230c6-120">Il tenant condiviso usato per effettuare il provisioning di questa offerta non può essere usato per altri servizi, ad esempio licenze di Office 365 o Dynamics.</span><span class="sxs-lookup"><span data-stu-id="230c6-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="230c6-121">È possibile annullare la sottoscrizione come qualsiasi altra sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="230c6-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="230c6-122">Passare alle impostazioni **Visualizza tutto**  >    >  **impostazioni Servizi condivisi**.</span><span class="sxs-lookup"><span data-stu-id="230c6-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="230c6-123">Selezionare la Azure - Servizi condivisi/Carico di lavoro interno e annullarla.</span><span class="sxs-lookup"><span data-stu-id="230c6-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="230c6-124">Accesso ai dettagli Servizi condivisi per partner di Azure consumo</span><span class="sxs-lookup"><span data-stu-id="230c6-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="230c6-125">Il consumo di Azure si trova nella fattura CSP e nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="230c6-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="230c6-126">Verrà incluso come parte della Microsoft Azure riga nella fattura.</span><span class="sxs-lookup"><span data-stu-id="230c6-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="230c6-127">Le informazioni dettagliate sul consumo saranno disponibili nel file di riconciliazione registrato nel tenant creato per questa offerta.</span><span class="sxs-lookup"><span data-stu-id="230c6-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="230c6-128">Servizi condivisi per partner di Azure prezzi</span><span class="sxs-lookup"><span data-stu-id="230c6-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="230c6-129">Per visualizzare il nuovo file di prezzi Servizi condivisi per partner di Azure, passare a **Vendere** prezzi e offerte  >   e selezionare il listino prezzi del mese corrente.</span><span class="sxs-lookup"><span data-stu-id="230c6-129">To see the new pricing file for Azure Partner Shared Services, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="230c6-130">Nelle prossime settimane verrà rilasciata anche un'API scheda tariffa specifica.</span><span class="sxs-lookup"><span data-stu-id="230c6-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="230c6-131">Offerte del Marketplace e Servizi condivisi per partner di Azure</span><span class="sxs-lookup"><span data-stu-id="230c6-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="230c6-132">A partire dal 1° marzo 2019, Servizi condivisi per partner di Azure (APSS) non supporta più le offerte del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="230c6-132">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="230c6-133">**Supporto di Marketplace**</span><span class="sxs-lookup"><span data-stu-id="230c6-133">**Marketplace support**</span></span>   |<span data-ttu-id="230c6-134">**APSS supportato prima del 1° marzo 2019**</span><span class="sxs-lookup"><span data-stu-id="230c6-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="230c6-135">**Dopo il 1° marzo 2019**</span><span class="sxs-lookup"><span data-stu-id="230c6-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="230c6-136">Bring Your Own License (BYOL) e servizi gratuiti</span><span class="sxs-lookup"><span data-stu-id="230c6-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="230c6-137">Sì</span><span class="sxs-lookup"><span data-stu-id="230c6-137">Yes</span></span>   | <span data-ttu-id="230c6-138">No</span><span class="sxs-lookup"><span data-stu-id="230c6-138">No</span></span>|
|<span data-ttu-id="230c6-139">Altre offerte del marketplace di terze parti</span><span class="sxs-lookup"><span data-stu-id="230c6-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="230c6-140">No</span><span class="sxs-lookup"><span data-stu-id="230c6-140">No</span></span>   |<span data-ttu-id="230c6-141">No</span><span class="sxs-lookup"><span data-stu-id="230c6-141">No</span></span>|

<span data-ttu-id="230c6-142">I partner che hanno BYOL o servizi gratuiti distribuiti tramite APSS non saranno influenzati; tuttavia dopo il 1° marzo 2019 non potranno acquistare nuovi servizi BYOL o gratuiti.</span><span class="sxs-lookup"><span data-stu-id="230c6-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="230c6-143">Per sfruttare il catalogo completo delle offerte del Marketplace disponibili (non solo BYOL e servizi gratuiti), è consigliabile che i partner CSP distribuiscono servizi condivisi usando sottoscrizioni web direct di Azure.</span><span class="sxs-lookup"><span data-stu-id="230c6-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="230c6-144">I partner CSP che hanno distribuito in precedenza risorse di servizi GRATUITI e BYOL di terze parti dal Marketplace e che vogliono continuare a usarle e distribuire altre offerte di terze parti sono invitati a eseguire la migrazione della sottoscrizione APSS alla migrazione diretta web delle sottoscrizioni di [Azure esistenti.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="230c6-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="230c6-145">I partner, che in programma di continuare a usare la sottoscrizione APSS dopo il 1° marzo 2019 e vogliono distribuire nuovi servizi [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) di terze parti o servizi gratuiti, possono seguire le istruzioni degli ISV per distribuirlo nelle sottoscrizioni APSS.</span><span class="sxs-lookup"><span data-stu-id="230c6-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="230c6-146">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="230c6-146">Next steps</span></span>

- [<span data-ttu-id="230c6-147">Vendere abbonamenti software tramite CSP</span><span class="sxs-lookup"><span data-stu-id="230c6-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)