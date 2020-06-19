---
title: Come leggere il file di fatturazione & Recon
ms.topic: article
ms.date: 06/05/2020
description: Informazioni sulla fattura & i file di riconciliazione. La fattura Mostra i costi del centro per i partner per il programma, i prodotti e i clienti per tale periodo mensile.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: fatturazione della sottoscrizione, fatturazione, fatturazione nel centro per i partner, fatturazione del centro per i partner, lettura fattura, fattura, fattura del centro partner, fattura CSP, dove è la fattura?
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df330ce2e66cf198ce97919c02a15eb7a50f6486
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991880"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Comprendere la fattura e il file di riconciliazione: informazioni su come trovarli nel centro per i partner

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale
- Amministratore fatturazione
- Agente amministratore


La **fattura** è un **Riepilogo di tutti gli addebiti** per il centro per i partner (attraverso il programma, tutti i prodotti e tutti i clienti). 

## <a name="invoice-types"></a>Tipi di fattura

Microsoft emetterà una fattura per tutti gli addebiti basati sulle licenze, ad esempio Office 365, e gli addebiti basati sull'utilizzo (ad esempio Azure) e una fattura separata per gli addebiti monouso, ad esempio Azure RI, Marketplace o piano di Azure.

Ad esempio,  

**Scenario 1 [singola valuta]**: il partner ha acquistato l'offerta 145P e le licenze O365  

- Il partner otterrà un PDF di fattura e 2 file di riconciliazione che coprono gli addebiti sia per O365 che per Azure (145P).  

**Scenario 2 [singola valuta]**: il partner dispone di acquisti per Azure ri, Marketplace e/o piano di Azure insieme agli acquisti 145P.

- Il partner otterrà una fattura PDF e un file di riconciliazione che copre gli addebiti per Azure (145P). 

- Il partner riceverà un'altra fattura PDF e un file di riconciliazione che copre i relativi addebiti per Azure RI, Marketplace, Azure Plan. 

**Scenario 3 [più valute]**: il partner ha acquistato per Azure ri in DKK e piano di Azure in EUR insieme agli acquisti di 145P in EUR.

- Il partner riceverà una fattura PDF e un file di riconciliazione che copre gli addebiti per Azure RI in DKK. 

- Il partner riceverà una fattura PDF e un file di riconciliazione che copre gli addebiti per il piano di Azure in EUR. 

- Il partner riceverà un'altra fattura PDF e un file di riconciliazione che copre gli addebiti per l'offerta 145P in EUR (o valuta fatturazione partner). 

## <a name="find-your-bill"></a>Trovare una fattura 

È possibile trovare la fattura nella pagina fatturazione del dashboard nel centro per i partner. In questa pagina è anche possibile trovare la cronologia di fatturazione, le tendenze di spesa e i file di riconciliazione. 

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/home) Centro per i partner. 

2. Nel menu a sinistra selezionare **fatturazione**. 

3. Nella pagina fatturazione selezionare la fattura che si desidera scaricare. 

È possibile trovare un collegamento alla fattura più recente nella parte superiore della pagina in saldo account come data ultima fattura. 

È possibile trovare le fatture precedenti nella sezione cronologia di fatturazione. Scegliere l'anno appropriato, quindi selezionare la freccia a discesa accanto al periodo di fatturazione appropriato. Selezionare il collegamento accanto a fatture (. pdf) per scaricare la fattura del periodo. 

## <a name="understanding-invoice-pdf"></a>Informazioni sulla fattura PDF 

**Fatture per i costi di utilizzo e di licenza**: le fatture per i servizi quali Office 365 e Azure saranno disponibili entro due (2) giorni dalla data di fatturazione selezionata [UTC].  

**Fatture per addebiti periodici e periodici: le**fatture per i servizi quali Azure ri, piano di Azure e Marketplace saranno disponibili non più di 8 di ogni mese.  

Di seguito sono riportati alcuni dei campi chiave nel documento di fattura PDF:

**Numero fattura**: identificatore univoco per il documento di fattura generato per il rispettivo periodo di fatturazione. 

**Periodo di fatturazione**: si tratta del periodo di tempo durante il quale sono disponibili servizi basati su licenze e utilizzi. 

**Data fattura**: data di fatturazione o data di anniversario in cui la fattura viene generata ogni mese. 

Scadenza **pagamento**: data in cui deve essere ricevuto il pagamento. 

**Addebiti**: importo dovuto alla valuta di fatturazione per il rispettivo periodo di fatturazione. 

**Crediti**: crediti, ad esempio SLA, o rettifiche per le modifiche apportate alle sottoscrizioni (ad esempio, aumenti o riduzioni della postazione). 

**Istruzioni**per il pagamento: Descrizione di come pagare la fattura in base all'area geografica. Quando si effettua un pagamento, assicurarsi sempre di includere il numero di fattura. 

Per una descrizione dettagliata di tutti i campi nel file di fattura (inclusi i campi per gli addebiti monouso), vedere [campi del file di fattura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Informazioni sui file di riconciliazione

 I file di riconciliazione, che forniscono dettagli relativi a drill-down/dettagliati degli addebiti, sono disponibili per il download insieme al PDF della fattura. I file di riconciliazione includono gli identificatori dei clienti e gli identificatori di sottoscrizione che è possibile usare per creare fatture del cliente. Per altre informazioni sui file di ricognizione, vedere  [come usare i file di riconciliazione](use-the-reconciliation-files.md) . 
