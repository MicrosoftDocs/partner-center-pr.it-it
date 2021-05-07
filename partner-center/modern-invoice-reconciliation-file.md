---
title: Campi di riconciliare i file per gli acquisti una sola volta CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Informazioni su tutti gli elementi nel file di riconciliazione dell'acquisto unico CSP in Partner Center, inclusi i valori di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 559b5334eb23ad76fe8cc51fc1beeaa3a86c6fa1
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702791"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campi del file di riconciliazione degli acquisti una sola volta CSP

**Ruoli appropriati**

- Amministratore degli account
- Agente di fatturazione

## <a name="using-the-recon-file"></a>Uso del file di ricognizione
La tabella seguente fornisce descrizioni e valori di esempio per i campi nel file di riconciliazione per gli acquisti una sola volta CSP.

Per altre informazioni sui file di riconciliazione, vedere [Usare i file di riconciliazione](use-the-reconciliation-files.md).

| Colonna | Descrizione | Valore di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore univoco in formato GUID per un'entità di fatturazione specifica. Non obbligatorio per la riconciliazione. È lo stesso per tutte le righe. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome dell'organizzazione del cliente come indicato nel Centro per i partner. Questa colonna è importante per riconcilare la fattura con le informazioni di sistema. | *John Modern Cust DE2* |
| CustomerDomainName | Nome di dominio del cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Paese in cui si trova il cliente. Vedere [l'elenco completo dei paesi per](./regional-authorization-overview.md) la propria area geografica.  | *De* |
| InvoiceNumber | Numero di fattura associato al file di riconciliazione.  | *G002297372* |
| MpnId | Identificatore MPN del partner CSP. Per altre informazioni, vedere [come ottenere informazioni dettagliate in base al partner.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. | *6048879* |
| OrderId | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare l'ordine quando si contatta il supporto tecnico. Non usato per la riconciliazione. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Data in formato UTC in cui è stato inserito l'ordine. | *10/3/2020* |
| ProductId | Identificatore univoco del prodotto. | *DZH318Z0BNZ5* |
| SkuId | Identificatore univoco dello SKU. | *006G* |
| Id disponibilità | Identificatore univoco della disponibilità. | *DZH318Z08B80* |
| SkuName | Nome dello SKU. | *Tabelle - LRS* |
| ProductName | Nome del prodotto. | *Tabelle* |
| ChargeType | Tipo [di addebito o](./recon-file-charge-types.md) rettifica. | *Nuovo* |
| UnitPrice | Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *0.045* |
| Quantity | Numero di licenze. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *1* |
| Subtotale | Totale al lordo delle imposte. Il subtotale deve essere uguale alla quantità fatturabile moltiplicata per il prezzo unitario effettivo. | *0* |
| TaxTotal | Addebito dell'importo dell'imposta. In base alle regole fiscali del mercato e a circostanze specifiche. | *0* |
| Totale | L'importo totale è uguale al subtotale più l'importo dell'imposta. | *0* |
| Valuta | La fattura viene generata nel contesto della valuta del cliente. Questo significa che se sei un partner che opera con i clienti da valute fatturabili diverse, riceverai una fattura per ogni tipo di valuta del cliente.  | *EUR* |
| PriceAdjustmentDescription | Motivi delle rettifiche nel prezzo unitario. Questi sono i motivi principali, ma non solo per determinare il prezzo unitario effettivo. | *["15,0% Credito ottenuto dal partner per i servizi gestiti"]* |
| PublisherName | Editore del prodotto.  | *Microsoft* |
| PublisherId | Identificatore univoco utilizzato Partner Center per identificare il server di pubblicazione. | *N/D* |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questa colonna è un campo identico a OfferName. | *Piano di Azure* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Non usato per la riconciliazione. Si noti che questo identificatore non corrisponde all'ID sottoscrizione nella console di amministrazione partner. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Data di inizio del periodo di fatturazione di una sottoscrizione. | *9/1/2020* |
| ChargeEndDate | Data di fine del periodo di fatturazione di una sottoscrizione. | *30/09/2020* |
| TermAndBillingCycle | L'impegno di durata per continuare la sottoscrizione al momento dell'acquisto. | *Dati archiviati (GB/mese)* |
| EffectiveUnitPrice | Prezzo unitario rifisso per calcolare il costo per il ciclo di fatturazione. Gli sconti, le rettifiche nei giorni di fatturazione e altri fattori determinano il prezzo unitario effettivo. Per altre informazioni, vedere [Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| Tipo di unità | Tipo di unità in cui viene addebitato il contatore. | *1 GB/mese* |
| AlternateId | ID alternativo della voce dell'ordine di riferimento. | *6dc5c039750a* |
| BillableQuantity | Quantità totale fatturata.  | *0.005001* |
| FatturazioneFrequency | Piano di fatturazione selezionato al momento dell'acquisto. | *N/D*  |
| PricingCurrency | La valuta usata nell'elenco prezzi. | *USD* |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta dei prezzi alla valuta di fatturazione. | *0.846202666* |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. | *30/09/2020* |
| MeterDescription | Descrizione del contatore.  | *Tabelle - Dati LRS archiviati (GB/mese)* |
| ReservationOrderId | ID ordine di prenotazione. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Descrizione del credito. | *Credito a consumo di Azure* |

>[!NOTE]
>È possibile riconciliare il consumo di Azure nel file di ricognizione di acquisto una sola volta. A tale scopo, passare al file di ricognizione sull'utilizzo giornaliero e cercare subscriptionID. Verranno visualizzati tutti i costi associati all'ID piano di Azure. L'ID sottoscrizione di Azure viene visualizzato come EntitlementID.

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione e imposte](billing.md)
