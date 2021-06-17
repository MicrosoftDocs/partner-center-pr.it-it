---
title: Risoluzione dei problemi relativi a pagamenti e utili
ms.topic: article
ms.date: 02/05/2021
description: Informazioni su come risolvere problemi come utili mancanti o non corretti, problemi di idoneità e come riconciliare gli utili degli incentivi.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ad71a6e02d6472ae844c504491e5acb05d5d6426
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277862"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Risoluzione dei problemi relativi a pagamenti mancanti, utili non corretti e altri problemi

**Ruoli appropriati:** Amministratore incentivi

Questo articolo consente di risolvere eventuali problemi di utili o di pagamento nel programma di incentivi. Gli argomenti trattati includono la tempistica dei pagamenti, la verifica dell'idoneità degli utili e l'importanza di configurare correttamente i profili di pagamento e fiscali.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>Chi può creare o aggiornare i profili di pagamento e fiscali per l'organizzazione?

Gli utenti con il ruolo di amministratore incentivi in Partner Center per il programma di incentivi pertinente e la posizione MPN possono aggiornare e visualizzare i profili di pagamento e fiscali per l'organizzazione.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>Quanto tempo è necessario affinché Microsoft approvi i profili di pagamento e/o fiscali in sospeso?

La convalida può richiedere fino a 48 ore. In questo periodo di tempo lo stato del profilo nella pagina di panoramica verrà visualizzato come Validating enrollment (Convalida della registrazione in corso). Al termine del processo, lo stato  verrà visualizzato come Registrato in caso di esito positivo o Azione richiesta - Aggiorna i dettagli relativi al pagamento **e/o** alle imposte, se necessario.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>In che modo ho la conferma di aver completato correttamente il profilo di pagamento e fiscale?

Lo stato della registrazione viene visualizzato nella pagina di panoramica. Al termine della creazione dei profili, lo stato sarà **Convalida della registrazione.** Dopo aver convalidato le informazioni, lo stato cambia in **Registrato.** Questo stato indica che il profilo di pagamento e fiscale e la registrazione sono stati completati correttamente.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>Perché è necessario aggiornare il profilo fiscale per usarlo con un nuovo programma Incentivi?

Microsoft addebita gli incentivi da diverse posizioni a seconda del tipo di incentivo. Queste posizioni diverse possono richiedere informazioni fiscali aggiuntive, in base alle regole del programma Incentivi, per eseguire correttamente l'elaborazione.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>Come si elimina un profilo di pagamento e/o fiscale?

Attualmente Microsoft non supporta l'opzione di eliminazione dei profili di pagamento e fiscali esistenti.

## <a name="my-payment-is-missing-or-incorrect"></a>Il pagamento è mancante o errato

I pagamenti mancanti o non corretti sono spesso correlati a una delle cause seguenti:

