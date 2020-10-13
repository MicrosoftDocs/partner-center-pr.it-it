---
title: Trasferire la sottoscrizione di Azure in un piano di Azure a un altro partner CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il partner del programma Cloud Solution provider associato alle sottoscrizioni di Azure di un cliente in un piano di Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980262"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Trasferire le sottoscrizioni di piano di Azure di un cliente a un partner diverso

## <a name="applies-to"></a>Si applica a

- Partner inclusi nel programma Cloud Solution Provider (CSP)

Questo articolo descrive come un cliente può cambiare le sottoscrizioni di Azure in un piano di Azure da un provider di soluzioni cloud (CSP) a un altro.

Per cambiare le sottoscrizioni di Azure di un cliente da un partner diverso, seguire questa procedura. Sia il partner che il cliente devono eseguire i passaggi necessari.

>[!Note]  
>Solo i partner con una relazione di fatturazione diretta con Microsoft possono accedere agli strumenti di transizione. I rivenditori indiretti devono collaborare con i provider indiretti per sfruttare questo strumento di transizione.

Il cliente deve essere in conversazione con entrambi i partner (attuali e futuri) prima che questo strumento venga usato. È necessario che una conversazione offline eviti confusione e varianza. Inoltre, i partner e i clienti devono comprendere queste considerazioni e i prerequisiti prima di avviare una transizione:

**Considerazioni principali:**

- Le prenotazioni di Azure non vengono spostate con la sottoscrizione a partner futuri
- I prezzi di CSP per i servizi di Azure in Current partner non vengono sottoposti a transizione  
- Le responsabilità del supporto per i clienti passeranno al partner futuro
- La fatturazione e la fatturazione passeranno a partner futuri al momento del trasferimento
- Il servizio di controllo di accesso (RBAC) di Azure Role-Based non è influenzato dal trasferimento
- Per impostazione predefinita, l'amministratore per conto di (AOBO) non verrà concesso al partner futuro
- I prodotti del Marketplace di terze parti vengono trasferiti fino a quando i prodotti passano il controllo di idoneità del Marketplace.
    - Non sono previsti sconti speciali o restrizioni a livello di area
    - I prodotti non sono basati su sottoscrizione
    - Il partner futuro dovrebbe collaborare con l'editore per assicurarsi che si trovino nell'elenco di elementi consentiti per la distribuzione del prodotto
    - Se non vengono soddisfatte tutte queste condizioni per trasferire i prodotti del Marketplace, è necessario annullare le sottoscrizioni di Azure e quindi riacquistare i prodotti Marketplace con il nuovo partner

**Prerequisiti:**

- Il cliente si impegna a eseguire la transizione del partner CSP corrente
- Il partner CSP futuro collabora con il cliente per garantire che le esigenze dei clienti possano essere soddisfatte
- Il partner CSP futuro stabilisce una relazione con il cliente prima dell'inizio della transizione  
- Il cliente deve firmare il contratto per i clienti Microsoft con il partner CSP futuro
- Il partner CSP futuro deve avere firmato il contratto per i partner Microsoft per usare questo strumento

## <a name="customer-tasks-to-be-completed"></a>Attività del cliente da completare

Per trasferire una sottoscrizione di Azure in un piano di Azure, il cliente deve avviare il processo contattando il partner corrente. Devono raccogliere il nome e il dominio della società del partner corrente, in modo che il partner futuro possa completare il modulo di richiesta di trasferimento per loro conto.

Il cliente deve inoltre identificare le sottoscrizioni che si desidera trasferire dal partner corrente. Non è possibile modificare i partner per le sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

>[!Note]  
>È responsabilità del partner futuro completare il modulo di richiesta di trasferimento che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del partner corrente. Il cliente deve pianificare di collaborare con il partner futuro e corrente per rendere la transizione senza problemi.

## <a name="future-partner-tasks-to-be-completed"></a>Attività future del partner da completare

Il partner futuro della sottoscrizione deve completare un modulo di richiesta di trasferimento dal centro per i partner per richiedere il trasferimento di una sottoscrizione:

1.  Dal menu centro per i partner selezionare **Customers**, quindi selezionare il cliente per il quale si desidera completare un modulo di richiesta di trasferimento.
2.  Dal menu cliente selezionare **sottoscrizioni**.
3.  Selezionare la sezione **richiesta di trasferimento** .
4.  Nella **sezione richiesta di trasferimento**selezionare **Aggiungi nuova richiesta**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sezione trasferimenti":::

5.  Completare il modulo **nuova richiesta di trasferimento** .

