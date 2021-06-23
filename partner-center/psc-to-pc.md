---
title: Eseguire la migrazione da Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come i partner Microsoft possono eseguire la migrazione da Partner Sales Connect (PSC) a Partner Center e creare o gestire le offerte inviate dai venditori Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551436"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guida al co-selling in Partner Center (PC) per i partner che eseere la migrazione da Partner Sales Connect (PSC)

**Ruoli appropriati:** Account admin | Informazioni di amministrazione delle segnalazioni | Partner Sales Connect (PSC) seller | Amministratore di Partner Sales Connect (PSC) | Partner Sales Connect (PSC) deal manager

Questo articolo fornisce indicazioni per i partner che eseguono la migrazione da Partner Sales Connect (PSC) a Partner Center (PC) in modo che possano continuare a creare e gestire le offerte di co-selling in Partner Center.

>[!Note]
> Se si è qui perché è stato visto un banner in PSC sulla migrazione, si è nel posto giusto. Questa guida non è applicabile a Solution Assessment (SA) e ai partner aziendali di gestione delle licenze OEM che gestiscono le proprie trattative in PSC.

>[!Important]
> A partire dal 1° aprile 2021 l'azienda non sarà in grado di creare o modificare offerte in PSC. **Sarà comunque possibile scaricare i dati delle trattative esistenti usando la funzionalità di esportazione in blocco in PSC. È anche possibile [eseguire la migrazione di offerte](psc-to-pc.md#psc-deals-migration) aperte da PSC Partner Center dopo questa data.** <br><br> Se sono presenti offerte su cui si sta lavorando attivamente che contengono soluzioni idonee per l'incentivo di co-selling IP, sono disponibili due opzioni: <br><br> 1. Contrassegnare l'accordo come vinto e completare la registrazione dell'offerta in PSC prima del 31 marzo 2021. <br> 2. [Eseguire la migrazione delle](psc-to-pc.md#psc-deals-migration) Partner Center in modo da ottenere più tempo per lavorare sull'accordo e per avviare la registrazione dell'offerta.

Come si sa, **l'azienda perderà l'accesso a PSC dopo il 30 aprile 2021.** Tuttavia, tutto ciò che si vuole fare in Partner Center, ad esempio creare offerte di co-selling, gestire le offerte e agire sulle offerte inviate dai venditori Microsoft.

Ci saranno tuttavia differenze. Le indicazioni seguenti consentono di semplificare la transizione a Partner Center più semplice e semplice.

## <a name="before-you-move-things-you-need-to-know"></a>Prima di procedere, è necessario conoscere le informazioni necessarie

### <a name="if-you-are-a-psc-admin"></a>Gli amministratori PSC

- È necessario un messaggio di posta elettronica di lavoro per accedere [a Partner Center](https://partner.microsoft.com/).
- Configurare l'account con l'aiuto dell'Partner Center [amministratore dell'account.](permissions-overview.md)
- Informazioni su come co-vendere in Partner Center leggendo questo documento.
- Configurare gli account utente in Partner Center per tutti gli utenti PSC (ruoli Amministratore, Gestore delle trattative e Venditore) e assegnare loro i ruoli di amministratore [delle segnalazioni.](permissions-overview.md)

>[!IMPORTANT]
> Assicurarsi che l'ID Microsoft Partner Network (MPN) visualizzato nel banner PSC sia disponibile nell'elenco delle località MPN in Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Immagine che mostra il banner PSC in cui i partner possono trovare l'ID MPN.":::

 Per verificare che l'ID MPN venga visualizzato come posizione MPN Partner Center, accedere al [dashboard](https://partner.microsoft.com/dashboard)di Partner Center , quindi selezionare **Impostazioni** (icona a forma di ingranaggio) in alto a destra nella schermata, seguita da **Impostazioni account**. Nel menu di spostamento a sinistra  di secondo livello selezionare Località per visualizzare l'elenco di tutti gli ID e i percorsi MPN associati all'account Partner Center locale.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se si è un gestore o un venditore PSC

- È necessario un messaggio di posta elettronica di lavoro per accedere al dashboard Partner Center [lavoro.](https://partner.microsoft.com/dashboard)
- Se si usa un account non aziendale in PSC o l'indirizzo di posta elettronica aziendale è per una società diversa da quella partner, contattare l'amministratore PSC per informazioni sulla configurazione dell'account.
- Rivolgersi all'amministratore PSC se la configurazione dell'account Partner Center è completa indipendentemente dall'account che si usa per accedere a PSC.
- Verificare se si ha accesso a Partner Center e alla sezione Segnalazioni.
- Leggere questo documento per comprendere i flussi di lavoro e le modifiche apportate Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Come amministratore in PSC, questi sono i passaggi successivi

Dal menu Partner Center di spostamento a sinistra selezionare **l'opzione Segnalazioni.** Verificare che sia possibile accedere alle pagine Segnalazioni.

  >[!Note]
  > Potrebbe essere necessario disconnettersi da Partner Center accedere di nuovo per aggiornare le credenziali per l'accesso alle pagine Segnalazioni.

Se l'opzione Segnalazioni non è visualizzata nel menu Partner Center o nelle pagine correlate alle segnalazioni, contattare l'amministratore  [dell'account](permissions-overview.md) aziendale e chiedere loro di concedere l'accesso all'opzione Segnalazioni e all'area correlata. 

Per trovare l'amministratore dell'account dell'azienda:

1. Selezionare **Impostazioni account** dall'icona a forma di ingranaggio in alto a destra nel dashboard Partner Center sicurezza.

1. Selezionare **Gestione utenti** dal menu di spostamento a sinistra di secondo livello.

1. Nella parte superiore dell'elenco utenti selezionare il menu **a** discesa Filtro. Modificare l'opzione in **Account admin**.

   Nella pagina verranno visualizzati tutti gli amministratori dell'account con i rispettivi indirizzi di posta elettronica. Inviare un messaggio di posta elettronica a uno di essi e chiedere di assegnare il ruolo di amministratore delle segnalazioni per l'account aziendale.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Immagine che mostra gli amministratori dell'account nella pagina di gestione utenti delle impostazioni partner.":::

>[!Important]
>- Se il ruolo implica solo la gestione degli utenti in PSC, chiedere all'amministratore dell'account dell'azienda di assegnare il ruolo di amministratore [dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) in Partner Center. 
>- Se il ruolo include anche la gestione delle opportunità di co-selling, chiedere di assegnare il ruolo di amministratore [delle](permissions-overview.md#manage-referrals) segnalazioni.
> - È buona idea anche designare un lead di gestione delle modifiche tra gli amministratori PSC. In questo modo, tutti gli amministratori PSC non doranno contattare singolarmente gli amministratori Partner Center account. Al contrario, il lead di gestione delle modifiche può quindi essere la persona principale che lavora con l Partner Center amministratore dell'account.

## <a name="user-migration"></a>Migrazione degli utenti

Dopo aver configurato l'account in Partner Center, usare la migrazione guidata utente nella pagina opportunità di co-selling per assegnare automaticamente i ruoli Partner Center ai dipendenti dell'azienda.

>[!Note]
> La migrazione degli utenti può essere eseguita solo [dagli amministratori dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) dell'azienda. Se non si ha il ruolo di amministratore dell'account, trovare un amministratore dell'account che possa aiutare a configurare gli account utente con l'aiuto della Migrazione guidata utenti.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Immagine che mostra la Migrazione guidata utente.":::

Gli amministratori dell'account vedranno un collegamento alla Migrazione guidata utenti PSC nella pagina delle opportunità di co-selling accanto alla guida alle segnalazioni. È possibile avviare la migrazione dell'utente selezionando il collegamento. Per avviare la migrazione degli utenti, gli amministratori possono selezionare il collegamento. Possono eseguire questo passaggio di migrazione utente più volte fino a quando a tutti gli utenti non vengono assegnati ruoli Partner Center.

La tabella di migrazione utente include i dettagli seguenti:

- Account utente - ID posta elettronica del dipendente
- Account partner PSC: account a cui è associato il dipendente in PSC
- Ruolo utente PSC: uno dei tre ruoli assegnati a in PSC.
- Posizione MPN del PC: località per cui all'utente verranno assegnati ruoli Partner Center (PC). L'account partner PSC MPN viene usato per trovare la posizione MPN equivalente Partner Center assegnare le autorizzazioni. L'intera organizzazione indica l'ID MPN vOrg.
- Ruolo utente PC: ai dipendenti vengono assegnati ruoli in base ai ruoli utente PSC. All'amministratore in PSC verranno assegnati i ruoli di amministratore delle segnalazioni Partner Center. Al venditore verrà assegnato il ruolo utente segnalazioni Partner Center. Altre informazioni sui ruoli Partner Center e sulle operazioni che gli utenti con questi ruoli possono eseguire Partner Center [qui](permissions-overview.md#manage-referrals)
- Tenant di PC AAD: tenant Microsoft Azure Active Directory (Azure AD) a cui sono assegnati gli utenti in Partner Center
- Stato: sono disponibili tre stati possibili per lo stato della migrazione
    - **Non migrato:** all'utente non è assegnato alcun Partner Center di segnalazioni
    - **Di cui è stata** eseguita la migrazione: l'utente è stato migrato correttamente con il ruolo pertinente assegnato, come illustrato nella tabella
    - **Errore** - Impossibile completare la migrazione a causa di un errore

In alcuni casi, la migrazione può avere esito negativo e causare errori. Ecco alcuni motivi per cui una migrazione potrebbe causare un errore e alcuni dei modi per risolvere il problema:

1. Gli utenti PSC possono usare un account non aziendale.

2. L'utente PSC potrebbe usare un account di un dominio diverso da quello in uso Partner Center.

   Per risolvere gli errori correlati agli scenari 1 e 2, chiedere all'utente di accedere Partner Center usando l'account aziendale collegato al tenant Azure AD lavoro. [L'amministratore globale](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) può essere utile.
   
   Per trovare l'amministratore globale: 
   - Accedere al dashboard Partner Center [e](https://partner.microsoft.com/dashboard) selezionare **Impostazioni account** dall'icona a forma di ingranaggio in alto a destra.
   - Selezionare **Gestione utenti** dalla barra di spostamento a sinistra di secondo livello.
   - Nella parte superiore dell'elenco utenti selezionare **il** menu a discesa Filtro e modificare l'opzione in **Amministratore globale**. Nella pagina vengono quindi visualizzati tutti gli amministratori globali con i rispettivi indirizzi di posta elettronica. Chiedere a uno di essi di assegnare il ruolo di amministratore delle segnalazioni per l'account aziendale.
   
      L'amministratore globale può creare un nuovo account utente nel tenant Azure AD o assegnare l'accesso utente guest agli altri utenti dell'account di dominio. Dopo aver configurato gli account per tutti i gestori e gli utenti PSC, devono accedere a Partner Center, selezionare **Segnalazioni** dal menu di spostamento a sinistra e verificare che possano visualizzare la pagina Segnalazioni.

3. L'utente ha già un ruolo di riferimento assegnato in Partner Center.
    - È possibile verificare il ruolo esistente dell'utente. Nell'angolo in alto a destra della Partner Center selezionare **Impostazioni** (icona a forma di ingranaggio), quindi **Impostazioni account**. Quando viene visualizzato un secondo menu di spostamento a sinistra, selezionare **Gestione utenti** e cercare l'utente.

## <a name="psc-deals-migration"></a>Migrazione di PSC Deals

Dopo aver completato la migrazione degli utenti, usare la migrazione guidata delle offerte nella pagina opportunità di co-selling per portare tutte le offerte aperte idonee da PSC a Partner Center. **Il collegamento alla migrazione delle offerte sarà visibile solo agli amministratori delle segnalazioni con l'intero ambito dell'organizzazione Partner Center.** Nella parte superiore destra della pagina Delle opportunità di co-selling verrà aperto il collegamento "Migrazione trattativa **PSC",** che aprirà la migrazione guidata delle trattative.

Leggere questa sezione prima di iniziare la migrazione dell'offerta.

**Idoneo per la migrazione**

Solo alcune offerte sono idonee per la migrazione da PSC a Partner Center. Questa migrazione guidata è stata creata per aiutare i partner a portare le proprie offerte Partner Center in cui stanno ancora lavorando attivamente con i clienti per chiudere l'accordo. **Per la migrazione sono idonee per la migrazione solo le trattative in stato aperto create a partire dal 1° gennaio 2020 con i dettagli validi dell'account partner (ID MPN valido) e non sottoposte alla registrazione dell'offerta.**

**Non idoneo per la migrazione**

- Le trattative di valutazione della soluzione non sono idonee per la migrazione delle trattative
- Le trattative aziendali sulle licenze OEM non sono idonee per la migrazione delle trattative
- Qualsiasi trattativa contrassegnata come vinta in PSC non è idonea per la migrazione. La registrazione dell'offerta, se idonea per le offerte contrassegnate come vinte, deve essere completata in PSC.

## <a name="pre-requisites-for-deal-migration"></a>Prerequisiti per la migrazione delle trattative

Prima di avviare la migrazione delle trattative Partner Center, seguire le istruzioni seguenti per configurare le trattative in PSC per una migrazione corretta.

1. Tutti i membri del team di vendita dell'azienda che lavorano alle trattative aperte sono informati su questa migrazione.
2. I membri del team di vendita sono addestrati per l'uso Partner Center per la gestione delle trattative.
3. Le trattative hanno tutte le informazioni necessarie, come descritto di seguito.
    - Dettagli dell'azienda del cliente, inclusi nome e indirizzo
    - Dettagli di contatto del cliente se si tratta di un accordo di co-selling
    - Almeno una soluzione
    - Almeno un membro del team con tutti i dettagli: nome, cognome, ID e-mail e numero di telefono
    - Valore dell'offerta
    - Data di chiusura dell'offerta stimata
    - Note per i partner

È possibile usare le funzionalità di download e caricamento in blocco in PSC per aggiungere tutti i dettagli mancanti nell'offerta per tutte le offerte idonee.

>[!Note]
> La migrazione delle transazioni avrà esito positivo anche se i prerequisiti precedenti non vengono soddisfatti. Tuttavia, non è possibile modificare lo stato dell'operazione se uno dei campi obbligatori indicati in precedenza Partner Center non sono disponibili. Sarà quindi necessario immettere tutte le informazioni necessarie mancanti nelle Partner Center per iniziare a lavorarvi. **È consigliabile pulire le offerte idonee in PSC prima di eseguire la migrazione a Partner Center.**

La migrazione delle trattative in Partner Center viene creata come esperienza con un solo clic. È necessario solo selezionare il pulsante "Esegui la migrazione **delle offerte"** quando l'azienda è pronta per eseguire la migrazione delle offerte idonee. **Non è possibile scegliere le offerte di cui si vuole eseguire la migrazione da PSC. Se non si vuole eseguire la migrazione di Partner Center, spostarle nello stato chiuso in PSC prima di avviare la migrazione.**

>[!Note]
> Dopo l'avvio della migrazione, la migrazione delle trattative può richiedere fino a **24 ore.**

Al termine della migrazione, lo stato del messaggio del banner verrà modificato per essere completato con un collegamento al report di migrazione. Scaricare il report per visualizzare i dettagli delle trattative di cui è stata eseguita la migrazione da PSC a Partner Center.

Il report include i dettagli seguenti.

1. **Partner Center ID engagement:** identificatore univoco in Partner Center per tutte le offerte in un engagement. Sono disponibili due offerte: una per il partner e una per Microsoft in un impegno di co-selling in Partner Center.
2. **Partner Center di segnalazione:** identificatore univoco in Partner Center per l'accordo appartenente al partner.
3. **Nome dell'offerta:** identificatore assegnato all'accordo in PSC.
4. **ID trattativa PSC:** identificatore univoco in PSC per l'operazione.
5. **Errori:** per indicare se si è verificato un errore durante la migrazione di un'operazione specifica.

Tutte le trattative di cui è stata eseguita la migrazione non saranno visibili in PSC. È possibile continuare a lavorare sulle trattative di cui è stata eseguita la migrazione Partner Center inclusa la registrazione delle trattative in Partner Center. Non verranno apportate modifiche alle interazioni con i venditori Microsoft per le offerte di co-selling.

Le offerte di cui è stata eseguita la migrazione da PSC saranno disponibili nelle schede In ingresso e In uscita in base all'origine dell'operazione. Tutte le offerte condivise dall'azienda saranno disponibili nella scheda In uscita e le offerte avviate da Microsoft saranno disponibili nella scheda In ingresso di Partner Center. Saranno disponibili due tipi di trattative che verranno create dopo la migrazione.

1. **Offerte di co-selling:** le offerte contrassegnate come co-selling in PSC verranno create come offerte di co-selling in Partner Center.
2. **Offerte guidate dai** partner: le offerte non contrassegnate come co-selling verranno create come offerte guidate dai partner Partner Center. Le offerte guidate dai partner sono visibili ai venditori Microsoft e possono essere aggiornate alle trattative di co-selling prima di raggiungere lo stato terminale (vinta, persa). Inoltre, le offerte guidate dai partner sono idonee per la registrazione delle trattative se è presente una soluzione idonea per incentivi.

>[!Important]
> Se si verificano errori a causa dei quali non è stato possibile eseguire la migrazione di alcune trattative, è possibile avviare nuovamente la migrazione dell'offerta facendo clic sul pulsante "Migrate deals" (Esegui la **migrazione delle trattative).** Verrà abilitato solo se è ancora necessario eseguire la migrazione di alcune offerte idonee. Questo sarà utile anche se ci si trova nella fase di transizione in cui vengono create nuove trattative in PSC dopo l'avvio della migrazione degli accordi.

Una volta completata la migrazione di tutte le trattative, verrà visualizzato il banner **"Nessuna** operazione di migrazione" con il pulsante **"Migrate deals"** che viene **disabilitato.**

Dopo aver completato la migrazione degli utenti e/o la migrazione dei dati, usare le indicazioni seguenti per decidere la strategia di migrazione:

Se l'azienda ha un Partner Development Manager (PDM): quando l'account Partner Center è configurato e gli utenti sono passati e hanno ruoli e autorizzazioni, è possibile spostare le attività di co-selling in Partner Center. Informare il PDM di effettuare il passaggio anziché attendere il completamento della migrazione, in modo da consentire a tutte le nuove offerte di passare a Partner Center.

>[!Note]
>Dopo aver effettuato questo passaggio, sarà possibile agire solo sulle trattative attive esistenti in PSC. Non è possibile creare nuove offerte né ricevere offerte dai venditori Microsoft in PSC.

Se l'azienda non ha un PDM: assicurarsi che tutti gli account utente siano impostati e verificati da tutti gli utenti. Si riceverà una notifica tramite un messaggio di posta elettronica e un banner in PSC relativo alla data esatta in cui è possibile avviare la co-selling Partner Center. Tenere presente che sarà comunque necessario gestire le trattative attive esistenti in PSC.

>[!Important]
> È possibile registrare le offerte contrassegnate come vinte fino al 30 aprile 2021.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Passaggi successivi per amministratori PSC, gestori di trattative PSC e venditori PSC

Informazioni su come co-vendere in Partner Center.
Si tratta di un passaggio importante che consente di prepararsi per la co-selling in Partner Center. Comprendere i flussi di lavoro e le modifiche Partner Center in modo che sia possibile eseguire il co-selling in modo efficace immediatamente. Per iniziare, leggere completamente questo documento. Un buon set di risorse è disponibile anche nella raccolta [di esperienze di co-selling.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Differenze principali tra I flussi di lavoro PSC e Partner Center di lavoro

|**Scenario**|**Partner Sales Connect**|**Centro per i partner**|
|-----|:-----|:-----|
|Ruoli utente|PSC ha ruoli di amministratore, gestore delle trattative e venditore.|Partner Center ha solo il ruolo [di amministratore delle](permissions-overview.md#manage-referrals) segnalazioni che concede sia l'autorizzazione di lettura che quella di scrittura per tutte le trattative.|
|Invitare Microsoft a un accordo di co-selling|Avviato dal venditore Microsoft, non viene chiesto esplicitamente dal partner.|Il partner dovrà effettuare una richiesta [esplicita se](manage-co-sell-opportunities.md#add-solutions) è necessaria un'assistenza per un venditore Microsoft per un'offerta. Il venditore Microsoft ha la possibilità di rifiutare la richiesta.|
|Expiry|Non esiste alcun concetto di scadenza dell'accordo.|Le offerte in ingresso del partner scadono tra 14 giorni se non vengono accettate dal partner. Lo stesso vale per le offerte in uscita dei partner in cui possono passare allo stato scaduto se il venditore Microsoft non agisce su di esse in 14 giorni.|
|Dettagli del venditore Microsoft|Visibile non appena viene creata una trattativa.|I dettagli del venditore Microsoft vengono condivisi con il partner solo se il venditore accetta esplicitamente l'invito per la co-selling dal partner.|
|[Pipeline privata](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Non disponibile.|I partner possono condividere la pipeline senza dare visibilità ai venditori Microsoft.|
|Soluzioni|È possibile aggiungere a un'offerta soluzioni appartenenti a un solo listino prezzi.|Il partner può [aggiungere soluzioni](manage-co-sell-opportunities.md#add-solutions) che appartengono ai seguenti elenchi. a) Le proprie soluzioni b) Soluzioni del catalogo microsoft di prima parte (simili al ruolo Transaction Deal in PSC) e c) soluzioni di co-selling di altri partner di terze parti (simili al ruolo ISV Deal in PSC).|
|Assegnazione di trattative|Solo il venditore assegnato può visualizzare e agire sulle offerte.|I membri del team possono essere aggiunti a un accordo per specificare le persone che lavorano a un accordo, non vi è alcun blocco degli altri amministratori delle segnalazioni di visualizzare o agire su tali offerte.|
|Organizzazione del cliente|Immissione di testo in formato libero.|È possibile cercare [nell'organizzazione del](manage-co-sell-opportunities.md#select-your-customer) cliente il [database D&B](https://www.dnb.com/) digitando solo alcuni caratteri. Il nome e l'indirizzo legali vengono popolati automaticamente in base alla scelta.|
|Contatto del cliente|Non obbligatorio.|Non obbligatorio per la condivisione di pipeline private. Obbligatorio se il venditore Microsoft è invitato a partecipare a una richiesta di co-selling.|
|API pubblica|Non disponibile.|[API pubblica per](/partner/develop/referrals) gestire le segnalazioni Partner Center a livello di codice.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Eseguire il mapping dei campi in PSC ai campi corrispondenti in Partner Center

Questa sezione confronta gli screenshot selezionati (o "mappe") mostrati per PSC con la visualizzazione corrispondente nella sezione Partner Center opportunità di co-selling.

In ogni coppia di screenshot verranno visualizzati cerchi numerati, gialli o rossi:

- **Cosa significano i cerchi gialli?** I cerchi gialli numerati vengono visualizzati per primi in ogni schermata PSC. Sarà quindi possibile trovare una schermata Partner Center seguente con molti degli stessi numeri.

   Per vedere come ogni campo o attributo in PSC viene mappato alla controparte in Partner Center, abbinare i cerchi numerati nei due screenshot correlati. Ad esempio, trovare la corrispondenza tra il numero numerato e giallo "1" nel primo screenshot PSC e il numero "1" nel secondo, Partner Center screenshot sottostante.

- **Che cosa significa un cerchio rosso?** Se viene visualizzato un cerchio rosso in uno screenshot, il campo PSC non è disponibile in Partner Center.

I mapping dei Partner Center da PSC a Partner Center per le aree seguenti:

1. PSC home page mappato alla visualizzazione Partner Center predefinita delle opportunità di co-selling
1. Visualizzazione griglia PSC mappata alla visualizzazione Partner Center deal
1. Visualizzazione dettagli trattativa PSC mappata alla Partner Center dettagli dell'offerta
1. Vista Aggiungi prodotti PSC mappata alla Partner Center aggiungi soluzioni
1. Vista di gestione utenti PSC mappata alla Partner Center di gestione utenti
1. Visualizzazione di assegnazione del ruolo utente PSC mappata alla Partner Center di assegnazione di ruolo
1. Visualizzazione notifiche PSC mappata alla visualizzazione Partner Center notifiche

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - PSC home page mappato alla Partner Center predefinita delle opportunità di co-selling

Confrontare i cerchi numerati corrispondenti tra lo screenshot PSC superiore e Partner Center screenshot sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non esiste alcun campo Partner Center corrispondente.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Immagine che mostra i mapping dei campi tra home page di Partner Sales Connect e la visualizzazione predefinita delle opportunità di co-selling in Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - Visualizzazione griglia PSC mappata alla vista Partner Center deal

Confrontare i cerchi numerati corrispondenti tra lo screenshot PSC superiore e Partner Center screenshot sottostante. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non esiste alcun campo Partner Center corrispondente.  

> [!NOTE]
> Altre considerazioni sono riportate sotto gli screenshot.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione griglia Partner Sales Connect (PSC) e la Partner Center della trattativa." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considerazioni speciali:**

- Non esiste alcuna visualizzazione elenco Partner Center come quella di PSC.  Tutte le offerte vengono elencate in base alla data di ricezione o creazione più recente con le informazioni del cliente e il tipo di trattativa. La prima operazione nella visualizzazione è selezionata per impostazione predefinita. La maggior parte dei valori visualizzati nel formato di tabella PSC è disponibile nella visualizzazione dettagli dell'operazione in Partner Center.
- Il ruolo Deal non è un campo obbligatorio in Partner Center. Non viene visualizzato o acquisito in nessuno dei flussi di lavoro. Viene derivato automaticamente dal lato del venditore Microsoft in base alle soluzioni aggiunte all'accordo.
- La data dell'ultima modifica non viene visualizzata nella pagina dei dettagli della segnalazione in Partner Center. I partner possono usare la funzionalità di ordinamento per ordinare le offerte in base alla data dell'ultimo aggiornamento.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - Visualizzazione dettagli trattativa PSC mappata a Partner Center

Confrontare lo screenshot dei cerchi numerati corrispondenti nella parte superiore (PSC) con Partner Center seguente. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non è presente alcun campo o area corrispondente Partner Center.

> [!NOTE]
> Altre considerazioni sono riportate sotto gli screenshot.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione dei dettagli dell'offerta Partner Sales Connect (PSC) e la Partner Center dettagli dell'offerta." lightbox="images/pscmigration/deal-details-expanded.png":::

**Considerazioni speciali:**

- I partner possono modificare un'offerta selezionando il pulsante Modifica nella visualizzazione dettagli dell'offerta partner (6). Dopo aver selezionato il pulsante di modifica, tutti i campi diventano modificabili. È quindi possibile salvare o annullare le modifiche apportate all'operazione.
- Non è possibile chiudere l'operazione come duplicata Partner Center.
- Customer Outcome non è disponibile in Partner Center. Tutti i dettagli relativi alle interazioni con i clienti possono essere aggiornati nella sezione Note in Partner Center.
- La data di chiusura stimata della soluzione è disponibile solo per le offerte IOT OEM Partner Center. Queste informazioni non vengono visualizzate per altri tipi di trattative.
- Il programma di gestione delle licenze non è necessario Partner Center. Queste informazioni vengono dedote automaticamente in base alle soluzioni selezionate nell'accordo.

>[!Note]
>Qualsiasi trattativa contrassegnata come vinta o persa non può essere modificata in seguito. Prestare attenzione durante lo spostamento di un accordo in uno di questi stati terminali.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - Vista "Aggiungi prodotti" PSC mappata alla vista Partner Center 'Aggiungi soluzioni'

Confrontare lo screenshot dei cerchi numerati corrispondenti nella parte superiore (PSC) con Partner Center seguente. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non è presente alcun campo o area corrispondente Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione Aggiungi prodotti partner Sales Connect (PSC) e la visualizzazione Partner Center aggiungi soluzioni." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - Gestione utenti in PSC e Partner Center

Confrontare lo screenshot dei cerchi numerati corrispondenti nella parte superiore (PSC) con Partner Center seguente. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non è presente alcun campo o area corrispondente Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Immagine che mostra i mapping dei campi tra la home page di gestione utenti di Partner Sales Connect (PSC) e la Partner Center pagina Gestione utenti nell'area Impostazioni account."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - Assegnazione di ruolo utente in PSC e Partner Center

Confrontare lo screenshot dei cerchi numerati corrispondenti nella parte superiore (PSC) con Partner Center seguente. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non è presente alcun campo o area corrispondente Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione di assegnazione di ruolo Partner Sales Connect (PSC) e la Partner Center di assegnazione di ruolo." lightbox="images/pscmigration/roles-expanded.png":::

**Considerazioni speciali:**

- Il ruolo equivalente per l'amministratore PSC è il ruolo di amministratore dell'account in Partner Center.
- C'è un solo ruolo in Partner Center per la gestione delle trattative di co-selling. Questo ruolo è il ruolo di amministratore delle segnalazioni.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - Notifiche in PSC rispetto Partner Center

Confrontare lo screenshot dei cerchi numerati corrispondenti nella parte superiore (PSC) con Partner Center seguente. I numeri corrispondenti mostrano dove è possibile trovare la funzionalità o l'attributo correlato a PSC in Partner Center. I cerchi rossi indicano che non è presente alcun campo o area corrispondente Partner Center.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Immagine che mostra il mapping tra le notifiche di Partner Sales Connect (PSC) e la Partner Center delle notifiche."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passaggio da PSC a Partner Center - Domande frequenti

Le sezioni seguenti rispondono a domande frequenti sulla migrazione.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1: cosa è necessario fare se non si ha accesso Partner Center?

È possibile contattare gli amministratori elencati nella pagina "Nessun accesso" per ottenere i ruoli assegnati. Sarà necessario il ruolo [di amministratore delle segnalazioni](permissions-overview.md#manage-referrals) per l'autorizzazione di lettura e scrittura nella sezione delle segnalazioni. Se si gestiscono solo i profili di business, sarà necessario il ruolo di amministratore del profilo business nel Centro per i partner.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Immagine che mostra l'esperienza di nessun accesso Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Chi può concedere l'accesso alla sezione Segnalazioni in Partner Center?

[L'amministratore dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) può concedere l'accesso alla scheda Segnalazioni. Per trovare l'amministratore dell'account, selezionare **Impostazioni account** dall'icona a forma di ingranaggio in alto a destra nel [dashboard Partner Center.](https://partner.microsoft.com/dashboard) Selezionare quindi **Gestione utenti dalla** barra di spostamento a sinistra di secondo livello. Nella parte superiore dell'elenco utenti selezionare il menu a discesa **Filtro** e modificare l'opzione in **Amministratore account**. Nella pagina verranno visualizzati tutti gli amministratori dell'account con i rispettivi indirizzi di posta elettronica. Chiedere a uno di essi di assegnare il ruolo di amministratore delle segnalazioni per l'account aziendale.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - Il pulsante +new deal è in grigio per l'account. Cosa è necessario fare per iniziare a creare offerte?

Ciò si verifica solo se non sono presenti soluzioni pronte per il co-selling collegate all'organizzazione MPN in uso in Partner Center. Contattare il PDM per correggere l'ID MPN delle soluzioni o creare un ticket di supporto che menziona il problema, "Pulsante New Deal (Nuovo contratto) in grigio dopo la migrazione PSC".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - È possibile assegnare offerte a una persona specifica dell'organizzazione, ad esempio PSC?

È possibile assegnare membri del team a un'offerta specifica. Non blocca la visualizzazione o l'azione di altri amministratori delle segnalazioni in base a tali offerte.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - È disponibile una visualizzazione di tutte le offerte assegnate?

È possibile usare la funzionalità Preferiti, che è una scheda a livello di utente. È possibile contrassegnare tutte le trattative assegnate come Preferiti per ottenere un rapido accesso alle trattative.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Esiste una visualizzazione di sola lettura per le trattative?

No, non è disponibile alcuna visualizzazione di sola lettura delle trattative nella sezione delle segnalazioni. Tutti gli amministratori delle segnalazioni avranno accesso completo in lettura e scrittura a tutte le trattative.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Come è possibile registrare un'offerta dopo aver contrassegnato come vinta?

Se l'accordo soddisfa i criteri seguenti, verrà visualizzato un popup per avviare la registrazione [dell'offerta.](./register-deals.md)

- Alla trattativa è associata una soluzione idonea per l'incentivo.
- Il venditore Microsoft è invitato a partecipare all'offerta o l'utente viene invitato all'offerta.
- La scheda Microsoft si trova nello stato Accettato o Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Viene visualizzato un messaggio di errore quando si seleziona il pulsante "+Registrazione del nuovo contratto" nella sezione Registrazione trattativa. Come si registrano le offerte?

Il **pulsante +New deal registration (+New deal registration)** deve essere usato solo dai partner registrati nel programma ISV Connect per la registrazione di un accordo senza alcuna opportunità di co-selling corrispondente in Partner Center. Per registrare le trattative con un'opportunità di co-selling, verrà visualizzato un popup quando l'offerta viene contrassegnata come vinta e se soddisfa i criteri per la registrazione dell'offerta.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - L'aggiunta di un'organizzazione del cliente è obbligatoria?

Sì, l'aggiunta [di un'organizzazione del](./manage-co-sell-opportunities.md#select-your-customer) cliente è obbligatoria Partner Center. Per iniziare, cercare la località in cui si trova il cliente. In base ai dettagli di cui si dispone; è possibile essere specifici, incluso il nome esatto dell'edificio o semplicemente fornire i dettagli della città. La ricerca dell'organizzazione recupererà tutte le persone legali corrispondenti al nome immesso in modo che non sia necessario immettere i dettagli dell'indirizzo. Tutti i dettagli vengono compilati automaticamente in base all'organizzazione selezionata.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - I dettagli di contatto del cliente sono obbligatori?

Dipende dal [tipo di trattativa](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) che si sta creando. Se si condivide solo la pipeline e non è necessario alcun aiuto da parte dell'organizzazione di vendita Microsoft, è possibile scegliere di non fornire i dettagli di contatto del cliente. Se si sta co-selling in cui si sta attivamente cercando aiuto dal venditore Microsoft, è necessario fornire i dettagli di contatto del cliente. È necessario ottenere il consenso esplicito del cliente prima di creare una richiesta di co-selling nel centro per i partner.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Quante soluzioni è possibile aggiungere a un accordo?

È possibile aggiungere fino a 50 soluzioni (analoghe ai "prodotti" in PSC) a un accordo. A differenza di PSC, è possibile combinare soluzioni di soluzioni idonee per il co-selling, SKU microsoft di prima parte e altre soluzioni idonee per il co-selling di terze parti. Non esiste alcun ruolo di trattativa che deve essere selezionato o disponibile nel Centro per i partner. Per gli SKU Microsoft, è possibile aggiungere facoltativamente quantità e prezzo per ogni SKU aggiunto all'offerta.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Quando è possibile conoscere i dettagli del venditore Microsoft dopo aver creato un'offerta?

I venditori Microsoft vengono assegnati solo dopo l'esatta corrispondenza del requisito di assistenza indicato durante la creazione dell'accordo con la persona del venditore pertinente sul lato Microsoft. Anche dopo l'assegnazione, i venditori Microsoft avranno la possibilità di accettare o rifiutare l'invito di co-selling. Solo se un invito di co-selling viene accettato da un venditore, l'offerta verrà aggiornata con i dettagli di contatto del venditore Microsoft. Il contratto di servizio per i venditori Microsoft per l'operazione è di 14 giorni. È lo stesso contratto di servizio che i partner devono agire sull'accordo prima di passarlo allo stato scaduto.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - Dove è possibile trovare l'ID opportunità?

L'ID opportunità in PSC è lo stesso dell'ID dell'Partner Center. È possibile trovare l'ID dell'offerta accanto al nome dell'offerta quando si apre un'offerta.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - Come può il PDM ottenere l'accesso Partner Center?

Partner Center i PDM non possono accedere direttamente a PSC. Sono disponibili più opzioni per abilitare questa funzionalità, come indicato di seguito.

- Informazioni dettagliate OCP: se i PDM visualizzano solo le offerte e lo stato di avanzamento correlati, possono usare il portale informazioni dettagliate di One Commercial Partner (OCP) per visualizzare l'organizzazione. Si tratta di uno strumento interno e disponibile solo per i PDM. Le informazioni dettagliate OCP non sono disponibili per gli utenti dell'azienda.
- Utente guest in Partner Center: è possibile aggiungere l'account PDM come utente guest nel Centro per i partner e assegnargli il ruolo di amministratore delle segnalazioni in modo che possa visualizzare e agire sulle @microsoft.com segnalazioni.
- Creazione [](./create-user-accounts-and-set-permissions.md#add-a-new-user) di un nuovo utente nel tenant: è possibile creare un nuovo utente nel tenant e condividere tali dettagli con PDM in modo che possano visualizzare e agire su segnalazioni simili ad altri utenti di riferimento nell'account.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Ricerca dell'ID MPN corretto se l'account in PSC non è associato a un MPN valido

Se si è qui perché è stato visto un banner in PSC che menziona il problema di associazione dell'ID MPN non valido di PSC, si è nel posto giusto. L'account potrebbe essere stato collegato a un ID MPN non valido per i motivi seguenti

- L'azienda non ha un account Partner Center account.
- Il PDM ha commesso un errore durante l'immissione dell'ID MPN dell'account nei sistemi interni che collegano l'account PSC all'account Partner Center (ID MPN).
- La società non ha completato la migrazione da Partner Membership Center (PMC) a Partner Center.

Per prima cosa, trovare l'ID MPN corretto seguendo questa procedura

- Accedere all'account Partner Center
- Usare le indicazioni fornite nella documentazione relativa alle [impostazioni dell'account](./partner-center-account-setup.md#locate-your-mpn-id) per individuare l'ID MPN.

Di seguito è riportata una schermata che mostra la posizione esatta in cui è possibile trovare l Partner Center ID MPN

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Immagine che mostra le impostazioni dell'account in cui il partner può trovare l'ID MPN."  lightbox="images/pscmigration/findingMPNID.png":::

Successivamente,

- Se si dispone di un PDM, chiedere loro di correggere l'ID MPN con l'ID MPN corretto dall'account del centro per i partner.
- Se non si ha un PDM, inviare un messaggio di posta elettronica all'indirizzo indicato nel banner PSC con le informazioni sull'account PSC visualizzate nel banner PSC e l'ID MPN corretto dall'account del centro per i partner.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Risorse che consentono di creare e gestire le offerte in Partner Center

Se non si sono già letti gli argomenti della Guida sul co-selling, le risorse seguenti consentono di gestire le trattative nel Centro per i partner.

|**Per eseguire questa operazione**   |**Leggi**   |
|-----------------------|:-----------------------|
|Informazioni sulle schede e sulla navigazione nella pagina delle opportunità di co-selling|[Esplorazione della sezione del co-selling](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selezione di un'organizzazione di clienti dall'elenco D&B |[Selezionare il cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modifica dei campi nella sezione dettagli dell'offerta|[Dettagli dell'offerta](./manage-co-sell-opportunities.md#deal-details)|
|Aggiunta dei membri del team a un team di trattative|[Aggiungere i dipendenti](./manage-co-sell-opportunities.md#add-team-members)|
|Risposta a un accordo di co-selling|[Gestire le offerte di co-selling](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registrare le offerte vinte in Partner Center |[Registrare una nuova trattativa](./register-deals.md)
|Ottenere informazioni dettagliate sulle segnalazioni e scoprire come stanno le segnalazioni |[Informazioni dettagliate sulle segnalazioni](./referral-insights.md)
|Creazione e gestione del profilo aziendale|[Gestire profilo di business](./create-a-marketing-profile.md)
|Gestire i lead per il profilo aziendale |[Gestire lead](./manage-leads.md)|

## <a name="next-steps"></a>Passaggi successivi


- [Partner Sales Connect to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) : cartella di lavoro per allineare i processi e i ruoli di vendita dei partner con i nuovi processi di vendita tramite Partner Center e Partner Sales Connect.
- Partner Center guida operativa [per il co-selling:](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) indicazioni per identificare un modello operativo tramite Partner Center per gestire i lead o le opportunità di co-selling e registrare le offerte.
- [Mazzo di gestione delle](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) segnalazioni: istruzioni dettagliate per gestire i lead e le opportunità di co-selling tramite Partner Center.
- [Pubblicazione e gestione nel marketplace](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) commerciale: istruzioni dettagliate per creare, gestire e pubblicare offerte tramite Partner Center nel marketplace commerciale.