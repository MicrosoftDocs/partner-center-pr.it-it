---
title: File di riconciliazione dell'utilizzo con classificazione giornaliera | Centro per i partner
ms.topic: article
ms.date: 01/14/2020
description: Informazioni su come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera nel centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a9c7f328cf1a10b4a23aeb775524d5931bdbb703
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021721"
---
# <a name="daily-rated-usage-reconciliation-files"></a>File di riconciliazione dell'utilizzo con classificazione giornaliera

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Agente di vendita
- Agente help desk

In questo argomento viene illustrato come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campi nei file di riconciliazione dell'utilizzo con classificazione giornaliera

| Column | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore partner in formato GUID. |
| PartnerName | Nome partner. |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. |
| CustomerName | Nome dell'organizzazione del cliente registrato nel Centro per i partner. *Questa colonna è molto importante per riconciliare la fattura con le informazioni del sistema.* |
| CustomerDomainName | Nome di dominio del cliente. |
| CustomerCountry | Paese in cui si trova il cliente. |
| MpnId | Identificatore MPN del partner CSP. |
| Tier2MpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. |
| InvoiceNumber | Numero di fattura in cui viene visualizzata la transazione specificata. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per un particolare SKU. |
| AvailabilityId | Identificatore della disponibilità di uno SKU specifico. Ciò indica se lo SKU è disponibile per l'acquisto in un determinato paese, valuta, segmento di settore e così via. |
| SkuName | Titolo di una particolare SKU. |
| ProductName | Nome del prodotto. |
| PublisherName | Nome dell'editore. |
| PublisherId | Identificatore del server di pubblicazione in formato GUID. |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Si tratta di un campo identico a **offername**. |
| SubscriptionId | Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Non utilizzato per la riconciliazione. *Questo identificatore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione (eccetto quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo di fatturazione precedente). L'ora indicata è sempre l'inizio della giornata, le 0:00. |
| ChargeEndDate | Data di fine del ciclo di fatturazione (tranne quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo biling precedente). L'ora indicata è sempre la fine della giornata, le 23:59. |
| UsageDate | Data di utilizzo del servizio. |
| MeterType | Tipo di misuratore. |
| MeterCategory | Servizio di primo livello per l'utilizzo. |
| MeterId | Identificatore del contatore utilizzato. |
| MeterSubCategory | Tipo di servizio di Azure, che può influire sulla frequenza. |
| MeterName | Unità di misura per il contatore utilizzato. |
| MeterRegion | Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato. |
| Unit | Unità del **nome**della risorsa. |
| ResourceLocation | Il data center in cui è in esecuzione il contatore. |
| ConsumedService | Il servizio della piattaforma Azure che è stato utilizzato. |
| ResourceGroup | Rappresenta un contenitore che include le risorse correlate per una soluzione di Azure. |
| ResourceURI | URI della risorsa in uso. |
| ChargeType | Tipo di addebito o rettifica.  |
| UnitPrice | Prezzo per licenza, pubblicato nell'elenco prezzi al momento dell'acquisto. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| Quantità | Numero di licenze. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| UnitType | Tipo di unità in cui viene addebitato il contatore.  |
| BillingPreTaxTotal | Importo totale della fatturazione prima delle imposte. |
| BillingCurrency | Valuta nell'area geografica del cliente. |
| PricingPreTaxTotal | I prezzi prima dell'aggiunta delle imposte. |
| PricingCurrency | Valuta nell'elenco prezzi. |
| ServiceInfo1 | Numero di connessioni del bus di servizio di cui è stato effettuato il provisioning e utilizzate in un determinato giorno. |
| ServiceInfo2 | Campo legacy che acquisisce i metadati facoltativi specifici del servizio. |
| Tag | Rappresenta un'organizzazione logica delle risorse di Azure impostate dall'utente. |
| AdditionalInfo | Eventuali informazioni aggiuntive non incluse in altre colonne. |
| EffectiveUnitPrice | Il valore effettivo addebitato per unità, inclusi eventuali sconti, crediti ottenuti e così via. |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta di fatturazione ai prezzi. |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. |
| EntitlementId | Rappresenta l'ID sottoscrizione di Azure. |
| EntitlementDescription | Rappresenta il nome dell'ID sottoscrizione di Azure. |
| PartnerEarnedCreditPercentage | Visualizza il PartnerEarnedCredit per l'elemento della riga. Il credito guadagnato sarà 0 o 15% |
