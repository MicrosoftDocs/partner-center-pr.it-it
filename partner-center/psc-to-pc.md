---
title: Eseguire la migrazione da partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri in che modo i partner Microsoft possono eseguire la migrazione da partner Sales Connect (PSC) al centro per i partner e creare o gestire le offerte inviate dai venditori Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: f84ceb4d17be7e02a4380e4da55d7ac199f43515
ms.sourcegitcommit: 2a3fe71ef30fbda25cc70f8f526b3efd2b3df687
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/05/2021
ms.locfileid: "99588751"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guida alla co-selling nel centro per i partner (PC) per i partner che eseguono la migrazione da partner Sales Connect (PSC)

**Ruoli appropriati**

- Amministratore degli account
- Amministratore delle segnalazioni
- Venditore partner Sales Connect (PSC)
- Amministratore di partner Sales Connect (PSC)
- Partner Sales Connect (PSC) Deal Manager

Questo articolo fornisce indicazioni per i partner che eseguono la migrazione da partner Sales Connect to partner Center, in modo che possano continuare a creare e gestire le offerte di co-selling nel centro per i partner.

Come è noto, l'azienda perderà l'accesso a PSC dopo il 31 marzo 2021. Tuttavia, si troverà comunque tutto ciò che si desidera eseguire nel centro per i partner, ad esempio creare offerte di co-selling, gestire le offerte e agire sulle offerte inviate dai venditori Microsoft.

Tuttavia, vi sono differenze. Le linee guida seguenti consentono di eseguire la transizione al centro per i partner più agevole e più semplice.

>[!Important]
> Se ci si trova nel punto in cui è stato visualizzato un banner in PSC sulla migrazione, l'utente si trova nel posto giusto. Questa guida non è applicabile per la valutazione della soluzione (SA) e i partner di Internet degli altri OEM che gestiscono le proprie offerte in CPS.

## <a name="before-you-move-things-you-need-to-know"></a>Prima di procedere, è necessario sapere

### <a name="if-you-are-a-psc-admin"></a>Se si è un amministratore di PSC

