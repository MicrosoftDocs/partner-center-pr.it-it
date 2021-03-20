---
title: Campi del file di ricognizione per gli acquisti monouso CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Informazioni su tutti gli elementi nel file di riconciliazione degli acquisti monouso CSP nel centro per i partner, inclusi i valori di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 74974c68c607ddcee4aff6abd53284a60653fb0b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712257"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campi del file di riconciliazione di acquisto monouso CSP

## <a name="using-the-recon-file"></a>Uso del file di ricognizione
La tabella seguente fornisce le descrizioni e i valori di esempio per i campi nel file di riconciliazione per gli acquisti monouso CSP.

Per altre informazioni sui file di riconciliazione, vedere [usare i file di riconciliazione](use-the-reconciliation-files.md).

| Colonna | Descrizione | Valore di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore univoco in formato GUID per un'entità di fatturazione specifica. Non obbligatorio per la riconciliazione. È lo stesso per tutte le righe. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome dell'organizzazione del cliente come indicato nel Centro per i partner. Questa colonna è importante per riconciliare la fattura con le informazioni del sistema. | *Johnny Modern cust DE2* |
| CustomerDomainName | Nome di dominio del cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Il paese in cui si trova il cliente. Vedere l' [elenco completo dei paesi](./regional-authorization-overview.md) per l'area geografica.  | *DE* |
| InvoiceNumber | Numero di fattura associato al file di riconciliazione.  | *G002297372* |
| MpnId | Identificatore MPN del partner CSP. Per ulteriori informazioni, vedere [How to descrivere by partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. | *6048879* |
| OrderId | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare l'ordine quando si contatta il supporto tecnico. Non utilizzato per la riconciliazione. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Data in cui è stato inserito l'ordine. | *10/3/2020* |
| ProductId | Identificatore univoco del prodotto. | *DZH318Z0BNZ5* |
| SkuId | Identificatore univoco dello SKU. | *006G* |
| AvailabilityId | Identificatore univoco di disponibilità. | *DZH318Z08B80* |
| SkuName | Nome dello SKU. | *Tabelle-con ridondanza locale* |
| ProductName | Nome del prodotto. | *Tabelle* |
| ChargeType | [Tipo di addebito](./recon-file-charge-types.md) o regolazione. | *Nuovo* |
| UnitPrice | Prezzo per licenza, pubblicato nell'elenco prezzi al momento dell'acquisto. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *0,045* |
| Quantità | Numero di licenze. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *1* |
| Subtotale | Totale al lordo delle imposte. Il subtotale deve essere uguale alla quantità fatturabile moltiplicata per il prezzo unitario effettivo. | *0* |
| TaxTotal | Addebito IVA. In base alle regole fiscali e alle circostanze specifiche del mercato. | *0* |
| Totale | L'importo totale è uguale al subtotale più l'importo dell'imposta. | *0* |
| Valuta | La fattura viene generata nel contesto della valuta del cliente. Questo significa che se sei un partner che opera con i clienti da valute fatturabili diverse, riceverai una fattura per ogni tipo di valuta del cliente.  | *EUR* |
| PriceAdjustmentDescription | I motivi per le rettifiche nel prezzo unitario. Questi sono i motivi principali, ma non limitati alla determinazione del prezzo unitario effettivo. | *["15,0% del partner ha guadagnato il credito per i servizi gestiti"]* |
| PublisherName | Autore del prodotto.  | *Microsoft* |
| PublisherId | Identificatore univoco utilizzato dal centro per identificare il server di pubblicazione. | *NA* |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questa colonna è un campo identico a Offername. | *Piano di Azure* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Non utilizzato per la riconciliazione. Si noti che questo identificatore non corrisponde all'ID sottoscrizione nella console di amministrazione partner. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Data in cui il centro per i partner addebita il costo della sottoscrizione. Se la sottoscrizione viene acquistata con un periodo di fatturazione annuale e un piano di fatturazione mensile, nel primo file di riconciliazione, questo è il giorno in cui viene acquistata la sottoscrizione. A partire dal successivo file di riconciliazione, verrà incrementato di 30 giorni. | *9/1/2020* |
| ChargeEndDate | Giorno finale degli addebiti per il ciclo di fatturazione della sottoscrizione. Se la sottoscrizione viene acquistata con un periodo di fatturazione annuale e un piano di fatturazione mensile, nel primo file di riconciliazione, questo è il 30 ° giorno dopo l'acquisto della sottoscrizione. A partire dal successivo file di riconciliazione, verrà incrementato di 30 giorni. | *30/09/2020* |
| TermAndBillingCycle | Impegno di durata per continuare la sottoscrizione al momento dell'acquisto. | *Dati archiviati (GB/mese)* |
| EffectiveUnitPrice | Prezzo unitario per calcolare il costo del ciclo di fatturazione. Gli sconti, le rettifiche nei giorni di fatturazione e altri fattori determinano il prezzo unitario effettivo. Per ulteriori informazioni, vedere [calcolo del prezzo unitario effettivo](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Tipo di unità in cui viene addebitato il contatore. | *1 GB/mese* |
| AlternateId | ID alternativo dell'elemento della riga di ordine a cui si fa riferimento. | *6dc5c039750a* |
| BillableQuantity | Quantità totale fatturata.  | *0,005001* |
| BillingFrequency | Piano di fatturazione selezionato al momento dell'acquisto. | *NA*  |
| PricingCurrency | La valuta usata nell'elenco prezzi. | *USD* |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta di fatturazione ai prezzi. | *0,846202666* |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. | *30/09/2020* |
| MeterDescription | Descrizione del contatore.  | *Tabelle-dati con ridondanza locale archiviati (GB/mese)* |
| ReservationOrderId | ID dell'ordine di prenotazione. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Descrizione del credito. | *Credito di consumo di Azure* |

>[!NOTE]
>È possibile riconciliare il consumo di Azure nel file di ricognizione degli acquisti monouso. A tale scopo, passare al file di ricognizione sull'utilizzo giornaliero e cercare il SubscriptionID. Vengono visualizzati tutti i costi associati all'ID piano di Azure. La SubscriptionID di Azure viene visualizzata come EntitlementID.

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione e imposte](billing.md)
