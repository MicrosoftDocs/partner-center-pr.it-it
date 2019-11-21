---
title: Conferma di accettazione da parte del cliente del contratto di Microsoft Cloud | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to confirm customer acceptance of the Microsoft Cloud Agreement. This may be needed to order Microsoft products and services for customers.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, customer agreement templates
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252587"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Conferma dell'accettazione del cliente del contratto di Microsoft Cloud

**Si applica a**
-  Centro per i partner

> [!NOTE]
> The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only. It is not applicable to:
> * Centro per i partner gestito da 21Vianet
> * Centro per i partner per Microsoft Cloud Germania
> * Centro per i partner per Microsoft Cloud for US Government

>[!NOTE]
>This agreement is valid until January 31, 2020. After that date, all customers, existing and new, must sign the new Microsoft Customer Agreement. To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).

As a partner, you need to obtain your customer's acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione, fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto: 

-   Nome

-   Cognome

-   Indirizzo e-mail

-   Numero di telefono (facoltativo)

-   Data di accettazione

To learn more, see the Microsoft Cloud Agreement customer acceptance confirmation [Frequently Asked Questions](https://docs.microsoft.com/partner-center/confirm-consent-faq).

Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Cloud Agreement when transacting through Partner Center or Partner Center API. La conferma è *obbligatoria*.

Se non viene fornita la conferma per un determinato cliente:

-   You won't be able to create new orders for this customer.

-   You won't be able to change the seat count of existing seat-based subscriptions for this customer.

Confirmation of customer acceptance can be done via Partner Center or the Partner Center API. To do this through the Partner Center API, see the following topics: 

-   [Get confirmation of customer consent](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Get agreement metadata](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirm customer consent](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


This applies to both production and sandbox environments.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirming customer acceptance in Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confermare l'accettazione da parte del cliente o un nuovo cliente

Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center. Tieni presente che devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Select **Customers**, and then **New customer** and then select **Account info**.
2. Immetti le informazioni nei campi **Società** e **Contatto primario**.

![Company information](images/mca/mca1.png)

3. In **Contratto di Microsoft Cloud**, seleziona **Il cliente ha accettato il contratto di Microsoft Cloud più recente**.
4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
5. Immetti i dettagli dell'utente che ha fornito l'accettazione.

![Add acceptance date](images/mca/MCA3.png)

Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto primario. If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and **Phone number* (optional) of the person who accepted the agreement.

6. Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confermare l'accettazione per un cliente esistente

Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.
2. Seleziona **Informazioni sull'account**.
3. In **Contratto di Microsoft Cloud**, seleziona **Aggiorna**.

![scheda Aggiorna](images/mca/mca4.png)

4. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.
5. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
6. Seleziona **Salva e continua**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente

If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation. A tale scopo, utilizza la procedura seguente.

1. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.
2. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
3. Seleziona **Salva e continua**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente

Puoi recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente che hai fornito in precedenza utilizzando la procedura seguente. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.
2. Seleziona **Informazioni sull'account**.
3. Under **Microsoft cloud agreement**, you'll see whether or not confirmation has been provided for this customer.
