---
title: Estratti conto
description: Informazioni sui riepiloghi e sulle istruzioni per i pagamenti e su come visualizzare ed esportare i dati di pagamento dal Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 10/29/2020
ms.openlocfilehash: 4a511dc026e3c71f05c5b18ca6d8915bd2654826
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756159"
---
# <a name="payout-statements"></a>Estratti conto

**Ruoli appropriati:**

- Amministratore degli account
- Amministratore globale

L'informativa sui **pagamenti** presenta una panoramica dei pagamenti offerti dalle offerte vendute attraverso il Marketplace commerciale. Mostra la cronologia transazionale dei tuoi guadagni, ne stima il pagamento successivo e Mostra le tendenze di pagamento. È inoltre possibile scaricare la cronologia delle transazioni e le istruzioni di pagamento. Questo articolo illustra come accedere al rendiconto dei pagamenti e le pagine di pagamento e i download disponibili nel centro per i partner.

>[!NOTE]
>Verranno visualizzati solo i dati per i programmi e gli ID MPN a cui si è associati. Se si desidera visualizzare dati aggiuntivi, rivolgersi all'amministratore dell'account per le autorizzazioni. 

## <a name="roles-and-permissions"></a>Ruoli e autorizzazioni

Per accedere a un'istruzione di pagamento, è necessario assegnare il ruolo di **proprietario dell'account** o **collaboratore finanziario** .

| Report/pagine | Proprietario dell'account | Manager | Developer | Collaboratore aziendale | Collaboratore finanza | Addetto al marketing |
| --- | --- | --- | --- | --- | --- | --- |
| Report Acquisizioni (inclusi dati quasi in tempo reale) | Può visualizzare | Può visualizzare | Nessun accesso | Nessun accesso | Può visualizzare | Nessun accesso |
| Report commenti e suggerimenti/risposte | Può visualizzare e inviare commenti e suggerimenti | Può visualizzare e inviare commenti e suggerimenti | Può visualizzare e inviare commenti e suggerimenti | Nessun accesso | Nessun accesso | Può visualizzare e inviare commenti e suggerimenti |
| Report sull'integrità (inclusi dati quasi in tempo reale) | Può visualizzare | Può visualizzare | Può visualizzare | Può visualizzare | Nessun accesso | Nessun accesso |
| Report sull'utilizzo | Può visualizzare | Può visualizzare | Può visualizzare | Può visualizzare | Nessun accesso | Nessun accesso |
| Account proventi | Può aggiornare | Nessun accesso | Nessun accesso | Nessun accesso | Può aggiornare | Nessun accesso |
| Profilo fiscale | Può aggiornare | Nessun accesso | Nessun accesso | Nessun accesso | Può aggiornare | Nessun accesso |
| Riepilogo proventi | Può visualizzare | Nessun accesso | Nessun accesso | Nessun accesso | Può visualizzare | Nessun accesso |
|

## <a name="access-your-payout-statement"></a>Accedere all'istruzione di pagamento

