---
title: 'Idoneità per il trasferimento: linee guida per il trasferimento di una sottoscrizione tra account di fatturazione, Azure Marketplace'
description: Linee guida per i controlli commerciali prima di trasferire una sottoscrizione tra gli account di fatturazione nel portale di Azure.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007221"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="b7174-103">Trasferire idoneità per una sottoscrizione tra account di fatturazione</span><span class="sxs-lookup"><span data-stu-id="b7174-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="b7174-104">È possibile [trasferire una sottoscrizione](/azure/cost-management-billing/understand/subscription-transfer) da un account di fatturazione a un altro nella sezione relativa alla fatturazione del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="b7174-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="b7174-105">Prima di un trasferimento, la sottoscrizione viene analizzata per i prodotti di terze parti.</span><span class="sxs-lookup"><span data-stu-id="b7174-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="b7174-106">Il trasferimento è consentito solo se *tutti* i prodotti vengono cancellati per il trasferimento (vedere i [criteri](#criteria-for-transfer-approval-or-denial) indicati di seguito).</span><span class="sxs-lookup"><span data-stu-id="b7174-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="b7174-107">Il sistema genererà messaggi di errore rilevanti per le app che non sono state cancellate per facilitare la determinazione dei passaggi successivi.</span><span class="sxs-lookup"><span data-stu-id="b7174-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="b7174-108">Questo articolo non si applica alle offerte SaaS perché le risorse SaaS sono collegate a un tenant, non a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="b7174-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="b7174-109">Le risorse SaaS sono trasferibili da un account di fatturazione a un altro, ma questa operazione viene eseguita per risorsa e dal supporto tecnico di Azure come richiesta di supporto.</span><span class="sxs-lookup"><span data-stu-id="b7174-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="b7174-110">Criteri per l'approvazione o il rifiuto del trasferimento</span><span class="sxs-lookup"><span data-stu-id="b7174-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="b7174-111">Non è possibile trasferire una sottoscrizione se una delle app di terze parti soddisfa uno dei criteri seguenti:</span><span class="sxs-lookup"><span data-stu-id="b7174-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="b7174-112">L'account di destinazione è commerciale e l'app è esplicitamente venduta tramite partner.</span><span class="sxs-lookup"><span data-stu-id="b7174-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="b7174-113">L'app è il consenso esplicito per i partner selezionati e l'account di destinazione non è presente nell'elenco Consenti.</span><span class="sxs-lookup"><span data-stu-id="b7174-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="b7174-114">L'offerta è stata un'offerta di anteprima nel passato per le sottoscrizioni selezionate oppure è stata un'offerta privata e la sottoscrizione non è più disponibile nell'elenco Consenti.</span><span class="sxs-lookup"><span data-stu-id="b7174-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="b7174-115">Il nuovo account di fatturazione si trova in un'area diversa da quella in cui viene venduta l'offerta e l'offerta non viene venduta in tale area.</span><span class="sxs-lookup"><span data-stu-id="b7174-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="b7174-116">Un trasferimento bloccato rimane attivo fino a quando non si rimuove la risorsa dalla sottoscrizione, dopodiché è possibile riprovare il trasferimento.</span><span class="sxs-lookup"><span data-stu-id="b7174-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b7174-117">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b7174-117">Next steps</span></span>

[<span data-ttu-id="b7174-118">Ottenere supporto per Microsoft AppSource e Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="b7174-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

