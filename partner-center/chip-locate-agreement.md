---
title: Trovare il numero di desktop e il livello di tariffa
ms.topic: how-to
ms.date: 02/18/2021
description: Informazioni su come usare la piattaforma Channel Incentives (CHIP) per trovare le informazioni sul numero di desktop e sul livello di tariffa per un contratto.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148993"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Individuare il numero di desktop e il livello di tariffa per un contratto

**Ruoli appropriati:** contatto principale o amministratore del programma

È possibile accedere al [explore.ms](https://www.explore.ms/) per esaminare il contratto o scaricare un file che fornisce i dettagli del contratto per il numero di desktop e il livello di tariffa.

## <a name="to-locate-the-information"></a>Per individuare le informazioni

### <a name="method-1--explorems"></a>Metodo 1: Explore.ms

1. Aprire [explore.ms](https://www.explore.ms/) in Internet Explorer. 

>[!Note]
>Non è possibile eseguire questa funzione in Google Chrome o Microsoft Edge.

2. Accedere con l'account aziendale o dell'istituto di istruzione o con l'ID live.  

3. Nel campo **Report** selezionare **Contratti.**

4. Nella pagina risultante immettere il numero di contratto nel campo **Cerca** e quindi selezionare **Seleziona/Ordina colonne**.

5. Nella finestra popup selezionare **Agreement Desktop Count** nell'elenco delle colonne disponibili e quindi selezionare la freccia destra per aggiungere la colonna. Selezionare **OK**.

6. Selezionare **Cerca.**

7. Nella schermata risultante scorrere i risultati per trovare la colonna **Agreement Desktop Count (Conteggio desktop** contratto). 

8. Usare il numero di desktop per determinare il livello di tariffa in base alla tabella delle tariffa riportata di seguito.  

| Livello di tariffa | Numero di desktop |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>I livelli di incentivi aziendali si basano sul numero di utenti o desktop (a seconda di quale sia il più alto) nelle registrazioni del settore pubblico e commerciale. Per le registrazioni senza desktop associato naturale o numero di utenti, Microsoft applica un numero di desktop in base al numero di desktop o al numero di utenti dell'EA associato. <br><br>Se non è presente alcun EA, il livello di tariffa è basato sul livello di prezzo della registrazione. Il livello di prezzo dell'offerta può essere visualizzato anche in [www.explore.ms](https://www.explore.ms/). <br><br>Se sono presenti più livelli di pool e/o prezzi nell'EA/EAS esistente, Microsoft paga gli incentivi al livello di prezzo/pool più alto assegnato, con il livello A il più basso e il livello D il più alto.

#### <a name="pool-and-pricing-levels"></a>Pool e livelli di prezzo

Dopo aver cercato il numero di contratto explore.ms la procedura descritta in precedenza, selezionare il numero di contratto. Verrà visualizzata la pagina dei dettagli dell'accordo, che mostra il riepilogo **e** **le offerte dell'accordo.** La sezione offerte contiene i livelli di prezzo.

## <a name="method-2---chip"></a>Metodo 2 - CHIP

1. Accedere a CHIP e selezionare Incentivi LSP.

2. Nella pagina **Riepilogo pagamento partner** selezionare il mese di report da visualizzare e quindi selezionare **Dettagli** calcolo nell'elenco a discesa in Esporta **in Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Individuare i dettagli del programma":::

3. L'esportazione verrà avviata ed è possibile aprire il file o salvare/salvare con nome in una destinazione.

4. Quando il report è aperto, passare alla **scheda DetailReport-FlatFile** all'estrema sinistra:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download di file flat":::

È ora possibile cercare il numero di contratto che si sta cercando nella colonna J. e il numero di desktop assegnato è disponibile nella colonna R, con l'etichetta Agreement_DesktopCount. È anche possibile confermare il livello di tariffa per questo contratto nella colonna "AI" con etichetta Livello.

## <a name="next-steps"></a>Passaggi successivi

- [Risolvere i problemi di accesso chip](chip-access-trouble.md)
