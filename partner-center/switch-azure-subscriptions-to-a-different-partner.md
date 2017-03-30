---
title: Passare le sottoscrizioni Azure a un altro partner | Centro partner
description: "Un cliente può cambiare il partner del programma Cloud Solution Provider (CSP) scelto per i servizi di Microsoft Azure. Tuttavia, questo è un processo manuale che richiede l&quot;intervento sia del partner che del cliente."
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.openlocfilehash: ec227dac6f8b0625120bf4b5d1bc76fbeaaae635
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="switch-azure-subscriptions-to-a-different-partner"></a>Passare le sottoscrizioni Azure a un altro partner

**Si applica a**

-  Centro per i partner

Un cliente può cambiare il partner del programma Cloud Solution Provider (CSP) scelto per i servizi di Microsoft Azure. Tuttavia, questo è un processo manuale che richiede l'intervento sia del partner che del cliente.

**Nota**  Non esiste attualmente un processo automatico che consenta ai clienti di Azure di passare al programma CSP da EA, Open o altri programmi di licenza. Questo è un processo manuale che richiede l'intervento sia del partner che del cliente. Inoltre, attualmente non è possibile cambiare partner per le sottoscrizioni Cloud Solution Provider per Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

 

**Cambiare partner per le sottoscrizioni Azure**

1.  Per trasferire una sottoscrizione Azure a un nuovo partner, il cliente deve avviare il processo e contattare il partner CSP Partner of Record corrente in forma scritta.

2.  Il CSP per la sottoscrizione deve eseguire le attività seguenti:

    Creare un ticket di servizio Azure dal Centro per i partner per richiedere un trasferimento della sottoscrizione:

    -   Nel menu Dashboard del Centro per i partner seleziona **Clienti**, seleziona il cliente nell'elenco e quindi seleziona **Gestione servizi**. Nella sezione **Ticket di supporto** seleziona l'elenco a discesa **Nuovo ticket** e scegli **Microsoft Azure**.

    -   Nel portale di Azure seleziona **Nuova richiesta di supporto**.

        Nel passaggio 1 scegli **Gestione della sottoscrizione** come tipo di problema, specifica l'ID sottoscrizione che vuoi trasferire e scegli **Cloud Solution Provider** come piano di supporto.

        Nel passaggio 2 seleziona **C–Impatto minimo** e scegli **Domande generali** come tipo di problema.

        Scarica il [modulo per il trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Partner CSP corrente per la sottoscrizione: compila il [modulo per il trasferimento della sottoscrizione CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), firmalo e quindi invialo al cliente. Per compilare il modulo, sono necessarie le informazioni seguenti:

    -   ID Microsoft e informazioni di contatto del partner corrente. Nel menu del Centro per i partner seleziona **Impostazioni account** &gt; **Profilo organizzazione** e usa i valori indicati per **ID Microsoft**, **Nome organizzazione** e **Indirizzo**.

    -   ID Microsoft del cliente. Nel menu del Centro per i partner seleziona **Clienti** e quindi espandi l'elenco dei clienti per visualizzare il relativo **ID Microsoft**.

    -   ID sottoscrizione da trasferire. Nell'elenco dei clienti espanso seleziona **Visualizza sottoscrizioni**, quindi espandi la sottoscrizione scelta per vedere l'**ID sottoscrizione**.

4.  Cliente e nuovo CSP per la sottoscrizione:

    Esamina il modulo, compila le informazioni sul nuovo partner e firmalo. Verifica che per il nuovo cliente sia in vigore un contratto. Invia il modulo al Partner of Record corrente.

    *Importante*: se il nuovo partner CSP non ha una relazione come rivenditore con il cliente, deve stabilirne una prima del trasferimento della sottoscrizione. [Puoi trovare informazioni sulla procedura qui](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

5.  Partner CSP corrente:

    Verifica che il modulo includa le informazioni di contatto per entrambi gli amministratori del partner: il personale del servizio di supporto Microsoft contatterà entrambi gli amministratori per verificare il trasferimento. Verifica che siano presenti tutte e tre le firme e quindi allega il modulo completo alla richiesta di servizio esistente usando l'opzione **Caricamento file**. Un tecnico del supporto Microsoft ti contatterà entro 8 ore lavorative per confermare la ricezione e il completamento.

6.  Nuovo partner CSP:

    Aggiorna le impostazioni della sottoscrizione di Azure per rimuovere il partner precedente dall'account. Per vedere le assegnazioni di ruolo di cui è stato effettuato il provisioning, esegui due cmdlet di PowerShell.

    -   Aggiungi il nuovo partner come rivenditore nell'account:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "NomeDominioCliente"**

        Per trovare il nome di dominio del cliente: nel menu del Centro per i partner scegli **Clienti**. Seleziona il cliente nell'elenco dei clienti. Nel menu del cliente scegli **Account** e usa le informazioni in **Nome di dominio**.

    -   Visualizza i ruoli dell'account, inclusi i partner CSP precedenti:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    Rimuovi le risorse e le autorizzazioni di accesso obsolete per la sottoscrizione gestendo la sottoscrizione nel portale di Azure. Nel menu del Centro per i partner scegli **Clienti**. Espandi l'elenco dei clienti e seleziona **Visualizza sottoscrizioni**. Nel menu del cliente scegli **Gestione servizi**. In **Microsoft Azure** fai clic sul link per passare al **Portale di gestione di Microsoft Azure**.

 

 



