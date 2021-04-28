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
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120784"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Controllo degli accessi in base al ruolo nel dashboard Partner Center Insights

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore
- Visualizzatore di report
- Visualizzatore di report esecutivi

Il dashboard Informazioni dettagliate usa due nuovi ruoli in Partner Center per gestire l'accesso dei dipendenti ai report: Executive Report Viewer e Report Viewer.  Gli utenti con il ruolo Executive Report Viewer hanno accesso a tutti i set di dati di report, mentre gli utenti con il ruolo Visualizzatore report non avranno accesso ai set di dati sensibili, ad esempio i ricavi e i dati personali di clienti/dipendenti.  

Come per altri Partner Center, l'amministratore globale o l'amministratore account sarà in grado di assegnare gli utenti a tali ruoli nella pagina Gestione utenti. I ruoli possono essere applicabili all'intera azienda o per località MPN specifiche. I ruoli assegnati per località MPN specifiche limitano l'utente alla visualizzazione dei dati dei report associati solo alle località MPN selezionate. Il partner può selezionare una o più località dalla visualizzazione seguente.

:::image type="content" source="images/pci/roles.png" alt-text="Mostra le impostazioni dei ruoli Partner Center informazioni dettagliate specifiche per il visualizzatore di report e il visualizzatore di report executive.":::

>[!Note]
> Gli utenti amministratori MPN dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo Executive **Report Viewer** a livello dell'azienda per tutte le posizioni per tale tenant. Questi utenti sono quindi in grado di accedere ai report come visualizzatore di report esecutivi senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente di questi utenti per aumentare o limitare ulteriormente le funzionalità.

## <a name="next-steps"></a>Passaggi successivi

- Altre informazioni su [Partner Center Insights](partner-center-insights.md) e sui vari report.
