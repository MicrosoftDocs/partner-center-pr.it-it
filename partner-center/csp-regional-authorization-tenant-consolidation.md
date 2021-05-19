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
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147582"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Istruzioni per il consolidamento dei tenant per l'autorizzazione regionale per CSP

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** Amministratore globale | Agente amministratore

\[Alcune informazioni riguardano prodotti pre-rilasciati che possono essere modificati in modo sostanziale prima che venga rilasciato commercialmente. Microsoft non riconosce alcuna garanzia, espressa o implicita, in merito alle informazioni qui fornite.\]

È possibile consolidare i tenant per l'azienda. Usa queste istruzioni per consolidare i tenant per paesi/aree geografiche diversi.

>[!NOTE]  
>È necessario essere a conoscenza di tutte le sottoscrizioni con provisioning e dei conteggi delle licenze per ogni cliente nell'account da cui si esegue la transizione. Nell'ambito del processo di migrazione, verrà nuovamente provisioning delle stesse sottoscrizioni esatte con gli stessi conteggi delle licenze nel nuovo account CSP centrale. Usa la funzionalità di esportazione di elenchi per creare un elenco di clienti da trasferire al tenant centralizzato.  Al termine del consolidamento, non è possibile ripristinare lo stato precedente del tenant. Potrebbe essere necessaria anche l'azione del cliente.

## <a name="prepare-for-migration"></a>Preparare la migrazione

- Accedere a **Partner Center** usando l'account  di transizione (quello di cui si eseguirà la transizione al nuovo account) ed esaminare tutti i clienti e tutti i servizi di cui è stato effettuato il provisioning per tali clienti.

- Disconnettersi da questo account.

## <a name="migrate-customer-accounts"></a>Eseguire la migrazione degli account dei clienti

1. Accedere a **Partner Center**  con l'account **transitioning** (nuovo) (quello in cui si sta effettuando la transizione dei clienti).

2. Seleziona **Clienti**.

3. Selezionare **Richiedi una relazione rivenditore**. Viene visualizzato un messaggio di posta elettronica predefinito da inviare ai clienti. Questo messaggio contiene un URL con l'ID organizzazione univoco per il tuo nuovo account del Centro per i partner.

4. **Azione del cliente:** assicurati che ogni cliente attivo di cui vuoi eseguire la migrazione visiti questo URL. All'apertura dell'URL, al cliente viene richiesto di accedere al portale di Office 365. Il cliente effettua l'accesso con lo stesso ID organizzazione usato per accedere ai portali di amministrazione di Azure e Office 365.

5. Dopo l'accesso, all'amministratore globale per **l'account** del cliente viene richiesto di inviare un contratto che concede privilegi di amministratore delegato al nuovo account CSP. Se è d'accordo, il cliente seleziona la casella di controllo e accetta di autorizzare la relazione.

I clienti verranno visualizzati nell'elenco dei clienti del partner dopo aver inviato il contratto, uno alla volta.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Office 365 e non Azure

1. Quando il cliente ha accettato il contratto, puoi ricreare le sue sottoscrizioni nel tuo tenant partner centralizzato.

2. Da **Partner Center** selezionare **Clienti**.

3. Apri il nome dell'azienda per il cliente di cui vuoi eseguire la migrazione.

4. Selezionare **Aggiungi sottoscrizione**.

5. Aggiungere le sottoscrizioni e i conteggi delle licenze corretti dal catalogo. Controlla in base alle informazioni fornite per gli account partner di **origine della transizione**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="elenco di clienti":::

6. Selezionare **Invia.**

   I servizi vengono ora forniti al cliente dall'account partner di **destinazione della transizione**.

7. Ripeti questi passaggi per eseguire la migrazione delle sottoscrizioni per tutti i clienti.

Prima di procedere alla sezione successiva, verifica che sia stato eseguito di nuovo il provisioning di tutte le sottoscrizioni dei clienti esistenti negli account partner di **origine della transizione** nell'account partner di **destinazione della transizione**.

> [!NOTE]
> I partner devono  sospendere le sottoscrizioni nell'account del tenant partner di transizione dal Partner Center lo  stesso giorno in cui tali sottoscrizioni vengono transizione e impostate nell'account del tenant partner di transizione al tenant partner nel Partner Center per garantire che non si verifichi la doppia fatturazione. Le richieste di supporto verranno negate per i crediti a causa di eventuali sovrapposizioni nella fatturazione dovute alla non corretta disabilitazione delle sottoscrizioni di transizione **da.**

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabilitazione delle sottoscrizioni di Office 365 nell'account partner di origine della transizione

La disabilitazione della sottoscrizione CSP negli account partner di **origine della transizione** interrompe eventuali fatturazioni future. Non è necessario disabilitare manualmente le sottoscrizioni di Azure, perché le sottoscrizioni di Azure vengono disabilitate automaticamente durante il processo di migrazione.

