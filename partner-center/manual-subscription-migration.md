---
title: Migrazione delle sottoscrizioni Dynamics AX a Dynamics 365 | Centro
description: "Microsoft introduce Dynamics 365, la nuova generazione di applicazioni aziendali intelligenti che consentono l'espansione, evoluzione e trasformazione della tua organizzazione per soddisfare le esigenze dei clienti esistenti e acquisire nuove opportunità."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrazione delle sottoscrizioni Dynamics AX a Dynamics 365

**Si applica a**

-  Centro per i partner

Microsoft introduce Dynamics 365, la nuova generazione di applicazioni aziendali intelligenti che consentono l'espansione, evoluzione e trasformazione della tua organizzazione per soddisfare le esigenze dei clienti esistenti e acquisire nuove opportunità. Nell'ambito del nuovo prodotto, Microsoft ha introdotto nuovi piani di sottoscrizione per Microsoft Dynamics per i clienti dal 1 novembre 2016, simili ma non identici ai piani correnti.

Le istruzioni in questo documento descrivono in che modo i provider indiretti possono eseguire il passaggio delle sottoscrizioni esistenti di Microsoft Dynamics AX e Microsoft Dymanics CRM Online dei clienti ai nuovi piani per Microsoft Dynamics 365. Le istruzioni si applicano anche agli altri prodotti Microsoft aggiornati a nuove versioni, per i quali è necessario che i provider eseguano la migrazione delle sottoscrizioni dei clienti a un nuovo SKU.

I piani Microsoft Dynamics CRM Online e AX sono stati ritirati.  A partire dal 1 luglio 2017 non sarà più possibile rinnovare i piani legacy. Anche le sottoscrizioni E4 esistenti non verranno rinnovate automaticamente alla scadenza.

Le sottoscrizioni CRM Online e AX verranno annullate alla scadenza. Per garantire la continuità, è opportuno trasferire i clienti con sottoscrizioni in scadenza a una delle opzioni SKU supportate indicate di seguito. Si consiglia di far sottoscrivere ai clienti nuove sottoscrizioni prima della data di scadenza annuale della sottoscrizione, al fine di evitare eventuali interruzioni del servizio. 

Per le sottoscrizioni in scadenza, nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione è passato a "Data di scadenza [data]" da "Rinnovo automatico il [data]". 

Se usi l'API (CREST o Centro per i partner), puoi individuare le sottoscrizioni in scadenza valutando la data di scadenza della sottoscrizione insieme alla proprietà auto renew = False. Le sottoscrizioni verranno impostate su auto renew=False il 1 luglio 2017. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

**Modifiche delle licenze per Microsoft Dynamics AX**

