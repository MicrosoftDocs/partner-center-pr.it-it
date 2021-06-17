---
title: Integrazioni per i partner di Azure Marketplace
description: Informazioni sulle Azure Marketplace che si integrano con l'ambiente Azure e ottenere un collegamento alle guide alla distribuzione dai partner Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276485"
---
# <a name="azure-marketplace-partner-integrations"></a>Integrazioni per i partner di Azure Marketplace

Informazioni su come integrare soluzioni partner nell'ambiente Azure. Questo articolo offre una panoramica di ogni soluzione e collegamenti a guide dettagliate sulla distribuzione. Le soluzioni sono elencate in ordine alfabetico. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka in Confluent Cloud

![Cloud confluente.](./media/partners/confluent-cloud.png)

Azure consente di eseguire l'integrazione con Confluent Cloud oltre alle applicazioni cloud. I clienti confluenti spesso passano tra portale di Azure e Confluent Cloud. Ad esempio, dopo che un utente ha acquistato un'offerta Confluent Cloud Azure Marketplace, è previsto che configura un account con Confluent Cloud. Questo processo aggiunge complessità e tempo e richiede agli utenti di gestire la configurazione e le risorse tra i due portali. Per ridurre il carico di gestione su più piattaforme, Microsoft, in collaborazione con Confluent Cloud, ha creato un livello di provisioning integrato da Azure a Confluent Cloud. La soluzione è disponibile in Azure Marketplace e offre un'esperienza facile per l'uso dell'offerta Confluent Cloud in Azure

La soluzione usa un provider di risorse abilitato in Azure per il provisioning delle risorse cloud confluenti. In questo modo gli utenti possono accedere allo streaming di eventi in tempo reale tramite portale di Azure, l'interfaccia della riga di comando di Azure e gli SDK di Azure. Confluent Cloud è proprietario ed esegue l'applicazione SaaS, che include ambienti, cluster, argomenti, chiavi API e connettori gestiti.

La profonda integrazione con Confluent Cloud consente le funzionalità seguenti:

- Effettuare il provisioning di una nuova risorsa dell'organizzazione Confluent Cloud dal portale di Azure con un'infrastruttura completamente gestita.
- Semplificare l'accesso Single Sign-On da Azure a Confluent Cloud con Azure Active Directory; non è necessaria alcuna autenticazione separata dal portale di Confluent Cloud.
- Ottenere la fatturazione unificata degli addebiti per l'utilizzo del cloud confluent tramite la fatturazione della sottoscrizione di Azure.
- Gestire le risorse di Confluent Cloud dal portale di Azure e tenerle traccia nella pagina **Tutte** le risorse, insieme alle risorse di Azure.

[Guide alla distribuzione di Confluent Cloud](https://docs.confluent.io/current/cloud/marketplace/index.html)

Per i problemi relativi a Confluent in Azure, vedere [https://support.confluent.io](https://support.confluent.io) . Se si è un utente per la prima volta, reimpostare la password prima di accedere al portale di supporto di Confluent. Se non si ha un account con Confluent, inviare un messaggio di posta elettronica a [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logo datadog.](./media/partners/datadog.png)

Datadog offre strumenti di osservabilità e sicurezza per consentire agli utenti di Azure di comprendere l'integrità e le prestazioni delle applicazioni in ambienti ibridi e multi-cloud. Tuttavia, la configurazione delle integrazioni necessarie spesso richiede la navigazione tra il portale di Azure e Datadog. Per semplificare la configurazione e la gestione delle risorse nei portali, Microsoft ha collaborato con Datadog per creare una soluzione Datadog integrata in Azure. Disponibile tramite il Azure Marketplace, questa soluzione offre ai clienti di Azure un'esperienza facile per usare la soluzione di monitoraggio cloud di Datadog.

Vedere la [documentazione Monitoraggio di Azure per](/azure/azure-monitor/platform/partners#datadog) altre informazioni su questa soluzione e iscriversi all'anteprima pubblica.

## <a name="next-steps"></a>Passaggi successivi

- [Azure Marketplace negozio online](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Creare un account Azure](/learn/modules/create-an-azure-account/)
