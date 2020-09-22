---
title: Risolvere i problemi relativi ai connettori di co-selling
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Domande frequenti su come risolvere i problemi di co-selling.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: ad09d7c805ce5a1138d7546fd041ae1eda77b00c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91002972"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Risolvere i problemi relativi ai connettori di co-selling

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

4. Quali sono i campi che devono essere configurati per primi nell'ambiente CRM? 

• Assicurarsi che la valuta sia appropriata per la propria posizione e che si trovi in un ambiente CRM in modo accurato. • Il team di vendita deve essere elencato nell'ambiente CRM come utenti CRM.

5.  Quali prerequisiti sono necessari per la creazione dell'ambiente di Power Automatic?

Per usare l'ambiente Power automatizzate, è necessario quanto segue:

- È necessaria una licenza di Power automatici.
- È necessario almeno 1 GB di spazio di archiviazione.

6.  È necessaria una sottoscrizione di Dynamics 365 per usare la soluzione connettori Salesforce?

La soluzione del connettore Salesforce è di tipo "Dynamics Flow" che supporta la sincronizzazione con altri sistemi CRM. Per la soluzione non è necessario disporre di un'istanza di Dynamics 365 o di una sottoscrizione. Durante l'installazione della soluzione Salesforce, può essere visualizzato un elenco a discesa con l'ambiente CDS esistente nell'azienda. È necessario selezionare l'ambiente. Inoltre, se si riceve l'errore non è stata trovata un'organizzazione Dynamics 365 connessa all'utente connesso ", sarà necessario creare un nuovo ambiente per il connettore.

## <a name="questions-and-answers-about-configuration"></a>Domande e risposte sulla configurazione

1. Cosa si deve fare se si affronta l'errore seguente durante l'attivazione dei flussi nella piattaforma Power automatizzate?

Errore: la richiesta di Azure Resource Manager non è riuscita con errore:' {"Error": {"code": "WorkflowTriggerNotFound", "message": "Impossibile trovare il trigger ' manual ' del flusso di lavoro."}}'. 

Seguire questa procedura di risoluzione dei problemi:

- Eliminare la connessione CDS e quindi ricreare le connessioni CDS.
- Attivare e disattivare il flusso figlio 
- Eliminare la soluzione e reinstallare la soluzione. 

2.  Cosa si deve fare se si affronta l'errore seguente durante l'aggiunta di un connettore del centro per i partner nella piattaforma Power automatizzate?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Messaggio di errore che richiede l'accesso":::

Seguire questa procedura di risoluzione dei problemi:

- Usare l'accesso al centro per i partner per accedere all'ambiente Microsoft Flow una volta (flow.microsoft.com).


3. Cosa è necessario fare se viene visualizzato l'errore seguente quando si attiva il centro per i partner al flusso di CRM nella piattaforma Power automatizzate?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Messaggio di errore che richiede aggiornamenti":::

Seguire questa procedura di risoluzione dei problemi:

- Attivare i seguenti due flussi figlio prima di attivare il centro per i partner al flusso CRM.
      - Centro per i partner per CRM-Helper (insider Preview)
      - Partner Center Microsoft co-selling degli aggiornamenti di riferimento a CRM (insider Preview)

4. Cosa fare quando non è possibile aggiungere connessioni al flusso quando si tenta di modificare il flusso?

Si aggiungono connessioni al flusso mentre il flusso è in esecuzione e si aggiungono a ogni flusso separatamente.  Se la finestra di dialogo per l'aggiunta di connessioni non viene aperta automaticamente durante la modifica del flusso, è possibile modificare ognuno dei passaggi e dei sottopassaggi dei flussi per aggiungere le connessioni.

- Selezionare ogni flusso e modificarli singolarmente.
- Espandi tutti i passaggi nel flusso 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Passaggi che richiedono connessioni":::

- Selezionare i passaggi in cui viene visualizzata un'icona di avviso che richiede di associare le connessioni e di aggiungere connessioni. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Modificare il flusso passo per passo":::