La linea di prodotti Microsoft Dynamics AX è stata ritirata a partire dal 1 novembre 2016. Per altre informazioni sulle nuove opzioni di licenza per Dynamics 365, consulta la [Guida alle licenze](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Fai riferimento alla tabella seguente per altri dettagli sul mapping delle licenze:

|**SKU ritirato**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Piano Microsoft Dynamics 365 for Unified Operations o Microsoft Dynamics 365 |
|Attività|Microsoft Dynamics 365 for Activity
|Attività/Servizio autonomo|Microsoft Dynamics 365 for Team Members|
|Dispositivo|Dispositivo Microsoft Dynamics 365 for Operations|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Modifiche delle licenze per Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

Il piano Microsoft Dynamics CRM Online corrente è stato ritirato a partire dal 1 novembre 2016. Per altre informazioni sulle nuove opzioni di licenza per Microsoft Dynamics 365, consulta la [Guida alle licenze](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Vedi le [Informazioni importanti per i clienti CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) per ulteriori informazioni sulle nuove opzioni di licenza.

Fai riferimento alla tabella seguente per altri dettagli sul mapping delle licenze:

|**SKU ritirato**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Piano Dynamics 365 Enterprise Customer Engagement |
|Professionale|Piano Dynamics 365 Enterprise Customer Engagement, Dynamics 365 for Sales oppure Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service oppure Piano Dynamics 365 Enterprise Customer Engagement|
|Essenziale|Dynamics 365 for Team Members|
|Componente aggiuntivo Field Service|Piano Dynamics 365 Enterprise Customer Engagement oppure Dynamics 365 for Field Service|
|Componente aggiuntivo Project Service Automation|Piano Dynamics 365 Customer Engagement oppure Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti


Microsoft offre continuamente nuovi prodotti e servizi a rivenditori e provider. In questi casi, un rivenditore potrebbe avere la necessità di aggiornare i clienti ai nuovi servizi o di eseguire la migrazione delle loro sottoscrizioni da SKU destinati a essere ritirati. La migrazione dei clienti da SKU precedenti a quelli più recenti richiede la sequenza seguente:

-   [Acquistare la nuova sottoscrizione](#manual-subscription-migration-purchasenewsubsc);
-   [Riassegnare le licenze utente correnti](#manual-subscription-migration-reassignlicenses);
-   [Annullare la sottoscrizione precedente](#manual-subscription-migration-cancelsubscriptions).

Le procedure seguenti illustrano come trasferire un cliente da Microsoft Dynamics AX o CRM Online a Dynamics 365.

In questo esempio, il rivenditore deve trasferire un cliente con una sottoscrizione esistente per Dynamics AX Enterprise a Dynamics 365 for Operations. Il primo passaggio consiste nell'acquistare Dynamics 365 for Operations.  Ripeti questa procedura per il passaggio di un cliente da CRM Online a Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Acquista la nuova sottoscrizione**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi scegli **Aggiungi sottoscrizioni**.
2.  Seleziona la sottoscrizione che vuoi acquistare dal catalogo (in questo caso Dynamics 365 for Operations, Enterprise Edition), immetti il numero di licenze e scegli **Invia**.

    Il cliente a questo punto dovrebbe avere sia la sottoscrizione nuova che quella precedente, in questo esempio la vecchia sottoscrizione Dynamics AX Enterprise e la nuova sottoscrizione di destinazione, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> Il passaggio successivo consiste nel riassegnare tutte le licenze utente esistenti alla nuova sottoscrizione.

**Riassegnare le licenze utente**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi scegli **Utenti e licenze**. Viene aperta la pagina Utenti e licenze del cliente.
2.  Per riassegnare le licenze utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.
3.  Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza **Dynamics AX Enterprise** e seleziona la licenza **Dynamics 365 for Operations**.
4.  Seleziona **Invia**. Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma.
5.  Ripeti la stessa procedura per tutti gli utenti del cliente per cui è necessaria la riassegnazione della licenza.

<a href="" id="cancelsubscriptions"></a> Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare la sottoscrizione precedente al livello principale del cliente.

**Annullare la sottoscrizione precedente**

1.  Nel menu **Dashboard** seleziona **Clienti**, seleziona il cliente di cui eseguire la migrazione e quindi seleziona la sottoscrizione che vuoi annullare.
2.  Nella pagina dei dettagli della sottoscrizione imposta lo **Stato** della sottoscrizione su **Sospeso**.
3.  Seleziona **Invia**.

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.

## <a name="additional-considerations"></a>Considerazioni aggiuntive


Se il cliente passa dal canale Open al programma per i servizi cloud per il provisioning di altre sottoscrizioni, dovrai eseguire anche la migrazione delle sottoscrizioni esistenti:

-   Se il cliente ha ricevuto la sottoscrizione precedente tramite il canale Open, il passaggio al programma CSP per il nuovo SKU è semplice.
-   Se il cliente non è ancora classificato come tuo cliente, puoi invitarlo. Per informazioni, vedi l'argomento della Guida [Richiedere una relazione con un cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Dopo che il cliente ti accetta come provider indiretto, la procedura per il provisioning è fondamentalmente la stessa descritta in precedenza, ovvero devi acquistare la nuova sottoscrizione e quindi assegnare le licenze utente. L'unica differenza riguarda l'annullamento delle sottoscrizioni precedenti. Un nuovo provider non può annullare/sospendere sottoscrizioni acquisite tramite altri canali. Se il cliente ha acquisito le sottoscrizioni precedenti tramite un altro canale di vendita, come il canale Open, il cliente dovrà annullare autonomamente tali sottoscrizioni tramite il canale originale.

 

 



