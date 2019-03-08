---
title: Conferma di accettazione da parte del cliente del contratto di Microsoft Cloud | Centro per i partner
ms.topic: article
ms.date: 02/22/2019
Description: Come partner, devi ottenere l'accettazione da parte del cliente del contratto di Microsoft Cloud prima di poter ordinare prodotti e servizi Microsoft per tale cliente. Per aiutare i partner soddisfano i requisiti di conformità, Microsoft richieda i partner per confermare l'accettazione, fornendo alcune particolarità, la persona che ha accettato il contratto.
author: LauraBrenner
ms.author: v-petand
keywords: cliente, i clienti, fornire il consenso, MCA, contratto di Microsoft Cloud, i modelli di contratto dei clienti
ms.localizationpriority: medium
ms.openlocfilehash: e8c4b66027eeb9e285bd09a4b77aaf9bb6574188
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587564"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Conferma dell'accettazione del cliente del contratto di Microsoft Cloud

**Si applica a**
-  Centro per i partner

Come partner, devi ottenere l'accettazione da parte del cliente del contratto di Microsoft Cloud prima di poter ordinare prodotti e servizi Microsoft per tale cliente. Per aiutare meglio i partner a soddisfare i requisiti di conformità, Microsoft richiede ai partner di confermare l'accettazione, fornendo i seguenti dettagli riguardanti la persona che ha accettato il contratto: 

-   Nome

-   Cognome

-   Indirizzo e-mail

-   Numero di telefono

-   Data di accettazione

Per altre informazioni, vedere la conferma dell'accettazione di contratto di Microsoft Cloud cliente [Frequently Asked Questions](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Pianificazione

**7 agosto 2018**

-   I partner con fatturazione diretta e i provider indiretti possono confermare l'accettazione da parte del cliente del contratto di Microsoft Cloud. La conferma è *facoltativa*.

-   Conferma dell'accettazione del cliente può essere eseguita tramite Centro per i Partner o Partner Center API.

-   La conferma dell'accettazione da parte del cliente è supportata solo il cloud pubblico di Microsoft.


**7 novembre 2018**

-   Indirizzare i partner di fattura e i provider indiretti **necessario** confermare l'accettazione del cliente del contratto di Microsoft Cloud quando vincolante tramite dashboard del centro per i Partner. La conferma è *obbligatoria*.

-   Se non viene fornita la conferma per un determinato cliente:

    -   Non sarai in grado di creare nuovi ordini per il cliente.

    -   Non sarai in grado di modificare il numero di postazioni degli abbonamenti basati su postazioni esistenti per il cliente.

-   Conferma dell'accettazione del cliente può essere eseguita tramite Centro per i Partner o Partner Center API.

-   La conferma dell'accettazione da parte del cliente è supportata solo il cloud pubblico di Microsoft.

-   Questo vale per gli ambienti sandbox sia di produzione.

**11 marzo 2018**

- Partner bill diretto e indiretto Providersmust confermare l'accettazione del cliente del contratto Microsoft Cloud nell'ambiente sandbox CSP quando vincolante tramite Partner Center API.
- Se non viene fornita la conferma per un determinato cliente:

    - Sarà in grado di creare nuovi ordini per il cliente tramite Partner Center API.
 
    - Sarà possibile modificare il numero di postazioni di sottoscrizioni esistenti basati sulle postazioni per il cliente tramite Partner Center API.
- La conferma dell'accettazione da parte del cliente è supportata solo il cloud pubblico di Microsoft. 

**22 marzo 12018**

- Partner bill diretto e indiretto Providersmust confermare l'accettazione del cliente del contratto Microsoft Cloud nell'ambiente di produzione CSP quando vincolante tramite Partner Center API.

- Se non viene fornita la conferma per un determinato cliente:
  - Sarà in grado di creare nuovi ordini per il cliente tramite Partner Center API.

  - Sarà possibile modificare il numero di postazioni di sottoscrizioni esistenti basati sulle postazioni per il cliente tramite Partner Center API.
-  La conferma dell'accettazione da parte del cliente è supportata solo il cloud pubblico di Microsoft.







## <a name="confirming-customer-acceptance-in-partner-center"></a>Per confermare l'accettazione del cliente nel centro per i Partner

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confermare l'accettazione da parte del cliente o un nuovo cliente

Utilizzare la procedura seguente per confermare l'accettazione del cliente durante la creazione di un nuovo tenant dei clienti nel centro per i Partner. Tieni presente che devi essere un agente amministratore o di vendita per eseguire questa operazione.
 
1.  Selezionare **clienti**e quindi **nuovo cliente** e quindi selezionare **Info sull'Account**.

2.  Immetti le informazioni nei campi **Società** e **Contatto primario**.

![Informazioni sulla società](images/mca/mca1.png)

3.  In **Contratto di Microsoft Cloud**, seleziona **Il cliente ha accettato il contratto di Microsoft Cloud più recente**. 

4.  In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

5.  Immetti i dettagli dell'utente che ha fornito l'accettazione. 

![Aggiungere la data di accettazione](images/mca/MCA3.png)

Per impostazione predefinita, vengono visualizzate le informazioni utente relative al contatto primario. Se queste informazioni non sono corrette, seleziona **Aggiorna**, quindi riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono* (facoltativo) della persona che ha accettato il contratto.

6.  Seleziona **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confermare l'accettazione per un cliente esistente

Devi essere un agente amministratore o di vendita per eseguire questa operazione. 

1.  Seleziona **Clienti**, quindi trova e seleziona il cliente che vuoi visualizzare. 

2.  Selezionare **Info sull'Account**.

3.  In **Contratto di Microsoft Cloud**, seleziona **Aggiorna**.

![Aggiornamenti](images/mca/mca4.png)

4.  Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.

5.  In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

6.  Seleziona **Salva e continua**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confermare l'accettazione da parte del cliente durante la creazione di un nuovo ordine per un cliente esistente

Se tenti di creare un nuovo ordine per un cliente esistente che non hai confermato prima, riceverai una richiesta per completare la conferma. Utilizzare la procedura seguente per eseguire questa operazione. 

1.  Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativa) dell'utente che ha accettato il contratto.

2.  In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

3.  Seleziona **Salva e continua**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente

Puoi recuperare la conferma dell'accettazione da parte del cliente per un cliente esistente che hai fornito in precedenza utilizzando la procedura seguente. Devi essere un agente amministratore o di vendita per eseguire questa operazione. 

1.  Seleziona **Clienti**, quindi trova e seleziona il cliente che vuoi visualizzare. 

2.  Selezionare **Info sull'Account**.

3.  In **Contratto di Microsoft Cloud** potrai vedere se la conferma è stata fornita o meno per tale cliente.

