---
title: Annunci 2021 di marzo
description: 2021 annunci per il centro per i partner Microsoft, incluse nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880736"
---
# <a name="march-2021-announcements"></a>Annunci 2021 di marzo

Questa pagina fornisce gli annunci per Microsoft Partner Center per il 2021 marzo.

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correzioni apportate al 1 ° marzo 2021 elenco prezzi software perpetuo

### <a name="categories"></a>Categorie

- Data: 2021-03-23
- Offerte/mercati

### <a name="impacted-audience"></a>Destinatari interessati

Provider indiretti e partner di fatturazione diretta che trasagiscono software perpetuo nel programma Cloud Solution Provider 

### <a name="details"></a>Dettagli

Il listino prezzi per il software perpetuo pubblicato il 1 ° marzo 2021 include i mercati che non dovrebbero essere presenti. Il listino prezzi software perpetuo è stato aggiornato il 17 marzo 2021 con le correzioni. Queste correzioni sono applicabili solo a:

- ID prodotto: DF77X4D43RKT 
- Nome prodotto: aggiornamento da Windows 10 Home a Pro per Microsoft 365 Business
- Mercati rimossi o non supportati: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LC, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, UR, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Queste modifiche si applicano solo al prodotto precedente. Altri prodotti non hanno alcuna correzione. 

### <a name="next-steps-and-resources"></a>Passaggi successivi e risorse

- I partner che eseguono transazioni software perpetue dovrebbero scaricare l'elenco dei prezzi software perpetuo più recente.
- Consultare i [codici paese regione](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) per un mapping descrittivo dell'abbreviazione di due lettere ai paesi.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Versione SDK in .NET Standard (v 1.17.0)

### <a name="categories"></a>Categorie

- Data: 2021-03-23

- Funzionalità
 
### <a name="impacted-audience"></a>Destinatari interessati

Partner di fatturazione diretta e provider indiretti che partecipano al programma CSP e usano .NET SDK del Centro per i partner.

### <a name="details"></a>Dettagli

