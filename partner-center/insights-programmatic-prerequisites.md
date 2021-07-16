---
title: Prerequisiti per accedere ai dati di analisi a livello di codice
description: Prerequisiti per accedere ai dati di analisi a livello di codice
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375352"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="bd9aa-103">Prerequisiti per accedere ai dati di analisi a livello di codice</span><span class="sxs-lookup"><span data-stu-id="bd9aa-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="bd9aa-104">**Ruoli appropriati:** Amministratore globale | Amministratore MPN</span><span class="sxs-lookup"><span data-stu-id="bd9aa-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="bd9aa-105">Prima di poter accedere a livello di codice ai dati di analisi delle informazioni dettagliate dei partner, è necessario soddisfare i requisiti seguenti.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="bd9aa-106">Registrazione al programma MPN</span><span class="sxs-lookup"><span data-stu-id="bd9aa-106">MPN Program enrollment</span></span>

<span data-ttu-id="bd9aa-107">Per accedere ai dati di analisi delle informazioni dettagliate dei partner a livello di codice, è necessario essere registrati nel programma MPN e avere un account Partner Center partner.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="bd9aa-108">Per informazioni, vedere [Creare un account MPN in Partner Center](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="bd9aa-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="bd9aa-109">Creare Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="bd9aa-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="bd9aa-110">Le normali credenziali utente non possono essere usate per l'accesso a livello di codice ai dati di Analisi Insights partner.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="bd9aa-111">Per accedere alle API di accesso a livello di codice, è necessario creare un'applicazione Azure Active Directory (AAD) insieme a un segreto (applicazione e accesso utente).</span><span class="sxs-lookup"><span data-stu-id="bd9aa-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="bd9aa-112">Per informazioni su come creare un'applicazione AAD e un segreto, vedere [Avvio rapido: Registrare un'applicazione](/azure/active-directory/develop/quickstart-register-app) con il Microsoft Identity Platform.   L'autorizzazione è necessaria per accedere a Microsoft API Partner.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="bd9aa-113">Per informazioni su come aggiungere autorizzazioni, vedere Autenticazione [API Partner - Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="bd9aa-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="bd9aa-114">Assegnare il ruolo Executive Report Viewer (ERV) all'utente</span><span class="sxs-lookup"><span data-stu-id="bd9aa-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="bd9aa-115">Per accedere ai dati di analisi delle informazioni dettagliate dei partner a livello di codice, è necessario disporre di Executive Report Viewer (ERV).</span><span class="sxs-lookup"><span data-stu-id="bd9aa-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="bd9aa-116">Per informazioni su come assegnare il ruolo ERV all'utente, [Partner Center Insights'accesso in](insights-roles.md) base al ruolo - Partner Center</span><span class="sxs-lookup"><span data-stu-id="bd9aa-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="bd9aa-117">Generare un token AAD</span><span class="sxs-lookup"><span data-stu-id="bd9aa-117">Generate an AAD token</span></span>

<span data-ttu-id="bd9aa-118">È necessario generare un token AAD usando l'ID applicazione (client), il segreto client, l'ID utente e la password.   [Vedere qui](insights-programmatic-first-api-call.md#token-generation) per la procedura per generare il token AAD.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="bd9aa-119">Il token è valido per un'ora.</span><span class="sxs-lookup"><span data-stu-id="bd9aa-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bd9aa-120">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="bd9aa-120">Next steps</span></span>
[<span data-ttu-id="bd9aa-121">Paradigma di accesso a livello di codice</span><span class="sxs-lookup"><span data-stu-id="bd9aa-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)