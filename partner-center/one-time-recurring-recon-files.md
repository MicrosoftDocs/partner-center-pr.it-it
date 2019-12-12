---
title: File di riconciliazione monouso e ricorrenti | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Informazioni sui file di riconciliazione monouso e periodici nel centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004900"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>File di riconciliazione singola e ricorrente

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Amministratore fatturazione
-   Agente amministratore
-   Agente di vendita

In questo argomento viene illustrato come leggere i file di riconciliazione monouso e periodici nel centro per i partner.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campi in un file di riconciliazione monouso e ricorrente

| Column | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore univoco del tenant Azure Active Directory (Azure AD) per un'entità di fatturazione specifica in formato GUID. Non obbligatorio per la riconciliazione. È lo stesso per tutte le righe. |
| Customer Id | Identificatore univoco del tenant Azure AD in formato GUID. Identifica il cliente. |
| Nome cliente | Nome dell'organizzazione del cliente, come indicato nel centro per i partner. |
| CustomerDomainName | Nome di dominio del cliente. Questo campo potrebbe risultare vuoto fino al secondo ciclo di fatturazione. *Non usare questo campo come identificatore univoco per il cliente. Il cliente/partner può aggiornare il dominio Vanity o default tramite il portale di Office 365.* |
| Customer Country | Paese in cui si trova il cliente. |
| Numero fattura | Numero di fattura in cui viene visualizzata la transazione specificata. |
| MpnId | Identificatore MPN del partner CSP. |
| Rivenditore MpnId | Identificatore MPN del rivenditore del record per la sottoscrizione. |
| ID ordine | Identificatore univoco per un ordine in Microsoft Commerce platform. Non utilizzato per la riconciliazione. |
| Data ordine | Data di effettuazione dell'ordine. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per un particolare SKU (unità di supporto). |
| AvailabilityId | Identificatore della disponibilità di uno SKU specifico. Ciò indica se lo SKU è disponibile per l'acquisto in un determinato paese, valuta, segmento di settore e così via. |
| Nome SKU | Titolo di una particolare SKU. |
| Nome del prodotto | Nome del prodotto. |
| PublisherName | Nome del server di pubblicazione del prodotto.
| PublisherID | Identificatore univoco per un server di pubblicazione specifico. |
| Descrizione della sottoscrizione | Nome descrittivo di una sottoscrizione. |
| ID sottoscrizione | Identificatore univoco per una sottoscrizione nella piattaforma Microsoft Commerce. Non utilizzato per la riconciliazione. *Questo identificatore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* |
| ChargeStartDate | Giorno di inizio degli addebiti. L'ora indicata è sempre l'inizio della giornata, le 0:00. |
| ChargeEndDate | Giorno di fine degli addebiti. L'ora indicata è sempre la fine della giornata, le 23:59. |
| Termini e billingcycle | Durata e ciclo di fatturazione per l'acquisto (ad esempio, *1 anno, mensile*). |
| Tipo di addebito | Tipo di addebito o rettifica. |
| Prezzo unitario | Prezzo unitario pubblicato nell'elenco prezzi al momento dell'acquisto. *Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione.* |
| Prezzo unitario effettivo | Prezzo unitario dopo le rettifiche apportate. |
| Quantità | Numero di unità. *Assicurarsi che corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione.* |
| Tipo di unità | Tipo di unità da acquistare. |
| DiscountDetails | Spiegazione di qualsiasi sconto applicabile. |
| Totale parziale | Totale al lordo delle imposte. Controlla se il subtotale corrisponde al totale previsto, in caso di sconto. |
| Imposta totale | Addebito IVA. In base alle regole fiscali e alle circostanze specifiche del mercato. |
| Totale | Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte. |
| Currency | Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Assicurarsi che corrisponda alla prima fattura e controllare di nuovo dopo gli aggiornamenti principali della piattaforma di fatturazione. |
| AlternateID | Identificatore alternativo a un **ID dell'ordine**. |
