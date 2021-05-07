---
title: Trasferire una sottoscrizione di Azure in un piano di Azure a un altro partner CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come modificare il Cloud Solution Provider partner del programma associato alle sottoscrizioni di Azure di un cliente in un piano di Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702723"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Trasferire le sottoscrizioni del piano di Azure di un cliente a un partner diverso

**Ruoli appropriati**

- Amministratore degli account
- Agente di vendita
- Agente di fatturazione

Questo articolo descrive come un cliente può cambiare le sottoscrizioni di Azure in un piano di Azure da un Cloud Solution Provider (CSP) a un altro.

Per cambiare le sottoscrizioni di Azure di un cliente da un partner diverso, seguire questa procedura. Sia il partner che il cliente devono completare i passaggi.

>[!Note]  
>Solo i partner con una relazione di fatturazione diretta con Microsoft possono accedere agli strumenti di transizione. I rivenditori indiretti devono collaborare con i propri provider indiretti per sfruttare questo strumento di transizione.

Il cliente deve essere in conversazione con entrambi i partner (attuale e futuro) prima di sfruttare questo strumento. È necessario che sia stata una conversazione offline per evitare confusione e varianza. Inoltre, i partner e i clienti devono comprendere queste considerazioni e prerequisiti prima di avviare una transizione:

**Considerazioni principali:**

- Le prenotazioni di Azure non verranno spostate con la sottoscrizione a un partner futuro
- La transizione dei prezzi CSP per i servizi di Azure con il partner corrente non verrà  
- Le responsabilità di supporto per il cliente verranno spostate nel partner futuro
- La fatturazione e la fatturazione verranno spostate nel partner futuro al momento del trasferimento
- Il trasferimento Role-Based controllo degli accessi in base al ruolo di Azure non è influenzato dal trasferimento
- L'amministratore per conto di (AOBO) non verrà concesso per impostazione predefinita al partner futuro
- I prodotti del marketplace di terze parti verranno trasferiti fino a quando i prodotti superano il controllo di idoneità al Marketplace.
    - Non sono presenti sconti speciali o restrizioni a livello di regione
    - I prodotti non sono basati su sottoscrizioni
    - Il partner futuro deve collaborare con l'editore per assicurarsi che siano presenti nell'elenco di elementi consentiti per la distribuzione del prodotto
    - Se non tutte queste condizioni vengono soddisfatte per trasferire i prodotti del Marketplace, è necessario annullare le sottoscrizioni di Azure e quindi riacquisire i prodotti del Marketplace con il nuovo partner

**Prerequisiti:**

- Il cliente interagisce con il partner CSP corrente per la transizione
- Il futuro partner CSP collabora con il cliente per garantire che le esigenze dei clienti possano essere soddisfatte
- Il futuro partner CSP stabilisce una relazione con il cliente e acquista un piano di Azure prima dell'inizio della transizione  
- Il cliente deve firmare Contratto del cliente Microsoft partner CSP futuro
- Il partner CSP futuro deve aver firmato il Contratto Microsoft Partner per usare questo strumento

## <a name="customer-tasks-to-be-completed"></a>Attività del cliente da completare

Per trasferire una sottoscrizione di Azure in un piano di Azure, il cliente deve avviare il processo contattando il partner corrente. Devono raccogliere il nome e il dominio della società del partner corrente in modo che il partner futuro possa completare il modulo di richiesta di trasferimento per loro conto.

Il cliente deve anche identificare le sottoscrizioni da trasferire dal partner corrente. Non è possibile modificare i partner per le sottoscrizioni di Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

>[!Note]  
>È responsabilità del partner futuro completare il modulo di richiesta di trasferimento che avvia il processo di trasferimento. Microsoft non può intervenire per conto del cliente o del partner corrente. Il cliente deve pianificare di collaborare a stretto contatto con il partner futuro e attuale per rendere la transizione senza problemi.

## <a name="future-partner-tasks-to-be-completed"></a>Attività future dei partner da completare

Il partner futuro della sottoscrizione deve completare un modulo di richiesta di trasferimento Partner Center per richiedere un trasferimento di sottoscrizione:

1.  Dal menu Partner Center selezionare **Clienti,** quindi selezionare il cliente per cui si vuole completare un modulo di richiesta di trasferimento per conto di .
2.  Scegliere Sottoscrizioni dal menu **Cliente**.
3.  Selezionare la **sezione Richiesta di** trasferimento.
4.  Nella sezione **Richiesta di trasferimento** selezionare Aggiungi nuova **richiesta**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sezione Trasferimenti":::

5.  Completare il **modulo Nuova richiesta di** trasferimento.

6.  Selezionare **Invia richiesta di trasferimento**  >  **Invia**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Modulo di richiesta di trasferimento completo":::

