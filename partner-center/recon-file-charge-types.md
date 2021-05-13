---
title: Tipi di addebito dei file di riconciliazione
ms.topic: article
ms.date: 06/05/2020
description: Individuare i tipi di addebiti (ad esempio, basati su licenza, basati sull'utilizzo e una sola volta), i crediti e gli sconti nei file Partner Center di riconciliazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855880"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Comprendere i diversi tipi di addebito nei Partner Center di riconciliazione

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** agente di amministrazione | Amministratore fatturazione | Amministratore globale

Questo articolo descrive i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere nel file di riconciliazione. La fattura fornisce un riepilogo degli addebiti. Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni di voci, inclusi i tipi di addebito. Per altre informazioni sui file di riconciliazione, vedere [Come usare i file di riconciliazione.](use-the-reconciliation-files.md)

Sia i file di [](license-based-recon-files.md) riconciliazione [basati sull'utilizzo](usage-based-recon-files.md) che i file di riconciliazione basati su licenza mostrano solo le transazioni e gli addebiti correlati all'utilizzo (unità utilizzate e addebiti correlati).

> [!NOTE]
> I crediti, gli sconti o i rimborsi una-off visualizzati nella fattura come Rettifiche non vengono visualizzati nel file di riconciliazione. 

## <a name="map-charge-types-to-invoice-charges"></a>Eseguire il mapping dei tipi di addebito agli addebiti per le fatture

Per fare riferimento incrociato agli importi degli addebiti tra la fattura e il file di riconciliazione, usare le opzioni di filtro in Microsoft Excel. Filtrare in base ai tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti della fattura a un set di scomposizione degli addebiti nel file di riconciliazione.

## <a name="license-based-charges"></a>Addebiti basati su licenza

Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la **colonna Amount** del file basato su licenza.

| Descrizione dell'addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Commissione di attivazione | Importo addebitato al cliente quando usa la sottoscrizione dopo l'acquisto. |
| Commissione di annullamento | Addebiti rirsiorati rimborsati al cliente quando vengono modificate le licenze associate. |
| Annullare il protaso dell'istanza | Addebiti prorate annullati quando la sottoscrizione del cliente con sottoscrizione mensile viene sospesa e le licenze associate vengono modificate nello stesso mese. |
| Tariffa periodica | Addebiti periodici per una sottoscrizione. |
| Ripartizione dell'istanza del ciclo | Addebiti prorate valutati dal cliente quando vengono modificate le licenze associate. |
| Addebiti con pagamento in prorata in caso di annullamento | Rimborso prorate per la parte inutilizzata del servizio in caso di annullamento. |
| Eseguire la prorata delle tariffe quando si esegue la conversione dall'offerta corrente | Addebiti prorate dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale. |
| Eseguire la prorata delle tariffe quando si esegue la conversione in una nuova offerta | Addebiti prorate dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale. |
| Ripartizione delle tariffe all'acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile o annuale. |
| Tariffa prorata al rinnovo | Tariffe prorate al rinnovo della sottoscrizione. |
| Rinnovare la tariffa | Addebito per il rinnovo di una sottoscrizione |
| Eseguire la prorata delle tariffe quando si esegue l'attivazione | Addebiti prorate dall'attivazione fino alla fine del periodo di fatturazione. |

## <a name="one-time-charges"></a>Addebiti una sola volta

Per eseguire il mapping di questi addebiti una sola volta alla fattura, sommare la **colonna Amount** dal file basato su licenza.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Nuova | Usato quando viene creato un nuovo acquisto. |
| addQuantity | Usato sia nel rimborso dell'acquisto originale che nella nuova quantità dopo un aumento. |
| removeQuantity | Usato sia nel rimborso dell'acquisto originale che nella nuova quantità dopo una diminuzione. |
| Annulla | Usato quando una sottoscrizione viene annullata. |
| Conversione | Usato quando una licenza viene aggiornata, ma il numero di licenze rimane invariato. |

## <a name="usage-charges"></a>Addebiti per utilizzo

Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione dell'addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Valutare la tariffa di utilizzo in caso di annullamento | Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente. |
| Valutare la tariffa di utilizzo per il ciclo corrente | Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente. |

### <a name="credits"></a>Credits

Per eseguire il mapping di questi crediti alla fattura:

- Sommare **TotalForCustomer** dal file basato su licenza.
- Sommare **la colonna PostTaxTotal** dal file basato sull'utilizzo.

| Descrizione dell'addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Offset di una voce | Rimborso parziale o totale per una voce, incluse le imposte. |

### <a name="usage-based-discounts"></a>Sconti basati sull'utilizzo

Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione dell'addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Sconto per l'attivazione | Sconto applicato all'attivazione della sottoscrizione. |
| Sconto ciclo | Sconto applicato agli addebiti periodici. |
| Rinnovare lo sconto | Sconto applicato al rinnovo della sottoscrizione. |
| Annullare lo sconto | Addebiti applicati quando vengono annullati gli sconti. |

### <a name="license-based-discounts"></a>Sconti basati su licenza

Per eseguire il mapping degli sconti basati su licenza alla fattura, sommare la **colonna TotalOtherDiscount** dal file basato su licenza.

*Gli sconti basati su licenza possono essere applicati a più tipi di addebito.*
