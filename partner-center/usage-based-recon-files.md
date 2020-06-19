---
title: File di riconciliazione in base all'uso
ms.topic: article
ms.date: 06/08/2020
description: Informazioni su tutti gli elementi nel file di riconciliazione basato sull'utilizzo nel centro per i partner. Include alcuni esempi.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9a84ca15cd51c02a3b5c53ad4478d72343add284
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909119"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Informazioni sui file di riconciliazione basati sull'utilizzo e sui rispettivi campi specifici nel centro per i partner

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

Per riconciliare gli addebiti rispetto all'utilizzo di un cliente, confrontare **ResellerID**, **ResellerName**e **ResellerBillableAccount** dal file di riconciliazione con il **nome del cliente** e l' **ID sottoscrizione** del centro per i partner.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campi nei file di riconciliazione basati sull'utilizzo

I campi seguenti illustrano quali servizi sono stati usati e la tariffa.

| Colonna | Descrizione | Valore/i di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore del partner, in formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nome partner. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificatore account partner. | *1010578050* |
| CustomerCompanyName | Nome dell'organizzazione del cliente, come indicato nel centro per i partner. *Molto importante per riconciliare la fattura con le informazioni sul sistema.* | *Testare il cliente* |
| MpnId | Identificatore MPN del partner CSP. | *4390934* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione.  |
| InvoiceNumber | Numero di fattura in cui è presente la transazione specificata. | *D020001IVK* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione, ad eccezione dei casi in cui vengono indicate le date relative a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora è sempre l'inizio del giorno, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Data di fine del ciclo di fatturazione, ad eccezione dei casi in cui vengono indicate le date relative a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente). L'ora indicata è sempre la fine della giornata, le 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando si contatta il supporto tecnico. Non utilizzato per la riconciliazione. *Non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Nome alternativo per l'offerta di servizio. | *Microsoft Azure* |
| SubscriptionDescription | Linea commerciale del servizio offerto. | *Microsoft Azure* |
| OrderID | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando si contatta il supporto tecnico. Non utilizzato per la riconciliazione. | *566890604832738111* |
| ServiceName | Nome del servizio di Azure in questione. | *MACCHINE VIRTUALI* |
| ServiceType | Tipo specifico di servizio di Azure. | *Bus di servizio: singolo o pacchetto*, *SQL Azure database-Business o Web Edition* |
| ResourceGuid | Identificatore univoco specifico per tutti i dati del servizio e la struttura dei prezzi. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| NomeRisorsa | Il nome della risorsa di Azure. | *Trasferimento dati in (GB)*, *trasferimento dati (GB)* |
| Region | Area a cui si applica l'utilizzo. Utilizzato principalmente per assegnare frequenze ai trasferimenti di dati, in quanto le tariffe variano in base all'area. | *Asia Pacifico*, *Europa*, *America Latina*, *America del Nord* |
| Sku | Identificatore Microsoft univoco per un'offerta. | *7UD-00001* |
| DetailLineItemId | Identificatore e quantità per descrivere frequenze diverse per un servizio o una risorsa in un determinato periodo di fatturazione. Per i prezzi di Azure a più livelli, è possibile che sia disponibile una sola tariffa per una determinata quantità di unità fatturabili, quindi una frequenza diversa dopo tale quantità. | *1* |
| ConsumedQuantity | Quantità di servizio utilizzata (ad esempio, ore o GB) durante il periodo di Reporting. Include anche l'utilizzo non fatturato dei periodi di report precedenti. | *11* |
| IncludedQuantity | Unità incluse nell'offerta. In genere non è presente in CSP. | *0* |
| OverageQuantity | Unità non incluse come parte dell'offerta. Questi devono essere pagati dal partner. Uguale a **ConsumedQuantity** meno **IncludedQuantity**. | *11* |
| ListPrice | Prezzo dell'offerta in vigore alla data di inizio della sottoscrizione. | *$0.0808* |
| PretaxCharges | Uguale a **ListPrist** moltiplicato per **OverageQuantity**, arrotondato al centesimo più vicino. | *$0.085* |
| TaxAmount | Importo fiscale addebitato. In base alle regole fiscali e alle circostanze specifiche del mercato. | *$0,08* |
| PostTaxTotal | Totale al netto delle imposte, quando applicabili. | *$0,93* |
| Valuta | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verificare che corrisponda alla prima fattura e quindi dopo gli aggiornamenti principali della piattaforma di fatturazione. | *EUR* |
| PretaxEffectiveRate | Prezzo per unità al lordo delle imposte. Uguale a **PretaxCharges** diviso per **OverageQuantity**, arrotondato al centesimo più vicino. | *$0,08* |
| PostTaxEffectiveRate | Prezzo per unità al netto delle imposte. Uguale a **PostTaxTotal** diviso per **OverageQuantity**, arrotondato al centesimo più vicino. Oppure, uguale a **PretaxEffectiveRate** più il tasso di imposta per unità, arrotondato al centesimo più vicino. | *$0,08* |
| ChargeType | [Tipo di addebito](recon-file-charge-types.md) o regolazione. | Vedere [tipi di addebito](recon-file-charge-types.md). |
| CustomerId | Identificatore Microsoft univoco per il cliente, in formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nome di dominio del cliente. Questo campo può essere vuoto fino al secondo ciclo di fatturazione. | *example.onmicrosoft.com* |
| BillingCycleType | Frequenza di fatturazione del tempo.| **Monthly** (Mensile)  |
| Unità | Unità del **nome**della risorsa. | *GB* o *ore* |
| CustomerBillableAccount | Identificatore univoco dell'account nella piattaforma di fatturazione Microsoft. | *1280018095* |
| UsageDate | Data della distribuzione del servizio. | *2/1/2019 0:00* |
| MeteredRegion | Identifica la posizione di un data center all'interno dell'area (per i servizi in cui questo valore è applicabile e popolato). | *Asia orientale*, *Sud Asia orientale*, *Europa settentrionale*, *Europa occidentale*, *Stati Uniti centro-settentrionali*, *Stati Uniti centro-meridionali* |
| MeteredService | Identifica il singolo utilizzo del servizio Azure quando non è identificato in modo specifico nella colonna **ServiceName** . I trasferimenti di dati, ad esempio, vengono segnalati come *Microsoft Azure tutti i servizi* nella colonna **ServiceName** . | *AccessControl*, rete *CDN*, *calcolo*, *database*, *ServiceBus*, *archiviazione* |
| MeteredServiceType | Sottotitolo per il campo **MeteredService** che fornisce informazioni aggiuntive sull'utilizzo dei servizi di Azure. | *ESTERNO* |
| Project | Nome definito dal cliente per la propria istanza del servizio. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Numero di connessioni del bus di servizio di Azure di cui è stato effettuato il provisioning e utilizzate in un determinato giorno. | *1,000000 connessioni/30 giorni* (se si dispone di una connessione con provisioning individuale durante un mese di 30 giorni), *25 connessioni/30 giorni: 1,000000* (se è stato eseguito il provisioning di 25 pacchetti di connessioni del bus di servizio ed è stato usato 1 durante tale giorno) |
