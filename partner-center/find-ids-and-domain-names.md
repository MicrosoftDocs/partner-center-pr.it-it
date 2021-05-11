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
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740285"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="5aa7a-104">Individuare GLI ID importanti per un utente</span><span class="sxs-lookup"><span data-stu-id="5aa7a-104">Locate important IDs for a user</span></span>

<span data-ttu-id="5aa7a-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="5aa7a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5aa7a-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="5aa7a-106">Global admin</span></span>

<span data-ttu-id="5aa7a-107">Questo articolo descrive come usare il portale di Azure [per](https://portal.azure.com/) individuare le informazioni seguenti per un utente:</span><span class="sxs-lookup"><span data-stu-id="5aa7a-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="5aa7a-108">ID Microsoft Azure Active Directory tenant (Azure AD) dell'organizzazione o della società dell'utente</span><span class="sxs-lookup"><span data-stu-id="5aa7a-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="5aa7a-109">Nome di dominio primario dell'organizzazione o della società associata al tenant Azure AD</span><span class="sxs-lookup"><span data-stu-id="5aa7a-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="5aa7a-110">ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="5aa7a-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="5aa7a-111">Trovare l'ID Microsoft Azure AD tenant e il nome di dominio primario</span><span class="sxs-lookup"><span data-stu-id="5aa7a-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="5aa7a-112">Seguire questa procedura per individuare l'ID tenant Azure AD o il nome di dominio primario all'interno del portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="5aa7a-113">Se si desidera trovare un ID tenant a livello di codice, vedere Trovare l'ID tenant con PowerShell o l'interfaccia della [riga di comando.](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="5aa7a-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="5aa7a-114">L'ID tenant può essere chiamato nomi diversi in applicazioni o risorse diverse.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="5aa7a-115">Ad esempio, l'ID tenant può essere denominato ID directory, tenant Azure Active Directory (Azure AD), ID Microsoft o per determinati report, anche *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="5aa7a-116">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5aa7a-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5aa7a-117">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portale di Azure l'opzione Azure Active Directory dal menu.":::

3. <span data-ttu-id="5aa7a-119">Verrà Azure Active Directory **pagina Panoramica.**</span><span class="sxs-lookup"><span data-stu-id="5aa7a-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="5aa7a-120">Per trovare l Azure AD'ID tenant o il nome di dominio primario, cercare il campo **ID tenant** e il **campo Dominio** primario.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="5aa7a-121">Questi campi vengono visualizzati nella sezione Informazioni sul tenant.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra la pagina Panoramica con due campi evidenziati, l'ID tenant e il nome di dominio primario.":::

4. <span data-ttu-id="5aa7a-123">È possibile trovare l'ID tenant nella portale di Azure in altri modi.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="5aa7a-124">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="5aa7a-125">Individuare quindi la **sezione Gestisci** nel menu e selezionare **Proprietà.**</span><span class="sxs-lookup"><span data-stu-id="5aa7a-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="5aa7a-126">Nella pagina Proprietà viene visualizzato anche l'ID tenant associato dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visualizza la pagina Proprietà con il campo ID tenant evidenziato.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="5aa7a-128">Trovare l'ID oggetto utente</span><span class="sxs-lookup"><span data-stu-id="5aa7a-128">Find the user object ID</span></span>

<span data-ttu-id="5aa7a-129">La semplice ricerca del nome di dominio e dell'ID tenant potrebbe non essere sempre sufficiente.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="5aa7a-130">Potrebbe anche essere necessario individuare l'ID oggetto specifico assegnato a un utente.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="5aa7a-131">Seguire questa procedura per trovare l'ID oggetto di un utente nella portale di Azure:</span><span class="sxs-lookup"><span data-stu-id="5aa7a-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="5aa7a-132">Accedere al [portale di Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5aa7a-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5aa7a-133">Selezionare **Azure Active Directory** dal menu.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="5aa7a-134">Individuare la **sezione** Gestisci nel menu e quindi selezionare **Utenti**.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu con l'opzione Utenti evidenziata.":::

4. <span data-ttu-id="5aa7a-136">Nella pagina Utenti digitare il nome dell'utente nella casella di ricerca.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visualizza la pagina Utenti con la casella di ricerca per cercare un utente specifico.":::

5. <span data-ttu-id="5aa7a-138">Selezionare il nome dell'utente in cui viene visualizzato nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visualizza la pagina Utente che visualizza una riga per l'utente cercato.":::

6. <span data-ttu-id="5aa7a-140">Individuare la sezione Identità nella pagina Profilo dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="5aa7a-141">Il campo ID oggetto viene visualizzato qui con l'ID oggetto univoco dell'utente.</span><span class="sxs-lookup"><span data-stu-id="5aa7a-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra la pagina Profilo utente con la sezione Identità e un campo evidenziato per ID oggetto.":::

## <a name="next-steps"></a><span data-ttu-id="5aa7a-143">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="5aa7a-143">Next steps</span></span>

- [<span data-ttu-id="5aa7a-144">Trovare l'ID tenant a livello di codice con PowerShell o l'interfaccia della riga di comando</span><span class="sxs-lookup"><span data-stu-id="5aa7a-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="5aa7a-145">Altre informazioni sui profili utente in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5aa7a-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="5aa7a-146">Informazioni su come i partner possono visualizzare o esportare i dettagli dei clienti in Partner Center</span><span class="sxs-lookup"><span data-stu-id="5aa7a-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

