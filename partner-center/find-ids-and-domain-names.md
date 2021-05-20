---
title: Trovare l'ID tenant, il nome di dominio, l'ID oggetto utente
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Informazioni su come trovare gli ID nel portale di Azure: ID tenant, nome di dominio o ID oggetto utente specifico Azure AD'organizzazione. Alcune attività necessitano di queste informazioni."
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150863"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="5f422-104">Individuare gli ID importanti per un utente</span><span class="sxs-lookup"><span data-stu-id="5f422-104">Locate important IDs for a user</span></span>

<span data-ttu-id="5f422-105">**Ruoli appropriati:** Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="5f422-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="5f422-106">Questo articolo descrive come usare il portale di Azure [per](https://portal.azure.com/) individuare le informazioni seguenti per un utente:</span><span class="sxs-lookup"><span data-stu-id="5f422-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="5f422-107">ID Microsoft Azure Active Directory tenant (Azure AD) dell'organizzazione o della società dell'utente</span><span class="sxs-lookup"><span data-stu-id="5f422-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="5f422-108">Nome di dominio primario dell'organizzazione o della società associata al tenant Azure AD locale</span><span class="sxs-lookup"><span data-stu-id="5f422-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="5f422-109">ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="5f422-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="5f422-110">Trovare l'ID Microsoft Azure AD tenant e il nome di dominio primario</span><span class="sxs-lookup"><span data-stu-id="5f422-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="5f422-111">Seguire questa procedura per individuare l'ID tenant Azure AD o il nome di dominio primario all'interno del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="5f422-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="5f422-112">Se si desidera trovare un ID tenant a livello di codice, vedere [Trovare l'ID tenant con PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)o l'interfaccia della riga di comando.</span><span class="sxs-lookup"><span data-stu-id="5f422-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="5f422-113">L'ID tenant può essere chiamato nomi diversi in applicazioni o risorse diverse.</span><span class="sxs-lookup"><span data-stu-id="5f422-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="5f422-114">Ad esempio, l'ID tenant può essere indicato come ID directory, tenant Azure Active Directory (Azure AD), ID Microsoft o per determinati report, anche *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="5f422-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="5f422-115">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5f422-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5f422-116">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5f422-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portale di Azure l'opzione Azure Active Directory dal menu.":::

3. <span data-ttu-id="5f422-118">Viene Azure Active Directory **pagina Panoramica.**</span><span class="sxs-lookup"><span data-stu-id="5f422-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="5f422-119">Per trovare l'ID tenant Azure AD o il nome di dominio primario, cercare il campo **ID tenant** e il **campo Dominio** primario.</span><span class="sxs-lookup"><span data-stu-id="5f422-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="5f422-120">Questi campi vengono visualizzati nella sezione Informazioni sul tenant.</span><span class="sxs-lookup"><span data-stu-id="5f422-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Visualizza la pagina Panoramica con due campi evidenziati, l'ID tenant e il nome di dominio primario.":::

4. <span data-ttu-id="5f422-122">È possibile trovare l'ID tenant nella portale di Azure in altri modi.</span><span class="sxs-lookup"><span data-stu-id="5f422-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="5f422-123">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5f422-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="5f422-124">Individuare quindi la **sezione Gestisci** nel menu e selezionare **Proprietà.**</span><span class="sxs-lookup"><span data-stu-id="5f422-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="5f422-125">La pagina Proprietà visualizza anche l'ID tenant associato dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5f422-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra la pagina Proprietà con il campo ID tenant evidenziato.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="5f422-127">Trovare l'ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="5f422-127">Find the user object ID</span></span>

<span data-ttu-id="5f422-128">La semplice ricerca del nome di dominio e dell'ID tenant potrebbe non essere sempre sufficiente.</span><span class="sxs-lookup"><span data-stu-id="5f422-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="5f422-129">Potrebbe anche essere necessario individuare l'ID oggetto specifico assegnato a un utente.</span><span class="sxs-lookup"><span data-stu-id="5f422-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="5f422-130">Seguire questa procedura per trovare l'ID oggetto di un utente nella portale di Azure:</span><span class="sxs-lookup"><span data-stu-id="5f422-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="5f422-131">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5f422-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5f422-132">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5f422-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="5f422-133">Individuare la **sezione** Gestisci nel menu e quindi selezionare **Utenti.**</span><span class="sxs-lookup"><span data-stu-id="5f422-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu con l'opzione Utenti evidenziata.":::

4. <span data-ttu-id="5f422-135">Nella pagina Utenti digitare il nome dell'utente nella casella di ricerca.</span><span class="sxs-lookup"><span data-stu-id="5f422-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra la pagina Utenti con la casella di ricerca per cercare un utente specifico.":::

5. <span data-ttu-id="5f422-137">Selezionare il nome dell'utente in cui viene visualizzato nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="5f422-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra la pagina Utente che visualizza una riga per l'utente cercato.":::

6. <span data-ttu-id="5f422-139">Individuare la sezione Identità nella pagina Profilo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5f422-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="5f422-140">Il campo ID oggetto viene visualizzato qui con l'ID oggetto univoco dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5f422-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra la pagina Profilo utente con la sezione Identità e un campo evidenziato per ID oggetto.":::

## <a name="next-steps"></a><span data-ttu-id="5f422-142">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="5f422-142">Next steps</span></span>

- [<span data-ttu-id="5f422-143">Trovare l'ID tenant a livello di codice con PowerShell o l'interfaccia della riga di comando</span><span class="sxs-lookup"><span data-stu-id="5f422-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="5f422-144">Altre informazioni sui profili utente in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5f422-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="5f422-145">Informazioni su come i partner possono visualizzare o esportare i dettagli dei clienti in Partner Center</span><span class="sxs-lookup"><span data-stu-id="5f422-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

