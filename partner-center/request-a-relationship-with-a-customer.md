---
title: Richiedere una relazione come rivenditore con un cliente
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Richiedere una relazione con un cliente per scenari multicanale multi-partner o se è necessario ripristinare i privilegi di amministratore delegato per un cliente.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 83f615e69a9285365e68305fa909104e0da52992
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551640"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Come richiedere una relazione di rivenditore da un cliente nel Centro per i partner

**Ruoli appropriati:** agente di amministrazione | Amministratore globale

Se si vuole gestire il servizio o la sottoscrizione di un cliente per loro conto, il cliente deve concedere all'utente le autorizzazioni di amministratore per tale servizio o sottoscrizione e firmare l'Contratto del cliente Microsoft.

Se si vuole stabilire una relazione come rivenditore con un cliente e gestire solo le sottoscrizioni di Azure di cui si effettua il provisioning, non è necessario ottenere le autorizzazioni di amministratore.

>[!NOTE] 
>L'opzione per non richiedere autorizzazioni non è disponibile per i partner che operano in Microsoft Cloud for US Government o Microsoft Cloud Germania. Per altre informazioni, vedere [Delegare i privilegi di amministrazione ai partner.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire con l'utente una relazione come rivenditore

È possibile richiedere una relazione come rivenditore con un cliente all'interno del proprio paese o della stessa area geografica.

1. Selezionare **Clienti** dal menu **Centro per i partner** e selezionare **Richiedi una relazione come rivenditore**.

2. Per richiedere autorizzazioni di amministratore a questo cliente, selezionare Includi privilegi di amministrazione delegata per Azure Active Directory **e Office 365.** Per stabilire la relazione senza richiedere autorizzazioni di amministratore, deselezionare questa opzione.

3. Nella pagina successiva esaminare la bozza del messaggio di posta elettronica. È possibile aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure è possibile copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica.

   Il testo nel messaggio di posta elettronica può essere modificato, ma è necessario assicurarsi di includere il collegamento, in quanto personalizzato, per collegare il cliente direttamente al proprio account. Al termine di questo passaggio, seleziona **Fatto**.

4. Inviare il messaggio di posta elettronica al cliente.

5. Dopo che il cliente ha accettato l'invito, verrà visualizzato nella **pagina** Clienti e potrà effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

   > [!NOTE]
   > Se il cliente non ha ancora accettato il Contratto del cliente Microsoft, gli verrà richiesto di farlo quando accetta l'invito. Il cliente deve essere un amministratore globale per accettare l'invito.

6. Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandi il record del cliente selezionando la freccia verso il basso accanto al nome.

> [!IMPORTANT]  
> I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione del servizio. Tuttavia, a meno che e fino a quando non si rinegozia il contratto con il cliente, l'utente continuerà a essere responsabile dell'assistenza clienti e dell'aderenza alle condizioni del Contratto Microsoft Partner, anche dopo che un cliente ha riassegnare o rimuovere le autorizzazioni di amministratore. In questo caso, se il cliente richiede assistenza, è possibile chiamare il supporto tecnico Microsoft per aprire una richiesta di servizio per conto del cliente.

## <a name="changes-to-the-customer-invitation-experience"></a>Modifiche all'esperienza di invito del cliente

L'esperienza del cliente per accettare un invito alla relazione come rivenditore da un partner Cloud Solution Provider (CSP) è ospitata da portali diversi per i clienti. La posizione del portale dipende dal fatto che un cliente si trova in un cloud pubblico Microsoft o in un cloud nazionale:

|Tipi di clienti cloud  | Dove un cliente accetta un invito alla relazione come rivenditore? |
|---------|---------
| Clienti nel cloud pubblico | Interfaccia di amministrazione di Microsoft 365 |
| Clienti in Partner Center per Microsoft Cloud Germania | Microsoft Office di amministrazione |
| Clienti in Partner Center per Microsoft Cloud for US Government | Microsoft Office di amministrazione |
|

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare contatti di supporto](assign-support-contacts.md)

- [Rimuovere una relazione con un cliente](remove-a-relationship.md)
