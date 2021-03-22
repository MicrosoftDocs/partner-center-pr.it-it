---
title: Connettore di co-selling per Dynamics 365 CRM Partner Center
description: Sincronizzare i riferimenti nel centro per i partner con il connettore di co-selling per Dynamics 365 CRM. È quindi possibile eseguire la co-selling con Microsoft dall'interno del sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768772"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Panoramica di co-selling Connector per Dynamics 365 CRM

### <a name="appropriate-roles"></a>Ruoli appropriati

- Amministratore delle segnalazioni
- Amministratore di sistema o verbi di sistema in CRM

I connettori di co-selling del centro partner consentono ai venditori di co-selling con Microsoft all'interno dei sistemi CRM. Non dovranno essere sottoposti a training per usare il centro per i partner per gestire le offerte di co-selling. Usare i connettori di co-selling per creare un nuovo riferimento di co-selling per coinvolgere un venditore Microsoft, ricevere riferimenti da Microsoft seller, accettare o rifiutare i riferimenti e modificare i dati dell'affare, ad esempio il valore dell'offerta e la data di chiusura. È anche possibile ricevere eventuali aggiornamenti dai venditori Microsoft per le offerte di co-selling. Per gestire tutti i riferimenti, è possibile usare il CRM preferito anziché il centro per i partner.

La soluzione si basa su Power automatici e usa le API del centro per i partner.

## <a name="prerequisites"></a>Prerequisiti

Prima di installare la soluzione, assicurarsi di soddisfare i prerequisiti seguenti.

