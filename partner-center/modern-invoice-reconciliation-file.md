---
title: Campi del file di riconciliare per gli acquisti CSP una sola volta
ms.topic: conceptual
ms.date: 01/29/2021
description: Informazioni su tutti gli elementi nel file di riconciliazione dell'acquisto unico CSP in Partner Center, inclusi i valori di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 7ff320124230ec8e0b3505b1c1dbbb7c811cb67f
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120717"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campi del file di riconciliazione dell'acquisto unico CSP

**Ruoli appropriati**

- Amministratore degli account
- Agente di fatturazione

## <a name="using-the-recon-file"></a>Uso del file di ricognizione
La tabella seguente fornisce descrizioni e valori di esempio per i campi nel file di riconciliazione per gli acquisti una sola volta CSP.

Per altre informazioni sui file di riconciliazione, vedere [Usare i file di riconciliazione.](use-the-reconciliation-files.md)

| Colonna | Descrizione | Valore di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore univoco in formato GUID per un'entità di fatturazione specifica. Non necessario per la riconciliazione. È lo stesso per tutte le righe. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificatore Univoco Microsoft per il cliente in formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nome dell'organizzazione del cliente come indicato nel Centro per i partner. Questa colonna è importante per riconcilare la fattura con le informazioni di sistema. | *Johnny Modern Cust DE2* |
| NomeDominioUtente | Nome di dominio del cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Paese in cui si trova il cliente. Vedere [l'elenco completo dei paesi](./regional-authorization-overview.md) per la propria area geografica.  | *De* |
| InvoiceNumber | Numero di fattura associato al file di riconciliazione.  | *G002297372* |
| MpnId | Identificatore MPN del partner CSP. Per altre informazioni, vedere [come visualizzare informazioni dettagliate in base al partner.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. | *6048879* |
| OrderId | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile identificare l'ordine quando si contatta il supporto tecnico. Non usato per la riconciliazione. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Data in cui è stato inserito l'ordine. | *10/3/2020* |
| ProductId | Identificatore univoco del prodotto. | *DZH318Z0BNZ5* |
| SkuId | Identificatore univoco dello SKU. | *006G* |
| AvailabilityId | Identificatore univoco della disponibilità. | *DZH318Z08B80* |
| SkuName | Nome dello SKU. | *Tabelle - LRS* |
| ProductName | Nome del prodotto. | *Tabelle* |
| ChargeType | Tipo [di addebito o](./recon-file-charge-types.md) rettifica. | *Nuovo* |
| UnitPrice | Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto. Assicurarsi che corrispondano alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *0.045* |
| Quantity | Numero di licenze. Assicurarsi che corrispondano alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *1* |
| Subtotale | Totale al lordo delle imposte. Il subtotale deve essere uguale alla quantità fatturabile moltiplicata per il prezzo unitario effettivo. | *0* |
| TaxTotal | Addebito dell'importo dell'imposta. In base alle regole fiscali del mercato e a circostanze specifiche. | *0* |
| Totale | L'importo totale è uguale al subtotale più l'importo dell'imposta. | *0* |
| Valuta | La fattura viene generata nel contesto della valuta del cliente. Questo significa che se sei un partner che opera con i clienti da valute fatturabili diverse, riceverai una fattura per ogni tipo di valuta del cliente.  | *EUR* |
| PriceAdjustmentDescription | Motivi delle rettifiche nel prezzo unitario. Questi sono i motivi principali, ma non solo per determinare il prezzo unitario effettivo. | *["15,0% credito ottenuto dal partner per i servizi gestiti"]* |
| PublisherName | Editore del prodotto.  | *Microsoft* |
| PublisherId | Identificatore univoco utilizzato Partner Center per identificare il server di pubblicazione. | *N/D* |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questa colonna è un campo identico a OfferName. | *Piano di Azure* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Non usato per la riconciliazione. Si noti che questo identificatore non corrisponde all'ID sottoscrizione nella console di amministrazione partner. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Data di inizio del periodo di fatturazione di una sottoscrizione. | *9/1/2020* |
| ChargeEndDate | Data di fine del periodo di fatturazione di una sottoscrizione. | *30/09/2020* |
| TermAndBillingCycle | Impegno di durata per continuare la sottoscrizione al momento dell'acquisto. | *Dati archiviati (GB/mese)* |
| EffectiveUnitPrice | Prezzo unitario prorate per calcolare il costo per il ciclo di fatturazione. Sconti, rettifiche nei giorni di fatturazione e altri fattori determinano il prezzo unitario effettivo. Per altre informazioni, vedere [Calcolo del prezzo unitario effettivo](./effective-unit-price-calculation.md).  | *0.03825* |
| UnitType | Tipo di unità in cui viene addebitato il contatore. | *1 GB/mese* |
| AlternateId | ID alternativo della voce dell'ordine di riferimento. | *6dc5c039750a* |
| BillableQuantity | Quantità totale fatturata.  | *0.005001* |
| FatturazioneFrequenza | Piano di fatturazione selezionato al momento dell'acquisto. | *N/D*  |
| PricingCurrency | La valuta usata nell'elenco prezzi. | *USD* |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta dei prezzi alla valuta di fatturazione. | *0.846202666* |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. | *30/09/2020* |
| MeterDescription | Descrizione del contatore.  | *Tabelle - Dati archiviati per l'archiviazione con accesso in lettura (GB/mese)* |
| ReservationOrderId | ID dell'ordine di prenotazione. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Descrizione del credito. | *Credito per il consumo di Azure* |

>[!NOTE]
>È possibile riconciliare il consumo di Azure nel file di riconciliazione di acquisto una sola volta. A tale scopo, passare al file di ricognizione sull'utilizzo con valutazione giornaliera e cercare SubscriptionID. Verranno visualizzati tutti i costi associati all'ID piano di Azure. L'ID sottoscrizione di Azure viene visualizzato come EntitlementID.

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione e imposte](billing.md)
