---
title: Estratti conto
description: Informazioni su estratti conto e riepiloghi e su come visualizzare ed esportare i dati di pagamento da Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: dc0c720544f4a8a3c95e5b91ec656e65dbce7c80
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276111"
---
# <a name="payout-statements"></a>Estratti conto

**Ruoli appropriati:** amministratore account | Amministratore globale

**L'estratto conto** presenta una panoramica dei pagamenti delle offerte vendute tramite il marketplace commerciale. Mostra la cronologia transazionale degli utili, stima il pagamento successivo e mostra le tendenze di pagamento. È anche possibile scaricare la cronologia delle transazioni e gli estratti conto di pagamento. Questo articolo illustra come accedere all'estratto conto e alle diverse pagine e download dei pagamenti accessibili in Partner Center.

>[!NOTE]
>Verranno visualizzati solo i dati per gli ID MPN e i programmi a cui si è associati. Per visualizzare dati aggiuntivi, contattare l'amministratore dell'account per le autorizzazioni. 

## <a name="roles-and-permissions"></a>Ruoli e autorizzazioni

Per accedere a un estratto conto, è necessario avere il ruolo Di proprietario **dell'account** o **Collaboratore** finanziario.

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

## <a name="access-your-payout-statement"></a>Accedere all'estratto conto

