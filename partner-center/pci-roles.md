---
title: Partner Center Insights-controllo degli accessi in base al ruolo | Centro per i partner
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Per visualizzare i report di Insights sono necessari ruoli specifici
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI, prestazioni, successo dei clienti, misurazioni, ruoli
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945863"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a>Controllo degli accessi in base al ruolo per il dashboard Insights

Il dashboard Insights usa due nuovi ruoli nel centro per i partner per gestire l'accesso dei dipendenti ai report, il Visualizzatore di report e il Visualizzatore di report.  Gli utenti nel ruolo di Visualizzatore report Executive possono accedere a tutti i set di dati di report, mentre gli utenti del ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i dati personali relativi a ricavi e clienti.  

Come per gli altri ruoli del centro per i partner, l'amministratore globale o l'amministratore dell'account sarà in grado di assegnare gli utenti a tali ruoli nella pagina di gestione degli utenti. I ruoli possono essere applicabili all'intera azienda o per percorsi MPN specifici. I ruoli assegnati per percorsi MPN specifici limitano l'utente alla visualizzazione dei dati di report associati solo alle posizioni MPN selezionate. Il partner può selezionare uno o più percorsi dalla vista sottostante.

![Ruoli](images/pci/roles.png)

>Si noti Gli utenti che sono amministratori MPN a partire dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo "Visualizzatore report Executive" a livello aziendale per tutte le località del tenant. Questi utenti possono quindi accedere ai report come visualizzatore di report Executive senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente a tali utenti per aumentarne o limitarne le funzionalità.