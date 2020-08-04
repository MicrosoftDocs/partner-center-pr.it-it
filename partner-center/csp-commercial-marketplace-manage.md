---
title: Gestione dei prodotti del Marketplace & offerte
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Con il centro per i partner, Scopri in che modo i provider di soluzioni cloud possono gestire le offerte ISV di terze parti acquistate per i clienti dal Marketplace commerciale.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96c07ee9d03b433992632337d13c561d6334a896
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527717"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Gestione dei prodotti e delle offerte del Marketplace commerciale per i clienti

**Si applica a**

- Centro per i partner
- Partner aderenti al programma CSP

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

I partner del programma Cloud Solution Provider (CSP) possono usare il portale del centro per i partner per acquistare molte offerte SaaS o sottoscrizioni ISV per i clienti dal Marketplace commerciale. Una volta acquistata un'offerta, sono disponibili diversi modi per gestirla.

## <a name="view-or-edit-a-subscription"></a>Visualizzare o modificare una sottoscrizione

Dopo aver acquistato una sottoscrizione da un server di pubblicazione ISV di terze parti, è possibile esaminarla o modificarla come indicato di seguito:

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **Customers** dal menu di spostamento a sinistra.

2. Selezionare un cliente appropriato, quindi selezionare **sottoscrizioni**. Verranno elencate tutte le sottoscrizioni basate sulle licenze acquistate per il cliente.

3. Nella colonna **sottoscrizione** selezionare la sottoscrizione che si desidera visualizzare o modificare. In questo modo vengono fornite ulteriori informazioni per la configurazione o il provisioning dell'offerta. Se per l'offerta sono necessarie altre azioni, è possibile che venga visualizzato anche lo stato "azione necessaria" visualizzato nella colonna stato. Questo può essere anche accompagnato da un collegamento al sito dell'editore ISV.

4. Dopo aver selezionato la sottoscrizione che si vuole visualizzare o modificare, la pagina dei dettagli della sottoscrizione consente di modificare la sottoscrizione ed eseguire operazioni come:

    - Modificare il nome alternativo della sottoscrizione

    - Aggiungere/ridurre il numero di licenze nella sottoscrizione

    - Annullare la sottoscrizione

    - Disattiva rinnovo automatico

    - Aggiungere un ID MPN rivenditore indiretto, se applicabile

> [!NOTE]
> Per poter eseguire alcune modifiche a una sottoscrizione, ad esempio l'annullamento di una sottoscrizione, potrebbe essere necessario completare alcuni passaggi definiti dal server di pubblicazione ISV.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Assegnare le licenze e attivare una sottoscrizione per conto di un cliente

Quando si acquista un'offerta SaaS (software as a Service) fornita da un editore di software indipendente (ISV) nel Marketplace commerciale, l'editore ISV consente di gestire il processo di assegnazione delle licenze e di attivazione della sottoscrizione per conto del cliente.

Il server di pubblicazione deve fornire un collegamento personalizzato e un codice di autorizzazione che identifichi l'acquisto specifico.

1. Questo collegamento personalizzato è reperibile nel server di pubblicazione ISV in diversi modi:

   - È possibile visualizzare il collegamento dalla pagina di conferma visualizzata dopo l'acquisto di un'offerta SaaS ISV. Per trovare il collegamento nella pagina, cercare e selezionare **Vai al sito del server di pubblicazione**.

   - È possibile visualizzare il collegamento dalla pagina sottoscrizioni del cliente specifico. Questo collegamento all'editore viene visualizzato nella riga associata all'offerta ISV o alla sottoscrizione acquistata per il cliente.

   - È possibile [recuperare il collegamento usando le API del centro per i partner](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Per eseguire questa operazione per conto del cliente, potrebbe essere necessario copiare il collegamento personalizzato, incollarlo in un browser privato e immettere le credenziali del cliente.

2. Quando ci si trova nel sito o nel sistema dell'editore ISV, il server di pubblicazione informerà eventuali passaggi aggiuntivi necessari per completare il processo di configurazione del cliente ed effettuare il provisioning o assegnare le licenze.

3. Un partner del programma CSP che lavora per conto del cliente è responsabile dell'esecuzione delle attività seguenti:

    - Inviare le informazioni necessarie al server di pubblicazione.

    - Inviare un URL necessario direttamente al cliente (o in altro modo comunicare direttamente i dettagli relativi a questa sottoscrizione al cliente)

4. Una volta fornite le informazioni necessarie al server di pubblicazione, il server di pubblicazione effettuerà il provisioning delle licenze appropriate. La fatturazione della sottoscrizione viene avviata solo dopo che si verificano gli eventi seguenti:

    - Il server di pubblicazione ISV ha assegnato le licenze appropriate

    - Il server di pubblicazione ISV ha confermato Microsoft (tramite un'API di evasione SaaS separata) che la configurazione dell'account è stata completata correttamente.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV

Quando si sottoscrive un prodotto SaaS basato su licenza offerto da un editore ISV all'interno del Marketplace commerciale, è possibile annullare la sottoscrizione entro il periodo di annullamento designato. Questo periodo di annullamento cambia a seconda che si disponga di una sottoscrizione mensile o annuale. È anche possibile scegliere se rinnovare automaticamente la sottoscrizione.

Per ulteriori informazioni sui periodi di annullamento applicabili, su come annullare o su come rinnovare automaticamente una sottoscrizione, vedere:

- [Annulla una sottoscrizione](create-a-new-subscription.md#cancel-a-subscription)

- [Rinnovo automatico di una sottoscrizione di Marketplace commerciale](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Aggiungere o rimuovere licenze per una sottoscrizione SaaS

Per le offerte del Marketplace commerciale SaaS, è possibile aggiungere o rimuovere le licenze utente per una sottoscrizione del cliente.

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **Customers** dal menu di spostamento a sinistra.

2. Selezionare un cliente appropriato, quindi selezionare **sottoscrizioni**. Verranno elencate tutte le sottoscrizioni basate sulle licenze acquistate per il cliente.

3. Nella colonna **sottoscrizione** selezionare la sottoscrizione che si desidera modificare.

4. Nella pagina Dettagli sottoscrizione individuare il campo **quantità** . Questo è il punto in cui è possibile aumentare o ridurre il numero di licenze.

5. Modificare la quantità, quindi selezionare **Invia**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gestire le sottoscrizioni usando le API del Centro per i partner

È anche possibile usare le API del centro per i partner per eseguire la gestione del ciclo di vita e gestire le fatture per le sottoscrizioni. Per ulteriori informazioni, vedere [la pagina relativa alla creazione di una sottoscrizione per prodotti Marketplace commerciali](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Passaggi successivi

- [Acquista offerte per Marketplace commerciali](csp-commercial-marketplace-purchase.md)
- [Informazioni sulla fatturazione nel Marketplace commerciale](csp-commercial-marketplace-billing.md)