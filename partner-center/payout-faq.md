---
title: Domande frequenti sui pagamenti e sui profili fiscali
description: Risposte alle domande comuni sui pagamenti e i dettagli fiscali in Partner Center. Include risposte sui motivi per cui gli utili sono diversi da quelli previsti.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 05/06/2021
ms.openlocfilehash: 7f5cf168a87c25f3afe0767769ce8dcc77d07f04
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145831"
---
# <a name="common-questions-about-payouts-and-taxes"></a>Domande comuni su pagamenti e imposte

**Ruoli appropriati:** amministratore account | Amministratore globale | Amministratore incentivi

Questo articolo risponde alle domande frequenti sui pagamenti e sui dettagli fiscali in Partner Center. Gli argomenti trattati includono la tempistica dei pagamenti, la verifica dell'idoneità degli utili e l'importanza di configurare correttamente i profili di pagamento e fiscali.

## <a name="profile-management"></a>Gestione dei profili

#### <a name="why-do-i-need-to-provide-or-update-my-payout-andor-tax-details"></a>Perché è necessario fornire o aggiornare i dettagli relativi ai pagamenti e/o alle imposte?

Tutti i partner che si iscriveno a un nuovo programma devono fornire dettagli fiscali e relativi ai pagamenti validi per completare la registrazione e ricevere i pagamenti. Una registrazione viene considerata completa solo dopo che Microsoft ha convalidato il profilo di pagamento e fiscale.

Potrebbe anche essere necessario aggiornare le informazioni se le regole per il programma cambiano o se gli aspetti del profilo scadono o diventano obsoleti. In questo caso, nella pagina Panoramica verrà visualizzato lo stato **Azione richiesta - Aggiorna il profilo bancario e/o fiscale**.

#### <a name="how-do-i-find-set-up-or-update-payout-and-tax-details"></a>Ricerca per categorie trovare, configurare o aggiornare i dettagli relativi a pagamenti e imposte?

Per informazioni dettagliate su come aggiornare i dettagli di pagamento e fiscali in Partner Center, vedere Configurare l'account dei pagamenti e [i moduli fiscali.](set-up-your-payout-account.md)

#### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>Perché non vedo le registrazioni quando assegno i profili di pagamento e fiscali?

È possibile che non si abbia le autorizzazioni appropriate o che si sia connessi con un account che non dispone di queste autorizzazioni. Ad esempio, solo gli amministratori degli incentivi per la posizione MPN possono creare o gestire profili di pagamento e fiscali. Contattare l'amministratore dell'organizzazione per gestire le autorizzazioni bancarie e fiscali.

#### <a name="im-only-able-to-sign-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>È possibile accedere solo con il @onmicrosoft.com dominio. Cosa devo fare?

Contattare l'amministratore account per aggiungere altri domini all'account AAD.
 
#### <a name="my-organization-is-participating-in-multiple-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>L'organizzazione partecipa a più programmi. È necessario fornire più volte il profilo di pagamento e fiscale?

Dipende dalle esigenze dell'organizzazione. I profili di pagamento vengono creati a livello di organizzazione, che consente di assegnare lo stesso profilo bancario tra più ID MPN e programmi all'interno di un'organizzazione. Nella maggior parte dei casi, è possibile riutilizzare un profilo esistente o crearne uno nuovo.

Tuttavia, quando si applica il profilo bancario a paesi o aree geografiche diverse, è possibile che ci siano delle eccezioni.

I profili fiscali creati per una località MPN vengono riutilizzati e popolati automaticamente quando la stessa località MPN partecipa a un altro programma. Ma possono esserci delle eccezioni. Ad esempio, per le regole di pagamento di un nuovo programma Incentivi potrebbero essere necessari altri dettagli per il profilo fiscale.

#### <a name="can-i-use-the-same-bank-and-tax-details-for-all-incentive-programs-at-microsoft"></a>È possibile usare gli stessi dettagli bancari e fiscali per tutti i programmi di incentivi microsoft?

Se l'azienda è invitata per più programmi, è possibile usare lo stesso account di pagamento per tutti i programmi oppure scegliere di avere account di pagamento diversi per i diversi programmi.