7.  Esaminare la conferma della richiesta di trasferimento

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Esaminare il trasferimento in sospeso":::

    >[!Note]
    >Il partner futuro può annullare  la richiesta di trasferimento selezionando Annulla richiesta nell'angolo superiore destro solo quando lo stato della richiesta di trasferimento è "in sospeso". Quando lo stato della richiesta di trasferimento è "in corso" o "completato", gli annullamenti non saranno possibili.

## <a name="current-partner-tasks-to-be-completed"></a>Attività partner correnti da completare

L'agente amministratore del partner corrente del cliente riceverà un messaggio di posta elettronica in cui il cliente richiede un trasferimento delle sottoscrizioni:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisione":::

Esaminare e accettare il modulo di richiesta di trasferimento Partner Center completare il trasferimento della sottoscrizione.

>[!Note]  
>Se il partner corrente non ha intrapreso alcuna azione entro 30 giorni, la richiesta scadrà e il partner futuro avrà un oggetto per creare una nuova richiesta di trasferimento.

1.  Selezionare **Rivedi richiesta di trasferimento** dal messaggio di posta elettronica OR
1.  Dal menu Partner Center clienti selezionare **Clienti** e quindi selezionare il cliente per cui è stata inviata una richiesta di trasferimento per conto di .
2.  Scegliere Sottoscrizioni dal menu **Cliente**.
3.  Selezionare la **sezione Richiesta di** trasferimento.
4.  Espandere le informazioni di trasferimento selezionando **l'ID richiesta di trasferimento selezionato** in Richieste **ricevute**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Richiesta di trasferimento delle verifiche di origine":::

5.  Esaminare la richiesta di trasferimento. Selezionare le sottoscrizioni di Azure richieste da trasferire.

>[!Note]  
> Prima di procedere, tenere presente che non si avrà più accesso alle sottoscrizioni selezionate.
> Non verrà fatturata l'ulteriore utilizzo.
> Le prenotazioni di Azure non vengono trasferite con le sottoscrizioni.

6.  Selezionare quindi **Accetta e trasferisci** per completare il processo di trasferimento.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selezionare le sottoscrizioni da trasferire nei piani di Azure":::

7.  Visualizzare la conferma di accettazione del trasferimento.

   A questo punto, il partner futuro, il cliente e il partner corrente riceveranno una notifica della richiesta di trasferimento accettata tramite posta elettronica.

   Dopo, la transizione è stata accettata, lo stato del trasferimento potrebbe rimanere In sospeso per un massimo di 15 minuti durante l'aggiornamento del sistema. Se l'operazione richiede più tempo, il sistema continuerà a provare per tre giorni. Se lo stato del trasferimento rimane Ancora In sospeso, il partner deve inviare una richiesta di servizio.

   Al termine del trasferimento, le sottoscrizioni incluse nella richiesta verranno visualizzate nel piano di Azure del partner futuro e non verranno più elencate con l'utente.

>[!Note]  
>Per i provider indiretti: informare il rivenditore indiretto che la richiesta di trasferimento è stata accettata.

### <a name="managing-your-transferred-customer-subscriptions"></a>Gestione delle sottoscrizioni dei clienti trasferite

- La transizione non influisce sull'accesso per utenti, gruppi o entità servizio esistenti assegnati con il controllo degli accessi in base al ruolo di Azure. Il controllo degli accessi in base al ruolo di [Azure](/azure/role-based-access-control/overview) consente al cliente di gestire chi può accedere alle risorse di Azure, cosa può fare con tali risorse e a quali aree può accedere. Come nuovo partner non si ha accesso al controllo degli accessi in base al ruolo alle risorse del cliente dopo il trasferimento della sottoscrizione. Il partner precedente del cliente mantiene l'accesso RBAC. Collaborare con il cliente per comprendere chi ha informazioni dettagliate sulle sottoscrizioni e come apportare le modifiche desiderate.

- Di conseguenza, è importante che il cliente rimova l'accesso al controllo degli accessi in base al ruolo di Azure per il partner precedente e aggiunge l'accesso per il nuovo partner. Per altre informazioni sul cliente che dà nuovo accesso, vedere Che cos'è il controllo degli accessi in base al [ruolo di Azure?](/azure/role-based-access-control/overview) Per altre informazioni sulla rimozione dell'accesso RBAC del partner precedente da parte del cliente, vedere [Rimuovere un'assegnazione di ruolo.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Inoltre, non si ottiene automaticamente l'accesso [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) alle sottoscrizioni. AOBO è necessario per i partner per gestire le sottoscrizioni di Azure del cliente per loro conto. Per altre informazioni sui privilegi di Azure, vedere Ottenere le autorizzazioni per gestire il servizio [o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Passaggi successivi:

- [(Controllo degli accessi in base al ruolo di Azure)](/azure/role-based-access-control/overview)
- [Ottenere le autorizzazioni per gestire il servizio o la sottoscrizione di un cliente.](./customers-revoke-admin-privileges.md)
