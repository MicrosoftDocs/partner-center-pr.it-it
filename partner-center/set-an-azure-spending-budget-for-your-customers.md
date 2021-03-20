---
title: Impostare un budget di spesa di Azure per i clienti
ms.topic: how-to
ms.date: 03/17/2021
description: Informazioni su come impostare o rimuovere i budget mensili per la spesa di Azure per i clienti e anche per visualizzare i dati di spesa di Azure e impostare le notifiche relative al budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712750"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Imposta, verifica o Rimuovi i budget mensili per la spesa di Azure per i clienti nel centro per i partner

**Ruoli appropriati**

- Agente amministratore

È possibile [impostare un budget mensile per la spesa di Azure per i clienti](#set-azure-spending-budget) nel centro per i partner. Ciò consente ai clienti di gestire la spesa di Azure. Questa opzione consente di confrontare la spesa di Azure da parte dei clienti al budget durante il mese. Consente inoltre ai clienti di ottenere un budget per la spesa di Azure in modo che la fattura mensile non sia più elevata del previsto.

> [!NOTE]  
> Questa funzionalità non è disponibile negli account sandbox o test negli ambienti di produzione (TIP).

Dopo aver [impostato un budget di spesa di Azure per i clienti](#set-azure-spending-budget), è anche possibile esaminare l'utilizzo dei clienti nei modi seguenti. Queste opzioni possono essere utili per individuare i servizi non configurati correttamente o tendenze insolite che potrebbero suggerire frodi. È quindi possibile collaborare con i clienti per identificare la causa principale e gestire i costi. Se necessario, è anche possibile [modificare il budget del cliente impostando](#set-azure-spending-budget) un importo superiore.

- [Controlla la spesa di Azure corrente](#check-current-azure-spending)

- [Attivare le notifiche tramite posta elettronica quando la spesa di un cliente sta per avvicinarsi al limite di budget](#notifications-for-budget-limits)

- [Visualizza i costi in base al servizio per le sottoscrizioni basate sull'utilizzo](#itemized-costs-by-service)

È anche possibile [rimuovere un budget di spesa di Azure](#remove-azure-spending-budget) per i clienti in qualsiasi momento.

## <a name="azure-spending-data"></a>Dati della spesa di Azure

I dati di spesa di Azure sono una *stima* e gli *importi di fatturazione effettivi possono variare*. Il valore dei dati *non riflette* tasse, crediti, rettifiche o altri addebiti che possono essere applicati.

I dati di spesa vengono *aggiornati una volta al giorno*. I clienti possono continuare a usare i servizi e le risorse di Azure, a meno che non si modifichino le impostazioni dell'account nella portale di Azure.

## <a name="set-azure-spending-budget"></a>Imposta budget di spesa di Azure

È possibile *impostare un budget mensile per la spesa di Azure* per più clienti nel centro per i partner:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.

3. Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti per i quali si desidera impostare un budget.

4. Immettere un valore per **budget mensile**.

5. Scegliere **applica** per salvare le modifiche.

È anche possibile *impostare un budget per un singolo cliente* nelle impostazioni della sottoscrizione:

1. Accedere al dashboard Centro per i partner.

2. Nel menu a sinistra in **CSP** scegliere **Customers (clienti**).

3. Nella pagina **Customers** selezionare il **nome della società** del cliente.

4. Nella pagina **sottoscrizioni** del cliente, in **sottoscrizione basata sull'utilizzo**, scegliere **Cambia budget**.

5. Immettere un valore per il budget.

6. Scegliere **applica** per salvare le modifiche.

## <a name="remove-azure-spending-budget"></a>Rimuovi budget di spesa di Azure

È possibile *rimuovere un budget mensile* per la spesa di Azure per i clienti nel centro per i partner:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.

3. Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, selezionare il cliente o i clienti di cui si desidera rimuovere il budget.

4. Scegliere **Rimuovi budget**.

## <a name="check-current-azure-spending"></a>Controlla la spesa di Azure corrente

Puoi *tenere traccia delle spese di Azure correnti e dei budget mensili dei clienti* in qualsiasi momento:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **spesa di Azure**.

3. Nella pagina **spesa di Azure** , in **clienti con Microsoft Azure sottoscrizioni**, è possibile visualizzare una panoramica dei budget mensili dei clienti, le stime di spesa correnti e la percentuale del budget usato.

## <a name="notifications-for-budget-limits"></a>Notifiche per i limiti del budget

È possibile *attivare le notifiche tramite posta elettronica* quando la spesa mensile del cliente si avvicina al limite di budget. Quando si attiva questa opzione, si riceverà una notifica quando i clienti usano il 80% o più del budget mensile. Questa opzione consente di tenere sotto controllo la fattura di Azure. Per configurare le notifiche di posta elettronica:

1. Accedere al Centro per i partner.

2. Passare a **Impostazioni**.

3. Selezionare **preferenze personali**.

4. Se non è possibile, configurare un indirizzo di posta elettronica preferito.

5. Configurare la lingua preferita per la notifica.

6. Selezionare la scheda **CSP** nella sezione **Preferenze di notifica** .

7. Controllare l'opzione di posta elettronica per la notifica di **spesa di Azure** e **salvare**.


## <a name="itemized-costs-by-service"></a>Costi in base al servizio

È possibile *visualizzare i costi (e l'utilizzo stimato) per servizio per le sottoscrizioni basate sull'utilizzo*:

1. Accedere al Centro per i partner.

2. Nel menu a sinistra in **CSP** scegliere **Customers (clienti**).

3. Nella pagina **Customers** selezionare il **nome della società** del cliente.

4. Nella pagina **sottoscrizioni** del cliente, in **sottoscrizioni basate sull'utilizzo**, selezionare il nome della **sottoscrizione**.

5. Nella pagina della sottoscrizione è possibile esaminare i **costi** in base al servizio e l' **utilizzo stimato** per il mese corrente.


## <a name="next-steps"></a>Passaggi successivi

- [Nuova esperienza commerciale in CSP - Fatturazione di Azure](azure-plan-billing.md)
