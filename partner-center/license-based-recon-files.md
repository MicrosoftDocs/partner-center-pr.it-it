---
title: File di riconciliazione in base alle licenze
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come leggere i file di riconciliazione basati sulle licenze nel centro per i partner. Questo articolo illustra il significato di ogni campo nel file di ricognizione basato sulle licenze.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bc97156d23fa4ea1082a0ad4a931ff36375897a7
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178919"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Informazioni sui campi nei file di riconciliazione basati su licenze per il centro per i partner

**Si applica a**

- Centro per i partner per Microsoft Government cloud

**Ruoli appropriati**

- Amministratore globale
- Amministratore gestione utenti
- Amministratore fatturazione
- Agente amministratore

Per riconciliare le modifiche rispetto agli ordini di un cliente, confrontare il **Syndication_Partner_Subscription_Number** dal file di riconciliazione con l' **ID sottoscrizione** dal centro per i partner.

## <a name="fields-in-license-based-reconciliation-files"></a>Campi nei file di riconciliazione basati su licenza

| Colonna | Descrizione | Valore di esempio |
| ------ | ----------- | ------------ |
| PartnerId | Identificatore univoco in formato GUID per un'entità di fatturazione specifica. Non obbligatorio per la riconciliazione. È lo stesso per tutte le righe. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nome dell'organizzazione del cliente, come indicato nel centro per i partner. *Campo molto importante per la riconciliazione della fattura con le informazioni sul sistema.* | *Test Customer A* |
| MpnId | Identificatore MPN del partner CSP. Vedere [How to descrivere by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Identificatore MPN del rivenditore del record per la sottoscrizione.  |
| OrderId | Identificatore univoco per un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare l'ordine quando si contatta il supporto tecnico. Non utilizzato per la riconciliazione. | *566890604832738111* |
| SubscriptionId | Identificatore univoco per una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando si contatta il supporto tecnico. Non utilizzato per la riconciliazione. *Questo valore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner. Vedere invece **SyndicationPartnerSubscriptionNumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificatore univoco per le sottoscrizioni. Un cliente può disporre di più sottoscrizioni per lo stesso piano. Questa colonna è importante per l'analisi dei file di riconciliazione. Questo campo esegue il mapping all' **ID sottoscrizione** nella console di amministrazione partner. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Identificatore dell'offerta univoco. Identificatore dell'offerta standard, come definito nell'elenco prezzi. *Questo valore non corrisponde all' **ID offerta** nell'elenco prezzi. Vedere invece **DurableOfferID** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Identificatore dell'offerta durevole univoco, come definito nell'elenco prezzi. *Questo valore corrisponde all' **ID offerta** dall'elenco prezzi.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. | *Microsoft Office 365 (Piano E3)* |
| SubscriptionStartDate | Data di inizio della sottoscrizione. L'ora è sempre l'inizio del giorno, 0:00. Questo campo viene impostato sul giorno dopo l'invio dell'ordine. Usato con **SubscriptionEndDate** per determinare: se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo. | *2/1/2019 0:00* |
| SubscriptionEndDate | Data di fine della sottoscrizione. L'ora è sempre l'inizio del giorno, 0:00. *12 mesi più **x** giorni dopo la data di inizio* per allinearsi alla data di fatturazione del partner o a *12 mesi dalla data di rinnovo*. In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente. È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico. | *2/1/2019 0:00* |
| ChargeStartDate | Giorno di inizio degli addebiti. L'ora è sempre l'inizio del giorno, 0:00. Usato per calcolare i prezzi giornalieri (addebiti *pro rata* ) quando un cliente modifica i numeri di licenza. | *2/1/2019 0:00* |
| ChargeEndDate | Giorno di fine degli addebiti. L'ora indicata è sempre la fine della giornata, le 23:59. Usato per calcolare i prezzi giornalieri (addebiti *pro rata* ) quando un cliente modifica i numeri di licenza. | *2/28/2019 23:59* |
| ChargeType | [Tipo di addebito](recon-file-charge-types.md) o regolazione. | Vedere [tipi di addebito](recon-file-charge-types.md). |
| UnitPrice | Prezzo per licenza, pubblicato nell'elenco prezzi al momento dell'acquisto. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *6,82* |
| Quantità | Numero di licenze. Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. | *2* |
| Amount | Prezzo totale per la quantità. Utilizzato per verificare se il calcolo della quantità corrisponde alla modalità di calcolo di questo valore per i clienti. | *13.32* |
| TotalOtherDiscount | Importo dello sconto applicato a questi addebiti. Le licenze dei prodotti incluse con una competenza o mappe, o nuove sottoscrizioni idonee per un incentivo, conterranno anche un importo di sconto in questo articolo. | *2,32* |
| Subtotale | Totale al lordo delle imposte. Controlla se il subtotale corrisponde al totale previsto, in caso di sconto. | *11* |
| Imposta | Addebito IVA. In base alle regole fiscali e alle circostanze specifiche del mercato. | *0* |
| TotalForCustomer | Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte. | *11* |
| Valuta | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Controllare se corrisponde alla prima fattura. Controllare di nuovo dopo gli aggiornamenti principali della piattaforma di fatturazione. | *EUR* |
| DomainName | Nome di dominio del cliente. Questo campo può essere vuoto fino al secondo ciclo di fatturazione. *Non usare questo campo come identificatore univoco per il cliente. Il cliente/partner può aggiornare il dominio Vanity o default tramite il portale di Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Nome alternativo sottoscrizione. Se non viene specificato alcun nome alternativo, il centro per i partner USA l' **offerta**. | *PROGETTO ONLINE* |
| SubscriptionDescription | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Si tratta di un campo identico a **offername**. | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| BillingCycleType | Frequenza di fatturazione una volta.| *Monthly* (Mensile) |