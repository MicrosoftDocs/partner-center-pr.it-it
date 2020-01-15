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
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="49eea-104">Controllo degli accessi in base al ruolo per il dashboard Insights</span><span class="sxs-lookup"><span data-stu-id="49eea-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="49eea-105">Il dashboard Insights usa due nuovi ruoli nel centro per i partner per gestire l'accesso dei dipendenti ai report, il Visualizzatore di report e il Visualizzatore di report.</span><span class="sxs-lookup"><span data-stu-id="49eea-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="49eea-106">Gli utenti nel ruolo di Visualizzatore report Executive possono accedere a tutti i set di dati di report, mentre gli utenti del ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i dati personali relativi a ricavi e clienti.</span><span class="sxs-lookup"><span data-stu-id="49eea-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="49eea-107">Come per gli altri ruoli del centro per i partner, l'amministratore globale o l'amministratore dell'account sarà in grado di assegnare gli utenti a tali ruoli nella pagina di gestione degli utenti.</span><span class="sxs-lookup"><span data-stu-id="49eea-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="49eea-108">I ruoli possono essere applicabili all'intera azienda o per percorsi MPN specifici.</span><span class="sxs-lookup"><span data-stu-id="49eea-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="49eea-109">I ruoli assegnati per percorsi MPN specifici limitano l'utente alla visualizzazione dei dati di report associati solo alle posizioni MPN selezionate.</span><span class="sxs-lookup"><span data-stu-id="49eea-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="49eea-110">Il partner può selezionare uno o più percorsi dalla vista sottostante.</span><span class="sxs-lookup"><span data-stu-id="49eea-110">Partner can select one or multiple locations from the below view.</span></span>

![Ruoli](images/pci/roles.png)

><span data-ttu-id="49eea-112">Si noti Gli utenti che sono amministratori MPN a partire dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo "Visualizzatore report Executive" a livello aziendale per tutte le località del tenant.</span><span class="sxs-lookup"><span data-stu-id="49eea-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="49eea-113">Questi utenti possono quindi accedere ai report come visualizzatore di report Executive senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente a tali utenti per aumentarne o limitarne le funzionalità.</span><span class="sxs-lookup"><span data-stu-id="49eea-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>