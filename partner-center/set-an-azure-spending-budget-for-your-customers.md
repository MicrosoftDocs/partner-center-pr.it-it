---
title: Impostare un budget di spesa di Azure per i clienti
ms.topic: how-to
ms.date: 03/17/2021
description: Informazioni su come impostare o rimuovere budget mensili di spesa di Azure per i clienti, visualizzare i dati di spesa di Azure e impostare notifiche correlate al budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855353"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Impostare, controllare o rimuovere i budget di spesa mensili di Azure per i clienti in Partner Center

**Ruoli appropriati:** Agente amministratore

È possibile [impostare un budget di spesa mensile di Azure per i clienti](#set-azure-spending-budget) in Partner Center. Ciò consente ai clienti di gestire la spesa di Azure. Questa opzione consente di confrontare la spesa di Azure dei clienti con il budget durante il mese. Consente inoltre ai clienti di bilanciare la spesa di Azure in modo che la fattura mensile non sia superiore a quanto previsto.

> [!NOTE]  
> Questa funzionalità non è disponibile negli account sandbox o Test in produzione (TIP).

Dopo aver [impostato un budget di spesa di Azure per](#set-azure-spending-budget)i clienti, è anche possibile esaminare l'utilizzo dei clienti nei modi seguenti. Queste opzioni consentono di individuare servizi non configurati correttamente o tendenze insolite che potrebbero suggerire frodi. È quindi possibile collaborare con i clienti per identificare la causa radice e gestire i costi. Se necessario, è anche possibile [modificare il budget del cliente](#set-azure-spending-budget) in un importo superiore.

- [Controllare la spesa corrente di Azure](#check-current-azure-spending)

- [Attivare le notifiche di posta elettronica per quando la spesa di un cliente sta per essere vicina al limite di budget](#notifications-for-budget-limits)

- [Visualizzare i costi in base al servizio per le sottoscrizioni basate sull'utilizzo](#itemized-costs-by-service)

È anche possibile [rimuovere un budget di spesa di Azure](#remove-azure-spending-budget) per i clienti in qualsiasi momento.

## <a name="azure-spending-data"></a>Dati di spesa di Azure

I dati di spesa di Azure sono una *stima e* gli importi di fatturazione effettivi *possono variare.* Il valore dei dati *non riflette* le imposte, i crediti, le rettifiche o altri addebiti applicabili.

I dati di spesa *vengono aggiornati una volta al giorno.* I clienti possono continuare a usare (e addebitare) i servizi e le risorse di Azure, a meno che non si cambino le impostazioni dell'account nel portale di Azure.

## <a name="set-azure-spending-budget"></a>Impostare il budget di spesa di Azure

È possibile *impostare un budget di spesa mensile di Azure* per più clienti in Partner Center:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**

3. Nella pagina Di spesa di **Azure,** in Clienti **con Microsoft Azure sottoscrizioni**, selezionare i clienti per cui si vuole impostare un budget.

4. Immettere un valore per **Budget mensile.**

5. Scegliere **Applica** per salvare le modifiche.

È anche possibile *impostare un budget per un singolo cliente nelle* impostazioni di sottoscrizione:

1. Accedere al dashboard Centro per i partner.

2. Nel menu a sinistra in **CSP** scegliere **Clienti.**

3. Nella pagina **Clienti** selezionare il nome società **del cliente.**

4. Nella pagina Sottoscrizioni **del** cliente, in **Sottoscrizione basata sull'utilizzo** scegliere **Modifica budget.**

5. Immettere un valore per il budget.

6. Scegliere **Applica** per salvare le modifiche.

## <a name="remove-azure-spending-budget"></a>Rimuovere il budget di spesa di Azure

È possibile *rimuovere un budget di spesa mensile* di Azure per i clienti in Partner Center:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**

3. Nella pagina Di spesa di **Azure,** in Clienti con Microsoft Azure **sottoscrizioni**, selezionare i clienti di cui si vuole rimuovere il budget.

4. Scegliere **Rimuovi budget.**

## <a name="check-current-azure-spending"></a>Controllare la spesa corrente di Azure

È possibile *tenere traccia delle spese correnti di Azure e dei budget mensili* dei clienti in qualsiasi momento:

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).

2. Nel menu a sinistra in **CSP** scegliere **Spesa di Azure.**

3. Nella pagina **Di spesa di Azure,** **in** Clienti con sottoscrizioni Microsoft Azure , è possibile visualizzare una panoramica dei budget mensili dei clienti, delle stime di spesa correnti e della percentuale del budget usato.

## <a name="notifications-for-budget-limits"></a>Notifiche per i limiti del budget

È possibile *attivare le notifiche tramite posta elettronica* per quando la spesa mensile del cliente sta per essere vicina al limite di budget. Quando si attiva questa opzione, si riceve una notifica quando i clienti usano l'80% o più del budget mensile. Questa opzione consente di tenere d'occhio la fattura di Azure. Per configurare le notifiche tramite posta elettronica:

1. Accedere al Centro per i partner.

2. Passare a **Impostazioni**.

3. Selezionare **Preferenze personali**.

4. Se non è stato fatto, configurare un indirizzo di posta elettronica preferito.

5. Configurare la lingua preferita per la notifica.

6. Selezionare **la scheda CSP** nella **sezione Preferenze di** notifica.

7. Selezionare l'opzione Posta elettronica per **Notifica di spesa** di Azure e **Salva**.


## <a name="itemized-costs-by-service"></a>Costi in base al servizio

È possibile *visualizzare i costi (e l'utilizzo stimato) in base al servizio per le sottoscrizioni basate sull'utilizzo:*

1. Accedere al Centro per i partner.

2. Nel menu a sinistra in **CSP** scegliere **Clienti**.

3. Nella pagina **Clienti** selezionare il nome della società **del cliente.**

4. Nella pagina Sottoscrizioni **del** cliente, in **Sottoscrizioni basate sull'utilizzo,** selezionare il nome della **sottoscrizione**.

5. Nella pagina della sottoscrizione è possibile esaminare i **costi** in base al servizio e l'utilizzo **stimato** per il mese corrente.


## <a name="next-steps"></a>Passaggi successivi

- [Nuova esperienza commerciale in CSP - Fatturazione di Azure](azure-plan-billing.md)
