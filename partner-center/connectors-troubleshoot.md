---
title: Risoluzione dei problemi relativi ai connettori di co-selling
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sulle risposte alle domande comuni sull'uso dei connettori di co-selling. Leggere le domande frequenti su come risolvere i problemi di co-selling.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031264"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Risoluzione dei problemi relativi ai connettori di co-selling

**Si applica a:**

- Centro per i partner
- Dynamics 365 CRM
- CRM Salesforce

**Ruoli appropriati**

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Domande e risposte sui prerequisiti

1. È possibile usare una soluzione di valutazione per la co-selling dei connettori per l'ambiente?

Se si utilizza l'ambiente di test/gestione temporanea, è possibile optare per la soluzione di valutazione. La versione a pagamento dei connettori è disponibile in AppSource a 15 dollari al mese. Con la connessione a pagamento, si otterranno 10.000 chiamate API al giorno. I connettori sono wrapper oltre alle API di riferimento del centro per i partner. Ogni volta che le soluzioni del connettore vengono eseguite per un evento di **creazione** o **aggiornamento** in caso di opportunità in un centro per i partner o sul lato CRM, viene eseguita una chiamata API.

2. Quale ruolo è necessario per creare sezioni nell'ambiente CRM?

Gli utenti che sono amministratori di sistema o personalizzatori di sistema possono applicare modifiche a tutti. Tutti gli utenti dell'app, tuttavia, possono personalizzare il sistema e persino condividere alcune delle loro personalizzazioni con altri utenti. 

3. I venditori partner hanno bisogno di ruoli speciali per lavorare al centro per i partner?
 
Ai venditori partner deve essere assegnato il ruolo di amministratore dei riferimenti. Per ulteriori informazioni, fare riferimento a [Cenni preliminari sulle autorizzazioni) (Create-User-Accounts-and-set-permissions).

4. Quali campi devono essere impostati per primi nell'ambiente CRM? 

• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trovi in un ambiente CRM in modo accurato. • Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.

5. Quali prerequisiti sono necessari per la creazione dell'ambiente di Power Automatic?

Per usare l'ambiente Power automatizzate, è necessario quanto segue:

- È necessaria una licenza di Power automatici.
- È necessario almeno 1 GB di spazio di archiviazione.

6.  È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione connettori Salesforce?

La soluzione del connettore Salesforce è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM. Per la soluzione non è necessario disporre di un'istanza di Dynamics 365 o di una sottoscrizione. Durante l'installazione della soluzione Salesforce, può essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda. È necessario selezionare l'ambiente. Inoltre, se si riceve l'errore "non è stato possibile trovare un'organizzazione Dynamics 365 connessa all'utente connesso", sarà necessario creare un nuovo ambiente per il connettore.

## <a name="questions-and-answers-about-configuration"></a>Domande e risposte sulla configurazione

1. Cosa si deve fare se si affronta l'errore seguente durante l'attivazione dei flussi nella piattaforma Power automatizzate?

Errore: la richiesta di Azure Resource Manager non è riuscita con errore:' {"Error": {"code": "WorkflowTriggerNotFound", "message": "Impossibile trovare il trigger ' manual ' del flusso di lavoro."}}'. 

Seguire questa procedura di risoluzione dei problemi:

- Eliminare la connessione CDS e quindi ricreare le connessioni CDS.
- Attivare e disattivare il flusso figlio 
- Eliminare la soluzione e reinstallare la soluzione. 

2.  Cosa si deve fare se si affronta l'errore di "accesso" durante l'aggiunta di un connettore del centro per i partner nella piattaforma Power automatizzate?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

Seguire questa procedura di risoluzione dei problemi:

- Usare le credenziali del centro per i partner per accedere all'ambiente Microsoft Flow una volta (flow.microsoft.com).


3. Cosa è necessario fare se viene visualizzato l'errore seguente quando si attiva il centro per i partner al flusso di CRM nella piattaforma Power automatizzate?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede l'accesso":::

Seguire questa procedura di risoluzione dei problemi:

- Attivare i seguenti due flussi figlio prima di attivare il centro per i partner al flusso CRM.
      - Centro per i partner per CRM-Helper (insider Preview)
      - Partner Center Microsoft co-selling degli aggiornamenti di riferimento a CRM (insider Preview)

4. Cosa fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?

Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.  Se la finestra di dialogo per l'aggiunta di connessioni non viene aperta automaticamente durante la modifica del flusso, è possibile modificare singolarmente i passaggi e i passaggi secondari dei flussi.

- Selezionare ogni flusso e modificarli singolarmente.
- Espandi tutti i passaggi nel flusso 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Messaggio di errore che richiede l'accesso":::

- Selezionare i passaggi in cui viene visualizzata un'icona di avviso che richiede di associare le connessioni e di aggiungere connessioni. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Messaggio di errore che richiede l'accesso":::


5. Cosa si deve fare se i flussi della soluzione per la co-selling dei connettori per i riferimenti non vengono attivati?

R. In Power automatizzate, sarà necessario modificare i flussi nell'ordine seguente e aggiornarli in modo da usare le connessioni corrette:

- Registrazione webhook del centro per i partner (anteprima Insider)
- Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)
- Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)
- Da partner Center a Salesforce (insider Preview)
- Da Salesforce al centro per i partner (anteprima di Insider)
- Opportunità di Salesforce per il centro per i partner (anteprima Insider)
- Salesforce Microsoft Solutions to partner Center (insider Preview)

 B. Per ogni flusso, selezionare l'opzione **Esegui solo utenti** . Selezionare **Usa connessione** anziché **fornita dall'utente di sola esecuzione**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Messaggio di errore che richiede l'accesso":::


C. Attivare questi flussi indicati di seguito:

 - Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)

- Da Salesforce al centro per i partner (anteprima di Insider)

    
D. Attivare tutti i flussi rimanenti.

E. Nella registrazione del webhook del centro per i partner Microsoft Flow selezionare **Esegui**. Fornire l' **URL http** dalla prima azione nel **centro per i partner al flusso di Salesforce** . Selezionare tutte e quattro le opzioni in **eventi da registrare** e selezionare **Sì** per Sovrascrivi.

## <a name="questions-and-answers-about-runmaintenance"></a>Domande e risposte su esecuzione/manutenzione

1. Come si risolvono i problemi in caso di errori durante l'esecuzione di Power automatizzare il flusso?

Per assicurarsi che i flussi vengano eseguiti come previsto e per risolvere gli errori durante l'esecuzione, vedere correggere gli [errori di flusso](/power-automate/fix-flow-failures).

2. Cosa è necessario fare se vengono visualizzati riferimenti che non sono sincronizzati correttamente nel centro per i partner o nell'ambiente CRM?
 
Per determinare lo stato della sincronizzazione dei riferimenti, selezionare **controllo**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Messaggio di errore che richiede l'accesso":::

Verificare che siano soddisfatte le condizioni seguenti:

- L'ID soluzione viene fornito come parte dell'opportunità.

- Il codice paese a due lettere è obbligatorio.

- Quando la Guida di Microsoft è selezionata per l'opportunità, le informazioni di contatto del cliente sono obbligatorie.

3. Come verificare che il riferimento venga sincronizzato in modo bidirezionale?

Eseguire i passaggi seguenti:

- Per i venditori partner è necessario assicurarsi di aver abilitato l'opzione **Sync with partner Center** nella sezione CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Messaggio di errore che richiede l'accesso" nel centro per i partner.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)
 
- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)