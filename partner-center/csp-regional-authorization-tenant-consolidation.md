---
title: Consolidamento dei tenant per l'autorizzazione regionale per CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi. Sono inclusi i passaggi per eseguire la migrazione degli account dei clienti e delle sottoscrizioni dei clienti.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276876"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Istruzioni per il consolidamento dei tenant per l'autorizzazione regionale per CSP

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** amministratore globale | Agente amministratore

\[Alcune informazioni riguardano un prodotto pre-rilasciato che può essere modificato sostanzialmente prima del rilascio in commercio. Microsoft non riconosce alcuna garanzia, espressa o implicita, in merito alle informazioni qui fornite.\]

È possibile consolidare i tenant per l'azienda. Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

>[!NOTE]  
>È necessario conoscere tutti i conteggi delle sottoscrizioni e delle licenze di cui è stato effettuato il provisioning per ogni cliente nell'account da cui si esegue la transizione. Nell'ambito del processo di migrazione, verrà nuovamente provisioning delle stesse sottoscrizioni esatte con gli stessi conteggi delle licenze nel nuovo account CSP centrale. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.  Al termine del consolidamento, non è possibile ripristinare lo stato precedente del tenant. Potrebbe essere necessaria anche l'azione del cliente.

## <a name="prepare-for-migration"></a>Preparare la migrazione

- Accedere a **Partner Center** l'account  di transizione (quello di cui si eseguirà la transizione al nuovo account) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.

- Disconnettersi da questo account.

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti

1. Accedere al **Partner Center**  con l'account **Transitioning** (nuovo) (quello in cui si sta effettuando la transizione dei clienti).

2. Seleziona **Clienti**.

3. Selezionare **Richiedi una relazione come rivenditore.** Viene visualizzato un messaggio di posta elettronica predefinito da inviare ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4. **Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5. Dopo l'accesso, all'amministratore globale per **l'account** cliente viene richiesto di inviare un contratto che concede privilegi di amministratore delegato al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

I clienti verranno visualizzati nell'elenco dei clienti del partner dopo aver inviato il contratto, uno alla volta.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure

1. Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.

2. In **Partner Center** selezionare **Clienti.**

3. Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.

4. Selezionare **Aggiungi sottoscrizione**.

5. Aggiungere le sottoscrizioni e i conteggi delle licenze corretti dal catalogo. Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco di clienti.":::

6. Selezionare **Invia.**

   I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.

7. Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.

Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.

> [!NOTE]
> I partner devono  sospendere le sottoscrizioni nell'account del tenant partner di transizione Partner Center stesso giorno  in cui tali sottoscrizioni vengono transizione e impostate nell'account del tenant partner di transizione nel Partner Center per garantire che non si verifichi una doppia fatturazione. Le richieste di supporto verranno negate per i crediti a causa di eventuali sovrapposizioni nella fatturazione dovute alla disabilitazione non corretta delle sottoscrizioni di **transizione dalle** sottoscrizioni.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione

La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non è necessario disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1. Accedere al portale di **Partner Center** con l'account **Transitioning From** CSP (Transizione da CSP) e passare all'elenco dei clienti.

2. Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.

3. Impostare la sottoscrizione su **sospeso** e quindi selezionare **Invia.**

   >[!Note]
   >La sospensione della sottoscrizione garantisce che non si verifichi una doppia fatturazione.

   La sottoscrizione viene visualizzata **come sospesa** nell'elenco delle sottoscrizioni.

4. Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5. Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure

A differenza delle sottoscrizioni CSP di Office 365, non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP basate sull'utilizzo di Azure. Microsoft Azure supporto tecnico eseguirà la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuite dagli account rivenditore **CSP** all'account del rivenditore **di** transizione a CSP. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1. Assicurarsi che gli account dei clienti di cui verrà eseguita la migrazione delle sottoscrizioni di Azure abbia accettato il contratto da associare al nuovo account di transizione **a** CSP.

2. Si invierà una notifica a Microsoft degli account dei clienti pronti per la migrazione e si forniranno i nomi delle società del cliente.

3. Microsoft esegue la migrazione delle sottoscrizioni basate sull'utilizzo di Azure e invia una notifica al termine della migrazione.

4. È necessario verificare che la sottoscrizione di Azure nell'account  del rivenditore **Transitioning From** CSP (Transizione da rivenditore CSP) sia ora contrassegnata come sospesa Partner Center nella sezione sottoscrizioni dei clienti.

5. Verificare che la sottoscrizione di Azure nell'account del rivenditore **Di** transizione a CSP ora mostra lo stato attivo **Partner Center** nella sezione sottoscrizioni dei clienti.

   >[!Note]
   > La disabilitazione delle sottoscrizioni del cliente non modifica l'aspetto del cliente nell'elenco Clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.

6. Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="additional-information"></a>Informazioni aggiuntive

- La disabilitazione della sottoscrizione dall'account **CSP** di transizione non influisce sul servizio del cliente finale, purché sia stato effettuato il provisioning del servizio dall'account di transizione a **CSP** prima di disabilitare la sottoscrizione.

- Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti in caso di sospensione o annullamento.

- Attualmente non è possibile rimuovere completamente un cliente **dall'elenco Clienti.**
- 
    >[!Note]
    > I partner devono sospendere le sottoscrizioni nell'account **del** tenant partner di transizione da Partner Center stesso giorno in cui tali sottoscrizioni vengono impostate e impostate nell'account  di transizione a per garantire che non si verifichi una doppia fatturazione. Microsoft non supporterà le richieste di crediti a causa di  eventuali sovrapposizioni nella fatturazione dovute all'impostazione non corretta delle sottoscrizioni di transizione da a sospeso.

### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1. Selezionare **Clienti** nella Partner Center per visualizzare l'elenco dei clienti. 

2. Apri il nome del cliente desiderato.

3. Nella pagina **Sottoscrizioni** selezionare Esporta **sottoscrizioni** per esportare i dettagli delle sottoscrizioni in un file di Excel.

4. Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, vedere [Configurare l'accesso all'API in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Passaggi successivi

- [Cloud Solution Provider mercati e valute regionali del programma in cui è possibile vendere offerte CSP](regional-authorization-overview.md)
