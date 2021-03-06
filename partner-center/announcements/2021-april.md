---
title: Annunci di aprile 2021
description: Annunci di aprile 2021 per Microsoft Partner Center nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150132"
---
# <a name="april-2021-announcements"></a>Annunci di aprile 2021

Questa pagina fornisce gli annunci per Microsoft Partner Center per aprile 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Conformità: aggiornamento dell'API di convalida dell'indirizzo del cliente CSP in corso di validità a giugno; Funzionalità di test ora disponibile

### <a name="categories"></a>Categorie

- Data: 2021-04-30
- Preparazione

### <a name="summary"></a>Riepilogo

Per consentire a partner e clienti di eseguire la propria attività in base alla fiducia, invitiamo i partner a testare le modifiche apportate all'API Convalida indirizzo per tutti i paesi di tutto il mondo.

### <a name="impacted-audience"></a>Destinatari interessati

Partner di fatturazione diretta CSP e provider indiretti che creano nuovi o aggiornano i dettagli dell'indirizzo dei clienti esistenti

### <a name="details"></a>Dettagli

Microsoft Microsoft si impegna a fornire un metodo conforme, sicuro e sicuro per la convalida degli indirizzi dei clienti per la transazione delle sottoscrizioni dei clienti nel programma CSP. A partire dal 31 marzo 2021 sono state introdotte modifiche all'API Convalida indirizzo. I partner sono invitati a testare l'API prima del go-live alla fine di giugno 2021. 

Si noti che queste modifiche influiscono solo sull'API Convalida indirizzo. Le API Crea cliente e Aggiorna profilo di fatturazione non sono interessate. Anche se l'indirizzo suggerito non deve attualmente essere usato con l'API Crea cliente, è altamente consigliato.

La risposta restituirà uno dei messaggi di stato seguenti:

| Stato     | Descrizione |    Numero di indirizzi suggeriti restituiti |
|-------|---------------|-------------------|
|Shippable verificato | L'indirizzo viene verificato e può essere spedito. | Single |
|Verified | L'indirizzo viene verificato. | Single |
|Interazione richiesta | L'indirizzo suggerito è stato modificato in modo significativo e richiede la conferma dell'utente. | Single |
|Via parziale | La via specificata nell'indirizzo è parziale e richiede altre informazioni. | Multiplo: massimo tre |
|Locale parziale | I locali (numero di edificio, numero di suite e altri) sono parziali e necessitano di altre informazioni. | Multiplo: massimo tre |
|Multipli | Esistono più campi che sono parziali nell'indirizzo (potenzialmente includendo anche parziale strada e parziale locale). | Multiplo: massimo tre |
|Nessuno | L'indirizzo non è corretto. | Nessuno |
|Non convalidato | Impossibile inviare l'indirizzo tramite il processo di convalida. | Nessuno |

I codici postali degli Stati Uniti restituiranno altre quattro cifre + trattino, ad esempio 12345-6789.

### <a name="next-steps"></a>Passaggi successivi

