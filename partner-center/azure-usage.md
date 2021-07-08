---
title: Dimensionamento delle VM di Azure per l'utilizzo massimo delle prenotazioni
description: Informazioni su come ridimensionare una macchina virtuale (VM) in base alle esigenze di calcolo dei clienti quando si acquistano Microsoft Azure prenotazioni per loro.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510194"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ridimensionamento della macchina virtuale di Microsoft Azure per l'utilizzo massimo delle prenotazioni

**Ruoli appropriati:** amministrazione dell'agente | Agente di vendita

Questo articolo illustra come ridimensionare una macchina virtuale (VM) in base alle esigenze di calcolo dei clienti quando si acquistano Microsoft Azure prenotazioni.
 
> [!NOTE]
> Questo articolo si applica solo ai partner del programma Cloud Solution Provider (CSP). I clienti che usano altri tipi di sottoscrizioni (ad esempio, sottoscrizioni con pagamento in base al go, singole, Contratto del cliente Microsoft o Enterprise Agreement) devono invece leggere la documentazione sulle prenotazioni di [Azure](/azure/cost-management-billing/reservations).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente

Quando si Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) dimensionata per soddisfare le esigenze di calcolo del cliente. È possibile trovare queste informazioni usando uno dei metodi seguenti:

- API di utilizzo di Azure
- Portale di Azure
- Azure PowerShell
- The Azure Resource Manager (ARM) API

Le istruzioni per l'uso di ognuno di questi metodi sono riportate di seguito. Dopo aver acquistato una prenotazione, lo sconto per la prenotazione viene applicato automaticamente alle macchine virtuali corrispondenti agli attributi e alla quantità della prenotazione. Non è necessario assegnare la prenotazione a una macchina virtuale.

>[!NOTE]
>Gli sconti per la prenotazione non si applicano alle macchine virtuali classiche o promozionali.

>[!IMPORTANT]
>Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, è necessario usare uno dei metodi descritti di seguito perché il tipo di serie di macchine virtuali non viene visualizzato correttamente nei file Partner Center di riconciliazione.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali usando l'API di utilizzo di Azure

1. Usare il valore per l'attributo ServiceType di additionalInfo nella risposta api per identificare le dimensioni della macchina virtuale da acquistare.

