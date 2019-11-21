---
title: Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente | Centro per i partner
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come confermare l'accettazione da parte del cliente del contratto per i clienti Microsoft. Questo potrebbe essere necessario per ordinare i prodotti e i servizi Microsoft per i clienti.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clienti, consenso, MCA, Contratto Microsoft Cloud, contratto del cliente Microsoft, modelli di contratto del cliente
ms.localizationpriority: medium
ms.openlocfilehash: 9d362f581d0d318b1a457ba6a75db54713fce6bb
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252228"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Conferma accettazione da parte del cliente del contratto Microsoft

Attualmente, prima che un partner CSP possa effettuare l'ordine per conto di un cliente, il cliente deve accettare e firmare il **contratto di Microsoft Cloud**applicabile. Il partner deve quindi confermare l'accettazione da parte del cliente fornendo informazioni sul firmatario a Microsoft. Se non viene fornita la conferma:
- Non sarà possibile creare nuovi ordini per questo cliente.
- Non sarà possibile modificare il numero di postazioni delle sottoscrizioni esistenti basate sul posto per questo cliente.

Per informazioni dettagliate su come confermare l'accettazione del Contratto Microsoft Cloud da parte di un cliente usando l'API o il dashboard Centro per i partner, vedi [Confermare l'accettazione del Contratto Microsoft Cloud](confirm-consent.md).

Il 1° ottobre 2019 Microsoft introdurrà il **contratto del cliente Microsoft** nel programma CSP in sostituzione del Contratto Microsoft Cloud. Per facilitare la migrazione dei partner al nuovo contratto, il Contratto Microsoft Cloud corrente sarà supportato nel programma CSP fino al 31 gennaio 2020. Per altri dettagli sulle date, vedi la tabella seguente:

| Data | Revisione principale | Dettagli |
|------------|------------|--------------------------------|
|1° agosto 2019|Esperienza utente in anteprima disponibile in sandbox|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando il dashboard Centro per i partner nell'ambiente sandbox CSP. I partner con accesso all'ambiente sandbox CSP visualizzano in anteprima le modifiche dell'esperienza utente. I partner senza accesso sandbox possono ottenere informazioni sulle modifiche in questo argomento.|
|3 settembre 2019|API in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate all'API e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|20 settembre 2019|.NET SDK in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando .NET SDK Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate a .NET SDK e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|1° ottobre 2019|Contratto del cliente Microsoft disponibile nell'ambiente di produzione|Microsoft introduce il contratto del cliente Microsoft nel programma CSP in sostituzione del Contratto Microsoft Cloud. I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API e il dashboard Centro per i partner nell'ambiente di produzione. Il Contratto Microsoft Cloud continua a essere supportato nel programma per i partner CSP. Si consiglia tuttavia ai partner di iniziare la migrazione al contratto del cliente Microsoft. Per i nuovi acquisti e per le modifiche del numero di postazioni degli abbonamenti esistenti sarà necessaria la conferma del contratto del cliente Microsoft o del Contratto Microsoft Cloud da parte del partner. Alcune nuove offerte, ad esempio il nuovo piano Azure, richiederanno la conferma del contratto del cliente Microsoft.|
|31 gennaio 2020|Contratto Microsoft Cloud rimosso dalla produzione|Il Contratto Microsoft Cloud non è più accettato nel programma per i partner CSP. Per i nuovi acquisti e per le modifiche del numero di postazioni degli abbonamenti esistenti sarà necessaria la conferma del contratto del cliente Microsoft da parte del partner. Questo requisito si applica ai nuovi clienti e ai clienti esistenti che hanno accettato in precedenza il Contratto Microsoft Cloud.|

## <a name="access-microsoft-customer-agreement-template"></a>Accedi al modello di contratto del cliente Microsoft
I partner possono scaricare manualmente la versione più recente del modello di contratto cliente Microsoft da [qui](https://aka.ms/customeragreement). Si noti che il contratto per i clienti Microsoft è specifico del paese. Quando si richiede il modello di contratto del cliente Microsoft, assicurarsi di selezionare il paese corretto in base alla posizione del cliente. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confermare l'accettazione del cliente tramite l'API/SDK del centro per i partner
I partner possono usare l'API/SDK del centro per i partner per confermare l'accettazione del contratto per i clienti Microsoft. Per informazioni dettagliate sull'API/SDK, vedere:

- [Ottenere i metadati per il contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Ottenere la conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Ottenere un collegamento per il download del modello di contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>Confermare l'accettazione da parte di un cliente nel Centro per i partner
I partner possono confermare l'accettazione da parte del cliente del contratto clienti Microsoft nel centro per i partner per i nuovi clienti e i clienti esistenti.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confermare l'accettazione per i nuovi clienti

Quando si crea il tenant di un nuovo cliente in Centro per i partner, segui questa procedura per confermare l'accettazione del contratto del cliente Microsoft da parte del cliente. Devi essere un agente amministratore o di vendita per eseguire questa procedura.

1. Seleziona **Clienti**, quindi **Nuovo cliente**.

2. In **Informazioni sull'account** immetti le informazioni relative alla società e al contatto principale.

3. In **Microsoft agreement** (Contratto Microsoft) fai clic su **Microsoft Customer Agreement** (Contratto del cliente Microsoft).

4. In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

5. Verifica che le informazioni di contatto dell'utente principale visualizzate siano corrette. Se non sono corrette, fai clic su **Aggiorna** e completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto.

6. Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

![Nuovo cliente](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confermare l'accettazione del cliente per i clienti esistenti

Devi essere un agente amministratore o di vendita per eseguire questa operazione:

1. Seleziona **Clienti**. Individua e seleziona il cliente.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft Customer Agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.

4. Completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto. In **Data di accettazione del contratto**, immetti la data appropriata. Non puoi impostarla su una data futura.

5. Scegli **Salva** e continua.

![Cliente esistente](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperare la conferma dell'accettazione del cliente

Puoi recuperare la conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente esistente seguendo questa procedura. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti**, quindi trova e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) visualizza se il cliente ha fornito o meno la conferma.