- Per indicazioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella raccolta [partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dedicata.
- Prepararsi a incorporare le modifiche usando l'API Partner Center e l'esperienza utente Web. 
- Condividere l'ID tenant della sandbox con l'esperto in materia (Ali Kpiki) da includere nel test, in modo da poter iniziare la preparazione per l'aggiornamento. 
- Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.

### <a name="questions"></a>Domande?

Se è necessario supporto per le operazioni con Microsoft, contattare il gruppo yammer di supporto partner o aprire una richiesta [di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nuova posizione per la Partner Center di Swagger dell'API

### <a name="categories"></a>Categorie

- Data: 26/04/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

Partner Center dei documenti Swagger dell'API sono stati migrati dal sito della [documentazione di Swagger](https://apidocs.microsoft.com/services/partnercenter) precedente a un [nuovo sito della documentazione di Swagger.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Destinatari interessati

Partner con fatturazione diretta e provider indiretti che partecipano al programma Cloud Solution Provider (CSP) che usano Partner Center API

### <a name="details"></a>Dettagli

A partire dal 26 aprile 2021 la documentazione di Swagger dell'API Partner Center, incluso il contenuto dell'API Rest, si trova in un [nuovo sito.](/rest/api/partner-center-rest/) Il sito precedente sarà inaccessibile dopo diverse settimane.

### <a name="benefits"></a>Vantaggi

La documentazione Partner Center'API Swagger fornirà una **funzione Try It.** Per usare questa funzione, è necessario disporre di un token di bearer, che è possibile generare seguendo i passaggi elencati in Partner Center [Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni all'interno dell'organizzazione in modo che il team appropriato possa esaminare e aggiornare i processi.

### <a name="questions"></a>Domande?

Per domande su queste offerte, controllare le community Yammer pertinenti.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Cloud Solution Provider criteri del periodo di restituzione software (CSP) e avviso di scadenza del collegamento di download

### <a name="categories"></a>Categorie

- Data: 2021-04-21
- Funzionalità

### <a name="summary"></a>Riepilogo

Sono state apportate modifiche ai criteri del periodo di restituzione del software CSP e alla scadenza del collegamento di download.

### <a name="impacted-audience"></a>Destinatari interessati

Partner che eselezionano offerte di sottoscrizione software o software perpetue in CSP

### <a name="details"></a>Dettagli

Si notino le notifiche importanti seguenti relative agli acquisti di sottoscrizioni software e software perpetue tramite Partner Center:

#### <a name="software-return-period-policy"></a>Criteri del periodo di restituzione software

A partire dal 1° giugno 2021, il periodo di restituzione delle offerte software in CSP, come indicato nel Contratto Microsoft Partner (MPA), cambierà da 60 giorni dalla data dell'ordine a 30 giorni dalla data dell'ordine.

Dopo l'invio di un ordine per un'offerta software, i partner avranno 30 giorni dalla data dell'ordine per inviare eventuali revisioni a tale ordine:

- Qualsiasi licenza software perpetua restituita entro il periodo di restituzione di 30 giorni riceverà un credito completo del prezzo di acquisto a pagamento.

- Qualsiasi prodotto di sottoscrizione software restituito entro il periodo di restituzione di 30 giorni riceverà un credito prorato del prezzo di acquisto a pagamento.

Questo messaggio è un follow-up delle comunicazioni di posta elettronica inviate il dicembre 2020 e aprile 2021 a tutti i partner CSP relativi al periodo di restituzione e ad altri aggiornamenti all'MPA. Fare riferimento a tali avvisi per informazioni dettagliate complete sulle modifiche che interessano l'MPA.

#### <a name="software-download-link-expiry"></a>Scadenza del collegamento di download software

A partire dal 3 giugno 2021, i collegamenti di download software per gli acquisti di prodotti in sottoscrizione software e software perpetui tramite Partner Center avranno una data di scadenza di cinque giorni dal download iniziale. Il periodo di scadenza verrà applicato a tutti gli acquisti prima del 3 giugno 2021, nonché il 3 giugno 2021 o dopo il 3 giugno 2021.

### <a name="next-steps"></a>Passaggi successivi

Esaminare il [periodo di restituzione CSP e le domande frequenti](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)sulla scadenza del collegamento di download e informare tutti i team appropriati all'interno dell'organizzazione delle modifiche seguenti:

### <a name="questions"></a>Domande?

Per domande su queste offerte, controllare le community Yammer pertinenti.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Programma open licensing: transizione dei rivenditori al programma Cloud Solution Provider (CSP)

### <a name="categories"></a>Categorie

- Data: 2021-04-19
- Far crescere l'azienda

### <a name="summary"></a>Riepilogo

Questa comunicazione illustra in dettaglio come prepararsi per le modifiche che saranno presto disponibili nel programma Open Licensing.

### <a name="impacted-audience"></a>Destinatari interessati

Partner CSP e Open License

### <a name="details"></a>Dettagli

Nel 2020 [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) ha annunciato che le licenze software perpetue saranno disponibili a livello generale per partner e clienti tramite il programma Cloud Solution Provider (CSP). La prima attività cardine è stata raggiunta nel gennaio 2021, quando sono disponibili offerte software perpetue commerciali. L'attività cardine successiva si avrà a luglio 2021, quando saranno disponibili [le](https://aka.ms/openlicensepublicsector) offerte del settore pubblico. È [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) stato anche comunicato che a partire dal 1° gennaio 2022 non è possibile effettuare nuovi acquisti o rinnovi di licenze software di Software Assurance o Servizi online tramite il programma Open License.

La transizione del software perpetuo al programma CSP nella nuova esperienza commerciale aiuterà i partner ad espandere le opportunità di offrire soluzioni e servizi gestiti diversi. Ciò accelererà anche la transizione dei clienti al cloud.  Per garantire una transizione senza problemi sia per i partner che per i clienti, sono stati apportati questi adattamenti e materiali per accelerare questa trasformazione digitale:

#### <a name="april-2021"></a>Aprile 2021

[Ora disponibile:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Materiali di transizione Open License-to-CSP per rivenditori

#### <a name="july-2021"></a>Luglio 2021

##### <a name="csp"></a>CSP

- 1° luglio: licenze software perpetue disponibili per i clienti del settore pubblico

- 7 luglio: Visual Studio licenze software perpetue pro e get genuine del Contratto Windows disponibili per tutti i segmenti

##### <a name="open-value"></a>Apri valore

- 1 luglio: SKU aggiuntivi disponibili nel programma Open Value per la formazione e le organizzazioni no profit, offrendo offerte simili al programma Open License

##### <a name="open-license"></a>Open License

- 1 luglio: Microsoft non avvierà più nuove offerte nel programma Open License.

#### <a name="january-2022"></a>Gennaio 2022

- 1 gennaio: non è possibile effettuare nuovi acquisti o rinnovi tramite il programma Open License

### <a name="next-steps"></a>Passaggi successivi

#### <a name="csp-indirect-providers"></a>Provider indiretti CSP

Usare i prossimi mesi per aiutare i rivenditori Open License a orientarsi nel programma CSP partecipando agli eventi della community dei partner e usando i materiali di transizione Open License-to-CSP per i rivenditori:

- Open [License-to-CSP transition](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)materials for resellers (Materiale per la transizione da licenza a CSP aperta per i rivenditori): presentazione panoramica personalizzabile, modello di posta elettronica, guida all'onboarding dei rivenditori indiretti CSP e altro ancora per facilitare l'adozione per i rivenditori su larga scala.

- [Eventi della community dei partner CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) ospitati da Microsoft Business Operations.  Partecipare alle varie sessioni per apprendere le nozioni di base di CSP (Nozioni fondamentali su CSP) o rimanere aggiornati e porre domande relative al software in CSP (Q&A Sessions).

- (Presto disponibili) Sessione di formazione incentrata sui rivenditori indiretti CSP ospitata da Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Rivenditori Open License

- Se l'organizzazione non è attualmente iscritta al programma CSP, contattare il distributore per informazioni su come iniziare. Connettersi con un provider indiretto [qui](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).

- Se l'organizzazione è già iscritta al programma CSP, vedere qui per altre informazioni sul software perpetuo in [CSP.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Domande?

Per altre domande su queste offerte, vedere le community Yammer pertinenti.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Now live: Global promo readiness guide (Guida all'idoneità per le promo globali)

### <a name="categories"></a>Categorie

- Data: 16/04/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

Launch Readiness ha pubblicato una nuova [guida all'idoneità per la promo globale](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) nella raccolta di risorse per l'idoneità per le operazioni. Questa guida offre una visualizzazione consolidata di tutte le [promozioni globali attive.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner volume licensing (VL), Dynamics Price List (DPL) e Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

I partner Microsoft hanno condiviso con Microsoft la necessità di fornire una visualizzazione consolidata di tutte le promozioni globali con i dettagli di supporto. Si desiderava che questa guida consolidata aiuta a usare le promozioni con la certezza che tutte le informazioni disponibili saranno facilmente accessibili in una posizione centrale e comoda.

A partire da aprile 2021, Microsoft aggiornerà questa guida su base mensile e sarà disponibile in una raccolta di guide alla preparazione della terapia globale dedicata nella raccolta di risorse preparazione operazioni.

I collegamenti a questa guida verranno inclusi anche nelle raccolte seguenti:

- [Avviare la raccolta di](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)calendari , che offre una visualizzazione centralizzata delle modifiche e dei lanci imminenti.

- [Raccolte della](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)community, che contengono materiale di supporto per le chiamate mensili dei partner, evidenziando le modifiche imminenti e gli argomenti di interesse operativo.

- [Newsletter per i partner,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)ad esempio l'aggiornamento mensile CSP

Come promemoria mensile, pubblicheremo anche un annuncio Partner Center con ogni nuovo numero della guida alla preparazione della descrizione globale.

### <a name="next-steps"></a>Passaggi successivi

All'inizio di ogni mese, è possibile trovare la guida più recente alla preparazione [delle promo](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globali nella raccolta di risorse [di Conformità alle operazioni](https://partner.microsoft.com/resources).

Condividere queste informazioni con i contatti appropriati all'interno dell'organizzazione e indicarci quanto sia utile la guida tramite il messaggio "Questa pagina è stata utile?" alla fine di ogni pagina.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Aggiornamento e promemoria della community di Cloud Solution Provider (CSP) di aprile

### <a name="categories"></a>Categorie

- Data: 2021-04-16
- Community | Inviti e promemoria

### <a name="summary"></a>Riepilogo

Le risorse della community CSP sono disponibili su richiesta e aggiornate mensilmente per tenervi informati e preparati per il cambiamento nel programma CSP.

### <a name="impacted-audience"></a>Destinatari interessati

Partner di fatturazione diretta CSP e provider indiretti

### <a name="details"></a>Dettagli

Questo mese, le risorse includono gli argomenti chiave seguenti:

- [Aggiornamento all'evoluzione del programma CSP e modifiche al programma Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Modifiche ai requisiti di onboarding dei clienti CSP in determinate aree](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nuovo formato per la nuova fattura pdf commerciale nel programma CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

[All'interno della raccolta della community CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)sono presenti:

- La newsletter di aggiornamento mensile [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)scaricabile, che aggrega annunci, aggiornamenti, eventi e promemoria CSP recenti in un documento di facile lettura.

- Calendario [degli annunci CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)che offre una visualizzazione temporale delle modifiche imminenti che interessano il programma.

- Il nuovo [calendario di lancio del](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)prodotto, in cui è possibile visualizzare i prossimi lanci di prodotti e offerte.

- [Il provider di servizi di configurazione avvia le](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) risorse di aggiornamento con contenuti facili da usare in base alle principali modifiche operative.

- [Aggiornamenti e promemoria su](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) argomenti CSP chiave che ricevono interesse e query.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

Sono disponibili&domande frequenti sulla chiamata della community per rispondere alle domande relative alle modifiche imminenti. Registrarsi ora per il programma CSP Community Call Q&che si stanno verificando nei mesi di aprile, maggio e giugno. Queste informazioni saranno incentrate sui lanci più recenti, sugli aggiornamenti importanti e sui promemoria.

[Registrarsi qui](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse della community e registrarsi per la chiamata alla community Q&A.

Per ottenere il massimo dalla chiamata alla community Q&A, esaminare il contenuto della community su richiesta e inviare le domande fino a 48 ore prima della chiamata.

### <a name="questions"></a>Domande?

Il piano mensile CSP Community Call Q&A è il posto migliore per le domande relative alle modifiche apportate al programma CSP. Ogni mese esaminare il materiale e inviare le domande in anticipo in modo da poter dedicare la sessione agli argomenti più importanti per l'utente.

Per altre informazioni, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Promemoria finale: Deprecazione della qualificazione GET il 6 maggio 2021

### <a name="categories"></a>Categorie

- Data: 04/05/2021

- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Partner che vendono offerte Academic, No profit e Government Community Cloud (GCC) tramite il programma Cloud Solution Provider usando l'API Partner Center

### <a name="details"></a>Dettagli

Questo annuncio è un follow-up delle Partner Center [miglioramenti rilasciati a dicembre.](./2020-december.md#1) Come parte di tale versione, sono state distribuite nuove API di qualifica GET e POST e, di conseguenza, la qualifica GET esistente verrà ritirata il 6 maggio **2021.** A questo punto, sarà necessario eseguire la transizione all'uso del nuovo POST Partner Center API. Le nuove API POST consentono di acquistare offerte Education, mentre le nuove API GET consentono di acquistare offerte non profit e GCC pre-qualificate.

### <a name="next-steps"></a>Passaggi successivi

- **Eseguire l'aggiornamento alle nuove API per** una transizione corretta e temporale.

- **Esaminare le nuove modifiche Partner Center'API** e la Guida nelle risorse conformità alle operazioni: Partner Center miglioramenti del processo di convalida dei clienti [di Education.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

- Condividere queste informazioni con i team appropriati all'interno dell'organizzazione e con i rivenditori per prepararsi a queste modifiche.

### <a name="questions"></a>Domande?

Per eventuali domande correlate a questa notifica, contattare il [supporto Partner Center .](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Registro delle modifiche

- 4 maggio 2021: promemoria finale dell'imminente deprecazione della qualifica GET

- 9 aprile 2021: promemoria dell'imminente deprecazione della qualifica GET 

- Febbraio: sono state aggiornate le sequenze temporali per la deprecazione delle & PUT GET

- Gennaio: promemoria delle prossime deprecazioni delle & PUT GET

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nuovo formato per la nuova fattura PDF commerciale in CSP

### <a name="categories"></a>Categorie

- Data: 2021-04-05
- Funzionalità

### <a name="summary"></a>Riepilogo

Microsoft sta introducendo un nuovo formato per la nuova fattura PDF commerciale nel programma Cloud Solution Provider (CSP) per visualizzare i dettagli di fatturazione in base ai dettagli del prodotto anziché alla descrizione dello SKU.

### <a name="impacted-audience"></a>Destinatari interessati

Partner che eseguono transazioni tramite il programma CSP

### <a name="details"></a>Dettagli

A partire da maggio 2021, Microsoft introduce un nuovo formato per la nuova fattura PDF commerciale nel programma CSP per visualizzare i dettagli di fatturazione in base ai dettagli del prodotto anziché alla descrizione dello SKU. Con questo nuovo aggiornamento, le voci verranno aggregate per tipo di prodotto, visualizzando ogni prodotto in una singola riga.

I partner noteranno che questa modifica sarà effettiva nella fattura di maggio per il periodo di fatturazione compreso tra il 1° aprile 2021 e il 30 aprile 2021. Le offerte interessate sono Microsoft Azure,sottoscrizioni di Azure (piano di Azure) e Marketplace.

Tutte le richieste di nuova fattura effettuate dopo l'aggiornamento del formato della fattura verranno generate nel nuovo formato.

#### <a name="partner-benefits"></a>Vantaggi per i partner

Questo aggiornamento offrirà i miglioramenti seguenti all'esperienza di fatturazione per i partner:

- Riduzione delle dimensioni della fattura mantenendo i dati critici

- Allineamento del formato agli standard del settore per le fatture compatte e di facile utilizzo 

Gli elementi seguenti non saranno interessati:

- Pagina di riepilogo della fatturazione nel PDF della fattura

- API di fatturazione esistenti

- File di riconciliazione (i file di riconciliazione possono essere usati per il recupero di dati granulari). 

- Fatture per l'utilizzo e gli addebiti basati su licenza

### <a name="next-steps"></a>Passaggi successivi

Esaminare le informazioni su questo argomento nella raccolta di risorse [per l'idoneità per le](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) operazioni nel sito Web dei partner Microsoft. Per altre informazioni su fatturazione e imposte, tra cui risorse di fatturazione, fatture, fatturazione CSP e imposte, vedere la sezione [Fatturazione](../billing.md) in Partner Center.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Modifiche apportate ai requisiti di onboarding dei clienti Cloud Solution Provider (CSP)

### <a name="categories"></a>Categorie

- Data: 02/04/2021
- Offerte/mercati

### <a name="summary"></a>Riepilogo

Nell'ambito dell'impegno per aiutare partner e clienti a eseguire la propria attività in base alla fiducia, microsoft richiederà informazioni aggiuntive sui clienti a partire dal 25 marzo 2021.

### <a name="impacted-audience"></a>Destinatari interessati

I provider indiretti e i partner con fatturazione diretta CSP con clienti nuovi o esistenti nei paesi elencati nella sezione successiva

### <a name="details"></a>Dettagli

Microsoft si impegna a fornire un metodo di convalida dei clienti conforme e sicuro per la vendita di sottoscrizioni cliente nel programma CSP. Il 25 marzo 2021 verranno introdotti miglioramenti all'API Partner Center e all'interfaccia utente che influiranno sui partner che soddisfano entrambi i criteri seguenti:

- Il partner ha una relazione di fatturazione diretta con Microsoft (ovvero, è un partner con fatturazione diretta o un provider indiretto).

- Il partner opera con clienti nuovi o esistenti nei paesi seguenti:

    - Thailandia
    - Vietnam
    - Turchia
    - Polonia
    - Sud Africa
    - India
    - Brasile
    - Iraq
    - Myanmar
    - Sud Sudan
    - Arabia Saudita
    - Emirati Arabi Uniti
    - Venezuela

I partner che soddisfano i criteri doranno inviare l'ID registrazione aziendale di un cliente (noto anche come INN dell'organizzazione del cliente) e il numero di telefono al successivo aggiornamento o creazione di una sottoscrizione per tale cliente. I partner possono anche immettere un secondo nome facoltativo per il cliente.

Si noti che quando si aggiunge l'ID registrazione aziendale, è necessario usare l'ID imposta aziendale e non l'ID personale del cliente.

I partner che svolgono attività con clienti nuovi o esistenti nei paesi seguenti hanno già eseguito l'onboarding di una versione precedente a novembre 2020.

- Armenia
- Azerbaigian
- Bielorussia
- Ungheria
- Kazakhstan
- Kirghizistan
- Moldova
- Russia
- Tagikistan
- Ucraina
- Uzbekistan

I partner con clienti nel resto del mondo avranno la possibilità di immettere l'ID di registrazione della società, il numero di telefono e il secondo nome per i clienti come dettagli facoltativi.

### <a name="next-steps"></a>Passaggi successivi

- Per istruzioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella [raccolta dedicata ai partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).
- Prepararsi ad adottare le modifiche usando l'API del Centro per i partner e l'esperienza utente Web. Saranno disponibili API e SDK a scopo di test.
- Assicurarsi di inviare i dati aggiuntivi quando si caricano nuovi clienti o si modificano i dettagli del cliente esistente.
- Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.

### <a name="questions"></a>Domande?

Contattare l'assistente fiscale o l'ufficio fiscale locale per eventuali domande relative all'ID di registrazione dell'azienda (detto anche INN o TIN). Microsoft non è in grado di fornire indicazioni sulle imposte.

Se è necessario supporto per le operazioni con Microsoft, aprire una richiesta [di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Visualizzare i lanci e le offerte del prodotto di questo mese

### <a name="categories"></a>Categorie

- Data: 2021-04-01
- Funzionalità
 
### <a name="summary"></a>Riepilogo

Il calendario di lancio del prodotto di aprile 2021 è ora pubblicato.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Il calendario di lancio del prodotto [di](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) aprile 2021 è ora disponibile nella raccolta di risorse conformità alle operazioni. Vedere i prossimi lanci e offerte del prodotto qui.

### <a name="next-steps"></a>Passaggi successivi

Esaminare il [calendario di lancio del](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)prodotto e condividere le informazioni con gli stakeholder appropriati nell'organizzazione.  

### <a name="questions"></a>Domande?

Per altre domande su queste offerte, vedere le community Yammer pertinenti.