2. Per altre informazioni, vedere Ottenere i record di utilizzo di un cliente [per Azure nell'API](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [Partner Center.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali usando il portale Microsoft Azure macchina virtuale

1. In Partner Center passare alla **pagina** Clienti.

2. Trovare il cliente che vuole acquistare prenotazioni di macchine virtuali di Azure e quindi selezionare la freccia giù per espandere le informazioni del cliente. Selezionare **Microsoft Azure portale di gestione** per aprire il record del cliente nel portale di Azure.

3. Selezionare **Macchine virtuali** dal menu del portale e quindi selezionare la macchina virtuale per cui si vuole acquistare una prenotazione.

4. Nella pagina dei dettagli della macchina virtuale trovare le informazioni sulle dimensioni e sull'area, come illustrato di seguito, e usare queste informazioni per acquistare la prenotazione in Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Informazioni su dimensioni e area nella pagina dei dettagli.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali usando Microsoft Azure PowerShell

Usare le informazioni nell'immagine seguente per ottenere la posizione e le dimensioni della macchina virtuale per cui si vuole acquistare una prenotazione. 

:::image type="content" source="images/usage2.png" alt-text="Posizione e dimensioni della macchina virtuale.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali usando l'API Azure Resource Manager (ARM)

1. Usando ARMClient o le API arm, chiamare il client ARM per la macchina virtuale per cui si vuole acquistare una prenotazione.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. La chiamata restituisce i valori per **vmSize** **e location**, come illustrato di seguito.

    :::image type="content" source="images/usage3.png" alt-text="Valore vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valore location.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificare l'utilizzo delle macchine virtuali di Azure e lo sconto per la prenotazione

Dopo aver acquistato un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento anticipato dello spazio della macchina virtuale viene applicato automaticamente alle macchine virtuali che corrispondono agli attributi e alla quantità della prenotazione del cliente.

È possibile verificare l'utilizzo della prenotazione del cliente e vedere a quali macchine virtuali vengono applicati gli sconti per la prenotazione usando uno dei metodi seguenti:

- Portale di Azure
- API di utilizzo di Azure

Le istruzioni per l'uso di ognuno di questi metodi sono riportate di seguito.

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra la macchina virtuale a cui viene applicato lo sconto.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verificare l'utilizzo della prenotazione del cliente nel portale Microsoft Azure

1. In Partner Center passare alla **pagina** Clienti.

2. Trovare il cliente di cui si desidera verificare lo sconto e l'utilizzo della prenotazione e quindi selezionare la freccia giù per espandere le informazioni del cliente. Selezionare **Microsoft Azure portale di gestione** per aprire il record del cliente nel portale di Azure.
3. Selezionare **Prenotazioni dal** menu del portale e quindi selezionare la prenotazione per cui si vuole verificare l'utilizzo.
4. Nella pagina **Panoramica** controllare il grafico di utilizzo della prenotazione, che mostra la quantità di prenotazione applicata alle macchine virtuali.

    >[!NOTE]
    >I dati di utilizzo possono essere posticipati fino a 8 ore.

    a. Se l'utilizzo della prenotazione è del 100%, il cliente sta ottenendo tutti i risparmi possibili che l'acquisto della prenotazione può offrire.
    b. Se l'utilizzo della prenotazione è 0%, lo sconto non viene applicato ad alcuna macchina virtuale.
    c. Se l'utilizzo della prenotazione è compreso tra l'1% e il 99%, si verificano vantaggi inutilizzati.

5. Per evitare questa situazione, determinare le dimensioni corrette della macchina virtuale per supportare le esigenze di calcolo del cliente prima di effettuare l'acquisto.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra la macchina virtuale a cui viene applicato lo sconto.  

È possibile ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente otterrà lo sconto per la prenotazione e per vedere a quali macchine virtuali (macchine virtuali) viene applicato lo sconto. Confrontare l'esempio A con l'esempio B per verificare l'utilizzo della prenotazione di un cliente.

:::image type="content" source="images/usage5.png" alt-text="Esempi di utilizzo della prenotazione.":::

- ReservationId identifica la prenotazione di Azure usata per applicare lo sconto alla macchina virtuale.
- consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto per la prenotazione.
- ReservationMeter mostra il costo di $ 0 dopo l'applicazione dello sconto per la prenotazione.

Per altre informazioni, vedere Ottenere i record di utilizzo di un cliente [per Azure nell'API](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) [Partner Center.](/partner-center/develop/)

>[!IMPORTANT]
>I costi software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di vm e verranno visualizzati come voci separate nel record dell'ordine e nella fattura. Tuttavia, se un cliente ha il vantaggio Azure Hybrid Use, i costi del software non verranno applicati. Per altre informazioni, vedere Windows [software non inclusi nelle istanze riservate.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Passaggi successivi

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure di macchine virtuali riservate](azure-reservations.md)
|Acquisto di prenotazioni di Azure per i clienti in Partner Center   | [Acquistare prenotazioni di Azure](azure-reservations-buying.md)
|Gestione delle prenotazioni di Azure in Partner Center | [Gestione delle prenotazioni di Azure in Partner Center](azure-reservations-manage.md)
|Acquisto di prenotazioni di Azure nel portale di Azure | [Pagamento preliminare per le macchine virtuali con istanze di macchine](/azure/virtual-machines/windows/prepay-reserved-vm-instances) virtuali riservate di Azure nella Guida di Azure |
|Gestione delle prenotazioni di Azure nell'portale di Azure   | [Gestire le istanze di macchine virtuali riservate](/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure  |
|Acquisto di prenotazioni di Azure tramite l'API Partner Center azure | [Acquistare istanze di macchine virtuali riservate di Azure](/partner-center/develop/purchase-azure-reservations) nella documentazione Partner Center per sviluppatori   |
|Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata per loro. | [Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure](give-customers-permission.md)   |