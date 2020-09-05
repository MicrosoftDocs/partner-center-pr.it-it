---
title: Accesso basato sui ruoli di partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui ruoli specifici necessari per visualizzare i report di partner Center Insights. Sono inclusi i ruoli del Visualizzatore report Executive e del Visualizzatore report.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490609"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Controllo degli accessi in base al ruolo per il dashboard di partner Center Insights

Il dashboard Insights usa due nuovi ruoli nel centro per i partner per gestire l'accesso dei dipendenti ai report, il Visualizzatore di report e il Visualizzatore di report.  Gli utenti nel ruolo di Visualizzatore report Executive possono accedere a tutti i set di dati di report, mentre gli utenti del ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i dati personali relativi a ricavi e clienti.  

Come per gli altri ruoli del centro per i partner, l'amministratore globale o l'amministratore dell'account sarà in grado di assegnare gli utenti a tali ruoli nella pagina di gestione degli utenti. I ruoli possono essere applicabili all'intera azienda o per percorsi MPN specifici. I ruoli assegnati per percorsi MPN specifici limitano l'utente alla visualizzazione dei dati di report associati solo alle posizioni MPN selezionate. Il partner può selezionare uno o più percorsi dalla vista sottostante.

:::image type="content" source="images/pci/roles.png" alt-text="Mostra le impostazioni dei ruoli specifici del centro per i partner per Visualizzatore report e Visualizzatore report Executive.":::

>[!Note]
> Gli utenti che sono amministratori MPN a partire dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo di **Visualizzatore report Executive** a livello aziendale per tutte le località del tenant. Questi utenti possono quindi accedere ai report come visualizzatore di report Executive senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente a tali utenti per aumentarne o limitarne le funzionalità.

## <a name="next-steps"></a>Passaggi successivi

- Scopri di più su [Partner Center Insights](partner-center-insights.md) e sui vari report.
