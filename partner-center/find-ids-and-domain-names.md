---
title: Trovare l'ID tenant, il nome di dominio, l'ID oggetto utente
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come trovare gli ID nell'portale di Azure, ovvero l'ID tenant, il nome di dominio o l'ID oggetto utente specifico di un'organizzazione Azure AD. Per alcune attività sono necessarie queste informazioni.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360072"
---
# <a name="locate-important-ids-for-a-user"></a>Individuare gli ID importanti per un utente

Questo articolo descrive come usare la [portale di Azure](https://portal.azure.com/) per individuare le informazioni seguenti per un utente:

- ID tenant di Microsoft Azure Active Directory (Azure AD) dell'organizzazione o dell'azienda dell'utente

- Nome di dominio primario dell'organizzazione o della società associata al tenant di Azure AD

- ID oggetto utente

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Trovare l'ID tenant Microsoft Azure AD e il nome di dominio primario

Seguire questa procedura per individuare l'ID tenant Azure AD o il nome di dominio primario all'interno del portale di Azure. Se si vuole trovare un ID tenant a livello di codice, vedere [trovare l'ID tenant con PowerShell o l'interfaccia](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)della riga di comando.

> [!NOTE]
> L'ID tenant può essere chiamato nomi diversi in applicazioni o risorse diverse. Ad esempio, l'ID tenant può essere indicato come ID directory, il tenant Azure Active Directory (Azure AD), l'ID Microsoft o per determinati report, anche *tenantguid*.

1. Accedere al [portale di Azure](https://portal.azure.com/).

2. Selezionare **Azure Active Directory** dal menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portale di Azure selezionando l'opzione Azure Active Directory dal menu.":::

3. Viene visualizzata una pagina di **panoramica** Azure Active Directory. Per trovare l'ID tenant Azure AD o il nome di dominio primario, cercare il campo **ID tenant** e il campo **dominio primario** . Questi campi vengono visualizzati nella sezione informazioni sul tenant.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra la pagina di panoramica con due campi evidenziati, l'ID tenant e il nome di dominio primario.":::

4. È possibile trovare l'ID tenant nel portale di Azure in altri modi. Selezionare **Azure Active Directory** dal menu. Individuare quindi la sezione **Gestisci** del menu e selezionare **Proprietà**.

   La pagina delle proprietà Visualizza anche l'ID tenant associato dell'utente.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Mostra la pagina delle proprietà con il campo ID tenant evidenziato.":::

## <a name="find-the-user-object-id"></a>Trovare l'ID oggetto utente

Solo la ricerca del nome di dominio e dell'ID tenant potrebbe non essere sempre sufficiente. Potrebbe anche essere necessario trovare l'ID oggetto specifico assegnato a un utente. Attenersi alla procedura seguente per trovare l'ID oggetto di un utente nel portale di Azure:

1. Accedere al [portale di Azure](https://portal.azure.com/).

2. Selezionare **Azure Active Directory** dal menu.

3. Individuare la sezione **Gestisci** del menu, quindi selezionare **utenti**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu con l'opzione evidenziata, utenti.":::

4. Nella pagina utenti digitare il nome dell'utente nella casella di ricerca.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Mostra la pagina utenti con la casella di ricerca per cercare un utente specifico.":::

5. Selezionare il nome dell'utente in cui viene visualizzato nell'elenco.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Mostra la pagina utente che visualizza una riga per l'utente cercato.":::

6. Individuare la sezione Identity nella pagina del profilo dell'utente. Il campo ID oggetto viene visualizzato con l'ID oggetto univoco dell'utente.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra la pagina del profilo utente con la sezione Identity e un campo evidenziato per l'ID oggetto.":::

## <a name="next-steps"></a>Passaggi successivi

- [Trovare l'ID tenant a livello di codice con PowerShell o l'interfaccia della riga di comando](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Altre informazioni sui profili utente in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Scopri in che modo i partner possono visualizzare o esportare i dettagli dei clienti nel centro per i partner](see-your-customer-list.md)
