---
title: Trasferire le sottoscrizioni di Azure a un altro partner
ms.topic: article
ms.date: 04/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come consentire a un cliente di modificare il partner del programma CSP associato alle sottoscrizioni di Azure di un cliente.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: LauraBrenner
ms.author: labrenne
keywords: sottoscrizione di Azure, switch partner, cambia partner, Ottieni nuovo partner, partner diverso
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 5976cba3c0d1ef6984fc88497412577e83e999f7
ms.sourcegitcommit: 53476b7837192fa4d60470bd5b99e5355e7e48c0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2020
ms.locfileid: "82205579"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Informazioni su come trasferire le sottoscrizioni di Azure di un cliente a un altro partner

**Si applica a**

- Centro per i partner per Microsoft Cloud for US Government
- Centro per i partner per Microsoft Global Cloud
- Partner inclusi nel programma Cloud Solution Provider (CSP)

Questo articolo descrive come un cliente può cambiare i servizi Microsoft Azure da un provider di soluzioni cloud (CSP) a un altro.

Per passare i servizi o le sottoscrizioni di Azure di un cliente a un altro partner, seguire questa procedura manuale. Sia il partner che il cliente devono completare la procedura.

>[!Note]  
>Attualmente, solo i provider diretti o indiretti possono trasferire le sottoscrizioni.
>Non è possibile modificare i partner per le sottoscrizioni Cloud Solution Provider associate alle sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

**Cambiare partner per le sottoscrizioni Azure**

1. Per trasferire una sottoscrizione di Azure a un nuovo partner, il cliente deve avviare il processo e contattare l'attuale partner del record per la scrittura.

   >[!Note]
   >È responsabilità del partner attuale creare il ticket di servizio che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del nuovo partner. Il cliente deve pianificare di collaborare con il partner corrente per rendere la transizione senza problemi.

2. Il partner per la sottoscrizione deve eseguire le attività seguenti:

   Creare un ticket di servizio Azure dal Centro per i partner per richiedere un trasferimento della sottoscrizione:

   - Dal menu centro per i partner selezionare **clienti**, selezionare il cliente dall'elenco e quindi selezionare **Gestione servizi**. Nella sezione **Ticket di supporto** seleziona l'elenco a discesa **Nuovo ticket** e scegli **Microsoft Azure**.

   - Dal [portale di Azure](https://portal.azure.com)selezionare **nuova richiesta di supporto**.

     Nel passaggio 1 scegli **Gestione della sottoscrizione** come tipo di problema, specifica l'ID sottoscrizione che vuoi trasferire e scegli **Cloud Solution Provider** come piano di supporto.

     Nel passaggio 2 Selezionare **C-minimo Impact** e scegliere **altre domande generali** come tipo di problema.

     Scaricare il [modulo di trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. Partner per la sottoscrizione: compilare il modulo di [trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), firmarlo e inviarlo al cliente. Per compilare il modulo, sono necessarie le informazioni seguenti:

   - ID Microsoft e informazioni di contatto del partner corrente. Nel menu del Centro per i partner seleziona **Impostazioni account** &gt; **Profilo organizzazione** e usa i valori indicati per **ID Microsoft**, **Nome organizzazione** e **Indirizzo**.

   - ID Microsoft del cliente. Nel menu del Centro per i partner seleziona **Clienti** e quindi espandi l'elenco dei clienti per visualizzare il relativo **ID Microsoft**.

   - ID sottoscrizione da trasferire. Nell'elenco dei clienti espanso seleziona **Visualizza sottoscrizioni**, quindi espandi la sottoscrizione scelta per vedere l'**ID sottoscrizione**.

   >[!Note]
   >Il trasferimento di una sottoscrizione comporta due ID di sottoscrizione che verrà visualizzato nella pagina **Modifica sottoscrizione** della sottoscrizione trasferita: **1**. l'ID sottoscrizione del centro per i partner viene usato ai fini della fatturazione. **2**-l'ID sottoscrizione di Azure originale viene mantenuto e verrà visualizzato nel centro per i partner e nel portale di gestione di Azure. Questo ID verrà visualizzato nel file di ricognizione.  **Quando si registrano ticket di supporto, è necessario usare entrambi gli ID.**

4. Il cliente e il nuovo partner per la sottoscrizione:

   Esamina il modulo, compila le informazioni sul nuovo partner e firmalo. Verifica che per il nuovo cliente sia in vigore un contratto. Invia il modulo al Partner of Record corrente.

   *Importante*: se il nuovo partner CSP non ha una relazione del rivenditore con il cliente, deve stabilirne uno prima del trasferimento della sottoscrizione. [Puoi trovare informazioni sulla procedura qui](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Il nuovo partner CSP e il tenant del cliente devono trovarsi nello stesso paese. 

5. Partner corrente:

   Verificare che il modulo includa le informazioni di contatto per entrambi gli amministratori partner. Supporto tecnico Microsoft contatterà entrambi gli amministratori per verificare il trasferimento. Assicurarsi di disporre di tutte e tre le firme. Usare quindi l'opzione di **caricamento file** per allegare il form completato alla richiesta di servizio esistente. Un tecnico del supporto Microsoft riceverà un ritorno entro otto ore lavorative per convalidare la ricezione e il completamento.

6. Nuovo partner:

   Aggiorna le impostazioni della sottoscrizione di Azure per rimuovere il partner precedente dall'account. Per visualizzare le assegnazioni di ruolo di cui è stato effettuato il provisioning, eseguire due cmdlet di PowerShell.

   - Aggiungi il nuovo partner come rivenditore nell'account:

     ```powershell
     Add-AzureRMAccount -tenant "CustomerDomainName"
     ```

     Per trovare il nome di dominio del cliente: nel menu del Centro per i partner scegli **Clienti**. Seleziona il cliente nell'elenco dei clienti. Nel menu del cliente scegli **Account** e usa le informazioni in **Nome di dominio**.

   - Visualizza i ruoli dell'account, inclusi i partner CSP precedenti:

     ```powershell
     Get-AzureRMRoleAssignment
     ```

7. Rimuovere le autorizzazioni di accesso obsolete

   - Nel menu del Centro per i partner scegli **Clienti**.
   - Espandi l'elenco dei clienti e seleziona **Visualizza sottoscrizioni**.
   - Nel menu del cliente seleziona **Gestione servizi**.
   - In **Microsoft Azure** fai clic sul link per passare al **Portale di gestione di Microsoft Azure**.