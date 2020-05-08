---
title: Ruoli, autorizzazioni per il credito guadagnato dal partner
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui ruoli e sulle autorizzazioni per i partner per poter guadagnare i crediti guadagnati dal partner (PEC). Questi sono diversi dai ruoli per lavorare nel centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: af21fe17afdab07ef259634d9df18d65ae072d5d
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908272"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Ruoli e autorizzazioni idonei per ottenere il credito guadagnato dal partner

I ruoli seguenti sono mappati ai livelli di autorizzazione che determinano se un partner è idoneo per i crediti ottenuti dal partner.

>[!Important]
>Questi ruoli e autorizzazioni non sono uguali ai ruoli e alle autorizzazioni che un utente deve usare nel centro per i partner.

|**Ruolo**   |**Descrizione**   |**Idoneo per PEC**   |
|-----------------|:------------------|:--------------|
|Proprietario  |Si gestiscono tutti gli elementi, incluso l'accesso alle risorse.|Sì|
|Collaboratore |Si gestiscono tutti gli elementi, ad eccezione della concessione dell'accesso alle risorse.|Sì|
|Lettore|È possibile visualizzare tutti gli elementi, ma non apportare modifiche|No|
|ACRDelete|eliminazione di ACR|Sì|
|ACRImageSigner|firmatario immagine acr|Sì|
|ACRPull|acr pull|Sì|
|AcrPush|acr push|Sì|
|AcrQuarantineReader|lettore di dati di quarantena acr|No|
|AcrQuarantineWriter| writer di dati di quarantena acr|Sì|
|Collaboratore servizio Gestione API|Può gestire il servizio e le API.|Sì|
|Ruolo operatore del servizio Gestione API|Può gestire il servizio ma non le API.|Sì|
|Ruolo lettura del servizio Gestione API|Consente l'accesso di sola lettura al servizio e alle API.|No|
|Collaboratore componente di Application Insights|Gestisce i componenti di Application Insights|Sì|
|Debugger di snapshot di Application Insights|Concede l'autorizzazione utente per visualizzare e scaricare gli snapshot di debug raccolti con Application Insights Snapshot Debugger. Si noti che queste autorizzazioni non sono incluse nei ruoli Proprietario e Collaboratore.|Sì|
|