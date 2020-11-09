---
title: Eseguire la migrazione da partner Sales Connect (PSC)
description: Scopri in che modo i partner Microsoft possono eseguire la migrazione da partner Sales Connect (PSC) al centro per i partner e creare o gestire le offerte inviate dai venditori Microsoft.
ms.topic: article
author: vikramb
ms.author: vikramb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/06/2020
ms.openlocfilehash: 1f352234f47ea8b2745c649401603f931ec68957
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381432"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guida alla co-selling nel centro per i partner (PC) per i partner che eseguono la migrazione da partner Sales Connect (PSC)

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore degli account
- Amministratore delle segnalazioni
- Venditore partner Sales Connect (PSC)
- Amministratore di partner Sales Connect (PSC)
- Partner Sales Connect (PSC) Deal Manager

Come è noto, l'azienda perderà l'accesso a PSC dopo il 31 marzo 2021. Tuttavia, troverai tutto quello che vuoi fare per creare offerte di co-selling, gestire le tue offerte e agire sulle offerte inviate da Microsoft Sellers all'utente nel centro per i partner. Esistono tuttavia alcune differenze e le linee guida seguenti consentono di eseguire la transizione al centro per i partner più agevole e in modo semplice.

>[!Important]
> Se ci si trova nel punto in cui è stato visualizzato un banner in PSC sulla migrazione, l'utente si trova nel posto giusto. Questa guida non è applicabile per la valutazione della soluzione (SA) e i partner di Internet degli altri OEM che gestiscono le proprie offerte in CPS.

## <a name="before-you-move-things-you-need-to-know"></a>Prima di procedere, è necessario sapere

### <a name="if-you-are-psc-admin"></a>Se si è amministratore di PSC

