---
title: Gestire sottoscrizioni e risorse nel piano di Azure | Centro per i partner
ms.topic: article
ms.date: 11/01/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Acquistare più sottoscrizioni di Azure nel piano di Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: ededae0c8e8212697648cda2c00f23fd457fa877
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653858"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Gestire sottoscrizioni e risorse nel piano di Azure

Quando esegui la transizione di un cliente al piano di Azure, per impostazione predefinita in Azure ti vengono assegnati i diritti di amministratore con privilegi (diritti del proprietario della sottoscrizione tramite l'opzione di amministratore per conto terzi).

 > [!NOTE]
 > I diritti di amministratore sulla sottoscrizione di Azure possono essere rimossi dal cliente a livello di sottoscrizione, gruppo di risorse o carico di lavoro. 

 I partner possono ottenere il controllo e la gestione operativi (24 ore su 24, 7 giorni su 7) delle risorse di Azure di un cliente in CSP usando diverse opzioni disponibili tramite la funzionalità di controllo degli accessi in base al ruolo. 

- **Amministratore per conto terzi (AOBO, Admin On Behalf Of)** : nella modalità [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) qualsiasi utente con il ruolo di agente amministratore nel tenant del partner avrà accesso come proprietario del controllo degli accessi in base al ruolo alle sottoscrizioni di Azure che crei tramite il programma CSP.

- **Azure Lighthouse**: la modalità AOBO non offre la flessibilità di creare gruppi distinti che funzionano con clienti diversi o di abilitare ruoli diversi per gruppi o utenti. Con Azure Lighthouse è possibile assegnare gruppi diversi a clienti o ruoli diversi. Poiché gli utenti avranno il livello di accesso appropriato tramite la gestione delle risorse delegata di Azure, è possibile ridurre il numero di utenti che hanno il ruolo di agente amministratore e quindi dispongono dell'accesso completo come amministratore per conto terzi. Questo consente di migliorare la sicurezza limitando l'accesso non necessario alle risorse dei clienti e inoltre offre maggiore flessibilità per la gestione di più clienti su larga scala. Per altre informazioni, leggi [Azure Lighthouse e programma Cloud Solution Provider](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).

-  **Utenti di directory, utenti guest o [Entità servizio](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** : è possibile delegare l'accesso granulare alle sottoscrizioni CSP aggiungendo utenti nella directory dei clienti oppure aggiungendo utenti guest e assegnando ruoli specifici del controllo degli accessi in base al ruolo. 

Come procedura di sicurezza, Microsoft consiglia di assegnare agli utenti le autorizzazioni minime necessarie per svolgere il loro lavoro. Vedi [Risorse di Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure). 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Collegare l'ID Partner (ID MPN) alle credenziali per la gestione delle risorse di Azure del cliente

La tabella seguente illustra i metodi usati per associare l'ID Partner alle diverse opzioni di accesso del controllo degli accessi in base al ruolo.

|**Categoria**   |**Scenario**   |**Associazione ID MPN**|
|-----------------|:------------------------|:------------------|
|Amministratore per conto terzi   |Il partner diretto o il provider indiretto CSP crea la sottoscrizione per il cliente diventando così il proprietario predefinito della sottoscrizione in base alla modalità Amministratore per conto terzi. Il partner diretto o il provider indiretto CSP concede l'accesso indiretto come rivenditore alla sottoscrizione usando la modalità Amministratore per conto terzi.|Automatica (nessun intervento necessario da parte del partner)|
|Azure Lighthouse|Il partner crea una nuova [offerta di servizi gestiti in Marketplace](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers). L'offerta viene accettata nella sottoscrizione CSP e il partner ottiene l'accesso alla sottoscrizione CSP.|Automatica (nessun intervento necessario da parte del partner)|
|Azure Lighthouse|Il partner distribuisce il [modello ARM](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) nella sottoscrizione di Azure.|Il partner deve associare l'ID MPN all'entità servizio o all'utente nel tenant del partner. Per altre informazioni, vedi [Collegare un ID Partner](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|
|Utenti di directory o utente guest|Il partner crea un nuovo utente o un'entità servizio nella directory del cliente e concede all'utente l'accesso alla sottoscrizione CSP. Il partner crea un nuovo utente o una nuova entità servizio nella directory del cliente. Partner aggiunge l'utente a un gruppo e concede al gruppo l'accesso alla sottoscrizione CSP.|Il partner deve associare l'ID MPN all'entità servizio o all'utente nel tenant del cliente. Per altre informazioni, vedi [Collegare un ID Partner](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Verificare di disporre dell'accesso come amministratore

Per gestire i servizi del cliente e ricevere i crediti ottenuti devi disporre dell'accesso come amministratore. Leggi [Crediti ottenuti dai partner](partner-earned-credit.md) per ottenere informazioni dettagliate sui crediti ottenuti. Esistono due modi per verificare di disporre dell'accesso come amministratore.

- Esaminare il file sull'utilizzo giornaliero: per eseguire questa verifica, esamina il prezzo unitario e il prezzo unitario effettivo nel file sull'utilizzo giornaliero e controlla se viene applicato uno sconto. Se ricevi lo sconto, significa che sei l'amministratore.

- Creare un avviso di monitoraggio di Azure: puoi creare un [avviso](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) del log attività di Monitoraggio di Azure per ricevere una notifica quando l'accesso assegnato dal controllo degli accessi in base al ruolo viene rimosso dalla sottoscrizione CSP.

### <a name="create-an-azure-monitor-alert"></a>Creare un avviso di Monitoraggio di Azure

1. Crea un avviso.

![avviso di Azure](images/azure/azurealert1.png)

2. Seleziona il tipo di azione che dovrà essere eseguita dall'avviso. Se, ad esempio, scegli un messaggio di posta elettronica, riceverai un messaggio di notifica dell'eliminazione di un'assegnazione di ruolo.

![configurare l'avviso](images/azure/azureconfigurealert2.png)

### <a name="aobo-removal"></a>Rimozione dell'accesso come Amministratore per conto terzi

I clienti possono gestire l'accesso alle rispettive sottoscrizioni tramite la funzionalità **Controllo di accesso** nel portale di Azure. Nella scheda **Assegnazioni ruolo** possono selezionare **Rimuovi accesso**. In questo caso, puoi:

- Parlare con il cliente per verificare se l'accesso amministratore può essere ripristinato.
- Usare l'accesso fornito tramite il [controllo degli accessi in base al ruolo](https://docs.microsoft.com/azure/role-based-access-control/overview).
- Usare l'accesso fornito tramite [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

L'accesso in base al ruolo è diverso dall'accesso amministratore. I ruoli delimitano in modo preciso le operazioni consentite e non. L'accesso amministratore è più ampio.

Per visualizzare i ruoli idonei al credito ottenuto dai partner, leggi [Ruoli e autorizzazioni per il credito ottenuto dai partner](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).




**Per altre informazioni**

- [Revocare e ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](revoke-reinstate-csp.md)

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)

- [Credito ottenuto dai partner per i servizi gestiti](partner-earned-credit-explanation.md)