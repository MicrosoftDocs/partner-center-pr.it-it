---
title: Annunci di marzo 2021
description: Annunci di marzo 2021 per Microsoft Partner Center nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 52db2c8ee7652633ee5d73a534e8c73daead867e
ms.sourcegitcommit: cce4d53127fa33e6c2bbf158dda6edd41b82441d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/25/2021
ms.locfileid: "112896816"
---
# <a name="march-2021-announcements"></a>Annunci di marzo 2021

Questa pagina fornisce gli annunci per Microsoft Partner Center marzo 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="19"></a>Idoneità: modifiche all'API di convalida dell'indirizzo Cloud Solution Provider (CSP) in corso di validità a giugno; Funzionalità di test ora disponibile

### <a name="categories"></a>Categorie

- Data: 2021-03-30
- Preparazione

### <a name="summary"></a>Riepilogo

Per consentire a partner e clienti di eseguire la propria attività in base alla fiducia, invitiamo i partner a testare le modifiche apportate all'API Convalida indirizzo per tutti i paesi di tutto il mondo.

### <a name="impacted-audience"></a>Destinatari interessati

I partner di fatturazione diretta CSP e i provider indiretti che creano nuovi o aggiornano i clienti esistenti indirizzano i dettagli.

### <a name="details"></a>Dettagli

Microsoft Microsoft si impegna a fornire un metodo conforme, sicuro e sicuro per la convalida degli indirizzi dei clienti per la transazione delle sottoscrizioni dei clienti nel programma CSP. A partire dal 31 marzo 2021 sono state introdotte modifiche all'API Convalida indirizzo che i partner hanno invitato a testare, prima di pubblicare le modifiche nel mese di giugno 2021.

Le modifiche influiscono solo sull'API Convalida indirizzo. Le API Crea cliente e Aggiorna profilo di fatturazione non sono influenzate.

La risposta restituirà uno dei messaggi di stato seguenti:

| Stato     | Descrizione |    Numero di indirizzi suggeriti restituiti |
|-------|---------------|-------------------|
|Shippable verificato | L'indirizzo viene verificato e può essere spedito a . | Single |
|Verified | L'indirizzo viene verificato. | Single |
|Interazione richiesta | L'indirizzo suggerito è stato modificato in modo significativo e richiede la conferma dell'utente. | Single |
|Via parziale | La via specificata nell'indirizzo è parziale e richiede altre informazioni. | Multiplo: massimo tre |
|Locale parziale | I locali (numero di edificio, numero di suite e altri) sono parziali e necessitano di altre informazioni. | Multiplo: massimo tre |
|Multipli | Sono presenti più campi parziali nell'indirizzo (potenzialmente includendo anche street partial e premises partial). | Multiplo: massimo tre |
|Nessuno | L'indirizzo non è corretto. | Nessuno |
|Non convalidato | Impossibile inviare l'indirizzo tramite il processo di convalida. | Nessuno |

I codici postali degli Stati Uniti restituiranno altre 4 cifre e un trattino, ad esempio 12345-6789.

Dopo l'invio di un indirizzo per la convalida tramite l'API Convalida indirizzo, verrà restituito lo schema di risposta seguente:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Esaminare questa risposta di esempio. Si noti che per gli Stati Uniti, la risposta restituirà un suffisso aggiuntivo a quattro cifre per la riga del codice postale se si immettono solo cinque cifre per il cap.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Passaggi successivi

- Condividere l'ID tenant sandbox con l'esperto di materia (Ali Kaki) da includere nel volo di test, in modo da poter iniziare a prepararsi per l'aggiornamento.

- Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.

### <a name="questions"></a>Domande?

Se è necessario supporto per le operazioni con Microsoft, contattare il gruppo di supporto Yammer partner.

### <a name="change-log"></a>Log delle modifiche:

- 31 marzo 2020: pubblicazione originale

- 30 aprile 2021: aggiornamenti per la risposta di esempio e i dettagli del codice postale

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="18"></a>Nuova Exchange'interfaccia di amministrazione (EAC)

### <a name="categories"></a>Categorie

- Data: 2021-03-29
- Funzionalità

### <a name="summary"></a>Riepilogo

A partire dal 27 aprile 2021, l'interfaccia di amministrazione di Exchange (EAC) eserciterà una nuova esperienza che migliorerà l'efficienza quotidiana degli utenti.

### <a name="impacted-audience"></a>Destinatari interessati

Amministratori delegati che accedono Exchange tramite Partner Center

### <a name="details"></a>Dettagli

A partire dal 27 aprile 2021, i partner che Exchange tramite Partner Center verranno reindirizzati al nuovo interfaccia di amministrazione di Exchange.

Questa nuova esperienza è attualmente disponibile come anteprima e gli amministratori possono attivare questa esperienza selezionando l'interruttore nell'angolo in alto a destra nell'interfaccia di amministrazione di Exchange classica. È anche possibile passare al nuovo interfaccia di amministrazione di Exchange selezionando il banner "Prova adesso" visualizzato in tutte le pagine.

