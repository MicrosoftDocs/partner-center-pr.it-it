---
title: Aggiungere tenant all'account Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant Azure AD nell'account Partner Center e sui motivi per cui è consigliabile farlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151203"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Aggiungere e gestire più tenant nell'account Partner Center


**Ruoli appropriati:** amministratore globale | Amministratore account

Questo articolo illustra come consolidare più tenant Azure Active Directory (Azure AD) per l'azienda e quindi aggiungerli e gestirli nell'account Partner Center aziendale. Esistono molti motivi per farlo. Esempio:

- Si supponiamo che l'azienda Contoso abbia acquisito un'altra società, Fabrikam. Si vuole che le due società rimangano separate, ma si vuole che i nuovi dipendenti possano usare Partner Center. In questo caso, si associa il tenant del Azure AD aziendale all'account globale del partner. Questa associazione consente agli utenti di entrambe le società di lavorare in Partner Center.

- Se si esegue l'azienda con più tenant (ad esempio, *contoso.com*, *contoso.uk* e *contoso.in*), è possibile usare la multi-tenant per raggrupparli nello stesso account PC.

- Se le linee guida per fusioni e acquisizioni richiedono l'uso  di tenant di entrambe le società, è necessario usare i tenant constoso.com e *fabrikam.com* tenant.

- Gli utenti di uno dei tenant devono essere in grado di:
    * Accesso Partner Center per il training, i download digitali o l'associazione Microsoft Certified Professional (MCP).
    * Essere assegnati Partner Center ruoli, ad esempio amministratore Microsoft Partner Network (MPN) o amministratore incentivi.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Aggiungere un tenant Azure AD all'account

1. Accedere come amministratore globale a [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. In alto a destra selezionare **Impostazioni,** quindi **Impostazioni account** e infine **Tenant.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot del pulsante Associa nel riquadro Azure AD profilo."::: 

1. Selezionare **Associa** e quindi indicare il tenant da associare.

1. Al prompt accedere come amministratore globale al tenant che si vuole associare e quindi selezionare **Conferma**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot del pulsante Conferma nel riquadro Conferma nuova Azure AD associazione."::: 

   Dopo aver confermato l'associazione, viene visualizzato un messaggio Tutti **i** set. Per visualizzare il tenant appena aggiunto, selezionare **Torna alla gestione del tenant.** 
 
>[!NOTE]
>Non è possibile associare un tenant a un account se è già associato a un altro Partner Center account.


## <a name="remove-a-tenant-from-your-account"></a>Rimuovere un tenant dall'account
 
1. Accedere come amministratore globale a [Microsoft Partner Center](https://partner.microsoft.com/dashboard).

1. In alto a destra selezionare **l'icona Impostazioni** e quindi Selezionare **Impostazioni account**.

1. Nel riquadro sinistro selezionare **Tenant**. In **Gestisci Azure AD tenant** selezionare la scheda **Partner.**
 
1. Selezionare **Rimuovi** accanto al tenant di cui si vuole rimuovere l'associazione.

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot delle associazioni di tenant correnti e dei relativi collegamenti Rimuovi.":::

   Come illustrato nello screenshot precedente, i collegamenti Rimuovi sono abilitati per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi.  

   > [!NOTE]   
   > Quando si rimuove un tenant, gli utenti in tale tenant non hanno più accesso all'account Partner Center e la rimozione potrebbe avere un impatto sulle competenze. 

## <a name="next-steps"></a>Passaggi successivi

- [Creare account utente](create-user-accounts-and-set-permissions.md)






