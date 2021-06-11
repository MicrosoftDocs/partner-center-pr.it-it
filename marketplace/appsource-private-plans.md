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
# <a name="private-plans-in-microsoft-appsource"></a>Piani privati in Microsoft AppSource

I piani privati sono il modo in cui gli editori forniscono piani personalizzati a clienti specifici. Questa opzione è ora disponibile in Microsoft AppSource. I piani privati possono essere venduti in AppSource per le  offerte SaaS (Software as a Service) con l'invito all'azione Scarica adesso.

## <a name="ask-your-isv-for-a-private-plan"></a>Richiedere un piano privato all'ISV

Perché un piano privato sia disponibile in AppSource, è necessario contattare direttamente l'ISV e negoziare un prezzo personalizzato e specifiche tecniche. Una volta accettate le condizioni del piano privato, l'ISV creerà automaticamente un piano e lo assegna all'ID tenant dell'organizzazione, che sarà necessario fornire.

### <a name="finding-your-tenant-id"></a>Ricerca dell'ID tenant

1. In AppSource, nell'angolo in alto a destra, selezionare l'icona del profilo dell'account e quindi **Visualizza tenant.**
2. Copiare l'ID tenant e specificarlo nell'ISV.

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Illustra come trovare l'ID tenant.":::

## <a name="find-a-private-plan-in-appsource"></a>Trovare un piano privato in AppSource

La pubblicazione del nuovo piano privato da parte dell'ISV può richiedere fino a 48 ore prima che venga visualizzato in AppSource. Per trovare i piani privati associati all'ID tenant, selezionare **Piani privati** (icona a forma di lucchetto) in alto a destra in AppSource.

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Mostra l'icona a forma di lucchetto (lucchetto) nella barra degli strumenti superiore.":::

Se non è stato eseguito l'accesso, verrà visualizzato un messaggio che richiede di eseguire questa operazione. È quindi possibile acquistare i piani privati associati all'ID tenant nella **scheda Piani e** prezzi.

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Mostra le offerte private nella scheda piano e prezzi.":::

Se i piani privati non sono disponibili per il tenant, verrà visualizzato un messaggio che indica che non sono presenti piani o offerte privati.

## <a name="purchase-a-private-plan"></a>Acquistare un piano privato

Un ISV può includere uno o più piani privati all'interno di un'offerta. Ogni offerta può avere piani sia pubblici che privati, ma i piani privati vengono visualizzati in una pagina separata di presentazione dell'offerta accessibile dall'icona offerte private (lucchetto) in alto a destra nella pagina.

I piani privati disponibili vengono visualizzati **nella scheda Piani e** prezzi. I piani privati hanno un badge blu distintivo.

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Mostra la notifica dell'offerta privata blu accanto alle offerte private.":::

Per acquistare un piano selezionato, selezionare **Scarica adesso** e seguire la procedura fornita.

## <a name="next-steps"></a>Passaggi successivi

- [Che cos'è Microsoft AppSource?](appsource-overview.md)
