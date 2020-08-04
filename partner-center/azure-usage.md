---
title: Dimensionamento delle VM di Azure per l'utilizzo massimo delle prenotazioni
ms.topic: how-to
ms.date: 07/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come ridimensionare una macchina virtuale (VM) in base alle esigenze di elaborazione dei clienti quando si acquistano Microsoft Azure prenotazioni.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 48f7fb317d35c87eaf3d8fddc7a5da907178ef36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527447"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ridimensionamento della macchina virtuale di Microsoft Azure per l'utilizzo massimo delle prenotazioni

**Si applica a**

- Centro per i partner
- Portale di Azure
- Partner in CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente

Quando si acquistano Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) ridimensionata per soddisfare le esigenze di calcolo del cliente. È possibile trovare queste informazioni usando uno dei metodi seguenti:

- API di utilizzo di Azure
- Portale di Azure
- Azure PowerShell
- API Azure Resource Manager (ARM)

Di seguito sono riportate le istruzioni per l'uso di ognuno di questi metodi. Dopo l'acquisto di una prenotazione, lo sconto relativo alla prenotazione viene applicato automaticamente alle macchine virtuali corrispondenti agli attributi e alla quantità della prenotazione. Non è necessario assegnare la prenotazione a una macchina virtuale.

>[!NOTE]
>Gli sconti per le prenotazioni non si applicano alle VM classiche o promozionali.

>[!IMPORTANT]
>Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, è necessario usare uno dei metodi descritti di seguito poiché il tipo di serie di VM non viene visualizzato correttamente nei file di riconciliazione del centro per i partner.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API di utilizzo di Azure

1. Usare il valore per l'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare.

2. Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Ottenere informazioni sul dimensionamento della macchina virtuale usando il portale di Microsoft Azure

1. Nel centro per i partner passare alla pagina **Customers (clienti** ).

2. Trovare il cliente che desidera acquistare le prenotazioni di macchine virtuali di Azure e quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente. Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.

3. Selezionare **macchine virtuali** dal menu del portale e quindi selezionare la macchina virtuale per cui si vuole acquistare una prenotazione.

4. Nella pagina dei dettagli della macchina virtuale individuare le informazioni sulle dimensioni e sull'area, come illustrato di seguito, e usare queste informazioni per acquistare la prenotazione nel centro per i partner.  

   :::image type="content" source="images/usage1.png" alt-text="Informazioni sulle dimensioni e sull'area nella pagina Dettagli":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Ottenere informazioni sul dimensionamento della macchina virtuale usando Microsoft Azure PowerShell

Usare le informazioni nell'immagine seguente per ottenere la posizione e le dimensioni della macchina virtuale per cui si vuole acquistare una prenotazione. 

:::image type="content" source="images/usage2.png" alt-text="Posizione e dimensioni della macchina virtuale":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API Azure Resource Manager (ARM)

1. Usando le API ARMClient o ARM, chiamare il client ARM per la macchina virtuale per cui si vuole acquistare una prenotazione.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. La chiamata restituisce i valori per **vmSize** e **location**, come illustrato di seguito.

    :::image type="content" source="images/usage3.png" alt-text="valore vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valore Location":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificare l'utilizzo della macchina virtuale di Azure e lo sconto per

Dopo aver acquistato un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento dello spazio della VM in anticipo viene applicato automaticamente alle macchine virtuali che corrispondono agli attributi e alla quantità della prenotazione del cliente.

È possibile verificare l'utilizzo della prenotazione del cliente e vedere a quali macchine virtuali vengono applicati gli sconti per la prenotazione utilizzando uno dei metodi seguenti:

- Portale di Azure
- API di utilizzo di Azure

Di seguito sono riportate le istruzioni per l'uso di ognuno di questi metodi.

>[!NOTE]
>Solo l'API di utilizzo di Azure indica a quale macchina virtuale viene applicato lo sconto.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure

1. Nel centro per i partner passare alla pagina **Customers (clienti** ).

2. Individuare il cliente per cui si desidera verificare lo sconto e l'utilizzo della prenotazione, quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente. Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.
3. Selezionare **prenotazioni** dal menu del portale e quindi selezionare la prenotazione per cui si vuole controllare l'utilizzo.
4. Nella pagina **Panoramica** controllare il grafico di utilizzo della prenotazione, che mostra la quantità di prenotazione applicata alle macchine virtuali.

    >[!NOTE]
    >I dati di utilizzo possono essere posticipati di un massimo di 8 ore.

    a. Se l'utilizzo della prenotazione è pari al 100%, il cliente è in grado di ottenere tutti i risparmi possibili che possono essere forniti dall'acquisto della prenotazione.
    b. Se l'utilizzo della prenotazione è 0%, lo sconto non viene applicato a nessuna macchina virtuale.
    c. Se l'utilizzo della prenotazione è compreso tra 1% e 99%, i vantaggi non vengono usati.

5. Per evitare questa situazione, determinare la VM di dimensioni corrette per supportare le esigenze di calcolo del cliente prima di effettuare l'acquisto.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure

>[!NOTE]
>Solo l'API di utilizzo di Azure indica a quale macchina virtuale viene applicato lo sconto.  

È possibile ottenere i dati di utilizzo delle prenotazioni con l'API di utilizzo di Azure per verificare che il cliente ottenga lo sconto per la prenotazione e per vedere a quali macchine virtuali (macchine virtuali) viene applicato lo sconto. Confrontare l'esempio a all'esempio B per vedere come verificare l'utilizzo della prenotazione di un cliente.

:::image type="content" source="images/usage5.png" alt-text="Esempi di utilizzo della prenotazione":::

- ReservationId identifica la prenotazione di Azure usata per applicare lo sconto alla macchina virtuale.
- consumptionMeter è il ID contatore per la macchina virtuale a cui è applicato lo sconto di prenotazione.
- Il ReservationMeter Mostra il costo $0 poiché è stato applicato lo sconto di prenotazione.

Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

>[!IMPORTANT]
>I costi del software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione della macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura. Tuttavia, se un cliente ha il vantaggio Azure Hybrid use, i costi del software non verranno applicati. Per ulteriori informazioni, vedere [costi del software Windows non inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Risorse per le prenotazioni di Azure

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica sulle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze di VM riservate](azure-reservations.md)
|Acquisto di prenotazioni di Azure per i clienti nel centro per i partner   | [Acquista prenotazioni di Azure](azure-reservations-buying.md)
|Gestione delle prenotazioni di Azure nel centro per i partner | [Gestione delle prenotazioni di Azure nel centro per i partner](azure-reservations-manage.md)
|Acquisto di prenotazioni di Azure nell'portale di Azure | [Pagamento anticipato per le macchine virtuali con le istanze di VM riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure |
|Gestione delle prenotazioni di Azure nell'portale di Azure   | [Gestire le istanze di VM riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure  |
|Acquisto di prenotazioni di Azure tramite l'API del centro per i partner | [Acquistare istanze di VM riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per gli sviluppatori del centro per i partner   |
|Concedere ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure da una sottoscrizione acquistata. | [Concedi ai clienti l'autorizzazione per acquistare le proprie prenotazioni di Azure](give-customers-permission.md)   |
