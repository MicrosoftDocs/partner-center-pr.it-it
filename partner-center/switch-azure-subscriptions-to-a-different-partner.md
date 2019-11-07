---
title: Trasferire le sottoscrizioni Azure | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Un cliente può cambiare il partner del programma Cloud Solution Provider (CSP) scelto per i servizi di Microsoft Azure. Tuttavia, questo è un processo manuale che richiede l'intervento sia del partner che del cliente.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.author: evansma
keywords: sottoscrizione di azure, cambiare partner, sostituire partner, ottenere nuovo partner, partner diverso
ms.localizationpriority: medium
ms.openlocfilehash: a0dd17c56e04368be430808ab5191a6c5adca8cf
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651538"
---
# <a name="transfer-azure-subscriptions"></a>Trasferire le sottoscrizioni di Azure 

**Si applica a**

-  Centro per i partner

Un cliente può decidere di passare a un partner Cloud Solution Provider o a un altro partner per i servizi di Microsoft Azure. Si tratta, tuttavia, di un processo manuale che richiede l'intervento sia del partner che del cliente.

>[!Note]  
>In questo momento solo i provider diretti o indiretti sono in grado di trasferire le sottoscrizioni.
>Non è attualmente possibile modificare i partner per le sottoscrizioni Cloud Solution Provider per le sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.



**Cambia partner per le sottoscrizioni di Azure**

1. Per trasferire una sottoscrizione Azure a un nuovo partner, il cliente deve avviare il processo e contattare il Partner of Record corrente in forma scritta. 
>[!Note]
>È responsabilità del partner attuale creare il ticket di servizio che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del nuovo partner. Il cliente deve pianificare di lavorare a stretto contatto con il partner attuale per facilitare la transizione.

2. Il partner per la sottoscrizione deve effettuare le attività seguenti:

Creare un ticket di servizio Azure dal Centro per i partner per richiedere un trasferimento della sottoscrizione:
-   Dal menu centro per i partner selezionare **clienti**, selezionare il cliente dall'elenco e quindi selezionare **Gestione servizi**. Nella sezione **Ticket di supporto** seleziona l'elenco a discesa **Nuovo ticket** e scegli **Microsoft Azure**.

-   Nel portale di Azure seleziona **Nuova richiesta di supporto**.

Nel passaggio 1 scegli **Gestione della sottoscrizione** come tipo di problema, specifica l'ID sottoscrizione che vuoi trasferire e scegli **Cloud Solution Provider** come piano di supporto.

Nel passaggio 2 Selezionare **C-minimo Impact** e scegliere **altre domande generali** come tipo di problema.

Scarica il [modulo per il trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. Il partner corrente per la sottoscrizione: compila il [modulo per il trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), firmalo e quindi invialo al cliente. Per compilare il modulo, sono necessarie le informazioni seguenti:

- ID Microsoft e informazioni di contatto del partner corrente. Nel menu centro partner selezionare **Impostazioni Account** &gt; **profilo organizzazione**e usare l' **ID Microsoft**, il nome dell' **organizzazione**e l' **Indirizzo** elencati qui.

- ID Microsoft del cliente. Nel menu del Centro per i partner seleziona **Clienti** e quindi espandi l'elenco dei clienti per visualizzare il relativo **ID Microsoft**.

- ID sottoscrizione da trasferire. Nell'elenco dei clienti espanso seleziona **Visualizza sottoscrizioni**, quindi espandi la sottoscrizione scelta per vedere l'**ID sottoscrizione**.

>[!Note]
>Il trasferimento di una sottoscrizione comporta la generazione di due ID sottoscrizione che verranno visualizzati nella pagina **Modifica sottoscrizione** della sottoscrizione trasferita: **1**- L'ID sottoscrizione del Centro per i partner viene utilizzato per scopi di fatturazione. 
**2**- L'ID sottoscrizione di Azure originale viene mantenuto e sarà visualizzato nel Centro per i partner e nel portale di gestione di Azure. Questo ID verrà visualizzato nel file di riconoscimento.  **Quando si registrano ticket di supporto, è necessario usare entrambi gli ID.**

4. Il cliente e nuovo partner per la sottoscrizione:

Esamina il modulo, compila le informazioni sul nuovo partner e firmalo. Verifica che per il nuovo cliente sia in vigore un contratto. Invia il modulo al Partner of Record corrente.

*Importante*: se il nuovo partner CSP non ha una relazione come rivenditore con il cliente, deve stabilirne una prima del trasferimento della sottoscrizione. [Puoi trovare informazioni sulla procedura qui](request-a-relationship-with-a-customer.md).

>[!Note]
>Il nuovo partner CSP e il tenant del cliente devono trovarsi nello stesso paese. 

5. Partner corrente:

Verifica che il modulo includa le informazioni di contatto per entrambi gli amministratori del partner: il personale del servizio di supporto tecnico Microsoft contatterà entrambi gli amministratori per verificare il trasferimento. Verifica che siano presenti tutte e tre le firme e quindi allega il modulo completo alla richiesta di servizio esistente usando l'opzione **Caricamento file**. Un tecnico del supporto Microsoft ti contatterà entro 8 ore lavorative per confermare la ricezione e il completamento.

6. Nuovo partner:

Aggiorna le impostazioni della sottoscrizione di Azure per rimuovere il partner precedente dall'account. Per vedere le assegnazioni di ruolo di cui è stato effettuato il provisioning, esegui due cmdlet di PowerShell.

-   Aggiungi il nuovo partner come rivenditore nell'account:

**PS C:\\&gt; Add-AzureRMAccount-tenant "CustomerDomainName"**

Per trovare il nome di dominio del cliente: nel menu del Centro per i partner scegli **Clienti**. Seleziona il cliente nell'elenco dei clienti. Nel menu del cliente scegli **Account** e usa le informazioni in **Nome di dominio**.

-   Visualizza i ruoli dell'account, inclusi i partner CSP precedenti:

**PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Rimuovi le autorizzazioni di accesso obsolete

-  Nel menu del Centro per i partner scegli **Clienti**. 
-  Espandi l'elenco dei clienti e seleziona **Visualizza sottoscrizioni**. 
-  Nel menu del cliente seleziona **Gestione servizi**. 
-  In **Microsoft Azure** fai clic sul link per passare al **Portale di gestione di Microsoft Azure**.

 

 



