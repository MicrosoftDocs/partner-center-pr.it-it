---
title: Risoluzione dei problemi relativi a pagamenti e utili
ms.topic: article
ms.date: 02/05/2021
description: Informazioni su come risolvere i problemi, ad esempio guadagni mancanti o non corretti, problemi di idoneità e come risolvere i guadagni degli incentivi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: c6ff8915384f8c7ab98fa058f2e45e3d0b4f7214
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179514"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Risoluzione dei problemi relativi a pagamenti mancanti, guadagni non corretti e altri problemi

**Ruoli appropriati**

- Amministratore degli incentivi

Questo articolo consente di risolvere eventuali problemi relativi a guadagni o pagamenti nel programma per gli incentivi. Gli argomenti trattati includono la tempistica dei pagamenti, il controllo dell'idoneità dei guadagni e l'importanza di configurare correttamente i profili di pagamento e fiscali.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Chi può creare o aggiornare i profili di pagamento e fiscali per la mia organizzazione?

Gli utenti che hanno il ruolo di amministratore di incentivi nel centro per i partner per il programma incentive pertinente e il percorso MPN possono aggiornare e visualizzare i profili di pagamento e fiscali per l'organizzazione.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Quanto tempo è necessario affinché Microsoft approvi i profili di pagamento e/o fiscali in sospeso?

La convalida può richiedere fino a 48 ore. In questo periodo di tempo lo stato del profilo nella pagina di panoramica verrà visualizzato come Validating enrollment (Convalida della registrazione in corso). Al termine del processo, lo stato verrà visualizzato come **registrato** in caso di esito positivo o **azione richiesta: aggiornare il pagamento e/o le informazioni fiscali** , se necessario.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>In che modo ho la conferma di aver completato correttamente il profilo di pagamento e fiscale?

Lo stato della registrazione viene visualizzato nella pagina di panoramica. Al termine della creazione dei profili, lo stato verrà **convalidato** per la registrazione. Dopo aver convalidato le informazioni, lo stato diventa **registrato**. Questo stato indica che il pagamento e il profilo fiscale e la registrazione sono stati completati correttamente.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Perché è necessario aggiornare il profilo fiscale per usarlo con un nuovo programma Incentivi?

Microsoft addebita gli incentivi da diverse posizioni a seconda del tipo di incentivo. Queste posizioni diverse possono richiedere informazioni fiscali aggiuntive, in base alle regole del programma Incentivi, per eseguire correttamente l'elaborazione.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Come si elimina un profilo di pagamento e/o fiscale?

Attualmente Microsoft non supporta l'opzione di eliminazione dei profili di pagamento e fiscali esistenti.

## <a name="my-payment-is-missing-or-incorrect"></a>Il pagamento è mancante o errato

I pagamenti mancanti o non corretti sono spesso correlati a una delle cause seguenti:

