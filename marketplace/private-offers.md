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
# <a name="private-offers-in-azure-marketplace"></a>Offerte private in Azure Marketplace

Le offerte private rappresentano il modo in cui i Publisher forniscono piani personalizzati a specifici clienti. Questa opzione è attualmente supportata solo nell'esperienza di Azure Marketplace nell'portale di Azure. Le offerte private sono disponibili solo per le offerte a pagamento che possono essere acquistate e installate direttamente dalla portale di Azure. Publisher non può creare offerte private per i servizi di consulenza, qualsiasi servizio che ha **contattato** come chiamata a azione o qualsiasi servizio gratuito, indipendentemente dal fatto che sia possibile installarlo o meno dal portale.

## <a name="find-private-offers-in-the-azure-portal"></a>Trova le offerte private nella portale di Azure

Quando un partner pubblica un'offerta privata, è visibile solo agli utenti idonei nella sezione **Marketplace** del portale di Azure. Questi utenti sono definiti tramite ID sottoscrizione o ID tenant, a seconda del tipo di offerta. Se si è idonei per offerte private, esistono due modi per individuarli nel portale.

> [!NOTE]
> Le offerte private non sono attualmente disponibili per la ricerca o filtrabili (per categoria) nell'portale di Azure.

Nella portale di Azure selezionare **+ Crea una risorsa** o cercare "Marketplace" per passare alla pagina del **Marketplace** . Se si è idonei per offerte private, si noterà che l'utente dispone di un banner **disponibile** nella parte superiore della pagina. Selezionare **Visualizza offerte private** per accedere alla pagina delle offerte private.

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banner visualizzato quando sono disponibili offerte private.":::

In alternativa, se viene visualizzato il banner delle offerte private, è anche possibile scorrere fino alla fine della pagina della raccolta di prodotti e viene visualizzato un subset delle offerte private. Selezionare il collegamento per **visualizzare altre informazioni** per passare alla pagina delle offerte private.

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Mostra le offerte private nella parte inferiore della schermata, insieme al collegamento Vedi altro.":::

## <a name="review-private-plans"></a>Esaminare i piani privati

Un'offerta privata è in realtà un piano privato all'interno di un'offerta. Ogni offerta può avere più piani, sia pubblici che privati, ma i piani privati vengono visualizzati in un elenco separato dei piani pubblici.

È possibile visualizzare i piani privati disponibili nella scheda **piani** , contrassegnati con una notifica **privata** distintiva:

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Pagina di piani contrassegnata come privata.":::

Se si dispone di più di una sottoscrizione, vengono visualizzate tutte le offerte private disponibili per tutte le sottoscrizioni. Quando si seleziona **Crea**, si viene indirizzati alla pagina di creazione della risorsa per iniziare a configurare la risorsa.

Se si seleziona **Crea** e si hanno più sottoscrizioni, ma non tutte vengono aggiunte al piano privato, la sottoscrizione predefinita potrebbe non essere la sottoscrizione idonea per questa offerta privata. In questo caso, selezionare la sottoscrizione corretta.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Il collegamento che mostra la disponibilità di offerte private è maggiore.":::

## <a name="next-steps"></a>Passaggi successivi

- [Che cos'è Azure Marketplace?](azure-marketplace-overview.md)
