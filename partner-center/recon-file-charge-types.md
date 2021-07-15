---
title: Tipi di addebito dei file di riconciliazione
ms.topic: article
ms.date: 06/05/2020
description: Individuare i tipi di addebiti (ad esempio, basati su licenza, basati sull'utilizzo e una sola volta), crediti e sconti nei file di riconciliazione Partner Center di riconciliazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989775"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Comprendere i diversi tipi di addebito nei Partner Center di riconciliazione

**Si applica a**: Partner Center | Partner Center per Microsoft Cloud for US Government

**Ruoli appropriati:** Agente di amministrazione | Gestione della fatturazione | Amministratore globale

Questo articolo descrive i mapping tra una sezione della fattura e i tipi di addebito associati che potrebbero essere nel file di riconciliazione. La fattura fornisce un riepilogo degli addebiti. Il file di riconciliazione fornisce una suddivisione dettagliata delle transazioni voci, inclusi i tipi di addebito. Per altre informazioni sui file di riconciliazione, vedere [Come usare i file di riconciliazione.](use-the-reconciliation-files.md)

Sia i file di [](license-based-recon-files.md) riconciliazione [basati](usage-based-recon-files.md) sull'utilizzo che i file di riconciliazione basati su licenza mostrano solo le transazioni e gli addebiti correlati all'utilizzo (unità utilizzate e addebiti correlati).

> [!NOTE]
> I crediti, gli sconti o i rimborsi una  sola volta visualizzati nella fattura come Rettifiche non vengono visualizzati nel file di riconciliazione.

## <a name="map-charge-types-to-invoice-charges"></a>Eseguire il mapping dei tipi di addebito agli addebiti delle fatture

Per fare riferimento incrociato agli importi degli addebiti tra la fattura e il file di riconciliazione, usare le opzioni di filtro in Microsoft Excel. Filtrare in base ai tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti della fattura a un set di scomposizione degli addebiti nel file di riconciliazione.

## <a name="license-based-charges"></a>Addebiti basati su licenza

Per eseguire il mapping di questi addebiti basati su licenza alla fattura, sommare la **colonna Amount** dal file basato su licenza.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Commissione di attivazione | Importo addebitato al cliente quando usa la sottoscrizione dopo l'acquisto. |
| Commissione di annullamento | Addebiti con valori prorate rimborsati al cliente quando vengono modificate le licenze associate. |
| Annullare la prorata dell'istanza | Addebiti prorate annullati quando la sottoscrizione del cliente con sottoscrizione mensile viene sospesa e le licenze associate vengono modificate nello stesso mese. |
| Tariffa periodica | Addebiti periodici per una sottoscrizione. |
| Ripartizione dell'istanza del ciclo | Addebiti prorate valutati dal cliente quando vengono modificate le licenze associate. |
| Addebiti con pagamento in prorata in caso di annullamento | Rimborso prorate per la parte inutilizzata del servizio in caso di annullamento. |
| Eseguire la prorata delle tariffe quando si esegue la conversione dall'offerta corrente | Addebiti prorate dopo la conversione dalla sottoscrizione mensile corrente a una sottoscrizione annuale. |
| Eseguire la prorata delle tariffe quando si esegue la conversione in una nuova offerta | Addebiti prorate dopo la conversione di una sottoscrizione mensile in una nuova sottoscrizione annuale. |
| Ripartizione delle tariffe all'acquisto | Tipo di addebito per una sottoscrizione quando si usa la fatturazione mensile o annuale. |
| Tariffa con pagamento in base al rinnovo | Tariffe prorate al rinnovo della sottoscrizione. |
| Rinnovare la tariffa | Addebito per il rinnovo di una sottoscrizione |
| Eseguire la prorata delle tariffe quando si esegue l'attivazione | Addebiti prorate dall'attivazione fino alla fine del periodo di fatturazione. |

## <a name="one-time-charges"></a>Addebiti una sola volta

Per eseguire il mapping di questi addebiti una sola volta alla fattura, sommare la **colonna Amount** dal file basato su licenza.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Nuovo | Usato quando viene creato un nuovo acquisto. |
| rinnovare | Usato quando una sottoscrizione viene rinnovata dopo la fine del periodo. |
| addQuantity | Usato sia nel rimborso dell'acquisto originale che nella nuova quantità dopo un aumento. |
| removeQuantity | Usato sia nel rimborso dell'acquisto originale che nella nuova quantità dopo una diminuzione. |
| cancelImmediate | Usato quando una sottoscrizione viene annullata. |
| convert | Usato quando una licenza viene aggiornata. |
| customerCredit | Usato quando i crediti (ad esempio Azure, contratto di servizio e così via) vengono dati su una transazione. |

## <a name="usage-charges"></a>Addebiti per utilizzo

Per eseguire il mapping di questi addebiti per l'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Valutare la tariffa di utilizzo in caso di annullamento | Tariffa per l'utilizzo dell'accesso in caso di annullamento per l'utilizzo non pagato durante il periodo di fatturazione corrente. |
| Valutare la tariffa di utilizzo per il ciclo corrente | Tariffa per l'utilizzo dell'accesso per il periodo di fatturazione corrente. |

### <a name="credits"></a>Credits

Per eseguire il mapping di questi crediti alla fattura:

- Sommare **TotalForCustomer** dal file basato su licenza.
- Sommare **la colonna PostTaxTotal** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Offset di un elemento riga | Rimborso parziale o totale per una voce, incluse le imposte. |

### <a name="usage-based-discounts"></a>Sconti basati sull'utilizzo

Per eseguire il mapping di questi sconti basati sull'utilizzo alla fattura, sommare la colonna **PretaxCharges** dal file basato sull'utilizzo.

| Descrizione addebito (colonna ChargeType nel file di riconciliazione) | Spiegazione dell'addebito |
| ------------------------------------------------------------- | ------------------ |
| Sconto per l'attivazione | Sconto applicato all'attivazione della sottoscrizione. |
| Sconto ciclo | Sconto applicato agli addebiti periodici. |
| Rinnovare lo sconto | Sconto applicato al rinnovo della sottoscrizione. |
| Annullare lo sconto | Addebiti applicati quando vengono annullati gli sconti. |

### <a name="license-based-discounts"></a>Sconti basati su licenza

Per eseguire il mapping degli sconti basati su licenza alla fattura, sommare la **colonna TotalOtherDiscount** dal file basato su licenza.

*Gli sconti basati su licenza possono essere applicati a più tipi di addebito.*
