---
title: Pianificazioni e processi di pagamento
description: Informazioni su pagamenti e transazioni, ad esempio pianificazioni dei pagamenti e processi di recupero per il marketplace commerciale e altre transazioni.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: f2ba8132677eb0a0368021b6d7065f5202589f24
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146953"
---
# <a name="payout-schedules-and-processes"></a>Pianificazioni e processi di pagamento

**Ruoli appropriati:** amministratore account | Amministratore globale

Questo articolo illustra la pianificazione dei pagamenti di Microsoft, dove trovare lo stato di un pagamento e il processo per il non pagamento da parte del cliente.

## <a name="payment-schedules"></a>Pianificazioni dei pagamenti

Le sezioni seguenti descrivono il processo di pagamento per Contratto Enterprise **transazioni** con carta **di credito/fattura.**

### <a name="enterprise-agreement-transactions"></a>Contratto Enterprise transazioni

Quando un cliente acquista un prodotto da Microsoft AppSource o Azure Marketplace usando l'Contratto Enterprise Microsoft esistente per le transazioni, microsoft riemetteremo i pagamenti nel ciclo di pagamento successivo di 30 giorni dopo la fattura del cliente. Le transazioni in cui un cliente usa una carta di credito hanno un periodo di conservazione di 30 giorni prima del pagamento.

Spesso si verifica un pagamento prima che Microsoft riscuota il pagamento dal cliente. Per [le azioni intraprese](#process-for-customer-non-payment) se il cliente non riesce a pagare Microsoft ma è già stato emesso un pagamento, vedere La procedura per il non pagamento da parte del cliente è riportata di seguito.

| Event | Descrizione | Visibilità dei report | Intervallo* |
| --- | --- | --- | --- |
| Utilizzo o mese della transazione | Il cliente usa o acquista un servizio. | [Dashboard utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) [o](/azure/marketplace/partner-center-portal/orders-dashboard) ordine | **Mese 1** |
| Microsoft calcola l'importo della fatturazione | Determinare l'utilizzo totale, il totale delle transazioni | [Dashboard utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) [o](/azure/marketplace/partner-center-portal/orders-dashboard) ordine | **Mese 2** |
| Pagamenti pubblicati | Determinare la tariffa d'agenzia e gli utili dei proventi | Contrassegnato come Non elaborato nella cronologia delle transazioni [nell'estratto conto](payout-statement.md) | **Mese 3 (prima settimana)** |
| Preparare i pagamenti | Gli utili vengono preparati per il pagamento mensile | Contrassegnato come Imminente nella cronologia delle transazioni [nell'estratto conto](payout-statement.md) | **Mese 3 (prima settimana)** |
| **Pagamenti inviati** | **Il pagamento viene inviato all'editore** | **Contrassegnato come Inviato nella cronologia delle transazioni e nella sezione Pagamenti [dell'estratto conto](payout-statement.md)** | **Mese 3 (non oltre il 15)** |
| Fattura pagata dal cliente | Microsoft riscuote il pagamento dal cliente | Nessuna modifica | **Mese da 4 a 12** |
|

\* La data di pagamento è in formato PST (Pacific Standard Time).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Sequenza temporale dei pagamenti per i clienti con contratto Enterprise Agreement.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transazioni con carta di credito o fattura (assegno/bonifico)

Tutti gli acquisti con carta di credito o fattura mensile hanno un periodo di conservazione di 30 giorni per garantire che i fondi siano raccolti dal cliente.

