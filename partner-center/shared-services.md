---
title: Aggiungere Servizi condivisi per partner di Azure
description: USA i servizi condivisi di Azure partner per acquistare sottoscrizioni di Azure per uso personale e per avere un metodo uniforme per l'acquisto, il monitoraggio e la gestione di Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 756fbfda3438933b50fc51936b396291986472a7
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028282"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Consente di aggiungere servizi condivisi di Azure partner per consentire ai partner di acquistare sottoscrizioni di Azure per uso personale

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore
- Agente di vendita

Azure - Servizi condivisi/Carico di lavoro interno è un nuovo tipo di offerta per i partner aderenti al programma CSP che consente di acquistare sottoscrizioni di Azure per uso proprio.Consente ai partner di usare un metodo uniforme per l'acquisto, il monitoraggio e la gestione di Azure, oltre alla possibilità di consolidare le licenze di Azure e di rivendere i contratti con Microsoft. Con i servizi condivisi del partner di Azure, i partner hanno ora la stessa flessibilità di usare le sottoscrizioni di Azure in CSP come nei programmi Microsoft Contratto Enterprise e Web Direct, aprendo scenari come: compilare ambienti di sviluppo e test, distribuire carichi di lavoro interni e ospitare servizi condivisi o applicazioni multi-tenant.  

## <a name="create-the-shared-services-tenant"></a>Creare il tenant di servizi condivisi

1. Passare a **Impostazioni**  >  **account impostazioni**  >  **servizi condivisi**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Impostazioni account > servizi condivisi":::

2. Se non si dispone già di un tenant di servizi condivisi, fare clic su **Crea servizi condivisi**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Creazione di servizi condivisi":::

3. In questo modo viene creato un tenant di servizi condivisi e viene acquistata la sottoscrizione ai servizi condivisi di Azure CSP, da usare per le risorse condivise e il carico di lavoro interno.

   :::image type="content" source="images/sharedservices5.png" alt-text="Creare il tenant e acquistare la sottoscrizione":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informazioni sull'offerta Azure-Servizi condivisi/Carico di lavoro interno

- Il Azure-Servizi condivisi/Carico di lavoro interno sottoscrizione è un nuovo tipo di offerta di Azure in CSP accessibile tramite il centro per i partner che i partner ottengono per l'uso di Azure.

- Le sottoscrizioni dei servizi condivisi di Azure partner sono idonee e possono essere usate per acquistare RIs.

- L'offerta Azure-Servizi condivisi/Carico di lavoro interno può essere applicata solo al tenant dei servizi condivisi.

- L'uso principale del Azure-Servizi condivisi/Carico di lavoro interno sottoscrizione è quello di poter usare Azure per scopi di sviluppo personalizzati. Il tenant condiviso usato per il provisioning di questa offerta non può essere usato per altri servizi, ad esempio le licenze di Office 365 o Dynamics.

- È possibile annullare la sottoscrizione come qualsiasi altra sottoscrizione. Passare a **Impostazioni**  >  **Visualizza tutte le impostazioni**  >  **servizi condivisi**. Selezionare la sottoscrizione Azure-Servizi condivisi/Carico di lavoro interno e annullarla.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Accesso ai dettagli sull'utilizzo dei servizi condivisi di Azure partner

Il consumo di Azure viene trovato nella fattura CSP e nel file di riconciliazione. Verrà incluso come parte dell'elemento Microsoft Azure riga della fattura. Le informazioni dettagliate sul consumo saranno disponibili nel file di riconciliazione registrato rispetto al tenant creato per questa offerta.

## <a name="azure-partner-shared-services-pricing"></a>Prezzi dei servizi condivisi di Azure partner

Per visualizzare il nuovo file dei prezzi per i servizi condivisi di Azure partner, vai a **vendere**  >  **prezzi e offerte** e seleziona l'elenco prezzi del mese corrente. Nelle prossime settimane verrà rilasciata anche un'API specifica della scheda tariffaria.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Offerte Marketplace e servizi condivisi di Azure partner

A partire dal 1 ° marzo 2019, Azure partner Shared Services (APSS) non supporta più le offerte del Marketplace.

|**Supporto per Marketplace**   |**APSS supportato prima del 1 ° marzo 2019**|**Dopo il 1 ° marzo 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring Your Own License (BYOL) e servizi gratuiti   | Sì   | No|
|Altre offerte del Marketplace di terze parti   | No   |No|

I partner con BYOL o servizi gratuiti distribuiti con APSS non saranno interessati. Tuttavia, dopo il 1 ° marzo 2019 non saranno in grado di acquistare nuovi servizi BYOL o free.

Per sfruttare i vantaggi del catalogo completo delle offerte Marketplace disponibili (non solo BYOL e servizi gratuiti), è consigliabile distribuire i servizi condivisi usando le sottoscrizioni di Azure dirette tramite Web.  I partner CSP che hanno distribuito in precedenza risorse di BYOL e servizi gratuiti di terze parti dal Marketplace e desiderano continuare a usarle e distribuire più offerte di terze parti sono invitati a eseguire la migrazione della sottoscrizione di APSS alla [migrazione di sottoscrizioni di Azure esistenti](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

I partner, che pianificano di continuare a usare la sottoscrizione di APSS dopo il 1 ° marzo 2019 e vogliono distribuire nuovi servizi [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) di terze parti o servizi gratuiti, possono seguire le istruzioni fornite dagli ISV per distribuirle nelle sottoscrizioni apss.

## <a name="next-steps"></a>Passaggi successivi

- [Vendere abbonamenti software tramite CSP](csp-software-subscriptions.md)