5. Cosa è necessario fare se i flussi della soluzione di co-selling dei connettori per i riferimenti non vengono attivati (attivazione)?

    R. In Power automatizzate, sarà necessario modificare i flussi nell'ordine seguente e aggiornarli per usare le rispettive connessioni:

    - Registrazione webhook del centro per i partner (anteprima Insider)
    - Creare un riferimento di co-selling-Salesforce al centro per i partner (anteprima Insider)
    - Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Salesforce (insider Preview)
    - Da partner Center a Salesforce (insider Preview)
    - Da Salesforce al centro per i partner (anteprima di Insider)
    - Opportunità di Salesforce per il centro per i partner (anteprima Insider)
    - Salesforce Microsoft Solutions to partner Center (insider Preview)

    B. Per ogni flusso, selezionare l'opzione **Esegui solo utenti** . Selezionare **Usa connessione** anziché **fornita dall'utente di sola esecuzione**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Per attivare un flusso":::

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

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Come sincronizzare i riferimenti":::

Verificare che siano soddisfatte le condizioni seguenti:

- L'ID soluzione viene fornito come parte dell'opportunità.

- Il codice paese a due lettere è obbligatorio.

- Quando la Guida di Microsoft è selezionata per l'opportunità, le informazioni di contatto del cliente sono obbligatorie.

3. In quali condizioni un riferimento non verrà sincronizzato in maniera bidirezionale

Verificare quanto segue:

- Per i venditori partner è necessario assicurarsi di aver abilitato l'opzione **Sync with partner Center** nella sezione CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Assicurarsi di aver abilitato la sincronizzazione":::

- I venditori devono fornire i ricavi e la data di chiusura quando qualificano un responsabile.

- Se l'ID CRM viene fornito durante la creazione o l'aggiornamento dell'opportunità di co-selling e se non viene trovato un lead o un'opportunità con tale ID in CRM, l'aggiornamento o la creazione verranno ignorati per tale opportunità.

- Verificare che il campo valuta referral sia configurato nell'ambiente Salesforce. 

4. Cosa è necessario fare se il connettore viene disconnesso e non viene eseguita una sincronizzazione dei riferimenti. 

Di seguito sono riportate alcune delle opzioni che è possibile provare:

- Controllare se il nome utente o la password è scaduta per l'utente del centro per i partner con i ruoli di amministratore di riferimento.

- È possibile passare all'opportunità non sincronizzata, effettuare un aggiornamento secondario e osservare se il riferimento è stato sincronizzato.

- Se i flussi sono stati eseguiti e non riusciti, selezionare il flusso e inviare di nuovo l'esecuzione che ha avuto esito negativo.

5. Cosa si deve fare quando si ricevono errori di accesso negato?

Verificare che siano presenti i ruoli appropriati

- Ruolo di amministratore di riferimento per il venditore del centro partner 
 
- Ruolo di amministratore di sistema o di sistema verbi nell'istanza di CRM

- Assicurarsi che l'utente di Power automatizzare l'accesso https://flow.microsoft.com all'account di flusso almeno una volta in anticipo

6. Se si nota che il **codice paese dell'account del cliente** non è presente durante la creazione di un'opportunità di co-selling, cosa si deve fare?

È necessario aggiungere il codice di paese a due lettere ISO all'account del cliente in CRM.

7. Cosa è necessario fare se viene visualizzato l'errore relativo all' **ID della soluzione necessaria** per la creazione di un'opportunità di co-selling?

Per creare un riferimento di co-selling, è necessaria una soluzione di co-selling per Microsoft. 

8. Cosa si deve fare quando vengono visualizzate opportunità di co-selling create in Partner Center che non vengono sincronizzate con CRM anche se non sono presenti errori di flusso:

Eseguire le operazioni seguenti:

- Dopo aver creato una nuova operazione di co-selling nel centro per i partner, verificare che venga richiamato il centro per i partner del flusso di Dynamics 365 (potrebbe essere richiamato più volte).

- Se il flusso viene richiamato, controllare tutti i flussi richiamati e identificare l'esecuzione del flusso che aggiornerà il CRM. È possibile seguire le azioni e verificare se il CRM è stato aggiornato o se si è verificato un problema.

- Controllare *New Deal** nel centro per i partner per verificare se viene popolato con l'ID CRM.

- Assicurarsi che l'operazione non sia chiusa accidentalmente come "Won" o "Lost" nel centro per i partner.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)
 
- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)