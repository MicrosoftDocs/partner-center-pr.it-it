---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account cliente e delle sottoscrizioni dei clienti.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: migrare i clienti, il provisioning, l'account tenant, il consolidamento dei tenant
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: c2667bf19f73dfb2498cd6f706bd97b595f67a31
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679068"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Istruzioni per il consolidamento dei tenant di autorizzazione regionale CSP

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

\[Alcune informazioni si riferiscono al prodotto pre-rilasciato che può essere modificato in modo sostanziale prima del rilascio commerciale. Microsoft non offre alcuna garanzia, espressa o implicita, relativamente alle informazioni fornite in questo articolo.\]

Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

>[!NOTE]  
>È necessario essere a conoscenza di tutte le sottoscrizioni e dei conteggi delle postazioni per i clienti sottoposti a provisioning dagli account di transizione. Verrà eseguito nuovamente il provisioning di tali sottoscrizioni esatte con lo stesso numero di postazioni del nuovo account CSP centrale come parte del processo di migrazione. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato. Il consolidamento dei tenant è una scelta del partner. Una volta completato il consolidamento, non sarà possibile ripristinare lo stato precedente. Potrebbe essere necessaria anche l'azione del cliente.

## <a name="prepare-for-migration"></a>Preparare la migrazione

- Accedere al centro per i **partner** con l'account di **transizione** (esistente) (quello che si eseguirà la transizione) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.

   :::image type="content" source="images/regionalcustomer1.png" alt-text="elenco dei clienti regionali":::

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti

1. Accedere al centro per i **partner** con l'account di **transizione** (nuovo) (quello in cui si sta effettuando la transizione) e passare all'elenco Customers (clienti) dai **clienti**.

2. Selezionare Clienti.

3. Fai cli su **Richiedi una relazione come rivenditore**. Viene visualizzato un messaggio e-mail predefinito per presentarti ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4. **Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5. Dopo l'accesso, all'amministratore globale per l'account del cliente viene richiesto di inviare un contratto per attribuire privilegi di amministratore delegato al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

I clienti verranno visualizzati nell'elenco dei clienti del partner dopo che hanno inviato il contratto, uno alla volta.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure

1. Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.

2. Dal **centro** per i partner selezionare **Customers**.

3. Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.

4. Selezionare **Aggiungi sottoscrizione**.

5. Aggiungi le sottoscrizioni e il numero di postazioni corretti dal catalogo. Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco dei clienti":::

6. Fare clic su **Invia.**

   I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.

7. Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.

Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.

> [!NOTE]
> I partner devono sospendere le sottoscrizioni in **fase di transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all' **account del tenant partner nel** centro per assicurarsi che non si verifichi la doppia fatturazione. Le richieste di assistenza verranno negate per gli accrediti causati da eventuali sovrapposizioni nella fatturazione dovute alla mancata disabilitazione delle sottoscrizioni nell'**origine della transizione**.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione

La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non devi disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1. Accedere al centro per i **partner** con l'account di **transizione da** CSP e passare all'elenco dei clienti.

2. Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.

3. Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.

   >[!Note]
   >La sospensione della sottoscrizione garantisce che non si verifichi la doppia fatturazione.

   La sottoscrizione è indicata con lo stato **Sospeso** nell'elenco delle sottoscrizioni.

4. Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5. Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure

Azure, le sottoscrizioni CSP basate sull'utilizzo non devono essere migrate manualmente come nel caso delle sottoscrizioni di Office 365 CSP. Il supporto tecnico di Microsoft Azure può eseguire la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuiti dagli account rivenditore CSP di **origine della transizione** all'account rivenditore CSP di **destinazione della transizione**. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1. Assicurati che gli account dei clienti per i quali deve essere eseguita la migrazione delle sottoscrizioni di Azure abbiano accettato il contratto da associare al nuovo account CSP di **destinazione della transizione**.

2. I partner notificano a Microsoft quali account cliente che dispongono di sottoscrizioni di Azure sono pronti per la migrazione e forniscono i nomi delle società dei clienti.

3. Microsoft esegue la migrazione delle sottoscrizioni in base all'uso di Azure e informa il partner una volta completata la migrazione.

4. Il partner verifica che la sottoscrizione di Azure per gli account rivenditore CSP di **origine della transazione** risulti ora sospesa nel Centro per i partner nella sezione delle sottoscrizioni del cliente.

5. Il partner verifica che la sottoscrizione di Azure per l'account rivenditore CSP di **destinazione della transazione** abbia ora lo stato **Attiva** nel Centro per i partner nella sezione delle sottoscrizioni del cliente.

   >[!Note]
   > La disabilitazione delle sottoscrizioni del cliente non comporta la modifica dell'aspetto del cliente nell'elenco dei clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.

6. Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="additional-information"></a>Informazioni aggiuntive

- La disabilitazione della sottoscrizione dalla **transizione dall'** account CSP non influisca sul servizio del cliente finale purché sia stato effettuato il provisioning del servizio dall'account **di transizione a** CSP prima di disabilitare la sottoscrizione.

- Le sottoscrizioni non possono essere utilizzate dal cliente e non generano addebiti quando vengono sospese o annullate.

- Non esiste attualmente alcun modo per rimuovere completamente un cliente dall'elenco Clienti.

    >[!Note]
    > I partner devono sospendere le sottoscrizioni per la **transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all'account del tenant partner nel centro per i partner per garantire che non si **verifichi la doppia** fatturazione. Microsoft non supporterà le richieste di crediti dovute a eventuali sovrapposizioni nella fatturazione che si verificano se non si imposta correttamente la **transizione dalle** sottoscrizioni a sospesa.

### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1. Fare clic su **clienti** nel centro per i partner per visualizzare l'elenco dei clienti nella struttura esistente.

2. Apri il nome del cliente desiderato.

3. Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.

4. Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, vedere [configurare l'accesso all'API nel centro per i partner](https://go.microsoft.com/fwlink/?linkid=847990).
