---
title: Trova il numero di desktop e il livello di tariffa
ms.topic: how-to
ms.date: 02/18/2021
description: Informazioni su come usare il CHIP (Channel incentives Platform) per trovare il numero di desktop e le informazioni sul livello di tariffa per un contratto.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756118"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Individuare il numero di desktop e il livello di tariffa per un contratto

**Ruoli appropriati**

- Contatto principale o amministratore del programma

È possibile accedere a [explore.ms](https://www.explore.ms/) per esaminare il contratto oppure scaricare un file contenente i dettagli del contratto per il numero di desktop e il livello di tariffa.

## <a name="to-locate-the-information"></a>Per individuare le informazioni

### <a name="method-1--explorems"></a>Metodo 1 – Explore.ms

1. Aprire [explore.ms](https://www.explore.ms/) in Internet Explorer. 

>[!Note]
>Non è possibile eseguire questa funzione in Google Chrome o Microsoft Edge.

2. Accedere con l'account aziendale o dell'Istituto di istruzione o con Live ID.  

3. Nel campo **report** selezionare **contratti**.

4. Nella pagina risultante immettere il numero del contratto nel campo di **ricerca** , quindi selezionare **Seleziona/Ordina colonne**.

5. Nella finestra popup selezionare **Agreement desktop count** nell'elenco colonne disponibili, quindi selezionare la freccia destra per aggiungere la colonna. Selezionare **OK**.

6. Selezionare **Cerca.**

7. Nella schermata risultante scorrere i risultati per trovare la colonna contratto di **conteggio desktop** . 

8. Usare il numero di desktop per determinare il livello di tariffa in base alla tabella dei tassi riportata di seguito.  

| Livello tariffa | Conteggio desktop |
| ------ | :-----------: |
|  A | 0 – 2.399    |
|  B | 2.400 – 5.999    |
|  C | 6.000 – 14.999    |
|  D | 15.000 +   |

>[!NOTE]
>I livelli di incentivi aziendali si basano sul numero di computer desktop o utenti (a seconda del valore più elevato) nelle registrazioni di settore commerciale e pubblico (PS). Per le registrazioni senza un numero di utenti o desktop associato naturale, Microsoft applica un numero di desktop basato sul numero di desktop o sul numero di utenti dell'EA di accompagnamento. <br><br>Se non è presente alcuna EA associata, il livello di tariffa si basa sul livello di prezzo della registrazione. Il piano tariffario dell'affare può anche essere visualizzato in [www.explore.ms](https://www.explore.ms/). <br><br>Se sono presenti più pool e/o livelli di prezzo per il contratto Enterprise/EAS esistente, Microsoft addebiterà gli incentivi al livello di prezzo/pool più elevato assegnato, con un livello che corrisponde al livello più basso e il livello D.

#### <a name="pool-and-pricing-levels"></a>Pool e livelli di prezzo

Dopo aver cercato il numero di contratto in explore.ms usando la procedura descritta in precedenza, selezionare il numero di contratto. Verrà visualizzata la pagina dei dettagli del contratto, che mostra il riepilogo e le **offerte** del **contratto** . La sezione offerte contiene i piani tariffari.

## <a name="method-2---chip"></a>Metodo 2-CHIP

1. Accedere a CHIP e selezionare gli incentivi per LSP.

2. Nella pagina **Riepilogo pagamenti partner** selezionare il mese per la creazione di report che si desidera visualizzare, quindi selezionare i **Dettagli di calcolo** nell'elenco a discesa in **Esporta in Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Individuare i dettagli del programma":::

3. L'esportazione viene avviata ed è possibile aprire il file o salvarlo o salvarlo in una destinazione.

4. Quando il report è aperto, passare alla scheda **DetailReport-Flatfile** all'estremità inferiore sinistra:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download file flat":::

È ora possibile cercare il numero di contratto che si sta cercando nella colonna J. il numero di desktop assegnati è disponibile nella colonna R, denominato Agreement_DesktopCount. È anche possibile verificare il livello di tariffa per il contratto nel livello con etichetta "AI" della colonna.

## <a name="next-steps"></a>Passaggi successivi

- [Risolvere i problemi di accesso al CHIP](chip-access-trouble.md)
