---
title: Pianificazioni e processi di pagamento
description: Informazioni sui pagamenti e sulle transazioni, ad esempio le pianificazioni dei pagamenti e i processi di recupero per il Marketplace commerciale e altre transazioni.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: 09e1301cb106c9e1ed40ff1fb6f70da92d2695ee
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861411"
---
# <a name="payout-schedules-and-processes"></a>Pianificazioni e processi di pagamento

**Ruoli appropriati:**

- Amministratore degli account
- Amministratore globale

Questo articolo illustra la pianificazione dei pagamenti di Microsoft, la posizione in cui trovare lo stato di un pagamento e il processo per il mancato pagamento del cliente.

## <a name="payment-schedules"></a>Pianificazioni dei pagamenti

Le sezioni seguenti descrivono il processo di pagamento per **contratto Enterprise** e transazioni con **carta di credito/fattura** .

### <a name="enterprise-agreement-transactions"></a>Transazioni Contratto Enterprise

Quando un cliente acquista un prodotto da Microsoft AppSource o Azure Marketplace usando il Contratto Enterprise Microsoft esistente per le transazioni, i pagamenti vengono rilasciati entro 30 giorni dalla fattura del cliente. Le transazioni in cui un cliente usa una carta di credito hanno un periodo di attesa di 30 giorni prima del pagamento.