Accedere a [Partner Center](https://partner.microsoft.com/dashboard/home) e selezionare l'icona dei pagamenti nell'angolo superiore destro della schermata per accedere a questi riepiloghi diversi:

- Cronologia delle transazioni
- Pagamenti
- Esportare i dati

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustra l'icona Proventi nell'angolo superiore destro del portale del Centro per i partner.":::

È anche possibile usare [l'API Partner Payout](https://apidocs.microsoft.com/services/partnerpayouts) per connettersi e ottenere direttamente i dati di transazione e pagamento dei pagamenti.


## <a name="transaction-history"></a>Cronologia delle transazioni

La **pagina Cronologia transazioni** mostra il riepilogo degli utili, il pagamento successivo stimato e la tendenza degli utili e dei pagamenti negli ultimi 36 mesi. È anche possibile scaricare i dettagli delle transazioni da questa sezione.<br><br>Questo report mostra tutti gli utili idonei per i proventi, inclusi i pagamenti non ancora inviati. Gli utili sono idonei per il pagamento quando un ISV ha completato tutte le informazioni bancarie e fiscali in Partner Center, ha ottenuto >$ 50, l'account ISV è attivo e il cliente è stato fatturato (per le transazioni EA) o il pagamento è stato ricevuto (per le transazioni non EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Panoramica delle transazioni.":::

- **Utili inviati quest'anno:** utili totali e scomposizione degli utili che sono stati pagati e che verranno pagati nel mese successivo.
- **Mese di pagamento stimato:** gli utili totali previsti nei prossimi mesi.
- **Andamento degli utili e dei** pagamenti: utili mensili e importi dei pagamenti per gli ultimi 36 mesi.
- **Download:** scaricare i dettagli della transazione .csv o TSV.

Usare la selezione dell'intervallo di date nell'angolo superiore destro della pagina per filtrare l'output della pagina in modo da visualizzare gli ultimi 3, 6, 12 o 36 mesi. In caso contrario, selezionare un intervallo di date personalizzato fino a 36 mesi. L'intervallo di date predefinito è 12 mesi. È anche possibile filtrare in base a ID registrazione, programma, ID pagamento, tipo di reddito, leve e stato. I dati sono disponibili per l'anno fiscale corrente (1 luglio - 30 giugno) e per i due anni fiscali precedenti.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Filtro di ricerca in alto a destra nella pagina.":::

Per visualizzare altri dettagli sugli utili, selezionare la freccia rivolta verso il basso sul lato destro della pagina. In questo modo verranno visualizzati la leve, l'importo dei ricavi, il prodotto e il cliente. Se per qualche motivo uno di questi dati non è disponibile, ma è necessario accedervi, contattare il supporto tecnico. Se il reddito è il risultato di una rettifica e non di una transazione, i campi Product e Customer non verranno visualizzati.

### <a name="transaction-history-summary"></a>Riepilogo della cronologia delle transazioni

Questa visualizzazione mostra i dettagli relativi ai ricavi, tra cui l'origine dei ricavi dal prodotto venduto, le date di guadagno, lo stato e il mese di pagamento stimato.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Cronologia delle transazioni.":::

- **Data di acquisto:** data di acquisto.
- **Tipo di reddito:** tipo di reddito, ad esempio Sell, Rebate o Co-op.
- **Importo totale:** importo netto del guadagno. Nel marketplace commerciale ciò significa che dopo aver detratto la tariffa del marketplace standard.
- **Stato:** ha tre opzioni:
    - **Imminente:** gli utili sono nel periodo di raffreddamento in sospeso.
    - **Elaborato:** gli utili vengono preparati per il pagamento successivo.
    - **Inviato:** gli utili sono stati pagati.
- **Mese di pagamento stimato:** mese previsto per il pagamento degli utili. Per altre [informazioni, vedere](#estimated-payment-month) la sezione successiva.

Le transazioni di guadagno vengono visualizzate quando la transazione soddisfa l'idoneità per i pagamenti. Per comprendere perché si potrebbero avere utili mancanti o imprevisti, vedere Domande comuni sui proventi del [marketplace commerciale.](payout-faq.md#why-are-my-earnings-missing)

#### <a name="estimated-payment-month"></a>Mese di pagamento stimato

La pagina Cronologia transazioni include ora una tabella che mostra gli importi di pagamento stimati per i prossimi mesi. È anche possibile visualizzare e scaricare queste informazioni nelle esportazioni del report Cronologia transazioni e Riepilogo. Queste informazioni semplificano le riconciliazione e le proiezioni di pagamento.

Il mese di pagamento stimato viene calcolato in base alle regole di configurazione del programma e alle sequenze temporali e viene elaborato nel ciclo di pagamento successivo/successivo.

Il mese di pagamento stimato è attualmente disponibile per tutti i tipi di guadagno, ad eccezione della co-op, che verrà visualizzato **come Non applicabile.** Per gli utili prima del 1° luglio 2020, il mese di pagamento stimato verrà visualizzato **come Non disponibile.**

La tabella seguente illustra un esempio di mese di pagamento stimato.

| Month | Amount |
| ------ | :-----------: |
|  Settembre 2020 |  $7.273,99   |
|  Ottobre 2020 | $8.692,30  |
|  Novembre 2020 | $107,89  |

L'importo stimato può variare dall'importo effettivo per diversi motivi:

- Riestatement dei ricavi: se gli utili vengono ricalcolati, l'importo effettivo sarà diverso
- Rettifiche: l'importo effettivo varia a seconda delle rettifiche che si sono verificate o sono state inviate.
- Modifica delle regole: una modifica delle regole può riflettere il ricalcolo dell'importo effettivo pagato
- Da pagare: se si verifica un errore di pagamento, l'importo effettivo potrebbe essere diverso

Si noti che il pagamento viene rilasciato solo nel mese proiettato se vengono soddisfatte le regole di soglia e di idoneità al pagamento del programma. Queste regole includono ma non sono limitate all'elenco seguente:

- Il profilo fiscale deve essere aggiornato
- Gli utili devono soddisfare o superare la soglia minima di guadagno definita nella guida al programma.
- Pagamento in attesa: se si seleziona l'opzione "Mantieni pagamento" nella pagina di assegnazione dei profili.
- Strumento di pagamento non disponibile: il pagamento o/e il profilo fiscale non sono stati completati.

### <a name="transaction-history-download"></a>Download della cronologia delle transazioni

Per visualizzare altri dettagli su un guadagno, selezionare **Scarica** nella parte superiore della pagina. Nella tabella seguente viene illustrata ogni colonna del report.

>[!NOTE]
>L'esportazione del download della cronologia delle transazioni include due nuovi campi a partire da agosto 2020:
>
>- **lastPaymentCurrency**  Valuta in cui è stato ricevuto il pagamento più recente, in tutti i mpn a cui il partner attualmente connesso ha accesso. Se non viene ricevuto alcun pagamento, l'ultima valuta di pagamento sarà in dollari STATUNITENSI.
>- **earningAmountInLastPaymentCurrency**  Importo di guadagno nell'ultima valuta di pagamento.

| Nome colonna | Descrizione | Applicabilità per programmi di incentivi/marketplace |
| --- | --- | --- |
| agreementEndDate | Data di fine del contratto | Incentivi: solo alcuni programmi |
| agreementNumber | Numero del contratto | Incentivi: solo alcuni programmi |
| agreementStartDate | Data di inizio del contratto | Incentivi: solo alcuni programmi |
| calculationDate | Data di calcolo del reddito nel sistema | Tutti |
| claimId | Identificatore univoco per l'attestazione | Incentivi: solo alcuni programmi |
| customerCountry | Paese/Area geografica del cliente | marketplaces |
| customerEmail |  |  |
| customerName | Può essere vuoto | Solo programmi di incentivi (eccezione: OEM) e marketplace. Per le transazioni CSP, nei marketplace verrà visualizzato il nome del provider di servizi condivisi |
| customerTenantId |  |  |
| distributorId | Identificatore del distributore | Incentivi: solo alcuni programmi |
| distributorName | Nome del distributore | Incentivi: solo alcuni programmi |
| earningAmount | Importo del reddito nella valuta della transazione originale | Tutti |
| earningAmountInLastPaymentCurrency | Importo del reddito nell'ultima valuta di pagamento. Il campo sarà vuoto se non sono stati corrisposti pagamenti precedenti. |  |
| earningAmountUSD | Importo del reddito in dollari statunitensi | Tutti |
| earningDate | Data del reddito | Tutti |
| earningExchangeRate | Tasso di cambio usato per visualizzare l'importo corrispondente in dollari statunitensi | Tutti |
| earningId | Identificatore univoco per ogni reddito | Tutti |
| earningRate | Tasso di incentivi applicato all'importo della transazione per generare un guadagno | Tutti |
| earningType | Indica se si tratta di corrispettivi, sconti, co-op, vendite e così via | Tutti |
| exchangeRateDate | Data del tasso di cambio usata per calcolare il valore in dollari statunitensi di EarningAmount | Tutti |
| externalReferenceId | Identificatore univoco per il programma | Programmi a pagamento diretto (incentivi e marketplace) |
| externalReferenceIdLabel | Etichetta identificatore univoco | Programmi a pagamento diretto (incentivi e marketplace) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Numero di fattura (applicabile solo per l'organizzazione) | Incentivi e marketplace: solo alcuni programmi |
| lastPaymentCurrency | Ultima valuta di pagamento. Il campo sarà vuoto se non sono stati corrisposti pagamenti precedenti. |  |
| lever | Indica la regola di business per il reddito | Tutti |
| LicensingProgramName | Nome del programma di licenza |  |
| LineItemId | Singola voce nella fattura di un cliente |  |
| localProviderSeller | Fornitore/gestore del sistema di pagamento locale |  |
| Mese di maturità | Mese di pagamento stimato | Tutti |
| OrderId | Si riferisce alla fattura di un cliente  | marketplaces |
| parentProductId | Identificatore univoco del prodotto padre. Se non è presente un prodotto padre per la transazione, l'ID del prodotto padre coincide con l'ID del prodotto. | marketplaces |
| parentProductName | Nome del prodotto padre. Se non è presente un prodotto padre per la transazione, il nome del prodotto padre coincide con il nome del prodotto. | marketplaces |
| participantId | Identità principale del partner che realizza un reddito nell'ambito del programma | Tutti |
| participantIdType | PRINCIPALMENTE ID programma per i programmi di incentivi e Seller IF per i marketplace | Tutti |
| participantName | Nome del partner beneficiario del reddito | Tutti |
| partnerCountryCode | Località/paese/area del partner beneficiario del reddito | Tutti |
| partNumber | È sempre vuoto | Alcuni programmi di incentivi e marketplace |
| paymentId | Identificatore univoco per correlare tutte le transazioni nel report delle transazioni con un pagamento specifico nel report di pagamento | Tutti |
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
| tpan | Indica la rete pubblicitaria di terze parti | Marketplaces Solo annunci |
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

### <a name="transaction-adjustment-codes"></a>Codici di rettifica delle transazioni

Nella tabella seguente sono elencati i codici motivo per le rettifiche e le relative descrizioni.

|**Codice motivo**   |**Descrizione**   |
|------------------|:-------------------------------------|
| Conformità ar | Rettifica che riduce gli utili quando le fatture Microsoft non vengono pagate in tempo dal partner. |
| Rollover co-op | Rettifica che trasferisce gli utili co-op in un altro periodo o converte gli utili co-op in sconti. |
| Regolazione delle operazioni | Rettifica che corregge gli errori di calcolo del sistema Microsoft. |
| Ops Adjustment Microsoft incorrect calc | Rettifica che corregge i calcoli erri. |
| Registrazione non corretta di Ops Adjustment Microsoft | Rettifica per i calcoli erri correlati alla registrazione. |
| Mapping partner (sottoscrizione) MCI/CSP | Rettifica che corregge il disallineamento della sottoscrizione. |
| Eccezione dei criteri | Regolazione che esegue l'override di una regola del programma.  |
| Utili del periodo precedente | Rettifica per gli utili al di fuori del periodo di guadagno corrente. |

## <a name="payments"></a>Pagamenti

La **pagina** Pagamenti dettaglia il denaro ottenuto con Microsoft. Mostra anche quando e quanto verrà pagato.

>[!Note]
> Per poter beneficiare del pagamento, gli introiti devono raggiungere la [soglia di pagamento](payment-thresholds-methods-timeframes.md) di 50 dollari statunitensi. Per altre informazioni, vedere il [Contratto di Microsoft Publisher.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Schermata panoramica dei pagamenti.":::

- **Totale pagato quest'anno:** il totale pagato quest'anno, in dollari statunitensi, per tutti i programmi.
- **Pagamento successivo stimato:** il singolo pagamento successivo in arrivo (anche se ce ne saranno altri in arrivo), in dollari statunitensi.
- **Ultimo pagamento:** importo (in dollari STATUNITENSI), nome del programma e programma del pagamento più recente.
- **Pagamento per origine:** importo dei pagamenti (in dollari STATUNITENSI), per programma, negli ultimi 12 mesi.

### <a name="payments-list"></a>Elenco pagamenti

La **tabella Elenco dei pagamenti** mostra i pagamenti a pagamento e in sospeso. È possibile scaricare le informazioni fiscali relative alle spese di servizio in formato PDF e visualizzare i dettagli di guadagno per un determinato pagamento.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Esportare la cronologia delle transazioni.":::

- **Pagamento:** tutti i pagamenti inviati correttamente. Scegliere l'anno nel menu a discesa per filtrare i pagamenti rilasciati in tale anno.
- **In sospeso:** pagamenti imminenti.
- **Imposta sulla tariffa del servizio (modulo PDF):** disponibile per i pagamenti soggetti all'imposta sulla tariffa del servizio. Le imposte sulle spese di servizio sono visualizzate in **Altre imposte**.
- **Visualizza:** reindirizza alla cronologia delle transazioni con un elenco di utili inclusi nel pagamento.

Per comprendere perché si potrebbero avere utili mancanti o imprevisti, vedere Domande comuni sui proventi del [marketplace commerciale.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Stato dei pagamenti

La tabella seguente illustra i diversi stati di guadagno.

| Stato degli utili | Motivo | È richiesta un'azione del partner? |
| --- | --- | --- |
| Non elaborato | Gli utili non sono idonei al pagamento. Rimane in questo stato per un periodo di raffreddamento, come definito nella guida al programma per il programma Incentivi. | No |
| In programma | Ordine di pagamento generato in attesa di verifiche interne prima dell'elaborazione del pagamento. | No |
| Pending tax invoice (Fattura fiscale in sospeso) | La fattura fiscale è incompleta o non valida. | È necessario aggiornare la fattura fiscale prima di poter essere pagati. |
| Rejected during review (Rifiutato durante la revisione) | Il pagamento è stato rifiutato durante la revisione. | Per informazioni dettagliate, contattare il supporto tecnico Microsoft. |
| Non riuscito | Il pagamento non è riuscito a causa di un errore di sistema Microsoft. | Per informazioni dettagliate, contattare il supporto tecnico Microsoft |
| In corso | Il pagamento è in corso. | No |
| Pagamento non corretto | Il recupero dei pagamenti è in corso. | No |
| Inviato | Il pagamento è stato inviato alla banca. | No |
| Reprocessing (Rielaborazione) | Il pagamento ha rilevato un errore di sistema Microsoft ed è in corso di rielaborazione. | No |
| Reversed | Il pagamento è stato annullato dalla banca e verrà inviato nuovamente nel ciclo di pagamento successivo. | No |
| Tax invoice rejected (Fattura fiscale rifiutata) | La fattura fiscale è stata rifiutata durante la revisione. Tutti i pagamenti in sospeso rimarranno in attesa fino al completamento della revisione della fattura fiscale. | Per informazioni dettagliate, contattare il supporto tecnico Microsoft |
| Tax invoice under review (Fattura fiscale in revisione) | È in corso la revisione della fattura fiscale. Il pagamento verrà rilasciato una volta che la fattura fiscale è stata approvata. | No |
| Rifiutato | Il pagamento è stato rifiutato dalla banca. | Per informazioni dettagliate, contattare la banca. |
|

### <a name="payments-download"></a>Download dei pagamenti

 Nella tabella seguente viene illustrata ogni colonna del report. Per visualizzare altri dettagli sui pagamenti, selezionare **Scarica** nella parte superiore della pagina Pagamenti.

| Nome colonna | Descrizione |
| --- | --- |
| participantID | Identità principale del partner che realizza un reddito nell'ambito del programma |
| participantIDType | In genere l'ID programma per i programmi incentivi e l'ID venditore per i programmi dello Store |
| participantName | Nome del partner beneficiario del reddito |
| programName | Incentivi/nome del programma del negozio |
| earned | Importo guadagnato nella valuta di pagamento per l'ID programma/participante |
| earnedUSD | Importo guadagnato per l'ID programma/participante, in dollari statunitensi |
| withheldTax | Importo delle imposte in valuta di pagamento per l'ID programma/participante |
| salesTax | Importo totale dell'imposta sulle vendite nella valuta Con pagamento a per il programma/ID partecipante (applicabile solo ai programmi di incentivi) |
| serviceFeeTax | Quantità totale di serviceFeeTax in valuta di pagamento per l'ID programma/participante (applicabile solo per i programmi Store e Azure Marketplace) |
| totalPayment | Pagamento totale in valuta locale, al netto di tutte ritenute e al lordo dell'imposta sulle vendite (se applicabile) per l'ID programma/participante |
| currencyCode | Codice della valuta di pagamento |
| paymentMethod | Metodo utilizzato per pagare il partner, ad esempio, bonifico bancario o nota di credito |
| paymentID | Identificatore univoco per il pagamento. Questo numero è in genere visibile nel rendiconto bancario (applicabile solo ai pagamenti SAP). |
| paymentStatus | Stato dei pagamenti |
| paymentStatusDescription | Descrizione descrittiva dello stato dei pagamenti |
| paymentDate | Data del pagamento inviato da Microsoft |
|

## <a name="export-data"></a>Esportare i dati

La **pagina Esporta** dati non viene aggiornata di per sé. Per visualizzare i dati più recenti, potrebbe essere necessario aggiornare la pagina manualmente. Selezionare una delle tre schede per esportare la cronologia delle **transazioni,** **i pagamenti,** il riepilogo **delle** transazioni o **l'istruzione cronologica**.

Il filtro potrebbe causare un **errore Nessun dato** disponibile. Ciò può verificarsi se il periodo di tempo predefinito è stato lasciato selezionato a tre mesi e quindi è stato selezionato un ID pagamento da un guadagno esterno a tale periodo. In questo caso, espandere il periodo di tempo e riprovare.

Ecco un esempio di esportazione dei pagamenti:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Esportare il report pagamenti.":::

### <a name="historical-statements"></a>Rendiconti cronologici

Il **riepilogo esporta dati** fornisce anche l'accesso alle istruzioni cronologiche.

> [!NOTE]
> Un'istruzione cronologica è uno snapshot e non viene aggiornata. Se [necessario, contattare](https://partner.microsoft.com/support/v2/?stage=1) il supporto tecnico e richiedere i dati più recenti.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Esportare le istruzioni cronologiche.":::

- La cronologia delle transazioni precedente al 1° luglio 2019 viene gestita separatamente e usa campi diversi dei report di cronologia successivi.
- La cronologia delle transazioni legacy include una colonna denominata "Reserved" che corrisponde alla colonna "Earnings" nella cronologia moderna, ad eccezione del fatto che esclude tutti gli utili con stato "Payment Sent".
- Filtri come 3M, 6M o 12M, non si applicano alla sezione dei rendiconti cronologici.

### <a name="historical-statement-downloads"></a>Download di istruzioni cronologiche

Nella tabella seguente viene illustrata ogni colonna in un'istruzione cronologica.

| Nome campo | Descrizione |
| --- | --- |
| Origine dei ricavi | Origine dei ricavi in base a dove si è verificata la transazione, ad esempio Microsoft Store, Windows Phone Store, Windows 8 Store o Microsoft Advertising |
| ID dell'ordine | Identificatore univoco dell'ordine. Questo ID consente di identificare le transazioni di acquisto con le rispettive transazioni non di acquisto, ad esempio rimborsi o chargeback. Entrambe avranno lo stesso ID ordine. Inoltre, se è presente un addebito suddiviso in cui sono stati usati più metodi di pagamento per un singolo acquisto, è possibile collegare le transazioni di acquisto. |
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