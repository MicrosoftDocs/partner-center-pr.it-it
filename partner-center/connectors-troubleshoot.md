---
title: Risoluzione dei problemi relativi ai connettori di co-selling
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Risposte alle domande comuni sull'uso dei connettori di co-selling. Leggere queste domande frequenti su come risolvere i problemi relativi ai connettori di co-selling.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148347"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Risoluzione dei problemi relativi ai connettori di co-selling

**Si applica a:** Dynamics 365 CRM | Salesforce CRM

**Ruoli appropriati:** amministratore delle segnalazioni | Amministratore di sistema o a personalizzatore di sistema in CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Domande e risposte sui prerequisiti

1. È possibile usare una soluzione connettori di co-selling per le segnalazioni di valutazione per l'ambiente?

Se si è nell'ambiente di test/gestione temporanea, è possibile scegliere la soluzione di valutazione. La versione a pagamento dei connettori è disponibile in AppSource all'indirizzo US$ 15/mese. Con la connessione a pagamento, si riceveranno 10.000 chiamate API al giorno. I connettori sono wrapper su Partner Center api di segnalazione. Ogni volta che le  soluzioni connettore vengono eseguite per un evento Create o **Update** sulle opportunità Partner Center o sul lato CRM, viene eseguita una chiamata API.

2. Quale ruolo è necessario per creare sezioni nell'ambiente CRM?

Gli utenti amministratori di sistema o a customizer del sistema possono applicare modifiche a tutti gli utenti. Tutti gli utenti dell'app, tuttavia, possono personalizzare il sistema e persino condividere alcune personalizzazioni con altri utenti. 

3. I venditori di partner hanno bisogno di ruoli speciali per lavorare Partner Center?
 
Ai venditori partner deve essere assegnato il ruolo "Amministratore delle segnalazioni". Per altre informazioni, vedere Panoramica [delle autorizzazioni.](create-user-accounts-and-set-permissions.md)

4. Quali campi devono essere impostati per primi nell'ambiente CRM? 

• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trova nell'ambiente CRM in modo accurato. • Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.

5. Quali prerequisiti sono necessari per la creazione Power Automate'ambiente?

Per usare l'Power Automate, è necessario:

- È Power Automate necessaria una licenza.
- È necessaria almeno 1 GB di archiviazione.

6.  È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione Salesforce Connectors?

La soluzione Salesforce Connector è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM. La soluzione non richiede un'istanza di Dynamics 365 o una sottoscrizione. Durante l'installazione della soluzione Salesforce, potrebbe essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda. È necessario selezionare l'ambiente. Inoltre, se viene visualizzato l'errore "Non è stato possibile trovare un'organizzazione dynamics 365 connessa all'utente connesso", sarà necessario creare un nuovo ambiente per il connettore.

## <a name="questions-and-answers-about-configuration"></a>Domande e risposte sulla configurazione

1. Cosa fare se si verifica l'errore seguente durante l'attivazione dei flussi in Power Automate Piattaforma?

Errore: Richiesta di Azure Resource Manager non riuscita con errore: '{"error":{"code":"workflowTriggerNotFound","message":"Il flusso di lavoro 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' non è stato trovato."}}'. 

Seguire questa procedura di risoluzione dei problemi:

- Eliminare la connessione CDS e quindi ricreare le connessioni CDS.
- Attivare e disattivare il flusso figlio 
- Eliminare la soluzione e reinstallarla. 

2.  Cosa fare se si verifica l'errore "Accedi" durante l'aggiunta di un connettore Partner Center in Power Automate Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

Seguire questo passaggio per la risoluzione dei problemi:

- Usare le credenziali Partner Center per accedere all'ambiente di flusso una sola volta (flow.microsoft.com).


3. Cosa è necessario fare se viene visualizzato l'errore seguente durante l'attivazione del Partner Center al flusso CRM in Power Automate Piattaforma?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede aggiornamenti":::

Seguire questi passaggi per la risoluzione dei problemi:

- Attivare i due flussi figlio seguenti prima di attivare il flusso Partner Center al flusso CRM.
      - Partner Center a CRM - Helper (Insider Preview)
      - Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a CRM (Insider Preview)

4. Cosa è necessario fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?

Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.  Se la finestra di dialogo per aggiungere connessioni non si apre automaticamente durante la modifica del flusso, è possibile modificare singolarmente i singoli passaggi e i passaggi secondari dei flussi.

- Selezionare ogni flusso e modificarlo singolarmente.
- Espandere tutti i passaggi nel flusso 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passaggi che necessitano di connessioni":::

- Selezionare i passaggi in cui viene visualizzata un'icona di avviso che chiede di associare le connessioni e aggiungere le connessioni. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modificare il flusso passo per passo":::


5. Cosa è necessario fare se i flussi della soluzione Connettori di segnalazioni di co-selling non si attivano?

A. In Power Automate, è necessario modificare i flussi nell'ordine seguente e aggiornarli per usare le connessioni corrette:

