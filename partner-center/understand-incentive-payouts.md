---
title: Visualizzare i dettagli dell'incentivo e del programma
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Usare queste pagine per visualizzare e gestire lo programma Incentivi stato
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818746"
---
# <a name="view-your-incentives-program-details"></a>Visualizzare i dettagli del programma incentivi

**Ruoli appropriati:** incentivi per l'amministratore | Incentivi per gli utenti | Amministratore globale | Amministratore partner MPN

Questo articolo illustra la **pagina di** panoramica degli incentivi, che mostra lo stato complessivo dei programmi di incentivi, nonché lo stato di ogni programma in ogni posizione. Fornisce anche i diversi stati di registrazione.

>[!NOTE]
>Per altre informazioni sulle funzionalità di incentivi e incentivi in Partner Center, vedere Investimenti e incentivi per i [partner](https://partner.microsoft.com/membership/partner-incentives) (è necessario l'accesso).

## <a name="access-the-incentives-overview-page"></a>Accedere alla pagina di panoramica degli incentivi

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).
1. Selezionare **Incentivi** e **quindi Panoramica** dal menu.
1. Visualizzare il riepilogo dei guadagni e dei pagamenti nella parte superiore della pagina e ulteriori dettagli nella tabella riportata di seguito. È anche possibile ordinare, raggruppare ed espandere la tabella che segue:

   - Per ordinare in base alla colonna, selezionare il nome della colonna.
   - Per raggruppare in base al programma, selezionare la **scheda Per** programma sopra la tabella.
   - Per raggruppare in base alla posizione, selezionare **la scheda Per** località sopra la tabella.
   - Per visualizzare informazioni più dettagliate sulle registrazioni all'interno di un gruppo specifico, selezionare il simbolo divron alla fine di una determinata riga. Questa espansione della visualizzazione viene espansa.
1. Se è necessaria un'ulteriore azione per la registrazione in un programma, queste informazioni verranno visualizzate nella colonna **Stato**. In questo caso, selezionare il simbolo della freccia di espansione per ottenere informazioni sui passaggi successivi da eseguire.

## <a name="enrollment-status"></a>Stato della registrazione

Nella tabella seguente vengono illustrati i diversi stati di registrazione visualizzati nella **colonna** Stato .

| **Status**         | **Viene visualizzato quando** |
|:------------------------------------|:------------------|
| Azione richiesta  | Il partner ha accettato un invito a iscriversi a un programma di incentivi, ma potrebbe essere necessario aggiornare le informazioni bancarie o fiscali. Vedere la **colonna Azioni necessarie** per i passaggi successivi o i collegamenti per aggiornare le informazioni bancarie o fiscali in Partner Center. |
| Non disponibile  | Il programma di incentivi specifico non è più disponibile nel sistema di incentivi. |
| Enrolled  | Tutte le informazioni fiscali e bancarie sono state convalidate. Il partner non richiede altre azioni di registrazione. |
| Enrolling  | L'utente non è un amministratore di incentivi e la registrazione è nello stato Azione **richiesta** o **Convalida della** registrazione.|
| Inattivo/Non idoneo | Al momento il programma di incentivi potrebbe non essere aperto alla registrazione o il partner non soddisfa l'idoneità corrente per la registrazione o la nuova registrazione. <br><br> Se lo stato **è Non idoneo,** il partner non soddisfa i requisiti di idoneità correnti per il programma; Selezionando il **collegamento Visualizza i requisiti di** idoneità sotto lo stato della registrazione verranno visualizzati i requisiti per l'idoneità e quali di questi requisiti sono stati soddisfatti. <br><br> È anche possibile che venga visualizzato uno stato **inattivo** per le registrazioni DIG (Virtual Organization) o PGA (Partner Global Account) che non sono più attive nel programma di incentivi.  |
| Invitato  | Un nuovo invito alla registrazione al programma di incentivi è stato inviato al partner, ma il partner non ha ancora avviato il processo di registrazione. La colonna Azioni **necessarie adiacente** mostra i passaggi successivi ed eventuali collegamenti correlati.  |
| Convalida della registrazione  | Il partner ha già completato o aggiornato le informazioni bancarie e fiscali per una registrazione nuova o esistente ed è in attesa che Microsoft convalidi queste informazioni. Durante il processo di convalida, **la convalida della registrazione** può essere visualizzata per un massimo di 48 ore.  |

## <a name="see-your-payment-information"></a>Visualizzare le informazioni di pagamento

Selezionare l'icona dei pagamenti nell'angolo superiore destro della schermata per accedere a questi riepiloghi diversi:

- Cronologia delle transazioni
- Pagamenti
- Esportare i dati

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustra l'icona pagamento nell'angolo superiore destro del portale Partner Center pagamento":::

Queste informazioni includono i guadagni e i pagamenti per gli incentivi totali, dal momento dell'iscrizione ai relativi programmi. In questa pagina sono inclusi anche i guadagni e i pagamenti per posizione o programma, nonché eventuali altre azioni da intraprendere per eseguire la registrazione in un programma in una posizione specifica. 

È anche possibile usare [l'API Partner Payout](https://apidocs.microsoft.com/services/partnerpayouts) per connettersi e ottenere direttamente i dati di transazione e pagamento dei pagamenti. Per [altre informazioni, vedere l'informativa](payout-statement.md) sui pagamenti.

## <a name="next-steps"></a>Passaggi successivi

- [Estratti conto](payout-statement.md)