I vantaggi della nuova interfaccia di amministrazione di Exchange includono:

- Aggiunta di informazioni dettagliate, report e meccanismi di avviso per i problemi correlati al flusso di posta. 

- Dashboard personalizzati per aumentare la produttività.

Per facilitare l'esplorazione della nuova esperienza, i video sono disponibili nella sezione **Training & Guide** della nuova esperienza EAC. In questo modo verrà fornita una panoramica di come usare al meglio il nuovo portale.

>[!NOTE]
>Con questa modifica, l'esperienza EAC classica non verrà deprecata. Si riceverà una notifica in anticipo prima dell'implementazione di qualsiasi modifica.

### <a name="next-steps"></a>Passaggi successivi

- Vedere le [risorse relative a questo argomento,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)in cui è possibile visualizzare gli screenshot della nuova esperienza.

- Condividere queste informazioni con le parti interessate appropriate nella propria organizzazione. 

### <a name="questions"></a>Domande?

Per eventuali domande su queste modifiche, controllare le community Yammer pertinenti.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="17"></a>Microsoft Operations: Introduzione al calendario di lancio del prodotto

### <a name="categories"></a>Categorie

- Data: 2021-03-25
- Offerte | Area di lavoro moderna

### <a name="summary"></a>Riepilogo

In risposta ai commenti e suggerimenti dei partner, Microsoft Operations semplifica le comunicazioni per il lancio del prodotto.

### <a name="impacted-audience"></a>Destinatari interessati

Partner Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Microsoft si impegna a migliorare continuamente le esperienze dei partner. Microsoft ha ricevuto commenti e suggerimenti che hanno ricevuto troppe comunicazioni da Microsoft, inclusi annunci duplicati per il lancio del prodotto.

In risposta ai commenti e suggerimenti, Microsoft ha semplificato l'esperienza di preparazione per i lanci di prodotti per le offerte nuove ed esistenti.

È ora disponibile una singola visualizzazione mensile dei lanci dei prodotti, pubblicata nella raccolta di risorse per l'idoneità alle operazioni. Questa visualizzazione [mensile del calendario](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) di lancio del prodotto sostituirà le singole comunicazioni di lancio del prodotto nella raccolta di risorse conformità alle operazioni e Partner Center annunci.