- Partner Center Webhook Registration (Insider Preview)
- Creare segnalazioni di co-selling - Salesforce per Partner Center (Insider Preview)
- Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a Salesforce (Insider Preview)
- Partner Center a Salesforce (Insider Preview)
- Da Salesforce a Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. Per ogni flusso selezionare **l'opzione Esegui solo utenti.** Selezionare **Usa connessione** anziché Fornito **dall'utente di sola esecuzione.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Per attivare un flusso":::


C. Attivare i flussi indicati di seguito:

 - Partner Center aggiornamenti delle segnalazioni di co-selling Microsoft a Salesforce (Insider Preview)

- Da Salesforce a Partner Center (Insider Preview)

    
D. Attivare tutti i flussi rimanenti.

E. In flow Partner Center Webhook Registration (Registrazione webhook) **selezionare Run (Esegui).** Specificare **l'URL HTTP** della prima azione nel **flusso Partner Center a Salesforce.** Selezionare tutte e quattro le opzioni **in Eventi da registrare** e selezionare **Sì** per Sovrascrivi.

## <a name="questions-and-answers-about-runmaintenance"></a>Domande e risposte su Esecuzione/Manutenzione

1. Come risolvere gli errori durante l'Power Automate del flusso?

Per assicurarsi che i flussi Power Automate siano eseguiti come previsto e per risolvere gli errori durante l'esecuzione, vedere [Correggere gli errori di flusso.](/power-automate/fix-flow-failures)

2. Cosa devi fare se vedi segnalazioni non sincronizzate correttamente nell'ambiente Partner Center o CRM?
 
Per determinare lo stato della sincronizzazione dei riferimenti, selezionare **Controlla**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Come sincronizzare le segnalazioni":::

Assicurarsi che siano soddisfatte le condizioni seguenti:

- L'ID soluzione viene fornito come parte dell'opportunità.

- È necessario un codice paese di due lettere.

- Quando si seleziona l'assistenza di Microsoft per l'opportunità, sono necessarie le informazioni di contatto del cliente.

3. Come assicurarsi che una segnalazione verrà sincronizzata bidirezionale?

Eseguire i passaggi seguenti:

- I venditori partner devono assicurarsi di aver abilitato l'opzione **Sincronizza con** Partner Center nella sezione CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Assicurarsi di aver abilitato Synch":::

- I venditori devono fornire ricavi e data di chiusura quando qualificano un lead.

- Se l'ID CRM  viene  specificato nella fase di creazione o aggiornamento dell'opportunità di co-selling, ma un'opportunità lead con tale ID non viene trovata in CRM, l'aggiornamento o la creazione verranno ignorati.

- Assicurarsi che il campo della valuta di riferimento sia configurato nell'ambiente Salesforce. 

4. Cosa fare se il connettore viene disconnesso e si perde una sincronizzazione delle segnalazioni?

Di seguito sono riportate alcune opzioni che è possibile provare:

- Controllare se il nome utente o la password sono scaduti per l Partner Center utente con ruoli di amministratore di riferimento.

- È possibile passare all'opportunità non sincronizzata, eseguire un aggiornamento secondario e osservare se la segnalazione è stata sincronizzata.

- Se i flussi sono stati eseguiti e non riusciti, selezionare il flusso e inviare nuovamente l'esecuzione che ha avuto esito negativo.

5. Cosa è necessario fare quando si ottengono errori di accesso negato?

Assicurarsi che esistano i ruoli appropriati

- Ruolo di amministratore delle segnalazioni per Partner Center venditore 
 
- Ruolo Amministratore di sistema o Asonalizzazione sistema nell'istanza di CRM

- Assicurarsi che l'Power Automate dell'account flusso di lavoro accerta https://flow.microsoft.com l'accesso almeno una volta in anticipo

6. Se viene visualizzato il **codice paese dell'account cliente** mancante durante la creazione di un'opportunità di co-selling, cosa si deve fare?

È necessario aggiungere il codice iso a due lettere del paese all'account cliente in CRM.

7. Cosa fare se viene visualizzato l'errore che indica che **l'ID soluzione è necessario** durante la creazione di un'opportunità di co-selling?

Per creare una segnalazione di co-selling, è necessaria una soluzione pronta per il co-selling Microsoft. 

8. Cosa fare quando vengono create opportunità di co-selling in Partner Center sincronizzate con CRM anche se non sono presenti errori di flusso?

Eseguire le operazioni seguenti:

- Dopo aver creato un nuovo accordo di co-selling in Partner Center, verificare se il flusso Partner Center a Dynamics 365 viene richiamato (potrebbe essere richiamato più volte).

- Se il flusso viene richiamato, controllare tutti i flussi richiamati e identificare l'esecuzione del flusso che aggiornerebbe il CRM. È possibile seguire le azioni e verificare se il CRM è stato aggiornato o si è verificato un problema.

- Selezionare **New deal** in Partner Center per verificare se viene popolato con l'ID CRM.

- Assicurarsi che l'accordo non sia chiuso accidentalmente come **Won** o **Lost** in Partner Center.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)
 
- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
