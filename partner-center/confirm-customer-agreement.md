---
title: Confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Scopri come confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Nel programma CSP questa operazione è necessaria per ordinare prodotti e servizi Microsoft per i clienti.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 66be96fe8621089bda8dae546b804320d05fcb25
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527824"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente nel programma per i partner CSP

**Si applica a**

- Centro per i partner
- Interfaccia di amministrazione di Microsoft 365

**Ruoli appropriati**

- Agente amministratore
- Agente di vendita

**Tipi di partner appropriati**

- Rivenditori indiretti, partner con fatturazione diretta, provider indiretti

Il 1° ottobre 2019 Microsoft ha introdotto il **contratto del cliente Microsoft** nel programma CSP in sostituzione del Contratto Microsoft Cloud. Sono disponibili altre [indicazioni](indirect-reseller-tasks-in-partner-center.md) per i rivenditori indiretti. Per facilitare la migrazione dei partner al nuovo contratto, il programma CSP ha previsto la coesistenza di entrambi i contratti fino al 31 gennaio 2020. A partire dal 1° febbraio 2020, il Contratto del cliente Microsoft ha sostituito il Contratto Microsoft Cloud.

I clienti hanno due opzioni per accettare il Contratto del cliente Microsoft. 

**Opzione 1**: attestazione del partner dell'accettazione da parte di un cliente. Il partner può confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner o tramite il dashboard Centro per i partner.

**Opzione 2**: accettazione diretta del cliente. Il partner può invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Accedere al modello del contratto del cliente Microsoft

