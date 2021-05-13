---
title: Trasferire la sottoscrizione di Azure a un altro partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il Cloud Solution Provider partner del programma di sottoscrizione associato alle sottoscrizioni di Azure di un cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856067"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Informazioni su come trasferire sottoscrizioni di Azure di un cliente a un altro partner

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** Amministratore globale

Questo articolo descrive in che modo un cliente può passare i servizi Microsoft Azure da un Cloud Solution Provider (CSP) a un altro.

Per passare i servizi o le sottoscrizioni di Azure di un cliente a un partner diverso, seguire questa procedura manuale. Sia il partner che il cliente devono completare la procedura.

>[!Note]  
>Attualmente solo i provider diretti o indiretti possono trasferire le sottoscrizioni.
>Non è possibile modificare i partner per Cloud Solution Provider sottoscrizioni associate al piano di Azure, a Office 365, a Enterprise Mobility Suite o alle sottoscrizioni di Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Cambiare partner per le sottoscrizioni Azure

1. Per trasferire una sottoscrizione di Azure a un nuovo partner, il cliente deve avviare il processo e contattare per scrittura il partner di registrazione corrente.

   >[!Note]
   > È responsabilità del partner corrente creare il ticket di servizio che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del nuovo partner. Il cliente deve pianificare una stretta collaborazione con il partner corrente per semplificare la transizione.

2. Il partner per la sottoscrizione deve eseguire le attività seguenti:

   Creare un ticket di servizio Azure dal Centro per i partner per richiedere un trasferimento della sottoscrizione:

   1. Dal menu Partner Center clienti selezionare **Clienti,** selezionare il cliente dall'elenco e quindi selezionare **Gestione dei servizi.**

   2. Nella sezione **Ticket di supporto** seleziona l'elenco a discesa **Nuovo ticket** e scegli **Microsoft Azure**.
   
   3. Nella pagina [portale di Azure](https://portal.azure.com)selezionare **Nuova richiesta di supporto.**
   
   4. Nel passaggio 1 scegli **Gestione della sottoscrizione** come tipo di problema, specifica l'ID sottoscrizione che vuoi trasferire e scegli **Cloud Solution Provider** come piano di supporto.
   
   5. Nel passaggio 2 selezionare **Impatto minimo C** e scegliere Altre domande **generali** come tipo di problema.
   
   6. Scaricare il [modulo di trasferimento della sottoscrizione CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Partner per la sottoscrizione: compilare il modulo CSP Subscription Transfer (Trasferimento della sottoscrizione [CSP),](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)firmarlo e inviarlo al cliente. 

   Per compilare il modulo, sono necessarie le informazioni seguenti:

   - ID Microsoft e informazioni di contatto del partner corrente. Nel menu del Centro per i partner seleziona **Impostazioni account** &gt; **Profilo organizzazione** e usa i valori indicati per **ID Microsoft**, **Nome organizzazione** e **Indirizzo**.

   - ID Microsoft del cliente. Nel menu del Centro per i partner seleziona **Clienti** e quindi espandi l'elenco dei clienti per visualizzare il relativo **ID Microsoft**.

   - ID sottoscrizione da trasferire. Nell'elenco dei clienti espanso seleziona **Visualizza sottoscrizioni**, quindi espandi la sottoscrizione scelta per vedere l'**ID sottoscrizione**.

   >[!Note]
   >Il trasferimento di una sottoscrizione comporta due ID  sottoscrizione che verranno visualizzati nella pagina Modifica sottoscrizione della sottoscrizione trasferita: **1**- L'ID sottoscrizione di Partner Center viene usato ai fini della fatturazione. **2:** l'ID sottoscrizione di Azure originale viene mantenuto e verrà visualizzato in Partner Center e nel portale di gestione di Azure. Questo ID verrà visualizzato nel file di ricognizione.  **Quando si esegue la registrazione dei ticket di supporto, è necessario usare entrambi gli ID.**

4. Il cliente e il nuovo partner per la sottoscrizione:

   Esamina il modulo, compila le informazioni sul nuovo partner e firmalo. Verifica che per il nuovo cliente sia in vigore un contratto. Invia il modulo al Partner of Record corrente.

   *Importante:* se il nuovo partner CSP non ha una relazione di rivenditore con il cliente, deve stabilirne una prima del trasferimento della sottoscrizione. [Puoi trovare informazioni sulla procedura qui](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Il nuovo partner CSP e il tenant del cliente devono essere nello stesso paese. 

5. Partner corrente:

   Assicurarsi che il modulo includa informazioni di contatto per entrambi gli amministratori partner. Supporto tecnico Microsoft contattare entrambi gli amministratori per verificare il trasferimento. Assicurarsi di avere tutte e tre le firme. Usare quindi **l'opzione Caricamento** file per collegare il modulo completato alla richiesta di servizio esistente. Un tecnico del supporto Microsoft tornerà all'utente entro otto ore lavorative per convalidare la ricezione e il completamento.

6. Nuovo partner:

   Aggiorna le impostazioni della sottoscrizione di Azure per rimuovere il partner precedente dall'account. Per visualizzare le assegnazioni di ruolo di cui viene eseguito il provisioning, eseguire due commandlet di PowerShell.

   - Aggiungi il nuovo partner come rivenditore nell'account:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > L'ID **tenant del** cliente viene Partner Center come ID Microsoft del **cliente.** Per trovare l'ID Microsoft (ID tenant) per un cliente specifico, accedere al [dashboard Partner Center.](https://partner.microsoft.com/dashboard) Selezionare quindi **Clienti** dal menu. Individuare il cliente nell'elenco. Selezionare la freccia giù per espandere l'elenco del cliente. Verranno visualizzate informazioni sul nome di dominio *del* cliente e sull'ID Microsoft del **cliente.** Usare **l'ID Microsoft** a 16 cifre nel cmdlet di PowerShell.

   - Visualizza i ruoli dell'account, inclusi i partner CSP precedenti:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Rimuovere le autorizzazioni di accesso obsolete:

   - Nel menu del Centro per i partner scegli **Clienti**.
   - Individuare il cliente nell'elenco. Selezionare (doppio clic) il nome della società. Questa azione apre la pagina **Sottoscrizioni del** cliente.
   - Nel menu dei dettagli del cliente selezionare **Gestione dei servizi.**
   - In **Microsoft Azure** selezionare il collegamento per passare al **portale di gestione di Microsoft Azure**.

## <a name="next-steps"></a>Passaggi successivi

- Scaricare il [modulo di trasferimento della sottoscrizione CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Informazioni sul [supporto multi-partner.](multipartner.md)

- [Supporto multi-partner](multipartner.md).
- [supporto multicanale](multichannel.md).
- [Trasferire le sottoscrizioni di Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)