A partire dal 23 2020 marzo, i partner possono iniziare a scaricare la versione di [MicrosoftPartnerCenter. NetSDK (raccolta NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), insieme agli esempi aggiornati di [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)public Partner Center SDK. Questa versione include aggiornamenti ai metodi seguenti:

#### <a name="audit-updated-new-operation-types"></a>Controllo aggiornato: nuovi tipi di operazione

Aggiunta di nuovi [tipi di operazione](https://docs.microsoft.com/partner-center/develop/auditing-resources) per sapere quando il cliente ha approvato e terminato DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Controllo aggiornato: nuovi tipi di risorse e operazioni

Aggiunta di nuovi [tipi di risorse e operazioni](https://docs.microsoft.com/partner-center/develop/auditing-resources) per supportare lo scenario del ruolo della directory dei clienti.

- Nuovo tipo di risorsa "CustomerDirectoryRole"

- Tipi di operazione "AddUserMember" e "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Aggiornamenti dell'SDK per gli account dei clienti

- Supporto per GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- OTTENERE/Customers/{Customer-Tenant-ID}/Qualifications

- POST/Customers/{customer_id}/Qualifications? code = {validationCode}

#### <a name="additional-changes"></a>Modifiche aggiuntive

Le modifiche seguenti sono state introdotte come parte del nuovo commercio e sono attualmente disponibili per invito solo ai partner che fanno parte di M365/d365 New Commerce Experience Technical Preview. I partner che non fanno parte del nuovo Commerce Technical Preview non devono essere in grado di rilevare gli effetti e dovrebbero essere compatibili con le versioni precedenti.

- Modifiche al catalogo:

  - OTTENERE/Products/{Product-ID}/SKUS/{SKU-ID}

- Acquistare e gestire:
  - OTTENERE/customers/{customerId}/subscriptions
  - OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH/customers/{customerId}/subscriptions/{subscriptionId}
  - OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST/customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Passaggi successivi

- Scaricare la versione più recente di [MicrosoftPartnerCenter. NetSDK (raccolta NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Scaricare ed esaminare gli [esempi di GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Offerta del Marketplace commerciale CSP e incentivi FY21 CSP per le offerte idonee

### <a name="categories"></a>Categorie

- Data: 2021-03-18
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Provider indiretti e partner di fatturazione diretta nel programma Cloud Solution Provider 

### <a name="details"></a>Dettagli

I provider indiretti e i partner di fatturazione diretta nel programma Cloud Solution Provider possono vendere offerte di terze parti e ottenere un incentivo per gli sconti per ogni offerta di terze parti idonea transazionale nel centro per i partner o nel portale di Azure. L'incentivo sarà sotto forma di sconto sulle vendite fatturate per le offerte idonee ed è **disponibile fino al 30 giugno 2021**.  

Continua a conoscere questa offerta del Marketplace commerciale CSP di seguito e contatta i clienti oggi stesso per identificare le offerte giuste per consentire la continua riuscita e la trasformazione digitale.

Collaboriamo con fornitori di software indipendenti (ISV) per offrire al mercato le soluzioni SaaS e IaaS più recenti per i clienti Microsoft. Gli editori ISV hanno la possibilità di abilitare le vendite delle loro offerte tramite il canale partner Microsoft. Le offerte idonee per gli incentivi rientrano in due categorie:

- Selezionare le offerte SaaS e IaaS di terze parti con lo stato incentivate di co-selling IP di Azure. 

- Applicazioni SaaS integrate con team o almeno due app per la produttività Microsoft 365, ad esempio PowerPoint, Word, Excel, Outlook o SharePoint.

### <a name="next-steps-and-resources"></a>Passaggi successivi e risorse

- Scopri come guadagnare gli [incentivi](https://partner.microsoft.com/membership/partner-incentives) per i partner per la vendita di app del Marketplace idonee per incentivare le app idonee. Le nuove offerte vengono aggiunte ogni mese.  
- [Risorse di Cloud Solution Provider Direct Bill partner incentive](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Risorse di incentivi per provider indiretto del provider di soluzioni cloud](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Per altre informazioni sulla vendita delle app del Marketplace commerciale, vedere questa [presentazione](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) . Vedere risorse aggiuntive [qui](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Esplorare il catalogo del Marketplace commerciale nel centro per i [partner](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) o [portale di Azure](https://ms.portal.azure.com/#home)
- Usare le [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) per integrare le app nel Marketplace aziendale
- Rivolgersi agli ISV a cui si è interessati a lavorare con
- I provider indiretti devono integrarsi usando le API e i rivenditori di guide in cui si vendono le app

### <a name="questions"></a>Domande?  

Vedere [questo articolo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) per una panoramica del Marketplace commerciale nel centro per i partner.

Se è necessaria assistenza aggiuntiva, è possibile creare una richiesta di supporto nel centro per i partner. Ulteriori informazioni sono disponibili all'indirizzo [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Nome dell'offerta Power BI Premium e aggiornamento dei prerequisiti

### <a name="categories"></a>Categorie

- Data: 2021-03-18
- Funzionalità

### <a name="summary"></a>Riepilogo

L'elenco dei prezzi finale del 1 ° aprile 2021 verrà aggiornato per aggiungere chiarezza alla denominazione e/o alle informazioni sui prerequisiti per le offerte Power BI Premium per utente.

### <a name="impacted-audience"></a>Destinatari interessati

Partner Cloud Solution Provider (CSP) diretti e indiretti

### <a name="details"></a>Dettagli

L'elenco dei prezzi finale del 1 ° aprile 2021 verrà aggiornato per aggiungere chiarezza alla denominazione e/o alle informazioni sui prerequisiti per le offerte Power BI Premium per utente.

Fino a quando non viene aggiornato l'elenco dei prezzi finale, utilizzare le informazioni contenute in questa sezione per assicurarsi che venga ordinato il prodotto corretto.

I dettagli seguenti mostrano lo SKU e i dettagli dei prerequisiti interessati.

| Nome visualizzato dell'offerta il 1 ° marzo elenco prezzi anteprima |  Nome visualizzato dell'offerta aggiornata l'elenco dei prezzi finale del 1 ° aprile| ID offerta |
| ------ | ----------- | ----------- |
| Power BI Premium per Add-On utente (prezzi per il personale non profit)  |  Power BI Premium per Add-On utente **(Office)** (prezzi per il personale non profit)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Per acquistare questa offerta, è necessario che i clienti abbiano uno dei prerequisiti seguenti:

| Nome visualizzato dell'offerta | ID offerta |
| ------ | ----------- |
| Microsoft 365 E5 (prezzi per il personale non profit)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 senza conferenza audio (prezzi del personale no profit)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (prezzi per il personale non profit)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Versione di valutazione di Office 365 E5 (prezzi per il personale non profit)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 senza conferenza audio (prezzi del personale no profit)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Il Power BI Premium offerta seguente ha un prerequisito necessario per l'acquisto:

| Nome visualizzato dell'offerta | ID offerta |
| ------ | ----------- |
|   Power BI Premium per Add-On utente (prezzi per il personale non profit)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

I clienti devono disporre di questo prerequisito per acquistare questa offerta:

| Nome visualizzato dell'offerta | ID offerta |
| ------ |----------|
| Power BI Pro (prezzi per il personale non profit)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Passaggi successivi

Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.  

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, consultare le community Yammer pertinenti. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Aggiornamenti dei prezzi di marzo per Microsoft 365 F3

### <a name="categories"></a>Categorie

- Data: 2021-03-16
- Offerte/mercati

### <a name="summary"></a>Riepilogo

I prezzi di marzo 2021 non corretti sono stati corretti per Microsoft 365 F3 British Pound (GBP) ed euro (EUR).

### <a name="impacted-audience"></a>Destinatari interessati

Partner che acquistano Microsoft 365 F3 in GBP o EUR tra il 1 ° marzo e il 17 marzo 2021 tramite il programma Cloud Solution Provider (CSP).

### <a name="details"></a>Dettagli

Microsoft ha risolto i prezzi non corretti per Microsoft 365 F3. I prezzi non corretti erano per GBP ed EUR e solo per le offerte acquistate tra il 1 ° marzo e il 17 marzo 2021. Le offerte e le valute interessate sono elencate di seguito. 

| Nome offerta | Valuta | ID offerta | ID materiale |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (carità) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (commerciale) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Gli elenchi prezzi di base per le licenze di marzo e aprile sono stati aggiornati il 16 marzo alle 17.00 ora solare Pacifico.

### <a name="next-steps"></a>Passaggi successivi

- I partner devono riscaricare gli elenchi prezzi correnti in base alla licenza, sia marzo sia l'anteprima di aprile, con queste correzioni dei prezzi, se applicabile.  
- Microsoft contatterà i partner interessati nelle prossime settimane via posta elettronica per informarli dei passaggi successivi relativi alla correzione delle transazioni interessate.

### <a name="questions"></a>Domande?

Per altre domande, consultare le community Yammer CSP pertinenti.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Aggiornare un nome di società legale tramite il centro per i partner

### <a name="categories"></a>Categorie

- Data: 2021-03-16
- Efficienza dell'unità & scalabilità

### <a name="summary"></a>Riepilogo

A partire dal 2021 marzo, i partner di Microsoft Partner Network (MPN) e i rivenditori indiretti del provider di soluzioni cloud (CSP) possono aggiornare il nome della società legale tramite il centro per i partner.

### <a name="impacted-audience"></a>Destinatari interessati

Partner MPN e rivenditori indiretti CSP (non applicabili ai partner per la fatturazione diretta CSP)

### <a name="details"></a>Dettagli

A partire dal 2021 marzo, i partner MPN e i rivenditori indiretti CSP possono aggiornare il nome della società legale tramite il centro per i partner in modo conforme e autonomo. Grazie a questa nuova funzionalità, i partner non dovranno più inviare un ticket di supporto per il centro per i partner per aggiornare il nome della società. Ciò consentirà ai partner un notevole risparmio in termini di tempo per l'esecuzione di queste attività. 

Per altre informazioni, vedere [aggiornare il profilo aziendale legale](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Verificare che il nome della società nel profilo aziendale legale sia privo di errori di ortografia e abbreviazioni e corrisponda esattamente ai record di registrazione aziendali formali. Per ulteriori informazioni sull'aggiornamento del profilo dell'organizzazione, fare riferimento a [verificare il profilo dell'organizzazione](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Passaggi successivi

Condividere queste informazioni all'interno dell'organizzazione in modo che il team appropriato possa rivedere e aggiornare i processi.

### <a name="questions"></a>Domande?

Per altre domande, consultare le community Yammer CSP pertinenti.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Aggiornamento all'evoluzione del programma Cloud Solution Provider (CSP) e alle modifiche al programma Open License

### <a name="categories"></a>Categorie

- Data: 2021-03-15
- Funzionalità

### <a name="summary"></a>Riepilogo

Le nuove offerte software perpetue per il settore commerciale e pubblico sono in arrivo al programma Cloud Solution Provider (CSP) insieme alle modifiche apportate al programma di licenza Open.

### <a name="impacted-audience"></a>Destinatari interessati

Distributori commerciali e rivenditori gestiti che vendono attraverso il programma di licenza Open, nonché tutti i partner CSP che trasformano software perpetuo

### <a name="details"></a>Dettagli

Nel settembre 2020, Microsoft [ha annunciato](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) una serie di passaggi del processo di trasformazione digitale per ampliare le opportunità ai partner del programma CSP, inclusa la disponibilità di software locale per i partner. Queste modifiche consentono ai partner di far crescere la propria azienda ed estendere la propria copertura sfruttando le licenze software in CSP, inserendole in modo da avere successo nel mondo odierno. Consentono inoltre di consentire ai clienti di passare al cloud e fornire ai partner la flessibilità necessaria per gli ambienti cloud ibridi del cliente.

Nella continuazione di questa trasformazione digitale sono state annunciate le modifiche seguenti:

- 1 ° luglio 2021: non verranno aggiunti nuovi SKU, prodotti o promozioni al listino prezzi del programma Open License.

- 7 luglio 2021: due offerte commerciali, ottenere Windows e Visual Studio Professional originali e le offerte di settore pubblico (Government, Education e No [profit) verranno](./2020-december.md#9)aggiunte all'elenco dei prezzi software perpetuo CSP.  Il listino prezzi è disponibile nella sezione software della pagina [Sell > pricing & offers](https://partnercenter.microsoft.com/pcv/sales) nel centro per i partner e verrà ripubblicato a tale data.

Per informazioni dettagliate sull'evoluzione del programma CSP e sulle modifiche al programma Open License, vedere i **passaggi successivi** .

### <a name="next-steps"></a>Passaggi successivi:

- Evoluzione del programma CSP: esaminare il [software perpetuo nei materiali di conformità del programma Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) . Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.

- Apri modifiche del programma di licenza: esaminare l' [evoluzione del programma CSP e i materiali di idoneità Open License changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) . Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.

### <a name="questions"></a>Domande

Per altre domande, consultare le community Yammer CSP pertinenti.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Aggiornamento a un annuncio precedente: valutazioni Premium, un componente aggiuntivo per Compliance Manager

### <a name="categories"></a>Categorie

- Data: 2021-03-15
- Espandi il business

### <a name="summary"></a>Riepilogo

Le offerte di valutazione non dovrebbero essere elencate nell'elenco prezzi e verranno rimosse.

### <a name="impacted-audience"></a>Destinatari interessati

Partner che trasagiscono tramite Cloud Solution Provider

### <a name="details"></a>Dettagli

Le offerte di valutazione non dovrebbero essere state incluse nell'elenco prezzi. Questi verranno rimossi dall'elenco dei prezzi del 1 ° maggio 2021.

L'annuncio originale è [qui](./2021-february.md#4).

### <a name="additional-resources"></a>Risorse aggiuntive

- [Sicurezza e conformità di Microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Compilare e gestire valutazioni in Microsoft Compliance Manager-Microsoft 365 conformità](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Passaggi successivi

Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.

### <a name="questions"></a>Domande?

Per domande su queste offerte, consultare le community Yammer pertinenti.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Esegui la migrazione delle tue soluzioni da un partner commerciale (OCP) go-to-Market (GTM) a Microsoft Commercial Marketplace

### <a name="categories"></a>Categorie

- Data: 2021-03-12
- Funzionalità

### <a name="summary"></a>Riepilogo

Dal 29 marzo 2021, si inizierà a provare a usare le funzionalità limitate di un partner commerciale (GTM). Ti invitiamo a eseguire la migrazione delle tue soluzioni al Marketplace commerciale nel centro per i partner.

### <a name="impacted-audience"></a>Destinatari interessati

Co-selling delle organizzazioni con soluzioni in OCP GTM

### <a name="details"></a>Dettagli

Nel dicembre 2020 abbiamo iniziato il nostro viaggio dallo strumento Microsoft OCP GTM a Microsoft Commercial Marketplace nel centro per i partner. Questa transizione espande le funzionalità del Marketplace commerciale, in cui è possibile presentare le soluzioni a milioni di clienti, condividere in modo bidirezionale le opportunità con altri venditori Microsoft e partner e vendere congiuntamente soluzioni innovative.

L'attività cardine successiva della transizione verrà eseguita il 29 marzo 2021. Questo è il momento in cui si iniziano a provare le funzionalità GTM OCP limitate, con alcuni campi che diventano di sola lettura. Se attualmente si condivide con le soluzioni in OCP GTM, si consiglia di eseguire la migrazione delle soluzioni al Marketplace commerciale per sfruttare le funzionalità e semplificare l'esperienza di pubblicazione. 

Il passaggio al Marketplace commerciale rende il centro partner la destinazione principale per l'esperienza di pubblicazione di co-selling. Puoi continuare a far crescere il tuo business connettendo le tue soluzioni con i nostri clienti condivisi attraverso gli stessi canali e le tue esperienze del prodotto usate per i prodotti Microsoft. [Scopri di più sul Marketplace commerciale](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Passaggi successivi

- Se non sono state ancora spostate le soluzioni, seguire le istruzioni riportate nella [Guida alla transizione](/azure/marketplace/co-sell-solution-migration) o visualizzare l'esercitazione dettagliata del [video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) per completare tutte le attività di migrazione e iniziare a pubblicare le soluzioni nel Marketplace commerciale.

- Per domande sull'esperienza limitata in OCP GTM, vedere i [requisiti di co-selling per la pubblicazione nelle domande frequenti su Microsoft Commercial Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). Vedere la sezione "OCP GTM Limited capabilities a partire dal 29 marzo 2021".

### <a name="questions"></a>Domande?

Per eventuali domande o per richiedere ulteriori informazioni, contattare il [supporto tecnico](https://partner.microsoft.com/support/?stage=1) .

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Ampliamento della nuova esperienza commerciale nel programma Cloud Solution Provider (CSP) per Azure in Russia

### <a name="categories"></a>Categorie

- Data: 2021-03-10
- Funzionalità

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner in Russia che operano attraverso il programma Cloud Solution Provider (CSP).

### <a name="details"></a>Dettagli

A partire da marzo 10 2021, siamo lieti di annunciare la disponibilità della **nuova esperienza commerciale in CSP per Azure in Russia**. Questa esperienza semplifica e migliora il modo in cui i clienti acquistano e utilizzano i servizi di Azure. Fornirà inoltre ai partner del programma CSP una visualizzazione coerente dei prezzi di Azure tra i movimenti di vendita, i prezzi USD per la coerenza globale, l'allineamento della data di fatturazione e l'accesso a gestione costi di Azure.

### <a name="next-steps"></a>Passaggi successivi

Sono disponibili diverse risorse che introducono la nuova esperienza di Azure Commerce e forniscono informazioni aggiuntive. Trovare le domande frequenti, i deck, i video e altro ancora più recenti nella [raccolta di risorse aggiornamenti del programma CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Codice di licenza software per il centro per i partner e evasione del download

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

Il download e la funzionalità di evasione delle chiavi di licenza del centro per i partner sono stati ripristinati.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner Cloud Solution Provider (CSP) che tramandano gli ordini software di abbonamento perpetuo e server tramite il centro per i partner

### <a name="details"></a>Dettagli

In risposta ai commenti dei partner, la funzionalità di evasione del centro per i partner viene ripristinare per ottenere il software e i codici di licenza per gli ordini software di abbonamento perpetuo e server. Verrà ripristinato lo stato precedente prima di essere rimosso il 19 gennaio 2021. Vedere l' [annuncio](2020-september.md#17).

Si noti che le chiavi di licenza software e i collegamenti di download sono asset di proprietà intellettuale preziosi e fortemente ricercati. Se utenti malintenzionati ne entrassero in possesso, i limiti di attivazione previsti potrebbero venire raggiunti rapidamente, con conseguenti ripercussioni negative sull'esperienza di utilizzo per clienti e partner.

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse seguenti per istruzioni sull'utilizzo e indicazioni importanti sulla distribuzione di chiavi software:

- [Vendere software locale tramite il programma CSP](../csp-on-premise-software.md)
- [Guida operativa di New Commerce](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) per il centro per i partner (vedere la sezione **linee guida sulla distribuzione di chiavi software** ).

### <a name="questions"></a>Domande?

In caso di ulteriori domande su questa comunicazione, consultare le community Yammer pertinenti.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Esegui la migrazione delle tue offerte da partner Sales Connect (PSC) al centro per i partner

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

Partner Sales Connect (PSC) passerà all'accesso in sola lettura a partire dal 31 marzo 2021, quindi si consiglia di iniziare la migrazione delle proprie offerte da CPS al centro per i partner.

### <a name="impacted-audience"></a>Destinatari interessati

Partner con deals in PSC

### <a name="details"></a>Dettagli

Nell'ambito del nostro impegno condiviso verso la crescita, la **co-selling con Microsoft** è il percorso che ti permette di individuare **, offrire le tue competenze e ampliare il footprint dei clienti** per ottenere risultati positivi per i clienti. Con una media di **3,5 volte più veloce** rispetto al normale, la gestione dell'esperienza di co-selling nel centro per i partner ti permette di vendere attraverso i canali diretti per clienti, partner e venditori Microsoft e di gestire l'intera pipeline di riferimento in un'unica posizione.

**PSC** passerà all' **accesso** in sola lettura a partire dal **31 marzo 2021**, quindi si consiglia di iniziare il passaggio al centro per i partner e accedere a questi miglioramenti delle funzionalità: 

- **Routing più accurato** delle offerte condivise con Microsoft al venditore appropriato, in base al tipo di assistenza necessario.
- Ottenere in **anticipo la convalida dell'idoneità** per soluzioni idonee per gli incentivi e per soddisfare i criteri del programma di connessione ISV, semplificando il processo di approvazione e l'attestazione del certificato di esecuzione (PoE) finale.
- **Esperienza utente trasparente** per gestire tutte le opportunità di co-selling e i lead qualificati per le vendite in un'unica posizione.

Sono state recentemente aggiunte nuove funzionalità al centro per i partner per facilitare lo spostamento:

- [Operazioni bulk per opportunità di co-selling](../bulk-operations.md)
- [Funzionalità di migrazione di Deal](../psc-to-pc.md) (vedere la sezione relativa alla **migrazione delle offerte di PSC** ).

Grazie all'esperienza di co-selling nel centro per i partner, i team addetti alle vendite avranno più tempo per concentrarsi sulla gestione di lead e opportunità, sulla chiusura di offerte e sulla creazione di relazioni dei clienti durevoli.

### <a name="next-steps"></a>Passaggi successivi

Usare la guida alla [transizione](../psc-to-pc.md) del centro per i partner per illustrare i passaggi necessari per eseguire la migrazione delle proprie offerte da CPS al centro per i partner.

### <a name="questions"></a>Domande?

Per altre domande, contattare il [supporto tecnico](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nuovi prodotti e offerte Microsoft Dynamics 365 disponibili il 1 ° aprile 2021

### <a name="categories"></a>Categorie

- Data: 2021-03-04
- Funzionalità

### <a name="summary"></a>Riepilogo

Il 1 ° aprile 2021, Microsoft lancerà diversi nuovi prodotti e offerte per il programma Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

Il 1 ° aprile 2021 Microsoft lancerà i nuovi prodotti e le offerte seguenti:

- Power BI Premium per utente
- Area geografica ed espansione del segmento di Customer Voice and marketing USL

**Power BI Premium per utente**

Microsoft introdurrà le prime offerte per Power BI Premium per singolo utente. Power BI Premium viene attualmente venduto solo in un costrutto di capacità. Power BI Premium per utente consente di accedere alle funzionalità di Enterprise business intelligence (BI) e di analisi. Le licenze flessibili per le singole postazioni si adattano alle aziende di piccole e medie dimensioni.

Per ulteriori informazioni su questa offerta, vedere i [Dettagli della versione Power bi](/power-platform-release-plan/2020wave2/power-bi/planned-features) .


**Dettagli dell'offerta**

Si noti che il nome dell'offerta è leggermente diverso dall'anteprima dell'elenco prezzi.

| Nome offerta | ID offerta |
| ------ |----------- |
| Power BI Premium per utente | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium per utente per i docenti | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium per utente per studenti | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium per utente (prezzi per il personale non profit) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium per utente Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Add-On per utente per i docenti | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Add-On per ogni utente per studenti | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium per Add-On utente (prezzi per il personale non profit) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Area geografica ed espansione del segmento di Customer Voice and marketing USL**

In seguito al lancio del dicembre 2020, le offerte di Dynamics 365 Customer Voice and marketing sono state modificate in modo da aggiungere nuovi paesi e SKU di formazione e non profit.

| Nome offerta | ID offerta |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (prezzi per il personale non profit) | 7a8642a5-481E-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL per istituti di facoltà | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Per ulteriori informazioni su queste offerte, visitare le pagine seguenti:

- [home page Voice del servizio clienti Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)
- [home page marketing di Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Passaggi successivi

Esaminare le risorse di questo argomento e condividere queste informazioni con le parti interessate appropriate nell'organizzazione.  

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, consultare le community Yammer pertinenti. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Universal Print ora disponibile in alcuni gruppi

### <a name="categories"></a>Categorie

- Data: 2021-03-33
- Funzionalità

### <a name="summary"></a>Riepilogo

Microsoft Universal Print sarà disponibile per le transazioni all'interno di Select Microsoft 365 suite e come componente aggiuntivo autonomo a partire dal 1 ° marzo 2021.

### <a name="impacted-audience"></a>Destinatari interessati

Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)

### <a name="details"></a>Dettagli

[Universal Print](https://aka.ms/universalprint) è un servizio di stampa Microsoft 365 che elimina la necessità di server di stampa locali e consente ai dispositivi Windows di stampare le stampanti registrate in Azure. Sarà disponibile per le transazioni a partire dall'1 marzo 2021.

I ruoli di lavoro traggono vantaggio dalla stampa senza driver, dall'individuazione di stampanti basata sulla posizione semplificata e da un'esperienza di stampa intuitiva senza alcuna curva di apprendimento. I dispositivi aggiunti a Azure Active Directory (Azure AD) utilizzano le credenziali Azure AD esistenti per la stampa in modo sicuro. Gli amministratori gestiscono la stampa tramite il portale di Azure e possono connettere facilmente le stampanti con supporto nativo per la stampa universale. La stampa universale può essere distribuita con stampanti non compatibili utilizzando il software connettore di stampa universale.

La stampa universale verrà ricaricata in fase di avvio a Windows E3, a3, E5 e a5 e Microsoft 365 BP, F3, E3, a3, E5 e a5.  

**Dettagli dell'offerta**

Si noti che il nome dell'offerta è leggermente diverso dall'anteprima dell'elenco prezzi.

| Nome offerta | ID offerta | ID materiale |
| ------ |----------- |----------- |  
| Componente aggiuntivo volume di stampa universale (500 processi)-Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Componente aggiuntivo volume di stampa universale (500 processi) per i docenti-Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Componente aggiuntivo volume di stampa universale (500 processi)-Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Componente aggiuntivo volume di stampa universale (500 processi) per i docenti-Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Passaggi successivi

Acquisire familiarità con l'elenco prezzi e la [Panoramica stampa universale](/universal-print/fundamentals/universal-print-whatis). Si consiglia di condividere queste informazioni con tutti i contatti appropriati nella propria organizzazione.

### <a name="questions"></a>Domande?

Per eventuali domande su queste offerte, consultare le community Yammer pertinenti.