6.  Selezionare **Invia richiesta di trasferimento**  >  **invio**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Sezione trasferimenti":::

7.  Verificare la conferma della richiesta di trasferimento

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Sezione trasferimenti" o "completo", gli annullamenti non saranno possibili.

## <a name="current-partner-tasks-to-be-completed"></a>Attività correnti del partner da completare

L'agente di amministrazione del partner corrente riceverà un messaggio di posta elettronica che indica che il cliente richiede il trasferimento delle sottoscrizioni:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Sezione trasferimenti":::

Esaminare e accettare il modulo di richiesta di trasferimento dal centro per i partner per completare il trasferimento della sottoscrizione.

>[!Note]  
>Se non viene eseguita alcuna azione da parte del partner corrente entro 30 giorni, la richiesta scadrà e il partner futuro avrà un per creare una nuova richiesta di trasferimento.

1.  Selezionare **Verifica trasferimento richiesta** dal messaggio di posta elettronica o
1.  Dal menu centro partner selezionare **Customers**, quindi selezionare il cliente a cui è stata inviata una richiesta di trasferimento per conto di.
2.  Dal menu cliente selezionare **sottoscrizioni**.
3.  Selezionare la sezione **richiesta di trasferimento** .
4.  Espandi le informazioni sul trasferimento selezionando l' **ID richiesta di trasferimento** selezionato in **richieste ricevute**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Sezione trasferimenti":::

5.  Esaminare la richiesta di trasferimento. Selezionare le sottoscrizioni di Azure richieste da trasferire.

>[!Note]  
> Prima di procedere, tenere presente che non sarà più possibile accedere alle sottoscrizioni selezionate.
> Non verrà fatturato alcun ulteriore utilizzo.
> Le prenotazioni di Azure non vengono trasferite con le sottoscrizioni.

6.  Selezionare quindi **Accept e transfer** per completare il processo di trasferimento.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sezione trasferimenti":::

7.  Visualizza conferma accettazione trasferimento.

   A questo punto, il partner futuro, il cliente e il partner corrente riceveranno una notifica della richiesta di trasferimento accettata tramite posta elettronica.

   Dopo che la transizione è stata accettata, lo stato del trasferimento potrebbe rimanere in sospeso per un massimo di 15 minuti durante l'aggiornamento del sistema. Se richiede più tempo, il sistema continuerà a provare per tre giorni. Se lo stato del trasferimento rimane ancora in sospeso, il partner deve inviare una richiesta di servizio.

   Al termine del trasferimento, le sottoscrizioni incluse nella richiesta verranno visualizzate nel piano Azure del partner futuro e non verranno più elencate.

>[!Note]  
>Per i provider indiretti, indicare al rivenditore indiretto che la richiesta di trasferimento è stata accettata.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gestione delle sottoscrizioni dei clienti trasferiti
- La transizione non influisce sull'accesso per utenti, gruppi o entità servizio esistenti assegnati con il controllo degli accessi in base al ruolo di Azure. Il controllo degli accessi in base al ruolo di Azure [(RBAC di Azure)](/azure/role-based-access-control/overview) consente ai clienti di gestire gli utenti che hanno accesso alle risorse di Azure, le operazioni che possono eseguire con tali risorse e le aree a cui hanno accesso. Con il nuovo partner, dopo il trasferimento della sottoscrizione non viene fornito alcun accesso RBAC alle risorse del cliente. Il partner precedente del cliente mantiene il controllo degli accessi in base al ruolo. Collaborare con il cliente per comprendere chi ha informazioni dettagliate sulle sottoscrizioni e come apportare le modifiche desiderate.

- Di conseguenza, è importante che il cliente elimini l'accesso RBAC di Azure per il partner precedente e aggiunga l'accesso per il nuovo partner. Per altre informazioni sul cliente che fornisce un nuovo accesso, vedere [che cos'è il controllo degli accessi in base al ruolo di Azure (RBAC di Azure)?](/azure/role-based-access-control/overview) Per ulteriori informazioni sul cliente che rimuove l'accesso RBAC del partner precedente, vedere [rimuovere un'assegnazione di ruolo](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Inoltre, non è possibile ottenere automaticamente l'accesso [dell'amministratore per conto di (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) alle sottoscrizioni. AOBO è necessario per i partner per gestire le sottoscrizioni di Azure del cliente per loro conto. Per altre informazioni sui privilegi di Azure, vedere [ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Passaggi successivi:

- [(RBAC di Azure)](/azure/role-based-access-control/overview)
- [Ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)