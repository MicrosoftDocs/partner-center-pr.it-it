---
title: Confermare l'accettazione del contratto del cliente Microsoft | Centro per i partner
ms.topic: article
ms.date: 04/16/2019
Description: In qualità di partner, è necessario ottenere l'accettazione del contratto del cliente Microsoft prima di poter ordinare i prodotti e i servizi Microsoft per tale cliente. Per aiutare i partner a soddisfare i requisiti di conformità, Microsoft chiede ai partner di confermare l'accettazione fornendo determinati dettagli relativi all'utente che ha accettato il contratto.
author: LauraBrenner
ms.author: labrenne
keywords: clienti, clienti, consenso, MCA, Microsoft Cloud Agreement, contratto del cliente Microsoft, modelli di contratto del cliente
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681757"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confermare l'accettazione del contratto per i clienti Microsoft (anteprima)

Attualmente, prima che un partner CSP possa effettuare l'ordine per conto di un cliente, il cliente deve accettare e firmare il **contratto di Microsoft Cloud**applicabile. Il partner deve quindi confermare l'accettazione da parte del cliente fornendo informazioni sul firmatario a Microsoft. Se un cliente non conferma l'accettazione del Microsoft Cloud contratto:
- Non sarai in grado di creare nuovi ordini per il cliente.
- Non sarai in grado di modificare il numero di postazioni degli abbonamenti basati su postazioni esistenti per il cliente.

Per informazioni dettagliate su come confermare l'accettazione da parte di un cliente del contratto di Microsoft Cloud usando il dashboard o l'API del centro per i partner, vedere [confermare l'accettazione del contratto Microsoft Cloud da](confirm-consent.md)parte del cliente.

Il 1 ° ottobre 2019 Microsoft introdurrà il **contratto del cliente Microsoft** per il programma CSP per sostituire il contratto di Microsoft Cloud. Per facilitare la migrazione dei partner al nuovo contratto, il contratto di Microsoft Cloud corrente sarà supportato nel programma CSP fino al 31 gennaio 2019. Per altri dettagli sulla cronologia, vedere la tabella seguente:

| Date | Revisione principale | Dettagli |
|------------|------------|--------------------------------|
|01 agosto 2019|Anteprima di UX disponibile in sandbox|I partner possono confermare l'accettazione del contratto del cliente Microsoft usando il dashboard del centro per i partner nell'ambiente sandbox CSP. I partner con accesso all'ambiente sandbox CSP visualizzano in anteprima le modifiche apportate all'esperienza utente. I partner senza accesso sandbox possono ottenere informazioni sulle modifiche apportate in questo argomento.|
|02 settembre, 2019|L'anteprima dell'API è disponibile in sandbox.|Il partner può confermare l'accettazione del contratto del cliente Microsoft mediante l'API del centro per i partner nell'ambiente CSP sandbox. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate all'API e iniziare a lavorare con l'integrazione dell'API per supportare il nuovo contratto.|
|01 ottobre 2019|Contratto clienti Microsoft disponibile nell'ambiente di produzione|Microsoft introduce il contratto del cliente Microsoft per il programma CSP per sostituire il contratto di Microsoft Cloud. I partner possono confermare l'accettazione del contratto del cliente Microsoft usando il dashboard e l'API del centro per i partner nell'ambiente di produzione. Il contratto di Microsoft Cloud rimane supportato nel programma per i partner CSP. Tuttavia, si consiglia ai partner di iniziare la migrazione al contratto per i clienti Microsoft. Le modifiche apportate ai nuovi acquisti e al numero di postazioni alle sottoscrizioni esistenti richiedono la conferma del partner per il contratto del cliente Microsoft o per il contratto Microsoft Cloud. Alcune nuove offerte, ad esempio il nuovo piano Azure, richiedono la conferma del contratto per i clienti Microsoft.|
|31 gennaio 2019|Microsoft Cloud accordo rimosso dalla produzione|Il contratto di Microsoft Cloud non è più accettato nel programma per i partner CSP. I nuovi acquisti e le modifiche ai conteggi delle postazioni per le sottoscrizioni esistenti richiederanno al partner di fornire la conferma del contratto per i clienti Microsoft. Questo requisito si applica ai nuovi clienti e ai clienti esistenti che hanno accettato in precedenza il contratto Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Conferma accettazione del cliente per i nuovi clienti

Quando si crea un nuovo tenant del cliente nel centro per i partner, attenersi alla procedura seguente per confermare l'accettazione da parte del cliente del contratto per i clienti Microsoft. Per eseguire questa procedura, è necessario essere un agente di amministrazione o un agente di vendita.

1. Seleziona **Clienti**, quindi **Nuovo cliente**.

2. In **Info account**immettere le informazioni per la società e il contatto principale.

3. In **Contratto Microsoft**selezionare il contratto per i **clienti Microsoft**.

4. In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

5. Verificare che le informazioni di contatto dell'utente principale visualizzate siano corrette. Se non è corretta, selezionare **Aggiorna** e immettere il **nome**, il **Cognome**, l' **indirizzo di posta elettronica**e il numero di **telefono** (facoltativo) dell'utente che ha accettato il contratto.

6. Seleziona **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

![Nuovo cliente](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Conferma accettazione del cliente per i clienti esistenti

Per eseguire questa operazione, è necessario essere un agente di amministrazione o un agente di vendita:

1. Selezionare **Customers**. Trovare e selezionare il cliente.

2. Selezionare le **informazioni sull'account**.

3. In **contratto cliente Microsoft**selezionare **Aggiorna**.

4. Immettere il **nome**, il **Cognome**, l' **indirizzo di posta elettronica**e il **numero di telefono** (facoltativo) dell'utente che ha accettato il contratto. In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

5. Selezionare **Salva** e continua.

![Cliente esistente](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Recupera la conferma dell'accettazione del cliente

È possibile recuperare la conferma che un cliente esistente ha accettato il contratto del cliente Microsoft attenendosi alla procedura seguente. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti**, quindi trova e seleziona il cliente che vuoi visualizzare.

2. Selezionare le **informazioni sull'account**.

3. Nel **Contratto Microsoft Cloud**, visualizzare se la conferma è stata o non è stata fornita da questo cliente.