| Event | Descrizione | Visibilità dei report | Intervallo* |
| --- | --- | --- | --- |
| Utilizzo o mese della transazione | Il cliente usa o acquista un servizio. | [Dashboard utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) [o](/azure/marketplace/partner-center-portal/orders-dashboard) ordine | **Mese 1** |
| Fattura pagata dal cliente | Determinare l'utilizzo totale, il valore totale della transazione e il pagamento della fattura da parte del cliente | [Dashboard utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) [o](/azure/marketplace/partner-center-portal/orders-dashboard) ordine | **Mese 2** |
| Pagamenti pubblicati | Determinare la tariffa d'agenzia e gli utili dei proventi | Contrassegnato come Non elaborato nella cronologia delle transazioni [nell'estratto conto](payout-statement.md) | **Mese 2** |
| Periodo di conservazione di 30 giorni | Garantire la raccolta di fondi, i possibili chargeback e le richieste di rimborso | Contrassegnato come Non elaborato nella cronologia delle transazioni [nell'estratto conto](payout-statement.md) | **Mese 3** |
| Preparare i pagamenti | Gli utili vengono preparati per il pagamento mensile | Contrassegnato come Imminente nella cronologia delle transazioni [nell'estratto conto](payout-statement.md) | **Mese 4 (prima settimana)** |
| **Pagamento inviato** | **Il pagamento viene inviato all'editore** | **Contrassegnato come Inviato nella cronologia delle transazioni e nella sezione Pagamenti [dell'estratto conto](payout-statement.md)** | **Mese 4 (non oltre il 15)** |
|

\* La data del pagamento è nell'ora solare Pacifico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Sequenza temporale dei pagamenti per i clienti con carta di credito e fattura.":::

## <a name="process-for-customer-non-payment"></a>Processo per il non pagamento da parte del cliente

In rari casi, Microsoft non è in grado di raccogliere i pagamenti dai clienti per gli acquisti nel marketplace commerciale. Quando un cliente non riesce a pagare Microsoft in base alla pianificazione della fatturazione, viene avviata la procedura di raccolta. Questo processo richiede circa quattro mesi e comporta una comunicazione permanente da Microsoft. Se il pagamento non viene ricevuto entro la fine di questo processo, Microsoft scrive i fondi come non raccolti.

In base al processo di pagamento articolato qui, Microsoft potrebbe aver già versato fondi agli editori (l'utente) che sono in ultima analisi poco riconoscibili. Di conseguenza, è necessario un processo per la riconciliazione di questi importi. Per assicurarsi di ricevere un avviso che il pagamento (già ricevuto) può essere riconciliato, si riceverà una notifica quando un cliente è nel processo di raccolta e gli acquisti potrebbero essere svasi.

Microsoft ricupererà tutti i pagamenti già versati usando uno dei metodi seguenti: (1) Microsoft può sottrarre gli importi non pagati dai pagamenti futuri; Ad esempio, se 1.000 dollari nei pagamenti vengono ritenuti non colti e svariati, i pagamenti futuri verranno ritenuti non rimborsati fino a quando non vengono recuperati i 1.000 dollari o (2) Microsoft può richiedere un rimborso o un editore di fatture per eventuali importi non recuperati.

La pianificazione seguente è un esempio:

| Evento | Data approssimativa* | Visibilità dei partner |
| --- | --- | --- |
| Data di pagamento di esempio | 10/15/2020 | Contrassegnato **come Inviato** nella cronologia delle transazioni e nella sezione Pagamenti nel dashboard dei pagamenti |
| <font color="red">Se il cliente non paga Microsoft</font> | 12/2/2020 – 12/5/2020 | Nessuna modifica, come sopra |
| Il cliente riceve il primo messaggio di posta elettronica di pagamento in ritardo | 12/6/2020 | Nessuno |
| Il cliente riceve messaggi di posta elettronica regolari di urgenza crescente | 12/7/2020 – 1/31/2021 | Nessuno |
| Il server di pubblicazione viene avvisato che è probabile che l'operazione di write-off | 1/7/2021 | Notifica tramite posta elettronica inviata all'editore che indica che il cliente non ha ancora inviato il pagamento. Sono inclusi l'ID transazione e l'importo in dollari. |
| Il cliente riceve un avviso di interruzione | 2/1/2021 | Nessuno |
| Fine del processo di raccolta/i fondi vengono svasi | 2/15/2021 | Notifica tramite posta elettronica inviata all'editore che i fondi sono stati svasi. Sono inclusi l'ID transazione e l'importo in dollari. |
| I pagamenti vengono detratti | 1/3/2021 | Il server di pubblicazione visualizza una transazione negativa nell Partner Center dei pagamenti |
| Il pagamento viene trattenuto | 3/15/2021 | I pagamenti futuri verranno visualizzati nell'Partner Center di pagamento. L'editore non riceverà il pagamento fino a quando il saldo non sarà più negativo.  |
|||

\* La data del pagamento è nell'ora solare Pacifico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Numero di giorni per cui i pagamenti raggiungono un account di pagamento

In genere, il giorno 15 del mese viene inviato qualsiasi pagamento dovuto in un determinato mese, ma il pagamento richiede un altro tempo per raggiungere l'account. Il numero di giorni dipende dal metodo di pagamento che viene utilizzato per l'account, come descritto di seguito.

> [!NOTE]
> I giorni indicati di seguito sono approssimativi. Qualsiasi pagamento può richiedere più o meno tempo per raggiungere l'account.

| Metodo di pagamento     | Numero di giorni per il trasferimento all'account per i proventi     |
|--------------------|--------------------------------------------|
| PayPal             | 1 giorno lavorativo                             |
| ACH/SEPA           | 2-3 giorni lavorativi                          |
| Bonifico bancario      | 7-10 giorni lavorativi                         |
|

## <a name="next-steps"></a>Passaggi successivi

- [Dettagli sulle imposte](tax-details-marketplace.md)
