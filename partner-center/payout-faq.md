---
title: Domande frequenti sul pagamento per Microsoft Commercial Marketplace
description: Risposte alle domande più comuni sui pagamenti nel Marketplace commerciale. Include le risposte ai motivi per cui i guadagni sono diversi da quelli previsti.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175288"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Domande comuni sui pagamenti del Marketplace commerciale

In questo articolo vengono fornite le risposte alle domande frequenti sui pagamenti nel Marketplace commerciale.

## <a name="earnings-incorrect-or-missing"></a>Guadagni non corretti o mancanti

#### <a name="why-are-my-earnings-missing"></a>Perché gli utili non sono presenti?

- L'ordine del cliente potrebbe non essere ancora idoneo per il pagamento. Per gli ordini di clienti non aziendali, Microsoft deve ricevere il pagamento del cliente prima che gli utili dell'editore risultino idonei. Per gli ordini dei clienti aziendali, gli utili saranno disponibili 1-2 giorni dopo la data dell'ordine di acquisto. Verificare lo stato dell'ordine nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Gli utili delle transazioni eseguite prima di luglio 2019 potrebbero non essere visualizzati nel report Cronologia transazioni. Controllare lo storico degli estratti in [Payout Download](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport) (Download del pagamento).
- Controllare l'intervallo [di tempo del ciclo di pagamento](payment-thresholds-methods-timeframes.md) e comprendere quando i guadagni dovrebbero essere visualizzati nell'istruzione di pagamento.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Perché la quantità di guadagni è diversa da quella prevista?

