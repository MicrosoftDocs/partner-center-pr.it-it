---
title: File di riconciliazione dell'utilizzo con classificazione giornaliera | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Informazioni sui file di riconciliazione dell'utilizzo giornalieri nel centro per i partner.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389699"
---
# <a name="daily-rated-usage-reconciliation-files"></a>File di riconciliazione dell'utilizzo con classificazione giornaliera

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

In questo argomento viene illustrato come leggere i file di riconciliazione dell'utilizzo con classificazione giornaliera.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campi nei file di riconciliazione dell'utilizzo con classificazione giornaliera

| Column | Descrizione |
| ------ | ----------- |
| PartnerId | Identificatore partner in formato GUID. |
| PartnerName | Nome del partner. |
| CustomerId | Identificatore Microsoft univoco per il cliente in formato GUID. |
| CustomerCompanyName | Nome dell'organizzazione del cliente registrato nel Centro per i partner. *Questa colonna è molto importante per riconciliare la fattura con le informazioni del sistema.* |
| CustomerDomainName | Nome di dominio del cliente. Non disponibile per l'attività corrente. |
| Paese del cliente | Paese in cui si trova il cliente. |
| MPNID | Identificatore MPN del partner CSP. |
| Rivenditore MPNID | Identificatore MPN del rivenditore del record per la sottoscrizione. Non disponibile per l'attività corrente. |
| InvoiceNumber | Numero di fattura in cui viene visualizzata la transazione specificata. Non disponibile per l'attività corrente. |
| ProductId | Identificatore del prodotto. |
| SkuId | Identificatore per un particolare SKU. |
| AvailabilityId | Identificatore della disponibilità di uno SKU specifico. Ciò indica se lo SKU è disponibile per l'acquisto in un determinato paese, valuta, segmento di settore e così via. |
| Nome SKU | Titolo di una particolare SKU. |
| PublisherName | Nome del server di pubblicazione. |
| PublisherID | Identificatore del server di pubblicazione in formato GUID. Non disponibile per l'attività corrente. |
| Descrizione della sottoscrizione | Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Si tratta di un campo identico a **offername**. |
| ID sottoscrizione | Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Non utilizzato per la riconciliazione. *Questo identificatore non corrisponde all' **ID sottoscrizione** nella console di amministrazione partner.* |
| ChargeStartDate | Data di inizio del ciclo di fatturazione (eccetto quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo di fatturazione precedente). L'ora indicata è sempre l'inizio della giornata, le 0:00. |
| ChargeEndDate | Data di fine del ciclo di fatturazione (tranne quando si presentano date di dati di utilizzo latenti precedentemente non addebitati dal ciclo biling precedente). L'ora indicata è sempre la fine della giornata, le 23:59. |
| Data di utilizzo | Data di utilizzo del servizio. |
| Tipo di misuratore | Tipo di misuratore. |
| Categoria misuratore | Servizio di primo livello per l'utilizzo. |
| ID contatore | Identificatore del contatore utilizzato. |
| Sottocategoria contatore | Tipo di servizio di Azure, che può influire sulla frequenza. |
| Nome contatore | Unità di misura per il contatore utilizzato. |
| Area del contatore | Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato. |
| Unità | Unità del **nome**della risorsa. |
| Quantità utilizzata | Quantità di servizio utilizzata (ad esempio, *ore* o *GB*) durante il periodo di Reporting. Include qualsiasi utilizzo non fatturato dei periodi di Reporting precedenti. |
| Percorso della risorsa | > il data center in cui è in esecuzione il contatore. |
| Servizio utilizzato | Il servizio della piattaforma Azure usato. |
| URI risorsa | URI della risorsa in uso. |
| Tipo di addebito | Tipo di addebito o rettifica. Non disponibile per l'attività corrente. |
| Prezzo unitario | Prezzo per licenza, pubblicato nell'elenco prezzi al momento dell'acquisto. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| Quantità | Numero di licenze. Verificare che il prezzo corrisponda alle informazioni archiviate nel sistema di fatturazione durante la riconciliazione. |
| Tipo di unità | Tipo di unità in cui viene addebitato il contatore. Non disponibile per l'attività corrente. |
| Pre-imposta fatturazione | Importo totale della fatturazione prima delle imposte. |
| Valuta fatturazione | Valuta nell'area geografica del cliente. |
| Prezzi pretassazione totali | I prezzi prima dell'aggiunta delle imposte. |
| Valuta prezzi | Valuta nell'elenco prezzi. |
| Informazioni servizio 1 | Numero di connessioni del bus di servizio di cui è stato effettuato il provisioning e utilizzate in un determinato giorno. |
| Informazioni servizio 2 | Campo legacy che acquisisce i metadati facoltativi specifici del servizio. |
| Informazioni aggiuntive | Eventuali informazioni aggiuntive non incluse in altre colonne. |
