---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. Nell'ambito del nuovo prodotto, Microsoft ha introdotto nuovi piani di sottoscrizione per Microsoft Dynamics per i clienti dal 1 novembre 2016, simili ma non identici ai piani correnti.

Le istruzioni in questo documento descrivono in che modo i provider indiretti possono eseguire il passaggio delle sottoscrizioni esistenti di Microsoft Dynamics AX e Microsoft Dymanics CRM Online dei clienti ai nuovi piani per Microsoft Dynamics 365. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

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


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Annullare la sottoscrizione precedente](#manual-subscription-migration-cancelsubscriptions).

Le procedure seguenti illustrano come trasferire un cliente da Microsoft Dynamics AX o CRM Online a Dynamics 365.

In questo esempio, il rivenditore deve trasferire un cliente con una sottoscrizione esistente per Dynamics AX Enterprise a Dynamics 365 for Operations. Il primo passaggio consiste nell'acquistare Dynamics 365 for Operations.  Ripeti questa procedura per il passaggio di un cliente da CRM Online a Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Acquista la nuova sottoscrizione**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



