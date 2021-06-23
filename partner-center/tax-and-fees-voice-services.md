---
title: Imposte e tariffe del servizio PSTN a livello regionale
description: Un partner di Office 365 che Microsoft 365 prodotti Voice può essere soggetto a imposte, tariffe o requisiti normativi per i servizi PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85eefb49cf62c4bcfa5533683abd8ddb0e854463
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112490071"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Imposte regionali, normative per i servizi PTSN (Public Switched Telephone Network)

**Ruoli appropriati:** Amministratore globale | Amministratore utenti | Agente amministratore

I servizi PSTN (Public Switched Telephone Network) in alcune giurisdizioni possono essere soggetti a requisiti fiscali e normativi speciali che possono influire sull'ordine e sulla fatturazione dei partner. Nel Stati Uniti, inclusi Porto Rico, i servizi PSTN, che includono audioconferenza, piani di chiamata e crediti di comunicazione, sono soggetti a requisiti fiscali e normativi speciali. Nei Stati Uniti e a Puerto Rico, Microsoft prezzi servizi PSTN come tax-inclusive.  Le imposte e le normative PSTN univoche influiranno sui partner di Office 365 che Microsoft 365 prodotti Voice.  Se un partner applica ricarichi al prezzo di un servizio PSTN Microsoft, potrebbe avere la responsabilità di calcolare e versare imposte e tariffe specifiche per i servizi PSTN.

## <a name="partner-recommendations"></a>Raccomandazioni per i partner

Coinvolgere il consulente fiscale e legale per comprendere la responsabilità dell'organizzazione in merito alla normativa, alle imposte e alle tariffe dei servizi PSTN e ad altre potenziali responsabilità.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Presentazione della fattura e file di riconciliazione partner

Le fatture Cloud Solution Provider (CSP) e i file di riconciliazione CSP nei servizi Stati Uniti, Puerto Rico e Canada, che includono i servizi PSTN di Skype for Business e Microsoft 365 Voice, forniranno voci separate per i componenti PSTN e non PSTN.

Inoltre, nelle fatture CSP verrà visualizzata la nota a piè di pagina seguente:

* Il prezzo visualizzato è un addebito per i servizi di audioconferenza e piano di chiamata.  Le eventuali imposte transazionali applicabili vengono addebitate esclusivamente sull'importo indicato, ad eccezione delle vendite effettuate all'interno del Stati Uniti.  Negli Stati Uniti, il prezzo visualizzato è fiscale inclusivo perché include un addebito per il piano di chiamata e i servizi di audioconferenza e un addebito per le imposte e le tariffe che è necessario addebitare.  I servizi di audioconferenza e piano di chiamata sono forniti dall'affiliata Microsoft autorizzata a fornirli.  Per informazioni dettagliate, vedere [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Esempio di file di riconciliazione

Office 365 Enterprise E5 presenta nel file di riconciliazione due voci con nomi identici e ID identici, ma ogni voce ha un prezzo unitario univoco (ad esempio, $ 28,40 e $ 2,00). Questo separa il componente Servizi di conferenza PST Skype for Business dell'offerta Office 365, in modo da poter applicare correttamente le imposte.

**Esempio di riconciliazione partner #1 (selezionare le colonne):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Tariffa periodica   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Tariffa periodica   |2,00   |

**Esempio di riconciliazione dei partner #2**

Microsoft 365 Business Voice disponibile in Canada ha componenti aggiuntivi tassabili PSTN consolidati nella fattura CSP (analogamente a Office 365 E5, vengono presentate due voci, una per i componenti PSTN e l'altra per i componenti non PSTN).  Il file di riconciliazione CSP per Microsoft 365 Business Voice visualizza tutti i componenti tassabili PSTN singolarmente (i singoli componenti PSTN non verranno consolidati nello strumento .CSV o API).  La somma dei dettagli dell'ordine e degli importi fatturati per i clienti trovati nel file di riconciliazione corrisponderà alla fattura CSP.

## <a name="additional-resources"></a>Risorse aggiuntive
Per altri dettagli, visitare il [sito Microsoft 365 per i](https://www.microsoft.com/microsoft-365/partners/) partner.

