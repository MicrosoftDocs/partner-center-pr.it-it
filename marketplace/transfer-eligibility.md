---
title: 'Idoneità per il trasferimento: linee guida per il trasferimento di una sottoscrizione tra account di fatturazione, Azure Marketplace'
description: Linee guida per i controlli commerciali prima di trasferire una sottoscrizione tra gli account di fatturazione nel portale di Azure.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412557"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Trasferire idoneità per una sottoscrizione tra account di fatturazione

È possibile [trasferire una sottoscrizione](/azure/cost-management-billing/understand/subscription-transfer) da un account di fatturazione a un altro nella sezione relativa alla fatturazione del portale di Azure. Prima di un trasferimento, la sottoscrizione viene analizzata per i prodotti di terze parti. Il trasferimento è consentito solo se *tutti* i prodotti vengono cancellati per il trasferimento (vedere i [criteri](#criteria-for-transfer-approval-or-denial) indicati di seguito). Il sistema genererà messaggi di errore rilevanti per le app che non sono state cancellate per facilitare la determinazione dei passaggi successivi.

> [!NOTE]
> Questo articolo non si applica alle offerte SaaS perché le risorse SaaS sono collegate a un tenant, non a una sottoscrizione. Le risorse SaaS sono trasferibili da un account di fatturazione a un altro, ma questa operazione viene eseguita per risorsa e dal supporto tecnico di Azure come richiesta di supporto.

## <a name="criteria-for-transfer-approval-or-denial"></a>Criteri per l'approvazione o il rifiuto del trasferimento

Non è possibile trasferire una sottoscrizione se una delle app di terze parti soddisfa uno dei criteri seguenti:

- L'account di destinazione è commerciale e l'app è esplicitamente venduta tramite partner.
- L'app è il consenso esplicito per i partner selezionati e l'account di destinazione non è presente nell'elenco Consenti.
- L'offerta è stata un'offerta di anteprima nel passato per le sottoscrizioni selezionate oppure è stata un'offerta privata e la sottoscrizione non è più disponibile nell'elenco Consenti.
- Il nuovo account di fatturazione si trova in un'area diversa da quella in cui viene venduta l'offerta e l'offerta non viene venduta in tale area.

Un trasferimento bloccato rimane attivo fino a quando non si rimuove la risorsa dalla sottoscrizione, dopodiché è possibile riprovare il trasferimento.

## <a name="next-steps"></a>Passaggi successivi

[Ottenere supporto per Microsoft AppSource e Azure Marketplace](get-support.md)

