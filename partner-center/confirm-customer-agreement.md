---
title: Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente | Centro per i partner
ms.topic: article
ms.date: 02/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Scopri come confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Questa operazione potrebbe essere necessaria per ordinare prodotti e servizi Microsoft per i clienti.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clienti, consenso, MCA, Contratto Microsoft Cloud, contratto del cliente Microsoft, modelli di contratto del cliente
ms.localizationpriority: high
ms.openlocfilehash: 51bfe2c132b4c5ba5d9b285164ee99a29cfcc22f
ms.sourcegitcommit: 43569a21c4f5cb5405f2acea6ace69640a2eee5e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/07/2020
ms.locfileid: "80805983"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente

**Si applica a**

- Centro per i partner
- Interfaccia di amministrazione di Microsoft 365

**Ruoli appropriati**

- Agente amministratore
- Agente di vendita

**Tipi di partner appropriati**

- Rivenditori indiretti, partner con fatturazione diretta, provider indiretti


Il 1° ottobre 2019 Microsoft ha introdotto il **contratto del cliente Microsoft** nel programma CSP in sostituzione del Contratto Microsoft Cloud. Sono disponibili altre [indicazioni](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fpartner-center%2Findirect-reseller-tasks-in-partner-center&data=02%7C01%7CChelsea.Kajs%40microsoft.com%7Cd5e0adc6b10646352ce508d7a4e84251%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637159189767080601&sdata=%2BPAWMBPVbVBkTx25r9CoD7cQxRqRVEYkxWIilrwwxZc%3D&reserved=0) per i rivenditori indiretti. Per facilitare la migrazione dei partner al nuovo contratto, il programma CSP ha previsto la coesistenza di entrambi i contratti fino al 31 gennaio 2020. A partire dal 1° febbraio 2020, il Contratto del cliente Microsoft ha sostituito il Contratto Microsoft Cloud. Per informazioni, vedi [Contratto del cliente Microsoft e come confermare il consenso](confirm-customer-agreement.md).

Per altri dettagli sulle date, vedi la tabella seguente:

| Data | Attività cardine | Dettagli |
|------------|------------|--------------------------------|
|1° agosto 2019|Esperienza utente in anteprima disponibile in sandbox|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando il dashboard Centro per i partner nell'ambiente sandbox CSP. I partner con accesso all'ambiente sandbox CSP visualizzano in anteprima le modifiche dell'esperienza utente. I partner senza accesso sandbox possono ottenere informazioni sulle modifiche in questo argomento.|
|3 settembre 2019|API in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate all'API e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|20 settembre 2019|.NET SDK in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando .NET SDK Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate a .NET SDK e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|1° ottobre 2019|Contratto del cliente Microsoft disponibile nell'ambiente di produzione|Microsoft introduce il contratto del cliente Microsoft nel programma CSP in sostituzione del Contratto Microsoft Cloud. I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API e il dashboard Centro per i partner nell'ambiente di produzione. Il Contratto Microsoft Cloud continua a essere supportato nel programma per i partner CSP. Si consiglia tuttavia ai partner di iniziare la migrazione al contratto del cliente Microsoft. Per i nuovi acquisti e per le modifiche del numero di postazioni degli abbonamenti esistenti sarà necessaria la conferma del contratto del cliente Microsoft o del Contratto Microsoft Cloud da parte del partner. Alcune nuove offerte, ad esempio il nuovo piano Azure, richiederanno la conferma del contratto del cliente Microsoft.|
|31 gennaio 2020|Contratto Microsoft Cloud rimosso dalla produzione|Il Contratto Microsoft Cloud non è più accettato nel programma per i partner CSP. Per i nuovi acquisti e per le modifiche del numero di postazioni degli abbonamenti esistenti sarà necessaria la conferma del contratto del cliente Microsoft da parte del partner. Questo requisito si applica ai nuovi clienti e ai clienti esistenti che hanno accettato in precedenza il Contratto Microsoft Cloud.|
|3 febbraio 2020|Il partner ha ora la possibilità di invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365 autenticata. | Il cliente può accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365. L'accettazione diretta del contratto da parte del cliente nell'interfaccia di amministrazione di Microsoft 365 conferma l'approvazione delle condizioni. 

