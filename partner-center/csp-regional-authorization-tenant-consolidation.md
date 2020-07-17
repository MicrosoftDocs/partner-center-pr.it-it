---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: article
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account cliente e delle sottoscrizioni dei clienti.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 46ba699bee0a7e4554042522528fdc6d2a18596a
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434920"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Istruzioni per il consolidamento dei tenant per l'autorizzazione regionale per CSP

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

\[Alcune informazioni si riferiscono al prodotto pre-rilasciato che può essere modificato in modo sostanziale prima del rilascio commerciale. Microsoft non offre alcuna garanzia, espressa o implicita, relativamente alle informazioni fornite in questo articolo.\]

È possibile consolidare i tenant per l'azienda. Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

>[!NOTE]  
>È necessario essere a conoscenza di tutte le sottoscrizioni di cui è stato effettuato il provisioning e del numero di postazioni per ogni cliente nell'account da cui si esegue la transizione. Verrà eseguito nuovamente il provisioning di tali sottoscrizioni esatte con lo stesso numero di postazioni del nuovo account CSP centrale come parte del processo di migrazione. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.  Al termine del consolidamento, non è possibile ripristinare lo stato precedente del tenant. Potrebbe essere necessaria anche l'azione del cliente.

## <a name="prepare-for-migration"></a>Preparare la migrazione

- Accedere al centro per i **partner** usando l'account di **transizione** (quello che si passerà al nuovo account) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.

- Disconnettersi da questo account.

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti

1. Accedere al centro per i **partner** con l'account di **transizione** (nuovo) (quello in cui si sta effettuando la transizione dei clienti).

2. Selezionare **Clienti**.

3. Fai cli su **Richiedi una relazione come rivenditore**. Viene visualizzato un messaggio di posta elettronica predefinito da inviare ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4. **Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5. Dopo l'accesso, all'amministratore globale per l' **account del cliente** viene richiesto di inviare un contratto che fornisce privilegi amministrativi delegati al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

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
> I partner devono sospendere le sottoscrizioni in **fase di transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui tali sottoscrizioni vengono sottoposte a transizione e configurate in base all' **account del tenant partner nel** centro per assicurarsi che non si verifichi la doppia fatturazione. Le richieste di supporto verranno negate per i crediti a causa di sovrapposizioni nella fatturazione che si verificano quando non si disabilita correttamente la **transizione dalle** sottoscrizioni.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione

La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non è necessario disabilitare manualmente le sottoscrizioni di Azure perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1. Accedere al centro per i **partner** con l'account di **transizione da** CSP e passare all'elenco dei clienti.

2. Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.

3. Imposta la sottoscrizione come **sospesa** e quindi fai clic su **Invia**.

   >[!Note]
   >La sospensione della sottoscrizione garantisce che non si verifichi la doppia fatturazione.

   La sottoscrizione Mostra **sospesa** nell'elenco delle sottoscrizioni.

4. Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5. Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure

A differenza delle sottoscrizioni di Office 365 CSP, non è necessario eseguire la migrazione manuale delle sottoscrizioni CSP basate sull'utilizzo di Azure. Il supporto Microsoft Azure eseguirà la migrazione delle sottoscrizioni di Azure, nonché di tutti i servizi o le risorse distribuiti dalla **transizione dagli account del** rivenditore CSP all' **account del rivenditore** CSP. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1. Assicurarsi che gli account cliente che disporranno di sottoscrizioni di Azure migrati abbiano accettato il contratto da associare alla nuova **transizione all'** account CSP.

2. Si invierà una notifica a Microsoft di quali account cliente sono pronti per la migrazione e si specificano i nomi delle società dei clienti.

3. Microsoft esegue la migrazione delle sottoscrizioni basate sull'utilizzo di Azure e invia una notifica al termine della migrazione.

4. È necessario verificare che la sottoscrizione di Azure nell'ambito dell'account reseller del rivenditore **di** CSP sia ora contrassegnata come **sospesa** nel centro per i partner nella sezione sottoscrizioni clienti.

5. Verificare che la sottoscrizione di Azure in **transizione all'** account rivenditore CSP Ora visualizzi lo stato **attivo** nel centro per i partner nella sezione sottoscrizioni clienti.

   >[!Note]
   > La disabilitazione delle sottoscrizioni del cliente non comporta la modifica dell'aspetto del cliente nell'elenco dei clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.

6. Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="additional-information"></a>Informazioni aggiuntive

- La disabilitazione della sottoscrizione dalla **transizione dall'** account CSP non influisca sul servizio del cliente finale purché sia stato effettuato il provisioning del servizio dall'account **di transizione a** CSP prima di disabilitare la sottoscrizione.

- Le sottoscrizioni non possono essere utilizzate dal cliente e non generano addebiti quando vengono sospese o annullate.

- Attualmente non è possibile rimuovere completamente un cliente dall'elenco dei **clienti** .
- 
    >[!Note]
    > I partner devono sospendere le sottoscrizioni per la **transizione dall'** account del tenant partner nel centro per i partner nello stesso giorno in cui vengono passate le sottoscrizioni e configurate in fase di **transizione a** account per assicurarsi che la doppia fatturazione non venga eseguita. Microsoft non supporterà le richieste di crediti dovute a eventuali sovrapposizioni nella fatturazione che si verificano se non si imposta correttamente la **transizione dalle** sottoscrizioni a sospesa.

### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1. Fare clic su **clienti** nel centro per i partner per visualizzare l'elenco dei clienti. 

2. Apri il nome del cliente desiderato.

3. Nella pagina **Sottoscrizioni** fai clic su **Esporta sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.

4. Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, vedere [configurare l'accesso all'API nel centro per i partner](https://go.microsoft.com/fwlink/?linkid=847990).

## <a name="next-steps"></a>Passaggi successivi

- [Configurazione e gestione degli account cliente per i partner rivenditori nel centro per i partner](customer-accounts.md)
