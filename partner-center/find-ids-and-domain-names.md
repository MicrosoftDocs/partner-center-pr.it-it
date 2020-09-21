---
title: Trovare l'ID tenant, il nome di dominio, l'ID oggetto utente
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come trovare gli ID nell'portale di Azure, ovvero l'ID tenant, il nome di dominio o l'ID oggetto utente specifico di un'organizzazione Azure AD. Per alcune attività sono necessarie queste informazioni.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/17/2020
ms.locfileid: "90740404"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="15237-104">Individuare gli ID importanti per un utente</span><span class="sxs-lookup"><span data-stu-id="15237-104">Locate important IDs for a user</span></span>

<span data-ttu-id="15237-105">Questo articolo descrive come usare la [portale di Azure](https://portal.azure.com/) per individuare le informazioni seguenti per un utente:</span><span class="sxs-lookup"><span data-stu-id="15237-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="15237-106">ID tenant di Microsoft Azure Active Directory (Azure AD) dell'organizzazione o dell'azienda dell'utente</span><span class="sxs-lookup"><span data-stu-id="15237-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="15237-107">Nome di dominio primario dell'organizzazione o della società associata al tenant di Azure AD</span><span class="sxs-lookup"><span data-stu-id="15237-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="15237-108">ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="15237-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="15237-109">Trovare l'ID tenant Microsoft Azure AD e il nome di dominio primario</span><span class="sxs-lookup"><span data-stu-id="15237-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="15237-110">Seguire questa procedura per individuare l'ID tenant Azure AD o il nome di dominio primario all'interno del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="15237-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span>

> [!NOTE]
> <span data-ttu-id="15237-111">L'ID tenant può essere chiamato nomi diversi in applicazioni o risorse diverse.</span><span class="sxs-lookup"><span data-stu-id="15237-111">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="15237-112">Ad esempio, l'ID tenant può essere indicato come ID directory, il tenant Azure Active Directory (Azure AD), l'ID Microsoft o per determinati report, anche *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="15237-112">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="15237-113">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="15237-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="15237-114">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="15237-114">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portale di Azure selezionando l'opzione Azure Active Directory dal menu.":::

3. <span data-ttu-id="15237-116">Viene visualizzata una pagina di **panoramica** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="15237-116">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="15237-117">Per trovare l'ID tenant Azure AD o il nome di dominio primario, cercare il campo **ID tenant** e il campo **dominio primario** .</span><span class="sxs-lookup"><span data-stu-id="15237-117">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="15237-118">Questi campi vengono visualizzati nella sezione informazioni sul tenant.</span><span class="sxs-lookup"><span data-stu-id="15237-118">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra la pagina di panoramica con due campi evidenziati, l'ID tenant e il nome di dominio primario.":::

4. <span data-ttu-id="15237-120">È possibile trovare l'ID tenant nel portale di Azure in altri modi.</span><span class="sxs-lookup"><span data-stu-id="15237-120">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="15237-121">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="15237-121">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="15237-122">Individuare quindi la sezione **Gestisci** del menu e selezionare **Proprietà**.</span><span class="sxs-lookup"><span data-stu-id="15237-122">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="15237-123">La pagina delle proprietà Visualizza anche l'ID tenant associato dell'utente.</span><span class="sxs-lookup"><span data-stu-id="15237-123">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra la pagina delle proprietà con il campo ID tenant evidenziato.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="15237-125">Trovare l'ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="15237-125">Find the user object ID</span></span>

<span data-ttu-id="15237-126">Solo la ricerca del nome di dominio e dell'ID tenant potrebbe non essere sempre sufficiente.</span><span class="sxs-lookup"><span data-stu-id="15237-126">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="15237-127">Potrebbe anche essere necessario trovare l'ID oggetto specifico assegnato a un utente.</span><span class="sxs-lookup"><span data-stu-id="15237-127">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="15237-128">Attenersi alla procedura seguente per trovare l'ID oggetto di un utente nel portale di Azure:</span><span class="sxs-lookup"><span data-stu-id="15237-128">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="15237-129">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="15237-129">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="15237-130">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="15237-130">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="15237-131">Individuare la sezione **Gestisci** del menu, quindi selezionare **utenti**.</span><span class="sxs-lookup"><span data-stu-id="15237-131">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu con l'opzione evidenziata, utenti.":::

4. <span data-ttu-id="15237-133">Nella pagina utenti digitare il nome dell'utente nella casella di ricerca.</span><span class="sxs-lookup"><span data-stu-id="15237-133">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra la pagina utenti con la casella di ricerca per cercare un utente specifico.":::

5. <span data-ttu-id="15237-135">Selezionare il nome dell'utente in cui viene visualizzato nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="15237-135">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra la pagina utente che visualizza una riga per l'utente cercato.":::

6. <span data-ttu-id="15237-137">Individuare la sezione Identity nella pagina del profilo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="15237-137">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="15237-138">Il campo ID oggetto viene visualizzato con l'ID oggetto univoco dell'utente.</span><span class="sxs-lookup"><span data-stu-id="15237-138">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra la pagina del profilo utente con la sezione Identity e un campo evidenziato per l'ID oggetto.":::

## <a name="next-steps"></a><span data-ttu-id="15237-140">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="15237-140">Next steps</span></span>

- [<span data-ttu-id="15237-141">Altre informazioni sui profili utente in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="15237-141">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="15237-142">Scopri in che modo i partner possono visualizzare o esportare i dettagli dei clienti nel centro per i partner</span><span class="sxs-lookup"><span data-stu-id="15237-142">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)