#### <a name="how-does-microsoft-ensure-that-the-bank-information-is-indeed-that-of-the-company-and-not-a-personal-bank-account-for-an-employee"></a>In che modo Microsoft garantisce che le informazioni bancarie siano effettivamente dell'azienda e non un conto bancario personale per un dipendente?

È responsabilità dell'azienda assicurarsi che il ruolo di amministratore degli incentivi, che ha le autorizzazioni per modificare queste informazioni, sia assegnato solo ai dipendenti appropriati.

#### <a name="my-tax-profile-has-expired-how-do-i-fix-update-it"></a>Il profilo fiscale è scaduto. Ricerca per categorie correggere l'aggiornamento?

Se un profilo fiscale è scaduto o sta per scadere, significa che il modulo fiscale fornito a Microsoft deve essere aggiornato. Per aggiornare il profilo fiscale, seguire questa procedura:

1. Accedere al [dashboard](https://partner.microsoft.com/dashboard/home)Partner Center e quindi selezionare l'icona a forma di ingranaggio per aprire **il** menu Impostazioni.
2. Selezionare **Account settings (Impostazioni account),** **espandere la sezione Payout and tax** (Pagamenti e imposte) e quindi selezionare Payout and tax profile **(Profilo di pagamento e** imposta).
3. Selezionare **Profilo** fiscale
4. Controllare la colonna **Expiration Date (Data** di scadenza) e passare al profilo fiscale scaduto o in scadenza.
5. Selezionare **Modifica** per avviare il processo di modifica del profilo fiscale.
6. Nella sezione del modulo fiscale specificare i dettagli aggiornati.

## <a name="earnings-incorrect-or-missing"></a>Utili errati o mancanti

#### <a name="why-are-my-earnings-missing"></a>Perché gli utili non sono presenti?

- L'ordine del cliente potrebbe non essere ancora idoneo per il pagamento. Per gli ordini di clienti non aziendali, Microsoft deve ricevere il pagamento del cliente prima che gli utili dell'editore risultino idonei. Per gli ordini dei clienti aziendali, gli utili saranno disponibili 1-2 giorni dopo la data dell'ordine di acquisto. Verificare lo stato dell'ordine nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Gli utili delle transazioni eseguite prima di luglio 2019 potrebbero non essere visualizzati nel report Cronologia transazioni. Controllare lo storico degli estratti in [Payout Download](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport) (Download del pagamento).
- Controllare [l'intervallo di tempo del](payment-thresholds-methods-timeframes.md) ciclo di pagamento e capire quando gli utili devono essere visualizzati nell'estratto conto.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Perché l'importo degli utili è diverso da quello previsto?

- Se l'ordine è stato parzialmente pagato dal cliente, l'importo del guadagno sarà basato sull'importo parzialmente pagato dopo la detrazione della tariffa e dell'imposta appropriata.
- Controllare la responsabilità di rimessa fiscale in base al paese. Nei paesi in cui l'imposta è responsabile di Microsoft, Microsoft raccoglie e deduce l'imposta dagli utili degli editori. L'importo della transazione indicato nell'estratto non include l'importo delle tasse. Vedere [Dettagli imposte](tax-details-marketplace.md).
- Le offerte SaaS e IaaS hanno una tariffa di agenzia scontata al 10% anziché al 20% standard, lasciando un tasso di utili del 90%. Si tratta di un requisito Co-Sell IP. Questa promozione è valida fino al 30 giugno 2021. 

**Altre informazioni:** Commercial Marketplace Publisher Agreement , [Payout policy details](payout-policy-details.md), Payment [threshold, method, and time frame](payment-thresholds-methods-timeframes.md), Getting [paid](marketplace-get-paid.md), [Tax](/legal/marketplace/msft-publisher-agreement) [details](tax-details-marketplace.md), [Payout Statements](payout-statement.md)

## <a name="earnings-reconciliation"></a>Riconciliazione degli utili

### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Come risolvere le differenze tra l'estratto conto e i report sugli ordini o sull'utilizzo nell'analisi?

Usare AssetID, orderID e l'ID voce visualizzati nel report della cronologia delle transazioni di pagamento con ordini analitici e report sull'utilizzo. Usare questo mapping:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Come fare per sapere quando si riceveranno i pagamenti per gli ordini dei clienti?

- In primo luogo, usando l'assetID, controllare gli ordini dei clienti nei [report degli ordini](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Controllare il canale del cliente per la sottoscrizione del cliente [nel report dei clienti.](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)
- Per i clienti aziendali, gli utili dell'editore vengono visualizzati nel rendiconto 1-2 giorni dopo la data dell'ordine di acquisto.
- Per i clienti non aziendali, gli utili dell'editore vengono visualizzati nel rendiconto 1-2 giorni dopo la ricezione del pagamento da parte del cliente.

**Altre informazioni:** [Rendiconti dei pagamenti,](payout-statement.md) [Dashboard ordini nell'analisi del marketplace commerciale](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payments-and-adjustments"></a>Pagamenti e rettifiche

#### <a name="why-is-my-payment-missing"></a>Perché manca il pagamento?

- Verificare che lo stato dei pagamenti e lo stato del profilo fiscale siano visualizzati *come validi* nella pagina [di panoramica](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- È possibile che non sia stata raggiunta la soglia minima per il pagamento. Per ricevere un pagamento l'importo deve essere di almeno 50 USD.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Ricerca per categorie l'account per non ricevere il pagamento?
È possibile mantenere i pagamenti in [Profilo di pagamento](https://partner.microsoft.com/dashboard/commercial-marketplace/overview). A tale scopo, selezionare **Blocco** e Microsoft conservi il pagamento fino a quando non si rilascia il blocco.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Perché ricevo il pagamento in una valuta diversa rispetto alla valuta di acquisto?

La valuta del pagamento si basa sulla valuta selezionata nel profilo di pagamento. La valuta di acquisto si basa sulla valuta pagata dal cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>Come riconciliare le rettifiche?

Le rettifiche di pagamento sono correzioni del pagamento per supportare le rettifiche compensative, ad esempio problemi di sistema. Nel rendiconto dei pagamenti ReasonCode specifica il motivo della rettifica. Questi non sono destinati a riconciliare direttamente con le singole transazioni.

**Altre informazioni:** [Contratto per editori del Marketplace commerciale,](/legal/marketplace/msft-publisher-agreement) [dettagli dei criteri](payout-policy-details.md)di pagamento, dettagli [fiscali,](tax-details-marketplace.md) [soglia di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Imposte

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>In che modo è possibile identificare la responsabilità del versamento imposte tra Microsoft o l'editore nell'estratto conto?

Nel download della cronologia delle transazioni trovare la colonna del modello fiscale. Qui viene visualizzata la gestione di MS o ISV. Consultare le leggi fiscali specifiche per un paese e ciò che implicano per i pagamenti in [Dettagli imposte](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Come scaricare i moduli della tassa sul servizio?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Viene visualizzato un collegamento al modulo Tassa sul servizio per un pagamento con tassa sul servizio.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano i moduli per le tasse di fine anno?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli per le tasse di fine anno.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Come trovare la ritenuta d'acconto per una transazione?
La ritenuta d'acconto è applicabile per gli editori degli Stati Uniti che hanno inviato il modulo W-9. La ritenuta d'acconto viene calcolata sui pagamenti mensili.

**Altre informazioni:** [Contratto per editori del Marketplace commerciale,](/legal/marketplace/msft-publisher-agreement) [dettagli dei criteri di pagamento](payout-policy-details.md)

## <a name="payout-statement-access"></a>Accesso all'estratto conto

#### <a name="how-do-i-access-a-payout-statement"></a>Come si accede all'estratto conto?

1. Controllare il proprio ruolo. Per accedere all'estratto conto, è necessario avere il ruolo di *collaboratore finanziario* o *proprietario dell'account*.
2. Nel riquadro di spostamento in alto a destra selezionare **l'icona Pagamento** per visualizzare l'estratto conto. Scegliere tra **Cronologia transazioni,** **Pagamento** e **Scarica.**

**Altre informazioni:** [Ruoli e autorizzazioni per i pagamenti,](payout-statement.md#roles-and-permissions)Estratti [conto](payout-statement.md) 

## <a name="payout-statement-report"></a>Report dell'estratto conto

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Cosa significano i campi nel download della transazione?

Per [un elenco dettagliato degli](payout-statement.md) attributi e dei relativi significati, vedere l'elenco dei pagamenti.

#### <a name="what-is-earning-status"></a>Cos'è lo stato degli utili?

Gli utili vengono visualizzati come non elaborati, elaborati o inviati.

- **Non elaborato: gli** utili sono in un periodo di deposito fino alla data di scadenza.
- **Elaborato:** gli utili sono maturi e vengono preparati in un pagamento mensile. I pagamenti vengono rilasciati entro il 15 di ogni mese.
- **Inviato:** il pagamento è stato rilasciato correttamente alla banca in base al profilo di pagamento.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Come scaricare i moduli della tassa sul servizio?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Viene visualizzato un collegamento al modulo Tassa sul servizio per un pagamento con tassa sul servizio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Ricerca per categorie scaricare un modulo di ritenuta d'acconto in formato PDF?

Andare alla pagina **Payout Payment** (Pagamento dei proventi), quindi alla sezione **List of Payment** (Elenco dei pagamenti). Accanto al pagamento viene visualizzato un collegamento al modulo per la ritenuta d'acconto. Un modulo di ritenuta d'acconto si applica solo a programmi di incentivi selezionati, non a un pagamento del marketplace commerciale.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Dove si trovano i moduli per le tasse di fine anno?

Passare alla [pagina del profilo](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) per visualizzare i moduli per le tasse di fine anno.

**Altre informazioni:** [Istruzioni per i pagamenti,](payout-statement.md)Download [della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Rendiconti cronologici

#### <a name="how-do-i-view-historical-information"></a>Ricerca per categorie visualizzare informazioni cronologiche?

Nel rendiconto cronologico viene visualizzato lo snapshot dei dati di pagamento a partire da ottobre 2019. Sfortunatamente, le informazioni sui pagamenti qui non vengono aggiornate. Per ricevere le informazioni più recenti, inviare un ticket di supporto per i dati più recenti.

**Altre informazioni:** [Istruzioni per i pagamenti,](payout-statement.md)Download [della cronologia delle transazioni](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API di esportazione dei pagamenti

#### <a name="how-do-i-download-payout-data"></a>Come si possono scaricare i dati relativi ai pagamenti?

Usare [l'API Partner Payout](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="commercial-marketplace-payout-policies"></a>Criteri di pagamento del marketplace commerciale

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Come trovare l'attuale commissione dell'agenzia e la tariffa di pagamento?

- Controllare la pagina del Contratto per gli editori del Marketplace. La commissione standard dell'agenzia è il 20%. Le transazioni idonee per il co-selling SaaS hanno una tariffa scontata del 10%. Controllare gli annunci di eventuali commissioni promozionali dell'agenzia.
- Nel rendiconto dei pagamenti, Earning Rate specifica la tariffa di pagamento effettiva per una determinata transazione.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Dopo che gli utili vengono visualizzati nell'estratto quando si riceverà il pagamento da Microsoft?
- Quando gli utili sono nello stato non elaborato, è possibile controllare la data di scadenza per il mese in cui verranno elaborati per il pagamento. Una volta preparato il pagamento, lo stato di guadagno cambierà in "elaborato".  Microsoft emette i pagamenti entro il 15 del mese di scadenza.
- Per gli ordini pagati con carta di credito, Microsoft mantiene i pagamenti per 30 giorni fino alla scadenza del guadagno.

 **Altre informazioni:** [Contratto per editori del Marketplace commerciale,](/legal/marketplace/msft-publisher-agreement) [dettagli dei criteri](payout-policy-details.md)di pagamento, [dettagli](tax-details-marketplace.md)fiscali, soglia [di pagamento, metodo e intervallo di tempo](payment-thresholds-methods-timeframes.md)

## <a name="next-steps"></a>Passaggi successivi

- [Come ottenere i pagamenti](marketplace-get-paid.md)
- [Configurare l'account proventi e i moduli fiscali](set-up-your-payout-account.md)