Puoi scaricare manualmente la versione più recente del modello di contratto del cliente Microsoft [qui](https://aka.ms/customeragreement). Il Contratto del cliente Microsoft è specifico del paese. Quando richiedi il modello del contratto del cliente Microsoft, assicurati di selezionare il paese corretto in base alla località in cui si trova il cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opzione 1: Confermare l'accettazione da parte di un cliente nel Centro per i partner

I partner possono confermare l'accettazione del Contratto del cliente Microsoft da parte di clienti nuovi ed esistenti nel Centro per i partner. I rivenditori non possono fornire un'attestazione per conto dei clienti e devono collaborare con il provider indiretto per completare l'attestazione.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confermare l'accettazione per i nuovi clienti

Quando si crea il tenant di un nuovo cliente in Centro per i partner, segui questa procedura per confermare l'accettazione del contratto del cliente Microsoft da parte del cliente. Devi essere un agente amministratore o di vendita per eseguire questa procedura.

1. Seleziona **Clienti** e quindi **Nuovo cliente**.

2. In **Informazioni sull'account** immetti le informazioni relative alla società e al contatto principale.

3. In **Microsoft agreement** (Contratto Microsoft) seleziona la casella per attestare che il cliente ha accettato il contratto del cliente Microsoft.

4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Verifica che le informazioni di contatto dell'utente principale visualizzate siano corrette. Se non è corretto, selezionare **Aggiorna** e immettere le informazioni accurate per la persona che ha accettato il contratto.

6. Selezionare **Avanti** per continuare a creare il tenant del cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nuovo cliente":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confermare l'accettazione del cliente per i clienti esistenti

Devi essere un agente amministratore o di vendita per eseguire questa procedura:

1. Seleziona **Clienti**. Individua e seleziona il cliente.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft Customer Agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.

4. Completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Scegli **Salva** e continua.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente esistente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperare la conferma dell'accettazione del cliente

Puoi recuperare la conferma dell'accettazione del contratto del cliente Microsoft da parte di un cliente esistente seguendo questa procedura. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) visualizza se il cliente ha fornito o meno la conferma.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner

Puoi usare l'API/SDK del Centro per i partner per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Per informazioni dettagliate su API/SDK, vedere:

- [Ottenere i metadati per il contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confermare l'accettazione del contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Ottenere la conferma dell'accettazione del Contratto del cliente Microsoft da parte di un cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Ottenere un collegamento per il download del modello di contratto del cliente Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opzione 2: Accettazione da parte del cliente nell'interfaccia di amministrazione di Microsoft 365

I partner possono invitare tramite un URL clienti nuovi ed esistenti a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365. Nelle prossime sezioni verrà illustrato come effettuare le operazioni seguenti:

- Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto.

- Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto.

- Invitare un cliente esistente a esaminare e accettare il contratto.

>[!NOTE]
> Per ottenere lo stato dell'accettazione diretta del Contratto del cliente Microsoft da parte di un cliente, puoi usare l'[API/SDK del Centro per i partner](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement).  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto

Segui questa procedura per creare un nuovo cliente nel Centro per i partner e quindi invitarlo a esaminare e accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365.

1. Dalla scheda **Clienti** nel Centro per i partner seleziona **Add customer** (Aggiungi cliente).

2. In **Informazioni sull'account** immetti le informazioni sul nuovo cliente in tutti i campi obbligatori, inclusi il nome della società e il contatto principale del cliente.

3. In **Customer Agreement** (Contratto del cliente) seleziona la prima opzione, ovvero **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Al cliente verrà chiesto di accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365). Completa gli altri campi obbligatori nella pagina.

4. Seleziona **Successivo: Rivedi** e quindi continua la procedura per creare il tenant del cliente. 

>[!NOTE] 
>I nuovi clienti non possono eseguire alcun nuovo acquisto finché non accettano il Contratto del cliente Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Creare un nuovo cliente":::

5. Quando raggiungi la schermata **Conferma** nel flusso di lavoro per il nuovo cliente, salva le credenziali del cliente. Dovrai fornire queste credenziali al cliente in un secondo momento.

6. All'esterno del Centro per i partner crea e invia un'e-mail per invitare il cliente ad accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365. Assicurati di includere questi elementi nell'e-mail:

   - Collegamento a questo [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (sono necessarie le informazioni di accesso)

   - Credenziali del cliente salvate nel passaggio 5.

7. Il cliente riceverà quindi l'invito tramite e-mail dal partner e selezionerà l'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Il cliente accede all'interfaccia di amministrazione di Microsoft 365 usando le credenziali ricevute in precedenza dal partner.

9. Il cliente seleziona quindi la casella per accettare il contratto del cliente Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft 

Segui questa procedura per invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft. 

1. Dalla scheda **Clienti** nell'ambito del Centro per i partner seleziona il collegamento **Richiedi una relazione come rivenditore**. 

2. Verrà generato un modello di e-mail automatico contenente il testo e un URL con parametri che indirizzerà il cliente all'interfaccia di amministrazione di Microsoft 365.

3. Puoi personalizzare il modello di e-mail generato automaticamente e quindi selezionare **Copia negli Appunti** o **Apri nell'email**.

4. Usa questo modello di e-mail per invitare il cliente ad accettare la richiesta di **relazione come rivenditore** e il **contratto del cliente Microsoft**. Nota: nell'invito tramite e-mail assicurati che il partner includa anche l'URL fornito automaticamente e le credenziali del cliente create di recente.

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Creare una relazione":::

5. Il cliente riceve l'invito tramite e-mail e fa clic sull'URL con parametri. 

6. Il cliente usa le credenziali fornite dal partner nell'e-mail per accedere all'interfaccia di amministrazione di Microsoft 365.

7. Il cliente seleziona la casella per accettare la **relazione come rivenditore** e il **contratto cliente Microsoft**. 

8. Nello stesso URL il cliente è in grado di visualizzare un elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Accettare il contratto":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Invitare un cliente esistente a esaminare e accettare il contratto

Segui questa procedura per invitare un cliente esistente a esaminare e accettare il contratto cliente Microsoft. 

1. Crea l'e-mail del cliente con l'URL incorporato per invitare il cliente ad accettare il contratto del cliente Microsoft.

2. Il cliente riceve l'invito tramite posta elettronica e fa clic sull'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Il cliente immette le proprie credenziali nell'interfaccia di amministrazione di Microsoft 365.

4. Il cliente seleziona la casella per accettare il contratto del cliente Microsoft. 

5. Nello stesso URL il cliente è in grado di visualizzare l'elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente":::

>[!NOTE]
>In alcuni scenari i clienti potrebbero non essere in grado di accettare direttamente il contratto del cliente Microsoft. Per altre informazioni su queste situazioni, vedi [Due scenari in cui è necessaria l'attestazione per conto del cliente](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Dettagli della sequenza temporale cronologica

| Data | Attività cardine | Dettagli |
|------------|------------|--------------------------------|
|1° agosto 2019|Esperienza utente in anteprima disponibile in sandbox|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando il dashboard Centro per i partner nell'ambiente sandbox CSP. I partner con accesso all'ambiente sandbox CSP visualizzano in anteprima le modifiche dell'esperienza utente. I partner senza accesso sandbox possono ottenere informazioni sulle modifiche in questo argomento.|
|3 settembre 2019|API in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate all'API e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|20 settembre 2019|.NET SDK in anteprima disponibile in sandbox.|I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando .NET SDK Centro per i partner nell'ambiente sandbox CSP. I partner API possono usare questa opportunità per visualizzare in anteprima le modifiche apportate a .NET SDK e iniziare a lavorare all'integrazione dell'API per supportare il nuovo contratto.|
|1° ottobre 2019|Contratto del cliente Microsoft disponibile nell'ambiente di produzione|Microsoft introduce il contratto del cliente Microsoft nel programma CSP in sostituzione del Contratto Microsoft Cloud. I partner possono confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente usando l'API e il dashboard Centro per i partner nell'ambiente di produzione. Il Contratto Microsoft Cloud continua a essere supportato nel programma per i partner CSP. Si consiglia tuttavia ai partner di iniziare la migrazione al contratto del cliente Microsoft. Per i nuovi acquisti e per le modifiche del numero di licenze delle sottoscrizioni esistenti sarà necessaria la conferma del Contratto del cliente Microsoft o del Contratto Microsoft Cloud da parte del partner. Alcune nuove offerte, ad esempio il nuovo piano Azure, richiederanno la conferma del contratto del cliente Microsoft.|
|31 gennaio 2020|Contratto Microsoft Cloud rimosso dalla produzione|Il Contratto Microsoft Cloud non è più accettato nel programma per i partner CSP. Per i nuovi acquisti e per le modifiche del numero di licenze delle sottoscrizioni esistenti sarà necessaria la conferma del Contratto del cliente Microsoft da parte del partner. Questo requisito si applica ai nuovi clienti e ai clienti esistenti che hanno accettato in precedenza il Contratto Microsoft Cloud.|
|3 febbraio 2020|Il partner ha ora la possibilità di invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365 autenticata. | Il cliente può accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365. L'accettazione diretta del contratto da parte del cliente nell'interfaccia di amministrazione di Microsoft 365 conferma l'approvazione delle condizioni. 