1. Accedere al Partner Center **con** l'account **Transitioning From** CSP (Transizione da CSP) e passare all'elenco dei clienti.

2. Apri il cliente con le sottoscrizioni da disabilitare e quindi seleziona la prima offerta da disabilitare.

3. Impostare la sottoscrizione su **suspended** e quindi selezionare **Submit (Invia).**

   >[!Note]
   >La sospensione della sottoscrizione garantisce che non si verifichi una doppia fatturazione.

   La sottoscrizione viene **visualizzata sospesa** nell'elenco delle sottoscrizioni.

4. Ripeti questi passaggi per tutte le sottoscrizioni per il cliente. Verifica che per tutte sia indicato lo stato **Sospeso**.

5. Seleziona il cliente successivo nell'elenco e ripeti il processo di disabilitazione di tutte le sottoscrizioni.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrazione di sottoscrizioni in base all'uso di Azure

A differenza delle sottoscrizioni CSP di Office 365, non è necessario eseguire manualmente la migrazione delle sottoscrizioni CSP basate sull'utilizzo di Azure. Microsoft Azure supporto eseguirà la migrazione delle sottoscrizioni di Azure e di tutti i servizi o le risorse distribuite dagli account rivenditore **CSP** all'account rivenditore **Transitioning To** CSP. Non ci saranno interruzioni del servizio per il cliente durante la transizione.

1. Assicurarsi che gli account cliente di cui verrà eseguita la migrazione delle sottoscrizioni di Azure abbia accettato il contratto da associare al nuovo account **Transitioning To** CSP.

2. Si invierà una notifica a Microsoft degli account dei clienti pronti per la migrazione e si forniranno i nomi delle società del cliente.

3. Microsoft esegue la migrazione delle sottoscrizioni basate sull'utilizzo di Azure e invia una notifica al termine della migrazione.

4. È necessario verificare che la sottoscrizione di Azure nell'account rivenditore **Transitioning From** CSP sia ora contrassegnata come sospesa **Partner Center** nella sezione sottoscrizioni dei clienti.

5. Verificare che la sottoscrizione di Azure nell'account rivenditore **Transitioning To** CSP (Transizione a CSP) ora mostra lo stato attivo **Partner Center** nella sezione Sottoscrizioni dei clienti.

   >[!Note]
   > La disabilitazione delle sottoscrizioni nel cliente non modifica l'aspetto del cliente nell'elenco Clienti. Attualmente non è disponibile alcuna opzione per rimuovere i clienti dall'elenco. I partner devono evitare di aggiungere di nuovo sottoscrizioni per questi clienti dall'account di **origine della transizione** in futuro.

6. Ripeti questi passaggi per tutte le sottoscrizioni di tutti i clienti per evitare addebiti futuri per gli account di **origini della transizione**. Il partner riceverà una sola fattura finale con un accredito per il numero di giorni inutilizzati tra il giorno di annullamento e l'ultimo giorno del periodo di fatturazione. Non verrà generata alcuna ulteriore fattura dopo questo periodo di fatturazione finale.

### <a name="additional-information"></a>Informazioni aggiuntive

- La disabilitazione della sottoscrizione dall'account **CSP** di transizione da non influisce sul servizio del cliente finale, purché sia stato effettuato il provisioning del servizio dall'account **Transitioning To** CSP prima di disabilitare la sottoscrizione.

- Le sottoscrizioni non possono essere usate dal cliente e non generano addebiti quando vengono sospese o annullate.

- Attualmente non è possibile rimuovere completamente un cliente **dall'elenco** Clienti.
- 
    >[!Note]
    > I partner devono sospendere le sottoscrizioni nell'account tenant partner Di transizione da Partner Center lo stesso giorno in cui tali sottoscrizioni vengono transizione Partner Center e impostate nell'account **transitioning** to per assicurarsi che non si verifichi una doppia fatturazione.  Microsoft non supporterà le richieste di crediti a causa di eventuali sovrapposizioni nella fatturazione dovute all'impostazione non corretta delle sottoscrizioni **transitioning from** su suspended.

### <a name="simplify-migration-using-export"></a>Semplificare la migrazione con l'esportazione

La **funzione di esportazione** consente di recuperare le sottoscrizioni che devi usare nella nuova struttura consolidata:

1. Selezionare **Clienti** nella Partner Center per visualizzare l'elenco dei clienti. 

2. Apri il nome del cliente desiderato.

3. Nella pagina **Sottoscrizioni** selezionare **Esporta** sottoscrizioni per esportare i dettagli delle sottoscrizioni in un file di Excel.

4. Usa questo elenco per ricreare le sottoscrizioni nel nuovo tenant consolidato.

### <a name="api-registration"></a>Registrazione dell'API

Per altre informazioni sulla registrazione dell'API, vedere [Configurare l'accesso alle API in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Passaggi successivi

- [Cloud Solution Provider i mercati regionali e le valute del programma in cui è possibile vendere offerte CSP](regional-authorization-overview.md)
