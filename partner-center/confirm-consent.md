---
title: Conferma cliente accettazione del contratto Microsoft Cloud | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: cliente, i clienti, il consenso
ms.localizationpriority: medium
ms.openlocfilehash: 356782420046cb8b49ac4e05981becd253d7049a
ms.sourcegitcommit: dcc0517b2441c5577994b802c455fc726cc5cb35
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/10/2019
ms.locfileid: "9000031"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Conferma cliente accettazione del contratto Microsoft Cloud

**Ambito di applicazione**
-  Centro per i partner

Come partner, è necessario ottenere accettazione del cliente del contratto Microsoft Cloud per ordinare i prodotti Microsoft e i servizi per tale cliente. Per aiutare meglio i partner soddisfano i requisiti di conformità, Microsoft richiede ai partner per confermare l'accettazione, fornendo le seguenti informazioni riguardanti la persona che ha accettato il contratto: 

-   Nome

-   Cognome

-   Indirizzo e-mail

-   Numero di telefono

-   Data di accettazione

Per altre informazioni, vedi la [conferma di accettazione cliente il contratto Microsoft Cloud domande frequenti](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Pianificazione

**7 agosto 2018**

-   I partner di addebito diretto e i provider indiretti confermare l'accettazione dei clienti del contratto Microsoft Cloud. Conferma è *facoltativo*.

-   Conferma di accettazione del cliente può essere eseguita tramite Centro per i Partner o API del centro per i Partner.

-   Conferma di accettazione del cliente è supportata solo con Microsoft Cloud pubblico.


**7 novembre 2018**

-   I partner di addebito diretto e i provider indiretti **devono** conferma l'accettazione cliente il contratto Microsoft Cloud. Conferma è *obbligatorio*.

-   Se conferma non viene fornita per un cliente specificato:

    -   Non sarai in grado di creare nuovi ordini per il cliente.

    -   Non sarai in grado di modificare il numero di postazioni di sottoscrizioni esistenti basati su postazioni per il cliente.

-   Conferma di accettazione del cliente può essere eseguita tramite Centro per i Partner o API del centro per i Partner.

-   Conferma di accettazione del cliente è supportata solo con Microsoft Cloud pubblico.


## <a name="confirming-customer-acceptance-in-partner-center"></a>Confermare l'accettazione dei clienti nel centro per i Partner

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Verifica di accettazione del cliente per un nuovo cliente

Utilizzare la procedura seguente per confermare accettazione del cliente, anche se creare un nuovo tenant cliente nel centro per i Partner. Tieni presente che è necessario essere un agente amministratore o l'agente di vendita per eseguire questa operazione. 
1.  Seleziona **i clienti**, quindi di **nuovo cliente** e quindi seleziona **info dell'Account**.

2.  Immettere le informazioni **sull'azienda** e **contatto principale**.

![Informazioni aziendali](images/mca/mca1.png)

3.  In base al **Contratto Microsoft cloud**, seleziona **il cliente ha accettato il contratto Microsoft cloud più recente**. 

4.  In **Data di accettazione del contratto**di immettere la data appropriata. È possibile impostare questo su una data futura.

5.  Immetti i dettagli dell'utente che ha fornito l'accettazione. 

![Aggiungere una data di accettazione](images/mca/MCA3.png)

Per impostazione predefinita, le informazioni utente contatto primario viene visualizzate. Se questo non è corretto, seleziona **l'aggiornamento** e quindi immetti il **nome**, **Cognome**, l' **indirizzo di posta elettronica**, e **numero di telefono* (facoltativo) della persona che ha accettato il contratto.


6.  Seleziona **Avanti** per continuare con la procedura per creare tenant del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Verifica di accettazione del cliente per un cliente esistente

È necessario essere un agente amministratore o l'agente di vendita per eseguire questa operazione. 

1.  Selezionare **i clienti**, quindi Trova e seleziona il cliente da visualizzare. 

2.  Seleziona **info dell'Account**.

3.  In base al **Contratto Microsoft cloud**, seleziona **l'aggiornamento**.

![Update](images/mca/mca4.png)

4.  Immetti il **nome**, **Cognome**, **indirizzo di posta elettronica**e **numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.

5.  In **Data di accettazione del contratto**di immettere la data appropriata. È possibile impostare questo su una data futura.

6.  Seleziona **Salva e continua**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Verifica di accettazione del cliente durante la creazione di nuovo ordine per un cliente esistente

Se si tenta di creare un nuovo ordine per un cliente esistente che non hai confermato prima, riceverai un prompt dei comandi per completare la conferma. Usa la procedura seguente per eseguire questa operazione. 

1.  Immetti il **nome**, **Cognome**, **indirizzo di posta elettronica**e **numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.

2.  In **Data di accettazione del contratto**di immettere la data appropriata. È possibile impostare questo su una data futura.

3.  Seleziona **Salva e continua**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperare la conferma dell'accettazione del cliente per un cliente esistente

È possibile recuperare conferma di accettazione del cliente per un cliente esistente che hai fornito in precedenza, utilizzando la procedura seguente. È necessario essere un agente amministratore o l'agente di vendita per eseguire questa operazione. 

1.  Selezionare **i clienti**, quindi Trova e seleziona il cliente da visualizzare. 

2.  Seleziona **info dell'Account**.

3.  In base al **Contratto Microsoft cloud**, vedrai o meno conferma è disponibile per il cliente.

