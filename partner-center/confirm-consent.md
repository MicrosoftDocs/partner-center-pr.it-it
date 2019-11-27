---
title: Conferma di accettazione da parte del cliente del contratto di Microsoft Cloud | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come confermare l'accettazione del Microsoft Cloud contratto da parte del cliente. Questo potrebbe essere necessario per ordinare i prodotti e i servizi Microsoft per i clienti.
author: LauraBrenner
ms.author: labrenne
keywords: Customer, Customers, acconsenti, MCA, Microsoft Cloud Agreement, modelli di contratto del cliente
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
> La risorsa del contratto è attualmente supportata dal centro per i partner nel cloud pubblico Microsoft. Non è applicabile a:
> * Centro per i partner gestito da 21Vianet
> * Centro per i partner per Microsoft Cloud Germania
> * Centro per i partner per Microsoft Cloud for US Government

>[!NOTE]
>Il presente contratto è valido fino al 31 gennaio 2020. Dopo tale data, tutti i clienti, esistenti e nuovi, devono firmare il nuovo contratto per i clienti Microsoft. Per altre informazioni, vedere [confermare l'accettazione del contratto clienti Microsoft](confirm-customer-agreement.md).

In qualità di partner, è necessario ottenere l'accettazione del Microsoft Cloud contratto da parte del cliente prima di poter ordinare i prodotti e i servizi Microsoft per quel cliente. Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione, fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto: 

-   Nome

-   Cognome

-   Indirizzo e-mail

-   Numero di telefono (facoltativo)

-   Data di accettazione

Per ulteriori informazioni, vedere le [domande frequenti](https://docs.microsoft.com/partner-center/confirm-consent-faq)sulla conferma dell'accettazione del cliente Microsoft Cloud contratto.

I partner diretti per la fatturazione e i provider indiretti devono confermare l'accettazione da parte del cliente del contratto Microsoft Cloud durante la transazione tramite l'API del centro per i partner o del centro La conferma è *obbligatoria*.

Se non viene fornita la conferma per un determinato cliente:

-   Non sarà possibile creare nuovi ordini per questo cliente.

-   Non sarà possibile modificare il numero di postazioni delle sottoscrizioni esistenti basate sul posto per questo cliente.

La conferma dell'accettazione del cliente può essere eseguita tramite il centro per i partner o l'API del centro per i partner. Per eseguire questa operazione tramite l'API del centro per i partner, vedere gli argomenti seguenti: 

-   [Ottenere la conferma del consenso del cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Ottenere i metadati del contratto](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Conferma consenso del cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Questo vale sia per gli ambienti di produzione che per quelli sandbox.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Conferma dell'accettazione del cliente nel centro per i partner

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confermare l'accettazione da parte del cliente o un nuovo cliente

Usare la procedura seguente per confermare l'accettazione da parte del cliente durante la creazione di un nuovo tenant del cliente nel centro per i partner. Tieni presente che devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Selezionare **Customers**, quindi **nuovo cliente** , quindi selezionare **Info account**.
2. Immetti le informazioni nei campi **Società** e **Contatto primario**.

![Informazioni sulla società](images/mca/mca1.png)

3. In **Contratto di Microsoft Cloud**, seleziona **Il cliente ha accettato il contratto di Microsoft Cloud più recente**.
4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
5. Immetti i dettagli dell'utente che ha fornito l'accettazione.

![Aggiungi data di accettazione](images/mca/MCA3.png)

Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto primario. Se il problema non è corretto, selezionare **Aggiorna** e quindi immettere il **nome**, il **Cognome**, l' **indirizzo di posta elettronica**e il **numero di telefono* (facoltativo) dell'utente che ha accettato il contratto.

6. Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confermare l'accettazione per un cliente esistente

Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.
2. Seleziona **Informazioni sull'account**.
3. In **Contratto di Microsoft Cloud**, seleziona **Aggiorna**.

![Aggiornamenti](images/mca/mca4.png)

4. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.
5. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
6. Seleziona **Salva e continua**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente

Se si tenta di creare un nuovo ordine per un cliente esistente che non è stato confermato in precedenza, si riceverà un messaggio di richiesta per completare la conferma. Utilizzare la procedura seguente per eseguire questa operazione.

1. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.
2. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.
3. Seleziona **Salva e continua**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente

Puoi recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente che hai fornito in precedenza utilizzando la procedura seguente. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.
2. Seleziona **Informazioni sull'account**.
3. Nel **Contratto Microsoft Cloud**si noterà se è stata fornita una conferma per questo cliente.
