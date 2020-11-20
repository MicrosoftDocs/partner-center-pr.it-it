---
title: Annunci di novembre 2020
description: Annunci di novembre 2020 relativi al Centro per i partner Microsoft comprendenti nuovi mercati e nuove funzionalità, promozioni, offerte o modifiche a offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691300"
---
# <a name="november-2020-announcements"></a>Annunci di novembre 2020

Questa pagina illustra in dettaglio gli annunci per il Centro per i partner Microsoft di novembre 2020.

Annunci 2020: [Aprile](2020-april.md) | [Maggio](2020-may.md) | [Giugno](2020-june.md) | [Luglio](2020-july.md) | [Agosto](2020-august.md) | [Settembre](2020-september.md) | [Ottobre](2020-October.md) | Novembre

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>Modifica della valuta di fatturazione dei partner per le nuove offerte commerciali nell'area UE/EFTA.  

### <a name="categories"></a>Categorie
- Data: 17/11/2020
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati  

Partner che eseguono transazioni tramite il programma Cloud Solution Provider nell'area geografica UE/EFTA 

### <a name="summary"></a>Riepilogo 

Nell'area geografica UE/EFTA, tutte le nuove offerte commerciali del programma Cloud Solution Provider useranno la località di fatturazione del partner invece della località di fatturazione del cliente. Ciò significa che i partner saranno fatturati da Microsoft in base alla valuta della località di appartenenza, non alla valuta della località dei clienti. Questa operazione verrà eseguita in due fasi: 

- **Fase 1: Nuovi clienti che acquistano una nuova offerta commerciale in CSP**

A partire da gennaio 2021, i partner che hanno nuovi clienti che acquistano nuove offerte commerciali saranno fatturati per tali acquisti nella valuta della località del partner. I partner con clienti esistenti che hanno già acquistato nuove offerte commerciali in CSP continueranno a essere fatturati in base alla valuta della località di fatturazione del cliente durante questa fase. 

 

- **Fase 2: Clienti esistenti che hanno acquistato una nuova offerta commerciale in CSP prima di gennaio 2021** 

Dopo la fase 1 e durante l'anno 2021, Microsoft eseguirà la transizione della fatturazione delle nuove offerte commerciali per i partner con clienti esistenti che hanno acquistato una nuova offerta commerciale in CSP prima di gennaio 2021, dalla valuta della località del cliente alla valuta della località del partner. I partner riceveranno una notifica prima dell'implementazione di questa modifica.  

>[Nota] Questa modifica influirà solo sulla valuta di fatturazione dei partner e non sui prezzi delle nuove offerte commerciali in CSP. 

Le nuove offerte commerciali interessate da questa modifica sono: sottoscrizioni di Azure che fanno parte di un piano di Azure, prenotazioni di Azure, sottoscrizioni server, software con licenza perpetua e acquisti del marketplace commerciale Microsoft nel programma Cloud Solution Provider.

### <a name="partner-benefits"></a>Vantaggi per i partner  

- Questo aggiornamento ridurrà la complessità e il sovraccarico della fatturazione a più valute nell'area geografica UE/EFTA per la nuova esperienza commerciale.  

- I partner riceveranno una fattura consolidata in una singola valuta e non più una fattura per ogni valuta della località del cliente. 

- I pagamenti di incentivi saranno nella stessa valuta specificata nella fattura del partner.

- I partner noteranno una riduzione della complessità nella procedura di fatturazione dovuta alla fatturazione a più valute. Ciò consentirà di risparmiare tempo e risorse attualmente associate a riconciliare gli account. 

- Per i partner che non hanno ancora adottato le nuove offerte commerciali, questa modifica è allineata al precedente modello di fatturazione del partner, che consente ai partner di passare più facilmente alla nuova esperienza commerciale in CSP. 

### <a name="resources"></a>Risorse 

