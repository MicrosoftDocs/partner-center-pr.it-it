---
title: Offerte private in Azure Marketplace
description: Informazioni sulle offerte private in Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007264"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="42f76-103">Offerte private in Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="42f76-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="42f76-104">Le offerte private rappresentano il modo in cui i Publisher forniscono piani personalizzati a specifici clienti.</span><span class="sxs-lookup"><span data-stu-id="42f76-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="42f76-105">Questa opzione è attualmente supportata solo nell'esperienza di Azure Marketplace nell'portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="42f76-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="42f76-106">Le offerte private sono disponibili solo per le offerte a pagamento che possono essere acquistate e installate direttamente dalla portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="42f76-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="42f76-107">Publisher non può creare offerte private per i servizi di consulenza, qualsiasi servizio che ha **contattato** come chiamata a azione o qualsiasi servizio gratuito, indipendentemente dal fatto che sia possibile installarlo o meno dal portale.</span><span class="sxs-lookup"><span data-stu-id="42f76-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="42f76-108">Trova le offerte private nella portale di Azure</span><span class="sxs-lookup"><span data-stu-id="42f76-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="42f76-109">Quando un partner pubblica un'offerta privata, è visibile solo agli utenti idonei nella sezione **Marketplace** del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="42f76-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="42f76-110">Questi utenti sono definiti tramite ID sottoscrizione o ID tenant, a seconda del tipo di offerta.</span><span class="sxs-lookup"><span data-stu-id="42f76-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="42f76-111">Se si è idonei per offerte private, esistono due modi per individuarli nel portale.</span><span class="sxs-lookup"><span data-stu-id="42f76-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="42f76-112">Le offerte private non sono attualmente disponibili per la ricerca o filtrabili (per categoria) nell'portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="42f76-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="42f76-113">Nella portale di Azure selezionare **+ Crea una risorsa** o cercare "Marketplace" per passare alla pagina del **Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="42f76-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="42f76-114">Se si è idonei per offerte private, si noterà che l'utente dispone di un banner **disponibile** nella parte superiore della pagina.</span><span class="sxs-lookup"><span data-stu-id="42f76-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="42f76-115">Selezionare **Visualizza offerte private** per accedere alla pagina delle offerte private.</span><span class="sxs-lookup"><span data-stu-id="42f76-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banner visualizzato quando sono disponibili offerte private.":::

<span data-ttu-id="42f76-117">In alternativa, se viene visualizzato il banner delle offerte private, è anche possibile scorrere fino alla fine della pagina della raccolta di prodotti e viene visualizzato un subset delle offerte private.</span><span class="sxs-lookup"><span data-stu-id="42f76-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="42f76-118">Selezionare il collegamento per **visualizzare altre informazioni** per passare alla pagina delle offerte private.</span><span class="sxs-lookup"><span data-stu-id="42f76-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Mostra le offerte private nella parte inferiore della schermata, insieme al collegamento Vedi altro.":::

## <a name="review-private-plans"></a><span data-ttu-id="42f76-120">Esaminare i piani privati</span><span class="sxs-lookup"><span data-stu-id="42f76-120">Review private plans</span></span>

<span data-ttu-id="42f76-121">Un'offerta privata è in realtà un piano privato all'interno di un'offerta.</span><span class="sxs-lookup"><span data-stu-id="42f76-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="42f76-122">Ogni offerta può avere più piani, sia pubblici che privati, ma i piani privati vengono visualizzati in un elenco separato dei piani pubblici.</span><span class="sxs-lookup"><span data-stu-id="42f76-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="42f76-123">È possibile visualizzare i piani privati disponibili nella scheda **piani** , contrassegnati con una notifica **privata** distintiva:</span><span class="sxs-lookup"><span data-stu-id="42f76-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Pagina di piani contrassegnata come privata.":::

<span data-ttu-id="42f76-125">Se si dispone di più di una sottoscrizione, vengono visualizzate tutte le offerte private disponibili per tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="42f76-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="42f76-126">Quando si seleziona **Crea**, si viene indirizzati alla pagina di creazione della risorsa per iniziare a configurare la risorsa.</span><span class="sxs-lookup"><span data-stu-id="42f76-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="42f76-127">Se si seleziona **Crea** e si hanno più sottoscrizioni, ma non tutte vengono aggiunte al piano privato, la sottoscrizione predefinita potrebbe non essere la sottoscrizione idonea per questa offerta privata.</span><span class="sxs-lookup"><span data-stu-id="42f76-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="42f76-128">In questo caso, selezionare la sottoscrizione corretta.</span><span class="sxs-lookup"><span data-stu-id="42f76-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Il collegamento che mostra la disponibilità di offerte private è maggiore.":::

## <a name="next-steps"></a><span data-ttu-id="42f76-130">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="42f76-130">Next steps</span></span>

- [<span data-ttu-id="42f76-131">Che cos'è Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="42f76-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
