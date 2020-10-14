---
title: File di riconciliazione dell'utilizzo con classificazione giornaliera
ms.topic: article
ms.date: 06/12/2020
description: Informazioni su come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera nel centro per i partner. Include le descrizioni per campi specifici nel file di ricognizione.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b45ef4767e4bde28befd35c5294ed19149bf034
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031964"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Informazioni su come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera nel centro per i partner

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di vendita
- Agente di supporto tecnico

Questo articolo illustra come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera.

>[!NOTE]
>L'utilizzo giornaliero con classificazione giornaliera richiede 24 ore per essere visualizzato nel centro per i partner o accessibile tramite l'API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campi nei file di riconciliazione dell'utilizzo con classificazione giornaliera

| Colonna | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore partner in formato GUID. |
| PartnerName | Nome partner. |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. |
| CustomerName | Nome dell'organizzazione del cliente come indicato nel Centro per i partner. *Questa colonna è importante per riconciliare la fattura con le informazioni del sistema.* |
| CustomerDomainName | Nome di dominio del cliente. |
| CustomerCountry | Paese in cui si trova il cliente. |
| MpnId | Identificatore MPN del partner CSP. |
| Tier2MpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. |
| InvoiceNumber | Numero di fattura in cui è presente la transazione specificata. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per un particolare SKU. |
| AvailabilityId | Identificatore della disponibilità di uno SKU specifico. In questa colonna viene indicato se lo SKU è disponibile per l'acquisto in un determinato paese, valuta, segmento di settore e così via. |
| SkuName | Titolo per uno SKU specifico. |
| ProductName | Nome del prodotto. |
| PublisherName | Nome del server di pubblicazione. |
| PublisherId | Identificatore del server di pubblicazione in formato GUID. |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questa colonna è un campo identico a **offername**. |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Non utilizzato per la riconciliazione. *Questo identificatore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione (eccetto quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo di fatturazione precedente). L'ora è sempre l'inizio del giorno, 0:00. |
| ChargeEndDate | Data di fine del ciclo di fatturazione (tranne quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo di fatturazione precedente). L'ora indicata è sempre la fine della giornata, le 23:59. |
| UsageDate | Data di utilizzo del servizio. |
| MeterType | Tipo di misuratore. |
| MeterCategory | Il servizio di primo livello per l'utilizzo. |
| MeterId | Identificatore del contatore utilizzato. |
| MeterSubCategory | Tipo di servizio di Azure, che può influire sulla frequenza. |
| MeterName | Unità di misura per il contatore utilizzato. |
| MeterRegion | Questa colonna identifica la posizione di un data center all'interno dell'area per i servizi in cui MeterRegion è applicabile e popolato. |
| Unità | Unità del **nome**della risorsa. |
| ResourceLocation | Il data center in cui è in esecuzione il contatore. |
| ConsumedService | Il servizio della piattaforma Azure che è stato utilizzato. |
| ResourceGroup | Rappresenta un contenitore che include le risorse correlate per una soluzione di Azure. |
| ResourceURI | URI della risorsa in uso. |
| ChargeType | Tipo di addebito o rettifica.  |
| UnitPrice | Prezzo per licenza, pubblicato nell'elenco prezzi al momento dell'acquisto. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| Quantità | Numero di licenze. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| UnitType | Tipo di unità in cui viene addebitato il contatore.  |
| BillingPreTaxTotal | Importo totale della fatturazione prima delle imposte.<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Valuta nell'area geografica del cliente. |
| PricingPreTaxTotal | I prezzi, prima che vengano aggiunte le imposte. |
| PricingCurrency | La valuta usata nell'elenco prezzi. |
| ServiceInfo1 | Numero di connessioni del bus di servizio di cui è stato effettuato il provisioning e che sono state usate in un determinato giorno. |
| ServiceInfo2 | Campo legacy che acquisisce i metadati facoltativi specifici del servizio. |
| Tag | Rappresenta un'organizzazione logica delle risorse di Azure impostate dall'utente. |
| AdditionalInfo | Eventuali informazioni aggiuntive non incluse in altre colonne. |
| EffectiveUnitPrice | Il valore effettivo addebitato per unità, inclusi gli sconti, il credito guadagnato e così via. |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta di fatturazione ai prezzi. |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. |
| EntitlementId | Rappresenta l'ID sottoscrizione di Azure. |
| EntitlementDescription | Rappresenta il nome dell'ID sottoscrizione di Azure. |
| PartnerEarnedCreditPercentage | Visualizza il PartnerEarnedCredit per l'elemento della riga. Il credito guadagnato sarà 0 o 15% |

>[!NOTE]
>L'utilizzo giornaliero con classificazione giornaliera richiede 24 ore per essere visualizzato nel centro per i partner o accessibile tramite l'API.


