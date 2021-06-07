---
title: Offerte private in Azure Marketplace
description: Informazioni sulle offerte private in Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534185"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="d2a43-103">Piani privati in Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d2a43-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="d2a43-104">I piani privati sono il modo in cui gli editori forniscono piani personalizzati a clienti specifici.</span><span class="sxs-lookup"><span data-stu-id="d2a43-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="d2a43-105">I piani privati sono disponibili solo per le offerte a pagamento che possono essere acquistate e installate direttamente dal portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="d2a43-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="d2a43-106">Gli editori non possono creare piani privati per i servizi di consulenza, qualsiasi servizio che abbia contattato **l'utente** come invito all'azione o qualsiasi servizio gratuito, indipendentemente dal fatto che possa essere installato o meno dal portale.</span><span class="sxs-lookup"><span data-stu-id="d2a43-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="d2a43-107">Trovare piani privati nella portale di Azure</span><span class="sxs-lookup"><span data-stu-id="d2a43-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="d2a43-108">Quando un partner pubblica un piano privato, è visibile solo agli utenti idonei nella sezione **Marketplace** del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="d2a43-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="d2a43-109">Questi utenti sono definiti dall'ID sottoscrizione o dall'ID tenant, a seconda del tipo di offerta.</span><span class="sxs-lookup"><span data-stu-id="d2a43-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="d2a43-110">Se si è idonei per i piani privati, è possibile trovarli nel portale in due modi.</span><span class="sxs-lookup"><span data-stu-id="d2a43-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="d2a43-111">I piani privati sono ricercabili ma non filtrabili (per categoria) nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="d2a43-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="d2a43-112">Nel portale di Azure selezionare + **Crea una** risorsa o cercare "marketplace" per passare alla pagina **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="d2a43-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="d2a43-113">Se si è idonei per i piani privati, nella parte superiore della pagina verrà visualizzato il **banner** Sono disponibili piani privati.</span><span class="sxs-lookup"><span data-stu-id="d2a43-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="d2a43-114">Selezionare **Visualizza offerte private e piani** per passare alla pagina dei piani privati.</span><span class="sxs-lookup"><span data-stu-id="d2a43-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Il banner visualizzato quando sono disponibili piani privati.":::

## <a name="review-private-plans"></a><span data-ttu-id="d2a43-116">Esaminare i piani privati</span><span class="sxs-lookup"><span data-stu-id="d2a43-116">Review private plans</span></span>

<span data-ttu-id="d2a43-117">Un piano privato fa parte di diversi piani di un'offerta.</span><span class="sxs-lookup"><span data-stu-id="d2a43-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="d2a43-118">Ogni offerta può avere più piani, pubblici e privati, ma i piani privati vengono visualizzati in un elenco separato dai piani pubblici.</span><span class="sxs-lookup"><span data-stu-id="d2a43-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="d2a43-119">È possibile visualizzare i piani privati disponibili nella **scheda Piani,** contrassegnati con un badge **privato** distintivo:</span><span class="sxs-lookup"><span data-stu-id="d2a43-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Pagina di piani contrassegnata come Privata.":::

<span data-ttu-id="d2a43-121">Se si hanno più sottoscrizioni, verranno visualizzati tutti i piani privati disponibili per tutte le sottoscrizioni.</span><span class="sxs-lookup"><span data-stu-id="d2a43-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="d2a43-122">Quando si seleziona **Crea**, si viene indirizzati alla pagina di creazione della risorsa per avviare la configurazione della risorsa.</span><span class="sxs-lookup"><span data-stu-id="d2a43-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="d2a43-123">Se si seleziona **Crea** e si hanno più sottoscrizioni, ma non tutte vengono aggiunte al piano privato, la sottoscrizione predefinita potrebbe non essere idonea per questo piano privato.</span><span class="sxs-lookup"><span data-stu-id="d2a43-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="d2a43-124">In questo caso, selezionare la sottoscrizione corretta.</span><span class="sxs-lookup"><span data-stu-id="d2a43-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Collegamento che mostra che sono disponibili più piani privati.":::

## <a name="next-steps"></a><span data-ttu-id="d2a43-126">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d2a43-126">Next steps</span></span>

- [<span data-ttu-id="d2a43-127">Che cos'è Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="d2a43-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
