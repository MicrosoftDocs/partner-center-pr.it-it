---
title: Gestire le prenotazioni di Azure per i clienti
description: Informazioni su come gestire le prenotazioni di Azure per un cliente, tra cui come annullare una prenotazione, scambiare una prenotazione o richiedere un rimborso.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149486"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Gestire, annullare, scambiare o rimborsare Microsoft Azure prenotazioni per i clienti

**Ruoli appropriati:** Agente di amministrazione | Amministratore globale | Supporto dell'agente | Agente di vendita | Amministratore di gestione utenti

Questo articolo illustra come gestire le prenotazioni di Azure per un cliente, incluso come annullare una prenotazione, scambiare una prenotazione o richiedere un rimborso.

> [!NOTE]
> Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP). I clienti che usano altri tipi di sottoscrizioni (ad esempio, sottoscrizioni con pagamento in base al go, singole, Contratto del cliente Microsoft o Contratto Enterprise) devono invece leggere la documentazione sulle prenotazioni di [Azure.](/azure/cost-management-billing/reservations)

Per gestire le prenotazioni di Azure dei clienti dopo l'acquisto, selezionare il cliente e la prenotazione da gestire in Partner Center e quindi apportare modifiche alla prenotazione nel portale di Azure.

1. Per iniziare, selezionare **Clienti** dal menu Partner Center e quindi selezionare il cliente di cui si desidera gestire le prenotazioni. 

2. Nel menu della pagina dei dettagli del cliente selezionare **Prenotazioni di Azure** e quindi selezionare la prenotazione specifica da gestire.  

3. In **Azioni** selezionare **Gestisci** per passare al record di prenotazione del cliente nel portale di Azure. Nella pagina dei dettagli della prenotazione seguire la procedura seguente per completare le attività.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Panoramica**   | Visualizzare i dettagli della prenotazione di un cliente, inclusi la data di scadenza, l'ambito e i dati di utilizzo. **NOTA** Selezionare **Rimborso** per creare una richiesta di supporto per un rimborso con tariffa pro. Selezionare **Exchange** per creare una richiesta di supporto per scambiare la parte inutilizzata del periodo di prenotazione.  
    | **Controllo di accesso (IAM)**   | Gestire l'accesso alle informazioni sulla prenotazione del cliente.|
    | **Configuration**   | Modificare l'ambito della prenotazione e/o la sottoscrizione di Azure a cui è associata la prenotazione.    |
    | **Proprietà**   | Visualizzare le proprietà della prenotazione e copiare negli Appunti l'ID prenotazione e l'ID ordine di prenotazione. **NOTA** Il supporto tecnico può richiedere l'ID prenotazione e l'ID ordine di prenotazione quando si richiede il supporto per conto di un cliente.    |
    | **Nuova richiesta di supporto**    | Richiedere assistenza a Supporto tecnico Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annullare o scambiare una prenotazione

Se in qualsiasi momento l'azienda di un cliente deve cambiare, può voler annullare una prenotazione e ottenere un rimborso o scambiare l'importo del rimborso prorate di una prenotazione da usare per il prezzo di una nuova prenotazione.

In entrambi questi scenari, Microsoft rimborsa l'importo dell'utente in modo da poter gestire le transazioni finanziarie risultanti con i clienti. Microsoft non contatta direttamente i clienti in caso di fatturazione, annullamento o rimborso.

### <a name="how-cancellations-work"></a>Funzionamento degli annullamenti

I clienti possono richiedere di annullare una prenotazione in qualsiasi momento (l'importo del rimborso è limitato a $ 50.000 all'anno). L'annullamento di una prenotazione consente al cliente di restituire l'importo dei mesi rimanenti di una prenotazione di Azure per una tariffa di terminazione anticipata. Il saldo prorate rimanente, meno la tariffa di terminazione anticipata, viene rimborsato all'account in modo da poter rimborsare l'account del cliente. 

Per i dettagli e le tariffe di annullamento, vedere di seguito.


|**Data di annullamento**<br> (giorni)   |**Utilizzo**    |**Credito**  |**Terminazione anticipata**<br> individuale    |**Limite di rimborso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o meno                         | No          | 100%       | No                              | $ 50.000 USD   |
|5 o meno                         | Sì         | Con rate pro  | No                              | $ 50.000 USD   |
|Più di 5                        | No          | Con rate pro  | 12%                             | $ 50.000 USD   |
|Più di 5                        | Sì         | Con rate pro  | 12%                             | $ 50.000 USD   |

### <a name="how-exchanges-work"></a>Funzionamento degli scambi 

Se un cliente vuole acquistare una prenotazione diversa da quella acquistata in origine, può richiedere uno scambio. Lo scambio di una prenotazione può essere un'alternativa interessante all'annullamento di una prenotazione perché consente al cliente di usare l'importo del rimborso prorato rispetto al prezzo della nuova prenotazione. 

L'importo del rimborso rifisso viene accreditato sull'account in modo da poter offrire al cliente uno scambio.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Richiedere un rimborso o uno scambio per conto di un cliente

Per richiedere un rimborso o uno scambio per conto dei clienti, selezionare il cliente e la prenotazione in Partner Center e quindi creare la richiesta di supporto nel portale di Azure. 

>[!NOTE]
>Supporto tecnico Microsoft agenti possono chiedere di specificare l'ID prenotazione e l'ID ordine di prenotazione. Queste informazioni sono disponibili nella pagina Proprietà **della** prenotazione nel portale di Azure.

1. Per iniziare, selezionare **Clienti dal** menu Partner Center e quindi selezionare il cliente che vuole un rimborso. 

2. Nella pagina dei dettagli del cliente selezionare **Prenotazioni di Azure** e quindi selezionare la prenotazione specifica che il cliente vuole rimborsare.  

3. In **Azioni** selezionare **Rimborso** per passare al record di prenotazione del cliente nel portale di Azure e avviare una richiesta di supporto.  

4. Nella pagina **Nuova richiesta di supporto** seguire questa procedura per richiedere un rimborso. Selezionare **Avanti** dopo ogni passaggio. 

   |**Step**                    |**Selezioni**    |
   |:---------------------------|:-----------------|
   |**1 Nozioni di base**                |Tipo di problema: Fatturazione.  |
   |**2 Problema**               |Tipo di problema: Gestione prenotazioni. Categoria: cambi e rimborsi. |
   |**3 Informazioni di contatto**   |Selezionare le preferenze e immettere le informazioni necessarie. 

5. Selezionare **Crea** al termine.

## <a name="azure-reservations-resources"></a>Risorse per le prenotazioni di Azure

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze riservate](azure-reservations.md) |
|Acquisto di prenotazioni di Azure per i clienti in Partner Center   | [Acquistare prenotazioni di Azure](azure-reservations-buying.md) |
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente   | [Ridimensionamento della macchina virtuale per l'utilizzo massimo della prenotazione di Azure](azure-usage.md)   |
|Acquisto di prenotazioni di Azure con l'API Partner Center azure | [Acquistare istanze di macchina virtuale riservate di Azure](/partner-center/develop/purchase-azure-reservations) nella Partner Center per sviluppatori   |
|Concedere ai clienti l'autorizzazione ad acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata per loro. | [Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure](give-customers-permission.md)   |