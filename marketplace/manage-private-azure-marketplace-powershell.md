---
title: 'Guida introduttiva: gestire Azure Marketplace privato con PowerShell'
description: Questa Guida introduttiva illustra come gestire le offerte in Azure Marketplace privato usando Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536080"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="d1db9-103">Guida introduttiva: gestire Azure Marketplace privato con PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1db9-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="d1db9-104">Questo articolo descrive come è possibile gestire le offerte in un Marketplace privato di Azure usando il modulo di PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .</span><span class="sxs-lookup"><span data-stu-id="d1db9-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d1db9-105">Azure Marketplace privato è attualmente disponibile in anteprima pubblica.</span><span class="sxs-lookup"><span data-stu-id="d1db9-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="d1db9-106">Questa versione in anteprima viene fornita senza un contratto di servizio.</span><span class="sxs-lookup"><span data-stu-id="d1db9-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="d1db9-107">Non è la scelta consigliata per carichi di lavoro di produzione.</span><span class="sxs-lookup"><span data-stu-id="d1db9-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="d1db9-108">Alcune funzionalità potrebbero non essere supportate o potrebbero avere funzionalità vincolate.</span><span class="sxs-lookup"><span data-stu-id="d1db9-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="d1db9-109">Per altre informazioni, vedere [Condizioni supplementari per l'utilizzo delle anteprime di Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="d1db9-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="d1db9-110">Requisiti</span><span class="sxs-lookup"><span data-stu-id="d1db9-110">Requirements</span></span>

* <span data-ttu-id="d1db9-111">Se non si ha una sottoscrizione di Azure, creare un account [gratuito](https://azure.microsoft.com/free/) prima di iniziare.</span><span class="sxs-lookup"><span data-stu-id="d1db9-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="d1db9-112">Se si sceglie di usare Azure PowerShell in locale:</span><span class="sxs-lookup"><span data-stu-id="d1db9-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="d1db9-113">[Installare il modulo Az di PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="d1db9-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="d1db9-114">Connettersi all'account Azure con il cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="d1db9-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="d1db9-115">Se si sceglie di usare Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="d1db9-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="d1db9-116">Vedere [Panoramica di Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) per altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="d1db9-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="d1db9-117">Mentre il modulo di PowerShell **AZ. Marketplace** è in anteprima, è necessario installarlo separatamente usando il `Install-Module` cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d1db9-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="d1db9-118">Quando il modulo di PowerShell diventerà disponibile a livello generale, entrerà a far parte delle future versioni del modulo Az di PowerShell e sarà disponibile per impostazione predefinita all'interno di Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="d1db9-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="d1db9-119">Se si possiedono più sottoscrizioni di Azure, scegliere quella appropriata in cui verranno fatturate le risorse.</span><span class="sxs-lookup"><span data-stu-id="d1db9-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="d1db9-120">Selezionare una sottoscrizione specifica usando il cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="d1db9-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="d1db9-121">Elencare gli archivi privati</span><span class="sxs-lookup"><span data-stu-id="d1db9-121">List private stores</span></span>

<span data-ttu-id="d1db9-122">Per recuperare un elenco di archivi privati, usare il cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="d1db9-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="d1db9-123">Nell'esempio seguente vengono elencati gli archivi privati creati nell'ambito del tenant.</span><span class="sxs-lookup"><span data-stu-id="d1db9-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="d1db9-124">Aggiungi un'offerta a un Marketplace privato</span><span class="sxs-lookup"><span data-stu-id="d1db9-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="d1db9-125">Per aggiungere un'offerta a un archivio privato, usare il cmdlet [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d1db9-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d1db9-126">Nell'esempio seguente viene aggiunta l'offerta specificata a un Marketplace privato per un archivio privato creato nell'ambito del tenant.</span><span class="sxs-lookup"><span data-stu-id="d1db9-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="d1db9-127">Ottieni offerte per lo store privato</span><span class="sxs-lookup"><span data-stu-id="d1db9-127">Get private store offers</span></span>

<span data-ttu-id="d1db9-128">Per ottenere una o più offerte di archivio privato, usare il cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d1db9-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d1db9-129">Nell'esempio seguente vengono ottenute le offerte associate all'archivio privato specificato aggiunte nell'ambito del tenant.</span><span class="sxs-lookup"><span data-stu-id="d1db9-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="d1db9-130">Rimuovere un'offerta</span><span class="sxs-lookup"><span data-stu-id="d1db9-130">Remove an offer</span></span>

<span data-ttu-id="d1db9-131">Per rimuovere un'offerta da uno store privato, usare il cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d1db9-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d1db9-132">Nell'esempio seguente viene rimossa un'offerta da un archivio privato creato nell'ambito del tenant.</span><span class="sxs-lookup"><span data-stu-id="d1db9-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="d1db9-133">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d1db9-133">Next steps</span></span>

<span data-ttu-id="d1db9-134">[Creare e gestire Azure Marketplace privato](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