Sono disponibili le due opzioni seguenti per fare in modo che i clienti accettino il contratto del cliente Microsoft.  

**Opzione 1**: attestazione del partner dell'accettazione da parte di un cliente. Il partner può confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner o tramite il dashboard Centro per i partner.

**Opzione 2**: accettazione diretta del cliente. Il partner può invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Accedere al modello del contratto del cliente Microsoft

Puoi scaricare manualmente la versione più recente del modello di contratto del cliente Microsoft [qui](https://aka.ms/customeragreement). Tieni presente che il contratto del cliente Microsoft è specifico del paese. Quando richiedi il modello del contratto del cliente Microsoft, assicurati di selezionare il paese corretto in base alla località in cui si trova il cliente. 

## <a name="option-1-confirm-customer-acceptance-using-partner-center-apisdk"></a>Opzione 1: Confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner

Puoi usare l'API/SDK del Centro per i partner per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Per informazioni dettagliate sull'API/SDK, vedi:

- [Ottenere i metadati per il contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Ottenere la conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Ottenere un collegamento per il download del modello di contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="confirm-customer-acceptance-in-partner-center"></a>Confermare l'accettazione da parte di un cliente nel Centro per i partner

I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente nel Centro per i partner per clienti nuovi ed esistenti. I rivenditori non possono fornire un'attestazione per conto dei clienti e devono collaborare con il provider indiretto per completare l'attestazione.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confermare l'accettazione per i nuovi clienti

Quando si crea il tenant di un nuovo cliente in Centro per i partner, segui questa procedura per confermare l'accettazione del contratto del cliente Microsoft da parte del cliente. Devi essere un agente amministratore o di vendita per eseguire questa procedura.

1. Seleziona **Clienti** e quindi **Nuovo cliente**.

2. In **Informazioni sull'account** immetti le informazioni relative alla società e al contatto principale.

3. In **Microsoft agreement** (Contratto Microsoft) seleziona la casella per attestare che il cliente ha accettato il contratto del cliente Microsoft. 

4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Verifica che le informazioni di contatto dell'utente principale visualizzate siano corrette. Se non sono corrette, fai clic su **Aggiorna** e completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto.

6. Scegli **Avanti** per continuare con i passaggi rimanenti per la creazione del tenant del cliente.

![Nuovo cliente](images/mca/newcustomeragreement.jpg)  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confermare l'accettazione del cliente per i clienti esistenti

Devi essere un agente amministratore o di vendita per eseguire questa procedura:

1. Seleziona **Clienti**. Individua e seleziona il cliente.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft Customer Agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.

4. Completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Scegli **Salva** e continua.

![Cliente esistente](images/mcua2-update2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperare la conferma dell'accettazione del cliente

Puoi recuperare la conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente esistente seguendo questa procedura. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) visualizza se il cliente ha fornito o meno la conferma.

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opzione 2: Accettazione da parte del cliente nell'interfaccia di amministrazione di Microsoft 365

I partner possono invitare tramite un URL clienti nuovi ed esistenti a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365. Nelle prossime sezioni verrà illustrato come effettuare le operazioni seguenti:

- Creare un cliente completamente nuovo e invitarlo a esaminare e accettare il contratto

- Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto

- Invitare un cliente esistente a esaminare e accettare il contratto

>[!NOTE]
> Per ottenere lo stato dell'accettazione diretta del Contratto del cliente Microsoft da parte di un cliente, puoi usare l'[API/SDK del Centro per i partner](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement).  

## <a name="create-a-net-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Creare un cliente completamente nuovo e invitarlo a esaminare e accettare il contratto

Segui questa procedura per creare un nuovo cliente nel Centro per i partner e quindi invitarlo a esaminare e accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365.

1. Dalla scheda **Clienti** nel Centro per i partner seleziona **Add customer** (Aggiungi cliente).

2. In **Informazioni sull'account** immetti le informazioni sul nuovo cliente in tutti i campi obbligatori, inclusi il nome della società e il contatto principale del cliente.

3. In **Customer Agreement** (Contratto del cliente) seleziona la prima opzione, ovvero **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Al cliente verrà chiesto di accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365). Completa gli altri campi obbligatori nella pagina.

4. Seleziona **Successivo: Rivedi** e quindi continua la procedura per creare il tenant del cliente. Nota: i nuovi clienti non possono effettuare un nuovo acquisto finché non accettano il contratto del cliente Microsoft.  

![Creare un nuovo cliente](images/mca/create-new-customer.jpg)

5. Quando raggiungi la schermata **Conferma** nel flusso di lavoro per il nuovo cliente, salva le credenziali del cliente. Dovrai fornire queste credenziali al cliente in un secondo momento.

6. All'esterno del Centro per i partner crea e invia un'e-mail per invitare il cliente ad accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365. Assicurati di includere questi elementi nell'e-mail:

   - Collegamento a questo [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (sono necessarie le informazioni di accesso)
   - Credenziali del cliente salvate nel passaggio 5

7. Il cliente riceverà quindi l'invito tramite e-mail dal partner e selezionerà l'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Il cliente accede all'interfaccia di amministrazione di Microsoft 365 usando le credenziali ricevute in precedenza dal partner.

9. Il cliente seleziona quindi la casella per accettare il contratto del cliente Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft 

Segui questa procedura per invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft. 

1. Dalla scheda **Clienti** nell'ambito del Centro per i partner seleziona il collegamento **Richiedi una relazione come rivenditore**. 

2. Verrà generato un modello di e-mail automatico contenente il testo e un URL con parametri che indirizzerà il cliente all'interfaccia di amministrazione di Microsoft 365.

3. Puoi personalizzare il modello di e-mail generato automaticamente e quindi selezionare **Copia negli Appunti** o **Apri nell'email**.

4. Usa questo modello di e-mail per invitare il cliente ad accettare la richiesta di **relazione come rivenditore** e il **contratto del cliente Microsoft**. Nota: nell'invito tramite e-mail assicurati che il partner includa anche l'URL fornito automaticamente e le credenziali del cliente create di recente.

![Creare una relazione](images/mca/createrelationship.png)

5. Il cliente riceve l'invito tramite e-mail e fa clic sull'URL con parametri. 

6. Il cliente usa le credenziali fornite dal partner nell'e-mail per accedere all'interfaccia di amministrazione di Microsoft 365.

7. Il cliente seleziona la casella per accettare la **relazione come rivenditore** e il **contratto cliente Microsoft**. 

8. Nello stesso URL il cliente è in grado di visualizzare un elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

![Accettare il contratto](images/mca/accept.jpg)

## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Invitare un cliente esistente a esaminare e accettare il contratto

Segui questa procedura per invitare un cliente esistente a esaminare e accettare il contratto cliente Microsoft. 

1. Crea l'e-mail del cliente con l'URL incorporato per invitare il cliente ad accettare il contratto del cliente Microsoft.

2. Il cliente riceve l'invito tramite e-mail e fa clic sull'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Il cliente immette le proprie credenziali nell'interfaccia di amministrazione di Microsoft 365.

4. Il cliente seleziona la casella per accettare il contratto del cliente Microsoft. 

5. Nello stesso URL il cliente è in grado di visualizzare l'elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

![Cliente](images/mca/customeraccept.png)

>[!NOTE]
>In alcuni scenari i clienti potrebbero non essere in grado di accettare direttamente il contratto del cliente Microsoft. Per altre informazioni su queste situazioni, vedi [Due scenari in cui è necessaria l'attestazione per conto del cliente](attest-acceptance-customer-agreement.md).
