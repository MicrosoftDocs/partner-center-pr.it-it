---
title: Gestisci prenotazioni di Azure per i clienti
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come gestire le prenotazioni di Azure per un cliente, tra cui come annullare una prenotazione, scambiare una prenotazione o richiedere un rimborso.
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3197f2281ef4a41a200e08290712218c634d1f52
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435760"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Gestione, annullamento, scambio o rimborso Microsoft Azure prenotazioni per i clienti

**Si applica a**

- Centro per i partner
- Portale di Microsoft Azure 
- Partner in CSP

**Ruoli appropriati**

- Agente amministratore
- Amministratore globale
- Agente di supporto tecnico
- Agente di vendita
- Amministratore gestione utenti

Per gestire le prenotazioni di Azure per i clienti dopo l'acquisto, selezionare il cliente e la prenotazione da gestire nel centro per i partner e quindi apportare modifiche alla prenotazione nel portale di Azure.

1. Per iniziare, selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente di cui si desidera gestire le prenotazioni. 

2. Nel menu della pagina dei dettagli del cliente selezionare **prenotazioni di Azure** e quindi selezionare la prenotazione specifica che si vuole gestire.  

3. In **azioni**selezionare **Gestisci** per passare al record di prenotazione del cliente nel portale di Azure. Nella pagina Dettagli prenotazione, attenersi alla procedura seguente per completare le attività.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Panoramica**   | Visualizza i dettagli della prenotazione di un cliente, inclusi i dati relativi alla data di scadenza, all'ambito e all'utilizzo. **Nota** Selezionare **rimborso** per creare una richiesta di supporto per un rimborso con valutazione Pro. Selezionare **Exchange** per creare una richiesta di supporto per scambiare la parte inutilizzata del periodo di prenotazione.  
    | **Controllo di accesso (IAM)**   | Consente di gestire l'accesso alle informazioni di prenotazione del cliente.|
    | **Configuration**   | Modificare l'ambito della prenotazione e/o la sottoscrizione di Azure a cui è associata la prenotazione.    |
    | **Proprietà**   | Visualizzare le proprietà della prenotazione e copiare negli Appunti l'ID prenotazione e l'ID ordine di prenotazione. **Nota** Il supporto tecnico potrebbe richiedere l'ID prenotazione e l'ID ordine di prenotazione quando si richiede il supporto per conto di un cliente.    |
    | **Nuova richiesta di supporto**    | Richiedere assistenza da supporto tecnico Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annulla o scambia una prenotazione

Se in qualsiasi momento le esigenze dell'azienda del cliente cambiano, è possibile che si desideri annullare una prenotazione e ottenere un rimborso o scambiare un importo di rimborso proporzionale della prenotazione da utilizzare per il prezzo di una nuova prenotazione.

In entrambi i casi, Microsoft rimborserà l'importo per poter gestire le transazioni finanziarie risultanti con i clienti. Microsoft non contatta i clienti direttamente in merito a fatturazione, annullamento o rimborsi.

### <a name="how-cancellations-work"></a>Funzionamento degli annullamenti

I clienti possono richiedere di annullare una prenotazione in qualsiasi momento (importo del rimborso limitato a $50.000 all'anno). L'annullamento di una prenotazione consente al cliente di restituire la quantità di mesi rimanenti di una prenotazione di Azure per una tariffa di terminazione anticipata. Il saldo proporzionale rimanente, meno il costo di terminazione anticipato, viene rimborsato al proprio account in modo che sia possibile rimborsare l'account del cliente. 

Per informazioni dettagliate sull'annullamento e tariffe, vedere di seguito.


|**Data di annullamento**<br> giorni   |**Utilizzo**    |**Credito**  |**Terminazione anticipata**<br> individuale    |**Limite di rimborso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o un numero inferiore                         | No          | 100%       | No                              | $50.000 USD   |
|5 o un numero inferiore                         | Sì         | Con classificazione Pro  | No                              | $50.000 USD   |
|Più di 5                        | No          | Con classificazione Pro  | 12%                             | $50.000 USD   |
|Più di 5                        | Sì         | Con classificazione Pro  | 12%                             | $50.000 USD   |

### <a name="how-exchanges-work"></a>Come funzionano gli scambi 

Se un cliente vuole acquistare una prenotazione diversa da quella acquistata originariamente dall'utente, può richiedere uno scambio. Lo scambio di una prenotazione può essere un'alternativa interessante per annullare una prenotazione, perché consente al cliente di usare l'importo del rimborso proporzionale verso il prezzo della nuova prenotazione. 

L'importo del rimborso proporzionale è accreditato per l'account, in modo da poter offrire al cliente uno scambio.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Richiedere un rimborso o uno scambio per conto di un cliente

Per presentare una richiesta di supporto per un rimborso o uno scambio per conto dei clienti, selezionare il cliente e la prenotazione nel centro per i partner e quindi creare la richiesta di supporto nella portale di Azure. 

>[!NOTE]
>Supporto tecnico Microsoft agenti potrebbero richiedere di specificare l'ID prenotazione e l'ID dell'ordine di prenotazione. È possibile trovare queste informazioni nella pagina delle **Proprietà** della prenotazione nel portale di Azure.

1. Per iniziare, selezionare **Customers** dal menu partner Center e quindi selezionare il cliente che desidera un rimborso. 

2. Nella pagina dei dettagli del cliente selezionare **prenotazioni di Azure** e quindi selezionare la prenotazione specifica che il cliente desidera rimborsare.  

3. In **azioni**selezionare **rimborso** per passare al record di prenotazione del cliente nel portale di Azure e avviare una richiesta di supporto.  

4. Nella pagina **nuova richiesta di supporto** , attenersi alla procedura seguente per richiedere un rimborso. Selezionare **Avanti** dopo ogni passaggio. 

   |**Step**                    |**Selezioni**    |
   |:---------------------------|:-----------------|
   |**1 Nozioni di base**                |Tipo di problema: fatturazione.  |
   |**2 problema**               |Tipo di problema: gestione prenotazione. Categoria: scambi e rimborsi. |
   |**3 informazioni di contatto**   |Selezionare le preferenze e immettere le informazioni necessarie. 

5. Selezionare **Crea** al termine.

## <a name="azure-reservations-resources"></a>Risorse per le prenotazioni di Azure

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica sulle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze riservate](azure-reservations.md) |
|Acquisto di prenotazioni di Azure per i clienti nel centro per i partner   | [Acquista prenotazioni di Azure](azure-reservations-buying.md) |
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo della macchina virtuale del cliente   | [Dimensionamento delle VM per l'utilizzo massimo della prenotazione di Azure](azure-usage.md)   |
|Acquisto di prenotazioni di Azure tramite l'API del centro per i partner | [Acquistare istanze di VM riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner   |
|Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata. | [Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure](give-customers-permission.md)   |