- **L'utente potrebbe non essere idoneo.**  Gli utili saranno disponibili solo se l'utente soddisfa i requisiti di idoneità operativa, vale a dire se è registrato nel rispettivo periodo retributivo del programma.
- **È possibile che i requisiti non sono stati soddisfatti.**  Verificare se sono state soddisfatte le regole relative all'idoneità e ai ricavi idonei per l'incentivo che si sta cercando.

  **Per verificare l'idoneità**

  1. Accedere agli [incentivi per i partner.](https://partner.microsoft.com/membership/partner-incentives)

  2. Scorrere verso il basso fino ai documenti per il programma.
  
  3. Selezionare il collegamento al documento desiderato e quindi rivedere le sezioni 

**Regole per l'idoneità dei partner** **e i ricavi idonei**.

- **Il profilo di pagamento potrebbe essere incompleto.** La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020.
- **Potrebbe essere in sospeso un'azione**.  È possibile che gli incentivi non vengano elaborati a causa di un'azione in sospeso.

  **Per visualizzare le azioni in sospeso**

  1. Accedere agli [incentivi per i partner.](https://partner.microsoft.com/membership/partner-incentives)
  2. Aprire la **pagina Cronologia** transazioni . Esaminare i campi in questa pagina per verificare se sono presenti azioni in sospeso da completare, ad esempio **Profilo** fiscale in sospeso, **Profilo** di pagamento in sospeso o Invio fattura **fiscale in sospeso.**

Se queste azioni non sono utili e i pagamenti sono ancora mancanti o non corretti, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>Come è possibile riconciliare le rettifiche?

È possibile individuare e riconciliare le rettifiche scaricando i dettagli relativi ai guadagni e alle transazioni.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Nella barra di spostamento superiore selezionare l'icona money e quindi selezionare **Cronologia transazioni**.
3. Applicare i filtri appropriati. Vedere la **nota importante** riportata di seguito.
4. Dopo aver filtrato i dati, selezionare **Start download (Avvia download)** e quindi **Export data (Esporta dati).** I dati verranno aperti in un file CSV.
5. Nel file CSV passare alla colonna P, **tipo di guadagno**.
6. Filtrare questa colonna **in base a Adjustment-Rebate**. È possibile visualizzare il mese di ogni rettifica nella colonna S.

>[!IMPORTANT]
>Le rettifiche applicate ai periodi di utili precedenti non saranno visibili negli utili per il mese in cui è stata applicata la rettifica. Le rettifiche si rifletteranno sempre nel report degli utili per il mese a cui è stata applicata la rettifica.
>
>Ad esempio, una rettifica per gli utili di gennaio 2019 elaborata nel mese di settembre 2019 non rifletterà l'importo degli utili per settembre 2019. Tuttavia, quando viene ricevuto il pagamento per settembre 2019, includerà la rettifica per gennaio 2019 applicata a settembre. In questo scenario è necessario scaricare i dettagli della transazione per gennaio 2019 per visualizzare la rettifica applicata.
>
>Tenere presente questo problema quando si impostano i filtri di data. Come accennato in precedenza, le rettifiche per i periodi precedenti saranno visibili solo nel mese in cui è stata applicata la rettifica. Verificare che l'intervallo di date selezionato corrisponda al mese della rettifica che si sta tentando di individuare. Potrebbe essere necessario selezionare **Cancella tutto** per rimuovere i filtri e quindi applicarne di nuovi.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>Perché i pagamenti delle attestazioni co-op sono stati effettuati in due valute diverse?

Quando si ricevono fondi co-op da entità Microsoft diverse, i pagamenti vengono effettuati nella valuta locale di ogni entità.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>Perché il pagamento viene effettuato in una valuta diversa dalla valuta dell’attestazione co-op?

Ogni programma di incentivi è associato a un profilo bancario creato durante la configurazione. La valuta specificata in tale profilo è la valuta in cui verrà effettuato il pagamento.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>Gli utili non vengono visualizzati per un determinato periodo

Quando gli utili non vengono visualizzati per un periodo in cui sono previsti, è in genere dovuto a uno dei problemi seguenti:

- **L'utente potrebbe non essere idoneo.**  Gli utili saranno disponibili solo se l'utente soddisfa i requisiti di idoneità operativa, vale a dire se è registrato nel rispettivo periodo retributivo del programma.

- **Il profilo di pagamento potrebbe essere incompleto.**  La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020.

Se sono stati completati i requisiti di idoneità, incluso l'onboarding con i dettagli relativi a proventi e imposte nel tempo e gli utili non sono ancora disponibili, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="my-earnings-are-missing-or-incorrect"></a>Gli utili sono mancanti o errati

Eventuali guadagni mancanti o non corretti potrebbero essere causati da uno dei problemi seguenti:

- **È possibile che i requisiti non siano stati soddisfatti.**  Verificare che siano state soddisfatte le regole di [idoneità](#my-payment-is-missing-or-incorrect) utente e idoneità per l'acquisizione di ricavi per l'incentivo desiderato.

- **Potrebbe essere presente una discrepanza.**  Se si [soddisfano](incentives-determined-your-program-eligibility.md) sia i [](incentives-confirm-your-earnings-eligibility.md) requisiti di idoneità al programma che i requisiti di idoneità agli utili e gli utili sembrano ancora non corretti, le informazioni seguenti possono essere utili per recuperare i dati.

Gli utili vengono visualizzati sia nella **pagina Cronologia transazioni** che nella **pagina** Pagamenti. È possibile accedere a entrambe le pagine selezionando **l'icona Pagamento** sulla barra di spostamento in Partner Center.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Informazioni sulla transazione.":::

Gli importi con reddito mensile nella visualizzazione Cronologia transazioni potrebbero non essere allineati all'importo del pagamento ricevuto per un mese specifico. Ciò è dovuto a ricalcoli e rettifiche per periodi di reddito precedenti che vengono applicati ai pagamenti futuri.

Ad esempio, una rettifica per gli utili di gennaio 2019 elaborata nel mese di settembre 2019 non verrà riflessa nell'importo degli utili per settembre 2019; Tuttavia, quando viene ricevuto il pagamento per settembre 2019, includerà la rettifica per gennaio 2019 applicata a settembre.

In questo scenario è necessario scaricare i dettagli della transazione per ottenere una visualizzazione completa di tutti gli utili inclusi nel pagamento.  È anche possibile passare alla visualizzazione Pagamenti per scaricare le transazioni per ogni pagamento.

### <a name="transaction-history"></a>Cronologia delle transazioni

Questa visualizzazione mostra le tendenze degli utili e dei pagamenti per mese, gli utili per stato e i dettagli delle transazioni insieme allo stato di pagamento per ogni transazione. I dati sono visibili solo per i programmi e gli ID MPN per cui si è un utente o un amministratore di incentivi.

### <a name="payments"></a>Pagamenti

Questa visualizzazione consente di visualizzare i pagamenti per tutti i programmi e gli ID MPN. I dati sono visibili solo per i programmi e gli ID MPN per cui si è un utente o un amministratore di incentivi. Da questa visualizzazione è possibile scaricare la rimessa o visualizzare i dettagli delle transazioni tramite pagamento.

| Per | Risorsa utile |
| ------ | :----------- | 
| Visualizzare le informazioni di pagamento per riga, inclusi gli importi degli utili e dei pagamenti nella valuta locale  | Vedere il **campo Elenco dei** pagamenti   |
| Scaricare una lettera di rimessa   |  Selezionare **La rimessa di pagamento**  |
| Visualizzare i dettagli a livello di transazione per un pagamento specifico |  Selezionare **Visualizza**  |
| Esportare i dettagli delle transazioni in Excel  |  Selezionare **Avvia download** e quindi Esporta **dati.** Tutti i filtri selezionati verranno applicati ai dati esportati. Dopo che lo stato è stato modificato in Completato, selezionare **Scarica** e seguire le istruzioni per esportare il report dettagliato delle transazioni. Aggiornare la pagina se lo stato non viene aggiornato entro cinque minuti.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Utili e pagamenti mancanti o non corretti

Se non è possibile individuare i dettagli di un pagamento o di una transazione, verificare se sono stati applicati i filtri corretti. Poiché alcuni nomi di programma sono cambiati (ad esempio, CSP 1T Direct Partner è ora CSP Direct Bill Partner), potrebbe essere necessario usare più selezioni.

Se non si trovano ancora gli utili o si ritiene che gli utili visualizzati non siano corretti, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>Ricerca per categorie riconciliare gli utili?

In caso di discrepanza negli utili, completare la procedura seguente:

1. **Verificare di essere idonei per gli utili.**  Gli utili saranno disponibili solo se si soddisfano sia l'idoneità [al programma](incentives-determined-your-program-eligibility.md) che [l'idoneità per gli utili](incentives-confirm-your-earnings-eligibility.md).

2. **Verificare che il profilo di pagamento sia completo.**  La data iniziale di acquisizione degli incentivi sarà il primo giorno del mese in cui tutti i requisiti di idoneità sono stati soddisfatti, incluso l'inserimento dei dati relativi a pagamenti e imposte. Gli utili non saranno disponibili per i mesi precedenti al pagamento e al completamento delle imposte. Se, ad esempio, si soddisfano tutti i requisiti durante il mese di aprile 2020, la data di inizio degli utili sarà il 1 aprile 2020. 

3. **Verificare di aver soddisfatto i requisiti.**  Verificare se sono state soddisfatte le regole [relative all'idoneità e](#my-payment-is-missing-or-incorrect) ai ricavi idonei per il programma di incentivi.

Se queste azioni non sono utili e gli utili non sono ancora riconciliati, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>Dove sono indicate le tariffe?

1. Accedere agli [incentivi per i partner.](https://partner.microsoft.com/membership/partner-incentives)

2. Scorrere verso il basso per accedere ai documenti per il programma.

3. Selezionare il collegamento al documento per il rispettivo programma.

4. Nel documento fare riferimento alla sezione **Struttura del programma e Tariffe.**

## <a name="next-steps"></a>Passaggi successivi

- [Gestire le attestazioni cooperative](incentives-managing-co-op-claims.md)