- Se l'ordine è stato parzialmente pagato dal cliente, la quantità di guadagno sarà basata sull'importo parzialmente pagato dopo la deduzione della tariffa e l'imposizione appropriata.
- Controllare la responsabilità delle imposte in base al paese. Nel caso di paesi in cui la responsabilità delle imposte ricade su Microsoft, Microsoft somma e sottrae le imposte dagli utili degli editori. L'importo della transazione indicato nell'estratto non include l'importo delle tasse. Vedere [Dettagli imposte](tax-details-marketplace.md).
- Le offerte SaaS e IaaS hanno una tariffa scontata per le agenzie al 10% anziché il 20% standard, lasciando una percentuale di guadagni pari al 90%. Questa promozione è valida fino al 30 giugno 2021.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [soglia di pagamento, metodo e](payment-thresholds-methods-timeframes.md)intervallo di tempo, pagamento [nel Marketplace commerciale](marketplace-get-paid.md), [Dettagli fiscali](tax-details-marketplace.md), [rendiconto dei pagamenti](payout-statement.md), [Dashboard ordini in analisi del Marketplace commerciale](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Riconciliazione degli utili
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Come risolvere le differenze tra l'estratto conto e i report sugli ordini o sull'utilizzo nell'analisi?
Utilizzare AssetID, orderID e l'ID dell'elemento linea visualizzati nel report Cronologia transazioni di pagamento con ordini analitici e report sull'utilizzo. Usare questo mapping:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Come fare per sapere quando si riceveranno i pagamenti per gli ordini dei clienti?
- Per prima cosa, usando il assetID, controllare gli ordini dei clienti nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Verificare il canale cliente per la sottoscrizione cliente nel [report clienti](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Per i clienti aziendali, i guadagni dell'editore vengono visualizzati nell'istruzione 1-2 giorni dopo la data dell'ordine di acquisto.
- Per i clienti non aziendali, i guadagni dell'editore vengono visualizzati nell'istruzione 1-2 giorni dopo la ricezione del pagamento del cliente.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [Dashboard ordini in analisi del Marketplace commerciale](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Criteri di pagamento

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Come trovare l'attuale commissione dell'agenzia e la tariffa di pagamento?

- Controllare la pagina del Contratto per gli editori del Marketplace. La commissione standard dell'agenzia è il 20%. SaaS Co-Sell le transazioni idonee hanno una tariffa scontata del 10%. Controllare gli annunci di eventuali commissioni promozionali dell'agenzia.
- Nell'istruzione per il pagamento, la velocità di guadagno specifica la percentuale effettiva di pagamento per una determinata transazione.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Dopo che gli utili vengono visualizzati nell'estratto quando si riceverà il pagamento da Microsoft?
- Quando gli utili sono nello stato non elaborato, è possibile controllare la data di scadenza per il mese in cui verranno elaborati per il pagamento. Una volta preparato il pagamento, lo stato di guadagno verrà modificato in "elaborato".  Microsoft emette i pagamenti entro il 15 del mese di scadenza.
- Per gli ordini pagati dalla carta di credito, Microsoft riceve i pagamenti per 30 giorni fino alla maturazione del guadagno.

 **Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [Dettagli sulle imposte](tax-details-marketplace.md), [soglia di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Pagamenti e rettifiche

#### <a name="why-is-my-payment-missing"></a>Perché manca il pagamento?

- Verificare che lo stato dei pagamenti e lo stato del profilo fiscale siano *validi* nella [pagina Panoramica](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- È possibile che non sia stata raggiunta la soglia minima per il pagamento. Per ricevere un pagamento l'importo deve essere di almeno 50 USD.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Ricerca per categorie impostare l'account in modo che non riceva pagamenti?
È possibile mantenere i pagamenti nel [profilo di pagamento](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); è sufficiente controllare l' **attesa**. Microsoft effettuerà il pagamento fino a quando non si rilascia il possesso.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Perché ricevo il pagamento in una valuta diversa rispetto alla valuta di acquisto?

La valuta del pagamento si basa sulla valuta selezionata nel profilo di pagamento. La valuta di acquisto si basa sulla valuta pagata dal cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>Come riconciliare le rettifiche?

Le rettifiche di pagamento sono correzioni del pagamento per supportare le rettifiche compensative, ad esempio problemi di sistema. Nell'estratto conto ReasonCode specifica il motivo della rettifica. Lo scopo non è quello di riconciliare direttamente le singole transazioni.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri](payout-policy-details.md)di pagamento, [Dettagli sulle imposte](tax-details-marketplace.md), [soglia di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Imposte

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>In che modo è possibile identificare la responsabilità del versamento imposte tra Microsoft o l'editore nell'estratto conto?

Nel download della cronologia delle transazioni trovare la colonna del modello fiscale. Qui viene visualizzata la gestione di MS o ISV. Consultare le leggi fiscali specifiche per un paese e ciò che implicano per i pagamenti in [Dettagli imposte](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Come scaricare i moduli della tassa sul servizio?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Viene visualizzato un collegamento al modulo Tassa sul servizio per un pagamento con tassa sul servizio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Come scaricare un modulo per la ritenuta d'acconto in formato PDF?

Andare alla pagina *Payout Payment* (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Accanto al pagamento viene visualizzato un collegamento al modulo per la ritenuta d'acconto.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano i moduli per le tasse di fine anno?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli per le tasse di fine anno.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Come trovare la ritenuta d'acconto per una transazione?
La ritenuta d'acconto è applicabile per gli editori degli Stati Uniti che hanno inviato il modulo W-9. La ritenuta d'acconto viene calcolata sui pagamenti mensili.

**Ulteriori**informazioni: [contratto per la pubblicazione nel Marketplace commerciale](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Dettagli sui criteri di pagamento](payout-policy-details.md)

## <a name="payout-statement-access"></a>Accesso alle istruzioni di pagamento

#### <a name="how-do-i-access-a-payout-statement"></a>Come si accede all'estratto conto?

1. Controllare il proprio ruolo. Per accedere all'estratto conto, è necessario avere il ruolo di *collaboratore finanziario* o *proprietario dell'account*.
2. Nella finestra di spostamento in alto a destra selezionare l'icona di **pagamento** per visualizzare l'istruzione per il pagamento. Scegliere tra la **cronologia delle transazioni**, il **pagamento**e il **download**.

**Ulteriori informazioni**: [ruoli e autorizzazioni per il pagamento](payout-statement.md#roles-and-permissions), [istruzioni di pagamento](payout-statement.md) 

## <a name="payout-statement-report"></a>Report sulle istruzioni di pagamento

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Cosa significano i campi nel download della transazione?

Per un elenco dettagliato degli attributi e dei relativi significati, vedere [istruzioni di pagamento](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Cos'è lo stato degli utili?

Ciò mostra i guadagni come non elaborati, elaborati o inviati.

- Non **elaborati** : i guadagni rientrano in un periodo di deposito fino alla data di scadenza.
- **Elaborati** : i guadagni sono maturi e vengono preparati in un pagamento mensile. I pagamenti vengono rilasciati entro il 15 di ogni mese.
- **Inviato** : il pagamento è stato rilasciato alla banca in base al profilo di pagamento.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Come scaricare i moduli della tassa sul servizio?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Viene visualizzato un collegamento al modulo Tassa sul servizio per un pagamento con tassa sul servizio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Ricerca per categorie scaricare un modulo per le imposte ritenute in formato PDF?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Accanto al pagamento viene visualizzato un collegamento al modulo per la ritenuta d'acconto.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano i moduli per le tasse di fine anno?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli per le tasse di fine anno.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [download della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Rendiconti cronologici

#### <a name="how-do-i-view-historical-information"></a>Ricerca per categorie visualizzare le informazioni cronologiche?

Nel rendiconto cronologico viene visualizzato lo snapshot dei dati di pagamento a partire da ottobre 2019. Sfortunatamente, le informazioni sui pagamenti non vengono aggiornate. Per ricevere le informazioni più aggiornate, inviare un ticket di supporto per i dati più recenti.

**Ulteriori informazioni**: [istruzioni](payout-statement.md)per i pagamenti, [download della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API di esportazione del pagamento

#### <a name="how-do-i-download-payout-data"></a>Come si possono scaricare i dati relativi ai pagamenti?

Usare l' [API](https://apidocs.microsoft.com/services/partnerpayouts)per i pagamenti dei partner.

## <a name="next-steps"></a>Passaggi successivi

- [Come ottenere i pagamenti nel marketplace commerciale](marketplace-get-paid.md)
