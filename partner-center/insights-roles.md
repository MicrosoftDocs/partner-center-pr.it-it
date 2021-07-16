---
title: Partner Center Insights accesso in base al ruolo
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui ruoli specifici necessari per visualizzare Partner Center Insights report. Sono inclusi i ruoli di Executive Report Viewer e Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 836ae2ab193437fca501dc5c5713a4fe09b49ef4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375268"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Controllo degli accessi in base al ruolo nel dashboard Partner Center Insights ruolo

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Visualizzatore di report | Visualizzatore di report executive

Il dashboard Insights usa due nuovi ruoli in Partner Center per gestire l'accesso dei dipendenti ai report: Executive Report Viewer e Report Viewer.  Gli utenti con il ruolo Executive Report Viewer hanno accesso a tutti i set di dati di report, mentre gli utenti nel ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio ricavi e dati personali di clienti/dipendenti.  

Come per altri Partner Center, l'amministratore globale o l'amministratore account sarà in grado di assegnare gli utenti a tali ruoli nella pagina Gestione utenti. I ruoli possono essere applicabili all'intera azienda o per località Microsoft Partner Network (MPN) specifiche. I ruoli assegnati per località MPN specifiche limitano l'utente alla visualizzazione dei dati di report associati solo alle località MPN selezionate. Il partner può selezionare una o più località dalla visualizzazione seguente.

:::image type="content" source="images/insights/roles.png" alt-text="Mostra le impostazioni dei ruoli Partner Center Insights posizione per Visualizzatore report e Visualizzatore report executive.":::

>[!Note]
> Gli utenti amministratori dei partner MPN a partire dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo **Visualizzatore** di report executive a livello aziendale per tutte le posizioni per il tenant. Questi utenti possono quindi accedere ai report come visualizzatore di report executive senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente di questi utenti per aumentare o limitare ulteriormente le funzionalità.

## <a name="next-steps"></a>Passaggi successivi

- Altre informazioni sui [Partner Center Insights](partner-center-insights.md) e sui vari report.
