---
title: Dettagli dei criteri di pagamento-Marketplace commerciale Microsoft
description: Dettagli relativi ai criteri di pagamento del Marketplace commerciale, incluse le pianificazioni e il recupero.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: mingshen-ms
ms.author: mingshen
ms.date: 04/24/2020
ms.openlocfilehash: 17fedcf4ef3d474eab679a03eecb221c90342a04
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335704"
---
# <a name="payout-policy-details"></a>Dettagli dei criteri dei proventi

Questo articolo illustra il processo di pagamento di Microsoft, la pianificazione dei pagamenti e i criteri di recupero e la posizione in cui trovare lo stato di un pagamento.

## <a name="where-to-find-upcoming-payouts"></a>Dove trovare i pagamenti imminenti

In centro per i partner selezionare l'icona del **payout** nell'angolo superiore destro della schermata:

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Viene illustrata l'icona di pagamento in alto a destra nel portale del centro per i partner.":::

> [!TIP]
> Non tutti i ruoli account hanno accesso alle informazioni sui pagamenti. Per informazioni dettagliate, vedere [ruoli e autorizzazioni](payout-statement.md#roles-and-permissions).

## <a name="payment-schedules"></a>Pianificazioni dei pagamenti

Le sezioni seguenti descrivono il processo di pagamento.

### <a name="enterprise-agreement-transactions-after-may-1-2020"></a>Enterprise Agreement le transazioni dopo il 1 ° maggio 2020

È stato eseguito l'aggiornamento seguente al modello di pagamento per l'editore del Marketplace commerciale:

A partire dal 1 ° maggio 2020, verranno aggiornati i criteri di pagamento relativi ai prodotti acquistati in Microsoft AppSource o Azure Marketplace da parte dei clienti con una Enterprise Agreement Microsoft. Quando un cliente acquista un prodotto da Azure Marketplace o AppSource usando il Enterprise Agreement Microsoft esistente per le transazioni, dopo il 1 ° maggio 2020 inizierà a emettere i pagamenti nel ciclo di pagamento successivo 30 giorni dopo la fattura del cliente. Le transazioni in cui un cliente usa una carta di credito restano invariate e continueranno a avere un periodo di attesa di 30 giorni prima del pagamento. Questa tabella mostra i dettagli relativi alla pianificazione dei pagamenti.

> [!NOTE]
> Per le azioni da eseguire se il cliente non è in grado di pagare ma è già stato emesso un pagamento, vedere il [processo per i clienti che non](#process-for-customer-non-payment) pagano.

| Evento  | Data (UTC) | Visibilità del partner: report del centro per i partner  |  Visibilità del partner: analisi del centro per i partner\* |
| --- | --- | --- | --- |
| Transazione o mese di utilizzo | 8/1/2020 – 8/31/2020 | N/D | **Report sull'utilizzo**: nuovo consumo visualizzato (aggiornato ogni quattro ore)<br>**Report ordini**: N/A |
| Fine termine (mese) | 31/8/2020 | N/D | **Report sull'utilizzo**: consumo finale mensile visualizzato<br>**Report ordini**: N/A |
| Ordine generato | 9/3/2020 – 9/7/2020 | N/D | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Calcolo del guadagno del pagamento | 9/4/2020 – 9/10/2020 | Contrassegnato come non **elaborato** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Pagamento mensile | 10/5/2020 | Contrassegnato come **imminente** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Data di pagamento\** | 10/15/2020 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione relativa ai pagamenti del dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Fattura cliente raccolta | 12/1/2020 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione relativa ai pagamenti del dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi  |
|  |  |  |  |

\* I report sull'utilizzo e sugli ordini sono accessibili nella sezione Analyze del centro per i partner.</br>\** La data di pagamento è nell'ora solare Pacifico (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Clienti che pagano usando la carta di credito o la fattura

Tutti gli acquisti con una carta di credito o una fattura mensile hanno un periodo di attesa di 30 giorni per garantire che i fondi vengano cancellati e che non siano presenti chargeback o sospetti illeciti.

| Evento  | Data (UTC) | Visibilità del partner: report del centro per i partner  |  Visibilità del partner: analisi del centro per i partner\*  |
| --- | --- | --- | --- |
| Transazione o mese di utilizzo | 8/1/2019 - 8/31/2019 | N/D | **Report sull'utilizzo**: nuovo consumo visualizzato (aggiornato ogni quattro ore)<br>**Report ordini**: N/A |
| Fine termine (mese) | 8/31/2019 | N/D | **Report sull'utilizzo**: consumo finale mensile visualizzato<br>**Report ordini**: N/A |
| Ordine generato | 9/3/2019 – 9/7/2019 | N/D | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Fattura cliente raccolta | 9/7/2019 – 9/10/2019 | N/D | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Calcola pagamenti | 9/8/2019 -9/12/2019 | Contrassegnato come non **elaborato** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Pagamento mensile | 5/11/2019\* | Contrassegnato come **imminente** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Data di pagamento\** | 15/11/2019 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione relativa ai pagamenti nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
|  |  |  |  |

\* I report sull'utilizzo e sugli ordini sono accessibili nella sezione Analyze del centro per i partner.</br>\** La data di pagamento è nell'ora solare Pacifico (PST).

### <a name="enterprise-agreement-transactions-prior-to-may-1-2020"></a>Enterprise Agreement le transazioni precedenti al 1 ° maggio 2020

Tutti gli acquisti che si verificano prima della data verranno elaborati e pagati in base alla pianificazione riportata di seguito dopo che Microsoft ha raccolto i pagamenti dai clienti ed elaborato la tariffa per il Marketplace.

| Evento  | Data (UTC)  | Visibilità del partner: report del centro per i partner  |  Visibilità del partner: analisi del centro per i partner\*  |
| --- | --- | --- | --- |
| Transazione o mese di utilizzo | 8/1/2019 – 8/31/2019 | N/D | **Report sull'utilizzo**: nuovo consumo visualizzato (aggiornato ogni quattro ore)<br>**Report ordini**: N/A |
| Fine termine (mese) | 8/31/2019 | N/D | **Report sull'utilizzo**: consumo finale mensile visualizzato<br>**Report ordini**: N/A |
| Ordine generato | 9/3/2019 – 9/7/2019 | N/D | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Fattura cliente raccolta | 12/1/2019 | N/D | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Calcola pagamenti | 12/5/2019 – 12/7/2019 | Contrassegnato come non **elaborato** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Pagamento mensile | 1/5/2019 | Contrassegnato come **imminente** nella cronologia delle transazioni nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
| Data di pagamento\** | 1/15/2019 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione relativa ai pagamenti nel dashboard dei pagamenti | **Report sull'utilizzo**: consumo visualizzato con OrderID/OrderLineItemID<br>**Report ordine**: ordini cliente visualizzati come attivi |
|  |  |  |  |

\* I report sull'utilizzo e sugli ordini sono accessibili nella sezione Analyze del centro per i partner.</br>\** La data di pagamento è nell'ora solare Pacifico (PST).

## <a name="process-for-customer-non-payment"></a>Processo per il mancato pagamento del cliente

In rare occasioni, Microsoft non è in grado di raccogliere i pagamenti dei clienti per gli acquisti in Marketplace commerciali. Quando un cliente non riesce a pagare Microsoft in base alla pianificazione di fatturazione, inizia il processo di raccolta. Questo processo richiede circa quattro mesi e implica una comunicazione permanente da Microsoft. Se il pagamento non viene ricevuto entro la fine di questo processo, Microsoft scrive i fondi come non raccolti.

In base al processo di pagamento, Microsoft potrebbe avere già pagato fondi per gli editori (l'utente) che non sono in definitiva disponibili per la raccolta. Quindi, abbiamo un processo per la riconciliazione di questi importi. Per assicurarsi che il pagamento (già ricevuto) venga riconciliato, si riceverà una notifica quando un cliente si trova nel processo di raccolta ed è probabile che gli acquisti vengano scritti.

Microsoft effettuerà il recupero di tutti i pagamenti già effettuati utilizzando uno dei metodi seguenti: (1) Microsoft può sottrarre gli importi non pagati dai pagamenti futuri; Se, ad esempio, $1.000 nei pagamenti sono considerati non raccoglibili e scritti, i pagamenti futuri verranno trattenuti fino a quando non viene recuperato il $1.000 oppure (2) Microsoft potrebbe richiedere un rimborso o fatturare gli editori per eventuali importi non raccolti.

Nella tabella seguente viene illustrata una pianificazione di esempio:

| Evento | Data approssimativa | Visibilità del partner |
| --- | --- | --- |
| Data di pagamento di esempio | 10/15/2020 | Contrassegnato come **inviato** nella cronologia delle transazioni e nella sezione pagamenti nel dashboard dei pagamenti |
| Se il cliente non paga Microsoft | 12/2/2020 – 12/5/2020 | Nessuna modifica, come sopra |
| Il cliente riceve il primo messaggio di posta elettronica in ritardo | 12/6/2020 | nessuno |
| Il cliente riceve messaggi di posta elettronica regolari con urgenza crescente | 12/7/2020 – 1/31/2021 | nessuno |
| È probabile che il server di pubblicazione riceva una notifica di scrittura | 1/7/2021 | Notifica tramite posta elettronica inviata al server di pubblicazione a cui il cliente non ha ancora inviato il pagamento. Sono inclusi ID transazione e importo in dollari. |
| Il cliente riceve l'avviso di terminazione | 2/1/2021 | nessuno |
| Il processo di raccolta termina/Funds viene scritto | 2/15/2021 | Notifica tramite posta elettronica inviata al server di pubblicazione. i fondi sono stati scritti. Sono inclusi ID transazione e importo in dollari. |
| Il pagamento viene sottratto | 3/1/2021 | Il server di pubblicazione visualizzerà una transazione negativa nell'istruzione per il pagamento del partner Center |
| Il pagamento è stato trattenuto | 3/15/2021 | I pagamenti futuri verranno visualizzati nell'istruzione per il pagamento del centro per i partner. Il server di pubblicazione non riceverà alcun pagamento finché il saldo non sarà più negativo.  |
|||

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Numero di giorni per i pagamenti per raggiungere un account di pagamento

In genere si inviano pagamenti a causa di un determinato mese il 15 ° giorno del mese, ma è necessario più tempo per il pagamento per raggiungere l'account. Il numero di giorni dipende dal metodo di pagamento usato per l'account, come descritto di seguito.

> [!NOTE]
> I giorni indicati di seguito sono approssimativi; eventuali pagamenti possono richiedere una quantità di tempo più lunga o più breve per raggiungere l'account.

| Metodo di pagamento     | Numero di giorni per il trasferimento all'account per i proventi     |
|--------------------|--------------------------------------------|
| PayPal             | 1 giorno lavorativo                             |
| ACH/SEPA           | 2-3 giorni lavorativi                          |
| Bonifico bancario      | 7-10 giorni lavorativi                         |

## <a name="next-step"></a>passaggio successivo

- [Dettagli sulle imposte](tax-details-marketplace.md)