Accedere al centro per i [partner](https://partner.microsoft.com/dashboard/home) e selezionare l'icona di pagamento nell'angolo superiore destro della schermata per accedere a questi riepiloghi diversi:

- Cronologia delle transazioni
- Pagamenti
- Esportazione dei dati

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Viene illustrata l'icona del payout nell'angolo superiore destro del portale del centro per i partner":::

È anche possibile usare l' [API](https://apidocs.microsoft.com/services/partnerpayouts) per i pagamenti dei partner per connettersi e ottenere direttamente i dati relativi a transazioni e pagamenti dei pagamenti.


## <a name="transaction-history"></a>Cronologia delle transazioni

Nella pagina **Cronologia transazioni** viene visualizzato il riepilogo dei tuoi guadagni, il pagamento stimato successivo e la tendenza per i guadagni e i pagamenti negli ultimi 36 mesi. È anche possibile scaricare i dettagli delle transazioni da questa sezione.


:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Cenni preliminari sulle transazioni.":::

- I guadagni sono stati **inviati quest'anno** , ovvero i guadagni totali e la ripartizione dei guadagni pagati e verranno pagati nel mese successivo.
- **Mese di pagamento stimato** : i guadagni totali previsti nei mesi successivi.
- **Guadagni e tendenza ai pagamenti** : importi mensili per guadagni e pagamenti per gli ultimi 36 mesi.
- **Download** : scaricare i dettagli della transazione nel formato CSV o TSV.

Utilizzare la selezione dell'intervallo di date nell'angolo superiore destro della pagina per filtrare l'output della pagina in modo da visualizzare gli ultimi 3, 6, 12 o 36 mesi. In alternativa, selezionare un intervallo di date personalizzato fino a 36 mesi. L'intervallo di date predefinito è 12 mesi. È anche possibile filtrare in base all'ID di registrazione, al programma, all'ID di pagamento, al tipo di guadagno, alla leva e allo stato. I dati sono disponibili per l'anno fiscale corrente (1 luglio-30 giugno) e i due anni fiscali precedenti.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Il filtro di ricerca nella parte superiore destra della pagina.":::

Per visualizzare altri dettagli sugli utili, selezionare la freccia rivolta verso il basso sul lato destro della pagina. In questo modo, vengono visualizzati la leva, l'importo dei ricavi, il prodotto e il cliente. Se per qualche motivo uno di questi dati non è disponibile, ma è necessario accedervi, contattare il supporto tecnico. Se il guadagno è il risultato di una modifica e non di una transazione, i campi prodotto e cliente non verranno visualizzati.

### <a name="transaction-history-summary"></a>Riepilogo cronologia transazioni

In questo esempio vengono visualizzati i dettagli, tra cui l'origine del guadagno ottenuto dal prodotto che ha venduto le date, lo stato e il mese di pagamento stimato.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Cronologia delle transazioni.":::

- **Data** di acquisto: data di acquisto.
- **Tipo di guadagno** : il tipo di guadagno, ad esempio vendita, sconto o co-op.
- **Importo totale** : importo del guadagno netto. Nel Marketplace commerciale, ciò significa che dopo la deduzione della tariffa del Marketplace standard.
- **Stato** : è costituito da tre opzioni:
    - **Imminente** : i guadagni sono in attesa di un periodo di raffreddamento.
    - **Elaborati** : i guadagni sono preparati per il pagamento successivo.
    - **Inviati** : i guadagni sono stati pagati.
- **Mese di pagamento stimato** : il mese in cui si prevede di pagare i guadagni. Per ulteriori informazioni, vedere la [sezione successiva](#estimated-payment-month) .

I guadagni delle transazioni vengono visualizzati quando la transazione soddisfa l'idoneità per i pagamenti. Per comprendere il motivo per cui si potrebbero ottenere guadagni mancanti o imprevisti, vedere [domande comuni sui pagamenti di Marketplace commerciali](payout-faq.md#why-are-my-earnings-missing).

#### <a name="estimated-payment-month"></a>Mese di pagamento stimato

La pagina Cronologia transazioni include ora una tabella che Mostra gli importi di pagamento stimati per i mesi successivi. È inoltre possibile visualizzare e scaricare queste informazioni nelle esportazioni della cronologia delle transazioni e dei report riepilogativi. Queste informazioni rendono più semplice la riconciliazione e le proiezioni di pagamento.

Il mese di pagamento stimato viene calcolato in base alle regole e alle sequenze temporali di configurazione del programma e viene elaborato nel ciclo di pagamento successivo o imminente.

Il mese di pagamento stimato è attualmente disponibile per tutti i tipi di guadagno eccetto co-op, che verrà visualizzato come **non applicabile**. Per i guadagni prima del 1 ° luglio 2020, il mese di pagamento stimato verrà visualizzato come **non disponibile**.

La tabella seguente mostra un esempio di mese di pagamento stimato.

| Month | Amount |
| ------ | :-----------: |
|  Sep-2020 |  $7.273,99   |
|  Ottobre-2020 | $8.692,30  |
|  Novembre 2020 | $107,89  |

L'importo stimato può variare rispetto all'importo effettivo per diversi motivi:

- Acquisizione della ripubblicazione: se i guadagni vengono ricalcolati, la quantità effettiva sarà diversa
- Rettifiche: l'importo effettivo varia in base alle rettifiche che si sono verificate o sono state inviate.
- Modifica delle regole: una modifica nelle regole può riflettere il ricalcolo della quantità effettiva a pagamento
- Pagabile: se si verifica un errore di pagamento, l'importo effettivo potrebbe essere diverso

Si noti che il pagamento viene rilasciato nel mese previsto solo se vengono soddisfatte le regole di idoneità per il pagamento e la soglia del programma. Queste regole includono ma non sono limitate all'elenco seguente:

- Il profilo fiscale deve essere aggiornato
- È necessario che i guadagni soddisfino o superino la soglia minima di guadagno definita nella guida del programma.
- Pagamento in attesa: se si seleziona l'opzione "Mantieni il pagamento" nella pagina Assegnazione profili.
- Lo strumento di pagamento non è disponibile: il pagamento o/e il profilo fiscale non sono completati.

### <a name="transaction-history-download"></a>Download cronologia transazioni

Per visualizzare altri dettagli su un guadagno, selezionare **download** nella parte superiore della pagina. Nella tabella seguente viene illustrata ogni colonna del report.

>[!NOTE]
>L'esportazione di download della cronologia delle transazioni include due nuovi campi a partire dal 2020 agosto:
>
>- **lastPaymentCurrency**  La valuta in cui è stato ricevuto il pagamento più recente, in tutte le MPNs a cui il partner attualmente connesso ha accesso. Se non viene ricevuto alcun pagamento, la valuta dell'ultimo pagamento sarà di dollari statunitensi.
>- **earningAmountInLastPaymentCurrency**  Importo guadagnato nell'ultima valuta di pagamento.

| Nome colonna | Descrizione | Applicabilità per programmi incentive/marketplace |
| --- | --- | --- |
| agreementEndDate | Data di fine del contratto | Incentivi: solo alcuni programmi |
| agreementNumber | Numero del contratto | Incentivi: solo alcuni programmi |
| agreementStartDate | Data di inizio del contratto | Incentivi: solo alcuni programmi |
| calculationDate | Data di calcolo del reddito nel sistema | Tutti |
| claimId | Identificatore univoco per l'attestazione | Incentivi: solo alcuni programmi |
| customerCountry | Paese/Area geografica del cliente | marketplaces |
| customerEmail |  |  |
| customerName | Può essere vuoto | Solo per i programmi incentive (eccezione: OEM) e Marketplace. Per le transazioni CSP, i Marketplace visualizzeranno il nome del CSP |
| customerTenantId |  |  |
| distributorId | Identificatore del distributore | Incentivi: solo alcuni programmi |
| distributorName | Nome del distributore | Incentivi: solo alcuni programmi |
| earningAmount | Importo del reddito nella valuta della transazione originale | Tutti |
| earningAmountInLastPaymentCurrency | Importo del reddito nell'ultima valuta di pagamento. Il campo sarà vuoto se non sono stati corrisposti pagamenti precedenti. |  |
| earningAmountUSD | Importo del reddito in dollari statunitensi | Tutti |
| earningDate | Data del reddito | Tutti |
| earningExchangeRate | Tasso di cambio usato per visualizzare l'importo corrispondente in dollari statunitensi | Tutti |
| earningId | Identificatore univoco per ogni reddito | Tutti |
| earningRate | Frequenza degli incentivi applicata alla quantità di transazioni per generare un guadagno | Tutti |
| earningType | Indica se si tratta di corrispettivi, sconti, co-op, vendite e così via | Tutti |
| exchangeRateDate | Data del tasso di cambio usata per calcolare il valore in dollari statunitensi di EarningAmount | Tutti |
| externalReferenceId | Identificatore univoco per il programma | Programmi a pagamento diretto (incentivi e Marketplace) |
| externalReferenceIdLabel | Etichetta identificatore univoco | Programmi a pagamento diretto (incentivi e Marketplace) |
| instantRebateAmount |  |  |
| DataFattura |  |  |
| invoiceNumber | Numero fattura (applicabile solo per Enterprise) | Incentivi e Marketplace: solo alcuni programmi |
| lastPaymentCurrency | Ultima valuta di pagamento. Il campo sarà vuoto se non sono stati corrisposti pagamenti precedenti. |  |
| lever | Indica la regola di business per il reddito | Tutti |
| LicensingProgramName | Nome del programma di licenza |  |
| LineItemId | Singola voce nella fattura di un cliente |  |
| localProviderSeller | Fornitore/gestore del sistema di pagamento locale |  |
| Mese maturità | Mese di pagamento stimato | Tutti |
| OrderId | Si riferisce alla fattura di un cliente  | marketplaces |
| parentProductId | Identificatore univoco del prodotto padre. Se non è presente un prodotto padre per la transazione, l'ID del prodotto padre coincide con l'ID del prodotto. | marketplaces |
| parentProductName | Nome del prodotto padre. Se non è presente un prodotto padre per la transazione, il nome del prodotto padre coincide con il nome del prodotto. | marketplaces |
| participantId | Identità principale del partner che realizza un reddito nell'ambito del programma | Tutti |
| participantIdType | Per la maggior parte dell'ID programma per incentivare i programmi e il venditore se per i Marketplace | Tutti |
| participantName | Nome del partner beneficiario del reddito | Tutti |
| partnerCountryCode | Località/paese/area del partner beneficiario del reddito | Tutti |
| partNumber | È sempre vuoto | Alcuni programmi e Marketplace per incentivi |
| paymentId | Identificatore univoco per il pagamento. Questo numero è visibile nell'estratto conto bancario | Solo pagamenti SAP |
| paymentStatus | Stato dei pagamenti | Tutti |
| paymentStatusDescription | Descrizione dello stato dei pagamenti | Tutti |
| productId | Identificatore univoco del prodotto | marketplaces |
| productName | Nome del prodotto correlato alla transazione | Tutti |
| productType | Tipo di prodotto, ad esempio app, componente aggiuntivo o gioco | marketplaces |
| Codice programma | Stringa da associare al nome del programma |  |
| programName | Nome del programma Incentive/Store | Tutti |
| purchaseOrderCoverageEndDate | È sempre vuoto | Programma Incentive: elemento del report personalizzato |
| purchaseOrderCoverageStartDate | È sempre vuoto | Programma Incentive: elemento del report personalizzato |
| purchaseOrderType | È sempre vuoto | Programma Incentive: elemento del report personalizzato |
| purchaseTypeCode | È sempre vuoto | Programma Incentive: elemento del report personalizzato |
| quantity | Varia in base al programma. Indica la quantità fatturata per i programmi transazionali | Tutti |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identificatore del rivenditore | Incentivi: solo alcuni programmi |
| resellerName | Nome del rivenditore |  |
| SkuId | ID SKU come definito durante la pubblicazione. Un'offerta può includere molti SKU, ma uno SKU può essere associato solo a una singola offerta. Incentivi: solo alcuni programmi |  |
| storeFee | Importo trattenuto da Microsoft come corrispettivo per rendere disponibile l'app o il componente aggiuntivo nello Store | marketplaces |
| subscriptionEndDate | Data di fine della sottoscrizione | Incentivi: solo alcuni programmi |
| subscriptionId | Identificatore della sottoscrizione associata al cliente | Incentivi: solo alcuni programmi |
| subscriptionStartDate | Data di inizio della sottoscrizione | Incentivi: solo alcuni programmi |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Parte responsabile del versamento delle imposte (vendite, utilizzo o IVA/GST) | marketplaces |
| taxRemitted | Importo delle imposte versate (vendite, utilizzo o IVA/GST) | marketplaces |
| taxState | Stato/Provincia del cliente |  |
| taxZipCode | CAP/Codice postale del cliente |  |
| tpan | Indica la rete pubblicitaria di terze parti | solo annunci Marketplace |
| transactionAmount | Importo della transazione nella valuta della transazione originale in base a cui vengono generati gli utili | Tutti |
| transactionAmountUSD | Importo della transazione in dollari statunitensi (USD) | Tutti |
| transactionCountryCode | Codice paese/area geografica in cui è avvenuta la transazione |  |
| transactionCurrency | Valuta in cui è avvenuta la transazione originale del cliente (non si tratta della valuta locale del partner) | Tutti |
| transactionDate | Data della transazione. Utile per i programmi in cui un reddito è il risultato di più transazioni. | Tutti |
| transactionExchangeRate | Data del tasso di cambio usato per visualizzare l'importo in dollari statunitensi della transazione corrispondente | Tutti |
| transactionId | Identificatore univoco della transazione | Tutti |
| transactionPaymentMethod | Strumento di pagamento del cliente usato per la transazione, ad esempio carta di credito, fatturazione operatore di telefonia mobile o PayPal | marketplaces |
| transactionType | Tipo di transazione, ad esempio acquisto, rimborso, storno o rifiuto di addebito | marketplaces |
| workload | Carico di lavoro | Incentivi: solo alcuni programmi |
|

### <a name="transaction-adjustment-codes"></a>Codici di regolazione delle transazioni

Nella tabella seguente sono elencati i codici motivo per le rettifiche e le relative descrizioni.

|**Codice motivo**   |**Descrizione**   |
|------------------|:-------------------------------------|
| Conformità AR | Regolazione che riduce i guadagni quando le fatture Microsoft non vengono pagate nel tempo dal partner. |
| Rollover co-op | Regolazione che trasferisce i guadagni della co-op a un altro periodo oppure converte i guadagni della co-op per lo sconto. |
| Regolazione Ops | Regolazione che corregge gli errori di calcolo del sistema Microsoft. |
| Regolazione Ops Microsoft calcolo non corretto | Regolazione che corregge i calcoli errati. |
| Regolazione Ops Microsoft registrazione non corretta | Regolazione degli errati calcoli relativi alla registrazione. |
| Mapping partner (sottoscrizione) MCI/CSP | Regolazione che corregge il errato allineamento della sottoscrizione. |
| Eccezione dei criteri | Regolazione che sostituisce una regola di programma.  |
| Guadagni del periodo precedente | Rettifica per i guadagni al di fuori del periodo di guadagno corrente. |

## <a name="payments"></a>Pagamenti

La pagina dei **pagamenti** descrive in dettaglio il denaro guadagnato con Microsoft. Indica anche quando e quanto verrà pagato.

>[!Note]
> Per poter beneficiare del pagamento, gli introiti devono raggiungere la [soglia di pagamento](payment-thresholds-methods-timeframes.md) di 50 dollari statunitensi. Per ulteriori informazioni, vedere il [contratto di Microsoft Publisher](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Schermata di panoramica dei pagamenti.":::

- **Totale pagato quest'anno** : il totale combinato pagato all'anno, in dollari statunitensi, per tutti i programmi.
- **Successivo pagamento stimato** : il singolo pagamento successivo (anche se ne saranno disponibili altri presto), in dollari statunitensi.
- **Ultimo pagamento** : la quantità (in dollari statunitensi), il nome del programma e il programma del pagamento più recente.
- **Pagamento in base all'origine** : quantità di pagamenti (in dollari statunitensi) per programma negli ultimi 12 mesi.

### <a name="payments-list"></a>Elenco pagamenti

La tabella **List of Payments** Mostra i pagamenti a pagamento e in sospeso. È possibile scaricare le informazioni fiscali sui costi del servizio in formato PDF e visualizzare i dettagli relativi a un determinato pagamento.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Esporta cronologia transazioni":::

- A **pagamento** : tutti i pagamenti sono stati inviati correttamente. Scegliere l'anno nel menu a discesa per filtrare i pagamenti rilasciati nell'anno.
- **In sospeso** : pagamenti imminenti.
- Tassa di **servizio (modulo PDF)** : disponibile per i pagamenti soggetti a tassa di tassa di servizio. Le tasse per la tariffa del servizio sono indicate in **altre imposte**.
- **View** : reindirizza alla cronologia delle transazioni con un elenco di guadagni inclusi nel pagamento.

Per comprendere il motivo per cui si potrebbero ottenere guadagni mancanti o imprevisti, vedere [domande comuni sui pagamenti di Marketplace commerciali](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Stato dei pagamenti

La tabella seguente illustra i diversi Stati di guadagno.

| Stato degli utili | Motivo | È richiesta un'azione del partner? |
| --- | --- | --- |
| Non elaborato | Gli utili non sono idonei al pagamento. Rimane in questo stato per un periodo di raffreddamento come definito nella Guida al programma per il programma incentives. | No |
| In programma | Ordine di pagamento generato in attesa di revisioni interne prima dell'elaborazione del pagamento. | No |
| Pending tax invoice (Fattura fiscale in sospeso) | La fattura dell'imposta è incompleta o non valida. | È necessario aggiornare la fattura fiscale prima di poter essere pagati. |
| Rejected during review (Rifiutato durante la revisione) | Il pagamento è stato rifiutato durante la revisione. | Per informazioni dettagliate, contattare il supporto tecnico Microsoft. |
| Non riuscito | Il pagamento non è riuscito a causa di un errore di sistema Microsoft. | Per ulteriori informazioni, contattare il supporto tecnico Microsoft |
| In corso | Il pagamento è in corso. | No |
| Pagamento non corretto | È in corso il recupero dei pagamenti. | No |
| Inviato | Il pagamento è stato inviato alla banca. | No |
| Reprocessing (Rielaborazione) | Il pagamento ha rilevato un errore di sistema Microsoft e viene rielaborato. | No |
| Reversed | Il pagamento è stato invertito dalla banca e verrà inviato di nuovo al successivo ciclo di pagamento. | No |
| Tax invoice rejected (Fattura fiscale rifiutata) | La fattura fiscale è stata rifiutata durante la revisione. Tutti i pagamenti in sospeso rimarranno in attesa fino al completamento della revisione della fattura fiscale. | Per ulteriori informazioni, contattare il supporto tecnico Microsoft |
| Tax invoice under review (Fattura fiscale in revisione) | È in corso la revisione della fattura fiscale. Il pagamento verrà rilasciato una volta che la fattura fiscale è stata approvata. | No |
| Rifiutato | Il pagamento è stato rifiutato dalla banca. | Per informazioni dettagliate, contattare la banca. |
|

### <a name="payments-download"></a>Download dei pagamenti

 Nella tabella seguente viene illustrata ogni colonna del report. Per visualizzare altri dettagli relativi ai pagamenti, fare clic su **download** nella parte superiore della pagina pagamenti.

| Nome colonna | Descrizione |
| --- | --- |
| participantID | Identità principale del partner che realizza un reddito nell'ambito del programma |
| participantIDType | In genere ID programma per incentivi programmi e ID venditore per i programmi di Store |
| participantName | Nome del partner beneficiario del reddito |
| programName | Incentivi/nome del programma di archiviazione |
| earned | Importo guadagnato nella valuta di pagamento per l'ID programma/participante |
| earnedUSD | Importo guadagnato per l'ID programma/participante, in dollari statunitensi |
| withheldTax | Importo delle imposte in valuta di pagamento per l'ID programma/participante |
| salesTax | Importo totale delle imposte sulle vendite in valuta per il programma/participantID (applicabile solo ai programmi per gli incentivi) |
| serviceFeeTax | Quantità totale di serviceFeeTax in valuta di pagamento per l'ID programma/participante (applicabile solo per i programmi Store e Azure Marketplace) |
| totalPayment | Pagamento totale in valuta locale, al netto di tutte ritenute e al lordo dell'imposta sulle vendite (se applicabile) per l'ID programma/participante |
| currencyCode | Codice della valuta di pagamento |
| paymentMethod | Metodo utilizzato per pagare il partner, ad esempio, bonifico bancario o nota di credito |
| paymentID | Identificatore univoco per il pagamento. Questo numero è in genere visibile nel rendiconto bancario (applicabile solo ai pagamenti SAP). |
| paymentStatus | Stato dei pagamenti |
| paymentStatusDescription | Descrizione descrittiva dello stato dei pagamenti |
| paymentDate | Data del pagamento inviato da Microsoft |
|

## <a name="export-data"></a>Esportazione dei dati

La pagina **Esporta dati** non viene aggiornata autonomamente. Per visualizzare i dati più recenti, potrebbe essere necessario aggiornare la pagina manualmente. Selezionare una delle tre schede per esportare la **cronologia delle transazioni**, i **pagamenti**, il **Riepilogo delle transazioni** o l' **istruzione cronologica**.

Il filtro potrebbe causare un errore di **Nessun dato disponibile** . Questo problema può verificarsi se il periodo di tempo predefinito è stato selezionato a tre mesi, quindi è stato selezionato un ID di pagamento da un guadagno che esula da tale periodo. In tal caso, espandere il periodo di tempo e riprovare.

Ecco un esempio di esportazione dei pagamenti:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Report di esportazione dei pagamenti.":::

### <a name="historical-statements"></a>Rendiconti cronologici

Il riepilogo **dei dati di esportazione** fornisce anche l'accesso alle istruzioni cronologiche.

> [!NOTE]
> Un'istruzione cronologica è uno snapshot e non viene aggiornata. Se necessario, contattare il [supporto tecnico](https://partner.microsoft.com/support/v2/?stage=1) e richiedere i dati più recenti.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Esporta istruzioni cronologiche.":::

- La cronologia delle transazioni precedente al 1 ° luglio 2019 viene gestita separatamente e utilizza campi diversi dai report di cronologia successivi.
- La cronologia delle transazioni legacy include una colonna denominata "riservata" che corrisponde alla colonna "guadagni" nella cronologia moderna, ad eccezione del fatto che esclude tutti i guadagni con stato uguale a "pagamento inviato".
- Filtri come 3M, 6M o 12M, non si applicano alla sezione dei rendiconti cronologici.

### <a name="historical-statement-downloads"></a>Download di istruzioni cronologiche

La tabella seguente illustra ogni colonna in un'istruzione cronologica.

| Nome campo | Descrizione |
| --- | --- |
| Origine dei ricavi | Origine dei ricavi in base a dove si è verificata la transazione, ad esempio Microsoft Store, Windows Phone Store, Windows 8 Store o Microsoft Advertising |
| ID dell'ordine | Identificatore univoco dell'ordine. Questo ID consente di identificare le transazioni di acquisto con le rispettive transazioni non di acquisto, ad esempio rimborsi o chargeback. Entrambe avranno lo stesso ID ordine. Se, inoltre, è presente un addebito suddiviso in cui sono stati usati più metodi di pagamento per un singolo acquisto, è possibile collegare le transazioni di acquisto. |
| TransactionID | Identificatore univoco della transazione. |
| Data/ora della transazione | Data e ora in cui si è verificata la transazione (UTC). |
| ID prodotto padre | Identificatore univoco del prodotto padre. Se non è presente un prodotto padre per la transazione, l'ID del prodotto padre coincide con l'ID del prodotto. |
| Product ID | Identificatore univoco del prodotto. |
| Nome prodotto padre | Nome del prodotto padre. Se non è presente un prodotto padre per la transazione, il nome del prodotto padre coincide con il nome del prodotto. |
| Nome prodotto | Nome del prodotto |
| Tipo prodotto | Tipo di prodotto, ad esempio app, componente aggiuntivo o gioco |
| Quantità | Quando l'origine dei ricavi è Microsoft Store per le aziende, la quantità corrisponde al numero di licenze acquistate. Per tutte le altre origini, la quantità è sempre pari a 1. Anche se una singola transazione viene suddivisa in due voci, perché sono stati utilizzati due metodi di pagamento diversi, ogni voce indica una quantità pari a 1. |
| Tipo di transazione | Tipo di transazione, ad esempio acquisto, rimborso, storno o rifiuto di addebito |
| Metodo di pagamento | Strumento di pagamento del cliente usato per la transazione, ad esempio carta di credito, fatturazione operatore di telefonia mobile o PayPal |
| Paese/Area | Paese/Area geografica in cui risiedono i dati |
| Provider/venditore locale | Provider/venditore locale del record |
| Valuta transazione | Valuta della transazione |
| Importo transazione | Importo della transazione |
| Imposte versate | Importo delle imposte versate (vendite, utilizzo o IVA/GST) |
| Entrate nette | Importo della transazione al netto delle imposte versate |
| Corrispettivi per lo Store | Percentuale delle entrate nette trattenuta da Microsoft come corrispettivo per rendere disponibile l'app o il componente aggiuntivo nello Store |
| Guadagno sull'app | Entrate nette meno corrispettivi per lo Store |
| Imposte trattenute | Importo dell'imposta sul reddito trattenuta (non incluso nel file CSV **riservato**) |
| Payment | Guadagno sull'app al netto di qualsiasi ritenuta d'acconto applicabile (importo indicato nella valuta della transazione). Non incluso nel file CSV **riservato**. |
| Tasso di cambio | Tasso di cambio utilizzato per convertire la valuta della transazione in valuta di pagamento |
| Valuta del pagamento | Valuta in cui viene effettuato il pagamento |
| Pagamento convertito | Importo del pagamento convertito in valuta di pagamento in base al tasso di cambio |
| Modello versamento imposte | Parte responsabile del versamento delle imposte (vendite, utilizzo o IVA/GST) |
| Data/ora di idoneità | La data e l'ora in cui i proventi della transazione diventano idonei per il pagamento (UTC). Quando viene creato un pagamento, vengono inclusi i proventi della transazione con data e ora di idoneità prima della data di creazione del pagamento (inclusa solo nel file CSV **riservato**). |
| Charges | Mostra una suddivisione di tutti i dettagli dell'addebito aggregati nella colonna Importo transazione (incluso solo per Azure Marketplace; non incluso nel file CSV **riservato**). |
|||

## <a name="next-steps"></a>Passaggi successivi

- [API di pagamento dei partner](https://apidocs.microsoft.com/services/partnerpayouts)
- [Dettagli dei criteri dei proventi](payout-policy-details.md)
- Per il supporto sulla fatturazione, contattare il [supporto per gli editori](https://partner.microsoft.com/support/v2/?stage=1) del marketplace commerciale.
