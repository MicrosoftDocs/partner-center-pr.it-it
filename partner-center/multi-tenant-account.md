---
title: Aggiungere altri tenant all'account del centro per i partner
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gestire più tenant tramite l'account del centro per i partner
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389516"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Aggiungere e gestire più tenant nell'account del centro per i partner

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner. Ad esempio, l'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner. Tuttavia, si vuole che le due società rimangano separate. In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PNG). Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.

## <a name="add-another-azure-ad-tenant-to-your-account"></a>Aggiungere un altro tenant Azure AD all'account

1. Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.
1. Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="associa tenant"::: 

3. Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.

1. Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione. 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="conferma associazione tenant"::: 

5. Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .  Selezionare **Torna a gestione tenant per** visualizzare l'elenco dei tenant appena aggiunti.
 
## <a name="next-steps"></a>Passaggi successivi

- [Aggiungere utenti](create-user-accounts-and-set-permissions.md)