- Per accedere al centro per i [partner](https://partner.microsoft.com/), è necessario un indirizzo di posta elettronica di lavoro.
- Configurare l'account con il supporto dell' [amministratore dell'account](permissions-overview.md)del centro per i partner.
- Leggere questo documento per informazioni su come co-selling nel centro per i partner.
- Configurare gli account utente nel centro per i partner per tutti gli utenti di PSC (amministratore, Deal Manager e ruoli venditore) e assegnare loro i [ruoli di amministratore di riferimento](permissions-overview.md).

>[!Important]
> Assicurarsi che l'ID MPN visualizzato nel banner del CPS sia disponibile nell'elenco di percorsi MPN nel centro per i partner. Per verificare l'elenco di tutti i MPNs associati all'account del centro per i partner, è possibile verificare che nel centro per i partner si trovino le "Impostazioni account" e "[località](manage-locations.md)".

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Immagine che mostra il banner del CPS in cui i partner possono trovare l'ID MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Se si è responsabile della gestione delle offerte PSC o del venditore

- Per accedere al centro per i [partner](https://partner.microsoft.com/), è necessario un indirizzo di posta elettronica di lavoro.
- Se si usa un account non di lavoro in CPS o l'indirizzo di posta elettronica aziendale è per una società diversa da quella del partner, contattare l'amministratore del CPS per la guida per la configurazione dell'account.
- Rivolgersi all'amministratore di PSC se la configurazione dell'account del centro per i partner è completa indipendentemente dall'account usato per accedere a CPS.
- Verificare se è possibile accedere al centro per i partner e alla sezione dei riferimenti.
- Leggere questo documento per comprendere i flussi di lavoro e le modifiche apportate al centro per i partner.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Come amministratore in PSC, questi sono i passaggi successivi

Se non viene visualizzata la scheda riferimenti:

- L' [amministratore globale](permissions-overview.md) dell'azienda può concedere l'accesso alla scheda riferimenti. Per trovare l'amministratore globale, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Selezionare la pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "Global Admins". La pagina visualizzerà quindi tutti gli amministratori globali con i rispettivi ID di posta elettronica. Contattarli per ottenere l'accesso "referral admin" per l'account aziendale.

  >[!Important]
  > Se il ruolo gestisce solo gli utenti in CPS, è possibile ottenere il ruolo di [amministratore dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) nel centro per i partner. Se il ruolo include anche la gestione di opportunità di co-selling, è necessario ottenere il ruolo di [amministratore dei riferimenti](permissions-overview.md#manage-referrals) . Inoltre, è possibile nominare un responsabile della gestione delle modifiche tra gli amministratori del CPS per collaborare con l'amministratore dell'account del centro per i partner invece che con tutti gli amministratori del CPS che raggiungono gli amministratori dell'account in PC singolarmente.

  :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Immagine che Mostra gli amministratori dell'account nella pagina Gestione utenti delle impostazioni partner.":::

- Passare alla scheda riferimenti nel riquadro di spostamento a sinistra e verificare se è possibile accedere alle pagine.

  >[!Note]
  > Potrebbe essere necessario disconnettersi dal centro per i partner e accedere di nuovo per aggiornare le credenziali per l'accesso alle pagine dei riferimenti.

## <a name="user-migration"></a>Migrazione degli utenti

Dopo aver configurato l'account nel centro per i partner, usare la migrazione guidata utenti nella pagina opportunità di co-selling per assegnare automaticamente i ruoli del centro partner ai dipendenti della società.

>[!Note]
> La migrazione degli utenti può essere eseguita solo dagli [amministratori dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) della società. Se non si ha il ruolo di amministratore dell'account, trovare un amministratore dell'account che consenta di configurare gli account utente con la guida alla migrazione guidata utenti. La funzionalità di migrazione utente sarà disponibile a partire dal 16 novembre 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Immagine che mostra la migrazione guidata utenti.":::

Gli amministratori dell'account otterranno un collegamento alla migrazione guidata utente PSC nella pagina di co-selling Opportunities accanto alla guida dei riferimenti. È possibile avviare la migrazione utente facendo clic sul collegamento. Questa azione può essere eseguita più volte fino a quando tutti gli utenti a cui la società vuole eseguire la migrazione non vengono assegnati ruoli appropriati nel centro per i partner.

La tabella di migrazione utente presenta i dettagli seguenti

- Account utente-ID di posta elettronica del dipendente
- Account partner PSC: l'account a cui è associato il dipendente in PSC
- Ruolo utente PSC: uno dei tre ruoli assegnati a in CPS.
- Percorso MPN del PC: il percorso a cui l'utente riceverà i ruoli del PC pertinenti. L'account partner PSC viene usato per trovare la posizione MPN equivalente nel centro per i partner per l'assegnazione delle autorizzazioni. L'intera organizzazione indica l'ID MPN di vOrg.
- Ruolo utente PC: ai dipendenti vengono assegnati ruoli in base ai rispettivi ruoli utente del CPS. All'amministratore in PSC verranno assegnati i ruoli di amministratore dei riferimenti in PC. Al venditore verrà assegnato il ruolo utente riferimenti in PC. Scopri di più sui ruoli del PC e sui vantaggi che gli utenti con questi ruoli possono eseguire [nel centro per](permissions-overview.md#manage-referrals) i partner
- Tenant di AAD per PC: il tenant a cui gli utenti sono assegnati nel centro per i partner
- Stato: esistono tre possibili stati per lo stato della migrazione
    - Non migrato-l'utente non ha un ruolo di riferimento per i PC assegnati
    - Migrated: l'utente è stato migrato correttamente con il ruolo pertinente assegnato, come illustrato nella tabella
    - Errore-non è possibile completare la migrazione a causa di un errore

La migrazione può avere esito negativo e causare errori in alcune condizioni per le quali le soluzioni sono fornite di seguito

1. È possibile che gli utenti del CPS stiano usando un account non di lavoro.

2. Gli utenti del PSC possono usare un account di un dominio diverso da quello usato nel centro per i partner.

   - Per risolvere gli errori correlati agli scenari 1 e 2, tutti gli utenti devono accedere al centro per i partner usando il proprio account di lavoro collegato al tenant di Azure AD. L' [amministratore globale](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) può essere d'aiuto per questa operazione. Per trovare l'amministratore globale, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Fare clic sulla pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "Global Admins". L'amministratore globale può creare un nuovo account utente nel tenant di Azure AD o assegnare l'accesso utente Guest agli altri utenti dell'account di dominio. Una volta configurati gli account per tutti gli utenti e i responsabili delle operazioni di PSC, è necessario accedere al centro per i partner, passare alla scheda referral nel pannello di navigazione a sinistra e verificare che possano visualizzare la pagina dei riferimenti.

3. All'utente è già assegnato un ruolo di riferimento nel centro per i partner.
    - È possibile verificare il ruolo esistente dell'utente dalla pagina di gestione degli utenti nelle impostazioni dell'account e modificarlo in base alle esigenze.

Dopo aver completato la migrazione degli utenti, usare le linee guida seguenti per decidere la strategia di migrazione: 

Se la società dispone di un PDM-quando l'account del centro per i partner è configurato e gli utenti sono stati spostati e hanno ruoli e autorizzazioni, è possibile spostare le attività di co-selling nel centro per i partner. Informare il PDM per eseguire il compartimento invece di attendere il completamento della scadenza della migrazione, in modo da consentire l'esecuzione di tutte le nuove offerte nel centro per i partner.

>[!Note]
>Una volta eseguito questo passaggio, sarà possibile agire solo sulle operazioni attive esistenti in CPS. Non è possibile creare nuove trattative né ricevere offerte da Microsoft Sellers in PSC.

Se la società non dispone di un PDM, assicurarsi che tutti gli account utente siano configurati e verificati da tutti gli utenti. Si riceverà una notifica tramite un messaggio di posta elettronica e un banner in PSC relativi alla data esatta in cui è possibile avviare la co-selling nel centro per i partner. Tenere presente che sarà comunque necessario gestire le operazioni attive esistenti in CPS.

>[!Important]
>Non verrà eseguita la migrazione delle offerte attive al PC. Fino al 31 dicembre 2020 per chiudere e registrare le offerte.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Passaggi successivi per gli amministratori del CPS, i gestori di Deal e i venditori del PSC

Informazioni su come co-selling nel centro per i partner.
Si tratta di un passaggio importante, che consente di prepararsi per il co-selling nel centro per i partner. Comprendere i flussi di lavoro e le modifiche apportate al centro per i partner, in modo da potervi covendere in modo efficace dal primo giorno. Per iniziare, leggere completamente questo documento. Un set di risorse valido è disponibile anche nella [raccolta di esperienze di co-selling](https://aka.ms/cosellexperience).

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

## <a name="psc-and-partner-center-field-mapping"></a>Mapping dei campi di CPS e del centro per i partner

In questa sezione viene illustrata la mappa esatta degli attributi tra CPS e centro per i partner. Ogni schermata in PSC viene confrontata con la visualizzazione pertinente nella sezione opportunità di co-selling del centro partner. 

>[!Note]
>Per trovare l'attributo equivalente nel centro per i partner, seguire i numeri sulle bolle gialle negli screenshot del CPS. Le bolle rosse indicano che il file archiviato non è disponibile nel centro per i partner.

**Home page di PSC e visualizzazione predefinita delle opportunità di co-selling nel centro per i partner**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Immagine che mostra i mapping dei campi tra il home page di partner Sales Connect e la visualizzazione predefinita di opportunità di co-selling nel centro per i partner.":::

**Visualizzazione griglia PSC e visualizzazione dell'accordo per il centro per i partner**

- Non è disponibile alcuna visualizzazione elenco nel centro per i partner come quello di CPS.  Tutte le offerte sono elencate in base alla data più recente ricevuta o creata con le informazioni sul cliente e il tipo di contratto. Per impostazione predefinita, la prima operazione nella vista è selezionata. La maggior parte dei valori visualizzati nel formato di tabella PSC è disponibile nella visualizzazione dettagli dell'operazione nel computer.
- Il ruolo Deal non è un campo obbligatorio in PC. Non viene né visualizzata né acquisita in nessuno dei flussi di lavoro. Viene derivato automaticamente sul lato venditore Microsoft in base alle soluzioni aggiunte all'affare.
- La data dell'Ultima modifica non viene visualizzata nella pagina dei dettagli del riferimento nel PC. I partner possono usare la funzionalità di ordinamento per ordinare le offerte in base alla data dell'ultimo aggiornamento.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione griglia partner Sales Connect (PSC) e la vista di gestione dei partner Center.":::

**Visualizzazione dei dettagli dell'offerta in CPS e centro per i partner**

- I partner possono modificare un'operazione facendo clic sul pulsante modifica nella visualizzazione dei dettagli del partner Deal (6). Quando si fa clic sul pulsante modifica, tutti i campi diventano modificabili con l'opzione per salvare o annullare le modifiche apportate all'operazione.
- Non è possibile chiudere l'affare come duplicato nel centro per i partner.
- Il risultato del cliente non è disponibile nel centro per i partner. Tutti i dettagli relativi alle interazioni dei clienti possono essere aggiornati nella sezione Note di PC.
- La data di chiusura della soluzione prevista è disponibile solo per le offerte per gli affari OEM nel centro per i partner. Non viene visualizzato per altri tipi di tratteggio.
- Il programma di licenza non è richiesto nel computer. Viene dedotto automaticamente in base alle soluzioni selezionate nell'affare.

>[!Note]
>Eventuali operazioni contrassegnate come vinte o perse non possono essere modificate post. Prestare attenzione quando si trasferisce un problema in uno di questi stati terminali.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione dettagli dell'affare partner Sales Connect (PSC) e la visualizzazione dettagli dell'affare del centro per i partner.":::

**Visualizzazione ' Aggiungi prodotti ' del CPS e la visualizzazione ' Aggiungi soluzioni ' al centro per i partner**

:::image type="content" source="images/pscmigration/products.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione di aggiunta dei prodotti partner Sales Connect (PSC) e la visualizzazione Aggiungi soluzioni per il centro per i partner.":::

**Gestione utenti in CPS e centro per i partner**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Immagine che mostra i mapping dei campi tra la Home page di gestione utenti del partner Sales Connect (PSC) e la gestione utenti del centro per i partner nella visualizzazione impostazioni account.":::

**Assegnazione di ruolo utente in CPS e centro per i partner**

- Il ruolo equivalente per l'amministratore del CPS è il ruolo di amministratore dell'account nel centro per i partner.
- Nel centro per i partner è disponibile un solo ruolo per la gestione delle operazioni di co-selling che rappresenta il ruolo di amministratore di riferimento.

:::image type="content" source="images/pscmigration/roles.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione assegnazione ruolo Partner Sales Connect (PSC) e la visualizzazione assegnazione ruolo centro partner.":::

**Notifiche in CPS e centro per i partner**

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Immagine che mostra il mapping tra le notifiche di partner Sales Connect (PSC) e la visualizzazione notifiche del centro per i partner.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passaggio da CPS al centro per i partner-domande frequenti

**Q1. Quali operazioni è necessario eseguire se non si ha accesso al centro per I partner?**

È possibile contattare gli amministratori elencati nella pagina "nessun accesso" per ottenere i ruoli assegnati. Per le autorizzazioni di lettura e scrittura, è necessario il ruolo "[amministratore di riferimento](permissions-overview.md#manage-referrals)" nella sezione dei riferimenti. Se si gestiscono solo i profili di business, sarà necessario il ruolo "amministratore del profilo di business" nel centro per i partner.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Immagine che mostra l'esperienza di accesso non disponibile nel centro per i partner.":::

**Q2. Chi può concedere l'accesso alla sezione relativa ai riferimenti nel centro per i partner?**

L' [amministratore dell'account](permissions-overview.md#manage-mpn-membership-and-your-company) può concedere l'accesso alla scheda riferimenti. Per trovare l'amministratore dell'account, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Fare clic sulla pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "account Admins". La pagina visualizzerà quindi tutti gli amministratori dell'account con i rispettivi ID di posta elettronica. Contattarli per ottenere l'accesso "referral admin" per l'account aziendale.

**Q3. Il pulsante + nuovo affare è disattivato per l'account. Cosa devo fare per iniziare a creare le offerte?**

Questa situazione si verifica solo se non sono presenti soluzioni di co-selling pronte collegate all'organizzazione MPN in uso nel centro per i partner. Contattare il PDM per ottenere l'ID MPN della soluzione corretta o creare un ticket di supporto che menzioni il problema relativo al pulsante nuovo affare disattivato dopo la migrazione di CPS.

**Q4. È possibile assegnare gli accordi a un utente specifico dell'organizzazione, ad esempio PSC?**

È possibile assegnare i membri del team a un affare specifico. Non impedisce ad altri amministratori di riferimento di visualizzare o agire su tali offerte. 

**Q5. È possibile visualizzare tutte le offerte assegnate all'utente?**

È possibile utilizzare la funzionalità Preferiti, ovvero una scheda livello utente. È possibile contrassegnare tutte le offerte che vengono assegnate come preferiti per ottenere un accesso rapido alle offerte.

**Q6. Esiste una visualizzazione di sola lettura per le offerte?**

No, non è disponibile alcuna visualizzazione di sola lettura delle offerte nella sezione dei riferimenti. Tutti gli amministratori dei riferimenti avranno accesso completo in lettura e scrittura a tutte le offerte.

**Q7. Come è possibile registrare una transazione dopo averla vinta?**

Se il problema soddisfa i criteri indicati di seguito, viene visualizzata una finestra popup per avviare la [registrazione dell'accordo](./register-deals.md).

- Una soluzione idonea per gli incentivi è allegata alla trattativa.
- Il venditore Microsoft è invitato a partecipare all'affare oppure ha invitato l'utente all'affare.
- La scheda Microsoft è nello stato accettato o vinto nel centro per i partner.

**(Domanda 8. Viene ricevuto un messaggio di errore quando si fa clic sul pulsante "+ New Deal Registration" nella sezione relativa alla registrazione dell'accordo. Come è possibile registrare le offerte?**

La registrazione "+ New Deal" deve essere usata solo dai partner registrati nel programma ISV Connect per la registrazione di una trattativa senza opportunità di co-selling corrispondenti nel centro per i partner. Per la registrazione di un'opportunità di co-selling, viene visualizzata una finestra popup quando l'accordo è contrassegnato come vinto e soddisfa i criteri per la registrazione dell'accordo.

**Q9. L'aggiunta di un'organizzazione cliente è obbligatoria?**

Sì, l'aggiunta di un' [organizzazione cliente](./manage-co-sell-opportunities.md#select-your-customer) è obbligatoria nel centro per i partner. Per iniziare, cercare il percorso in cui si trova il cliente. In base ai dettagli disponibili; è possibile essere specifici, tra cui il nome esatto della compilazione, o fornire solo i dettagli della città. La ricerca nell'organizzazione recupererà tutte le entità legali che corrispondono al nome immesso, in modo da non dover immettere i dettagli degli indirizzi. Tutti i dettagli vengono compilati automaticamente in base all'organizzazione selezionata.

**Q10. I dettagli del contatto del cliente sono obbligatori?**

Dipende dal [tipo di problema](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) che si sta creando. Se si sta semplicemente condividendo la pipeline senza richiedere assistenza da parte di Microsoft Sales Organization, è possibile scegliere di non fornire i dettagli di contatto del cliente. Se si sta eseguendo la co-selling in cui si cerca attivamente assistenza da parte del venditore Microsoft, sarà necessario fornire i dettagli di contatto del cliente. Prima di creare una richiesta di co-selling nel centro per i partner, si dovrebbe ottenere il consenso esplicito del cliente.

**Q11. Quante soluzioni è possibile aggiungere a una trattativa?**

È possibile aggiungere fino a un massimo di 50 soluzioni, in modo analogo a "prodotti" in CPS. A differenza di PSC, è possibile combinare soluzioni da soluzioni di co-selling personalizzate, SKU Microsoft e altre soluzioni idonee per la co-selling di terze parti. Non è presente alcun ruolo di gestione che deve essere selezionato o disponibile nel centro per i partner. Per gli SKU Microsoft, è possibile aggiungere facoltativamente la quantità e il prezzo per ogni SKU aggiunto al problema.

**Q12. Quando si riceveranno informazioni dettagliate sui venditori Microsoft dopo la creazione di una trattativa?**

I venditori Microsoft vengono assegnati solo dopo la corrispondenza del requisito esatto della Guida indicato durante la creazione dell'affare con la persona venditore pertinente sul lato Microsoft. Anche dopo l'assegnazione, i venditori Microsoft avranno la possibilità di accettare o rifiutare l'invito al co-selling. Solo se un invito al co-selling viene accettato da un venditore, l'operazione verrà aggiornata con i dettagli di contatto del venditore Microsoft. Il contratto di contratto per i venditori Microsoft che operano sull'accordo è di 14 giorni. Si tratta dello stesso contratto di prezzo che i partner devono agire prima di passare allo stato scaduto.

**Q13. Dove è possibile trovare l'ID opportunità?**

L'ID opportunità in PSC è identico a quello dell'ID dell'accordo in PC. È possibile trovare l'ID dell'affare accanto al nome dell'affare quando si apre qualsiasi affare.

**Q14. In che modo il PDM può accedere al PC?**

Non è possibile accedere direttamente al centro per i partner PDM a differenza di PSC. Sono disponibili più opzioni per abilitare questa funzionalità, come indicato di seguito.

- Informazioni dettagliate su OCP: se PDM sono semplicemente in grado di visualizzare le offerte & stato di avanzamento correlato, possono usare il portale di OCP Insights per ottenere la visualizzazione dell'organizzazione. Si tratta di uno strumento interno ed è disponibile solo per PDM. Si noti che OCP Insights non è disponibile per gli utenti della società.
- Utente guest in centro per i partner: è possibile aggiungere l' @microsoft.com account PDM come utente Guest nel centro per i partner e assegnare loro un ruolo di amministratore in modo che possano visualizzare e agire sui riferimenti.
- Creazione di un [nuovo utente](./create-user-accounts-and-set-permissions.md#add-a-new-user) nel tenant: è possibile creare un nuovo utente nel tenant e condividere i dettagli con il PDM in modo che possano visualizzare i riferimenti e agire su di essi in modo analogo ad altri utenti di riferimento nell'account.

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

Seguire queste risorse aggiuntive:

- [Partner Sales connettersi alla cartella](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) di lavoro del centro per i partner-cartella di lavoro per allineare i processi di vendita e i ruoli dei partner con i nuovi processi di vendita tramite partner Center e partner Sales Connect.
- [Guida alla co-selling del centro](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) per i partner: linee guida per identificare un modello operativo tramite il centro per i partner per gestire i lead o le opportunità di co-selling e registrare le offerte
- [Deck di gestione dei riferimenti](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : istruzioni dettagliate visualizzate per gestire i lead e le opportunità di co-selling tramite il centro per i partner.
- [Pubblicazione e gestione nel Marketplace commerciale](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : istruzioni dettagliate visualizzate per creare, gestire e pubblicare offerte tramite il centro per i partner del Marketplace commerciale.
