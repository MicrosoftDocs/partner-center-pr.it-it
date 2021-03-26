---
title: Richiedere una relazione con un cliente
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Richiedere una relazione con un cliente per scenari multicanale e multicanale o se è necessario ripristinare i privilegi amministrativi delegati per un cliente.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 2403ec6cdb2776ab04fa76a37d690a748de38714
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/25/2021
ms.locfileid: "105548972"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Come richiedere una relazione di rivenditore da un cliente nel Centro per i partner

Se si desidera gestire il servizio o la sottoscrizione di un cliente per loro conto, il cliente deve concedere le autorizzazioni di amministratore per tale servizio o sottoscrizione e firmare il contratto per i clienti Microsoft.

Se si vuole stabilire una relazione del rivenditore con un cliente e gestire solo le sottoscrizioni di Azure di cui si esegue il provisioning, non è necessario ottenere le autorizzazioni di amministratore.

>[!NOTE] 
>L'opzione per non richiedere autorizzazioni non è disponibile per i partner che operano in Microsoft Cloud per il governo degli Stati Uniti o per Microsoft Cloud Germania. Per altre informazioni, vedere [i clienti che delegano i privilegi di amministrazione ai partner](customers-revoke-admin-privileges.md).

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitare un cliente a stabilire con l'utente una relazione come rivenditore

È possibile richiedere una relazione del rivenditore con un cliente all'interno del proprio paese o della stessa area.

1. Selezionare **Clienti** dal menu **Centro per i partner** e selezionare **Richiedi una relazione come rivenditore**.

2. Per richiedere le autorizzazioni di amministratore da questo cliente, selezionare **Includi privilegi di amministrazione delegata per Azure Active Directory e Office 365**. Per stabilire la relazione senza richiedere autorizzazioni di amministratore, deselezionare questa opzione.

3. Nella pagina successiva esaminare la bozza del messaggio di posta elettronica. È possibile aprire la bozza del messaggio nell'applicazione di posta elettronica predefinita oppure è possibile copiare il messaggio negli Appunti e incollarlo in un messaggio di posta elettronica.

   Il testo nel messaggio di posta elettronica può essere modificato, ma è necessario assicurarsi di includere il collegamento, in quanto personalizzato, per collegare il cliente direttamente al proprio account. Al termine di questo passaggio, seleziona **Fatto**.

4. Inviare il messaggio di posta elettronica al cliente.

5. Dopo aver accettato l'invito, il cliente verrà visualizzato nella pagina **Clienti** e potrai effettuare il provisioning e gestire il servizio per il cliente da questa pagina.

   > [!NOTE]
   > Se il cliente non ha ancora accettato il contratto per i clienti Microsoft, verrà richiesto di farlo al momento dell'accettazione dell'invito. Il cliente deve essere amministratore globale per accettare l'invito.

6. Per gestire l'account, i servizi, gli utenti e le licenze del cliente, espandi il record del cliente selezionando la freccia verso il basso accanto al nome.

> [!IMPORTANT]  
> I clienti possono riassegnare o rimuovere le autorizzazioni di amministratore nel portale di amministrazione del servizio. Tuttavia, a meno che e fino a quando non si rinegoziano i contratti con il cliente, l'utente continuerà a essere responsabile del supporto tecnico e della conformità alle condizioni del contratto partner Microsoft, anche dopo che un cliente ha riassegnato o rimosso le autorizzazioni di amministratore. In questa situazione, se il cliente richiede assistenza, è possibile contattare il supporto tecnico Microsoft per aprire una richiesta di assistenza per conto del cliente.

## <a name="changes-to-the-customer-invitation-experience"></a>Modifiche all'esperienza di invito dei clienti

L'esperienza del cliente per l'accettazione di un invito alle relazioni rivenditore da un partner Cloud Solution Provider è ospitata da portali diversi per i clienti. Il percorso del portale dipende dal fatto che un cliente si trovi in un cloud pubblico Microsoft o in un cloud nazionale:

|Tipi di clienti cloud  | Dove un cliente accetta un invito alla relazione Reseller? |
|---------|---------
| Clienti nel cloud pubblico | Interfaccia di amministrazione di Microsoft 365 |
| Clienti nel centro per i partner per Microsoft Cloud Germania | Portale di amministrazione di Microsoft Office |
| Clienti nel centro per i partner per Microsoft Cloud per il governo degli Stati Uniti | Portale di amministrazione di Microsoft Office |
|

## <a name="next-steps"></a>Passaggi successivi

- [Assegnare contatti di supporto](assign-support-contacts.md)

- [Rimuovere una relazione con un cliente](remove-a-relationship.md)
