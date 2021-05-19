---
title: Gestire i prodotti del marketplace & offerte
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usando Partner Center, informazioni su come Cloud Solution Provider può gestire le offerte ISV di terze parti acquistate per i clienti dal marketplace commerciale.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147905"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Gestire prodotti e offerte del marketplace commerciale per i clienti


**Ruoli appropriati:** amministratore globale | Agente amministratore

I partner del programma Cloud Solution Provider (CSP) possono usare il portale di Partner Center per acquistare molte offerte o sottoscrizioni IsV SaaS per i propri clienti dal marketplace commerciale. Dopo aver acquistato un'offerta, è possibile gestirla in diversi modi.

## <a name="view-or-edit-a-subscription"></a>Visualizzare o modificare una sottoscrizione

Dopo aver acquistato una sottoscrizione da un editore ISV di terze parti, è possibile esaminarla o modificarla come segue:

1. Accedere al dashboard Partner Center [e](https://partner.microsoft.com/dashboard)quindi selezionare **Clienti** dal menu di spostamento a sinistra.

2. Selezionare un cliente appropriato e quindi **Sottoscrizioni.** Vengono elencate tutte le sottoscrizioni basate su licenza acquistate per il cliente.

3. Nella **colonna Sottoscrizione** selezionare la sottoscrizione che si vuole visualizzare o modificare. In questo modo sono disponibili altre informazioni per configurare o effettuare il provisioning dell'offerta. Se sono necessarie altre azioni sull'offerta, nella colonna Stato potrebbe essere visualizzato anche lo stato "Azione necessaria". Può anche essere accompagnata da un collegamento al sito dell'editore isv.

4. Dopo aver selezionato la sottoscrizione che si vuole visualizzare o modificare, la pagina dei dettagli della sottoscrizione consente di modificare la sottoscrizione ed eseguire operazioni come:

    - Modificare il nome alternativo della sottoscrizione

    - Aggiungere o ridurre il numero di licenze nella sottoscrizione

    - Annullare la sottoscrizione

    - Disattivare il rinnovo automatico

    - Aggiungere un ID MPN rivenditore indiretto, se applicabile

> [!NOTE]
> Potrebbe essere necessario completare alcuni passaggi definiti dal server di pubblicazione ISV prima di poter eseguire alcune modifiche a una sottoscrizione, ad esempio l'annullamento di una sottoscrizione.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Assegnare licenze e attivare una sottoscrizione per conto di un cliente

Quando si acquista un'offerta Software as a Service (SaaS) fornita da un editore isv (Independent Software Vendor) nel marketplace commerciale, l'editore ISV consente di gestire il processo di assegnazione delle licenze e attivazione della sottoscrizione per conto del cliente.

L'editore deve fornire un collegamento personalizzato e un codice di autorizzazione che identifica l'acquisto specifico.

1. È possibile trovare questo collegamento personalizzato dall'editore ISV in diversi modi:

   - È possibile visualizzare il collegamento dalla pagina di conferma visualizzata dopo l'acquisto di un'offerta SaaS ISV. Per trovare questo collegamento nella pagina, cercare e selezionare **Vai al sito dell'editore**.

   - È possibile visualizzare il collegamento dalla pagina Sottoscrizioni del cliente specifico. Questo collegamento all'editore viene visualizzato nella riga associata all'offerta o alla sottoscrizione ISV acquistata per il cliente.

   - È possibile [recuperare il collegamento usando Partner Center API .](/partner-center/develop/get-activation-link-by-order-line-item)

   > [!NOTE]
   > Per eseguire questa operazione per conto del cliente, potrebbe essere necessario copiare il collegamento personalizzato, incollarlo in un browser privato e immettere le credenziali del cliente.

2. Una volta che si è nel sito o nel sistema dell'editore ISV, l'editore invierà all'utente eventuali passaggi aggiuntivi da eseguire per completare il processo di configurazione del cliente e il provisioning o l'assegnazione delle licenze.

3. In quanto partner del programma CSP che lavora per conto del cliente, si è responsabili di eseguire le attività seguenti:

    - Inviare le informazioni necessarie al server di pubblicazione.

    - Inviare qualsiasi URL richiesto direttamente al cliente (o comunicare direttamente i dettagli relativi a questa sottoscrizione al cliente)

4. Dopo aver fornito le informazioni necessarie all'editore, l'editore eseguirà il provisioning e assegna le licenze appropriate. La fatturazione della sottoscrizione inizierà solo dopo che si verificano gli eventi seguenti:

    - L'editore ISV ha assegnato correttamente le licenze appropriate

    - L'editore ISV ha confermato a Microsoft (tramite un'API di adempimenti SaaS separata) che la configurazione dell'account è stata completata correttamente

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Annullare una sottoscrizione SaaS basata su licenza da un editore ISV

Quando si sottoscrive un prodotto SaaS basato su licenza offerto da un editore ISV all'interno del marketplace commerciale, è possibile annullare la sottoscrizione entro il periodo di annullamento designato. Questo periodo di annullamento cambia a seconda che si abbia una sottoscrizione mensile o annuale. È anche possibile scegliere se rinnovare automaticamente la sottoscrizione.

Per altre informazioni sui periodi di annullamento applicabili, su come annullare o rinnovare automaticamente una sottoscrizione, vedere:

- [Annullare una sottoscrizione](create-a-new-subscription.md#cancel-a-subscription)

- [Rinnovare automaticamente una sottoscrizione del marketplace commerciale](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Aggiungere o rimuovere licenze per una sottoscrizione SaaS

Per le offerte del marketplace commerciale SaaS, è possibile aggiungere o rimuovere licenze utente per una sottoscrizione del cliente.

1. Accedere al dashboard Partner Center [e](https://partner.microsoft.com/dashboard)quindi selezionare **Clienti** dal menu di spostamento a sinistra.

2. Selezionare un cliente appropriato, quindi **selezionare Sottoscrizioni**. Vengono elencate tutte le sottoscrizioni basate su licenza acquistate per il cliente.

3. Nella colonna **Sottoscrizione** selezionare la sottoscrizione da modificare.

4. Nella pagina dei dettagli della sottoscrizione individuare il **campo** Quantità. Qui è possibile aumentare o ridurre il numero di licenze.

5. Modificare la quantità e quindi selezionare **Invia**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gestire le sottoscrizioni usando le API del Centro per i partner

È anche possibile usare le API Partner Center per eseguire la gestione del ciclo di vita e gestire le fatture per le sottoscrizioni. Per altre informazioni, vedere [Creare una sottoscrizione per i prodotti del marketplace commerciale.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Passaggi successivi

- [Acquistare offerte del marketplace commerciale](csp-commercial-marketplace-purchase.md)
- [Informazioni sulla fatturazione nel marketplace commerciale](csp-commercial-marketplace-billing.md)