Si verificherà spesso un versamento prima che Microsoft raccolga i pagamenti dal cliente. Vedere il [processo per i clienti che non](#process-for-customer-non-payment) pagano di seguito per le azioni da intraprendere se il cliente non riesce a pagare Microsoft, ma è già stato emesso un pagamento.

| Event | Descrizione | Visibilità report | Intervallo |
| --- | --- | --- | --- |
| Utilizzo o mese di transazione | Il cliente USA o acquista un servizio. | Dashboard di [utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) o [ordine](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mese 1** |
| Calcolo importo fatturazione Microsoft | Determinare l'utilizzo totale, le transazioni totali | Dashboard di [utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) o [ordine](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mese 2** |
| Fattura pagata dal cliente | Microsoft raccoglie i pagamenti dal cliente | Nessuna modifica | **Mese 2** |
| Pagamento inviato | Determinazione della tariffa dell'Agenzia e degli utili per i pagamenti | Contrassegnato come non elaborato nella cronologia delle transazioni nell' [istruzione payout](payout-statement.md) | **Mese 3 (prima settimana)** |
| Preparare i pagamenti | I guadagni sono preparati per il pagamento mensile | Contrassegnato come imminente nella cronologia delle transazioni nell' [istruzione payout](payout-statement.md) | **Mese 3 (prima settimana)** |
| **Pagamento inviato** | **Il pagamento viene inviato al server di pubblicazione** | **Contrassegnato come inviato nella cronologia delle transazioni e nella sezione relativa ai pagamenti dell'istruzione per il [pagamento](payout-statement.md)** | **Mese 3 (entro il 15)** |
| Fattura pagata dal cliente | Microsoft raccoglie i pagamenti dal cliente | Nessuna modifica | **Dal mese 4 a 12** |
|

\* La data di pagamento è nell'ora solare Pacifico (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Cronologia dei pagamenti per i clienti con contratto Enterprise Agreement.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transazioni con carta di credito o fattura (check/Wire)

Tutti gli acquisti con una carta di credito o una fattura mensile hanno un periodo di attesa di 30 giorni per garantire che i fondi vengano raccolti dal cliente.

| Event | Descrizione | Visibilità report | Intervallo |
| --- | --- | --- | --- |
| Utilizzo o mese di transazione | Il cliente USA o acquista un servizio. | Dashboard di [utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) o [ordine](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mese 1** |
| Fattura pagata dal cliente | Determinare l'utilizzo totale, il valore totale della transazione e la fattura dei clienti | Dashboard di [utilizzo](/azure/marketplace/partner-center-portal/usage-dashboard) o [ordine](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mese 2** |
| Pagamento inviato | Determinazione della tariffa dell'Agenzia e degli utili per i pagamenti | Contrassegnato come non elaborato nella cronologia delle transazioni nell' [istruzione payout](payout-statement.md) | **Mese 2** |
| periodo di attesa di 30 giorni | Verificare la raccolta dei fondi, i chargeback possibili e le richieste di rimborso | Contrassegnato come non elaborato nella cronologia delle transazioni nell' [istruzione payout](payout-statement.md) | **Mese 3** |
| Preparare i pagamenti | I guadagni sono preparati per il pagamento mensile | Contrassegnato come imminente nella cronologia delle transazioni nell' [istruzione payout](payout-statement.md) | **Mese 4 (prima settimana)** |
| **Pagamento inviato** | **Il pagamento viene inviato al server di pubblicazione** | **Contrassegnato come inviato nella cronologia delle transazioni e nella sezione relativa ai pagamenti dell'istruzione per il [pagamento](payout-statement.md)** | **Mese 4 (entro il 15)** |
|

\* La data di pagamento è nell'ora solare Pacifico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Cronologia dei pagamenti per i clienti con carta di credito e fattura.":::

## <a name="process-for-customer-non-payment"></a>Processo per il mancato pagamento del cliente

In rare occasioni, Microsoft non è in grado di raccogliere i pagamenti dei clienti per gli acquisti in Marketplace commerciali. Quando un cliente non riesce a pagare Microsoft in base alla pianificazione di fatturazione, inizia il processo di raccolta. Questo processo richiede circa quattro mesi e implica una comunicazione permanente da Microsoft. Se il pagamento non viene ricevuto entro la fine di questo processo, Microsoft scrive i fondi come non raccolti.

In base al processo di pagamento, Microsoft potrebbe avere già pagato fondi per gli editori (l'utente) che non sono in definitiva disponibili per la raccolta. Quindi, abbiamo un processo per la riconciliazione di questi importi. Per assicurarsi che il pagamento (già ricevuto) venga riconciliato, si riceverà una notifica quando un cliente si trova nel processo di raccolta ed è probabile che gli acquisti vengano scritti.

Microsoft effettuerà il recupero di tutti i pagamenti già effettuati utilizzando uno dei metodi seguenti: (1) Microsoft può sottrarre gli importi non pagati dai pagamenti futuri; Se, ad esempio, $1.000 nei pagamenti sono considerati non raccoglibili e scritti, i pagamenti futuri verranno trattenuti fino a quando non viene recuperato il $1.000 oppure (2) Microsoft potrebbe richiedere un rimborso o fatturare gli editori per eventuali importi non raccolti.

Di seguito è riportato un esempio di pianificazione:

| Evento | Data approssimativa * | Visibilità del partner |
| --- | --- | --- |
| Data di pagamento di esempio | 10/15/2020 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione pagamenti nel dashboard dei pagamenti |
| <font color="red">Se il cliente non paga Microsoft</font> | 12/2/2020 – 12/5/2020 | Nessuna modifica, come sopra |
| Il cliente riceve il primo messaggio di posta elettronica in ritardo | 12/6/2020 | nessuno |
| Il cliente riceve messaggi di posta elettronica regolari con urgenza crescente | 12/7/2020 – 1/31/2021 | nessuno |
| È probabile che il server di pubblicazione riceva una notifica di scrittura | 1/7/2021 | Notifica tramite posta elettronica inviata al server di pubblicazione a cui il cliente non ha ancora inviato il pagamento. Sono inclusi ID transazione e importo in dollari. |
| Il cliente riceve l'avviso di terminazione | 2/1/2021 | nessuno |
| Il processo di raccolta termina/Funds viene scritto | 2/15/2021 | Notifica tramite posta elettronica inviata al server di pubblicazione. i fondi sono stati scritti. Sono inclusi ID transazione e importo in dollari. |
| Il pagamento viene sottratto | 1/3/2021 | Il server di pubblicazione visualizzerà una transazione negativa nell'istruzione per il pagamento del partner Center |
| Il pagamento è stato trattenuto | 3/15/2021 | I pagamenti futuri verranno visualizzati nell'istruzione per il pagamento del centro per i partner. Il server di pubblicazione non riceverà alcun pagamento finché il saldo non sarà più negativo.  |
|||

\* La data di pagamento è nell'ora solare Pacifico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Numero di giorni per i pagamenti per raggiungere un account di pagamento

In genere si inviano pagamenti a causa di un determinato mese il 15 ° giorno del mese, ma è necessario più tempo per il pagamento per raggiungere l'account. Il numero di giorni dipende dal metodo di pagamento usato per l'account, come descritto di seguito.

> [!NOTE]
> I giorni indicati di seguito sono approssimativi; eventuali pagamenti possono richiedere più o meno tempo per raggiungere l'account.

| Metodo di pagamento     | Numero di giorni per il trasferimento all'account per i proventi     |
|--------------------|--------------------------------------------|
| PayPal             | 1 giorno lavorativo                             |
| ACH/SEPA           | 2-3 giorni lavorativi                          |
| Bonifico bancario      | 7-10 giorni lavorativi                         |
|

## <a name="next-steps"></a>Passaggi successivi

- [Dettagli sulle imposte](tax-details-marketplace.md)
