---
title: 'Guida introduttiva: gestire Azure Marketplace privato con PowerShell'
description: Questa Guida introduttiva illustra come gestire le offerte in Azure Marketplace privato usando Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412455"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Guida introduttiva: gestire Azure Marketplace privato con PowerShell

Questo articolo descrive come è possibile gestire le offerte in un Marketplace privato di Azure usando il modulo di PowerShell [AZ. Marketplace](/powershell/module/az.marketplace) .

> [!IMPORTANT]
> Azure Marketplace privato è attualmente disponibile in anteprima pubblica. Questa versione in anteprima viene fornita senza un contratto di servizio. Non è la scelta consigliata per carichi di lavoro di produzione. Alcune funzionalità potrebbero non essere supportate o potrebbero avere funzionalità vincolate. Per altre informazioni, vedere [Condizioni supplementari per l'utilizzo delle anteprime di Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).

## <a name="requirements"></a>Requisiti

* Se non si ha una sottoscrizione di Azure, creare un account [gratuito](https://azure.microsoft.com/free/) prima di iniziare.

* Se si sceglie di usare Azure PowerShell in locale:
  * [Installare il modulo Az di PowerShell](/powershell/azure/install-az-ps).
  * Connettersi all'account Azure con il cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).
* Se si sceglie di usare Azure Cloud Shell:
  * Vedere [Panoramica di Azure Cloud Shell](/azure/cloud-shell/overview) per altre informazioni.

  > [!IMPORTANT]
  > Mentre il modulo di PowerShell **AZ. Marketplace** è in anteprima, è necessario installarlo separatamente usando il `Install-Module` cmdlet. Quando il modulo di PowerShell diventerà disponibile a livello generale, entrerà a far parte delle future versioni del modulo Az di PowerShell e sarà disponibile per impostazione predefinita all'interno di Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Se si possiedono più sottoscrizioni di Azure, scegliere quella appropriata in cui verranno fatturate le risorse. Selezionare una sottoscrizione specifica usando il cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Elencare gli archivi privati

Per recuperare un elenco di archivi privati, usare il cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) . Nell'esempio seguente vengono elencati gli archivi privati creati nell'ambito del tenant.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Aggiungi un'offerta a un Marketplace privato

Per aggiungere un'offerta a un archivio privato, usare il cmdlet [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) . Nell'esempio seguente viene aggiunta l'offerta specificata a un Marketplace privato per un archivio privato creato nell'ambito del tenant.

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

## <a name="get-private-store-offers"></a>Ottieni offerte per lo store privato

Per ottenere una o più offerte di archivio privato, usare il cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) . Nell'esempio seguente vengono ottenute le offerte associate all'archivio privato specificato aggiunte nell'ambito del tenant.

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

## <a name="remove-an-offer"></a>Rimuovere un'offerta

Per rimuovere un'offerta da uno store privato, usare il cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) . Nell'esempio seguente viene rimossa un'offerta da un archivio privato creato nell'ambito del tenant.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Passaggi successivi

[Creare e gestire Azure Marketplace privato](create-manage-private-azure-marketplace.md).