---
title: Integrazioni di partner di Azure Marketplace
description: Scopri le soluzioni di Azure Marketplace che si integrano con l'ambiente Azure e Ottieni il collegamento alle guide di distribuzione dei partner Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691656"
---
# <a name="azure-marketplace-partner-integrations"></a>Integrazioni di partner di Azure Marketplace

Informazioni su come integrare soluzioni partner nell'ambiente Azure. Questo articolo fornisce una panoramica di ogni soluzione e i collegamenti alle guide dettagliate per la distribuzione. Le soluzioni sono elencate in ordine alfabetico. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka nel cloud Confluent

![Cloud Confluent](./media/partners/confluent-cloud.png)

Azure ti permette di eseguire l'integrazione con il cloud Confluent, oltre alle applicazioni cloud. I clienti più Fluent passano spesso tra il portale di Azure e il cloud Confluent. Ad esempio, quando un utente acquista un'offerta cloud Confluent in Azure Marketplace, è previsto che configurano un account con il cloud Confluent. Questo processo aggiunge complessità e tempo e richiede agli utenti di gestire la configurazione e le risorse tra i due portali. Per ridurre il carico di gestione tra le diverse piattaforme, Microsoft, in collaborazione con il cloud Confluent, ha creato un livello di provisioning integrato da Azure al cloud Confluent. La soluzione è disponibile in Azure Marketplace e offre un'esperienza uniforme per l'uso dell'offerta cloud Confluent in Azure

La soluzione USA un provider di risorse abilitato in Azure per effettuare il provisioning di risorse cloud confluenti. Questo consente agli utenti di accedere a flussi di eventi in tempo reale tramite l'portale di Azure, l'interfaccia della riga di comando di Azure e Azure SDK. Il cloud Confluent è proprietario ed esegue l'applicazione SaaS, che include gli ambienti, i cluster, gli argomenti, le chiavi API e i connettori gestiti.

L'integrazione completa con il cloud Confluent offre le funzionalità seguenti:

- Effettuare il provisioning di una nuova risorsa dell'organizzazione cloud Confluent dalla portale di Azure con l'infrastruttura completamente gestita.
- Semplifica la Single Sign-On da Azure al cloud confluenti con Azure Active Directory; non è necessaria alcuna autenticazione separata dal portale cloud Confluent.
- Ottieni la fatturazione unificata dei costi di consumo cloud confluenti tramite la fatturazione della sottoscrizione di Azure.
- Gestire le risorse cloud Confluent dalla portale di Azure e tenerne traccia nella pagina **tutte le risorse** , insieme alle risorse di Azure.

[Guide alla distribuzione cloud Confluent](https://docs.confluent.io/current/cloud/marketplace/index.html)

Per i problemi relativi a Confluent in Azure, vedere [https://support.confluent.io](https://support.confluent.io) . Se si è un utente per la prima volta, reimpostare la password prima di accedere al portale di supporto di Confluent. Se non si dispone di un account con Confluent, inviare un messaggio di posta elettronica a [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logo di DataDog](./media/partners/datadog.png)

Datadog offre strumenti di osservazione e sicurezza per gli utenti di Azure per comprendere l'integrità e le prestazioni delle applicazioni in ambienti ibridi e cloud diversi. Tuttavia, la configurazione delle integrazioni necessarie spesso richiede lo spostamento tra il portale di Azure e Datadog. Per semplificare la gestione della configurazione e delle risorse tra i portali, Microsoft ha collaborato con Datadog per creare una soluzione Datadog integrata in Azure. Disponibile tramite Azure Marketplace, questa soluzione offre un'esperienza uniforme per i clienti di Azure per l'uso della soluzione di monitoraggio cloud di Datadog.

Per ulteriori informazioni su questa soluzione e per iscriversi all'anteprima pubblica, vedere la [documentazione di monitoraggio di Azure](/azure/azure-monitor/platform/partners#datadog) .

## <a name="next-steps"></a>Passaggi successivi

- [Archivio online di Azure Marketplace](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: creare un account Azure](/learn/modules/create-an-azure-account/)
