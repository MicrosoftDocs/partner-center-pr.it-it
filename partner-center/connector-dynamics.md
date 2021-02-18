---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizzare i riferimenti nel centro per i partner con il connettore di co-selling per Dynamics 365 CRM. I venditori possono quindi co-vendere con Microsoft dall'interno dei sistemi CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645771"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Co-selling Connector per Dynamics 365 CRM-Panoramica

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

Il connettore di co-selling del centro partner consente ai venditori di co-selling con Microsoft all'interno dei sistemi CRM. Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling. Usare i connettori di co-selling, per creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare/rifiutare i riferimenti, modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura. È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling. Per gestire tutti i riferimenti, è possibile usare il CRM preferito anziché il centro per i partner. 

La soluzione è basata sulla soluzione Microsoft Power automatizzate e usa le API del centro per i partner.

## <a name="before-you-install---pre-requisites"></a>Prima di installare-prerequisiti

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network |È necessario un ID MPN valido|Per aggiungere [MPN](https://partner.microsoft.com/)|
|Coselling pronto|La soluzione IP/servizi deve essere pronta per il co-selling.|[Vendi con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Account del Centro per i partner|L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling. Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|Il ruolo utente CRM è amministratore sistema o sistema verbi|[Assegnare i ruoli in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizzare l'account di flusso|Creazione di un nuovo ambiente di produzione con database per test/gestione temporanea e produzione. Se è presente un ambiente di produzione con database, può essere riutilizzato. L'utente che installa la soluzione connettore deve avere la licenza Power automatizzate e l'accesso a questo ambiente. È possibile monitorare lo stato di avanzamento e ottenere maggiori dettagli in caso di errore di installazione in [Power automatici](https://flow.microsoft.com/) facendo clic su Visualizza cronologia in soluzioni.|[Crea o Gestisci ambiente](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 (soluzione Power automatici)

1. Passare a [Power automatici](https://flow.microsoft.com) e selezionare **ambienti** nell'angolo superiore destro. In questo passaggio vengono visualizzate le istanze di CRM disponibili.

2. Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.

3. Selezionare **soluzioni** sulla barra di spostamento a sinistra.

4. Fare clic sul collegamento **Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Apri AppSource":::

5. Cercare i **connettori dei riferimenti del centro per i partner per Dynamics 365** nella schermata popup.  

6. Fai clic sul pulsante **Get it Now (Ottieni ora** ) e **continua**.

7. Verrà visualizzata la pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione.  Accettare i termini e le condizioni.

8. È possibile monitorare lo stato di avanzamento e ottenere maggiori dettagli in caso di errore di installazione in Power automatici facendo clic su **Visualizza cronologia** in **soluzioni**.
 

9. Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare **soluzioni** dall'area di spostamento a sinistra. Si noti che la **sincronizzazione dei riferimenti del centro per i partner per Dynamics 365** è disponibile nell'elenco soluzioni.

10. Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**. Sono disponibili i flussi e le entità seguenti per l'automazione dell'energia elettrica:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="DISPONGONO disponibili":::

## <a name="best-practice-test-before-you-go-live"></a>Procedura consigliata: testare prima di iniziare

Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging.

- Installare la soluzione Microsoft Power automatizzate in un ambiente di gestione temporanea o in un'istanza di CRM.
- Configurare e personalizzare la soluzione Microsoft Power automatizzate in ambiente di gestione temporanea.
- Testare la soluzione in un'istanza di staging/CRM. 
- In caso di esito positivo, importare come soluzione gestita nell'istanza di produzione. 

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).


2. Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.

3. È necessario creare connessioni che associano i tre account utente:

   - Utente del centro per i partner con credenziali di amministratore per i riferimenti

   - Eventi del Centro per i partner

   - L'amministratore di CRM con la funzionalità Power automatizza i flussi nella soluzione.

      1. Selezionare **Connections (connessioni** ) dalla barra di spostamento a sinistra e selezionare la soluzione "Partner Center referrals" dall'elenco.

      2. Creare una connessione facendo clic su **Crea una connessione**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Creare la connessione":::

      3. Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.

      4. Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.

      5. Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.

      6. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.
     
      7. Una volta aggiunte tutte le connessioni, nell'ambiente verranno visualizzate le connessioni seguenti:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Connessioni":::
   
## <a name="edit-the-connections"></a>Modificare le connessioni

1. Tornare alla pagina **soluzioni** e selezionare **soluzione predefinita**. Selezionare **riferimento alla connessione (anteprima)** facendo clic su **tutto**.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Connettere":::

2. Modificare ognuna delle connessioni una alla volta selezionando l'icona a tre punti. Aggiungere le connessioni pertinenti.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Connessioni elencate"::: 

3.  Tornare alla pagina soluzioni, selezionare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 e attivare il flusso facendo clic sull'icona a tre punti accanto a ogni flusso nella sequenza seguente. Se si verificano problemi durante l'attivazione del flusso, vedere la procedura di [personalizzazione](connector-dynamics.md#customize-synchronization-steps) e i passaggi per la [risoluzione dei problemi](connectors-troubleshoot.md). 

Attivare i flussi nella sequenza seguente:

- Registrazione webhook del centro per i partner (anteprima Insider)
- Creazione di un riferimento di co-selling: Dynamics 365 al centro per i partner (anteprima Insider)
- Personalizzare Crea o Ottieni dettagli da Dynamics 365 Flow 
- Da partner Center a Dynamics 365-Helper (insider Preview)
- Partner Center Microsoft co-selling degli aggiornamenti di riferimento a Dynamics 365 (insider Preview)
- Da partner Center a Dynamics 365 (insider Preview)
- Da Dynamics 365 al centro per i partner (anteprima Insider)
- Dynamics 365 opportunity to partner Center (insider Preview)
- Dynamics 365 Microsoft Solutions to partner Center (insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Usare le API webhook per registrare gli eventi di modifica delle risorse

Le API webhook del centro per i partner consentono di effettuare la registrazione per gli eventi di modifica delle risorse. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Selezionare **centro per i partner per Dynamics 365 (insider Preview)**.

2. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

3. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copia l'URL":::

4. Selezionare ora "registrazione del webhook del centro per i partner (anteprima di Insider)" Power automatizzare il flusso e selezionare **Esegui**.

5. Assicurarsi che la finestra "Esegui flusso" si apra nel riquadro di destra e fare clic su **continua**.

6. Immettere i dettagli seguenti:

   - **Endpoint trigger http**: URL copiato dal passaggio precedente

   - **Eventi da registrare**: selezionare tutti gli eventi disponibili ("creazione di un riferimento", "riferimento-aggiornato", "correlato-riferimento-creato", "correlato-riferimento-aggiornato")

   -**Sovrascrivi endpoint di trigger esistenti se presenti**: Sì è importante notare che è possibile registrare un solo URL per un determinato evento del webhook. È importante tenere presente che è possibile registrare un solo URL per un determinato evento del webhook. 

7. Selezionare **Esegui** , quindi fare clic su **fine.**

Il webhook ora può restare in ascolto per creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

I sistemi CRM sono altamente personalizzati ed è possibile personalizzare la soluzione Power automatizzate in base alla configurazione di CRM.  Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati nella [Guida al mapping dei campi personalizzati](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate in **[personalizzare] creare o ottenere i dettagli dalle variabili di ambiente o di flusso di Dynamics 365**  . Si consiglia di non aggiornare altri flussi nella soluzione Power automatizzate, perché può influire sugli aggiornamenti futuri della soluzione. 

Di seguito sono riportate le personalizzazioni disponibili:

- Segno di spunta in nome opportunità: per impostazione predefinita, viene visualizzato un segno di spunta accanto a nome opportunità per indicare che la sincronizzazione tra il centro per i partner e Dynamics 365 CRM è stata eseguita correttamente. Analogamente, se la sincronizzazione non riesce, verrà visualizzato un contrassegno incrociato. Per evitare l'aggiunta di un segno di spunta o di un contrassegno incrociato nel nome dell'opportunità, impostare il valore corrente del segno di spunta visualizzato nella variabile di ambiente nome opportunità su No

- Valore di Deal: per impostazione predefinita, il valore di Deal dal centro per i partner verrà sincronizzato da e verso **estimatedvalue** in CRM. Se è presente un campo diverso in CRM per il valore di Deal da sincronizzare:

    a.    Aggiornare il nome del campo del valore dell'affare nella variabile di ambiente Dynamics 365 con il nome del campo di CRM. Si noti che è necessario specificare il nome del campo non il nome visualizzato.

    b.    Modificare **[personalizzare] creare o ottenere dettagli da Dynamics 365 Flow**  e passare a **creare o aggiornare** l'opportunità in CRM e aggiornare **creare una nuova opportunità** e aggiornare le azioni di **opportunità esistenti** per assegnare il valore **DealValue** al campo corretto in CRM. Rimuovere anche l' **assegnazione DealValue** dal campo **stimato dei ricavi** .

- Codice paese dell'account del cliente: è obbligatorio fornire un codice paese di due lettere (ISO 3166) quando si crea un nuovo riferimento. Per impostazione predefinita, il codice paese verrà sincronizzato da e verso il campo address1_country dell'account in CRM. Se è presente un campo diverso in CRM per il codice paese da sincronizzare:

   a.    Per un campo di codice paese non di ricerca nell'account che contiene il codice di due lettere:

   - Aggiornare il nome del campo del codice paese dell'account del cliente nella variabile di ambiente Dynamics 365 con il nome del campo di CRM. Si noti che è necessario specificare il nome del campo non il nome visualizzato.

   - Modificare **[personalizzare] creare o ottenere dettagli da Dynamics 365 Flow**  e passare a creare o ottenere un account cliente in azione CRM per assegnare il valore del paese al campo corretto in CRM. Rimuovere anche assegnazione valore paese dal campo Indirizzo 1: paese/area geografica.

   b.    Per un campo di codice paese basato su ricerca nell'account:

   - Aggiungere un nuovo campo personalizzato nell'account e popolarlo automaticamente con codice paese di due lettere (ISO 3166) in base al valore selezionato nel campo basato su ricerca e viceversa.

   - Seguire i passaggi precedenti per il campo codice paese non di ricerca per sincronizzare il nuovo campo personalizzato da CRM a e dal centro per i partner.

- Campi delle opportunità: se sono presenti campi obbligatori in occasione che devono essere popolati, modificare **[Personalizza] creare o ottenere i dettagli da Dynamics 365 Flow**  e passare a **Crea o aggiorna opportunità** in CRM e aggiornare **Crea una nuova azione di opportunità** per assegnare i valori ai campi obbligatori in base ai requisiti aziendali.

- Campi principali: se sono presenti campi obbligatori in lead che devono essere popolati, modificare **[Personalizza] creare o ottenere dettagli da Dynamics 365 Flow**  e passare a **Crea o aggiorna lead** in CRM e aggiornare **Crea una nuova azione lead** per assegnare i valori ai campi obbligatori in base ai requisiti aziendali.

- Account cliente: quando un nuovo riferimento viene sincronizzato dal centro per i partner a CRM, la soluzione Power automatizzate tenta di cercare un account esistente in CRM usando il nome e il codice postale della società del cliente. Se non ne viene trovato uno, verrà creato un nuovo account cliente in CRM. Per aggiornare i criteri di ricerca e i nuovi dettagli di creazione dell'account, modificare **[Personalizza] creare o ottenere dettagli da Dynamics 365 Flow** e passare a **creare o ottenere l'account cliente** in CRM e **creare un'azione dell'account cliente**.

## <a name="update-environment-variable"></a>Aggiorna variabile di ambiente

Per aggiornare un valore della variabile di ambiente:

1. Passare alla pagina **soluzioni** e selezionare **soluzione predefinita**. Selezionare la **variabile di ambiente** facendo clic su tutto.

2. Selezionare la variabile di ambiente per il valore che deve essere aggiornato e fare clic su **modifica** utilizzando tre puntini di sospensione.

3. Aggiornare il valore **corrente** (non aggiornare il valore predefinito) utilizzando l'opzione **nuovo valore** e fornire il valore. Il valore deve corrispondere al tipo di dati della variabile, ad esempio Sì/nessun tipo di dati accetterà un valore Sì o no.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Casella di modifica per i valori predefiniti":::

- Sincronizzazione del riferimento bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 e centro per i partner.

### <a name="pre-requisites"></a>Prerequisiti

Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM, la soluzione Power automatizzate delimita chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione consente ai team dei venditori di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.

Un set di campi e oggetti personalizzati viene aggiunto come parte dell'installazione della soluzione. Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizza con il centro** per i partner: indica se sincronizzare l'opportunità con il centro per i partner Microsoft. Per impostazione predefinita, il valore di questo campo è no e deve essere impostato in modo esplicito su Sì dal venditore per condividere un'opportunità con Microsoft. Il valore del campo per i nuovi riferimenti condivisi dal centro per i partner a CRM è impostato su Sì.

- **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner Microsoft

- **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner Microsoft
- In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento. Per creare un riferimento di co-selling, selezionare la guida appropriata richiesta da Microsoft. Un contatto del cliente deve essere associato all'opportunità di creare un riferimento di co-selling. Per creare un riferimento non di co-selling lasciare questo campo non selezionato. Un riferimento non di co-selling può essere convertito in un riferimento di co-selling in qualsiasi momento selezionando l'opzione appropriata per la guida.

- **Visibilità del riferimento del centro per i partner Microsoft**: selezionare visibilità per il riferimento al centro per i partner Microsoft. Rendendolo visibile ai venditori Microsoft, un riferimento non di co-selling può essere convertito in co-selling. Quando è richiesta la Guida Microsoft, il riferimento è visibile ai venditori Microsoft per impostazione predefinita. Una volta contrassegnato come visibile, questo campo non può essere ripristinato.

- **Identificatore Microsoft CRM**: quando un riferimento di co-selling viene creato e accettato da Microsoft, questo campo viene popolato con l'identificatore CRM di Microsoft.

- **Prodotti: obsoleto** – non usare questo campo o aggiungerlo alla sezione CRM, è disponibile solo per la compatibilità con le versioni precedenti. Usare invece le soluzioni del centro per i partner Microsoft.

- **Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner

- **Soluzioni del centro per i partner Microsoft**: oggetto personalizzato per associare soluzioni di co-selling pronte o soluzioni Microsoft con la possibilità. È possibile aggiungere e/o rimuovere una o più soluzioni dall'opportunità. È obbligatorio aggiungere almeno una soluzione di co-selling pronta o Microsoft alla possibilità prima di condividerla con Microsoft. Per associare questo oggetto all'opportunità, aggiornare il modulo chance in CRM:

  Selezionare la scheda appropriata nel modulo opportunità e aggiungere una griglia secondaria, come illustrato di seguito:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Modulo opportunità":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Dopo aver aggiunto le soluzioni Microsoft, è possibile pre-popolare i dettagli delle soluzioni pronte per la co-selling, in modo che i venditori non debbano aggiungerli. Per aggiungere un nuovo dettaglio della soluzione, passare all'oggetto dettagli della soluzione Microsoft in CRM e fare clic su **Aggiungi record** per aggiungere una voce o usare il **caricamento di Excel** per aggiungere più voci.

:::image type="content" source="images/dynamic-1a.png" alt-text="Dettagli della soluzione":::

### <a name="scenarios"></a>SCENARI

1. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:

   1. Accedere al proprio ambiente di Dynamics 365 CRM con un utente che abbia visibilità nella sezione **opportunità** del CRM.

   2. Assicurarsi che la sezione centro per i partner Microsoft sia presente quando si crea una "nuova opportunità" nell'ambiente Dynamics 365

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nuova opportunità"::: 

   3. Per sincronizzare questa opportunità con il centro per i partner, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Come può essere utile Microsoft?**: per creare un riferimento di co-selling selezionare un'opzione di guida appropriata.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Come ottenere i campi appropriati nella visualizzazione scheda":::

      - **Contatto del cliente**: per creare un riferimento di co-selling, aggiungere un contatto del cliente all'opportunità.
      - **Sincronizza con il centro per i partner**: Sì

      - Microsoft Solutions: per condividere un riferimento con Microsoft, è possibile aggiungere una valida soluzione di co-selling o una soluzione Microsoft alle opportunità.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="ID soluzione":::

   4. Dopo aver creato l'opportunità in Dynamics 365 con l'opzione sync with partner Center impostata su Sì, attendere 10 minuti e quindi accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Dynamics 365 e l'identificatore del riferimento. Il collegamento di riferimento viene popolato. In caso di errore, il campo audit verrà popolato con le informazioni sull'errore.
     
    5. Analogamente, per un'opportunità con l'opzione "Sync with partner Center" impostata su "Yes", se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.

    6. Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.

2. Sincronizzazione del riferimento quando il riferimento viene creato o aggiornato nel centro per i partner Microsoft e sincronizzato nell'ambiente Dynamics 365:

   1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

   2. Selezionare **riferimenti** dal menu a sinistra.

   3. Creare un nuovo riferimento di co-selling dal centro per i partner selezionando l'opzione  **New Deal** .

   4. Accedere al proprio ambiente Dynamics 365 CRM.

   5. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner Microsoft è ora sincronizzato in Dynamics 365 CRM.

   6. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)

- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)

- [Altre informazioni sulla piattaforma Microsoft Power automatizzate?](/power-automate/)

- [Webhook del Centro per i partner](/partner-center/develop/partner-center-webhooks)