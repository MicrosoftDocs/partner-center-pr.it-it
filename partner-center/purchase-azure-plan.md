---
title: Acquistare il piano di Azure
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come acquistare una o più sottoscrizioni e prenotazioni di Azure, configurare le risorse e visualizzare o aggiungere sottoscrizioni usando il piano di Azure.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 004044902b21c223af75414a1ec999173b481058
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854962"
---
# <a name="purchase-the-azure-plan-for-customers--access-the-latest-azure-services-at-pay-as-you-go-rates"></a>Acquistare il piano di Azure per i clienti e accedere ai servizi di Azure più recenti con pagamento in base al consumo

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente di vendita

Quando acquisti un piano di Azure per i clienti in base al contratto del cliente Microsoft, puoi accedere al catalogo completo dei servizi di Azure più recenti a tariffe con pagamento in base al consumo. I partner CSP potranno ora accedere a qualsiasi servizio di Azure quando diventa disponibile a livello generale. In un piano di Azure un partner può avere più sottoscrizioni di Azure. 

## <a name="countryregion-availability"></a>Disponibilità per Paese/area geografica

Si prevede che la nuova esperienza commerciale in CSP per Azure sia disponibile in 139 paesi. Consulta l'elenco completo di questi [Paesi/aree geografiche](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x). 

## <a name="how-to-purchase-azure-plan"></a>Come acquistare il piano di Azure

La modalità di acquisto del piano di Azure è simile all'acquisto di qualsiasi altra sottoscrizione. La differenza principale consiste nel fatto che, prima di inviare effettivamente l'ordine, devi verificare che il cliente abbia firmato il contratto del cliente Microsoft.

1. Seleziona **Segmento: Commerciale** e digita **Microsoft Azure**. 
2. In Piano di Azure seleziona **Aggiungi al carrello**.

:::image type="content" source="images/azure/Azurepurchase1.png" alt-text="Acquisto":::

Il partner deve verificare che il cliente abbia esaminato e accettato le condizioni del contratto del cliente Microsoft. Per altre informazioni su come eseguire questa operazione, leggi [Verificare l'accettazione da parte del cliente del contratto del cliente Microsoft](confirm-customer-agreement.md). Altre risorse sono disponibili nella [raccolta delle risorse](https://partner.microsoft.com/resources/collection/Microsoft-Customer-Agreement-in-the-CSP-program#/).

**Per confermare**: 

1. Conferma digitalmente oppure

2. Invita il cliente a firmare il contratto del cliente Microsoft direttamente con Microsoft. 

### <a name="to-confirm"></a>Per verificare 

1. Nella pagina **Account** del cliente seleziona **Aggiorna** accanto a **Contratto del cliente Microsoft**.  

2. Compila le informazioni relative alla persona presso la società del cliente che ha accettato il contratto del cliente Microsoft.

3. Seleziona **Salva e continua**.  

## <a name="review-and-buy"></a>Verificare e acquistare

Torna alla pagina **Aggiungi prodotto**  in cui puoi vedere che è stato aggiunto il piano di Azure. Seleziona **Verifica** per verificare l'acquisto e quindi seleziona **Acquista**. 

>[!Note]
>Dopo aver acquistato il piano di Azure per un cliente, non potrai più acquistare Microsoft Azure (0145p) per lo stesso cliente. Dovrai creare future sottoscrizioni tramite il piano di Azure.

## <a name="purchase-azure-reservations-under-the-azure-plan"></a>Acquistare prenotazioni di Azure in base al piano di Azure 
  
Nel Centro per i partner puoi anche acquistare prenotazioni di Microsoft Azure in base al piano di Azure per conto dei tuoi clienti. In alternativa, se preferisci, puoi [concedere ai clienti l'autorizzazione ad acquistare le proprie prenotazioni di Azure](give-customers-permission.md) da una sottoscrizione precedentemente acquistata per loro.

1. Dal menu del Centro per i partner nel tuo [dashboard](https://partner.microsoft.com/dashboard/) seleziona **Clienti**. Trova il cliente che vuole acquistare prenotazioni di Azure e quindi seleziona la freccia a discesa per espandere la riga del cliente.

2. Seleziona **Aggiungi prodotti** e quindi **Azure**. 

   - Scegli il segmento di mercato del cliente dall'elenco **Segmento**.
   - Scegli **Prenotazioni** dall'elenco **Tipo di prodotto**.
   - Scegli il tipo di prenotazione desiderata dal cliente dall'elenco **Tipo di prenotazione**.

Le prenotazioni di Azure devono essere associate a un piano di Azure attivo. Scegli il piano di Azure a cui vuoi aggiungere le prenotazioni di Azure dall'elenco di sottoscrizioni del cliente. 

>[!Important] 
>Se il cliente non ha ancora un piano di Azure attivo, seleziona Azure per aggiungerne uno ora. Per altre istruzioni, leggi [Acquista prenotazioni di Azure](azure-reservations-buying.md#purchase-azure-reservations).

>[!Note]
>Attualmente, nel Centro per i partner l'ambito di una prenotazione può essere impostato solo su **Condiviso**. Per selezionare l'ambito di sottoscrizione singola o l'aggiornamento dall'ambito condiviso a quello di sottoscrizione **singola, passare Microsoft Azure portale** di gestione seguendo le istruzioni seguenti. 

:::image type="content" source="images/azure/addprods1.png" alt-text="Impostazione ambito condiviso delle prenotazioni":::

Per gestire la prenotazione del cliente nel portale di Azure: 

1. In **Clienti** seleziona il cliente che vuoi gestire. 

2. Con la freccia rivolta verso il basso, espandi la riga del cliente e seleziona **Portale di gestione di Microsoft Azure**.  
 
## <a name="view-azure-subscriptions-under-the-azure-plan"></a>Visualizzare le sottoscrizioni di Azure nel piano di Azure

Nella sezione Basato sull'utilizzo della pagina **Sottoscrizioni** espandi **Piano di Azure** per visualizzare le sottoscrizioni di Azure associate nel piano di Azure.

:::image type="content" source="images/azure/addprods2.png" alt-text="Visualizzazione dell'elenco delle sottoscrizioni di Azure"::: 


## <a name="add-subscriptions-and-configure-resources"></a>Aggiungere sottoscrizioni e configurare risorse

Nel portale di Azure potrai aggiungere sottoscrizioni e configurare risorse per il cliente. Potrai anche separare l'ambiente del cliente in base al carico di lavoro o al progetto. È possibile gestire le sottoscrizioni tramite [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) e tramite il portale di Azure. 

Per gestire le risorse e le sottoscrizioni del cliente, devi avere i privilegi di **Amministratore per conto terzi** (AOBO, Admin on Behalf Of). Per informazioni sulla gestione dell'accesso, leggi [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md).

## <a name="next-steps"></a>Passaggi successivi

- [Transizioni dei clienti al piano di Azure](azure-plan-transition.md)

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)
