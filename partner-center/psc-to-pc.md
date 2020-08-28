---
title: Riferimenti 101 per i partner che eseguono la migrazione da partner Sales Connect (PSC) al centro per i partner (PC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I partner Microsoft qualificati possono co-vendere con Microsoft. Scopri come definire le offerte, invitare Microsoft a collaborare o visualizzare le offerte inviate.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fd58f9e84ce8e1e3dd8d1da39f24614db1da99b5
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/27/2020
ms.locfileid: "89041052"
---
# <a name="referrals-guide-for-managing-your-deals-in-partner-center-instead-of-partner-sales-connect-psc"></a>Guida ai riferimenti per la gestione delle offerte nel centro per i partner invece che in Partner Sales Connect (PSC)

**Si applica a**

- Segnalazioni
- Co-selling con Microsoft
- Configurazione dell'account utente PSC
- Utenti del partner Sales Connect (PSC) 

**Ruoli appropriati**

- Amministratore degli account
- Amministratore delle segnalazioni
- Venditore partner Sales Connect (PSC)
- Amministratore di partner Sales Connect (PSC)
- Partner Sales Connect (PSC) Deal Manager

Come è noto, l'azienda perderà l'accesso a CPS dopo il 31 dicembre 2020. Troverai tutto quello che ti serve per gestire le tue offerte e agire sulle offerte inviate da Microsoft Sellers all'utente nel centro per i partner. Esistono tuttavia alcune differenze e le linee guida seguenti consentono di eseguire la transizione al centro per i partner più agevole e in modo semplice.

## <a name="before-you-move-things-you-need-to-know"></a>Prima di procedere, è necessario sapere

### <a name="if-you-are-psc-admin"></a>Se si è amministratore di PSC

- Per accedere al centro per i [partner](https://partner.microsoft.com/), è necessario un indirizzo di posta elettronica di lavoro.
- Configurare l'account con il supporto dell' [amministratore dell'account](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant)del centro per i partner.
- Leggere questo documento per informazioni su come co-selling nel centro per i partner.
- Configurare gli account di gestione delle offerte e dei venditori di PSC nel centro per i partner e assegnare loro un ruolo di [amministratore di riferimento](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) .

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Se si è responsabile della gestione delle offerte PSC o del venditore

- Per accedere al centro per i [partner](https://partner.microsoft.com/), è necessario un indirizzo di posta elettronica di lavoro.
- Se si usa un account non di lavoro in CPS o un dominio diverso da quello che altri utenti usano in CPS, contattare l'amministratore del CPS per la guida per la configurazione dell'account.
- Rivolgersi all'amministratore di PSC se la configurazione dell'account del centro per i partner è completa indipendentemente dall'account usato per accedere a CPS.
- Verificare se è possibile accedere al centro per i partner e alla sezione dei riferimenti.
- Leggere questo documento per comprendere i flussi di lavoro e le modifiche apportate al centro per i partner.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Come amministratore in PSC, questi sono i passaggi successivi

Se non viene visualizzata la scheda riferimenti:

- L'amministratore dell' [account](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) aziendale può concedere l'accesso alla scheda riferimenti. Per trovare l'amministratore dell'account, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Selezionare la pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "account Admins". La pagina visualizzerà quindi tutti gli amministratori dell'account con i rispettivi ID di posta elettronica. Contattarli per ottenere l'accesso "referral admin" per l'account aziendale.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Immagine che Mostra gli amministratori dell'account nella pagina di gestione degli utenti delle impostazioni di partner.":::

- Passare alla scheda riferimenti nel riquadro di spostamento a sinistra e verificare se è possibile accedere alle pagine.

Dopo aver configurato l'account nel centro per i partner,

- Invitare tutti gli utenti che hanno un ruolo "Deal Manager" o "seller" da CPS al centro per i partner come passaggio successivo.
- L' [amministratore dell'account](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) che ha aiutato l'accesso ai riferimenti può invitare tutti gli utenti.
- Quando si invitano gli utenti, chiedere all'amministratore dell'account di assegnare il ruolo di [amministratore di riferimento](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) .
- Alcuni utenti di PSC potrebbero usare un account non aziendale o un account di un dominio diverso da quello usato nel centro per i partner. Tutti questi utenti devono accedere al centro per i partner usando il proprio account di lavoro collegato al tenant di Azure AD. L' [amministratore globale](https://docs.microsoft.com/partner-center/permissions-overview#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) può essere d'aiuto per questa operazione. Per trovare l'amministratore globale, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Fare clic sulla pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "Global Admins".
- L'amministratore globale può creare un nuovo account utente nel tenant di Azure AD o assegnare l'accesso utente Guest agli altri utenti dell'account di dominio.
- Una volta configurati gli account per tutti gli utenti e i responsabili delle operazioni di PSC, è necessario accedere al centro per i partner, passare alla scheda referral nel pannello di navigazione a sinistra e verificare che possano visualizzare la pagina dei riferimenti.

Se la società dispone di un PDM-quando l'account del centro per i partner è configurato e gli utenti sono stati spostati e hanno ruoli e autorizzazioni, è possibile spostare le attività di co-selling nel centro per i partner. Informare il PDM per eseguire il compartimento, in modo da consentire la propagazione di tutte le nuove offerte al centro per i partner.
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
|Ruoli utente|PSC ha ruoli di amministratore, Deal Manager e seller.|Il computer dispone solo di un ruolo di [amministratore di riferimento](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) che fornisce le autorizzazioni di lettura e scrittura per tutte le offerte.|
|Richiesta di co-selling|Avviato da Microsoft seller, non esiste alcuna domanda esplicita da un partner.|Il partner dovrà effettuare una [richiesta esplicita](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) se è necessaria una guida a Microsoft seller per un'operazione. Microsoft Seller offre un'opzione per rifiutare la richiesta.|
|Expiry|Non esiste alcun concetto di scadenza della trattativa.|Le offerte per i partner in ingresso scadono entro 14 giorni se non vengono accettate dal partner. Lo stesso avviene con le trattative in uscita partner che possono passare allo stato scaduto se il venditore Microsoft non agisce su di essi entro 14 giorni.|
|Dettagli sui venditori Microsoft|Visibile non appena viene creata una trattativa.|I dettagli di Microsoft seller sono condivisi con il partner solo se il venditore accetta in modo esplicito l'invito per il co-selling dal partner.|
|[Pipeline privata](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities)|Non disponibile.|I partner possono condividere la propria pipeline senza fornire visibilità ai venditori Microsoft.|
|Soluzioni|Le soluzioni che appartengono a un solo listino prezzi possono essere aggiunte a un'operazione.|Il partner può aggiungere [soluzioni](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) che appartengono agli elenchi seguenti. a) soluzioni b) dal catalogo delle prime parti Microsoft (ruolo di Deal: transazione in PSC) e c) Co-selling di soluzioni di altri partner di terze parti (ruolo di Deal: ISV in CPS).|
|Assegnazione di Deal|Solo i venditori assegnati possono visualizzare e agire sulle offerte.|I membri del team possono essere aggiunti a una trattativa per specificare gli utenti che lavorano a una trattativa, non vi è alcun blocco di altri amministratori dei riferimenti da visualizzare o agire su tali offerte.|
|Organizzazione del cliente|Immissione di testo in formato libero.|È possibile cercare l' [organizzazione del cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) nel [database D&B](https://www.dnb.com/) semplicemente digitando alcuni caratteri. Il nome e l'indirizzo validi vengono popolati automaticamente in base alla scelta.|
|Contatto del cliente|Non obbligatorio.|Non obbligatorio per la condivisione di pipeline privata. Obbligatorio se il venditore Microsoft è invitato a partecipare a una richiesta di co-selling.|
|API pubblica|Non disponibile.|[API pubblica](https://docs.microsoft.com/partner/develop/referrals) per gestire a livello di codice i riferimenti del centro per i partner.|

## <a name="psc-and-partner-center-field-mapping"></a>Mapping dei campi di CPS e del centro per i partner

Questa sezione consente di comprendere il mapping esatto degli attributi tra CPS e centro per i partner. Ogni schermata in PSC viene confrontata con la visualizzazione pertinente nella sezione opportunità di co-selling del centro partner. 

>[!Note]
>Per trovare l'attributo equivalente nel centro per i partner, seguire i numeri sulle bolle gialle negli screenshot del CPS. Le bolle rosse indicano che il file archiviato non è disponibile nel centro per i partner.

### <a name="home-page-of-psc-and-default-view-of-the-co-sell-opportunities-in-partner-center"></a>Home page di PSC e visualizzazione predefinita delle opportunità di co-selling nel centro per i partner

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Immagine che mostra i mapping dei campi tra il home page di partner Sales Connect e la visualizzazione predefinita di opportunità di co-selling nel centro per i partner.":::

### <a name="psc-grid-view-and-the-partner-center-deal-view"></a>Visualizzazione griglia PSC e visualizzazione dell'accordo per il centro per i partner

- Non è disponibile alcuna visualizzazione elenco nel centro per i partner come quello di CPS.  Tutte le offerte sono elencate in base alla data più recente ricevuta o creata con le informazioni sul cliente e il tipo di contratto. Per impostazione predefinita, la prima operazione nella vista è selezionata. La maggior parte dei valori visualizzati nel formato di tabella PSC è disponibile nella visualizzazione dettagli dell'operazione nel computer.
- Il ruolo Deal non è un campo obbligatorio in PC. Non viene né visualizzato né acquisito in alcun flusso di lavoro. Viene derivato automaticamente sul lato venditore Microsoft in base alle soluzioni aggiunte all'affare.
- La data dell'Ultima modifica non viene visualizzata nella pagina dei dettagli del riferimento nel PC. I partner possono usare la funzionalità di ordinamento per ordinare le offerte in base alla data dell'ultimo aggiornamento.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione griglia partner Sales Connect (PSC) e la vista di gestione dei partner Center.":::

### <a name="deal-details-view-in-psc-and-partner-center"></a>Visualizzazione dei dettagli dell'offerta in CPS e centro per i partner

- I partner possono modificare un'operazione facendo clic sul pulsante modifica nella visualizzazione dei dettagli del partner Deal (6). Quando si fa clic sul pulsante modifica, tutti i campi diventano modificabili con l'opzione per salvare o annullare le modifiche apportate all'operazione.
- Non è possibile chiudere l'affare come duplicato nel centro per i partner.
- Il risultato del cliente non è disponibile nel centro per i partner. Tutti i dettagli relativi alle interazioni dei clienti possono essere aggiornati nella sezione Note di PC.
- La data di chiusura della soluzione stimata è disponibile solo per gli OEM. Non viene visualizzato per altri tipi di tratteggio.
- Il programma di licenza non è richiesto nel computer. Viene dedotto automaticamente in base alle soluzioni selezionate nell'affare.

>[!Note]
>Eventuali operazioni contrassegnate come vinte o perse non possono essere modificate post. Prestare attenzione quando si trasferisce un problema in uno di questi stati terminali.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione dettagli dell'affare partner Sales Connect (PSC) e la visualizzazione dettagli dell'affare del centro per i partner.":::

### <a name="psc-add-products-view-and-the-partner-center-add-solutions-view"></a>Visualizzazione di aggiunta dei prodotti di CPS e della visualizzazione Aggiungi soluzioni al centro per i partner

 :::image type="content" source="images/pscmigration/products.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione di aggiunta dei prodotti partner Sales Connect (PSC) e la visualizzazione Aggiungi soluzioni per il centro per i partner.":::

### <a name="user-management-in-psc-and-partner-center"></a>Gestione utenti in CPS e centro per i partner

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Immagine che mostra i mapping dei campi tra la Home page di gestione utenti del partner Sales Connect (PSC) e la gestione utenti del centro per i partner nella visualizzazione impostazioni account.":::

### <a name="user-role-assignment-in-psc-and-partner-center"></a>Assegnazione di ruolo utente in CPS e centro per i partner

- Il ruolo equivalente per l'amministratore del CPS è il ruolo di amministratore dell'account nel centro per i partner.
- Nel centro per i partner è disponibile un solo ruolo per la gestione delle operazioni di co-selling che rappresenta il ruolo di amministratore di riferimento.
- A tutti i responsabili delle operazioni e ai venditori in PSC deve essere assegnato il ruolo di amministratore di riferimento.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Immagine che mostra i mapping dei campi tra la visualizzazione assegnazione ruolo Partner Sales Connect (PSC) e la visualizzazione assegnazione ruolo centro partner.":::

### <a name="notifications-in-psc-and-partner-center"></a>Notifiche in CPS e centro per i partner

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Immagine che mostra il mapping tra le notifiche di partner Sales Connect (PSC) e la visualizzazione notifiche del centro per i partner.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Passaggio da CPS al centro per i partner-domande frequenti

### <a name="q-what-should-i-do-if-i-dont-have-access-to-partner-center"></a>Q. Quali operazioni è necessario eseguire se non si ha accesso al centro per I partner?

È possibile contattare gli amministratori elencati nella pagina "nessun accesso" per ottenere i ruoli assegnati. https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals)Per l'autorizzazione di lettura e scrittura nella sezione relativa ai riferimenti è necessario disporre di "[referral admin] ((" Role per l'autorizzazione di lettura e scrittura. Se si gestiscono solo i profili di business, sarà necessario il ruolo "amministratore del profilo di business" nel centro per i partner.

### <a name="q-who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>Q. Chi può concedere l'accesso alla sezione relativa ai riferimenti nel centro per i partner?

L' [amministratore dell'account](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) può concedere l'accesso alla scheda riferimenti. Per trovare l'amministratore dell'account, passare a impostazioni partner dall'icona a forma di ingranaggio nella parte superiore destra del centro per i partner. Fare clic sulla pagina Gestione utenti nel secondo livello della barra di spostamento a sinistra. Fare clic sull'elenco a discesa che mostra "tutti gli utenti" nella parte superiore destra della pagina e passare a "account Admins". La pagina visualizzerà quindi tutti gli amministratori dell'account con i rispettivi ID di posta elettronica. Contattarli per ottenere l'accesso "referral admin" per l'account aziendale.

### <a name="q-the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>Q. Il pulsante + nuovo affare è disattivato per l'account. Cosa devo fare per iniziare a creare le offerte?

Questa situazione si verifica solo se non sono presenti soluzioni di co-selling pronte collegate all'organizzazione MPN in uso nel centro per i partner. Contattare il PDM per ottenere l'ID MPN della soluzione corretta o creare un ticket di supporto che menzioni il problema relativo al pulsante nuovo affare disattivato dopo la migrazione di CPS.

### <a name="q-can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>Q. È possibile assegnare gli accordi a un utente specifico dell'organizzazione, ad esempio PSC?

È possibile assegnare i membri del team a un affare specifico. Non impedisce ad altri amministratori di riferimento di visualizzare o agire su tali offerte. 

### <a name="q-is-there-a-view-of-all-the-deals-assigned-to-me"></a>Q. È possibile visualizzare tutte le offerte assegnate all'utente?

È possibile utilizzare la funzionalità Preferiti, ovvero una scheda livello utente. È possibile contrassegnare tutte le offerte che vengono assegnate come preferiti per ottenere un accesso rapido alle offerte.

### <a name="q-is-there-a-read-only-view-for-the-deals"></a>Q. Esiste una visualizzazione di sola lettura per le offerte?

No, non è disponibile alcuna visualizzazione di sola lettura delle offerte nella sezione dei riferimenti. Tutti gli amministratori dei riferimenti avranno accesso completo in lettura e scrittura a tutte le offerte.

### <a name="q-how-can-i-register-a-deal-after-making-it-as-won"></a>Q. Come è possibile registrare una transazione dopo averla vinta?

Se il problema soddisfa i criteri indicati di seguito, viene visualizzata una finestra popup per avviare la [registrazione dell'accordo](https://docs.microsoft.com/partner-center/register-deals).

- Una soluzione idonea per gli incentivi è allegata alla trattativa.
- Il venditore Microsoft è invitato a partecipare all'affare oppure ha invitato l'utente all'affare.
- La scheda Microsoft è nello stato accettato o vinto nel centro per i partner.

### <a name="q-i-get-an-error-message-when-i-click-on-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>Q. Viene ricevuto un messaggio di errore quando si fa clic sul pulsante "+ New Deal Registration" nella sezione relativa alla registrazione dell'accordo. Come è possibile registrare le offerte?

La registrazione "+ New Deal" deve essere usata solo dai partner registrati nel programma ISV Connect per la registrazione di una trattativa senza opportunità di co-selling corrispondenti nel centro per i partner. Per la registrazione di un'opportunità di co-selling, viene visualizzata una finestra popup quando l'accordo è contrassegnato come vinto e soddisfa i criteri per la registrazione dell'accordo.

### <a name="q-is-adding-a-customer-organization-mandatory"></a>Q. L'aggiunta di un'organizzazione cliente è obbligatoria?

Sì, l'aggiunta di un' [organizzazione cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) è obbligatoria nel centro per i partner. Per iniziare, cercare il percorso in cui si trova il cliente. In base ai dettagli disponibili; è possibile essere specifici, tra cui il nome esatto della compilazione, o fornire solo i dettagli della città. La ricerca nell'organizzazione recupererà tutte le entità legali che corrispondono al nome immesso, in modo da non dover immettere i dettagli degli indirizzi. Tutti i dettagli vengono compilati automaticamente in base all'organizzazione selezionata.

### <a name="q-are-customer-contact-details-mandatory"></a>Q. I dettagli del contatto del cliente sono obbligatori?

Dipende dal [tipo di problema](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities) che si sta creando. Se si sta semplicemente condividendo la pipeline senza richiedere assistenza da parte di Microsoft Sales Organization, è possibile scegliere di non fornire i dettagli di contatto del cliente. Se si sta eseguendo la co-selling in cui si cerca attivamente assistenza da parte del venditore Microsoft, sarà necessario fornire i dettagli di contatto del cliente. Prima di creare una richiesta di co-selling nel centro per i partner, si dovrebbe ottenere il consenso esplicito del cliente.

### <a name="q-how-many-solutions-can-i-add-to-a-deal"></a>Q. Quante soluzioni è possibile aggiungere a una trattativa?

È possibile aggiungere fino a un massimo di 50 soluzioni (prodotti in PSC) a una trattativa. A differenza di PSC, è possibile combinare soluzioni da soluzioni di co-selling personalizzate, SKU Microsoft e altre soluzioni idonee per la co-selling di terze parti. Non è presente alcun ruolo di gestione che deve essere selezionato o disponibile nel centro per i partner. Per gli SKU Microsoft, è possibile aggiungere facoltativamente la quantità e il prezzo per ogni SKU aggiunto al problema.

### <a name="q-when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>Q. Quando si riceveranno informazioni dettagliate sui venditori Microsoft dopo la creazione di una trattativa?

I venditori Microsoft vengono assegnati solo dopo la corrispondenza del requisito esatto della Guida indicato durante la creazione dell'affare con la persona venditore pertinente sul lato Microsoft. Anche dopo l'assegnazione, i venditori Microsoft avranno la possibilità di accettare o rifiutare l'invito al co-selling. Solo se un invito al co-selling viene accettato da un venditore, l'operazione verrà aggiornata con i dettagli di contatto del venditore Microsoft. Il contratto di contratto per i venditori Microsoft che operano sull'accordo è di 14 giorni. Si tratta dello stesso contratto di prezzo che i partner devono agire prima di passare allo stato scaduto.

### <a name="q-where-can-i-find-the-opportunity-id"></a>Q. Dove è possibile trovare l'ID opportunità?

L'ID opportunità in PSC è identico a quello dell'ID dell'accordo in PC. È possibile trovare l'ID dell'affare accanto al nome dell'affare quando si apre qualsiasi affare.

### <a name="q-how-can-my-pdm-get-access-to-pc"></a>Q. In che modo il PDM può accedere al PC?

Non è possibile accedere direttamente al centro per i partner PDM a differenza di PSC. Sono disponibili più opzioni per abilitare questa funzionalità, come indicato di seguito.

- Informazioni dettagliate su OCP: se PDM sono semplicemente in grado di visualizzare le offerte & stato di avanzamento correlato, possono usare il portale di OCP Insights per ottenere la visualizzazione dell'organizzazione. Si tratta di uno strumento interno ed è disponibile solo per PDM e per gli utenti.
- Utente guest in centro per i partner: è possibile aggiungere l' @microsoft.com account PDM come utente Guest nel centro per i partner e assegnare loro un ruolo di amministratore in modo che possano visualizzare e agire sui riferimenti.
- Creazione di un [nuovo utente](https://docs.microsoft.com/partner-center/create-user-accounts-and-set-permissions#add-a-new-user) nel tenant: è possibile creare un nuovo utente nel tenant e condividere i dettagli con il PDM in modo che possano visualizzare i riferimenti e agire su di essi in modo analogo ad altri utenti di riferimento nell'account.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Risorse che consentono di creare e gestire le proprie offerte nel centro per i partner

Se non sono stati ancora letti gli argomenti della Guida di co-selling, le risorse seguenti consentiranno di gestire le offerte nel centro per i partner.

|**Per eseguire questa operazione**   |**Leggi**   |
|-----------------------|:-----------------------|
|Informazioni sulle schede e sulla navigazione nella pagina opportunità di co-selling|[Esplorazione della sezione di co-selling](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#navigating-the-co-sell-section)|
|Selezione di un'organizzazione cliente dall'elenco D&B |[Selezionare il cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)|
|Modifica dei campi nella sezione dettagli sull'accordo|[Dettagli sull'offerta](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#deal-details)|
|Aggiunta dei dipendenti della società a un team di gestione|[Aggiungere i dipendenti](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-your-employees)|
|Risposta a un affare di co-selling|[Gestisci le offerte di co-selling](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#responding-to-a-co-sell-opportunity)
|Registra le offerte acquisite nel centro per i partner |[Registrare una nuova trattativa](https://docs.microsoft.com/partner-center/register-deals)
|Ottieni informazioni dettagliate sul riferimento e Scopri come fanno i tuoi riferimenti |[Informazioni dettagliate sulle segnalazioni](https://docs.microsoft.com/partner-center/referral-insights)
|Creazione e gestione del profilo di business|[Gestire profilo di business](https://docs.microsoft.com/partner-center/create-a-marketing-profile)
|Gestisci lead per il tuo profilo business |[Gestire lead](https://docs.microsoft.com/partner-center/manage-leads)|

## <a name="additional-resources"></a>Risorse aggiuntive

- [Partner Sales connettersi alla cartella](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) di lavoro del centro per i partner-cartella di lavoro per allineare i processi di vendita e i ruoli dei partner con i nuovi processi di vendita tramite partner Center e partner Sales Connect.
- [Guida alla co-selling del centro](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) per i partner: linee guida per identificare un modello operativo tramite il centro per i partner per gestire i lead o le opportunità di co-selling e registrare le offerte
- [Deck di gestione dei riferimenti](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : istruzioni dettagliate visualizzate per gestire i lead e le opportunità di co-selling tramite il centro per i partner.
- [Pubblicazione e gestione nel Marketplace commerciale](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : istruzioni dettagliate visualizzate per creare, gestire e pubblicare offerte tramite il centro per i partner del Marketplace commerciale.