|**Argomenti**   |**Dettagli**   |**Collegamenti**   |
|--------------|--------------------|------|
|ID Microsoft Partner Network (MPN) |È necessario un ID MPN valido.|[Unisciti alla rete partner](https://partner.microsoft.com/)|
|Co-selling pronto|La soluzione IP/servizi deve essere pronta per il co-selling.|[Vendi con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Account del Centro per i partner|L'ID MPN associato al tenant del centro per i partner deve corrispondere all'ID MPN associato alla soluzione di co-selling. Prima di distribuire i connettori, verificare che sia possibile visualizzare i riferimenti di co-selling nel portale del centro per i partner.|[Gestire l'account](create-user-accounts-and-set-permissions.md)|
|Ruoli utente del Centro per i partner|Il dipendente che installerà e userà i connettori deve essere un amministratore dei riferimenti.|[Assegnare autorizzazioni e ruoli utente](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|Il ruolo utente CRM è amministratore sistema o verbi di sistema.|[Assegnare i ruoli in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power automatizzare l'account di flusso|Creazione di un nuovo ambiente di produzione con un database per test, gestione temporanea e produzione. Se è presente un ambiente di produzione con un database, è possibile riutilizzarlo. L'utente che installa la soluzione Connector deve disporre di una licenza Power automatizzate e di accesso a questo ambiente. Se l'installazione ha esito negativo, è possibile monitorare lo stato di avanzamento e ottenere altre informazioni in [Power automatizzate](https://flow.microsoft.com/) . Selezionare **Visualizza cronologia** in **soluzioni**.|[Crea o Gestisci ambiente](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Installare la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365 (soluzione Power automatici)

1. Passare a [Power automatici](https://flow.microsoft.com)e selezionare **ambienti** nell'angolo superiore destro. In questo passaggio vengono visualizzate le istanze di CRM disponibili.

1. Selezionare l'istanza di CRM appropriata dall'elenco a discesa nell'angolo in alto a destra.

1. Selezionare **Solutions (soluzioni** ) a sinistra.

1. Selezionare il collegamento **Apri AppSource** nel menu in alto.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Screenshot che mostra AppSource aperto.":::

1. Cercare i **connettori dei riferimenti del centro per i partner per Dynamics 365** nella schermata popup.  

1. Selezionare il pulsante **Get it now** , quindi selezionare **continue (continua**).

1. Viene visualizzata una pagina in cui è possibile selezionare l'ambiente CRM (Dynamics 365) per installare l'applicazione. Accettare i termini e le condizioni.

1. È possibile monitorare lo stato di avanzamento e, in caso di errore dell'installazione, è possibile ottenere altri dettagli in Power automatizzate selezionando **Visualizza cronologia** in **soluzioni**.

1. Al termine dell'installazione, tornare a [Power automatizzate](https://flow.microsoft.com) e selezionare Solutions ( **soluzioni** ) a sinistra. La **sincronizzazione dei riferimenti del centro per i partner per Dynamics 365** è ora disponibile nell'elenco **soluzioni** .

1. Selezionare **la sincronizzazione dei riferimenti del centro per i partner per Dynamics 365**. Sono disponibili i flussi e le entità di Power automatizzazione seguenti.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Screenshot che mostra dispongono disponibili.":::

## <a name="test-before-you-go-live"></a>Esegui test prima di iniziare

Prima di installare, configurare e personalizzare la soluzione Power automatizzate nell'ambiente di produzione, assicurarsi di testare la soluzione in un'istanza di CRM di staging. È necessario:

- Installare la soluzione Power automatizzate in un'istanza di CRM dell'ambiente di staging.
- Configurare e personalizzare la soluzione Power automatizzate in un ambiente di gestione temporanea.
- Testare la soluzione in un'istanza di CRM di staging.
- Dopo un test riuscito, importare come soluzione gestita nell'istanza di produzione.

## <a name="configure-the-solution"></a>Configurare la soluzione

1. Dopo aver installato la soluzione nell'istanza di CRM, tornare a [Power automatizzate](https://flow.microsoft.com/).

1. Dall'elenco a discesa **ambienti** nell'angolo superiore destro selezionare l'istanza di CRM in cui è stata installata la soluzione Power automatizzate.

1. È necessario creare connessioni che associano i tre account utente:

   - Utente del centro per i partner con credenziali di amministratore per i riferimenti
   - Eventi del Centro per i partner
   - Amministratore CRM con i flussi di automazione dell'alimentazione nella soluzione

   1. Selezionare **Connections (connessioni** ) a sinistra e selezionare la soluzione centro per i partner per i **riferimenti** dall'elenco.

   1. Creare una connessione selezionando **Crea una connessione**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Screenshot che mostra la creazione di una connessione.":::

   1. Cercare i riferimenti per il centro per i **partner (anteprima)** nella barra di ricerca nell'angolo superiore destro.

   1. Creare una connessione per l'utente del centro per i partner con il ruolo delle credenziali di amministratore dei riferimenti.

   1. Successivamente, creare una connessione per gli eventi del centro partner per l'utente del centro per i partner con le credenziali di amministratore dei riferimenti.

   1. Creare una connessione per Common Data Service (ambiente corrente) per l'utente amministratore CRM.
     
   1. Dopo aver aggiunto tutte le connessioni, nell'ambiente verranno visualizzate le connessioni seguenti.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Screenshot che mostra le connessioni.":::

## <a name="edit-the-connections"></a>Modificare le connessioni

1. Tornare alla pagina **soluzioni** e selezionare **soluzione predefinita**. Selezionare **riferimento alla connessione (anteprima)** selezionando **tutti**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Screenshot che mostra la modifica delle connessioni.":::

1. Modificare ognuna delle connessioni una alla volta selezionando l'icona con i puntini di sospensione. Aggiungere le connessioni pertinenti.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Screenshot che mostra le connessioni elencate.":::

1.  Tornare alla pagina **soluzioni** , selezionare la **sincronizzazione dei riferimenti del centro per i Partner per Dynamics 365** e attivare il flusso selezionando l'icona con i puntini di sospensione accanto a ogni flusso nella sequenza seguente. Se si verificano problemi durante l'attivazione del flusso, vedere procedure di [personalizzazione](connector-dynamics.md#customize-synchronization-steps) e procedure per la [risoluzione dei problemi](connectors-troubleshoot.md).

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

Per registrare gli eventi di modifica delle risorse, è possibile usare le API webhook del centro per i partner. Questi eventi di modifica vengono inviati all'URL come post HTTP.

1. Selezionare **centro per i partner per Dynamics 365 (insider Preview)**.

1. Selezionare l'icona di **modifica** e selezionare **quando viene ricevuta una richiesta http**.

1. Selezionare l'icona **copia** per copiare l'URL post HTTP specificato.

   :::image type="content" source="images/webhook-video.gif" alt-text="Screenshot che Mostra come usare i webhook per registrare le modifiche alle risorse.":::

1. Selezionare il flusso di **registrazione del webhook del centro per i partner (anteprima di insider Preview)** , quindi selezionare **Esegui**.

1. Assicurarsi che la finestra **Esegui flusso venga** visualizzata nel riquadro destro e selezionare **continua**.

1. Immettere i dettagli seguenti:

   - **Endpoint trigger http**: questo URL è stato copiato da un passaggio precedente.
   - **Eventi da registrare**: selezionare tutti gli eventi disponibili, ovvero **creazione** di un riferimento, **riferimento-aggiornato**, **correlato-riferimento-creato** e **correlato-riferimento-aggiornato**.
   - **Sovrascrivi gli endpoint del trigger esistenti se presenti?**: Sì. È possibile registrare un solo URL per un determinato evento del webhook.

1. Selezionare **Esegui flusso**, quindi fare clic su **fine.**

Il webhook può ora ascoltare, creare e aggiornare gli eventi.

## <a name="customize-synchronization-steps"></a>Personalizzare i passaggi di sincronizzazione

I sistemi CRM sono altamente personalizzati ed è possibile personalizzare la soluzione Power automatizzate in base alla configurazione di CRM. Quando i riferimenti di co-selling sono sincronizzati tra il centro per i partner e il sistema CRM, i campi sincronizzati nel PC del centro per i partner sono elencati nella [Guida al mapping dei campi personalizzati](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Seguire la guida al mapping dei campi e, se necessario, apportare le modifiche appropriate in **[personalizzare] creare o ottenere i dettagli dalle variabili di ambiente o di flusso di Dynamics 365** . Non aggiornare altri flussi nella soluzione Power automatizzate perché può influenzare gli aggiornamenti futuri della soluzione.

Sono disponibili le seguenti personalizzazioni:

- **Visualizza il segno di spunta nel nome dell'opportunità**: per impostazione predefinita, viene visualizzato un segno di spunta accanto al nome dell'opportunità per indicare che la sincronizzazione tra il centro per i partner e Dynamics 365 CRM è stata eseguita correttamente. Analogamente, se la sincronizzazione non riesce, verrà visualizzato un contrassegno incrociato. Per evitare di aggiungere un segno di spunta o un segno incrociato nel nome dell'opportunità, impostare il valore corrente del **segno di spunta visualizzato nella** variabile di ambiente nome opportunità su No.
- **Valore di Deal**: per impostazione predefinita, il valore dell'affare da partner Center verrà sincronizzato da e verso **estimatedvalue** nel CRM. Se si dispone di un campo diverso in CRM per il valore di Deal da sincronizzare:

  - Aggiornare il nome del campo del **valore dell'affare** nella variabile di ambiente Dynamics 365 con il nome del campo di CRM. Assicurarsi di specificare il nome del campo, non il nome visualizzato.
  - Modificare **[personalizzare] creare o ottenere dettagli da Dynamics 365 Flow** e passare a **Crea o aggiorna opportunità** in CRM e aggiornare **creare una nuova opportunità** e aggiornare le azioni di **opportunità esistenti** per assegnare il valore **DealValue** al campo corretto nel CRM. Rimuovere anche l'assegnazione **DealValue** dal campo dei **ricavi stimati** .

- **Codice paese dell'account del cliente**: è obbligatorio fornire un codice paese di due lettere (ISO 3166) quando si crea un nuovo riferimento. Per impostazione predefinita, il codice paese verrà sincronizzato da e verso il campo **address1_country** dell'account nel CRM. Se nel CRM è presente un campo diverso per il codice paese da sincronizzare:

   - Per un campo di codice paese non di ricerca nell'account che contiene un codice di due lettere:
     - Aggiornare il nome del campo del **codice paese dell'account del cliente** nella variabile di ambiente Dynamics 365 con il nome del campo di CRM. Assicurarsi di specificare il nome del campo, non il nome visualizzato.
     - Modificare **[personalizzare] creare o ottenere i dettagli da Dynamics 365 Flow** e passare a **Crea o ottenere un account cliente** nell'azione CRM per assegnare un valore di **paese** al campo corretto nel CRM. Rimuovere anche l'assegnazione del valore del **paese** dal campo **Indirizzo 1: paese/area geografica** .

   - Per un campo di codice paese basato su ricerca nell'account:
     - Aggiungere un nuovo campo personalizzato nell'account e popolarlo automaticamente con un codice paese di due lettere (ISO 3166) in base al valore selezionato nel campo basato sulla ricerca e viceversa.
     - Attenersi ai passaggi precedenti per il campo codice paese non di ricerca per sincronizzare un nuovo campo personalizzato da CRM a e dal centro per i partner.

- **Campi delle opportunità**: se sono presenti campi obbligatori **che devono** essere popolati, modificare **[Personalizza] creare o ottenere i dettagli da Dynamics 365 Flow** e passare a **Crea o aggiorna opportunità** nell'azione CRM e aggiorna **Crea una nuova opportunità** per assegnare i valori ai campi obbligatori in base ai requisiti aziendali.
- **Campi principali**: se sono presenti campi obbligatori in **Lead** che devono essere popolati, modificare **[Personalizza] creare o ottenere i dettagli da Dynamics 365 Flow** e passare a **Crea o aggiorna lead** in CRM e aggiornare **Crea una nuova azione lead** per assegnare i valori ai campi obbligatori in base ai requisiti aziendali.
- **Account cliente**: quando un nuovo riferimento viene sincronizzato dal centro per i partner al CRM, la soluzione Power automatizzate tenta di cercare un account esistente nel CRM usando il nome e il codice postale della società del cliente. Se non ne viene trovato uno, verrà creato un nuovo account cliente nel CRM. Per aggiornare i criteri di ricerca e i nuovi dettagli di creazione dell'account, modificare **[Personalizza] crea o Ottieni dettagli da Dynamics 365 Flow** e passare a **Crea o Ottieni account cliente** nell'azione CRM e **Crea account cliente**.

## <a name="update-environment-variable"></a>Aggiorna variabile di ambiente

Per aggiornare un valore della variabile di ambiente:

1. Passare alla pagina **soluzioni** e selezionare **soluzione predefinita**. Selezionare la **variabile di ambiente** selezionando **tutti**.

1. Selezionare la variabile di ambiente per il valore che deve essere aggiornato e selezionare **modifica** utilizzando l'icona con i puntini di sospensione.

1. Aggiornare il valore **corrente** (non aggiornare il **valore predefinito**) utilizzando l'opzione **nuovo valore** e specificando il valore. Il valore deve corrispondere al tipo di dati della variabile. Il tipo di dati Yes o no, ad esempio, accetterà il valore Yes o no.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Screenshot che mostra le variabili ambientali dell'aggiornamento.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronizzazione del riferimento bidirezionale end-to-end

Dopo aver installato, configurato e personalizzato la soluzione Power automatizzate, è possibile testare la sincronizzazione dei riferimenti di co-selling tra Dynamics 365 e centro per i partner.

### <a name="prerequisites"></a>Prerequisiti

Per sincronizzare i riferimenti tra il centro per i partner e Dynamics 365 CRM, la soluzione Power automatizzate delimita chiaramente i campi di riferimento specifici di Microsoft. Questa identificazione consente ai team dei venditori di decidere quali riferimenti desidera condividere con Microsoft per la co-selling.

Come parte dell'installazione della soluzione verrà aggiunto un set di campi e oggetti personalizzati. Un utente amministratore CRM dovrà creare una sezione CRM separata con i campi personalizzati **opportunity** .

I campi personalizzati seguenti devono far parte della sezione CRM:

- **Sincronizzare con il centro** per i partner: se sincronizzare l'opportunità con il centro per i partner. Per impostazione predefinita, il valore di questo campo è no e deve essere impostato in modo esplicito su Sì dal venditore per condividere un'opportunità con Microsoft. Il valore del campo per i nuovi riferimenti condivisi dal centro per i partner a CRM è impostato su Sì.
- **Identificatore del riferimento**: campo dell'identificatore di sola lettura per il riferimento al centro per i partner.
- **Collegamento di riferimento**: un collegamento di sola lettura al riferimento nel centro per i partner.
- In **che modo può essere utile Microsoft?**: guida richiesta da Microsoft per il riferimento. Per creare un riferimento di co-selling, selezionare la guida appropriata richiesta da Microsoft. Un contatto del cliente deve essere associato all'opportunità di creare un riferimento di co-selling. Per creare un riferimento non di co-selling, non selezionare questo campo. Un riferimento non di co-selling può essere convertito in un riferimento di co-selling in qualsiasi momento selezionando l'opzione appropriata per la guida.
- **Visibilità del riferimento del centro per i partner Microsoft**: selezionare visibilità per il riferimento al centro per i partner. Rendendolo visibile ai venditori Microsoft, un riferimento non di co-Selling potrebbe essere convertito in co-selling. Quando è richiesta la Guida Microsoft, il riferimento è visibile ai venditori Microsoft per impostazione predefinita. Quando questo campo è contrassegnato come visibile, non può essere ripristinato.
- **Identificatore Microsoft CRM**: quando un riferimento di co-selling viene creato e accettato da Microsoft, questo campo viene popolato con l'identificatore CRM di Microsoft.
- **Prodotti: obsoleto**: non usare questo campo o aggiungerlo alla sezione CRM. È disponibile solo per compatibilità con le versioni precedenti. Usare invece le soluzioni del centro per i partner.
- **Audit**: audit trail di sola lettura per la sincronizzazione con i riferimenti del centro per i partner.
- **Soluzioni del centro per i partner Microsoft**: oggetto personalizzato per associare soluzioni di co-selling pronte o soluzioni Microsoft con la possibilità. Una o più soluzioni possono essere aggiunte o rimosse dall'opportunità. È obbligatorio aggiungere almeno una soluzione di co-selling pronta o Microsoft alla possibilità prima di condividerla con Microsoft. Per associare questo oggetto alla possibilità, aggiornare il modulo **opportunity** nel CRM.

  Selezionare la scheda appropriata nel modulo **opportunità** e aggiungere una sottogriglia come illustrato di seguito.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Screenshot che mostra il modulo di opportunità.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Screenshot che mostra le soluzioni Microsoft.":::

- Dopo aver aggiunto le soluzioni Microsoft, è possibile prepopolare i dettagli della soluzione di co-selling pronto, in modo che i venditori non debbano aggiungerli. Per aggiungere un nuovo dettaglio della soluzione, passare all'oggetto dettagli della soluzione Microsoft in CRM e selezionare **Aggiungi record** per aggiungere una voce o usare il **caricamento di Excel** per aggiungere più voci.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Screenshot che mostra i dettagli della nuova soluzione Microsoft.":::

### <a name="scenarios"></a>Scenari

1. Sincronizzazione dei riferimenti quando il riferimento viene creato o aggiornato in CRM e sincronizzato nel centro per i partner:

   1. Accedere all'ambiente di Dynamics 365 CRM con l'utente che ha visibilità nella sezione relativa alle **opportunità** del CRM.

   1. Assicurarsi che la sezione centro per i **partner Microsoft** sia presente quando si crea una nuova opportunità nell'ambiente Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Screenshot che mostra una nuova opportunità.":::

   1. Per sincronizzare questa opportunità con il centro per i partner, assicurarsi di impostare i campi seguenti nella visualizzazione scheda:

      - **Come è possibile fare per Microsoft?**: per creare un riferimento di co-selling, selezionare un'opzione appropriata per la guida.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Screenshot che Mostra come ottenere i campi appropriati nella visualizzazione scheda.":::

      - **Contatto del cliente**: per creare un riferimento di co-selling, aggiungere un contatto del cliente all'opportunità.
      - **Sincronizza con il centro per i partner**: Sì.
      - **Microsoft Solutions**: per condividere un riferimento con Microsoft, è possibile aggiungere una soluzione di co-selling pronta o Microsoft valida alla possibilità.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Screenshot che mostra l'ID della soluzione.":::

   1. Dopo la creazione dell'opportunità in Dynamics 365 con l'opzione **Sync with partner Center** impostata su Yes, attendere 10 minuti. Quindi accedere all'account del centro per i partner. I riferimenti verranno sincronizzati con Dynamics 365 e l' **identificatore del riferimento**. Il **collegamento di riferimento** viene popolato. Se si verifica un errore, il campo **Audit** verrà popolato con le informazioni sull'errore.
     
    1. Analogamente, per un'opportunità per cui l'opzione **Sincronizza con partner Center** è impostata su Sì, se si aggiorna l'opportunità in Dynamics 365 CRM, le modifiche verranno sincronizzate nell'account del centro per i partner.

    1. Le opportunità sincronizzate con il centro per i partner verranno identificate con ✔ icona in Dynamics 365.

1. Sincronizzazione dei riferimenti quando il riferimento viene creato o aggiornato nel centro per i partner e sincronizzato nell'ambiente Dynamics 365:

   1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home)del centro per i partner.

   1. Selezionare **riferimenti** dal menu a sinistra.

   1. Creare un nuovo riferimento di co-selling dal centro per i partner selezionando l'opzione **New Deal** .

   1. Accedere all'ambiente di Dynamics 365 CRM.

   1. Passare a **Open Opportunities**. Il riferimento creato nel centro per i partner è ora sincronizzato in Dynamics 365 CRM.

   1. Quando si seleziona un riferimento sincronizzato, i dettagli della visualizzazione della scheda vengono popolati.

## <a name="next-steps"></a>Passaggi successivi

- [Gestire lead](manage-leads.md)
- [Gestire opportunità di co-selling](manage-co-sell-opportunities.md)
- [Altre informazioni su Microsoft Power automatizzate Platform](/power-automate/)
- [Webhook del Centro per i partner](/partner-center/develop/partner-center-webhooks)
