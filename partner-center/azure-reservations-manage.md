---
title: Gestire le prenotazioni di Azure per conto del cliente | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to manage Azure reservations on behalf of a customer, including how to cancel a reservation, exchange a reservation, or request a refund.
author: LauraBrenner
ms.author: labrenne
keywords: azure, reservations, manage, billing, buying, cancel, exchange, early termination fee
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b71457f0bd75008db9ed704784a39b082983501d
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252636"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Gestire le prenotazioni di Microsoft Azure per conto dei clienti       

**Si applica a**

-  Centro per i partner
-  Portale di Microsoft Azure 
-  Partner di CSP

To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal. 

1. To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage. 

2. On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.  

3. Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal. Nella pagina dei dettagli della prenotazione segui i passaggi qui sotto per completare le attività.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Panoramica**   | View details of a customer's reservation, including expiration date, scope, and utilization data. **NOTA:** seleziona **Rimborsa** per creare una richiesta di supporto per un rimborso proporzionale. Selezionare **Cambio** per creare una richiesta di supporto in vista del cambio del periodo di prenotazione non utilizzato.  
    | **Access Control (IAM)**   | Manage access to the customer's reservation information.|
    | **Configurazione**   | Change the reservation's scope and/or the Azure subscription the reservation is associated with.    |
    | **Proprietà**   | View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID. **NOTA:** quando chiedi supporto per conto di un cliente, ti potrebbero essere richiesti l'ID della prenotazione e l'ID dell'ordine di prenotazione.    |
    | **New support request**    | Richiedere assistenza al Supporto tecnico Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Annullare o cambiare una prenotazione 

If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.

In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers. Microsoft does not contact customers directly about billing, cancellations, or refunds.   
 

**How cancellations work**

Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year). Cancelling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee. The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account. 

See below for cancellation details and fees.


|**Cancellation date**<br> (days)   |**Usage**    |**Credit**  |**Early termination**<br> individuale    |**Refund cap** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 or fewer                         | No          | 100%       | No                              | $50,000 USD   |
|5 or fewer                         | Sì         | Pro-rated  | No                              | $50,000 USD   |
|More than 5                        | No          | Pro-rated  | 12%                             | $50,000 USD   |
|More than 5                        | Sì         | Pro-rated  | 12%                             | $50,000 USD   |


**How exchanges work** 

If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange. Exchanging a reservation can be an attractive alternative to cancelling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation. 

The prorated refund amount is credited to your account so that you can offer the customer an exchange.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Richiedere un rimborso o un cambio per conto di un cliente 

To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal. 

>[!NOTE]
>Gli agenti del Supporto tecnico Microsoft potrebbero richiedere l'ID della prenotazione e l'ID dell'ordine di prenotazione. You can find this information on the reservation's **Properties** page in the Azure portal. 

1. To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund. 

2. On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.  

3. Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.  

4. Nella pagina **Nuova richiesta di supporto** attieniti alla procedura seguente per richiedere un rimborso. Seleziona **Avanti** dopo ogni passaggio. 

    |**Step**                    |**Selections**    |
    |:---------------------------|:-----------------|
    |**1 Basics**                |Tipo di problema: fatturazione  |
    |**2 Problem**               |Tipo di problema: gestione della prenotazione. Categoria: scambi e rimborsi |
    |**3 Contact information**   |Seleziona le preferenze e immetti le informazioni necessarie. 

5.  Al termine, seleziona **Crea**.

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure
|**For information about**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Sell Microsoft Azure Reserved Instances](azure-reservations.md) |
|Purchasing Azure reservations for your customers in Partner Center   |[Buy Azure reservations](azure-reservations-buying.md) |
|Determinare le dimensioni corrette della macchina virtuale e verificare l'utilizzo di macchine virtuali da parte dei clienti   |[VM sizing for maximum Azure reservation usage](azure-usage.md)   |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner

