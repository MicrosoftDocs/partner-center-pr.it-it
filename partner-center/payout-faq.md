---
title: Domande frequenti sul pagamento per Microsoft Commercial Marketplace
description: Risposte alle domande più comuni sui pagamenti nel Marketplace commerciale.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335701"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Domande comuni sui pagamenti del Marketplace commerciale

In questo articolo vengono fornite le risposte alle domande frequenti sui pagamenti nel Marketplace commerciale.

## <a name="earnings-incorrect-or-missing"></a>Guadagni non corretti o mancanti

#### <a name="why-are-my-earnings-missing"></a>Perché mancano i guadagni?

- L'ordine del cliente potrebbe non essere ancora idoneo per il pagamento. Per gli ordini dei clienti non aziendali, è necessario che Microsoft riceva i pagamenti dei clienti prima che i guadagni del Publisher risultino idonei. Per gli ordini dei clienti aziendali, i guadagni saranno disponibili 1-2 giorni dopo la data dell'ordine di acquisto. Verificare lo stato dell'ordine nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- I guadagni dalle transazioni prima del 2019 luglio potrebbero non essere visualizzati nel report Cronologia transazioni. Controllare le istruzioni cronologiche nel [download del pagamento](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Controllare l'intervallo [di tempo del ciclo di pagamento](payment-thresholds-methods-timeframes.md) e comprendere quando i guadagni dovrebbero essere visualizzati nell'istruzione di pagamento.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Perché la quantità di guadagni è diversa da quella prevista?

- Se l'ordine è stato parzialmente pagato dal cliente, la quantità di guadagno sarà basata sull'importo parzialmente pagato dopo la deduzione della tariffa e l'imposizione appropriata.
- Controllare la responsabilità delle imposte in base al paese. Nel caso di paesi in cui il fisco è responsabile di Microsoft, Microsoft raccoglie e sottrae le imposte dai guadagni degli editori. L'importo della transazione indicato nell'istruzione è after Tax Amount. Vedere [i dettagli delle imposte](tax-details-marketplace.md).
- Le offerte SaaS e IaaS hanno una tariffa scontata per le agenzie al 10% anziché il 20% standard, lasciando una percentuale di guadagni pari al 90%. Questa promozione è valida fino al 30 giugno 2021.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [soglia di pagamento, metodo e](payment-thresholds-methods-timeframes.md)intervallo di tempo, pagamento [nel Marketplace commerciale](marketplace-get-paid.md), [Dettagli fiscali](tax-details-marketplace.md), [rendiconto dei pagamenti](payout-statement.md), [Dashboard ordini in analisi del Marketplace commerciale](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Riconciliazione degli utili
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Ricerca per categorie risolvere le differenze tra le istruzioni di pagamento e i report sugli ordini o sull'utilizzo in Analytics?
Utilizzare AssetID, orderID e l'ID dell'elemento linea visualizzati nel report Cronologia transazioni di pagamento con ordini analitici e report sull'utilizzo. Usare questo mapping:

- Cronologia transazioni di pagamento. AssetID = Order. OrderID
- Cronologia delle transazioni di pagamento. OrderID & LineItem = Usage. UsageReferenceID [OrderID: LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Ricerca per categorie sa quando prevedere i pagamenti per gli ordini dei clienti?
- Per prima cosa, usando il assetID, controllare gli ordini dei clienti nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Verificare il canale cliente per la sottoscrizione cliente nel [report clienti](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Per i clienti aziendali, i guadagni dell'editore vengono visualizzati nell'istruzione 1-2 giorni dopo la data dell'ordine di acquisto.
- Per i clienti non aziendali, i guadagni dell'editore vengono visualizzati nell'istruzione 1-2 giorni dopo la ricezione del pagamento del cliente.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [Dashboard ordini in analisi del Marketplace commerciale](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Criteri di pagamento

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Ricerca per categorie trovare la tariffa dell'Agenzia corrente e la tariffa di pagamento?

- Controllare il contratto per la pubblicazione nel Marketplace commerciale. La tariffa standard per l'Agenzia è il 20%. Le transazioni idonee per la co-selling SaaS hanno una tariffa scontata del 10%. Controllare gli annunci di eventuali tariffe promozionali per l'Agenzia.
- Nell'istruzione per il pagamento, la velocità di guadagno specifica la percentuale effettiva di pagamento per una determinata transazione.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Quando si può prevedere un pagamento da Microsoft quando I guadagni sono visualizzati nella mia istruzione?
- Quando il guadagno è in stato non elaborato, è possibile controllare la data di scadenza per il mese in cui verranno elaborati i guadagni per il pagamento. Una volta preparato il pagamento, lo stato di guadagno verrà modificato in "elaborato".  Microsoft rilascia i pagamenti entro il 15 del mese di maturità.
- Per gli ordini pagati dalla carta di credito, Microsoft riceve i pagamenti per 30 giorni fino alla maturazione del guadagno.

 **Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [Dettagli sulle imposte](tax-details-marketplace.md), [soglia di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Pagamenti e rettifiche

#### <a name="why-is-my-payment-missing"></a>Perché manca il pagamento?

- Verificare che lo stato dei pagamenti e lo stato del profilo fiscale siano *validi* nella [pagina Panoramica](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- È possibile che non sia stata soddisfatta la soglia minima per un pagamento. I guadagni devono essere di almeno $50 USD per ricevere un pagamento.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Ricerca per categorie impostare l'account in modo che non riceva pagamenti?
È possibile mantenere i pagamenti nel [profilo di pagamento](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); è sufficiente controllare l' **attesa**. Microsoft effettuerà il pagamento fino a quando non si rilascia il possesso.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Perché ricevo una valuta diversa rispetto alla valuta di acquisto?

La valuta del pagamento è basata sulla valuta selezionata in profilo di pagamento. La valuta di acquisto è basata sulla valuta pagata dal cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>Ricerca per categorie riconciliare le modifiche?

Le rettifiche di pagamento sono correzioni di pagamento per supportare le regolazioni compensative, ad esempio problemi di sistema. Nell'istruzione di pagamento ReasonCode specifica il motivo della regolazione. Questi non sono progettati per riconciliare direttamente le singole transazioni.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [Dettagli sulle imposte](tax-details-marketplace.md), [soglia di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Imposte

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>In che modo è possibile identificare la responsabilità delle dichiarazioni fiscali tra Microsoft o Publisher nell'istruzione di pagamento?

Nel download della cronologia delle transazioni trovare la colonna modello di imposta. Questo mostra la gestione di MS o ISV. Vedere le regole fiscali specifiche per i paesi e le implicazioni dei pagamenti nei [Dettagli delle imposte](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Ricerca per categorie scaricare i moduli fiscali per la tariffa del servizio?

Passare alla pagina **pagamento** pagamenti, quindi alla sezione **elenco di pagamenti** . Viene visualizzato un collegamento al modulo di imposta della tassa di servizio per un pagamento con la tassa di servizio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Ricerca per categorie scaricare un modulo per le imposte ritenute in formato PDF?

Passare alla pagina *pagamento* pagamenti, quindi alla sezione **elenco di pagamenti** . Accanto a un pagamento viene visualizzato un collegamento a un modulo per le imposte ritenute.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano I moduli fiscali di tipo year-end?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli fiscali di tipo year-end.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Ricerca per categorie trovare le imposte ritenute per una transazione?
Per gli autori degli Stati Uniti che hanno presentato un modulo W-9 è applicabile la ritenuta delle imposte. Le imposte di ritenuta vengono calcolate in un pagamento mensile.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri di pagamento](payout-policy-details.md)

## <a name="payout-statement-access"></a>Accesso alle istruzioni di pagamento

#### <a name="how-do-i-access-a-payout-statement"></a>Ricerca per categorie accedere a una dichiarazione di pagamento?

1. Controllare i ruoli. È necessario avere il ruolo di *collaboratore finanziario* o di *proprietario dell'account* per accedere all'istruzione per il pagamento.
2. Nella finestra di spostamento in alto a destra selezionare l'icona di **pagamento** per visualizzare l'istruzione per il pagamento. Scegliere tra la **cronologia delle transazioni**, il **pagamento**e il **download**.

**Ulteriori informazioni**: [ruoli e autorizzazioni per il pagamento](payout-statement.md#roles-and-permissions), [istruzioni di pagamento](payout-statement.md) 

## <a name="payout-statement-report"></a>Report sulle istruzioni di pagamento

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Cosa significa ogni campo nel download della transazione?

Per un elenco dettagliato degli attributi e dei relativi significati, vedere [istruzioni di pagamento](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Che cosa sta guadagnando lo stato?

Ciò mostra i guadagni come non elaborati, elaborati o inviati.

- Non **elaborati** : i guadagni rientrano in un periodo di deposito fino alla data di scadenza.
- **Elaborati** : i guadagni sono maturi e vengono preparati in un pagamento mensile. I pagamenti vengono rilasciati entro il 15 di ogni mese.
- **Inviato** : il pagamento è stato rilasciato alla banca in base al profilo di pagamento.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Ricerca per categorie scaricare i moduli fiscali per la tariffa del servizio?

Passare alla pagina **pagamento** pagamenti, quindi alla sezione **elenco di pagamenti** . Viene visualizzato un collegamento al modulo di imposta della tassa di servizio per un pagamento con la tassa di servizio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Ricerca per categorie scaricare un modulo per le imposte ritenute in formato PDF?

Passare alla pagina **pagamento** pagamenti, quindi alla sezione **elenco di pagamenti** . Accanto a un pagamento viene visualizzato un collegamento a un modulo per le imposte ritenute.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano I moduli fiscali di tipo year-end?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli fiscali di tipo year-end.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [download della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Rendiconti cronologici

#### <a name="how-do-i-view-historical-information"></a>Ricerca per categorie visualizzare le informazioni cronologiche?

Nell'istruzione cronologica viene visualizzato lo snapshot dei dati di pagamento a partire dal 2019 ottobre. Sfortunatamente, le informazioni sui pagamenti non vengono aggiornate. Per ricevere le informazioni più aggiornate, inviare un ticket di supporto per i dati più recenti.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [download della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API di esportazione del pagamento

#### <a name="how-do-i-download-payout-data"></a>Ricerca per categorie scaricare i dati sui pagamenti?

Usare l' [API](https://apidocs.microsoft.com/services/partnerpayouts)per i pagamenti dei partner.

## <a name="next-steps"></a>Passaggi successivi

- [Come ottenere i pagamenti nel marketplace commerciale](marketplace-get-paid.md)
