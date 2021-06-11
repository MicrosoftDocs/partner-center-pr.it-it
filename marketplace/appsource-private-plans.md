---
title: Piani privati in Microsoft AppSource
description: Configurazione di piani privati in Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008553"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="3ca58-103">Piani privati in Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="3ca58-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="3ca58-104">I piani privati sono il modo in cui gli editori forniscono piani personalizzati a clienti specifici.</span><span class="sxs-lookup"><span data-stu-id="3ca58-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="3ca58-105">Questa opzione è ora disponibile in Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="3ca58-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="3ca58-106">I piani privati possono essere venduti in AppSource per le  offerte SaaS (Software as a Service) con l'invito all'azione Scarica adesso.</span><span class="sxs-lookup"><span data-stu-id="3ca58-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="3ca58-107">Richiedere un piano privato all'ISV</span><span class="sxs-lookup"><span data-stu-id="3ca58-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="3ca58-108">Perché un piano privato sia disponibile in AppSource, è necessario contattare direttamente l'ISV e negoziare un prezzo personalizzato e specifiche tecniche.</span><span class="sxs-lookup"><span data-stu-id="3ca58-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="3ca58-109">Una volta accettate le condizioni del piano privato, l'ISV creerà automaticamente un piano e lo assegna all'ID tenant dell'organizzazione, che sarà necessario fornire.</span><span class="sxs-lookup"><span data-stu-id="3ca58-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="3ca58-110">Ricerca dell'ID tenant</span><span class="sxs-lookup"><span data-stu-id="3ca58-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="3ca58-111">In AppSource, nell'angolo in alto a destra, selezionare l'icona del profilo dell'account e quindi **Visualizza tenant.**</span><span class="sxs-lookup"><span data-stu-id="3ca58-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="3ca58-112">Copiare l'ID tenant e specificarlo nell'ISV.</span><span class="sxs-lookup"><span data-stu-id="3ca58-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Illustra come trovare l'ID tenant.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="3ca58-114">Trovare un piano privato in AppSource</span><span class="sxs-lookup"><span data-stu-id="3ca58-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="3ca58-115">La pubblicazione del nuovo piano privato da parte dell'ISV può richiedere fino a 48 ore prima che venga visualizzato in AppSource.</span><span class="sxs-lookup"><span data-stu-id="3ca58-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="3ca58-116">Per trovare i piani privati associati all'ID tenant, selezionare **Piani privati** (icona a forma di lucchetto) in alto a destra in AppSource.</span><span class="sxs-lookup"><span data-stu-id="3ca58-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Mostra l'icona a forma di lucchetto (lucchetto) nella barra degli strumenti superiore.":::

<span data-ttu-id="3ca58-118">Se non è stato eseguito l'accesso, verrà visualizzato un messaggio che richiede di eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="3ca58-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="3ca58-119">È quindi possibile acquistare i piani privati associati all'ID tenant nella **scheda Piani e** prezzi.</span><span class="sxs-lookup"><span data-stu-id="3ca58-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Mostra le offerte private nella scheda piano e prezzi.":::

<span data-ttu-id="3ca58-121">Se i piani privati non sono disponibili per il tenant, verrà visualizzato un messaggio che indica che non sono presenti piani o offerte privati.</span><span class="sxs-lookup"><span data-stu-id="3ca58-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="3ca58-122">Acquistare un piano privato</span><span class="sxs-lookup"><span data-stu-id="3ca58-122">Purchase a private plan</span></span>

<span data-ttu-id="3ca58-123">Un ISV può includere uno o più piani privati all'interno di un'offerta.</span><span class="sxs-lookup"><span data-stu-id="3ca58-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="3ca58-124">Ogni offerta può avere piani sia pubblici che privati, ma i piani privati vengono visualizzati in una pagina separata di presentazione dell'offerta accessibile dall'icona offerte private (lucchetto) in alto a destra nella pagina.</span><span class="sxs-lookup"><span data-stu-id="3ca58-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="3ca58-125">I piani privati disponibili vengono visualizzati **nella scheda Piani e** prezzi. I piani privati hanno un badge blu distintivo.</span><span class="sxs-lookup"><span data-stu-id="3ca58-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Mostra la notifica dell'offerta privata blu accanto alle offerte private.":::

<span data-ttu-id="3ca58-127">Per acquistare un piano selezionato, selezionare **Scarica adesso** e seguire la procedura fornita.</span><span class="sxs-lookup"><span data-stu-id="3ca58-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3ca58-128">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="3ca58-128">Next steps</span></span>

- [<span data-ttu-id="3ca58-129">Che cos'è Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="3ca58-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
