---
title: Partner Center'accesso in base al ruolo di Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui ruoli specifici necessari per visualizzare i report Partner Center Insights. Sono inclusi i ruoli di Executive Report Viewer e Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb06a863218446b0e88b38af242b4dac044560c0
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565305"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Controllo degli accessi in base al ruolo nel dashboard Partner Center Insights

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Visualizzatore di report | Visualizzatore di report executive

Il dashboard di Insights usa due nuovi ruoli in Partner Center per gestire l'accesso dei dipendenti ai report: Executive Report Viewer e Report Viewer.  Gli utenti con il ruolo Executive Report Viewer hanno accesso a tutti i set di dati di report, mentre gli utenti nel ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i ricavi e i dati personali di clienti/dipendenti.  

Come per altri Partner Center, l'amministratore globale o l'amministratore account sarà in grado di assegnare gli utenti a tali ruoli nella pagina Gestione utenti. I ruoli possono essere applicabili all'intera azienda o per località Microsoft Partner Network (MPN) specifiche. I ruoli assegnati per località MPN specifiche limitano l'utente alla visualizzazione dei dati di report associati solo alle località MPN selezionate. Il partner può selezionare una o più località dalla visualizzazione seguente.

:::image type="content" source="images/pci/roles.png" alt-text="Mostra le impostazioni dei ruoli Partner Center informazioni dettagliate specifiche della posizione per Visualizzatore report e Visualizzatore report executive.":::

>[!Note]
> Gli utenti amministratori di partner MPN a partire dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo Visualizzatore di report executive a livello aziendale per tutte le posizioni per il tenant.  Questi utenti possono quindi accedere ai report come visualizzatore di report executive senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente di questi utenti per aumentare o limitare ulteriormente le funzionalità.

## <a name="next-steps"></a>Passaggi successivi

- Altre informazioni su [Partner Center Insights](partner-center-insights.md) e sui vari report.