- **Il Licenziatario potrebbe non essere idoneo.**  Gli utili saranno disponibili solo se l'utente soddisfa i requisiti di idoneità operativa, vale a dire se è registrato nel rispettivo periodo retributivo del programma.
- **È possibile che non siano stati soddisfatti i requisiti.**  Verificare se sono state soddisfatte le regole di idoneità e i ricavi idonei per l'incentivo che si sta cercando.

  **Per verificare l'idoneità**

  1. Accedi a [incentivi](https://partner.microsoft.com/membership/partner-incentives)per i partner.

  2. Scorrere verso il basso fino ai documenti del programma.
  
  3. Selezionare il collegamento al documento desiderato, quindi esaminare le sezioni 

**Idoneità partner** e **regole dei ricavi idonei**.

- **Il profilo di pagamento potrebbe essere incompleto.** La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020.
- **È possibile che si verifichi un'azione in attesa**.  È possibile che gli incentivi non vengano elaborati a causa di un'azione in sospeso.

  **Per visualizzare le azioni in attesa**

  1. Accedi a [incentivi](https://partner.microsoft.com/membership/partner-incentives)per i partner.
  2. Aprire la pagina **Cronologia transazioni** . Esaminare i campi in questa pagina per tutte le azioni in sospeso da completare, ad esempio il **profilo fiscale in sospeso**, il **profilo di pagamento in sospeso** o l' **invio di fatture fiscali in sospeso**.

Se queste azioni non sono utili e i pagamenti rimangono mancanti o errati, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>In che modo è possibile riconciliare le regolazioni?

È possibile individuare e risolvere le modifiche apportate scaricando i dettagli relativi a guadagni e transazioni.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Sulla barra di spostamento superiore selezionare l'icona Money, quindi selezionare **Cronologia transazioni**.
3. Applicare i filtri appropriati. (Vedere la Nota **importante** più avanti).
4. Dopo aver filtrato i dati, selezionare **Avvia download**, quindi selezionare **Esporta dati**. I dati si apriranno in un file CSV.
5. Nel file CSV passare alla colonna P, ottenendo il **tipo**.
6. Filtrare questa colonna per la **regolazione-riduzione**. È possibile visualizzare il mese di ogni rettifica nella colonna S.

>[!IMPORTANT]
>Le modifiche applicate ai periodi di guadagno precedenti non saranno visibili nei guadagni per il mese in cui è stata applicata la regolazione. Le rettifiche rifletteranno sempre nel report degli utili per il mese a cui è stata applicata la regolazione.
>
>Ad esempio, un adattamento per i guadagni di gennaio 2019 elaborati nel settembre 2019 non rifletterà l'importo degli utili per il 2019 settembre. Tuttavia, quando viene ricevuto il pagamento per il 2019 settembre, sarà inclusa la rettifica per il 2019 gennaio che è stata applicata a settembre. In questo scenario, è necessario scaricare i dettagli della transazione per il 2019 gennaio per visualizzare la regolazione applicata.
>
>Tenere presente questo aspetto quando si impostano i filtri per la data. Come indicato in precedenza, le modifiche per i periodi precedenti saranno visibili solo nel mese in cui è stata applicata la regolazione. Verificare che l'intervallo di date selezionato corrisponda al mese della regolazione che si sta tentando di trovare. Potrebbe essere necessario selezionare **Clear All (Cancella tutto** ) per rimuovere i filtri, quindi applicare quelli nuovi.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Perché i pagamenti delle attestazioni co-op sono stati effettuati in due valute diverse?

Quando si ricevono fondi co-op da entità Microsoft diverse, i pagamenti vengono effettuati nella valuta locale di ogni entità.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Perché il pagamento viene effettuato in una valuta diversa dalla valuta dell’attestazione co-op?

Ogni programma di incentivi è associato a un profilo bancario creato durante la configurazione. La valuta specificata in tale profilo è la valuta in cui verrà effettuato il pagamento.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Non vedo i guadagni per un determinato periodo

Quando non vengono visualizzati i guadagni per un periodo di tempo in cui sono previsti, è in genere dovuto a uno dei problemi seguenti:

- **Il Licenziatario potrebbe non essere idoneo.**  Gli utili saranno disponibili solo se l'utente soddisfa i requisiti di idoneità operativa, vale a dire se è registrato nel rispettivo periodo retributivo del programma.

- **Il profilo di pagamento potrebbe essere incompleto.**  La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020.

Se sono stati completati i requisiti di idoneità, tra cui il caricamento con i dettagli relativi a pagamenti e imposte in tempo, e i guadagni sono ancora mancanti, contattare il [supporto](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="my-earnings-are-missing-or-incorrect"></a>I miei guadagni sono mancanti o non corretti

Eventuali guadagni mancanti o non corretti potrebbero essere causati da uno dei problemi seguenti:

- **È possibile che i requisiti non siano stati soddisfatti.**  Verificare che siano state soddisfatte le regole di [idoneità](#my-payment-is-missing-or-incorrect) utente e idoneità per l'acquisizione di ricavi per l'incentivo desiderato.

- **Potrebbe essere presente una discrepanza.**  Se si soddisfano i requisiti di idoneità del [programma](incentives-determined-your-program-eligibility.md) e di [idoneità](incentives-confirm-your-earnings-eligibility.md) per i guadagni e i guadagni sembrano ancora non corretti, le informazioni seguenti possono essere utili per recuperare i dati.

I guadagni vengono visualizzati nella pagina **Cronologia transazioni** e nella pagina **pagamenti** . È possibile accedere a entrambe le pagine selezionando l'icona del **payout** sulla barra di spostamento del centro per i partner.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Informazioni sulla transazione":::

Gli importi mensili che si ottengono nella visualizzazione della cronologia delle transazioni potrebbero non allinearsi con l'importo di pagamento ricevuto per un mese specifico. Ciò è dovuto a ricalcoli e modifiche per i periodi di guadagno precedenti applicati ai pagamenti futuri.

Ad esempio, un adattamento per i guadagni di gennaio 2019 elaborati nel settembre 2019 non verrà riflesso nell'importo dei guadagni per il 2019 settembre; Tuttavia, quando viene ricevuto il pagamento per il 2019 settembre, sarà inclusa la rettifica per il 2019 gennaio che è stata applicata a settembre.

In questo scenario, è necessario scaricare i dettagli della transazione per ottenere una visualizzazione completa di tutti i guadagni inclusi nel pagamento.  Inoltre, è possibile passare alla visualizzazione pagamenti per scaricare le transazioni per ogni pagamento.

### <a name="transaction-history"></a>Cronologia delle transazioni

Questa visualizzazione Mostra le tendenze per il pagamento e i pagamenti per mese, i guadagni in base allo stato e i dettagli della transazione insieme allo stato di pagamento per ogni transazione. I dati sono visibili solo per i programmi e gli ID MPN per i quali si è un utente o un amministratore di incentivi.

### <a name="payments"></a>Pagamenti

Questa visualizzazione consente di visualizzare i pagamenti per tutti i programmi e gli ID MPN. I dati sono visibili solo per i programmi e gli ID MPN per i quali si è un utente o un amministratore di incentivi. Da questa visualizzazione è possibile scaricare la rimessa o visualizzare i dettagli delle transazioni per pagamento.

| Per | Risorsa utile |
| ------ | :----------- | 
| Visualizza le informazioni di pagamento per riga, inclusi i guadagni e gli importi di pagamento nella valuta locale  | Vedere il campo **elenco di pagamenti**   |
| Scarica una lettera di rimessa   |  Seleziona **rimessa pagamento**  |
| Visualizza i dettagli a livello di transazione per un pagamento specifico |  Selezione **visualizzazione**  |
| Esporta dettagli transazione in Excel  |  Selezionare **Avvia download**, quindi selezionare **Esporta dati**. Tutti i filtri selezionati verranno applicati ai dati esportati. Una volta che lo stato è stato modificato in completato, selezionare **Scarica** e seguire le istruzioni per esportare il report dettagliato sulle transazioni. Aggiornare la pagina se lo stato non viene aggiornato entro cinque minuti.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Guadagni e pagamenti mancanti o non corretti

Se non si è in grado di individuare i dettagli di un pagamento o di una transazione, verificare se sono stati applicati i filtri corretti. Poiché alcuni nomi di programma sono stati modificati (ad esempio, CSP 1T Direct partner è ora CSP Direct Bill partner), potrebbe essere necessario usare più selezioni.

Se non si riesce ancora a trovare i guadagni o se si ritiene che i guadagni visualizzati non siano corretti, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Ricerca per categorie riconciliare i miei guadagni?

In caso di discrepanza negli utili, completare la procedura seguente:

1. **Verificare di essere idonei per gli utili.**  I guadagni saranno disponibili solo se si soddisfano l'idoneità del [programma](incentives-determined-your-program-eligibility.md) e l' [idoneità ai guadagni](incentives-confirm-your-earnings-eligibility.md).

2. **Verificare che il profilo di pagamento sia completo.**  La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020. 

3. **Verificare di aver soddisfatto i requisiti.**  Verificare se sono state soddisfatte le regole di [idoneità](#my-payment-is-missing-or-incorrect) e i ricavi idonei per il programma incentive.

Se queste azioni non sono utili e i guadagni non sono ancora riconciliati, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>Dove sono indicate le tariffe?

1. Accedi a [incentivi](https://partner.microsoft.com/membership/partner-incentives)per i partner.

2. Scorrere verso il basso per accedere ai documenti per il programma.

3. Selezionare il collegamento al documento per il rispettivo programma.

4. Nel documento, fare riferimento alla sezione **struttura e tariffe del programma**.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire le attestazioni cooperative](incentives-managing-co-op-claims.md)