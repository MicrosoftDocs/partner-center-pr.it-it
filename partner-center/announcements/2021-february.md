---
title: Annunci 2021 di febbraio
description: Febbraio 2021 annunci per Microsoft Partner Center, incluse nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 02/04/2021
ms.openlocfilehash: 8348179438ad65449ea75cd5ebce8ba0a92d7b9a
ms.sourcegitcommit: 0416562dd89408524f8312a8acd5b6944b6d91c4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/16/2021
ms.locfileid: "100540999"
---
# <a name="february-2021-announcements"></a>Annunci 2021 di febbraio

In questa pagina vengono illustrati in dettaglio gli annunci per Microsoft Partner Center per il 2021 febbraio.

________________
## <a name="now-live-docusign-migration-to-adobe-sign-for-partners-under-microsoft-partner-agreements-mpas"></a><a name="9"></a> Ora Live: DocuSign migrazione ad Adobe Sign per partner in Microsoft partner Agreements (MPAs)

### <a name="categories"></a>Categorie

- Data: 2021-02-16
- Funzionalità

### <a name="summary"></a>Riepilogo

Microsoft eseguirà la transizione di tutte le operazioni di elaborazione della firma elettronica da DocuSign ad Adobe Sign.

### <a name="impacted-audience"></a>Destinatari interessati

Partner Cloud Solution Provider (CSP) diretti e indiretti esistenti in MPA.

### <a name="details"></a>Dettagli

Nel febbraio 2021, Microsoft inizierà a eseguire la transizione di tutte le operazioni di elaborazione della firma elettronica da DocuSign ad Adobe Sign per i partner CSP.

Si prevede una transizione priva di problemi. Al momento della migrazione, si riceverà un messaggio di posta elettronica da adobesign@adobesign.com , invece di DocuSign, ogni volta che è richiesta la firma elettronica. Questo messaggio di posta elettronica fornirà un collegamento alla pagina Web di Adobe Sign, in cui sarà necessario firmare. I partner Microsoft non dovranno firmare nuovamente i contratti esistenti, ma solo i contratti di canale futuri. I partner in Ucraina, Russia e Kazakistan saranno tenuti a firmare di nuovo in modo fisico o elettronico il rider ogni anno.

