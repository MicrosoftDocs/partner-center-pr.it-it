---
title: Aggiungere Servizi condivisi per partner di Azure
description: Usare Servizi condivisi per partner di Azure per acquistare sottoscrizioni di Azure per uso personale e avere un metodo uniforme per l'acquisto, il rilevamento e la gestione di Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855336"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Aggiungere Servizi condivisi per partner di Azure in modo che i partner possano acquistare sottoscrizioni di Azure per uso personale

**Ruoli appropriati:** Amministratore globale | Agente amministratore | Agente di vendita

Azure - Servizi condivisi/Carico di lavoro interno è un nuovo tipo di offerta per i partner aderenti al programma CSP che consente di acquistare sottoscrizioni di Azure per uso proprio.Consente ai partner di usare un metodo uniforme per l'acquisto, il rilevamento e la gestione di Azure, oltre alla possibilità di consolidare i contratti di licenza e rivendita di Azure con Microsoft. Con Servizi condivisi per partner di Azure, i partner hanno ora la stessa flessibilità di usare le sottoscrizioni di Azure in CSP come nei programmi Microsoft Contratto Enterprise e Web Direct, aprendo scenari come la creazione di ambienti di sviluppo e test, la distribuzione di carichi di lavoro interni e l'hosting di servizi condivisi o applicazioni multi-tenant.  

## <a name="create-the-shared-services-tenant"></a>Creare il tenant dei servizi condivisi

1. Passare a **Impostazioni**  >  **Impostazioni Account Servizi**  >  **condivisi**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Impostazioni dell'account > servizi condivisi":::

2. Se non si dispone già di un tenant di servizi condivisi, fare clic **su Crea servizi condivisi**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Creare servizi condivisi":::

3. Viene creato un tenant di servizi condivisi e viene acquistata la Azure CSP di Servizi condivisi da usare per le risorse condivise e il carico di lavoro interno.

   :::image type="content" source="images/sharedservices5.png" alt-text="Creare il tenant e acquistare la sottoscrizione":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informazioni sull'Azure - Servizi condivisi/Carico di lavoro interno offerta

- La Azure - Servizi condivisi/Carico di lavoro interno è un nuovo tipo di offerta di Azure in CSP accessibile tramite Partner Center che i partner ottengono per il proprio uso di Azure.

- Servizi condivisi per partner di Azure le sottoscrizioni sono idonee e possono essere usate per acquistare le richieste pull.

- L Azure - Servizi condivisi/Carico di lavoro interno'offerta può essere applicata solo al tenant dei servizi condivisi.

- L'uso principale per la Azure - Servizi condivisi/Carico di lavoro interno è in modo che sia possibile usare Azure per scopi di sviluppo personalizzati. Il tenant condiviso usato per effettuare il provisioning di questa offerta non può essere usato per altri servizi, ad esempio licenze di Office 365 o Dynamics.

- È possibile annullare la sottoscrizione come qualsiasi altra sottoscrizione. Passare alle impostazioni **Visualizza tutto**  >    >  **impostazioni Servizi condivisi**. Selezionare la Azure - Servizi condivisi/Carico di lavoro interno e annullarla.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Accesso ai dettagli Servizi condivisi per partner di Azure consumo

Il consumo di Azure si trova nella fattura CSP e nel file di riconciliazione. Verrà incluso come parte della Microsoft Azure riga nella fattura. Le informazioni dettagliate sul consumo saranno disponibili nel file di riconciliazione registrato nel tenant creato per questa offerta.

## <a name="azure-partner-shared-services-pricing"></a>Servizi condivisi per partner di Azure prezzi

Per visualizzare il nuovo file di prezzi Servizi condivisi per partner di Azure, passare a **Vendere** prezzi e offerte  >   e selezionare il listino prezzi del mese corrente. Nelle prossime settimane verrà rilasciata anche un'API scheda tariffa specifica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Offerte del Marketplace e Servizi condivisi per partner di Azure

A partire dal 1° marzo 2019, Servizi condivisi per partner di Azure (APSS) non supporta più le offerte del Marketplace.

|**Supporto del Marketplace**   |**APSS supportato prima del 1° marzo 2019**|**Dopo il 1° marzo 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring Your Own License (BYOL) e servizi gratuiti   | Sì   | No|
|Altre offerte del marketplace di terze parti   | No   |No|

I partner con BYOL o i servizi gratuiti distribuiti tramite APSS non saranno influenzati; tuttavia dopo il 1° marzo 2019 non potranno acquistare nuovi servizi BYOL o gratuiti.

Per sfruttare il catalogo completo delle offerte del Marketplace disponibili (non solo BYOL e servizi gratuiti), è consigliabile che i partner CSP distribuiscono servizi condivisi usando sottoscrizioni web direct di Azure.  I partner CSP che hanno distribuito in precedenza risorse di servizi GRATUITI e BYOL di terze parti dal Marketplace e che vogliono continuare a usarle e distribuire altre offerte di terze parti sono invitati a eseguire la migrazione della sottoscrizione APSS alla migrazione diretta web delle sottoscrizioni di [Azure esistenti.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

I partner, che pianificano di continuare a usare la sottoscrizione APSS dopo il 1° marzo 2019 e vogliono distribuire nuovi servizi [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) o servizi gratuiti di terze parti, possono seguire le istruzioni degli ISV per distribuirlo nelle sottoscrizioni APSS.

## <a name="next-steps"></a>Passaggi successivi

- [Vendere abbonamenti software tramite CSP](csp-software-subscriptions.md)