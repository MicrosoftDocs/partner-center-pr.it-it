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
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="3cecd-104">Controllo degli accessi in base al ruolo nel dashboard Partner Center Insights</span><span class="sxs-lookup"><span data-stu-id="3cecd-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="3cecd-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="3cecd-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3cecd-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="3cecd-106">Global admin</span></span>
- <span data-ttu-id="3cecd-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="3cecd-107">Admin agent</span></span>
- <span data-ttu-id="3cecd-108">Visualizzatore di report</span><span class="sxs-lookup"><span data-stu-id="3cecd-108">Report viewer</span></span>
- <span data-ttu-id="3cecd-109">Visualizzatore di report esecutivi</span><span class="sxs-lookup"><span data-stu-id="3cecd-109">Executive report viewer</span></span>

<span data-ttu-id="3cecd-110">Il dashboard Informazioni dettagliate usa due nuovi ruoli in Partner Center per gestire l'accesso dei dipendenti ai report: Executive Report Viewer e Report Viewer.</span><span class="sxs-lookup"><span data-stu-id="3cecd-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="3cecd-111">Gli utenti con il ruolo Executive Report Viewer hanno accesso a tutti i set di dati di report, mentre gli utenti con il ruolo Visualizzatore report non avranno accesso ai set di dati sensibili, ad esempio i ricavi e i dati personali di clienti/dipendenti.</span><span class="sxs-lookup"><span data-stu-id="3cecd-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="3cecd-112">Come per altri Partner Center, l'amministratore globale o l'amministratore account sarà in grado di assegnare gli utenti a tali ruoli nella pagina Gestione utenti.</span><span class="sxs-lookup"><span data-stu-id="3cecd-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="3cecd-113">I ruoli possono essere applicabili all'intera azienda o per località MPN specifiche.</span><span class="sxs-lookup"><span data-stu-id="3cecd-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="3cecd-114">I ruoli assegnati per località MPN specifiche limitano l'utente alla visualizzazione dei dati dei report associati solo alle località MPN selezionate.</span><span class="sxs-lookup"><span data-stu-id="3cecd-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="3cecd-115">Il partner può selezionare una o più località dalla visualizzazione seguente.</span><span class="sxs-lookup"><span data-stu-id="3cecd-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Mostra le impostazioni dei ruoli Partner Center informazioni dettagliate specifiche per il visualizzatore di report e il visualizzatore di report executive.":::

>[!Note]
> <span data-ttu-id="3cecd-117">Gli utenti amministratori MPN dal 20 gennaio 2020 vengono aggiunti automaticamente al ruolo Executive **Report Viewer** a livello dell'azienda per tutte le posizioni per tale tenant.</span><span class="sxs-lookup"><span data-stu-id="3cecd-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="3cecd-118">Questi utenti sono quindi in grado di accedere ai report come visualizzatore di report esecutivi senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore account. Gli amministratori globali e gli amministratori dell'account possono eseguire l'override dei ruoli assegnati automaticamente di questi utenti per aumentare o limitare ulteriormente le funzionalità.</span><span class="sxs-lookup"><span data-stu-id="3cecd-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3cecd-119">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="3cecd-119">Next steps</span></span>

- <span data-ttu-id="3cecd-120">Altre informazioni su [Partner Center Insights](partner-center-insights.md) e sui vari report.</span><span class="sxs-lookup"><span data-stu-id="3cecd-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