- Per accedere al centro per i [partner](https://partner.microsoft.com/), è necessario un indirizzo di posta elettronica di lavoro.
- Configurare l'account con il supporto dell' [amministratore dell'account](permissions-overview.md)del centro per i partner.
- Leggere questo documento per informazioni su come co-selling nel centro per i partner.
- Configurare gli account utente nel centro per i partner per tutti gli utenti di PSC (amministratore, Deal Manager e ruoli venditore) e assegnare loro i [ruoli di amministratore di riferimento](permissions-overview.md).

>[!IMPORTANT]
> Verificare che l'ID MPN visualizzato nel banner del CPS sia disponibile nell'elenco di percorsi MPN nel centro per i partner.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Immagine che mostra il banner del CPS in cui i partner possono trovare l'ID MPN.":::

 Per verificare che l'ID MPN sia visualizzato come percorso MPN del centro per i partner, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **Impostazioni** (icona a forma di ingranaggio) in alto a destra nella schermata, seguito da **Impostazioni account**. Nel menu di spostamento a sinistra di secondo livello selezionare **locations (percorsi** ) per visualizzare l'elenco di tutti gli ID MPN e le posizioni associate all'account del centro per i partner.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se si è un rivenditore o un venditore di gestione delle offerte di PSC

- Per accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, è necessario un indirizzo di posta elettronica di lavoro.
- Se si usa un account non di lavoro in CPS o l'indirizzo di posta elettronica aziendale è per una società diversa da quella del partner, contattare l'amministratore del CPS per la guida per la configurazione dell'account.
- Rivolgersi all'amministratore di PSC se la configurazione dell'account del centro per i partner è completa indipendentemente dall'account usato per accedere a CPS.
- Verificare se è possibile accedere al centro per i partner e alla sezione dei riferimenti.
- Leggere questo documento per comprendere i flussi di lavoro e le modifiche apportate al centro per i partner.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Come amministratore in PSC, questi sono i passaggi successivi

Dal menu di spostamento a sinistra del centro per i partner selezionare l'opzione **riferimenti** . Verificare che sia possibile accedere alle pagine dei riferimenti.

  >[!Note]
  > Potrebbe essere necessario disconnettersi dal centro per i partner e accedere di nuovo per aggiornare le credenziali per l'accesso alle pagine dei riferimenti.

Se non viene visualizzata l'opzione **riferimenti** nel menu del centro per i partner o nelle pagine correlate ai riferimenti, contattare l' [amministratore dell'account](permissions-overview.md) aziendale e chiedere di concedere l'accesso all'opzione relativa ai **riferimenti** e all'area correlata.

Per trovare l'amministratore dell'account aziendale:

1. Selezionare **Impostazioni account** dall'icona a forma di ingranaggio nella parte superiore destra del dashboard del centro per i partner.

1. Selezionare **Gestione utenti** dal menu di spostamento a sinistra di secondo livello.

1. Nella parte superiore dell'elenco utenti selezionare il menu a discesa **filtro** . Modificare l'opzione di **amministratore account**.

   La pagina visualizzerà tutti gli amministratori dell'account con i rispettivi indirizzi di posta elettronica. Inviare un messaggio di posta elettronica a uno di essi e chiedere di assegnare il ruolo di amministratore dei riferimenti per l'account aziendale.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Immagine che Mostra gli amministratori dell'account nella pagina Gestione utenti delle impostazioni partner.":::

>[!Important]
>- Se il ruolo prevede solo la gestione degli utenti in CPS, richiedere all'amministratore dell'account aziendale di assegnare il ruolo di [amministratore dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) nel centro per i partner. 
>- Se il ruolo include anche la gestione delle opportunità di co-selling, richiedere l'assegnazione del ruolo di [amministratore dei riferimenti](permissions-overview.md#manage-referrals) .
> - È consigliabile anche designare un responsabile della gestione delle modifiche tra gli amministratori del CPS. In tal modo si impedirà a tutti gli amministratori del CPS di dover contattare singolarmente gli amministratori dell'account del centro per i partner. Al contrario, il responsabile della gestione delle modifiche può essere la persona principale che lavora con l'amministratore dell'account del centro per i partner.

## <a name="user-migration"></a>Migrazione degli utenti

Dopo aver configurato l'account nel centro per i partner, usare la migrazione guidata utenti nella pagina opportunità di co-selling per assegnare automaticamente i ruoli del centro partner ai dipendenti della società.

>[!Note]
> La migrazione degli utenti può essere eseguita solo dagli [amministratori dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) della società. Se non si ha il ruolo di amministratore dell'account, trovare un amministratore dell'account che consenta di configurare gli account utente con la guida della migrazione guidata utenti. La funzionalità di migrazione utente sarà disponibile a partire dal 18 novembre 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Immagine che mostra la migrazione guidata utenti.":::

Gli amministratori dell'account visualizzeranno un collegamento della migrazione guidata utenti di PSC nella pagina di co-selling Opportunities accanto alla guida dei riferimenti. È possibile avviare la migrazione degli utenti selezionando il collegamento. Per avviare la migrazione degli utenti, gli amministratori possono selezionare il collegamento. Questi passaggi possono essere eseguiti più volte fino a quando a tutti gli utenti non vengono assegnati ruoli appropriati nel centro per i partner.

La tabella di migrazione utente presenta i dettagli seguenti:

- Account utente-ID di posta elettronica del dipendente
- Account partner PSC: l'account a cui è associato il dipendente in PSC
- Ruolo utente PSC: uno dei tre ruoli assegnati a in CPS.
- Percorso MPN del PC: il percorso a cui l'utente riceverà i ruoli del PC pertinenti. L'account partner PSC viene usato per trovare la posizione MPN equivalente nel centro per i partner per l'assegnazione delle autorizzazioni. L'intera organizzazione indica l'ID MPN di vOrg.
- Ruolo utente PC: ai dipendenti vengono assegnati ruoli in base ai rispettivi ruoli utente del CPS. All'amministratore in PSC verranno assegnati i ruoli di amministratore dei riferimenti in PC. Al venditore verrà assegnato il ruolo utente riferimenti in PC. Scopri di più sui ruoli del PC e sui vantaggi che gli utenti con questi ruoli possono eseguire [nel centro per](permissions-overview.md#manage-referrals) i partner
- Tenant di AAD per PC: il tenant a cui gli utenti sono assegnati nel centro per i partner
- Stato: esistono tre possibili stati per lo stato della migrazione
    - **Non migrato** -l'utente non ha un ruolo di riferimento per i PC assegnati
    - **Migrated** : l'utente è stato migrato correttamente con il ruolo pertinente assegnato, come illustrato nella tabella
    - **Errore** -non è possibile completare la migrazione a causa di un errore

In alcuni casi, la migrazione può avere esito negativo e causare errori. Ecco alcuni motivi per cui una migrazione può causare un errore e alcune delle modalità di risoluzione del problema:

1. È possibile che gli utenti del CPS stiano usando un account non di lavoro.

2. È possibile che l'utente PSC usi un account di un dominio diverso da quello usato nel centro per i partner.

   Per risolvere gli errori correlati agli scenari 1 e 2, richiedere all'utente di accedere al centro per i partner usando il proprio account di lavoro collegato al tenant di Azure AD. L' [amministratore globale](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) può essere di aiuto.
   
   Per trovare l'amministratore globale: 
   - Accedere al [Dashboard](https://partner.microsoft.com/dashboard) del centro per i partner e selezionare **Impostazioni account** dall'icona a forma di ingranaggio in alto a destra.
   - Selezionare **Gestione utenti** nella barra di spostamento a sinistra di secondo livello.
   - Nella parte superiore dell'elenco utenti selezionare il menu a discesa **filtro** e impostare l'opzione su **amministratore globale**. La pagina Visualizza quindi tutti gli amministratori globali con i rispettivi indirizzi di posta elettronica. Chiedere a uno di loro di assegnare il ruolo di amministratore di riferimento per l'account aziendale.
   
      L'amministratore globale può creare un nuovo account utente nel tenant di Azure AD o assegnare l'accesso utente Guest agli altri utenti dell'account di dominio. Una volta configurati gli account per tutti gli utenti e i responsabili delle operazioni di PSC, è necessario accedere al centro per i partner, selezionare **riferimenti** dal menu di spostamento a sinistra e verificare che possano visualizzare la pagina dei riferimenti.

3. All'utente è già assegnato un ruolo di riferimento nel centro per i partner.
    - È possibile verificare il ruolo dell'utente esistente. Nell'angolo in alto a destra del centro per i partner selezionare **Impostazioni** (icona a forma di ingranaggio), quindi **Impostazioni account**. Quando viene visualizzato un secondo menu di spostamento a sinistra, selezionare **Gestione utenti** e cercare l'utente.

## <a name="psc-deals-migration"></a>Migrazione delle offerte di PSC

Dopo aver completato la migrazione degli utenti, usare la migrazione guidata delle offerte nella pagina opportunità di co-selling per riunire tutte le offerte di apertura idonee da CPS a PC. **Il collegamento per la migrazione delle offerte sarà visibile solo agli amministratori di riferimento con l'ambito completo dell'organizzazione nel centro per i partner.** Nella parte superiore destra della pagina di co-selling Opportunities verrà visualizzato un collegamento denominato **"PSC Deal Migration"** , che consente di aprire la migrazione guidata dell'accordo.

Leggere questa sezione prima di iniziare la migrazione dell'accordo.

**Idoneo per la migrazione**

Solo alcune offerte sono idonee per la migrazione da CPS a PC. Questa migrazione guidata è stata creata per aiutare i partner a partecipare al centro per i partner, dove continuano a collaborare attivamente con i clienti per chiudere l'offerta. **Solo le offerte in stato aperto con i dettagli validi per l'account partner (ID MPN valido) e la registrazione non in corso non sono idonee per la migrazione.**

**Non idoneo per la migrazione**

- Le trattative della valutazione della soluzione non sono idonee per la migrazione di Deal
- Le offerte aziendali per le licenze OEM non sono idonee per la migrazione di Deal
- Qualsiasi accordo contrassegnato come vinto in PSC non è idoneo per la migrazione. Gestire la registrazione se idonea per le offerte contrassegnate come vinte deve essere completata in CPS.

## <a name="pre-requisites-for-deal-migration"></a>Prerequisiti per la migrazione di Deal

Prima di avviare la migrazione degli accordi dal PC, seguire le istruzioni riportate di seguito per configurare le offerte di PSC per una corretta migrazione.

1. Tutti i membri del team di vendita della società che lavorano sulle offerte aperte sono informati sulla migrazione.
2. I membri del team di vendita hanno eseguito il training per usare il centro per la gestione dei partner.
3. Tutte le informazioni necessarie sono elencate di seguito.
    - Dettagli aziendali del cliente, inclusi nome e indirizzo
    - Dettagli del contatto del cliente se si tratta di un'offerta di co-selling
    - Almeno una soluzione
    - Almeno un membro del team con tutti i dettagli, il nome, il cognome, l'ID di posta elettronica e il numero di telefono
    - Valore di Deal
    - Data di chiusura dell'affare stimata
    - Note partner

È possibile utilizzare le funzionalità di download e caricamento bulk in PSC per pulire i dati per tutte le offerte idonee.

>[!Note]
> La migrazione dell'accordo avrà esito positivo anche se i prerequisiti precedenti non vengono soddisfatti. Tuttavia, non è possibile modificare lo stato dell'operazione se uno dei campi obbligatori indicati in precedenza nel centro per i partner non è disponibile. Sarà quindi necessario immettere tutte le informazioni richieste mancanti nelle offerte del centro per i partner per iniziare a utilizzarle. **È consigliabile pulire le offerte idonee in PSC prima di eseguirne la migrazione al centro per i partner.**

La migrazione dell'affare nel centro per i partner è stata creata con una sola esperienza. È sufficiente fare clic sul pulsante **"migrate Deals"** quando la società è pronta per la migrazione delle offerte idonee. **Non è possibile scegliere le offerte di cui si vuole eseguire la migrazione da CPS. Se non si vuole eseguire la migrazione di eventuali offerte al centro per i partner, spostarle nello stato Closed in PSC prima di avviare la migrazione.**

>[!Note]
> Dopo l'avvio della migrazione, **potrebbero essere necessarie fino a 24 ore per la migrazione delle offerte**.

Al termine della migrazione, lo stato del messaggio del banner verrà modificato per essere completato con un collegamento al report di migrazione. Scaricare il report per visualizzare i dettagli delle offerte migrate dal CPS al PC.

Il report include i dettagli seguenti.

1. **ID engagement del centro** per i partner: identificatore univoco nel centro per tutte le operazioni in un engagement. Sono disponibili due offerte, una per il partner e una per Microsoft in un impegno di co-selling nel centro per i partner.
2. **ID di riferimento del centro** per i partner: identificatore univoco nel centro partner per l'operazione appartenente al partner.
3. **Nome dell'operazione** : identificatore assegnato alla trattazione in CPS.
4. **ID Deal PSC** : identificatore univoco in PSC per l'operazione.
5. **Errors** : per indicare se si è verificato un errore durante la migrazione di un'operazione specifica.

Tutte le operazioni di cui è stata eseguita la migrazione non saranno visibili in CPS. È possibile lavorare sulle offerte migrate nel computer. Non verranno apportate modifiche alle interazioni con i venditori Microsoft per le offerte di co-selling.

Le offerte migrate da CPS saranno disponibili nelle schede in ingresso e in uscita in base all'origine dell'operazione. Tutti gli accordi creati dal partner saranno disponibili nella scheda in uscita e le offerte avviate da Microsoft saranno disponibili nella scheda in ingresso del centro per i partner. Ci saranno due tipi di offerte che verranno create dopo la migrazione.

1. Offerte di **co-selling** : le offerte contrassegnate come co-selling in CPS verranno create come offerte di co-selling nel centro per i partner.
2. **Offerte gestite da partner** : le trattative non contrassegnate come co-sell verranno create come offerte per i partner nel centro per i partner. Le trattative di partner sono visibili ai venditori Microsoft e possono essere aggiornate alle offerte di co-selling prima di raggiungere lo stato finale (vinto, perso). Inoltre, le trattative dei partner sono idonee per la registrazione dell'accordo se è presente una soluzione incentive idonea nell'affare.

>[!Important]
> Se si verificano errori dovuti alla migrazione di alcune offerte, **è possibile riavviarla facendo clic sul pulsante "migrate** Deals". Verrà abilitato solo se sono ancora presenti alcune offerte idonee da migrare. Questa operazione sarà utile anche se ci si trova nella fase di transizione in cui vengono create nuove trattative in PSC dopo l'avvio della migrazione dell'accordo.

Una volta completata la migrazione di tutte le trattative, verrà visualizzato il banner **"nessuna operazione di migrazione"** con il pulsante **"migrate Deals"** **disabilitato**.

Dopo aver completato la migrazione degli utenti e/o aver eseguito la migrazione, usare le linee guida seguenti per decidere la strategia di migrazione:

Se la società ha un partner Development Manager (PDM): quando l'account del centro per i partner è configurato e gli utenti sono passati e hanno ruoli e autorizzazioni, è possibile spostare le attività di co-selling nel centro per i partner. Informare il PDM per eseguire il compartimento invece di attendere il completamento della scadenza della migrazione, in modo da consentire l'esecuzione di tutte le nuove offerte nel centro per i partner.

>[!Note]
>Una volta eseguito questo passaggio, sarà possibile agire solo sulle operazioni attive esistenti in CPS. Non è possibile creare nuove trattative né ricevere offerte da Microsoft Sellers in PSC.

Se la società non dispone di un PDM, assicurarsi che tutti gli account utente siano configurati e verificati da tutti gli utenti. Si riceverà una notifica tramite un messaggio di posta elettronica e un banner in PSC relativi alla data esatta in cui è possibile avviare la co-selling nel centro per i partner. Tenere presente che sarà comunque necessario gestire le operazioni attive esistenti in CPS.

>[!Important]
>Non verrà eseguita la migrazione delle offerte attive al PC. Fino al 31 marzo 2021 per chiudere e registrare le offerte.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Passaggi successivi per gli amministratori del CPS, i gestori di Deal e i venditori del PSC

Informazioni su come co-selling nel centro per i partner.
Si tratta di un passaggio importante, che consente di prepararsi per il co-selling nel centro per i partner. Comprendere i flussi di lavoro e le modifiche apportate al centro per i partner, in modo da potervi covendere immediatamente. Per iniziare, leggere completamente questo documento. Un set di risorse valido è disponibile anche nella [raccolta di esperienze di co-selling](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principali differenze tra i flussi di lavoro PSC e PC

|**Scenario**|**Connessione vendite partner**|**Centro per i partner**|
|-----|:-----|:-----|
|Ruoli utente|PSC ha ruoli di amministratore, Deal Manager e seller.|Il computer dispone solo di un ruolo di [amministratore di riferimento](permissions-overview.md#manage-referrals) che fornisce le autorizzazioni di lettura e scrittura per tutte le offerte.|
|Invito a Microsoft in un'offerta di co-selling|Avviato da Microsoft seller, non esiste alcuna domanda esplicita da un partner.|Il partner dovrà effettuare una [richiesta esplicita](manage-co-sell-opportunities.md#add-solutions) se è necessaria una guida a Microsoft seller per un'operazione. Microsoft Seller offre un'opzione per rifiutare la richiesta.|
|Expiry|Non esiste alcun concetto di scadenza della trattativa.|Le offerte per i partner in ingresso scadono entro 14 giorni se non vengono accettate dal partner. Lo stesso avviene con le trattative in uscita partner che possono passare allo stato scaduto se il venditore Microsoft non agisce su di essi entro 14 giorni.|
|Dettagli sui venditori Microsoft|Visibile non appena viene creata una trattativa.|I dettagli di Microsoft seller sono condivisi con il partner solo se il venditore accetta in modo esplicito l'invito per il co-selling dal partner.|
|[Pipeline privata](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Non disponibile.|I partner possono condividere la propria pipeline senza fornire visibilità ai venditori Microsoft.|
|Soluzioni|Le soluzioni che appartengono a un solo listino prezzi possono essere aggiunte a un'operazione.|Il partner può aggiungere [soluzioni](manage-co-sell-opportunities.md#add-solutions) che appartengono agli elenchi seguenti. a) soluzioni b) dal catalogo di Microsoft First Party (simile al ruolo Transaction Deal in CPS) e c) Co-selling di altri partner di terze parti (in modo analogo al ruolo di Deal ISV in CPS).|
|Assegnazione di Deal|Solo i venditori assegnati possono visualizzare e agire sulle offerte.|I membri del team possono essere aggiunti a una trattativa per specificare gli utenti che lavorano a una trattativa, non vi è alcun blocco di altri amministratori dei riferimenti da visualizzare o agire su tali offerte.|
|Organizzazione del cliente|Immissione di testo in formato libero.|È possibile cercare l' [organizzazione del cliente](manage-co-sell-opportunities.md#select-your-customer) nel [database D&B](https://www.dnb.com/) semplicemente digitando alcuni caratteri. Il nome e l'indirizzo validi vengono popolati automaticamente in base alla scelta.|
|Contatto del cliente|Non obbligatorio.|Non obbligatorio per la condivisione di pipeline privata. Obbligatorio se il venditore Microsoft è invitato a partecipare a una richiesta di co-selling.|
|API pubblica|Non disponibile.|[API pubblica](/partner/develop/referrals) per gestire a livello di codice i riferimenti del centro per i partner.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Eseguire il mapping dei campi in PSC ai campi corrispondenti nel centro per i partner

In questa sezione vengono confrontate le schermate selezionate (o "mappe") visualizzate per CPS rispetto alla visualizzazione corrispondente nella sezione relativa alle opportunità di co-selling del centro per i partner.

Vengono visualizzati i cerchi numerati, gialli o rossi in ogni coppia di schermate:

- **Cosa significano i cerchi gialli?** I cerchi numerati, gialli vengono visualizzati per primi in ogni schermata del CPS. Si troverà quindi uno screenshot del centro partner complementare sotto con molti degli stessi numeri.

   Per vedere in che modo ogni campo o attributo in PSC è mappato alla controparte del centro per i partner, abbinare i cerchi numerati tra loro nelle due schermate correlate. Ad esempio, trovare la corrispondenza con il valore "1" giallo nella prima schermata del PSC, per il numero giallo "1", nella seconda schermata del centro per i partner.

- **Che cosa significa un cerchio rosso?** Se viene visualizzato un cerchio rosso in una schermata, che indica che il campo PSC non è disponibile nel centro per i partner.

I mapping dei campi del centro da PSC a partner vengono visualizzati per le aree seguenti:

1. PSC home page mappato alla visualizzazione predefinita per le opportunità di co-selling del centro partner
1. Visualizzazione griglia di PSC mappata alla visualizzazione dell'accordo del centro per i partner
1. Visualizzazione dettagli affare PSC mappato alla visualizzazione dettagli dell'affare del centro per i partner
1. Visualizzazione Aggiungi prodotti di CPS mappato al centro per i partner Aggiungi visualizzazione soluzioni
1. Visualizzazione della gestione utenti del CPS mappata alla vista Gestione utenti del centro per i partner
1. Visualizzazione assegnazione ruolo utente PSC mappata alla visualizzazione assegnazione ruolo del centro per i partner
1. Visualizzazione notifiche PSC mappata alla visualizzazione notifiche del centro per i partner

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-PSC home page mappato alla visualizzazione predefinita per le opportunità di co-selling del centro partner

Confrontare i circoli corrispondenti e numerati tra lo screenshot principale del PSC e lo screenshot del centro per i partner. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo del centro per i partner corrispondente.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Immagine che mostra i mapping dei campi tra il home page di partner Sales Connect e la visualizzazione predefinita di opportunità di co-selling nel centro per i partner." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-visualizzazione griglia del PSC mappata alla visualizzazione dell'accordo del centro per i partner

Confrontare i circoli corrispondenti e numerati tra lo screenshot principale del PSC e lo screenshot del centro per i partner. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo del centro per i partner corrispondente.  

> [!NOTE]
> Altre considerazioni vengono visualizzate sotto le schermate.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione griglia partner Sales Connect (PSC) e la vista di gestione dei partner Center." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considerazioni speciali:**

- Non è disponibile alcuna visualizzazione elenco nel centro per i partner come quello di CPS.  Tutte le offerte sono elencate in base alla data più recente ricevuta o creata con le informazioni sul cliente e il tipo di contratto. Per impostazione predefinita, la prima operazione nella vista è selezionata. La maggior parte dei valori visualizzati nel formato di tabella PSC è disponibile nella visualizzazione dettagli dell'operazione nel computer.
- Il ruolo Deal non è un campo obbligatorio in PC. Non viene visualizzato o acquisito in nessuno dei flussi di lavoro. Viene derivato automaticamente sul lato venditore Microsoft in base alle soluzioni aggiunte all'affare.
- La data dell'Ultima modifica non viene visualizzata nella pagina dei dettagli del riferimento nel PC. I partner possono usare la funzionalità di ordinamento per ordinare le offerte in base alla data dell'ultimo aggiornamento.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-visualizzazione dettagli affare PSC mappata al centro per i partner

Confrontare i circoli corrispondenti e numerati nella schermata superiore (PSC) con lo screenshot del centro per i partner sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo o area corrispondente nel centro per i partner.

> [!NOTE]
> Altre considerazioni vengono visualizzate sotto le schermate.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione dettagli dell'affare partner Sales Connect (PSC) e la visualizzazione dettagli dell'affare del centro per i partner." lightbox="images/pscmigration/deal-details-expanded.png":::

**Considerazioni speciali:**

- I partner possono modificare un'operazione selezionando il pulsante modifica nella visualizzazione dei dettagli del partner Deal (6). Dopo aver selezionato il pulsante modifica, tutti i campi diventeranno modificabili. Sarà quindi possibile salvare o annullare le modifiche apportate all'operazione.
- Non è possibile chiudere l'affare come duplicato nel centro per i partner.
- Il risultato del cliente non è disponibile nel centro per i partner. Tutti i dettagli relativi alle interazioni dei clienti possono essere aggiornati nella sezione Note di PC.
- La data di chiusura della soluzione prevista è disponibile solo per le trattative degli OEM nel centro per i partner. Queste informazioni non vengono visualizzate per altri tipi di tratteggio.
- Il programma di licenza non è richiesto nel computer. Queste informazioni vengono dedotte automaticamente in base alle soluzioni selezionate nell'affare.

>[!Note]
>Eventuali operazioni contrassegnate come vinte o perse non possono essere modificate in seguito. Prestare attenzione quando si trasferisce una trattativa in uno di questi stati terminali.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-la visualizzazione ' Aggiungi prodotti ' del CPS è mappata alla visualizzazione ' Aggiungi soluzioni ' del centro per i partner

Confrontare i circoli corrispondenti e numerati nella schermata superiore (PSC) con lo screenshot del centro per i partner sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo o area corrispondente nel centro per i partner.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione di aggiunta dei prodotti partner Sales Connect (PSC) e la visualizzazione Aggiungi soluzioni per il centro per i partner." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-Gestione utenti in CPS rispetto al centro per i partner

Confrontare i circoli corrispondenti e numerati nella schermata superiore (PSC) con lo screenshot del centro per i partner sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo o area corrispondente nel centro per i partner.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Immagine che mostra i mapping dei campi tra la Home page di gestione utenti del partner Sales Connect (PSC) e la visualizzazione della pagina Gestione utenti del centro per i partner all'interno dell'area Impostazioni account."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-assegnazione di ruolo utente in CPS rispetto al centro per i partner

Confrontare i circoli corrispondenti e numerati nella schermata superiore (PSC) con lo screenshot del centro per i partner sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo o area corrispondente nel centro per i partner.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione assegnazione ruolo Partner Sales Connect (PSC) e la visualizzazione assegnazione ruolo centro partner." lightbox="images/pscmigration/roles-expanded.png":::

**Considerazioni speciali:**

- Il ruolo equivalente per l'amministratore del CPS è il ruolo di amministratore dell'account nel centro per i partner.
- Nel centro per i partner è disponibile un solo ruolo per la gestione dei deal di co-selling. Questo ruolo è il ruolo di amministratore di riferimento.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-notifiche in CPS rispetto al centro per i partner

Confrontare i circoli corrispondenti e numerati nella schermata superiore (PSC) con lo screenshot del centro per i partner sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC nel centro per i partner. I cerchi rossi indicano che non esiste alcun campo o area corrispondente nel centro per i partner.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Immagine che mostra il mapping tra le notifiche di partner Sales Connect (PSC) e la visualizzazione notifiche del centro per i partner."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passaggio da CPS al centro per i partner-domande frequenti

Le sezioni seguenti rispondono a domande frequenti sulla migrazione.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1: cosa fare se non si ha accesso al centro per I partner?

È possibile contattare gli amministratori elencati nella pagina "nessun accesso" per ottenere i ruoli assegnati. Per le autorizzazioni di lettura e scrittura, è necessario il ruolo di [amministratore](permissions-overview.md#manage-referrals) dei riferimenti nella sezione dei riferimenti. Se si gestiscono solo i profili di business, sarà necessario il ruolo di amministratore del profilo di business nel centro per i partner.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Immagine che mostra l'esperienza di accesso non disponibile nel centro per i partner.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-chi può concedere l'accesso alla sezione relativa ai riferimenti in centro per i partner?

L' [amministratore dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) può concedere l'accesso alla scheda riferimenti. Per trovare l'amministratore dell'account, selezionare **Impostazioni account** dall'icona a forma di ingranaggio nella parte superiore destra del [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner. Selezionare quindi **Gestione utenti** nella barra di spostamento di secondo livello a sinistra. Nella parte superiore dell'elenco di utenti selezionare il menu a discesa **filtro** e modificare l'opzione di **amministratore account**. La pagina visualizzerà tutti gli amministratori dell'account con i rispettivi indirizzi di posta elettronica. Chiedere a uno di loro di assegnare il ruolo di amministratore di riferimento per l'account aziendale.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3: il pulsante + nuovo affare è disattivato per l'account. Cosa devo fare per iniziare a creare le offerte?

Questa situazione si verifica solo se non sono presenti soluzioni di co-selling pronte collegate all'organizzazione MPN in uso nel centro per i partner. Contattare il PDM per ottenere l'ID MPN della soluzione corretta o creare un ticket di supporto che menzioni il problema, "pulsante nuovo affare disattivato dopo la migrazione di CPS".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-è possibile assegnare gli accordi a un utente specifico dell'organizzazione, ad esempio PSC?

È possibile assegnare i membri del team a un affare specifico. Non impedisce ad altri amministratori di riferimento di visualizzare o agire su tali offerte.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5: è disponibile una vista di tutte le offerte assegnate all'utente?

È possibile usare la funzionalità Preferiti, che è una scheda a livello di utente. È possibile contrassegnare tutte le offerte che vengono assegnate come preferiti per ottenere un accesso rapido alle offerte.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6: esiste una visualizzazione di sola lettura per le offerte?

No, non è disponibile alcuna visualizzazione di sola lettura delle offerte nella sezione dei riferimenti. Tutti gli amministratori dei riferimenti avranno accesso completo in lettura e scrittura a tutte le offerte.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-come è possibile registrare una transazione dopo averla contrassegnata come vinta?

Se il problema soddisfa i criteri indicati di seguito, viene visualizzata una finestra popup per avviare la [registrazione dell'accordo](./register-deals.md).

- Una soluzione idonea per gli incentivi è allegata alla trattativa.
- Il venditore Microsoft è invitato a partecipare all'affare oppure ha invitato l'utente all'affare.
- La scheda Microsoft è nello stato accettato o vinto nel centro per i partner.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-viene ricevuto un messaggio di errore quando si seleziona il pulsante "+ nuova registrazione per la registrazione" nella sezione relativa alla registrazione dell'accordo. Come è possibile registrare le offerte?

Il pulsante **+ nuovo contratto di registrazione** deve essere usato solo dai partner registrati nel programma ISV Connect per la registrazione di una trattativa senza opportunità di co-selling corrispondenti nel centro per i partner. Per la registrazione di un'opportunità di co-selling, viene visualizzata una finestra popup quando l'accordo è contrassegnato come vinto e soddisfa i criteri per la registrazione dell'accordo.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-l'aggiunta di un'organizzazione cliente è obbligatoria?

Sì, l'aggiunta di un' [organizzazione cliente](./manage-co-sell-opportunities.md#select-your-customer) è obbligatoria nel centro per i partner. Per iniziare, cercare il percorso in cui si trova il cliente. In base ai dettagli disponibili; è possibile essere specifici, tra cui il nome esatto della compilazione, o fornire solo i dettagli della città. La ricerca nell'organizzazione recupererà tutte le entità legali che corrispondono al nome immesso, in modo da non dover immettere i dettagli degli indirizzi. Tutti i dettagli vengono compilati automaticamente in base all'organizzazione selezionata.

### <a name="10---are-customer-contact-details-mandatory"></a>10-i dettagli del contatto del cliente sono obbligatori?

Dipende dal [tipo di problema](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) che si sta creando. Se si sta semplicemente condividendo la pipeline senza richiedere assistenza da parte di Microsoft Sales Organization, è possibile scegliere di non fornire i dettagli di contatto del cliente. Se si sta eseguendo la co-selling in cui si cerca attivamente assistenza da parte del venditore Microsoft, sarà necessario fornire i dettagli di contatto del cliente. Prima di creare una richiesta di co-selling nel centro per i partner, si dovrebbe ottenere il consenso esplicito del cliente.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-Quante soluzioni è possibile aggiungere a una trattativa?

È possibile aggiungere fino a un massimo di 50 soluzioni, in modo analogo a "prodotti" in CPS. A differenza di PSC, è possibile combinare soluzioni da soluzioni di co-selling personalizzate, SKU Microsoft e altre soluzioni idonee per la co-selling di terze parti. Non è presente alcun ruolo di gestione che deve essere selezionato o disponibile nel centro per i partner. Per gli SKU Microsoft, è possibile aggiungere facoltativamente la quantità e il prezzo per ogni SKU aggiunto al problema.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12: quando si riceveranno informazioni dettagliate sui venditori Microsoft dopo la creazione di una trattativa?

I venditori Microsoft vengono assegnati solo dopo la corrispondenza del requisito esatto della Guida indicato durante la creazione dell'affare con la persona venditore pertinente sul lato Microsoft. Anche dopo l'assegnazione, i venditori Microsoft avranno la possibilità di accettare o rifiutare l'invito al co-selling. Solo se un invito al co-selling viene accettato da un venditore, l'operazione verrà aggiornata con i dettagli di contatto del venditore Microsoft. Il contratto di contratto per i venditori Microsoft che operano sull'accordo è di 14 giorni. Si tratta dello stesso contratto di prezzo che i partner devono agire prima di passare allo stato scaduto.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-dove è possibile trovare l'ID opportunità?

L'ID opportunità in PSC è identico a quello dell'ID dell'accordo in PC. È possibile trovare l'ID dell'affare accanto al nome dell'affare quando si apre qualsiasi affare.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14: come può ottenere l'accesso al PC da PDM?

Non è possibile accedere direttamente al centro per i partner PDM a differenza di PSC. Sono disponibili più opzioni per abilitare questa funzionalità, come indicato di seguito.

- OCP Insights: se PDM Visualizza solo le offerte e lo stato di avanzamento correlati, è possibile usare il portale di OCP Insights per ottenere la visualizzazione dell'organizzazione. Si tratta di uno strumento interno ed è disponibile solo per PDM. Si noti che OCP Insights non è disponibile per gli utenti della società.
- Utente guest in centro per i partner: è possibile aggiungere l' @microsoft.com account PDM come utente Guest nel centro per i partner e assegnare loro un ruolo di amministratore in modo che possano visualizzare e agire sui riferimenti.
- Creazione di un [nuovo utente](./create-user-accounts-and-set-permissions.md#add-a-new-user) nel tenant: è possibile creare un nuovo utente nel tenant e condividere i dettagli con il PDM in modo che possano visualizzare i riferimenti e agire su di essi in modo analogo ad altri utenti di riferimento nell'account.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Individuazione dell'ID MPN corretto se l'account in CPS non è associato a un MPN valido

Se ci si trova nel punto in cui si è visto un banner in PSC che menziona "CPS non valido MPN ID Association problem", l'utente si trova nel posto giusto.

Per prima cosa, trovare l'ID MPN corretto attenendosi alla procedura seguente

- Accedere all'account del centro per i partner
- Usare le indicazioni fornite nella [documentazione delle impostazioni dell'account](./partner-center-account-setup.md#locate-your-mpn-id) per individuare l'ID MPN.

Successivamente,

- Se si dispone di un PDM, chiedere loro di correggere l'ID MPN con l'ID MPN corretto dall'account del centro per i partner.
- Se non si dispone di un PDM, inviare un messaggio di posta elettronica all'indirizzo indicato nel banner del CPS con le informazioni sull'account PSC visualizzate nel banner del CPS e l'ID MPN corretto dall'account del centro per i partner.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Risorse che consentono di creare e gestire le proprie offerte nel centro per i partner

Se non sono stati ancora letti gli argomenti della Guida di co-selling, le risorse seguenti consentiranno di gestire le offerte nel centro per i partner.

|**Per eseguire questa operazione**   |**Leggi**   |
|-----------------------|:-----------------------|
|Informazioni sulle schede e sulla navigazione nella pagina opportunità di co-selling|[Esplorazione della sezione di co-selling](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selezione di un'organizzazione cliente dall'elenco D&B |[Selezionare il cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modifica dei campi nella sezione dettagli sull'accordo|[Dettagli sull'offerta](./manage-co-sell-opportunities.md#deal-details)|
|Aggiunta dei membri del team a un team di gestione|[Aggiungere i dipendenti](./manage-co-sell-opportunities.md#add-team-members)|
|Risposta a un affare di co-selling|[Gestisci le offerte di co-selling](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registra le offerte acquisite nel centro per i partner |[Registrare una nuova trattativa](./register-deals.md)
|Ottieni informazioni dettagliate sul riferimento e Scopri come fanno i tuoi riferimenti |[Informazioni dettagliate sulle segnalazioni](./referral-insights.md)
|Creazione e gestione del profilo di business|[Gestire profilo di business](./create-a-marketing-profile.md)
|Gestisci lead per il tuo profilo business |[Gestire lead](./manage-leads.md)|

## <a name="next-steps"></a>Passaggi successivi


- [Partner Sales connettersi alla cartella](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) di lavoro del centro per i partner-cartella di lavoro per allineare i processi di vendita e i ruoli dei partner con i nuovi processi di vendita tramite partner Center e partner Sales Connect.
- [Guida alla co-selling del centro](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) per i partner: linee guida per identificare un modello operativo tramite il centro per i partner per gestire i lead o le opportunità di co-selling e registrare le offerte
- [Deck di gestione dei riferimenti](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : istruzioni dettagliate visualizzate per gestire i lead e le opportunità di co-selling tramite il centro per i partner.
- [Pubblicazione e gestione nel Marketplace commerciale](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : istruzioni dettagliate visualizzate per creare, gestire e pubblicare offerte tramite il centro per i partner del Marketplace commerciale.