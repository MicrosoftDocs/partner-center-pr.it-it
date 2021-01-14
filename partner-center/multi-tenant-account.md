---
title: Aggiungere altri tenant all'account del centro per i partner
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant di Azure AD nell'account del centro per i partner. Altre informazioni su alcuni dei motivi per cui si potrebbe voler eseguire questa operazione.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182435"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Aggiungere e gestire più tenant nell'account del centro per i partner


**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

Questa funzionalità consente all'utente di gestire più tenant per la propria azienda e di consolidarli nell'account del Centro per i partner. Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner. Ad esempio:

- L'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner. Tuttavia, si vuole che le due società rimangano separate. In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PGA). Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.

- Se si dispone di più tenant per l'esecuzione dell'attività, ad esempio contoso.com, contoso.uk, contoso.in, è possibile usare il multi-tenant per collegarli con lo stesso account del computer.

- Per le fusioni e le acquisizioni è necessario usare più di un tenant (ad esempio, se contoso acquisisce Fabrikam, è necessario poter usare sia Constoso.com che Fabrikam.com rispettivi tenant).

- È necessario che gli utenti di uno dei tenant siano in grado di:
    1.  Accedi al centro per i partner per corsi di formazione, download digitali, associazione MCP
    2.  Sono assegnati ruoli del centro per i partner, ad esempio MPN admin, incentives admin e così via.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Aggiungere un altro tenant Azure AD all'account

1. Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.
1. Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associa tenant"::: 

3. Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.

1. Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="conferma associazione tenant"::: 

5. Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .  Selezionare **Torna a gestione tenant per** visualizzare il tenant appena aggiunto. 
 

>[!NOTE]
>Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.


## <a name="remove-a-tenant-from-your-account"></a>Rimuovere un tenant dall'account
 
1. Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.

1. Nell'icona **Impostazioni** selezionare **impostazioni account** -> tenant e fare clic sulla scheda **partner** .
 
3. Fare clic su **Rimuovi** per il tenant a cui si desidera eseguire l'associazione.

4. L'annullamento dell'associazione di un tenant implica che gli utenti di tale tenant non avranno più accesso all'account del centro per i partner e questo potrebbe avere un effetto sulle competenze. 

Il pulsante **Rimuovi** è abilitato per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi.

:::image type="content" source="images/disassociate.png" alt-text="tenant con il pulsante Rimuovi":::
 

## <a name="next-steps"></a>Passaggi successivi

- [Aggiungere utenti](create-user-accounts-and-set-permissions.md)






