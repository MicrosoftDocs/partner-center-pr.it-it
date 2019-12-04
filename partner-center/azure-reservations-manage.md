---
title: Gestire le prenotazioni di Azure per conto del cliente | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come gestire le prenotazioni di Azure per conto di un cliente, tra cui come annullare una prenotazione, scambiare una prenotazione o richiedere un rimborso.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, prenotazioni, gestione, fatturazione, acquisto, annullamento, scambio, tariffa per la terminazione anticipata
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: eedfe20cea239918e5ece6f10b2b5f5988da9c50
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722274"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gestire le prenotazioni di Microsoft Azure per conto dei clienti

**Si applica a**

- Centro per i partner
- Portale di Microsoft Azure 
- Partner di CSP

**Ruoli appropriati**

- Agente amministratore
- Amministratore globale
- Agente help desk
- Agente di vendita
- Amministratore gestione utenti

Per gestire le prenotazioni di Azure per i clienti dopo l'acquisto, selezionare il cliente e la prenotazione da gestire nel centro per i partner e quindi apportare modifiche alla prenotazione nel portale di Azure.

1. Per iniziare, selezionare **Customers (clienti** ) dal menu centro partner e quindi selezionare il cliente di cui si desidera gestire le prenotazioni. 

2. Nel menu della pagina dei dettagli del cliente selezionare **prenotazioni di Azure** e quindi selezionare la prenotazione specifica che si vuole gestire.  

3. In **azioni**selezionare **Gestisci** per passare al record di prenotazione del cliente nel portale di Azure. Nella pagina dei dettagli della prenotazione segui i passaggi qui sotto per completare le attività.  

    | **Selezionare**   | **A**    |
    |:-----------------------------|:-----------------|
    | **Panoramica**   | Visualizza i dettagli della prenotazione di un cliente, inclusi i dati relativi alla data di scadenza, all'ambito e all'utilizzo. **NOTA:** seleziona **Rimborsa** per creare una richiesta di supporto per un rimborso proporzionale. Selezionare **Cambio** per creare una richiesta di supporto in vista del cambio del periodo di prenotazione non utilizzato.  
    | **Controllo di accesso (IAM)**   | Consente di gestire l'accesso alle informazioni di prenotazione del cliente.|
    | **Configurazione**   | Modificare l'ambito della prenotazione e/o la sottoscrizione di Azure a cui è associata la prenotazione.    |
    | **Proprietà**   | Visualizzare le proprietà della prenotazione e copiare negli Appunti l'ID prenotazione e l'ID ordine di prenotazione. **NOTA:** quando chiedi supporto per conto di un cliente, ti potrebbero essere richiesti l'ID della prenotazione e l'ID dell'ordine di prenotazione.    |
    | **Nuova richiesta di supporto**    | Richiedere assistenza al Supporto tecnico Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annullare o cambiare una prenotazione 

Se in qualsiasi momento le esigenze dell'azienda del cliente cambiano, è possibile che si desideri annullare una prenotazione e ottenere un rimborso o scambiare un importo di rimborso proporzionale della prenotazione da utilizzare per il prezzo di una nuova prenotazione.

In entrambi i casi, Microsoft rimborserà l'importo per poter gestire le transazioni finanziarie risultanti con i clienti. Microsoft non contatta i clienti direttamente in merito a fatturazione, annullamento o rimborsi.


**Funzionamento degli annullamenti**

I clienti possono richiedere di annullare una prenotazione in qualsiasi momento (importo del rimborso limitato a $50.000 all'anno). L'annullamento di una prenotazione consente al cliente di restituire la quantità di mesi rimanenti di una prenotazione di Azure per una tariffa di terminazione anticipata. Il saldo proporzionale rimanente, meno il costo di terminazione anticipato, viene rimborsato al proprio account in modo che sia possibile rimborsare l'account del cliente. 

Per informazioni dettagliate sull'annullamento e tariffe, vedere di seguito.


|**Data di annullamento**<br> giorni   |**Utilizzo**    |**Credito**  |**Terminazione anticipata**<br> individuale    |**Limite di rimborso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o un numero inferiore                         | No          | 100%       | No                              | $50.000 USD   |
|5 o un numero inferiore                         | Sì         | Con classificazione Pro  | No                              | $50.000 USD   |
|Più di 5                        | No          | Con classificazione Pro  | 12                             | $50.000 USD   |
|Più di 5                        | Sì         | Con classificazione Pro  | 12                             | $50.000 USD   |


**Come funzionano gli scambi** 

Se un cliente vuole acquistare una prenotazione diversa da quella acquistata originariamente dall'utente, può richiedere uno scambio. Lo scambio di una prenotazione può essere un'alternativa interessante per annullare una prenotazione perché consente al cliente di usare l'importo del rimborso proporzionale verso il prezzo della nuova prenotazione. 

L'importo del rimborso proporzionale è accreditato per l'account, in modo da poter offrire al cliente uno scambio.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Richiedere un rimborso o un cambio per conto di un cliente 

Per presentare una richiesta di supporto per un rimborso o uno scambio per conto dei clienti, selezionare il cliente e la prenotazione nel centro per i partner e quindi creare la richiesta di supporto nella portale di Azure. 

>[!NOTE]
>Gli agenti del Supporto tecnico Microsoft potrebbero richiedere l'ID della prenotazione e l'ID dell'ordine di prenotazione. È possibile trovare queste informazioni nella pagina delle **Proprietà** della prenotazione nel portale di Azure. 

1. Per iniziare, selezionare **Customers** dal menu partner Center e quindi selezionare il cliente che desidera un rimborso. 

2. Nella pagina dei dettagli del cliente selezionare **prenotazioni di Azure** e quindi selezionare la prenotazione specifica che il cliente desidera rimborsare.  

3. In **azioni**selezionare **rimborso** per passare al record di prenotazione del cliente nel portale di Azure e avviare una richiesta di supporto.  

4. Nella pagina **Nuova richiesta di supporto** attieniti alla procedura seguente per richiedere un rimborso. Seleziona **Avanti** dopo ogni passaggio. 

    |**Passo**                    |**Selezioni**    |
    |:---------------------------|:-----------------|
    |**1 Nozioni di base**                |Tipo di problema: fatturazione  |
    |**2 problema**               |Tipo di problema: gestione della prenotazione. Categoria: scambi e rimborsi |
    |**3 informazioni di contatto**   |Seleziona le preferenze e immetti le informazioni necessarie. 

5.  Al termine, seleziona **Crea**.

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure
|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze riservate](azure-reservations.md) |
|Acquisto di prenotazioni di Azure per i clienti nel centro per i partner   |[Acquista prenotazioni di Azure](azure-reservations-buying.md) |
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo di macchine virtuali da parte dei clienti   |[Dimensionamento delle VM per l'utilizzo massimo della prenotazione di Azure](azure-usage.md)   |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner

