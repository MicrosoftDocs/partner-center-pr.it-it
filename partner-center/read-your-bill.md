---
title: Come leggere il file di & fattura
ms.topic: article
ms.date: 06/05/2020
description: Informazioni sulla fattura e sui & di riconciliazione. La fattura mostra Partner Center addebiti per il programma, i prodotti e i clienti per tale periodo mensile.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551198"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Comprendere la fattura e il file di riconciliazione: informazioni su come trovarli in Partner Center


**Ruoli appropriati:** amministratore globale | Amministratore fatturazione | Agente amministratore


La **fattura** è un **riepilogo di tutti gli addebiti Partner Center** cliente (nel programma, tutti i prodotti e tutti i clienti). 

## <a name="find-your-bill-and-reconciliation-file"></a>Trovare la fattura e il file di riconciliazione 

È possibile trovare la fattura nella pagina Fatturazione del dashboard in Partner Center. In questa pagina è anche possibile trovare la cronologia di fatturazione, le tendenze di spesa e i file di riconciliazione. 

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/home) Centro per i partner. 

2. Nel menu a sinistra selezionare **Fatturazione.** 

3. Nella pagina relativa allo stato della fatturazione seleziona una fattura o un file di riconciliazione per visualizzare informazioni più dettagliate. 

È possibile trovare un collegamento alla fattura più recente nella parte superiore della pagina in Saldo dell'account alla data dell'ultima fattura. 

È possibile trovare le fatture precedenti nella sezione Cronologia di fatturazione. Scegliere l'anno appropriato, quindi selezionare la freccia a discesa accanto al periodo di fatturazione appropriato. Selezionare il collegamento accanto a Fatture (.pdf) per scaricare la fattura del periodo. 

## <a name="invoice-types"></a>Tipi di fattura

Microsoft emettere una fattura per gli addebiti basati su licenza (ad esempio Office 365) e gli addebiti in base all'utilizzo (ad esempio Azure) e una fattura separata per gli addebiti una sola volta (ad esempio istanza istanza di Azure, Marketplace o piano di Azure).

Ad esempio,  

**Scenario 1 [Valuta singola]:** il partner ha acquisti per l'offerta 145P e le licenze di Office 365,  

- Il partner riceverà una fattura in formato PDF e due file di riconciliazione che coprono gli addebiti sia per Office 365 che per Azure (145p).  

**Scenario 2 [valuta singola]:** il partner ha acquisti per le istanza istanza singola di Azure, il Marketplace e/o il piano di Azure insieme agli acquisti da 145p.

- Il partner riceverà una fattura in formato PDF e un file di riconciliazione che copre gli addebiti per Azure (145p). 

- Il partner riceverà un altro pdf della fattura e un file di riconciliazione che copre gli addebiti per l'istanza riservata di Azure, il Marketplace e il piano di Azure. 

**Scenario 3 [multi-valuta]:** il partner ha acquisti per l'istanza ri di Azure in DKK e il piano di Azure in EUR, oltre a acquisti di 145p in EUR.

- Il partner riceverà una fattura in formato PDF e un file di riconciliazione che copre gli addebiti per l'istanza ri di Azure in DKK. 

- Il partner riceverà una fattura in formato PDF e un file di riconciliazione che copre gli addebiti per il piano di Azure in EUR. 

- Il partner riceverà un altro PDF della fattura e un file di riconciliazione che copre gli addebiti per un'offerta di 145p in EUR (o valuta di fatturazione del partner). 


## <a name="understanding-invoice-pdf"></a>Informazioni sul PDF della fattura 

**Fatture** per l'utilizzo e gli addebiti basati su licenza: le fatture per gli addebiti per servizi come Office 365 e Azure saranno disponibili entro due (2) giorni dalla data di fatturazione selezionata [UTC].  

**Fatture per addebiti** una volta sola e ricorrenti: le fatture per gli addebiti per servizi come l'istanza di istanza di Azure, il piano di Azure e il Marketplace saranno disponibili non oltre l'ottavo di ogni mese.  

Di seguito sono riportati alcuni dei campi chiave nel documento PDF della fattura:

**Numero di fattura:** identificatore univoco per il documento di fattura generato per il rispettivo periodo di fatturazione. 

**Periodo di fatturazione:** periodo durante il quale si hanno utilizzi e servizi basati su licenza. 

**Data fattura:** data di fatturazione o data dell'anniversario in cui viene generata la fattura ogni mese. 

**Data di scadenza del** pagamento: data entro la quale deve essere ricevuto il pagamento. 

**Addebiti:** importo dovuto nella valuta di fatturazione per il rispettivo periodo di fatturazione. 

**Crediti:** crediti (ad esempio contratto di servizio) o rettifiche per le modifiche apportate alle sottoscrizioni (ad esempio, aumenti o diminuzioni delle licenze). 

**Istruzioni di pagamento:** descrizione di come pagare la fattura, in base all'area. Assicurarsi sempre di includere il numero di fattura quando si effettua un pagamento. 

Per una descrizione dettagliata di tutti i campi nel file della fattura (inclusi i campi per gli addebiti una sola volta), vedere [Campi del file della fattura.](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Comprendere i file di riconciliazione

 I file di riconciliazione, che forniscono un drill-down o dettagli dettagliati degli addebiti, sono disponibili per il download insieme al PDF della fattura. I file di riconciliazione includono gli identificatori dei clienti e gli identificatori di sottoscrizione che è possibile usare per creare le fatture dei clienti. Per altre informazioni sui file di riconciliazione, vedere [Come usare i file di riconciliazione.](use-the-reconciliation-files.md) 

## <a name="next-steps"></a>Passaggi successivi

- [Come usare i file di riconciliazione](use-the-reconciliation-files.md)