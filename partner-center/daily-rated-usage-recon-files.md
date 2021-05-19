---
title: File di riconciliazione dell'utilizzo con frequenza giornaliera
ms.topic: article
ms.date: 06/12/2020
description: Informazioni su come leggere i file di riconciliazione dell'utilizzo con frequenza giornaliera in Partner Center. Include descrizioni per campi specifici nel file di ricognizione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147276"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Informazioni su come leggere i file di riconciliazione dell'utilizzo con frequenza giornaliera in Partner Center

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** Agente di amministrazione | Gestione della fatturazione | Agente di vendita | Agente del supporto

Questo articolo illustra come leggere i file di riconciliazione dell'utilizzo con frequenza giornaliera.

>[!NOTE]
>L'utilizzo con frequenza giornaliera richiede in genere 24 ore per essere visualizzato Partner Center o per l'accesso tramite l'API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campi nei file di riconciliazione dell'utilizzo con frequenza giornaliera

| Colonna | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore del partner in formato GUID. |
| PartnerName | Nome partner. |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. |
| CustomerName | Nome dell'organizzazione del cliente come indicato nel Centro per i partner. *Questa colonna è importante per riconcilare la fattura con le informazioni di sistema.* |
| CustomerDomainName | Nome di dominio del cliente. |
| CustomerCountry | Paese in cui si trova il cliente. |
| MpnId | Identificatore MPN del partner CSP. |
| Tier2MpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. |
| InvoiceNumber | Numero di fattura in cui è presente la transazione specificata. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per uno SKU specifico. |
| AvailabilityId | Identificatore per la disponibilità di uno SKU specifico. Questa colonna indica se lo SKU è disponibile per l'acquisto nel paese, nella valuta, nel segmento di settore e così via. |
| SkuName | Titolo per uno SKU specifico. |
| ProductName | Nome del prodotto. |
| PublisherName | Nome del server di pubblicazione. |
| PublisherId | Identificatore del server di pubblicazione in formato GUID. |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questa colonna è un campo identico a **OfferName**. |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Non usato per la riconciliazione. *Questo identificatore non corrisponde **all'ID** sottoscrizione nella console di amministrazione partner.* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione(tranne quando si presentano le date dei dati di utilizzo latenti non ricaricati in precedenza dal ciclo di fatturazione precedente). L'ora è sempre l'inizio del giorno, 0:00. |
| ChargeEndDate | Data di fine del ciclo di fatturazione(tranne quando si presentano le date dei dati di utilizzo latenti non ricaricati in precedenza dal ciclo di fatturazione precedente). L'ora indicata è sempre la fine della giornata, le 23:59. |
| UsageDate | Data di utilizzo del servizio. |
| MeterType | Tipo di contatore. |
| MeterCategory | Il servizio di primo livello per l'utilizzo. |
| MeterId | Identificatore del contatore in uso. |
| MeterSubCategory | Tipo di servizio di Azure, che può influire sulla frequenza. |
| MeterName | Unità di misura per il contatore utilizzato. |
| MeterRegion | Questa colonna identifica la posizione di un data center all'interno dell'area per i servizi in cui MeterRegion è applicabile e popolato. |
| Unità | Unità della risorsa **Nome**. |
| ResourceLocation | Oggetto data center in cui è in esecuzione il contatore. |
| ConsumedService | Il servizio della piattaforma Azure che è stato utilizzato. |
| ResourceGroup | Rappresenta un contenitore che contiene le risorse correlate per una soluzione di Azure. |
| ResourceURI | URI della risorsa in uso. |
| ChargeType | Tipo di addebito o rettifica.  |
| UnitPrice | Prezzo per licenza, come pubblicato nel listino prezzi al momento dell'acquisto. Assicurarsi che questo prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| Quantity | Numero di licenze. Assicurarsi che questo prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| UnitType | Tipo di unità a cui viene addebitato il contatore.  |
| FatturazionePreTaxTotal | Importo totale della fatturazione prima delle imposte.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Valuta nell'area geografica del cliente. |
| PricingPreTaxTotal | I prezzi, prima dell'aggiunta delle imposte. |
| PricingCurrency | La valuta usata nell'elenco prezzi. |
| ServiceInfo1 | Numero di connessioni del bus di servizio di cui è stato effettuato il provisioning e usate in un determinato giorno. |
| ServiceInfo2 | Campo legacy che acquisisce metadati facoltativi specifici del servizio. |
| Tag | Rappresenta un'organizzazione logica delle risorse di Azure impostate dall'utente. |
| AdditionalInfo | Eventuali informazioni aggiuntive non incluse in altre colonne. |
| EffectiveUnitPrice | Valore effettivo addebitato per unità, inclusi eventuali sconti, credito ottenuto e così via. |
| PCToBCExchangeRate | Tasso di cambio applicato per la valuta dei prezzi alla valuta di fatturazione. |
| PCToBCExchangeRateDate | Data in cui viene determinata la valuta dei prezzi per la valuta di fatturazione. |
| EntitlementId | Rappresenta l'ID sottoscrizione di Azure. |
| EntitlementDescription | Rappresenta il nome dell'ID sottoscrizione di Azure. |
| PartnerEarnedCreditPercentage | Visualizza PartnerEarnedCredit per la voce. Il credito ottenuto sarà 0 o 15% |
| CreditPercentage | Visualizza il credito per il consumo di Azure. Il credito ottenuto sarà 0 o 100%. |
| CreditType | Tipo di credito. Ad esempio, **Credito Azure applicato.** |
>[!NOTE]
>L'utilizzo giornaliero valutato richiede in genere 24 ore per essere visualizzato Partner Center o per essere accessibile tramite l'API.


