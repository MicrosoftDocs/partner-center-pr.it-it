---
title: Visualizza i dettagli relativi a incentivi e programmi
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Usare queste pagine per visualizzare e gestire lo stato del programma incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4c4b3a9a71027f5fb02bc29566c20c214e3df371
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022809"
---
# <a name="view-your-incentives-program-details"></a>Visualizza i dettagli del programma incentives

**Ruoli appropriati**

- Amministratore incentivo
- Utente incentive
- Amministratore globale
- Amministratore partner MPN

Questo articolo illustra la pagina **Panoramica dei miei incentivi** , che mostra lo stato complessivo dei programmi di incentivazione, nonché lo stato di ogni programma in ogni sede. Fornisce inoltre i diversi Stati di registrazione.

>[!NOTE]
>Per ulteriori informazioni sugli incentivi e sulle funzionalità di incentivazione del centro per i partner, vedere [investimenti e incentivi](https://partner.microsoft.com/membership/partner-incentives) per i partner (accesso richiesto).

## <a name="access-the-incentives-overview-page"></a>Accedere alla pagina Panoramica degli incentivi

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).
1. Selezionare **incentivi**, quindi **Panoramica** dal menu.
1. Visualizzare il riepilogo dei guadagni e dei pagamenti nella parte superiore della pagina e ulteriori dettagli nella tabella riportata di seguito. È anche possibile ordinare, raggruppare ed espandere la tabella associata:

   - Per eseguire l'ordinamento in base alla colonna, selezionare il nome della colonna.
   - Per raggruppare in base al programma, selezionare la scheda **in base al programma** sopra la tabella.
   - Per raggruppare in base alla posizione, selezionare la scheda **per località** sopra la tabella.
   - Per visualizzare altri dettagli sulle registrazioni in un gruppo specifico, selezionare il simbolo della freccia di espansione alla fine di una determinata riga. Questa freccia di espansione espande la visualizzazione.
1. Se è necessaria un'ulteriore azione per la registrazione in un programma, queste informazioni verranno visualizzate nella colonna **Stato**. In questo caso, selezionare il simbolo della freccia di espansione per ottenere informazioni sui passaggi successivi da eseguire.

## <a name="enrollment-status"></a>Stato della registrazione

La tabella seguente illustra i diversi Stati di registrazione indicati nella colonna **stato** .

| **Status**         | **Viene visualizzato quando** |
|:------------------------------------|:------------------|
| Azione richiesta  | Il partner ha accettato un invito a iscriversi a un programma di incentivi, ma potrebbe dover aggiornare le informazioni bancarie o fiscali. Vedere la colonna **azioni necessarie** per i passaggi successivi o i collegamenti per aggiornare le informazioni bancarie o fiscali nel centro per i partner. |
| Non disponibile  | Il programma di incentivazione specifico non è più disponibile nel sistema di incentivi. |
| Enrolled  | Tutte le informazioni fiscali e bancarie sono state convalidate. Non è richiesta alcuna ulteriore azione di registrazione da parte del partner. |
| Enrolling  | L'utente non è un amministratore di incentivi e la registrazione è nell' **azione necessaria** o per la **convalida** degli Stati di registrazione.|
| Inattivo/non idoneo | Il programma incentive potrebbe non essere aperto per la registrazione in questo momento o il partner non soddisfa l'idoneità corrente per la registrazione o la nuova registrazione. <br><br> Se lo stato non è **idoneo**, il partner non soddisfa i requisiti di idoneità correnti per il programma; Se si seleziona il collegamento **vedere i requisiti di idoneità** sotto lo stato di registrazione, vengono visualizzati i requisiti per l'idoneità e quali di questi requisiti sono stati soddisfatti. <br><br> È anche possibile che vengano visualizzate le registrazioni stato **inattivo** per l'organizzazione virtuale (VORG) o partner Global account (PGA) che non sono più attive nel programma incentive.  |
| Invitato  | Un nuovo invito alla registrazione del programma incentive è stato inviato al partner, ma il partner non ha ancora avviato il processo di registrazione. La colonna adiacente, **azioni richieste** Mostra i passaggi successivi ed eventuali collegamenti correlati.  |
| Convalida della registrazione  | Il partner ha già completato o aggiornato le informazioni fiscali e bancarie per una registrazione nuova o esistente ed è in attesa della convalida delle informazioni da parte di Microsoft. Durante il processo di convalida, è possibile che venga visualizzata la **convalida della registrazione** per un massimo di 48 ore.  |

## <a name="see-your-payment-information"></a>Visualizza le informazioni di pagamento

Selezionare l'icona del payout nell'angolo superiore destro della schermata per accedere a questi riepiloghi diversi:

- Cronologia delle transazioni
- Pagamenti
- Esportazione dei dati

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Viene illustrata l'icona del payout nell'angolo superiore destro del portale del centro per i partner":::

Queste informazioni includono i guadagni e i pagamenti per gli incentivi totali, dal momento dell'iscrizione ai relativi programmi. In questa pagina sono inclusi anche i guadagni e i pagamenti per posizione o programma, nonché eventuali altre azioni da intraprendere per eseguire la registrazione in un programma in una posizione specifica. 

È anche possibile usare l' [API](https://apidocs.microsoft.com/services/partnerpayouts) per i pagamenti dei partner per connettersi e ottenere direttamente i dati relativi a transazioni e pagamenti dei pagamenti. Per ulteriori informazioni, vedere le istruzioni relative ai [pagamenti](payout-statement.md) .

## <a name="next-steps"></a>Passaggi successivi

- [Estratti conto](payout-statement.md)
