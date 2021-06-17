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
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276940"
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
|  Una | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>I livelli di incentivi Enterprise si basano sul numero di utenti o desktop (a seconda del valore più alto) nelle registrazioni del settore pubblico e commerciale. Per le registrazioni senza desktop o numero di utenti associato naturale, Microsoft applica un numero di desktop in base al numero di desktop o al numero di utenti del relativo EA. <br><br>Se non è presente alcun EA, il livello di tariffa è basato sul livello di prezzo della registrazione. Il livello di prezzo della trattativa può essere visualizzato anche in [www.explore.ms](https://www.explore.ms/). <br><br>Se sono presenti più pool e/o livelli di prezzo per il piano EA/EAS esistente, Microsoft paga gli incentivi al livello di prezzo/pool più alto assegnato, con il livello A che è il più basso e il livello D il più alto.

#### <a name="pool-and-pricing-levels"></a>Livelli di pool e prezzi

Dopo aver cercato il numero di contratto explore.ms usando la procedura descritta in precedenza, selezionare il numero di contratto. Verrà visualizzata la pagina dei dettagli del contratto, che mostrerà Riepilogo **contratto** **e Offerte.** La sezione offerte contiene i livelli di prezzo.

## <a name="method-2---chip"></a>Metodo 2 - CHIP

1. Accedere a CHIP e selezionare Incentivi LSP.

2. Nella pagina **Partner Payment Summary (Riepilogo pagamento** partner) selezionare il mese di report da visualizzare e quindi selezionare Calculation **Details** (Dettagli calcolo) nell'elenco a discesa in Export to **Excel (Esporta in Excel):**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Individuare i dettagli del programma.":::

3. Verrà avviata l'esportazione ed è possibile aprire il file o salvare/salvare con nome in una destinazione.

4. Quando il report è aperto, passare alla scheda **DetailReport-FlatFile** all'estrema sinistra:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download di file flat.":::

È ora possibile cercare il numero di contratto che si sta cercando nella colonna J. Il numero di desktop assegnato è disponibile nella colonna R, con etichetta Agreement_DesktopCount. È anche possibile confermare il livello di tariffa per questo contratto nella colonna "Intelligenza artificiale" con etichetta Livello.

## <a name="next-steps"></a>Passaggi successivi

- [Risolvere i problemi di accesso chip](chip-access-trouble.md)