Vedere le informazioni relative a questo argomento nella [raccolta delle operazioni](https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ del sito Web dei partner Microsoft.  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>Limitazione delle richieste per le API ai partner che chiamano le API del Centro per i partner

### <a name="categories"></a>Categorie

- Data: 17/11/2020
- Funzionalità

### <a name="summary"></a>Riepilogo

Microsoft introduce la limitazione delle richieste per le API ai partner che chiamano le API del Centro per i partner per migliorare le prestazioni in un determinato intervallo di tempo.

### <a name="impacted-audience"></a>Destinatari interessati

Partner che eseguono transazioni tramite il programma Cloud Solution Provider

### <a name="details"></a>Dettagli

Microsoft implementerà la limitazione delle richieste per le API nel primo trimestre del 2021 per garantire prestazioni più coerenti in un intervallo di tempo per i partner che chiamano le API del Centro per i partner. La limitazione delle richieste limita il numero di richieste a un servizio entro un determinato intervallo di tempo per evitare l'utilizzo eccessivo delle risorse. Quando viene superata una soglia di limitazione delle richieste, il Centro per i partner limiterà eventuali altre richieste del client per un determinato periodo di tempo.  

### <a name="partner-benefits"></a>Vantaggi per i partner 

Il Centro per i partner è progettato per gestire un volume elevato di richieste, ma se un numero eccessivo di richieste viene effettuato da pochi partner, la limitazione delle richieste consentirà di mantenere le prestazioni e l'affidabilità a un livello ottimale per tutti i partner. Garantisce tempi di inattività minimi. Riducendo il volume elevato di richieste, è possibile garantire prestazioni coerenti per tutti i partner. 


### <a name="apis-to-be-throttled"></a>API soggette alla limitazione delle richieste

|**Operazione**|**Documentazione sul Centro per i partner**|
|-------------------------|----------------------------------|
|{baseURL}/v1/customers/{customer_id}/subscriptions|[Ottenere tutte le sottoscrizioni di un cliente](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[Ottenere un abbonamento in base all'ID](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/customers/{customer_id}/orders||[Ottenere tutti gli ordini di un cliente](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}|[Ottenere un ordine in base all'ID](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus|[Ottenere lo stato del provisioning di un abbonamento](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[Gestire gli ordini e gestire una sottoscrizione](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons|[Ottenere un elenco dei componenti aggiuntivi per un abbonamento](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements|[Ottenere un elenco dei diritti di Azure per una sottoscrizione](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus|[Ottenere lo stato della registrazione di un abbonamento](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/customers/{customer-tenant-id}/transfers|[Ottenere tutti i trasferimenti di un cliente](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{upgrade-id}/status|[Ottenere lo stato di aggiornamento dei prodotti](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions|[Ottenere un elenco delle offerte di conversione della copia di valutazione](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

Questo annuncio intende fornire ai partner una conoscenza tempestiva delle modifiche previste, consentendo loro di prepararsi a gestirle. Si consiglia ai partner di acquisire familiarità con queste API e prendere in considerazione l'uso dell'API del log attività per una maggiore efficienza ed evitare la limitazione delle richieste. Per altre informazioni su questa funzionalità, fare riferimento ai dettagli in [Indicazioni sulla limitazione delle richieste per le API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance). 

### <a name="next-steps"></a>Passaggi successivi

Esaminare [Indicazioni sulla limitazione delle richieste per le API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance) ed eseguire le operazioni necessarie. 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>Errori 409 dovuti a richieste MCA duplicate

### <a name="categories"></a>Categorie

- Data: 16/11/2020
- Funzionalità

### <a name="context"></a>Context

- Nel febbraio di quest'anno ai partner è stato richiesto di firmare il Contratto del cliente Microsoft (MCuA). Si trattava di una migrazione dal precedente Contratto Microsoft Cloud (MCA). 
- Nell'ambito di questa modifica, è stato richiesto ai partner di includere il parametro del tipo di contratto come documentato [qui](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement).

### <a name="what-happened-next"></a>Sviluppi successivi:

- Non tutti i partner hanno incluso il parametro richiesto nell'implementazione. Microsoft ha restituito il Contratto Microsoft Cloud a questi partner.
- Il partner ha quindi inviato nuovamente la richiesta di firma al cliente e il Contratto Microsoft Cloud a Microsoft. 
- La duplicazione ha influito sulla capacità di Microsoft di fornire assistenza ai partner.
- A settembre 2020 è stata inviata una notifica ai partner, tramite Yammer in più forum, richiedendo ai partner di correggere il parametro. Microsoft non potrà più accettare i duplicati e i partner riceveranno errori 409.

>[Nota] Non si tratta di una nuova modifica del contratto/dell'API per i partner.

- Nel mese di ottobre Microsoft ha lavorato a stretto contatto con i partner che hanno avuto il maggior numero di richieste duplicate per risolvere il problema.
- Attualmente, vengono inviati promemoria ai partner e messaggi di posta elettronica personali ai primi 10 trasgressori, affinché possano esaminare le richieste e contattare Microsoft per testare e risolvere il problema.
- Il 10 novembre 2020 è stata interrotta l'accettazione dei duplicati e i partner che non avevano corretto i parametri hanno riscontrato errori 409.
- Successivamente, la modifica relativa al rifiuto dei duplicati è stata annullata. 
- Il 14 gennaio 2021, tuttavia, i duplicati non saranno più accettati. In questo modo, i partner avranno a disposizione più tempo per apportare le modifiche necessarie. È già stata ricevuta una notifica da parte di un partner che prevede di distribuire un aggiornamento il 16/11 per il quale si collaborerà a stretto contatto.
- È importante che i partner contattino Microsoft per ricevere assistenza nel testing, in modo che i loro tenant possano essere aggiunti a un pacchetto in anteprima con le modifiche e possano garantire che l'aggiornamento della soluzione funzioni come previsto.



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>Test disponibile: aggiornamenti delle API e miglioramenti dell'interfaccia utente (UI) del Centro per i partner per il processo di convalida dei clienti del settore della formazione

### <a name="categories"></a>Categorie

- Data: 10/11/2020
- Funzionalità |Sviluppo dell'efficienza e della scalabilità

### <a name="impacted-audience"></a>Destinatari interessati

Partner che vendono offerte per il settore accademico tramite il programma Cloud Solution Provider (CSP).

### <a name="summary"></a>Riepilogo

È ora disponibile il test per gli aggiornamenti delle API e i miglioramenti dell'interfaccia utente del Centro per i partner per il processo di convalida dei clienti del settore della formazione.

### <a name="details"></a>Dettagli

Microsoft si impegna a fornire un metodo di convalida dei clienti conforme e sicuro per la vendita di offerte per il settore accademico nel programma CSP. Nell'ambito di questo impegno, verranno introdotti miglioramenti all'interfaccia utente e all'API del Centro per i partner nel secondo trimestre dell'anno fiscale 2021 (FY21 Q2). Questi miglioramenti aggiungeranno chiarezza e visibilità nel processo di convalida dei clienti e offriranno la possibilità di inserire dati più accurati, in modo da migliorare la convalida dei clienti.

**Miglioramenti del Centro per i partner**

- Nuove API di qualifica GET e POST per supportare l'inserimento preciso dei dati e migliorare il processo di convalida dei clienti del settore della formazione da parte di Microsoft.

- Miglioramenti dell'interfaccia utente per supportare l'inserimento preciso dei dati e ottimizzare il processo di convalida dei clienti del settore della formazione da parte di Microsoft.

Test

Per una migliore comprensione delle API e dell'inserimento dei dati necessari per la corretta convalida dei clienti, i partner avranno la possibilità di testare questi miglioramenti a partire dal mese di ottobre 2020. A breve verranno fornite altre informazioni sulla tempistica esatta e sulle modalità di partecipazione. Le API esistenti del Centro per i partner verranno ritirate prima della fine del secondo trimestre dell'anno fiscale 2021 (FY21 Q2). A quel punto, sarà necessario eseguire la transizione alle nuove API del Centro per i partner.

   - Disponibilità dei test Le date dei test per i partner sono comprese tra il 2 ottobre e il 2 dicembre 2020. I partner che intendono partecipare dovranno scaricare la guida ai test per i clienti del settore della formazione del Centro per i partner in cui troveranno informazioni su come prepararsi, come iscriversi e cosa aspettarsi durante la fase di test.

**Clienti del settore biblioteche e musei**

Oltre a questi miglioramenti, Microsoft è lieta di annunciare che, nel secondo trimestre dell'anno fiscale 2021 (FY21 Q2), verranno abilitate offerte con gli stessi prezzi del settore della formazione per biblioteche e musei, espandendo così i clienti del settore della formazione a cui sarà possibile vendere offerte CSP.

Microsoft si riserva il diritto di esaminare lo stato di qualsiasi cliente effettivo o potenziale per verificarne i requisiti di utente del settore della formazione. Per informazioni dettagliate, vedere i [requisiti dell'utente qualificato del settore della formazione](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7).

## <a name="next-steps"></a>Passaggi successivi

Esaminare le modifiche apportate all'interfaccia utente e all'API del Centro per i partner e leggere la guida ai test nella [raccolta di contenuti sui miglioramenti apportati al processo di convalida dei clienti del settore della formazione nel Centro per i partner](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

• Iscriversi per partecipare ai test (vedere la [guida ai test](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) per informazioni dettagliate). 

• Verificare che l'organizzazione conosca i [requisiti dell'utente qualificato del settore della formazione](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7). 

• Condividere queste informazioni con i team appropriati all'interno dell'organizzazione e con i rivenditori per aiutarli nella preparazione in vista di queste modifiche.



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>Espansione dei contenuti per i partner con licenze commerciali nella raccolta per l'idoneità operativa

### <a name="categories"></a>Categorie

- Data: 05/11/2020
- Funzionalità

### <a name="summary"></a>Riepilogo

A partire dal 5 novembre 2020, i contenuti per i partner con licenze commerciali di Partner University saranno disponibili anche nella raccolta per l'idoneità operativa.

### <a name="impacted-audience"></a>Destinatari interessati

Partner commerciali

### <a name="details"></a>Dettagli

A partire dal 5 novembre 2020, i contenuti per i partner con licenze commerciali di Partner University saranno disponibili anche nella raccolta per l'idoneità operativa. In questo modo, i contenuti relativi al lancio per i partner con licenze operative e commerciali, già esistenti nella raccolta per l'idoneità operativa, verranno uniti ai contenuti consolidati per i partner con licenze commerciali di Partner University. I partner potranno così usufruire di un'esperienza di formazione più uniforme. Alla raccolta per l'idoneità operativa sono stati aggiunti i contenuti seguenti:

- [Microsoft Azure - Offers and Licensing](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [Commercial Licensing - CSP Spotlight Call](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [Commercial Licensing - Licensing Updates Call](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>Passaggi successivi

Si consiglia di condividere queste informazioni con tutti i contatti appropriati nella propria organizzazione.

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5"></a>Lancio dello SKU Premium di Microsoft Teams Rooms

### <a name="categories"></a>Categorie

- Data: 03/11/2020
- Offerte/mercati

### <a name="summary"></a>Riepilogo

Lo SKU Premium di Microsoft Teams Rooms per Microsoft Teams tramite il programma Cloud Solution Provider (CSP) è ora disponibile.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Il nuovo SKU Premium di Microsoft Teams Rooms per Microsoft Teams è ora disponibile per i clienti che acquistano CSP tramite l'utente a 50 USD al mese per ogni dispositivo. Lo SKU Premium di Microsoft Team Rooms è un'alternativa allo SKU Standard di Microsoft Teams Room (in precedenza denominato licenza Sala riunioni). Questo SKU include tutti gli elementi dell'offerta standard, ad esempio le licenze necessarie per Microsoft Teams, Skype for Business Online e la gestione di Intune. L'offerta consente anche di abilitare Sistema telefonico, necessario per l'integrazione della rete PSTN (Public Switched Telephone Network), e Audioconferenza, se disponibile. 

Con l'offerta premium, i clienti possono accedere a Servizi gestiti di Microsoft Team Rooms appena rilasciato, in cui la gestione e le operazioni relative alle sale riunioni vengono gestite da esperti per conto del cliente. Questo servizio di gestione e monitoraggio IT basato sul cloud consente di mantenere aggiornati e sicuri i dispositivi Microsoft Teams Rooms e le relative periferiche. Consente inoltre di monitorare e gestire questi dispositivi in modo proattivo, mantenendo l'ambiente ottimizzato per un'esperienza in sala di elevata qualità.

#### <a name="released-at-launch"></a>Rilasciate all'avvio

   |****|**Microsoft Teams Rooms Standard 15 USD al mese per dispositivo**|**Microsoft Teams Rooms Premium 50 USD al mese per dispositivo**|
   |-------------------|:------|:------|
   |Skype for Business|Sì| |
   |Microsoft Teams|Sì|Sì|
   |Sistema telefonico|Sì|Sì|
   |Audioconferenza|Sì|Sì|
   |Microsoft Intune|Sì|Sì|
   | |Microsoft Teams Rooms Standard 15 USD al mese per dispositivo|Microsoft Teams Rooms Premium 50 USD al mese per dispositivo|
   |Servizi gestiti di Microsoft Teams Rooms| |Sì|
   |Disponibilità a livello mondiale|Sì|In alcuni mercati|

#### <a name="microsoft-teams-rooms-managed-services"></a>Servizi gestiti di Microsoft Teams Rooms

- Gestione proattiva: gestione delle sale riunioni 24x7x365, incluse l'applicazione di patch, la gestione della configurazione e altro ancora.
•   Monitoraggio in tempo reale e analisi della causa radice: monitoraggio e rilevamento con risposta orchestrata di gestione degli incidenti eseguita da Microsoft in stretto coordinamento con il cliente, se necessario. L'app per dispositivi mobili consente di essere avvisati anche quando si è fuori ufficio.
- Aggiornamenti gestiti: gestione e distribuzione di aggiornamenti dell'applicazione, di KB di Windows e del firmware.
- Protezione dalle minacce alla sicurezza: protezione dalle possibili minacce alla sicurezza con Microsoft Defender Advanced Threat Protection.
- Supporto tecnico: supporto tecnico 24x7x365 tramite centro operativo dedicato con correzione assistita degli incidenti per i casi non automatizzati. Controllo dettagliato degli accessi in base al ruolo.
- Informazioni dettagliate e raccomandazioni: informazioni dettagliate aggregate per i vari clienti e report relativi allo stato delle sale, alle scorte, al consumo, alle riunioni online e alle tendenze degli incidenti.

#### <a name="offer-details"></a>Dettagli dell'offerta

   |**Nome offerta**|**ID offerta**|**ID materiale**|
   |-------------------|:------|:------|
   |Teams Rooms Premium|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Teams Rooms Premium (Stati Uniti e Canada)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Teams Rooms Premium per docenti|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>Passaggi successivi

- Consultare le [domande frequenti]() per acquisire familiarità con la nuova offerta e la relativa disponibilità geografica.
- Acquisire familiarità con la nuova offerta e la relativa disponibilità geografica. 
- Visitare il sito Web all'indirizzo [rooms.microsoft.com](https://rooms.microsoft.com/) per altre informazioni su Microsoft Rooms e sulle offerte correlate.
- Usare la [guida per i partner di Teams](https://aka.ms/teamscallingmeetingsguide) per sviluppare la pratica con le sale riunioni di Teams e creare un'offerta pronta per il co-selling.
- Leggere le [domande frequenti su Microsoft Teams Rooms](https://aka.ms/PartnerMTRFAQ) per altre informazioni sul prodotto e sui servizi. 
- Condividere queste informazioni con tutti i contatti appropriati all'interno dell'organizzazione e comprendere le opportunità di upselling e cross-selling.

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>Nuovi SKU di Comunicazioni avanzate di Microsoft Teams per Government Community Cloud (GCC) presto disponibili

### <a name="categories"></a>Categorie

- Data: 2-11-2020
- Offerte/mercati

### <a name="summary"></a>Riepilogo

Il nuovo SKU aggiuntivo di Comunicazioni avanzate per Microsoft Teams in GCC sarà disponibile dal 1° dicembre 2020.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Il nuovo componente aggiuntivo Comunicazioni avanzate per Microsoft Teams in GCC è ora disponibile a 12 USD per utente al mese. È possibile acquistare gli SKU dei componenti aggiuntivi per qualsiasi altra suite Microsoft 365 che contiene Microsoft Teams. Comunicazioni avanzate fornisce un nuovo set di funzionalità per riunioni con un elevato numero di partecipanti, criteri di comunicazione, integrazioni e strumenti avanzati per la gestione IT. 

#### <a name="offer-details"></a>Dettagli dell'offerta

   |**Nome offerta**|**ID offerta**|**ID materiale**|
   |-------------------|:------|:------|
   |Comunicazioni avanzate per GCC|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>Domande frequenti 

**Cosa sono le comunicazioni avanzate?** Questo nuovo componente aggiuntivo di Microsoft Teams consente ai clienti di migliorare ulteriormente l'esperienza di comunicazione. Può essere acquistato in aggiunta a qualsiasi SKU di Microsoft 365 a cui è stata effettuata la sottoscrizione.

**Quanto costa?** Il prezzo stimato al dettaglio commerciale è di 12 USD per utente al mese.

**Quali clienti possono acquistare il componente aggiuntivo?** Il componente aggiuntivo può essere acquistato dai clienti GCC.

**Come è possibile acquistare l'offerta?** È possibile acquistare il componente aggiuntivo tramite Enterprise Agreement, Enterprise Agreement Subscription, Enrollment for Education Solutions, CSP o Web Direct.

**Dove è possibile vendere l'offerta?** È possibile venderla nei mercati statunitensi.

**Quali sono i prerequisiti?** Qualsiasi suite Microsoft 365 o Office 365 con Microsoft Teams può includere questo componente aggiuntivo.

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni con i contatti pertinenti nell'organizzazione e comprendere le opportunità di upselling e cross-selling. Vedere la sezione relativa alle risorse della [guida per i partner di Teams](https://aka.ms/teamscallingmeetingsguide).

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365: nuovi prodotti e offerte lanciati di recente e presto disponibili

### <a name="categories"></a>Categorie

- Data: 2-11-2020
- Offerte/mercati

### <a name="impacted-audience"></a>Destinatari interessati

Provider diretti, provider indiretti e rivenditori indiretti

### <a name="details"></a>Dettagli

#### <a name="new-offers"></a>Nuove offerte

Il 1° novembre 2020 Microsoft ha rilasciato le offerte di Dynamics 365 Project Operations e ha rimosso Dynamics 365 Project Service Automation (PSA) per i clienti commerciali. Questa comunicazione fornisce informazioni aggiuntive sul mapping dei diritti di doppio utilizzo dal lancio e sulle nuove offerte incorporate di fornitori di software indipendenti (ISV).

#### <a name="project-operations-isv-embed-offers"></a>Offerte incorporate ISV di Project Operations

Il 1° novembre 2020 Microsoft ha rilasciato altre tre offerte incorporate ISV della durata di 36 mesi per Dynamics 365 per Project Operations a clienti di Cloud Solution Provider (CSP). Per i dettagli degli SKU, vedere la scheda Project Operations nel [documento di Excel relativo alle offerte CSP per Dynamics di novembre 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls).

#### <a name="project-operations-dual-use-rights-mapping"></a>Mapping dei diritti di doppio utilizzo di Project Operations

Per informazioni sul mapping locale dei diritti di doppio utilizzo di Dynamics 365 per le offerte di Project Operations, vedere la tabella seguente:

   |**Offerta di D365 Operations**|**Mapping locale dei diritti di doppio utilizzo di D365**|
   |-------------------|:------|
   |Offerta di D365 Operations|Mapping locale dei diritti di doppio utilizzo di D365|
   |D365 Project Operations|D365 per Operations, sistema locale (Server AX) con SKU Dyn365 Project Operations (109108477)|
   |D365 Project Operations Attach|D365 per Operations, sistema locale (Server AX) con SKU Dyn365 Project Operations (109108477)|
   |D365 Finance con Project Operations|D365 per Operations, sistema locale (Server AX) con SKU Dyn365 Project Operations (109108477)|
   |D365 Finance Attach con Project Operations|D365 per Operations, sistema locale (Server AX) con SKU Dyn365 Project Operations (109108477)|
   |D365 Unified Operations - Attività con Project Operations|D365 per Operations, sistema locale (Server AX) con SKU Dyn365 Project Operations (109108477)|

#### <a name="previously-announced"></a>Annunciato in precedenza

Il 1° novembre 2020 Microsoft ha rilasciato i prodotti e le offerte di Dynamics 365 e Power Platform nuovi e aggiornati indicati di seguito per CSP:

- Dynamics 365 Customer Voice USL 

Per i dettagli degli ID delle offerte, vedere la scheda Project Operations nel [documento di Excel relativo alle offerte CSP per Dynamics di novembre 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls).

Per accedere ad altre risorse, vedere la home page di Microsoft Dynamics 365 Customer Voice.

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni con le persone appropriate all'interno dell'organizzazione.

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>Introduzione a Microsoft 365 Business Voice per organizzazioni no profit

### <a name="categories"></a>Categorie

- Data: 2-11-2020
- Offerte/mercati

### <a name="summary"></a>Riepilogo

Il 1° novembre 2020 Microsoft ha presentato nuovi SKU per Microsoft 365 Business Voice per le organizzazioni no profit.

### <a name="impacted-audience"></a>Destinatari interessati

Provider diretti, provider indiretti e rivenditori indiretti

### <a name="details"></a>Dettagli

Il 1° novembre 2020 Microsoft ha presentato nuovi SKU per Business Voice. La suite completa è disponibile in Canada, Regno Unito e Stati Uniti. Business Voice senza piano per chiamate sarà disponibile in tutti gli altri mercati. 

Microsoft 365 Business Voice è un sistema telefonico basato sul cloud per aziende di piccole e medie dimensioni che integrano Office 365. Con l'aggiunta di Business Voice alla sottoscrizione di Office 365 di un cliente è possibile offrire una soluzione di comunicazione e collaborazione all-in-one, che combina chiamate, chat e riunioni in un'unica applicazione, Microsoft Teams.

Per informazioni dettagliate sui prezzi, vedere il listino prezzi.

È possibile aggiungere Microsoft 365 Business Voice alle sottoscrizioni seguenti per un massimo di 300 utenti:

- Office 365: Business Essentials, Business Premium, A1, E1, A3 ed E3
- Microsoft 365: Business, A3 ed E3


### <a name="next-steps"></a>Passaggi successivi

- Acquisire familiarità e condividere le informazioni incluse nel listino prezzi di anteprima con tutti i contatti appropriati all'interno dell'organizzazione. 
- Vedere tutti i materiali relativi alla conformità nella raccolta di risorse per gli aggiornamenti al programma Cloud Solution Provider: [Presentazione di Microsoft 365 Business Voice per piccole e medie aziende](https://partner.microsoft.com/resources/collection/m365-voice-smb#/). 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>Promozione di Cloud Solution Provider (CSP) per Microsoft 365 Business Voice ora disponibile

### <a name="categories"></a>Categorie

- Data: 2-11-2020
- Offerte/mercati

### <a name="summary"></a>Riepilogo

Prezzi scontati disponibili per i rinnovi e le nuove sottoscrizioni di Microsoft 365 Business Voice con piano per chiamate e Microsoft 365 Business Voice senza piano per chiamate.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma CSP

### <a name="details"></a>Dettagli

Dal 1° novembre 2020 al 30 aprile 2021, i rinnovi e le nuove sottoscrizioni di Microsoft 365 Business Voice con piano per chiamate e Microsoft 365 Business Voice senza piano per chiamate vengono offerti a prezzi scontati. Microsoft 365 Business Voice con piano per chiamate è soggetto a uno sconto del 25 percento per 12 mesi, mentre Microsoft 365 Business Voice senza piano per chiamate è soggetto a uno sconto del 33 percento per 12 mesi. 

#### <a name="offer-details"></a>Dettagli dell'offerta

   |**Nome offerta**|**ID offerta**|**ID materiale**|
   |-------------------|:------|:------|
   |Promozione per l'adozione di Microsoft 365 Business Voice|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Promozione per l'adozione di Microsoft 365 Business Voice|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Promozione per l'adozione di Microsoft 365 Business Voice (Stati Uniti)|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Promozione per l'adozione di Microsoft 365 Business Voice (senza piano per chiamate)|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Promozione per l'adozione di Microsoft 365 Business Voice (senza piano per chiamate)|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Promozione per l'adozione di Microsoft 365 Business Voice (senza piano per chiamate)|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |Promozione per l'adozione di Microsoft 365 Business Voice (senza piano per chiamate) per gli Stati Uniti|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

Queste promozioni interessano i clienti seguenti:

- Tenant di clienti completamente nuovi
- Tenant di clienti esistenti che non hanno attivato o recentemente annullato (negli ultimi 30 giorni) sottoscrizioni per qualsiasi licenza di Business Voice o del servizio di audioconferenza in CSP, Web Direct o qualsiasi altro canale commerciale Microsoft

#### <a name="additional-resources"></a>Risorse aggiuntive

- Per altre informazioni su Business Voice, visitare la [pagina per i partner di Microsoft 365 Business Voice](https://www.microsoft.com/microsoft-365/partners/businessvoice). 
- Altre informazioni su questa promozione sono disponibili nelle [domande frequenti dei partner](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo) correlate.

### <a name="next-steps"></a>Passaggi successivi

- Acquisire familiarità con le soluzioni promozionali per le riunioni e le chiamate e condividere queste informazioni con tutti i contatti appropriati nell'organizzazione.
- Incorporare queste offerte nella vendita di Microsoft 365.
- Sensibilizzare i clienti sul valore creato dall'aggiunta di Business Voice in Teams. 

________________
