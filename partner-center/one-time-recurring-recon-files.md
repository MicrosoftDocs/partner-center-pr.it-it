---
title: File di riconciliazione singola e ricorrente
ms.topic: article
ms.date: 05/26/2020
description: Comprendere il significato di ogni campo o colonna nel centro per i partner e riconciliare i file una sola volta.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84bed4fac8984b3fc8757b8185da514c5d8212d6
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749193"
---
# <a name="one-time-and-recurring-reconciliation-files-in-partner-center"></a>File di riconciliazione monouso e ricorrente nel centro per i partner

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Amministratore fatturazione
- Agente amministratore
- Agente di vendita

In questo argomento viene illustrato come leggere i file di riconciliazione monouso e periodici nel centro per i partner.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campi in un file di riconciliazione monouso e ricorrente

| Colonna | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore univoco del tenant Azure Active Directory (Azure AD) per un'entità di fatturazione specifica in formato GUID. Non obbligatorio per la riconciliazione. È lo stesso per tutte le righe. |
| CustomerId | Identificatore univoco del tenant Azure AD in formato GUID. Identifica il cliente. |
| CustomerName | Nome dell'organizzazione del cliente, come indicato nel centro per i partner. |
| CustomerDomainName | Nome di dominio del cliente. Questo campo può essere vuoto fino al secondo ciclo di fatturazione. *Non usare questo campo come identificatore univoco per il cliente. Il cliente/partner può aggiornare il dominio Vanity o default tramite il portale di Office 365.* |
| CustomerCountry | Paese in cui si trova il cliente. |
| InvoiceNumber | Numero di fattura in cui è presente la transazione specificata. |
| MpnId | Identificatore MPN del partner CSP. |
| OrderId | Identificatore univoco per un ordine in Microsoft Commerce platform. Non utilizzato per la riconciliazione. |
| OrderDate | Data in cui è stato inserito l'ordine. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per un particolare SKU (unità di supporto). |
| AvailabilityId | Identificatore della disponibilità di uno SKU specifico. Ciò indica se lo SKU è disponibile per l'acquisto in un determinato paese, valuta, segmento di settore e così via. |
| SkuName | Titolo per uno SKU specifico. |
| ProductName | Nome del prodotto. |
| ChargeType | Tipo di addebito o rettifica. |
| UnitPrice | Prezzo unitario pubblicato nell'elenco prezzi al momento dell'acquisto. *Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione.* |
| Quantità | Numero di unità. *Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione.* |
| SubTotal | Totale al lordo delle imposte. Controlla se il subtotale corrisponde al totale previsto, in caso di sconto. |
| TaxTotal | Addebito IVA. In base alle regole fiscali e alle circostanze specifiche del mercato. |
| Totale | Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte. |
| Valuta | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Assicurarsi che corrisponda alla prima fattura e controllare di nuovo dopo gli aggiornamenti principali della piattaforma di fatturazione. |
| PriceAdjustmentDescription | Spiegazione di qualsiasi sconto applicabile. |
| PublisherName | Nome del server di pubblicazione del prodotto.
| PublisherId | Identificatore univoco per un server di pubblicazione specifico. |
| SubscriptionDescription | Nome descrittivo di una sottoscrizione. |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma Microsoft Commerce. Non utilizzato per la riconciliazione. *Questo identificatore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* |
| ChargeStartDate | Giorno di inizio degli addebiti. L'ora è sempre l'inizio del giorno, 0:00. |
| ChargeEndDate | Giorno di fine degli addebiti. L'ora indicata è sempre la fine della giornata, le 23:59. |
| TermAndBillingcycle | Durata e ciclo di fatturazione per l'acquisto (ad esempio, *1 anno, mensile*). |
| EffectiveUnitPrice | Prezzo unitario dopo le rettifiche apportate. |
| UnitType | Tipo di unità da acquistare. |
| AlternateId | Identificatore alternativo a un **ID dell'ordine**. |
| BillableQuantity | Rappresenta le unità totali acquistate o utilizzate. |
| BillingFrequency | Descrive se l'elemento della riga è una frequenza di fatturazione mensile o una volta sola. *Questa operazione è attualmente supportata solo per Azure RI, con i valori supportati come mensili. Se il RI viene acquistato con una frequenza di fatturazione monouso, questo campo nel file di ricognizione verrà visualizzato come vuoto.* |
| PricingCurrency | Il prezzo di listino della risorsa o dell'offerta. |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta di fatturazione ai prezzi. |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. |
| MeterDescription | Descrizione del contatore per l'elemento della riga a consumo. |
