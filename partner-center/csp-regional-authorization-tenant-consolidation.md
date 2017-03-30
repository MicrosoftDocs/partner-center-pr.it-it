---
title: Consolidamento dei tenant per l&quot;autorizzazione regionale per CSP
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: cc87659cd0412876a29a2f8fe48d005a84026509
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>Consolidamento dei tenant per l'autorizzazione regionale per CSP

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud Germania

\[Alcune informazioni sono relative a un prodotto non definitivo che potrebbe subire modifiche sostanziali prima del rilascio sul mercato. Microsoft non riconosce alcuna garanzia, espressa o implicita, in merito alle informazioni qui fornite.\]

Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

**Nota** Devi conoscere tutte le sottoscrizioni e il numero di postazioni per i tuoi clienti di cui è stato eseguito il provisioning dagli account per la transizione. Nell'ambito della migrazione, i partner dovranno eseguire nuovamente il provisioning delle stesse identiche sottoscrizioni con lo stesso numero di postazioni nel nuovo account CSP centralizzato. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato. Il consolidamento dei tenant è una scelta del partner. Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente. Tieni presente che potrebbe essere richiesto anche l'intervento dei clienti.

 

## <a name="prepare-for-migration"></a>Prepararsi per la migrazione


-   Accedi a <https://partnercenter.microsoft.com> con l'account per la transizione (esistente) e prendi nota di tutti i clienti e di tutti i servizi di cui è stato eseguito il provisioning per tali clienti.

![elenco dei clienti regionali](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti


1.  Accedi a <https://partnercenter.microsoft.com> con l'account per la transizione (nuovo) e passa all'elenco Clienti dal dashboard del Centro per i partner.

2.  Seleziona Cliente.

3.  Fai cli su **Richiedi una relazione come rivenditore**. Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4.  **Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5.  Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

I clienti verranno visualizzati nell'elenco dei clienti del partner dopo l'invio del contratto, uno alla volta.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure


1.  Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.

2.  Nel dashboard del Centro per i partner fai clic su **Clienti** nel menu di spostamento a sinistra.

3.  Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.

4.  Fai clic su **Aggiungi sottoscrizione**.

5.  Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo. Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.

    ![screenshot dell'elenco clienti](images/regionalcustomer2.png)

6.  Fai clic su **Invia**.

I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.

Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.

Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.

**Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni. Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione


La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1.  Accedi a <https://partnercenter.microsoft.com> con l'account CSP di **origine della transizione** e passa all'elenco dei clienti.

2.  Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.
3.  Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.

    **Nota** La sospensione della sottoscrizione consente di evitare doppie fatturazioni.

     

    La sottoscrizione è indicata con lo stato **Sospeso** nell'elenco delle sottoscrizioni.

4.  Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5.  Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure


Nota che non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP in base all'uso di Azure come nel caso delle sottoscrizioni CSP di Office 365. Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1.  Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.
2.  I partner comunicano a Microsoft gli account dei clienti con sottoscrizioni di Azure pronti per la migrazione e forniscono i nomi dell'azienda dei clienti.
3.  Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.
4.  Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.
5.  Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.

    **Nota** La disabilitazione delle sottoscrizioni per il cliente non cambia l'aspetto del cliente nell'elenco Clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.

     

6.  Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="notes"></a>Note

-   Disabilitare la sottoscrizione dall'account CSP di **origine della transizione** non influisce sul servizio del cliente finale, a condizione che il provisioning del servizio sia stato eseguito dall'account CSP di **destinazione della transizione** prima della disabilitazione.

-   Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.

-   Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.

-   **Nota** I partner devono sospendere le sottoscrizioni nell'account del tenant partner di **origine della transizione** nel Centro per i partner lo stesso giorno in cui viene eseguita la transizione e la configurazione di queste sottoscrizioni nell'account del tenant partner di **destinazione della transizione** nel Centro per i partner per assicurarsi di evitare doppie fatturazioni. Microsoft non supporterà le richieste di accrediti causate da eventuali sovrapposizioni nella fatturazione dovute alla mancata sospensione delle sottoscrizioni nell'**origine della transizione**.

     

### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1.  Fai clic su **Clienti** nel tuo dashboard per visualizzare l'elenco dei clienti nella struttura esistente.

2.  Apri il nome del cliente desiderato.

3.  Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.

4.  Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, [vedi questa pagina](https://msdn.microsoft.com/en-us/library/partnercenter/mt267552.aspx).

## <a name="partner-center-activity-log"></a>Log attività del Centro per i partner


Con il log attività i partner possono visualizzare un record di tutte le modifiche effettuate nel loro tenant con effetti sui clienti. Queste informazioni sono utili per tenere traccia delle modifiche apportate nel tenant di un cliente.

**Visualizzare il log attività**

1.  Dal dashboard del Centro per i partner fai clic su link **Log attività**.
2.  Nella pagina **Log attività** visualizza le modifiche apportate agli account dei clienti. Per filtrare il log attività in base alla data, seleziona l'intervallo desiderato in **da** e **a** per limitare i record selezionati nel log. Per filtrare in base al cliente, usa la casella di ricerca nella pagina **Log attività**.

**Esportare il log attività**

-   Fai clic su **Esporta log** per esportare i dati del log attività in un file CSV.

    Puoi anche esportare l'elenco dei clienti e l'elenco delle sottoscrizioni di un singolo cliente (dalla pagina delle sottoscrizioni del cliente).

 

 



