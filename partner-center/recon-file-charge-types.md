---
title: Tipi di addebito file di riconciliazione
ms.topic: article
ms.date: 06/05/2020
description: Individuare i tipi di addebiti (ad esempio, basati su licenza, utilizzo e una volta), crediti e sconti nei file di riconciliazione del centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7a5c227748ba24001288ecbec0a5487d38033897
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467511"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Informazioni sui diversi tipi di addebito nei file di riconciliazione del centro per i partner

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale

In questo argomento vengono descritti i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere presenti nel file di riconciliazione. La fattura fornisce un riepilogo degli addebiti. Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di elementi riga, inclusi i tipi di addebito. Per ulteriori informazioni sui file di riconciliazione, vedere [come utilizzare i file di riconciliazione](use-the-reconciliation-files.md).

Sia [i file di riconciliazione basati sull'utilizzo](usage-based-recon-files.md) che [i file di riconciliazione basati sulle licenze](license-based-recon-files.md) mostrano solo le transazioni e gli addebiti relativi all'utilizzo (unità utilizzate e addebiti correlati).

> [!NOTE]
> I crediti, gli sconti o i rimborsi unidirezionali visualizzati nella fattura come **modifiche** non vengono visualizzati nel file di riconciliazione.

## <a name="map-charge-types-to-invoice-charges"></a>Mappare i tipi di addebito ai costi fattura

Per fare riferimento incrociato agli importi tra la fattura e il file di riconciliazione, utilizzare le opzioni di filtro in Microsoft Excel. Filtrare in base ai tipi di addebito sul file di riconciliazione per eseguire il mapping degli addebiti per la fattura a un set di suddivisione dei costi nel file di riconciliazione

## <a name="license-based-charges"></a>Addebiti basati su licenza

Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la colonna **Amount** del file basato su licenze.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Commissione di attivazione | Importo addebitato al cliente quando utilizza la sottoscrizione dopo l'acquisto. |
| Commissione di annullamento | Addebiti rivalutati per il cliente quando vengono modificate le postazioni associate. |
| Annulla profrequenza istanza | Addebiti rivalutati annullati quando al cliente con sottoscrizione mensile è stata sospesa la sottoscrizione e le postazioni associate sono state modificate nello stesso mese |
| Tariffa periodica | Addebiti periodici per una sottoscrizione. |
| Ripartizione dell'istanza del ciclo | Addebiti rivalutati dal cliente quando vengono modificate le postazioni associate. |
| Tariffe propagate quando si annulla | Rimborso proporzionale per la parte di servizio inutilizzata al momento dell'annullamento. |
| Tariffe propagate quando si esegue la conversione a partire dall'offerta corrente | Addebiti rivalutati dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale. |
| Tariffe della propagazione durante la conversione in una nuova offerta | Addebiti rivalutati dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale. |
| Ripartizione delle tariffe all'acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione annuale. |
| Tariffa di acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile. |
| Tariffa della propagazione al rinnovo | Tariffe riordinate al rinnovo della sottoscrizione. |
| Tassa di rinnovo | Addebito per il rinnovo di una sottoscrizione |
| Tariffe propagate all'attivazione | Tariffe rivalutate dall'attivazione fino alla fine del periodo di fatturazione. |

## <a name="one-time-charges"></a>Addebiti monouso

Per eseguire il mapping di questi addebiti monouso alla fattura, sommare la colonna **Amount** del file basato su licenze.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Nuovo | Utilizzato quando viene creato un nuovo acquisto. |
| addQuantity | Usato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo un aumento. |
| removeQuantity | Utilizzato sia per il rimborso dell'acquisto originale che per la nuova quantità dopo una riduzione. |
| Annulla | Utilizzato quando viene annullata una sottoscrizione. |
| Conversione | Usato quando viene aggiornata una licenza, ma il numero di postazioni rimane invariato. |

## <a name="usage-charges"></a>Addebiti per utilizzo

Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Valutazione della tariffa di utilizzo quando viene annullata | Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente. |
| Valutazione della tariffa di utilizzo per il ciclo corrente | Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente. |

### <a name="credits"></a>Credits

Per eseguire il mapping di questi crediti alla fattura:

- Sommare il **TotalForCustomer** dal file basato sulle licenze.
- Sommare la colonna **PostTaxTotal** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Offset di un elemento linea | Rimborso parziale o totale per una voce, incluse le imposte. |

### <a name="usage-based-discounts"></a>Sconti basati sull'utilizzo

Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione di addebito |
| ------------------------------------------------------------- | ------------------ |
| Sconto attivazione | Sconto applicato quando la sottoscrizione è stata attivata. |
| Sconto del ciclo | Sconto applicato agli addebiti periodici. |
| Sconto rinnovo | Sconto applicato quando la sottoscrizione è stata rinnovata. |
| Annulla sconto | Addebiti applicati quando vengono annullati gli sconti. |

### <a name="license-based-discounts"></a>Sconti basati su licenza

Per eseguire il mapping degli sconti basati sulle licenze alla fattura, sommare la colonna **TotalOtherDiscount** del file basato su licenza.

*Gli sconti basati sulle licenze possono essere applicati a più tipi di addebito.*
