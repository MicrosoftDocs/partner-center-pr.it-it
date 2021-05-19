---
title: Iscriversi come CPV (Control Panel Vendor)
description: Informazioni su come eseguire la registrazione come fornitore Pannello di controllo (CPV) in Partner Center in modo da poter integrare meglio i sistemi partner CSP con Partner Center API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147140"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a>Iscriversi come fornitore del pannello di controllo per integrare i sistemi di partner CSP con le API del Centro per i partner


**Ruoli appropriati**: Amministratore globale

Un Pannello di controllo Vendor (CPV) è un fornitore di software indipendente che sviluppa applicazioni per l'uso da parte di partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con Partner Center API. Un Pannello di controllo fornitore non è un partner CSP con accesso diretto al dashboard Partner Center o alle API Partner Center client.

Sia che si sia un fornitore di Pannello di controllo (CPV) o un nuovo CPV che vuole collaborare con i partner Microsoft, Microsoft richiede ora la registrazione a Partner Center per registrare le applicazioni e supportare i partner Cloud Solution Provider. Per creare un account, un partner CPV può usare un tenant partner CSP esistente o un tenant CPV esistente oppure creare un nuovo tenant come parte del processo di onboarding. Se il partner CPV sceglie di usare il tenant CSP esistente, dovrà creare applicazioni multi-tenant separate e registrarle in Partner Center per le attività CPV. Un'applicazione non può essere registrata come applicazione CSP e CPV. Dopo aver registrato in Partner Center e registrato le applicazioni, si avrà accesso alle API Partner Center applicazioni.  Contattare Microsoft tramite una Supporto tecnico Microsoft richiesta se è necessario un account sandbox. Se si ha già un account sandbox, continuare a usarlo. Non sarà necessaria una nuova sandbox

Esaminare il [contratto microsoft Pannello di controllo vendor](https://go.microsoft.com/fwlink/?linkid=2055198)


## <a name="working-in-partner-center"></a>Lavorare nel Centro per i partner

Dopo aver registrato l'esperienza Partner Center CPV e aver accettato il contratto CPV, è possibile:

- Gestire applicazioni multi-tenant (aggiungere applicazioni per portale di Azure, registrare e annullare la registrazione delle applicazioni in Partner Center).

    >[!Note] 
    >I CPV devono registrare le applicazioni in Partner Center per ottenere l'autorizzazione per Partner Center API. La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner. 

- Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo 

- Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo. L'amministratore globale è l'unico ruolo che un CPV può avere.

## <a name="next-steps"></a>Passaggi successivi

-[Aggiungere altri tenant all'account Partner Center locale](multi-tenant-account.md)