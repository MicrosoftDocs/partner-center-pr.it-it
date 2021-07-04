---
title: Come verificare che il cliente abbia accettato l'Contratto del cliente Microsoft al programma CSP
description: I partner Cloud Solution Provider (CSP) devono confermare l'accettazione del Contratto del cliente Microsoft prima di ordinare i servizi Microsoft per i clienti.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277012"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Come verificare che il cliente abbia accettato l'Contratto del cliente Microsoft al programma CSP

**Ruoli appropriati:** agente di amministrazione | Agente di vendita


I clienti hanno due opzioni per il modo in cui accettano il Contratto del cliente Microsoft.

**Opzione 1**: attestazione del partner dell'accettazione da parte di un cliente. Il partner può confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner o tramite il dashboard Centro per i partner.

**Opzione 2**: accettazione diretta del cliente. Il partner può invitare tramite un URL il cliente a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Accedere al modello del contratto del cliente Microsoft

Puoi scaricare manualmente la versione più recente del modello di contratto del cliente Microsoft [qui](https://aka.ms/customeragreement). Il Contratto del cliente Microsoft è specifico del paese. Quando richiedi il modello del contratto del cliente Microsoft, assicurati di selezionare il paese corretto in base alla località in cui si trova il cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opzione 1: Confermare l'accettazione da parte di un cliente nel Centro per i partner

I partner con fatturazione diretta possono confermare l'accettazione del Contratto del cliente Microsoft in Partner Center per i clienti nuovi ed esistenti. I rivenditori indiretti non possono eseguire l'attestazione per conto dei clienti e devono collaborare con il provider indiretto per completare l'attestazione.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confermare l'accettazione per i nuovi clienti

Quando si crea il tenant di un nuovo cliente in Centro per i partner, segui questa procedura per confermare l'accettazione del contratto del cliente Microsoft da parte del cliente. Devi essere un agente amministratore o di vendita per eseguire questa procedura.

1. Seleziona **Clienti** e quindi **Nuovo cliente**.

2. In **Informazioni sull'account** immetti le informazioni relative alla società e al contatto principale.

3. In **Microsoft agreement** (Contratto Microsoft) seleziona la casella per attestare che il cliente ha accettato il contratto del cliente Microsoft.

4. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Verifica che le informazioni di contatto dell'utente principale visualizzate siano corrette. Se non è corretto, selezionare **Aggiorna** e immettere le informazioni accurate per la persona che ha accettato il contratto.

6. Selezionare **Avanti** per continuare a creare il tenant del cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nuovo cliente.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confermare l'accettazione del cliente per i clienti esistenti

Devi essere un agente amministratore o di vendita per eseguire questa procedura:

1. Seleziona **Clienti**. Individua e seleziona il cliente.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft Customer Agreement** (Contratto del cliente Microsoft) fai clic su **Aggiorna**.

4. Completa i campi **Nome**, **Cognome**, **Indirizzo di posta elettronica** e **Numero di telefono** (facoltativo) della persona che ha accettato il contratto. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

5. Scegli **Salva** e continua.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente esistente.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperare la conferma dell'accettazione del cliente

Per recuperare la conferma che un cliente esistente ha accettato il Contratto del cliente Microsoft, seguire questa procedura. Devi essere un agente amministratore o di vendita per eseguire questa operazione.

1. Seleziona **Clienti** e quindi individua e seleziona il cliente che vuoi visualizzare.

2. Seleziona **Informazioni sull'account**.

3. In **Microsoft customer agreement** (Contratto del cliente Microsoft) visualizza se il cliente ha fornito o meno la conferma.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confermare l'accettazione da parte di un cliente tramite l'API/SDK del Centro per i partner

Puoi usare l'API/SDK del Centro per i partner per confermare l'accettazione del contratto del cliente Microsoft da parte di un cliente. Per informazioni dettagliate su API/SDK, vedere:

- [Ottenere i metadati per il contratto del cliente Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confermare l'accettazione del contratto del cliente Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Ottenere la conferma dell'accettazione del Contratto del cliente Microsoft da parte di un cliente](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Ottenere un collegamento per il download del modello di contratto del cliente Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opzione 2: Accettazione da parte del cliente nell'interfaccia di amministrazione di Microsoft 365

I partner possono invitare tramite un URL clienti nuovi ed esistenti a esaminare e accettare il contratto nell'interfaccia di amministrazione di Microsoft 365. Nelle prossime sezioni verrà illustrato come effettuare le operazioni seguenti:

- Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto.

- Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto.

- Invitare un cliente esistente a esaminare e accettare il contratto.

>[!NOTE]
> Per ottenere lo stato dell'accettazione diretta del Contratto del cliente Microsoft da parte di un cliente, puoi usare l'[API/SDK del Centro per i partner](/partner-center/develop/get-direct-sign-status-of-customer-agreement).  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Creare un nuovo cliente nuovo e invitarlo a esaminare e accettare il contratto

Segui questa procedura per creare un nuovo cliente nel Centro per i partner e quindi invitarlo a esaminare e accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365.

1. Dalla scheda **Clienti** nel Centro per i partner seleziona **Add customer** (Aggiungi cliente).

2. In **Informazioni sull'account** immetti le informazioni sul nuovo cliente in tutti i campi obbligatori, inclusi il nome della società e il contatto principale del cliente.

3. In **Contratto del** cliente selezionare Customer will be asked to accept the Contratto del cliente Microsoft in Amministrazione Microsoft 365 **Center**. Completa gli altri campi obbligatori nella pagina.

4. Seleziona **Successivo: Rivedi** e quindi continua la procedura per creare il tenant del cliente. 

>[!NOTE] 
>I nuovi clienti non possono effettuare un acquisto fino a quando non accettano il Contratto del cliente Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Creare un nuovo cliente.":::

5. Quando raggiungi la schermata **Conferma** nel flusso di lavoro per il nuovo cliente, salva le credenziali del cliente. Dovrai fornire queste credenziali al cliente in un secondo momento.

6. All'esterno del Centro per i partner crea e invia un'e-mail per invitare il cliente ad accettare il contratto del cliente Microsoft nell'interfaccia di amministrazione di Microsoft 365. Assicurati di includere questi elementi nell'e-mail:

   - Collegamento a questo [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (sono necessarie le informazioni di accesso)

   - Le credenziali del cliente salvate nel passaggio 5.

7. Il cliente riceverà quindi l'invito tramite e-mail dal partner e selezionerà l'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Il cliente accede Amministrazione Microsoft 365 Center usando le credenziali del cliente specificate.

9. Il cliente controlla la casella per accettare il Contratto del cliente Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft 

Segui questa procedura per invitare un nuovo cliente a esaminare e accettare la relazione come rivenditore e il contratto cliente Microsoft. 

1. Dalla scheda **Clienti** nell'ambito del Centro per i partner seleziona il collegamento **Richiedi una relazione come rivenditore**. 

2. Verrà generato un modello di e-mail automatico contenente il testo e un URL con parametri in grado di indirizzare il cliente all'interfaccia di amministrazione di Microsoft 365.

3. Puoi personalizzare il modello di e-mail generato automaticamente e quindi selezionare **Copia negli Appunti** o **Apri nell'email**.

4. Usa questo modello di e-mail per invitare il cliente ad accettare la richiesta di **relazione come rivenditore** e il **contratto del cliente Microsoft**. Nota: nell'invito tramite e-mail assicurati che il partner includa anche l'URL fornito automaticamente e le credenziali del cliente create di recente.

   :::image type="content" source="images/mca/createrelationship.png" alt-text="creare una relazione.":::

5. Il cliente riceve l'invito tramite e-mail e fa clic sull'URL con parametri. 

6. Il cliente usa le credenziali specificate all'interno della posta elettronica per accedere Amministrazione Microsoft 365 Center.

7. Il cliente seleziona la casella per accettare la **relazione come rivenditore** e il **contratto cliente Microsoft**. 

8. Nello stesso URL il cliente è in grado di visualizzare un elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Accettare il contratto.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Invitare un cliente esistente a esaminare e accettare il contratto

Segui questa procedura per invitare un cliente esistente a esaminare e accettare il contratto cliente Microsoft. 

1. Crea l'e-mail del cliente con l'URL incorporato per invitare il cliente ad accettare il contratto del cliente Microsoft.

2. Il cliente riceve l'invito tramite posta elettronica e fa clic sull'[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Il cliente immette le proprie credenziali nell'interfaccia di amministrazione di Microsoft 365.

4. Il cliente seleziona la casella per accettare il contratto del cliente Microsoft. 

5. Nello stesso URL il cliente è in grado di visualizzare l'elenco consolidato di partner diversi con cui lavora e può selezionare un partner per visualizzare i dettagli.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente.":::

>[!NOTE]
>In alcuni scenari i clienti potrebbero non essere in grado di accettare direttamente il contratto del cliente Microsoft. Per altre informazioni su queste situazioni, vedere Due scenari in cui è necessario attestare per conto del cliente, di seguito.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Due scenari in cui è necessaria l'attestazione per conto del cliente

Esistono due scenari in cui i clienti potrebbero non essere in grado di accettare direttamente il Contratto del cliente Microsoft all'interno Amministrazione Microsoft 365 Center.

**Scenario 1:** un cliente esistente ha acquistato uno degli elementi seguenti tramite una relazione partner esistente: offerte, sottoscrizioni software o software, istanze riservate o piano di Azure. Il cliente tenta ora di effettuare un nuovo acquisto (escluso il rinnovo automatico). Quando il cliente seleziona l'URL, riceve un messaggio che indica di rivolgersi al partner per confermare l'accettazione del Contratto del cliente Microsoft.  

**Per risolvere il problema**: devi attestare l'accettazione per conto del cliente.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Screenshot della pagina dell'interfaccia di amministrazione di Microsoft 365 che chiede di contattare il proprio partner per confermare l'accettazione del Contratto del cliente Microsoft.":::

**Scenario 2**: un cliente esistente ha acquistato una delle opzioni seguenti: offerta, software o abbonamento software, istanza riservata o piano di Azure. Il cliente tenta ora di effettuare un nuovo acquisto con un nuovo partner.

Quando il cliente seleziona l'URL dell'interfaccia di amministrazione di Microsoft 365 per accettare la relazione con il nuovo partner e il contratto, riceve un messaggio che indica di rivolgersi al partner per confermare l'accettazione del Contratto del cliente Microsoft.  

**Per risolvere il problema**: devi attestare l'accettazione per conto del cliente.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Verificare che un cliente abbia accettato il contratto

Se si tenta di creare un nuovo ordine per un cliente esistente non confermato prima, si riceverà la richiesta di completare la conferma. Utilizzare la procedura seguente per eseguire questa operazione.

1. Riempi i campi **Nome**, **Cognome**, **Indirizzo e-mail** e **Numero di telefono** (facoltativo) dell'utente che ha accettato il contratto.

2. In **Agreement acceptance date** (Data di accettazione del contratto) immetti la data appropriata. Non puoi impostare questo campo su una data futura.

3. Fai clic su **Salva e continua**. 

## <a name="next-steps"></a>Passaggi successivi

- [Verificare o aggiornare le informazioni del profilo aziendale](update-your-partner-profile.md)
- [Contratti del cliente Microsoft (per area geografica e lingua)](Agreements.md)
