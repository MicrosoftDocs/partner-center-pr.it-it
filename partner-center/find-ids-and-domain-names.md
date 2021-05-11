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
# <a name="locate-important-ids-for-a-user"></a>Individuare GLI ID importanti per un utente

**Ruoli appropriati**

- Amministratore globale

Questo articolo descrive come usare il portale di Azure [per](https://portal.azure.com/) individuare le informazioni seguenti per un utente:

- ID Microsoft Azure Active Directory tenant (Azure AD) dell'organizzazione o della società dell'utente

- Nome di dominio primario dell'organizzazione o della società associata al tenant Azure AD

- ID oggetto utente

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Trovare l'ID Microsoft Azure AD tenant e il nome di dominio primario

Seguire questa procedura per individuare l'ID tenant Azure AD o il nome di dominio primario all'interno del portale di Azure. Se si desidera trovare un ID tenant a livello di codice, vedere Trovare l'ID tenant con PowerShell o l'interfaccia della [riga di comando.](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)

> [!NOTE]
> L'ID tenant può essere chiamato nomi diversi in applicazioni o risorse diverse. Ad esempio, l'ID tenant può essere denominato ID directory, tenant Azure Active Directory (Azure AD), ID Microsoft o per determinati report, anche *tenantguid*.

1. Accedere al [portale di Azure](https://portal.azure.com/).

2. Selezionare **Azure Active Directory** dal menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Mostra portale di Azure l'opzione Azure Active Directory dal menu.":::

3. Verrà Azure Active Directory **pagina Panoramica.** Per trovare l Azure AD'ID tenant o il nome di dominio primario, cercare il campo **ID tenant** e il **campo Dominio** primario. Questi campi vengono visualizzati nella sezione Informazioni sul tenant.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Mostra la pagina Panoramica con due campi evidenziati, l'ID tenant e il nome di dominio primario.":::

4. È possibile trovare l'ID tenant nella portale di Azure in altri modi. Selezionare **Azure Active Directory** dal menu. Individuare quindi la **sezione Gestisci** nel menu e selezionare **Proprietà.**

   Nella pagina Proprietà viene visualizzato anche l'ID tenant associato dell'utente.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Visualizza la pagina Proprietà con il campo ID tenant evidenziato.":::

## <a name="find-the-user-object-id"></a>Trovare l'ID oggetto utente

La semplice ricerca del nome di dominio e dell'ID tenant potrebbe non essere sempre sufficiente. Potrebbe anche essere necessario individuare l'ID oggetto specifico assegnato a un utente. Seguire questa procedura per trovare l'ID oggetto di un utente nella portale di Azure:

1. Accedere al [portale di Azure](https://portal.azure.com/).

2. Selezionare **Azure Active Directory** dal menu.

3. Individuare la **sezione** Gestisci nel menu e quindi selezionare **Utenti**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Mostra Azure Active Directory menu con l'opzione Utenti evidenziata.":::

4. Nella pagina Utenti digitare il nome dell'utente nella casella di ricerca.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Visualizza la pagina Utenti con la casella di ricerca per cercare un utente specifico.":::

5. Selezionare il nome dell'utente in cui viene visualizzato nell'elenco.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Visualizza la pagina Utente che visualizza una riga per l'utente cercato.":::

6. Individuare la sezione Identità nella pagina Profilo dell'utente. Il campo ID oggetto viene visualizzato qui con l'ID oggetto univoco dell'utente.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Mostra la pagina Profilo utente con la sezione Identità e un campo evidenziato per ID oggetto.":::

## <a name="next-steps"></a>Passaggi successivi

- [Trovare l'ID tenant a livello di codice con PowerShell o l'interfaccia della riga di comando](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Altre informazioni sui profili utente in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Informazioni su come i partner possono visualizzare o esportare i dettagli dei clienti in Partner Center](see-your-customer-list.md)