È possibile trovare un esempio di un messaggio di posta elettronica di richiesta di firma del segno Adobe nella [raccolta di risorse](https://partner.microsoft.com/resources/detail/adobe-sign-signature-request-email-pdf).

Per un'esperienza ottimale, assicurarsi di eseguire le operazioni seguenti:

1. Aggiungere adobesign@adobesign.com all'elenco Mittenti attendibili per evitare che i messaggi di posta elettronica di questo account si trovino direttamente nella cartella posta indesiderata.
2. Collaborare con il reparto IT per:
    - Aggiungere l' adobesign@adobesign.com indirizzo di posta elettronica all'elenco mittenti sicuri per assicurarsi che non sia incluso in alcuna regola di phishing prestabilita.
    - Aggiornare i criteri di sicurezza esistenti per assicurarsi che tutti i destinatari necessari possano firmare la documentazione con la licenza Adobe Sign Enterprise.

Le risorse relative alle domande sull'onboarding, sulle funzionalità e sui processi aziendali sono disponibili nella pagina del partner per la [migrazione di Adobe Sign](https://aka.ms/eSignature/External).

Adobe Sign è la soluzione Microsoft preferita per la firma elettronica. La transizione ad Adobe Sign assicurerà un'esperienza di firma elettronica sicura ed efficiente che offrirà maggiore valore ai clienti e ai partner.

Per ulteriori informazioni sulla firma elettronica dei documenti e sulla delega della firma elettronica, vedere le esercitazioni seguenti:

- [Firma elettronica un documento | Esercitazioni di Adobe Sign](https://helpx.adobe.com/sign/how-to/adobe-for-signers.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/continuinged/collection.ccx.js&ref=helpx.adobe.com)
- [Delegare un altro utente per firmare un documento | Esercitazioni di Adobe Sign](https://helpx.adobe.com/sign/how-to/use-the-delegator-role.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/orientation/collection.ccx.js&ref=helpx.adobe.com)

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni con le parti interessate appropriate nella propria organizzazione.

### <a name="questions"></a>Domande?

In caso di domande, contattare il centro operativo locale usando lo [strumento di registrazione delle chiamate (CLT)](https://clt.partners.extranet.microsoft.com/CLT) o in [Esplora MS](https://www.explore.ms/). Seguire attentamente il processo CLT standard, in modo che la richiesta possa essere gestita il più rapidamente possibile.

### <a name="change-log"></a>Registro delle modifiche

- 15 gennaio 2021: pubblicazione originale 
- 16 febbraio 2021: ora Live, nuova risorsa: pagina del partner per la migrazione di Adobe Sign 

_____________

## <a name="reminder-introducingapithrottlingtopartners-calling-partner-centerapis"></a><a name="8"></a> Promemoria: Introduzione alla limitazione delle API ai partner che chiamano le API del centro per i partner

### <a name="categories"></a>Categorie

- Data: 2021-02-16
- Crescita aziendale

### <a name="summary"></a>Riepilogo

Microsoft implementerà la limitazione API per garantire prestazioni più coerenti in un intervallo di tempo per i partner che chiamano le API del centro per i partner.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che trasagiscono tramite il programma Cloud Solution Provider (CSP)  

### <a name="details"></a>Dettagli

A partire da febbraio 2021, Microsoft implementerà la limitazione API per garantire prestazioni più coerenti entro un intervallo di tempo per i partner che chiamano le API del centro per i partner.La limitazione limita il numero di richieste a un servizio in un intervallo di tempo per evitare un utilizzo eccessivo delle risorse.Quando viene superata una soglia di limitazione, il centro per i partner limita eventuali altre richieste del client per un determinato periodo di tempo.

**Vantaggi per i partner:**

Il centro per i partner è progettato per gestire un volume elevato di richieste, ma se un numero eccessivo di richieste viene effettuato da pochi partner, la limitazione consente di mantenere le prestazioni e l'affidabilità ottimali per tutti i partner.  

- La limitazione garantisce tempi di inattività minimi.
- La limitazione riduce il numero di richieste di volume elevato, contribuendo a garantire prestazioni coerenti per tutti i partner.

**API da limitare:**

| Operazione | Documentazione del Centro per i partner |
| ------ | ------- |
|{baseURL}/v1/customers/{customer_id}/subscriptions  | [Get-all-of-a-customer-s-subscriptions](/partner-center/develop/get-all-of-a-customer-s-subscriptions&data) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [Ottenere un abbonamento in base all'ID](/partner-center/develop/get-a-subscription-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders  | [Ottenere tutti gli ordini dei clienti](/partner-center/develop/get-all-of-a-customer-s-orders) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}  | [Ottenere un ordine in base all'ID](/partner-center/develop/get-an-order-by-id) |
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus  | [Ottenere lo stato del provisioning di un abbonamento](/partner-center/develop/get-subscription-provisioning-status) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}  | [Gestire gli ordini e gestire una sottoscrizione](/partner-center/develop/manage-orders#manage-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons  | [Ottenere un elenco dei componenti aggiuntivi per un abbonamento](/partner-center/develop/get-a-list-of-add-ons-for-a-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements | [Ottenere un elenco di diritti di Azure per una sottoscrizione](/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription) |
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus  | [Ottenere lo stato della registrazione di un abbonamento](/partner-center/develop/get-subscription-registration-status) |
|{baseURL}/v1/customers/{customer-tenant-id}/transfers  | [Ottenere tutti i trasferimenti di un cliente](/partner-center/develop/get-all-of-a-customer-s-transfers) |
|{baseURL}/v1/productUpgrades/{upgrade-id}/status  | [Ottenere lo stato di aggiornamento dei prodotti](/partner-center/develop/get-product-upgrade-status) |
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions   | [Ottenere un elenco delle offerte di conversione della copia di valutazione](/partner-center/develop/get-a-list-of-trial-conversion-offers) |
 
Si consiglia vivamente ai partner di usare l'API del log attività per una maggiore efficienza ed evitare la limitazione delle richieste.Per altre informazioni su questa funzionalità, vedere [qui](/partner-center/develop/api-throttling-guidance)i dettagli.  

### <a name="next-steps"></a>Passaggi successivi

Esaminare le [risorse](/partner-center/develop/api-throttling-guidance)   di questo argomento ed eseguire le operazioni necessarie.  

_______________

## <a name="introducing-microsoft-viva-topics"></a><a name="7"></a>Argomenti relativi all'introduzione a Microsoft viva

### <a name="categories"></a>Categorie

- Data: 12 febbraio 2021
- Funzionalità

### <a name="affected-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Gli argomenti di Microsoft viva applicano intelligenza artificiale per identificare le conoscenze e le competenze da tutta l'organizzazione e gestirle in argomenti condivisi come prodotti, clienti o progetti. Con le schede degli argomenti e le pagine degli argomenti immersive, le informazioni trovano nel contesto dei team, dei progetti e dei documenti. Intelligenza artificiale e persone collaborano per migliorare la conoscenza e la loro superficie nelle app che usi ogni giorno. 

Gli utenti devono avere una licenza di uno dei seguenti elementi per essere idonei per gli argomenti di viva:   
- Microsoft 365 F1, F3, E3, a3, E5 o a5 
- Office 365 F3, E1, a1, E3, a3, E5 o a5 
- Microsoft 365 Business Basic, standard o Premium 
- SharePoint K, piano 1 o Plan2 

**Dettagli dell'offerta**

Queste offerte avranno "esperienze di argomento" nei nomi delle offerte negli elenchi prezzi di 1 febbraio. Questi nomi di offerta verranno aggiornati con "argomenti viva" quando gli elenchi prezzi vengono aggiornati il 1 ° marzo.

|**Nome offerta**|**ID offerta**|**ID materiale**|
|------------------|:--------------------|:------------------|
|Argomenti di viva|b9ef0c81-9ca6-45fd-a6c1-627745ba8b8a|1JV-00005|
|Argomenti di viva per i docenti|8c930d38-db61-4afa-83f9-77c595c5cdfc|1TK-00006|
|Argomenti di viva per studenti|5de461d5-8ccc-4a8e-98ae-58a3ad400a57|1TK-00007|

### <a name="next-steps"></a>Passaggi successivi

- Esaminare le risorse di questo argomento e condividere queste informazioni con le parti interessate appropriate nell'organizzazione.  
- Altre informazioni sono disponibili nel [Centro risorse degli argomenti di viva](https://resources.techcommunity.microsoft.com/viva-topics).

_______________

## <a name="microsoft-365-e3-price-changes-coming-for-march-2021"></a><a name="6"></a>Modifiche al prezzo di Microsoft 365 E3 in arrivo per il 2021 marzo

### <a name="categories"></a>Categorie

- Data: 11 febbraio 2021
- Offerte/mercati

### <a name="affected-audience"></a>Destinatari interessati

Tutti i partner che operano attraverso il programma Cloud Solution Provider (CSP) in EUR, AUD, GBP e JPY.

### <a name="details"></a>Dettagli

L'elenco prezzi per l'anteprima basata su licenza per il 2021 marzo è stato aggiornato in modo da includere le variazioni dei prezzi per Microsoft 365 E3. L'offerta e le valute interessate sono elencate di seguito. 
 
Nome offerta: Microsoft 365 ID offerta E3: ID materiale 2b3b8d2d-10aa-4BE4-b5fd-7f2feb0c3091: AAA-35638

Questi aggiornamenti dei prezzi Microsoft 365 E3 sono limitati solo alle valute seguenti: JPY (Yen giapponese), GBP (Great British Pound), EUR (Unione europea), AUD (Dollaro australiano). Nel file di marzo sono presenti altre modifiche ai prezzi e i partner devono ottenere l'anteprima più recente per visualizzare le altre modifiche previste.

### <a name="next-steps"></a>Passaggi successivi

I partner devono scaricare i file dell'elenco prezzi più recenti dal centro per i partner per ottenere i prezzi più recenti di marzo. 

_______________

## <a name="license-based-preview-price-list-updated-for-norwegian-krone"></a><a name="5"></a>Elenco prezzi anteprima basata su licenza aggiornato per corona norvegese

### <a name="categories"></a>Categorie

- Data: 10 febbraio 2021
- Offerte/mercati

### <a name="affected-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="summary"></a>Riepilogo

Il listino prezzi per l'anteprima basata su licenza è stato aggiornato per i prezzi della corona norvegese prevista per il 1 ° marzo 2021.

### <a name="details"></a>Dettagli

Le modifiche al tasso FX per marzo non sono state incluse negli elenchi prezzi precedenti basati sulle licenze di marzo. Questo file è stato aggiornato per riflettere le modifiche previste del prezzo della corona norvegese. Per visualizzare le modifiche previste per il 1 ° marzo 2021, i partner devono ottenere il file di prezzi di anteprima corrente più recente. Queste modifiche sono solo per i prezzi della valuta scandinava norvegese.

### <a name="next-steps"></a>Passaggi successivi

I partner devono scaricare il file di anteprima Listino prezzi corrente per le modifiche previste per il 1 ° marzo 2021.

_______________

## <a name="premium-assessments-an-add-on-to-compliance-manager-is-coming-on-march-1-2021"></a><a name="4"></a>Valutazioni Premium, un componente aggiuntivo di Compliance Manager, sarà disponibile il 1 ° marzo 2021

### <a name="categories"></a>Categorie

- Data: 5 febbraio 2021
- Funzionalità

### <a name="affected-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="summary"></a>Riepilogo

Le valutazioni Premium saranno incluse nell'anteprima dell'elenco prezzi di febbraio e saranno disponibili a partire dall'1 marzo 2021.

### <a name="details"></a>Dettagli

Le valutazioni Premium sono un componente aggiuntivo facoltativo di Compliance Manager e possono aiutare i clienti a conformarsi ai requisiti nazionali, regionali e specifici del settore che regolano la raccolta e l'uso dei dati. Le valutazioni Premium sono riservate per i clienti di Office 365 E5, a5 e G5 e Microsoft 365 E5, a5 e G5.

|**Nome offerta**|**ID offerta**|**ID materiale**|
|------------------|:--------------------|:------------------|
|CSP-Corp-addon|[76be61a7-2c03-4b3e-8330-63b11bd904ed](https://commoffertool.catalog.cp.microsoft.com/Prod/Office365/offer/details/76be61a7-2c03-4b3e-8330-63b11bd904ed)|8JA-00003|
|CSP-Corp-versione di valutazione|[f2f6ae44-24fe-450c-9cd7-529e7c8cfcb4](https://commoffertool.catalog.cp.microsoft.com/Prod/Office365/offer/details/f2f6ae44-24fe-450c-9cd7-529e7c8cfcb4)|8JA-00004|
|CSP-Educational-facoltà-addon|[fa7f5773-063a-48cf-b3e2-de509ea1262f](https://commoffertool.catalog.cp.microsoft.com/Prod/Office365/offer/details/fa7f5773-063a-48cf-b3e2-de509ea1262f)|8JB-00003|
|CSP-Educational-facoltà-versione di valutazione|[828cecbd-8728-4339-B0C2-51e009a67d88](https://commoffertool.catalog.cp.microsoft.com/Prod/Office365/offer/details/828cecbd-8728-4339-b0c2-51e009a67d88)|8JB-00004|

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse seguenti per questo argomento e condividere le informazioni con le parti interessate appropriate all'interno dell'organizzazione.   

- [Sicurezza e conformità di Microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?rtc=1&activetab=m365-enterprise:primaryr5)
- [Crea e Gestisci valutazioni in Microsoft Compliance Manager](https://docs.microsoft.com/microsoft-365/compliance/compliance-manager-assessments&preserve-view=true=o365-worldwide)

_________________________________________________________

## <a name="responding-to-covid-19-microsoft-partner-network-update"></a><a name="3"></a> Risposta a COVID-19: Microsoft Partner Network aggiornamento

### <a name="categories"></a>Categorie

- Data: 4 febbraio 2021
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner

### <a name="details"></a>Dettagli

Microsoft offre un'estensione delle competenze (ad eccezione delle competenze per il cloud Business Applications) e un'estensione di specializzazione avanzata per i partner con date di anniversario (AD) comprese tra il 1 ° gennaio 2021 e il 30 giugno 2021. Per ulteriori informazioni, vedere il [post di Blog del partner](https://blogs.partner.microsoft.com/mpn/responding-to-covid-19-microsoft-partner-network/) .
________________
## <a name="new-updates-to-the-referrals-module-in-partner-center"></a><a name="2"></a> Nuovi aggiornamenti del modulo dei riferimenti nel centro per i partner

### <a name="categories"></a>Categorie

- Data: 5 febbraio 2021
- Funzionalità
 
### <a name="impacted-audience"></a>Destinatari interessati

- Partner con offerte di co-selling pronte
- Partner con un'offerta transazionale che usa una soluzione Azure incentive-idonea nel Marketplace commerciale
- Tutti i partner che usano il modulo referrals nel centro per i partner.

### <a name="details"></a>Dettagli

Quando passiamo al nuovo anno, stiamo aggiungendo funzionalità per migliorare e arricchire l'esperienza di co-selling nel centro per i partner. Queste nuove funzionalità consentiranno di accelerare la velocità dell'offerta, estendere l'accesso ai venditori e migliorare la scalabilità dell'azienda. Introdotta nel modulo referrals, queste nuove aggiunte consentiranno di raggiungere un maggior numero di clienti tramite altri partner Microsoft o venditori Microsoft, gestendo al tempo stesso la pipeline con Microsoft in un'unica posizione.  

Ecco le novità del modulo dei riferimenti al centro per i partner:

#### <a name="all-partners-using-the-referrals-module-in-partner-center"></a>Tutti i partner che usano il modulo referrals nel centro per i partner  

- [Creazione di nuove connessioni SMB](https://docs.microsoft.com/partner-center/connect-with-your-customers): co-selling e collaborazione con i venditori Microsoft per ottenere opportunità in ingresso correlate ai clienti SMB.

- [Espandere autorizzazioni di riferimento](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals): assegnare le autorizzazioni di riferimento degli utenti a seconda che si desideri avere autorizzazioni di amministratore (accesso a tutte le opportunità di co-selling) o autorizzazioni utente (accesso alle opportunità di co-selling specifiche dell'utente).

- [Migrazione utente per partner Sales Connect](https://docs.microsoft.com/partner-center/psc-to-pc#user-migration): mappare le autorizzazioni utente per le vendite partner esistenti per le autorizzazioni utente per l'amministratore e il riferimento del centro per i partner corrispondenti, quindi applicare a massa le nuove autorizzazioni per gli utenti. Per ulteriori informazioni sulla gestione dei riferimenti, vedere la [documentazione sulle autorizzazioni](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) per i riferimenti.  

#### <a name="partners-with-co-sell-ready-offers"></a>Partner con offerte di co-selling pronte

- [Co-selling con altri partner](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities): invita un altro partner del nostro potente ecosistema di partner per co-selling con l'utente e sbloccare l'accesso a più destinatari del cliente.  

#### <a name="partners-with-a-transactable-offer-using-an-azure-incentive-eligible-solution-in-the-commercial-marketplace"></a>Partner con un'offerta transazionale che usa una soluzione Azure incentive-idonea nel Marketplace commerciale

- [Usare la registrazione automatica dell'affare](https://docs.microsoft.com/partner-center/register-deals): risparmiare tempo e assicurare l'accuratezza registrando le offerte di Azure Commercial Marketplace transazionale con la casella di controllo, "questa operazione/vittoria è stata o verrà sottoposta a transazione tramite Azure Marketplace o AppSource". Se la data della transazione è corretta, le informazioni per la registrazione dell'accordo verranno estratte direttamente da Microsoft Commercial Marketplace.

### <a name="questions"></a>Domande?

Per assistenza sull'uso di una delle nuove funzionalità, vedere la [sezione relativa ai riferimenti](https://docs.microsoft.com/partner-center/referrals) nella Knowledge base o i materiali di supporto disponibili nella [raccolta di esperienze di co-selling](https://aka.ms/CoSellExperience) (accesso richiesto).

È possibile [aprire un ticket con il team di supporto del partner](https://partner.microsoft.com/support/?stage=1) per assistenza.

________________
## <a name="deprecation-and-retirement-of-put-qualification-apis-for-the-education-customer-validation-process-by-february-25-2021-and-get-qualification-by-may-4-2021"></a><a name="1"></a> Deprecazione e ritiro delle API PUT qualificate per il processo di convalida dei clienti Education entro il 25 febbraio 2021 e ottenere la qualifica entro il 4 maggio 2021.

### <a name="categories"></a>Categorie

- Data: 4 febbraio 2021
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Partner che vendono soluzioni accademiche, no profit e GCC tramite il programma Cloud Solution Provider tramite l'API del centro per i partner

### <a name="details"></a>Dettagli

Questo annuncio è un completamento per i miglioramenti apportati al centro per i partner [rilasciati nel dicembre](https://docs.microsoft.com/partner-center/announcements/2020-december#1). Come parte di questa versione, sono state distribuite le nuove API per le qualifiche GET e POST e, di conseguenza, **le API del centro per i partner del centro per le API esistenti di put ritireranno entro il 25 febbraio 2021 e otterranno la qualifica entro il 4 maggio 2021**. A questo punto, sarà necessario passare all'uso delle nuove API del centro per i partner per poter acquistare le offerte di formazione e la nuova API per ottenere le qualificazioni per acquistare le offerte non profit e GCC prequalificate.

### <a name="next-steps"></a>Passaggi successivi

- **Aggiornamento alle nuove API** per una transizione corretta e tempestiva
- **Esaminare le nuove modifiche e la guida dell'API del centro** per i partner nelle risorse per la preparazione delle operazioni: miglioramenti apportati al [processo di convalida dei clienti di Education Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)
- **Condividere queste informazioni con i team appropriati** all'interno dell'organizzazione e con i rivenditori per aiutarli a prepararsi a queste modifiche.

### <a name="questions"></a>Domande?

Per eventuali domande relative a questa notifica, contattare il [supporto tecnico del Centro per i partner](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Registro delle modifiche

- Febbraio: sequenze temporali aggiornate per la deprecazione di GET & le qualifiche PUT
- Gennaio: promemoria dei futuri deprecazioni di GET & le qualifiche PUT
