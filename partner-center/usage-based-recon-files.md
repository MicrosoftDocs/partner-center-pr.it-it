---
title: File di riconciliazione in base all'uso
ms.topic: article
ms.date: 06/08/2020
description: Informazioni su tutti gli elementi nel file di riconciliazione basato sull'utilizzo in Partner Center. Include alcuni esempi.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431708"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Comprendere i file di riconciliazione basati sull'utilizzo e i relativi campi specifici in Partner Center

**Ruoli appropriati:** amministratore account | Amministratore fatturazione

Per riconciliare gli addebiti con l'utilizzo di un cliente, confrontare **ResellerID**  , **ResellerName** e **ResellerBillableAccount** dal file di riconciliazione con il nome del cliente e **l'ID** sottoscrizione di Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campi nei file di riconciliazione basati sull'utilizzo

I campi seguenti illustrano quali servizi sono stati usati e la tariffa.

| Colonna | Descrizione | Valori di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore partner, in formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nome partner. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificatore dell'account partner. | *1010578050* |
| CustomerCompanyName | Nome dell'organizzazione del cliente, come indicato in Partner Center. *Questo valore è molto importante per riconciliare la fattura con le informazioni di sistema.* | *Cliente di test* |
| MpnId | Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP). | *4390934* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione.  |
| InvoiceNumber | Numero di fattura in cui è presente la transazione specificata. | *D020001IVK* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione, ad eccezione dei casi in cui vengono indicate le date relative a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora è sempre l'inizio del giorno, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data di fine del ciclo di fatturazione, ad eccezione dei casi in cui vengono indicate le date relative a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora indicata è sempre la fine della giornata, le 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando si contatta il supporto tecnico. Non usato per la riconciliazione. *Non corrisponde **all'ID** sottoscrizione nella console di amministrazione partner.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Nome alternativo per l'offerta di servizio. | *Microsoft Azure* |
| SubscriptionDescription | Linea commerciale del servizio offerto. | *Microsoft Azure* |
| OrderID | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando si contatta il supporto tecnico. Non usato per la riconciliazione. | *566890604832738111* |
| ServiceName | Nome del servizio di Azure in questione. | *MACCHINE VIRTUALI* |
| ServiceType | Tipo specifico di servizio di Azure. | *Bus di servizio - Singolo o Pack,* *database SQL di Azure - Business o Web Edition* |
| ResourceGuid | Identificatore univoco specifico per tutti i dati del servizio e la struttura dei prezzi. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| NomeRisorsa | Il nome della risorsa di Azure. | *Trasferimento dei dati in (GB),* *trasferimento dei dati in uscita (GB)* |
| Region | Area a cui si applica l'utilizzo. Usato principalmente per assegnare tariffe ai trasferimenti di dati, perché le tariffe variano in base all'area. | *Asia Pacifico*, *Europa*, *America Latina*, *America del Nord* |
| Sku | Identificatore Microsoft univoco per un'offerta. | *7UD-00001* |
| DetailLineItemId | Identificatore e quantità per visualizzare in modo specifico tariffe diverse per un servizio o una risorsa in un determinato periodo di fatturazione. Per i prezzi a livelli di Azure, potrebbe essere prevista una tariffa per un massimo di una determinata quantità di unità fatturabili, quindi una tariffa diversa dopo tale quantità. | *1* |
| ConsumedQuantity | Quantità di servizio utilizzata (ad esempio ore o GB) durante il periodo di reporting. Include anche l'utilizzo non fatturato dei periodi di report precedenti. | *11* |
| IncludedQuantity | Unità incluse nell'offerta. In genere non è presente in CSP. | *0* |
| OverageQuantity | Unità non incluse nell'offerta. Queste devono essere pagate dal partner. Uguale a **ConsumedQuantity** meno **IncludedQuantity**. | *11* |
| ListPrice | Prezzo dell'offerta in vigore alla data di inizio della sottoscrizione. | *$0.0808* |
| PretaxCharges | Uguale a **ListPrist** moltiplicato per **OverageQuantity**, arrotondato al centesimo più vicino. | *$0.085* |
| TaxAmount | Importo dell'imposta addebitato. In base alle regole fiscali del mercato e a circostanze specifiche. | *$0,08* |
| PostTaxTotal | Totale al netto delle imposte, quando applicabili. | *$0,93* |
| Valuta | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verificare che corrisponda alla prima fattura e quindi dopo gli aggiornamenti principali della piattaforma di fatturazione. | *EUR* |
| PretaxEffectiveRate | Prezzo per unità al lordo delle imposte. Uguale a **PretaxCharges** diviso per **OverageQuantity,** arrotondato al centesimo più vicino. | *$0,08* |
| PostTaxEffectiveRate | Prezzo per unità al netto delle imposte. Uguale a **PostTaxTotal** diviso per **OverageQuantity,** arrotondato al centesimo più vicino. Oppure, uguale a **PretaxEffectiveRate** più l'aliquota fiscale per importo unitario, arrotondata al centesimo più vicino. | *$0,08* |
| ChargeType | Tipo [di addebito o](recon-file-charge-types.md) rettifica. | Vedere [Tipi di addebito](recon-file-charge-types.md). |
| CustomerId | Identificatore Microsoft univoco per il cliente, in formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nome di dominio del cliente. Questo campo può essere vuoto fino al secondo ciclo di fatturazione. | *example.onmicrosoft.com* |
| BillingCycleType | Frequenza di fatturazione dell'ora.| **Monthly** (Mensile)  |
| Unità | Unità della risorsa **Nome**. | *GB* o *ORE* |
| CustomerBillableAccount | Identificatore univoco dell'account nella piattaforma di fatturazione Microsoft. | *1280018095* |
| UsageDate | Data della distribuzione del servizio. | *2/1/2019 0:00* |
| MeteredRegion | Identifica la posizione di un data center all'interno dell'area (per i servizi in cui questo valore è applicabile e popolato). | *Asia orientale*, *South Asia orientale*, *North Europe*, West *Europe*, North *Central US*, South *Central US* |
| MeteredService | Identifica il singolo utilizzo del servizio di Azure quando non viene identificato in modo specifico nella **colonna ServiceName.** Ad esempio, i trasferimenti di dati vengono *segnalati come Microsoft Azure - Tutti i servizi* nella colonna **ServiceName.** | *AccessControl,* *rete CDN,* *calcolo,* *database,* *ServiceBus,* *archiviazione* |
| MeteredServiceType | Sottotesto per **il campo MeteredService** che fornisce chiarimenti aggiuntivi sull'utilizzo del servizio di Azure. | *EXTERNAL* |
| Project | Nome definito dal cliente per la propria istanza del servizio. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Numero di connessioni bus di servizio di Azure di cui è stato effettuato il provisioning e utilizzate in un determinato giorno. | *1.000000 connessioni /30* giorni (se è stato effettuato il provisioning di una connessione singolarmente durante un mese di 30 giorni), *25 connessioni /30 giorni - Usato: 1.0000000* (se è stato effettuato il provisioning di un pacchetto di 25 connessioni del bus di servizio e ne è stato usato 1 durante tale giorno) |

## <a name="next-steps"></a>Passaggi successivi

- [Informazioni sui campi nei Partner Center di riconciliazione basati su licenza](license-based-recon-files.md)