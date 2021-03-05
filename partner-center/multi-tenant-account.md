---
title: Aggiungere i tenant all'account del centro per i partner
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant di Azure AD nell'account del centro per i partner e per informazioni sul motivo per cui è possibile eseguire questa operazione.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124806"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Aggiungere e gestire più tenant nell'account del centro per i partner


**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

Questo articolo illustra come consolidare più tenant di Azure Active Directory (Azure AD) per la società e quindi aggiungerli e gestirli nell'account del centro per i partner. Esistono diversi motivi per eseguire questa operazione. Ad esempio:

- Supponiamo che l'azienda, contoso, abbia acquisito un'altra società, fabrikam. Si vuole che le due società rimangano separate, ma si vuole che i nuovi dipendenti siano in grado di usare il centro per i partner. In questo caso, associare il tenant Azure AD della nuova società con l'account globale del partner (PGA). Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.

- Se si esegue l'attività aziendale con più di un tenant, ad esempio *contoso.com*, *contoso.uk* e *contoso.in*, è possibile usare la multitenant per raggrupparli nello stesso account PC.

- Se le linee guida per fusioni e acquisizioni richiedono l'uso di tenant di entrambe le società, si useranno entrambi i tenant *constoso.com* e *Fabrikam.com* .

- Gli utenti di qualsiasi tenant devono poter:
    * Accedi al centro per i partner per corsi di formazione, download digitali o associazione Microsoft Certified Professional (MCP).
    * Sono assegnati ruoli del centro per i partner, ad esempio l'amministratore di Microsoft Partner Network (MPN) o gli incentivi.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Aggiungere un tenant di Azure AD all'account

1. Accedere come amministratore globale al centro per i [partner Microsoft](https://partner.microsoft.com/dashboard).

1. In alto a destra selezionare **Impostazioni**, selezionare **Impostazioni account**, quindi selezionare **tenant**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot del pulsante associa nel riquadro del profilo Azure AD."::: 

1. Selezionare **associa** e quindi indicare il tenant che si vuole associare.

1. Al prompt accedere come amministratore globale al tenant che si vuole associare, quindi selezionare **Confirm (conferma**). 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot del pulsante conferma del riquadro Conferma nuova associazione Azure AD."::: 

   Una volta confermata l'associazione, viene visualizzato un messaggio di **tutti i set** . Per visualizzare il tenant appena aggiunto, selezionare **Torna a gestione tenant**. 
 
>[!NOTE]
>Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.


## <a name="remove-a-tenant-from-your-account"></a>Rimuovere un tenant dall'account
 
1. Accedere come amministratore globale al centro per i [partner Microsoft](https://partner.microsoft.com/dashboard).

1. In alto a destra, selezionare l'icona **delle impostazioni** e quindi selezionare **Impostazioni account**.

1. Nel riquadro sinistro selezionare **tenant**. In **gestisci Azure ad tenant** selezionare la scheda **partner** .
 
1. Selezionare **Rimuovi** accanto al tenant di cui si vuole rimuovere l'associazione.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot delle associazioni del tenant corrente e dei relativi collegamenti di rimozione.":::

   Come illustrato nella schermata precedente, i collegamenti di **rimozione** sono abilitati per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi. 

   > [!NOTE]   
   > Quando si rimuove un tenant, gli utenti del tenant non hanno più accesso all'account del centro per i partner e la rimozione potrebbe avere un effetto sulle competenze. 

## <a name="next-steps"></a>Passaggi successivi

- [Creare account utente](create-user-accounts-and-set-permissions.md)






