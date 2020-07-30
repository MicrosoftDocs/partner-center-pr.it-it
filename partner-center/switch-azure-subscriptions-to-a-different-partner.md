---
title: Trasferire la sottoscrizione di Azure a un altro partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il partner del programma Cloud Solution provider associato alle sottoscrizioni di Azure di un cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/29/2020
ms.openlocfilehash: 2ffb35ecb0b0b92b1adfbd11172b14776a5a27d3
ms.sourcegitcommit: d7e620f826cd6570113384c3db34bd96e2f0359b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "87412437"
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
>Non è possibile modificare i partner per le sottoscrizioni Cloud Solution Provider associate ad Azure Plan, Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Cambiare partner per le sottoscrizioni Azure

1. Per trasferire una sottoscrizione di Azure a un nuovo partner, il cliente deve avviare il processo e contattare l'attuale partner del record per la scrittura.

   >[!Note]
   >È responsabilità del partner attuale creare il ticket di servizio che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del nuovo partner. Il cliente deve pianificare di collaborare con il partner corrente per rendere la transizione senza problemi.

2. Il partner per la sottoscrizione deve eseguire le attività seguenti:

   Creare un ticket di servizio Azure dal Centro per i partner per richiedere un trasferimento della sottoscrizione:

   - Dal menu centro per i partner selezionare **clienti**, selezionare il cliente dall'elenco e quindi selezionare **Gestione servizi**. Nella sezione **Ticket di supporto** seleziona l'elenco a discesa **Nuovo ticket** e scegli **Microsoft Azure**.

   - Dal [portale di Azure](https://portal.azure.com)selezionare **nuova richiesta di supporto**.

     Nel passaggio 1 scegli **Gestione della sottoscrizione** come tipo di problema, specifica l'ID sottoscrizione che vuoi trasferire e scegli **Cloud Solution Provider** come piano di supporto.

     Nel passaggio 2 Selezionare **C-minimo Impact** e scegliere **altre domande generali** come tipo di problema.

     Scaricare il [modulo di trasferimento della sottoscrizione CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

3. Partner per la sottoscrizione: compilare il modulo di [trasferimento della sottoscrizione CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA), firmarlo e inviarlo al cliente. Per compilare il modulo, sono necessarie le informazioni seguenti:

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
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > L' **ID tenant** del cliente viene visualizzato nel centro per i partner come **ID Microsoft**del cliente. Per trovare l'ID Microsoft (ID tenant) per un cliente specifico, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner. Quindi selezionare **Customers** dal menu. Individuare il cliente nell'elenco. Selezionare la freccia rivolta verso il basso per espandere l'elenco del cliente. Vengono visualizzate informazioni sul *nome di dominio* del cliente e sull' **ID Microsoft**del cliente. Usare l' **ID Microsoft** a 16 cifre nella cmdlet di PowerShell.

   - Visualizza i ruoli dell'account, inclusi i partner CSP precedenti:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Rimuovere le autorizzazioni di accesso obsolete

   - Nel menu del Centro per i partner scegli **Clienti**.
   - Individuare il cliente nell'elenco. Selezionare (fare doppio clic) il nome della società. Verrà visualizzata la pagina **sottoscrizioni** clienti.
   - Nel menu Customer Details selezionare **gestione dei servizi**.
   - In **Microsoft Azure** fai clic sul link per passare al **Portale di gestione di Microsoft Azure**.

## <a name="next-steps"></a>Passaggi successivi

- Scaricare il [modulo di trasferimento della sottoscrizione CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).
- Informazioni sul [supporto](multipartner.md)per più partner.
- Scopri di più sul supporto per più [canali](multichannel.md).