È anche possibile accedere a questo [calendario di lancio del prodotto](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) dalle raccolte della [community,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [dalle visualizzazioni del](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)calendario e dalle newsletter [CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Quando verrà pubblicato il calendario di lancio del prodotto di ogni mese, verrà visualizzato un annuncio nella raccolta di risorse conformità alle operazioni.

È comunque possibile trovare informazioni sulle offerte nuove ed esistenti nei log delle modifiche del listino prezzi e nell'anteprima del listino prezzi, nonché nei blog dei prodotti, nelle guide alle licenze e nelle pagine di marketing dei prodotti.

La modifica verrà applicata ai lanci per i prodotti seguenti:

- Dynamics locale
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- Strumenti
- Teams e Telco

Microsoft continuerà a inviare annunci specifici per i lanci di prodotti che richiedono dettagli sull'idoneità per le operazioni.

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse relative a questo argomento e condividere queste informazioni con gli stakeholder appropriati nell'organizzazione.

### <a name="questions"></a>Domande?

Per altre domande su queste offerte, vedere le community Yammer pertinenti.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="16"></a>Modifiche ai requisiti di onboarding dei clienti CSP

### <a name="categories"></a>Categorie

- Data: 25/03/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

Nell'ambito dell'impegno per aiutare partner e clienti a eseguire la propria attività in base alla fiducia, microsoft richiederà informazioni aggiuntive sui clienti a partire dal 25 marzo 2021.

### <a name="impacted-audience"></a>Destinatari interessati

Cloud Solution Provider (CSP) con fatturazione diretta partner e provider indiretti che hanno clienti nuovi o esistenti nei paesi elencati nella sezione successiva

### <a name="details"></a>Dettagli

Microsoft si impegna a fornire un metodo di convalida dei clienti conforme e sicuro per la vendita di sottoscrizioni cliente nel programma CSP. Il 25 marzo 2021 verranno introdotti miglioramenti all'API e all'interfaccia utente di Partner Center che influiranno sui partner che soddisfano entrambi i criteri seguenti:

1. Il partner ha una relazione di fatturazione diretta con Microsoft (ovvero, è un partner con fatturazione diretta o un provider indiretto).

2. Il partner opera con clienti nuovi o esistenti nei paesi seguenti:

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

I partner che soddisfano i criteri doranno inviare l'ID registrazione aziendale di  un cliente (noto anche come **INN** dell'organizzazione del cliente) e il numero di telefono quando si esegue l'onboarder di nuovi clienti o si modificano i dettagli dei clienti esistenti.  I partner possono anche immettere un **secondo nome** facoltativo per il cliente.

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

I partner con clienti nel resto del mondo avranno la possibilità il 25 marzo 2021  di immettere **l'ID** di registrazione della **società,** il numero di telefono e il secondo nome per i clienti come dettagli facoltativi.

### <a name="next-steps"></a>Passaggi successivi

- Per indicazioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella raccolta dedicata dei [partner.](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- Prepararsi a incorporare le modifiche usando l'API Partner Center e l'esperienza utente Web. Saranno disponibili API e SDK a scopo di test.

- Assicurarsi di inviare i dati aggiuntivi quando si caricano nuovi clienti o si modificano i dettagli del cliente esistente.

- Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.

### <a name="questions"></a>Domande?

In caso di domande relative all'identificatore legale (noto anche come INN o codice identificativo del contribuente), contattare il consulente fiscale o l'ufficio fiscale locale. Microsoft non è in grado di fornire indicazioni sulle imposte.

Se è necessario supporto per le operazioni con Microsoft, [aprire una richiesta di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="15"></a>Correzioni apportate al listino prezzi perpetuo del 1° marzo 2021

### <a name="categories"></a>Categorie

- Data: 23/03/2021
- Offerte/mercati

### <a name="impacted-audience"></a>Destinatari interessati

Provider indiretti e partner con fatturazione diretta che eselezionano software perpetuo nel Cloud Solution Provider programma 

### <a name="details"></a>Dettagli

Il listino prezzi per il software perpetuo pubblicato il 1° marzo 2021 includeva mercati che non dovevano essere presenti. Il listino prezzi perpetuo del software è stato aggiornato il 17 marzo 2021 con le correzioni. Queste correzioni erano applicabili solo a:

- ID prodotto: DF77X4D43RKT 
- Nome prodotto: Windows 10 Home per Pro Upgrade for Microsoft 365 Business
- Mercati rimossi o non supportati: AE, AF, AL, AM, AO, BA, BB, BD,UF, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME , MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Queste modifiche si applicano solo al prodotto precedente. Altri prodotti non hanno apportato correzioni. 

### <a name="next-steps-and-resources"></a>Passaggi successivi e risorse

- I partner che eselezionano software perpetuo devono scaricare il listino prezzi del software perpetuo più recente.
- Consultare i [codici paese dell'area](/azure/marketplace/commercial-marketplace-co-sell-countries) geografica per un mapping descrittivo dell'abbreviazione di due lettere ai paesi.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="14"></a> Versione dell'SDK .NET Standard (v1.17.0)

### <a name="categories"></a>Categorie

- Data: 23/03/2021

- Funzionalità
 
### <a name="impacted-audience"></a>Destinatari interessati

Partner di fatturazione diretta e provider indiretti che partecipano al programma CSP e usano .NET SDK del Centro per i partner.

### <a name="details"></a>Dettagli

A partire dal 23 marzo 2020, i partner possono iniziare a scaricare la versione di [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), insieme agli esempi di SDK per Centro per i partner [GitHub aggiornati.](https://github.com/Microsoft/Partner-Center-DotNet-Samples) Questa versione include aggiornamenti ai metodi seguenti:

#### <a name="audit-updated-new-operation-types"></a>Controllo aggiornato: nuovi tipi di operazione

Aggiunta di nuovi [tipi di operazione](/partner-center/develop/auditing-resources) per sapere quando il cliente ha approvato e terminato il DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Controllo aggiornato: nuovi tipi di risorsa e di operazione

Aggiunta di nuovi [tipi di risorsa e di operazione](/partner-center/develop/auditing-resources) per supportare lo scenario del ruolo della directory del cliente.

- Nuovo tipo di risorsa "CustomerDirectoryRole"

- Tipi di operazione "AddUserMember" e "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Aggiornamenti dell'SDK per gli account dei clienti

- Supporto per GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Modifiche aggiuntive

Le modifiche seguenti vengono introdotte come parte di New Commerce e sono attualmente disponibili su invito solo per i partner che fanno parte dell'anteprima tecnica M365/D365 New Commerce. I partner che non fanno parte di New Commerce Technical Preview non devono notare gli effetti e devono essere compatibili con le versioni precedenti.

- Modifiche al catalogo:

  - GET /products/{product-id}/skus/{sku-id}

- Acquistare e gestire:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Passaggi successivi

- Scaricare la versione più [recente di MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Scaricare ed esaminare gli [esempi di GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="13"></a>Offerta del marketplace commerciale CSP e incentivi CSP FY21 per le offerte idonee

### <a name="categories"></a>Categorie

- Data: 2021-03-18
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Provider indiretti e partner di fatturazione diretta nel programma Cloud Solution Provider indiretto 

### <a name="details"></a>Dettagli

I provider indiretti e i partner con fatturazione diretta nel programma Cloud Solution Provider possono vendere offerte di terze parti e ottenere un incentivo per ogni offerta di terze parti idonea transazionata in Partner Center o nel portale di Azure. L'incentivo sarà sotto forma di sconto sulle vendite fatturate per le offerte idonee ed è disponibile fino al **30 giugno 2021.**  

Continuare a conoscere questo incentivo dell'offerta del Marketplace commerciale CSP di seguito e contattare i clienti oggi stesso per identificare le offerte giuste per consentire il successo continuo e la trasformazione digitale.

Microsoft collabora con fornitori di software indipendenti (ISV) per commercializzazione delle soluzioni IaaS e SaaS più recenti per i clienti Microsoft. Gli editori ISV hanno la possibilità di abilitare le vendite delle offerte tramite il canale partner Microsoft. Le offerte idonee per gli incentivi rientrano in due categorie:

- Selezionare Offerte di terze parti SaaS e IaaS con stato incentivato di co-selling ip di Azure. 

- Applicazioni SaaS integrate con Teams o almeno due app di produttività Microsoft 365, ad esempio PowerPoint, Word, Excel, Outlook o SharePoint.

### <a name="next-steps-and-resources"></a>Passaggi successivi e risorse

- Informazioni su come ottenere incentivi [per i partner per](https://partner.microsoft.com/membership/partner-incentives) la vendita di app del marketplace idonee per le app idonee per gli incentivi. Le nuove offerte vengono aggiunte ogni mese.  
- [Cloud Solution Provider risorse di incentivi per i partner con fatturazione diretta](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Cloud Solution Provider risorse di incentivazione del provider indiretto](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Per altre [informazioni sulla](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) vendita delle app del marketplace commerciale, vedere questa presentazione. Per altre risorse, vedere [qui](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Esplorare il catalogo del marketplace commerciale in [Partner Center](../csp-commercial-marketplace-discover.md) o [portale di Azure](https://ms.portal.azure.com/#home)
- Usare [le API per](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) integrare le app nel marketplace aziendale
- Contattare gli ISV con cui si è interessati a fare affari
- I provider indiretti devono integrarsi usando le API e guidare i rivenditori sulle app da vendere

### <a name="questions"></a>Domande?  

Fare riferimento [a questo articolo](../csp-commercial-marketplace-overview.md) per una panoramica del marketplace commerciale in Partner Center.

Se è necessaria assistenza aggiuntiva, è possibile creare una richiesta di supporto in Partner Center. Per altre informazioni, vedere [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="12"></a>Power BI Premium di denominazione dell'offerta e aggiornamento dei prerequisiti

### <a name="categories"></a>Categorie

- Data: 2021-03-18
- Funzionalità

### <a name="summary"></a>Riepilogo

Il listino prezzi finale del 1° aprile 2021 verrà aggiornato per aggiungere maggiore chiarezza alle informazioni sulla denominazione e/o sui prerequisiti per le Power BI Premium per utente.

### <a name="impacted-audience"></a>Destinatari interessati

Cloud Solution Provider (CSP) partner diretti e indiretti

### <a name="details"></a>Dettagli

Il listino prezzi finale del 1° aprile 2021 verrà aggiornato per aggiungere maggiore chiarezza alle informazioni sulla denominazione e/o sui prerequisiti per le Power BI Premium per utente.

Fino all'aggiornamento del listino prezzi finale, usare le informazioni contenute in questa sezione per assicurarsi che il prodotto corretto sia ordinato.

I dettagli seguenti mostrano lo SKU interessato e i dettagli dei prerequisiti.

| Nome visualizzato dell'offerta nell'anteprima del listino prezzi del 1° marzo |  Aggiornamento del nome visualizzato dell'offerta nel listino prezzi finale del 1° aprile| ID offerta |
| ------ | ----------- | ----------- |
| Power BI Premium Per utente Add-On (prezzi del personale no profit)  |  Power BI Premium Per utente Add-On **(Office)** (prezzi del personale no profit)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Per acquistare questa offerta, i clienti devono avere uno dei prerequisiti seguenti:

| Nome visualizzato dell'offerta | ID offerta |
| ------ | ----------- |
| Microsoft 365 E5 (prezzi del personale no profit)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 senza audioconferenza (prezzi del personale no profit)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (prezzi del personale no profit)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (prezzi del personale no profit)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 senza audioconferenza (prezzi del personale no profit)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

L'Power BI Premium seguente presenta un prerequisito necessario per l'acquisto:

| Nome visualizzato dell'offerta | ID offerta |
| ------ | ----------- |
|   Power BI Premium Per utente Add-On (prezzi del personale no profit)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

I clienti devono avere questo prerequisito per acquistare questa offerta:

| Nome visualizzato dell'offerta | ID offerta |
| ------ |----------|
| Power BI Pro (prezzi del personale no profit)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Passaggi successivi

Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.  

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, controllare le community Yammer pertinenti. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="11"></a>Aggiornamenti dei prezzi di marzo per Microsoft 365 F3

### <a name="categories"></a>Categorie

- Data: 2021-03-16
- Offerte/mercati

### <a name="summary"></a>Riepilogo

I prezzi di marzo 2021 non corretti sono stati corretti per Microsoft 365 F3 British Pound (GBP) ed Euro (EUR).

### <a name="impacted-audience"></a>Destinatari interessati

I partner Microsoft 365 F3 in GBP o EUR tra il 1° e il 17 marzo 2021 tramite il programma Cloud Solution Provider (CSP).

### <a name="details"></a>Dettagli

Microsoft ha risolto prezzi non corretti per Microsoft 365 F3. I prezzi non corretti erano per GBP ed EUR e solo per le offerte acquistate tra il 1° e il 17 marzo 2021. Le offerte e le valute influenzate sono elencate di seguito. 

| Nome offerta | Valuta | ID offerta | ID materiale |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Rieti) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Commerciale) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
I listini prezzi di anteprima di marzo e aprile sono stati aggiornati il 16 marzo alle 17:00 ora solare Pacifico.

### <a name="next-steps"></a>Passaggi successivi

- I partner devono scaricare nuovamente i listini prezzi correnti basati su licenza, sia di marzo che dell'anteprima di aprile, con queste correzioni di prezzo, se applicabile.  
- Microsoft contattierà i partner interessati nelle prossime settimane tramite posta elettronica per informarli dei passaggi successivi relativi alla correzione delle transazioni interessate.

### <a name="questions"></a>Domande?

Per altre domande, controllare le community di Yammer CSP pertinenti.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="10"></a> Aggiornare il nome di una società legale tramite Partner Center

### <a name="categories"></a>Categorie

- Data: 16/03/2021
- Aumentare l'efficienza & scalabilità

### <a name="summary"></a>Riepilogo

A partire da marzo 2021, i partner Microsoft Partner Network (MPN) e i rivenditori indiretti di Cloud Solution Provider (CSP) possono aggiornare il nome della società legale tramite Partner Center.

### <a name="impacted-audience"></a>Destinatari interessati

Partner MPN e rivenditori indiretti CSP (non applicabili ai partner con fatturazione diretta CSP)

### <a name="details"></a>Dettagli

A partire da marzo 2021, i partner MPN e i rivenditori indiretti CSP possono aggiornare il nome della società legale tramite Partner Center in modo conforme e self-service. Con questa nuova funzionalità, i partner non dovranno più inviare un ticket Partner Center di supporto per aggiornare il nome della società. Ciò consentirà ai partner un notevole risparmio in termini di tempo per l'esecuzione di queste attività. 

Per altre informazioni, vedere [Aggiornare il profilo di business legale.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Assicurarsi che il nome della società nel profilo aziendale legale sia privo di errori di ortografia e abbreviazioni e che corrisponda esattamente ai record di registrazione aziendale formali dell'azienda. Per altre informazioni sull'aggiornamento del profilo dell'organizzazione, vedere [Verificare il profilo dell'organizzazione.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni all'interno dell'organizzazione in modo che il team appropriato possa esaminare e aggiornare i processi.

### <a name="questions"></a>Domande?

Per altre domande, controllare le community di Yammer CSP pertinenti.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="9"></a>Aggiornamento all'evoluzione Cloud Solution Provider (CSP) e modifiche al programma Open License

### <a name="categories"></a>Categorie

- Data: 15/03/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

Nuove offerte software perpetue del settore pubblico e commerciale sono in arrivo nel programma Cloud Solution Provider (CSP) insieme alle modifiche apportate al programma Open Licensing.

### <a name="impacted-audience"></a>Destinatari interessati

Distributori commerciali e rivenditori gestiti che vendono tramite il programma Open License, nonché tutti i partner CSP che eselezionano software perpetuo

### <a name="details"></a>Dettagli

Nel mese di settembre 2020 [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) ha annunciato una serie di passaggi nel percorso di trasformazione digitale per espandere le opportunità per i partner nel programma CSP, inclusa la disponibilità di software locale per i partner. Queste modifiche consentono ai partner di far crescere la propria azienda ed estendere la propria copertura sfruttando le licenze software in CSP, posizionandole per il successo nel mondo attuale in cui il cloud è al primo posto. Consentono inoltre ai clienti di passare al cloud e offrono ai partner la flessibilità necessaria per gli ambienti cloud ibridi dei clienti.

Nel proseguimento di questa trasformazione digitale vengono annunciate le modifiche seguenti:

- 1 luglio 2021: non verranno aggiunti nuovi SKU, prodotti o promozioni al listino prezzi del programma Open License.

- 7 luglio 2021: al listino prezzi perpetuo del software CSP verranno aggiunte due [](./2020-december.md#9)offerte commerciali, Get Genuine Windows e Visual Studio Professional, e offerte del settore pubblico (enti pubblici, istruzione e no profit , vedere l'annuncio).  Il listino prezzi è disponibile nella sezione Software della pagina [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) in Partner Center e verrà ripubblicato in questa data.

Per informazioni dettagliate sull'evoluzione del programma CSP e sulle modifiche al programma Open License, vedere **Passaggi successivi più** avanti.

### <a name="next-steps"></a>Passaggi successivi:

- Evoluzione del programma CSP: esaminare il [software perpetuo nei Cloud Solution Provider per l'idoneità](https://partner.microsoft.com/resources/collection/software-in-csp#/) al programma. Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.

- Modifiche al programma Open License: esaminare l'evoluzione [del programma CSP e i materiali di idoneità per](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) le modifiche al programma Open License. Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.

### <a name="questions"></a>Domande

Per altre domande, controllare le community di Yammer CSP pertinenti.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="8"></a>Aggiornamento a un annuncio precedente: Premium assessments, un componente aggiuntivo per Compliance Manager

### <a name="categories"></a>Categorie

- Data: 15/03/2021
- Espandi il business

### <a name="summary"></a>Riepilogo

Le offerte di valutazione non dovrebbero essere elencate nel listino prezzi e verranno rimosse.

### <a name="impacted-audience"></a>Destinatari interessati

Partner che ese transazionali tramite Cloud Solution Provider

### <a name="details"></a>Dettagli

Le offerte di valutazione non dovrebbero essere state incluse nel listino prezzi. Questi verranno rimossi dal listino prezzi del 1° maggio 2021.

L'annuncio originale è [qui.](./2021-february.md#4)

### <a name="additional-resources"></a>Risorse aggiuntive

- [Microsoft 365 E5 sicurezza e conformità](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Creare e gestire valutazioni in Microsoft Compliance Manager - Microsoft 365 conformità](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Passaggi successivi

Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.

### <a name="questions"></a>Domande?

Per domande su queste offerte, controllare le community Yammer pertinenti.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="7"></a> Eseguire la migrazione delle soluzioni da Un partner commerciale (OCP) go-to-market (GTM) al marketplace commerciale Microsoft

### <a name="categories"></a>Categorie

- Data: 12/03/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

A partire dal 29 marzo 2021, inizierà a sperimentare funzionalità OCP (One Commercial Partner) limitate per il go-to-market (GTM). Si consiglia di eseguire la migrazione delle soluzioni al marketplace commerciale in Partner Center.

### <a name="impacted-audience"></a>Destinatari interessati

Co-selling delle organizzazioni con soluzioni in OCP GTM

### <a name="details"></a>Dettagli

A dicembre 2020 è iniziato il percorso dallo strumento Microsoft OCP GTM al marketplace commerciale Microsoft in Partner Center. Questa transizione espande le funzionalità del marketplace commerciale in cui è possibile presentare le soluzioni a milioni di clienti, condividere opportunità bidirezionali con altri venditori Microsoft e partner e vendere insieme soluzioni innovative.

L'attività cardine successiva della transizione avrà luogo il 29 marzo 2021. Questo è il momento in cui si inizieranno a sperimentare funzionalità OCP GTM limitate, con alcuni campi che diventano di sola lettura. Se attualmente si sta co-selling con soluzioni in OCP GTM, è necessario eseguire la migrazione delle soluzioni al marketplace commerciale per sfruttarne le funzionalità e semplificare l'esperienza di pubblicazione.

Il passaggio al marketplace commerciale rende Partner Center destinazione principale per l'esperienza di pubblicazione del co-selling. È qui che è possibile continuare a far crescere l'azienda connettendo le soluzioni ai clienti condivisi tramite gli stessi canali e le esperienze all'interno del prodotto usate per i prodotti Microsoft. [Altre informazioni sul marketplace commerciale.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Passaggi successivi

- Se le soluzioni non sono ancora state spostate, seguire le istruzioni dettagliate nella guida alla transizione o visualizzare l'esercitazione [video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) dettagliata per completare tutte le attività di migrazione e iniziare a pubblicare le soluzioni nel marketplace commerciale. [](/azure/marketplace/co-sell-solution-migration)

- Per domande sull'esperienza di funzionalità limitate in OCP GTM, vedere i requisiti di [co-selling](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf)da pubblicare nelle domande frequenti sul Marketplace commerciale Microsoft. Vedere la sezione "Funzionalità limitate di OCP GTM a partire dal 29 marzo 2021".

### <a name="questions"></a>Domande?

Per [domande](https://partner.microsoft.com/support/?stage=1) o per altre informazioni, contattare il supporto tecnico.

________________
## <a name="programmatic-access-to-commercial-marketplace-analytics"></a><a name="6"></a>Accesso a livello di codice all'analisi del marketplace commerciale

### <a name="categories"></a>Categorie

- Data: 2021-03-10
- Funzionalità

### <a name="summary"></a>Riepilogo

I partner possono ora accedere ai report di analisi a livello di codice per monitorare le vendite, valutare le prestazioni e ottimizzare le offerte nel marketplace commerciale.

### <a name="impacted-audience"></a>Destinatari interessati

Partner con offerte nel marketplace commerciale.

### <a name="details"></a>Dettagli

L'API per l'accesso ai report del marketplace commerciale consente di pianificare report personalizzati dei dati di analisi in modo asincrono.

La funzionalità consente di definire query e modelli di report in base alle esigenze, impostare una pianificazione e ottenere report affidabili e in tempo reale a intervalli pianificati.

### <a name="next-steps"></a>Passaggi successivi

Per altre informazioni, vedere [Introduzione all'accesso a livello di codice all'analisi.](/azure/marketplace/analytics-get-started)

### <a name="questions"></a>Domande?

Per [altre domande,](https://go.microsoft.com/fwlink/?linkid=2165533) contattare il supporto tecnico.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Espansione della nuova esperienza commerciale nel programma Cloud Solution Provider (CSP) per Azure in Russia

### <a name="categories"></a>Categorie

- Data: 2021-03-10
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner in Russia che esitono transazioni tramite il Cloud Solution Provider (CSP).

### <a name="details"></a>Dettagli

A partire dal 10 marzo 2021, siamo entusiasti di annunciare la disponibilità della nuova esperienza commerciale **in CSP per Azure in Russia.** Questa esperienza semplifica e migliora il modo in cui i clienti acquistano e utilizzano i servizi di Azure. Offrirà inoltre ai partner del programma CSP una visualizzazione coerente dei prezzi di Azure tra i movimenti di vendita, i prezzi in USD per la coerenza globale, l'allineamento della data di fatturazione e l'accesso alle Gestione costi di Azure.

### <a name="next-steps"></a>Passaggi successivi

Sono disponibili diverse risorse che introducono la nuova esperienza commerciale di Azure e forniscono informazioni aggiuntive. Per domande frequenti, mazzi, video e altro ancora, vedere [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partner Center codice di licenza software e download fulfillment

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

La Partner Center di download del software e la funzionalità di adempimento della chiave di licenza è stata ripristinata.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti Cloud Solution Provider partner CSP (Transactal and Server Subscription Software Orders) tramite Partner Center

### <a name="details"></a>Dettagli

In risposta ai commenti e suggerimenti dei partner, viene ripristinata la capacità Partner Center di adempimento per ottenere software e chiavi di licenza per gli ordini software di sottoscrizione perpetua e server. Verrà ripristinato allo stato precedente prima di essere rimosso il 19 gennaio 2021. Vedere [l'annuncio](2020-september.md#17).

Si noti che le chiavi di licenza software e i collegamenti di download sono asset di proprietà intellettuale preziosi e molto ricercati. Se utenti malintenzionati ne entrassero in possesso, i limiti di attivazione previsti potrebbero venire raggiunti rapidamente, con conseguenti ripercussioni negative sull'esperienza di utilizzo per clienti e partner.

### <a name="next-steps"></a>Passaggi successivi

Per istruzioni sull'utilizzo e indicazioni importanti sulla distribuzione delle chiavi software, vedere le risorse seguenti:

- [Vendere software locale tramite il programma CSP](../csp-on-premise-software.md)
- [Partner Center nuova Guida operativa di Commerce](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (vedere la sezione Indicazioni sulla distribuzione delle **chiavi** software).

### <a name="questions"></a>Domande?

Per altre domande su questo avviso, controllare le community Yammer pertinenti.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Eseguire la migrazione delle offerte da Partner Sales Connessione (PSC) a Partner Center

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

Partner Sales Connessione (PSC) verrà spostato all'accesso di sola lettura a partire dal 31 marzo 2021, quindi è necessario iniziare a eseguire la migrazione delle offerte da PSC a Partner Center.

### <a name="impacted-audience"></a>Destinatari interessati

Partner con trattative in PSC

### <a name="details"></a>Dettagli

Nell'ambito dell'impegno condiviso per la crescita, il **co-selling** con Microsoft è il percorso per **scoprire,** offrire le proprie competenze ed espandere il footprint dei clienti per ottenere risultati positivi per i clienti. Con un'offerta media **3,5** volte più veloce del normale, la gestione dell'esperienza di co-selling in Partner Center consente di vendere attraverso i canali di vendita diretta di clienti, partner e venditori Microsoft e gestire l'intera pipeline di segnalazione in un'unica posizione.

**PSC** passa  all'accesso in sola lettura a partire dal **31 marzo 2021,** pertanto è necessario iniziare il passaggio a Partner Center e accedere a questi miglioramenti delle funzionalità: 

- **Routing più accurato** delle offerte che si condividono con Microsoft al venditore corretto, in base al tipo di assistenza necessaria.
- **Convalida anticipata** dell'idoneità alle trattative per le soluzioni idonee agli incentivi e per soddisfare i criteri del programma ISV Connessione, semplificando il processo di approvazione e l'attestazione finale della prova di esecuzione (POE).
- **Esperienza utente facile per** gestire tutte le opportunità di co-selling e i lead qualificati per le vendite in un'unica posizione.

Di recente sono state aggiunte anche nuove funzionalità in Partner Center per facilitare lo spostamento:

- [Operazioni bulk per opportunità di co-selling](../bulk-operations.md)
- [Funzionalità di migrazione delle trattative](../psc-to-pc.md) (vedere la **sezione Migrazione delle offerte PSC).**

Usando l'esperienza di co-selling in Partner Center, i team di vendita avranno più tempo per concentrarsi sul consolidamento di lead e opportunità, sulla chiusura delle trattative e sulla creazione di relazioni durevoli con i clienti.

### <a name="next-steps"></a>Passaggi successivi

Usare la Partner Center [di transizione](../psc-to-pc.md) per illustrare i passaggi per eseguire la migrazione delle offerte da PSC a Partner Center.

### <a name="questions"></a>Domande?

Per altre domande, contattare il [supporto](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nuovi prodotti e offerte di Microsoft Dynamics 365 disponibili il 1° aprile 2021

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

Il 1° aprile 2021 Microsoft lancierà diversi nuovi prodotti e offerte per il programma Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Il 1° aprile 2021 Microsoft lancierà i nuovi prodotti e le offerte seguenti:

- Power BI Premium Per utente
- Espansione geografica e segmento usl di Customer Voice and Marketing USL

**Power BI Premium Per utente**

Microsoft introdurrà le prime offerte Power BI Premium per utente. Power BI Premium attualmente viene venduto solo in un costrutto di capacità. Power BI Premium Per utente fornisce l'accesso alle funzionalità di business intelligence aziendali (BI) e di analisi. Le licenze per singoli posti flessibili si rivolge alle piccole e medie imprese.

Esaminare i [Power BI sulla versione per](/power-platform-release-plan/2020wave2/power-bi/planned-features) altre informazioni su questa offerta.


**Dettagli dell'offerta**

Si noti che il nome dell'offerta è leggermente diverso dall'anteprima del listino prezzi.

| Nome offerta | ID offerta |
| ------ |----------- |
| Power BI Premium Per utente | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium Per utente per istituti di docente | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium Per utente per studenti | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium Per utente (prezzi del personale no profit) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium Per utente Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Per utente Add-On per istituti di docente | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Per utente Add-On per studenti | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Per utente Add-On (prezzi del personale no profit) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Espansione geografica e segmento usl di Customer Voice e Marketing USL**

Come follow-up del lancio di dicembre 2020, le offerte di Dynamics 365 Customer Voice e Marketing USL sono state modificate per aggiungere nuovi paesi e altri SKU didattici e no profit.

| Nome offerta | ID offerta |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (prezzi del personale no profit) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL for Faculty | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Per altre informazioni su queste offerte, visitare le pagine seguenti:

- [Dynamics 365 Customer Service Voice home page](https://dynamics.microsoft.com/customer-voice/overview/)
- [Dynamics 365 Marketing home page](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse in questo argomento e condividere queste informazioni con gli stakeholder appropriati nell'organizzazione.  

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, controllare le community Yammer pertinenti. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Stampa universale ora disponibile in alcune suite

### <a name="categories"></a>Categorie

- Data: 03/03/2021
- Funzionalità

### <a name="summary"></a>Riepilogo

Microsoft Stampa universale sarà disponibile per la transazione entro Microsoft 365 suite e come componente aggiuntivo autonomo a partire dal 1° marzo 2021.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

[Stampa universale](https://aka.ms/universalprint) è un Microsoft 365 di stampa locale che elimina la necessità di server di stampa locali e consente ai dispositivi Windows di stampare su stampanti registrate in Azure. Sarà disponibile per la transazione a partire dal 1° marzo 2021.

I dipendenti traggono vantaggio dalla stampa senza driver, dall'individuazione semplificata delle stampanti basate sulla posizione e da un'esperienza di stampa intuitiva senza curva di apprendimento. I dispositivi aggiunti a Azure Active Directory (Azure AD) usano credenziali Azure AD esistenti per la stampa sicura. Gli amministratori gestiscono la stampa usando portale di Azure e possono connettere facilmente le stampanti con il supporto nativo per Stampa universale. Stampa universale può essere distribuito con stampanti non compatibili usando connettore Stampa universale software.

Stampa universale verrà riempito nuovamente al momento del lancio a Windows E3, A3, E5 e A5 e Microsoft 365 BP, F3, E3, A3, E5 e A5.  

**Dettagli dell'offerta**

Si noti che il nome dell'offerta è leggermente diverso dall'anteprima del listino prezzi.

| Nome offerta | ID offerta | ID materiale |
| ------ |----------- |----------- |  
| Stampa universale volume aggiuntivo (500 processi) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Stampa universale volume aggiuntivo (500 processi) per istituti di Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Stampa universale del volume (500 processi) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Stampa universale volume aggiuntivo (500 processi) per istituti di Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Passaggi successivi

Acquisire familiarità con il listino prezzi e la [Stampa universale panoramica.](/universal-print/fundamentals/universal-print-whatis) Si consiglia di condividere queste informazioni con tutti i contatti appropriati nella propria organizzazione.

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, controllare le community Yammer pertinenti.