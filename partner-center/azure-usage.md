---
title: Ridimensionamento della macchina virtuale Microsoft Azure per l'utilizzo massimo della prenotazione | Centro per i partner
ms.topic: article
ms.date: 08/05/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Quando si acquistano Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) ridimensionata per soddisfare le esigenze di calcolo del cliente.
author: LauraBrenner
ms.author: labrenne
keywords: azure, prenotazioni, vm, gestire, utilizzo, ridimensionamento
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9d0c2935bd5a2202b50ffc470fbef144ce4d20e2
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653777"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Ridimensionamento della macchina virtuale Microsoft Azure per un utilizzo ottimale delle prenotazioni

**Si applica a**

- Centro per i partner
- Portale di Azure
- Partner di CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinare le dimensioni della macchina virtuale per la prenotazione di Azure di un cliente 

Quando si acquistano Microsoft Azure prenotazioni per conto dei clienti, è necessario scegliere una macchina virtuale (VM) ridimensionata per soddisfare le esigenze di calcolo del cliente. Puoi trovare queste informazioni scegliendo uno dei metodi seguenti:

- API di utilizzo Azure
- Portale di Azure
- Azure PowerShell
- L'API di Azure Resource Manager (ARM)

Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito. Dopo aver acquistato una prenotazione, il relativo sconto verrà applicato automaticamente alle macchine virtuali che rispondono agli attributi e alla quantità della prenotazione. Non è necessario assegnare la prenotazione a una macchina virtuale.

>[!NOTE]
>Gli sconti per le prenotazioni non si applicano alle VM classiche o promozionali.

>[!IMPORTANT]
>Per identificare correttamente il tipo e le dimensioni della macchina virtuale da acquistare per conto del cliente, dovrai utilizzare uno dei metodi descritti di seguito poiché la serie della macchina virtuale non viene visualizzata correttamente nei file di riconciliazione del Centro per i partner.

**Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API di utilizzo di Azure**

1. Utilizza il valore dell'attributo ServiceType da additionalInfo nella risposta dell'API per identificare le dimensioni della macchina virtuale da acquistare.
2. Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

**Ottenere informazioni sul dimensionamento della macchina virtuale usando il portale di Microsoft Azure**

1. Nel centro per i partner passare alla pagina **Customers (clienti** ).
2. Trovare il cliente che desidera acquistare le prenotazioni di macchine virtuali di Azure e quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente. Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.
3. Seleziona **Macchine virtuali** dal menu del portale, quindi seleziona la macchina virtuale per cui desideri acquistare una prenotazione.
4. Nella pagina dei dettagli della macchina virtuale individuare le informazioni sulle dimensioni e sull'area, come illustrato di seguito, e usare queste informazioni per acquistare la prenotazione nel centro per i partner.  

    ![Informazioni sulle dimensioni e sull'area nella pagina Dettagli](images/usage1.png)

**Ottenere informazioni sul dimensionamento della macchina virtuale usando Microsoft Azure PowerShell**

Per ottenere la posizione e le dimensioni della macchina virtuale per cui desideri acquistare una prenotazione, utilizza le informazioni nell'immagine seguente. 

![Posizione e dimensioni della macchina virtuale](images/usage2.png)

**Ottenere informazioni sul dimensionamento delle macchine virtuali tramite l'API Azure Resource Manager (ARM)**

1. Tramite le API di ARMClient o ARM, chiama il client ARM per la macchina virtuale per cui desideri acquistare una prenotazione.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. La chiamata restituisce valori per **vmSize** e **location**, come illustrato di seguito.

    ![valore vmSize](images/usage3.png) ![percorso](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Verificare lo sconto su prenotazione e utilizzo della macchina virtuale di Azure

Dopo aver acquistato un'istanza di macchina virtuale riservata di Azure per conto di un cliente, lo sconto per il pagamento dello spazio della VM in anticipo viene applicato automaticamente alle macchine virtuali che corrispondono agli attributi e alla quantità della prenotazione del cliente.

È possibile verificare l'utilizzo della prenotazione del cliente e vedere a quali macchine virtuali vengono applicati gli sconti per la prenotazione utilizzando uno dei metodi seguenti:

- Portale di Azure
- API di utilizzo Azure

Le istruzioni per l'uso di ciascuno dei seguenti metodi sono riportate di seguito.

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verificare l'utilizzo della prenotazione del cliente nel portale di Microsoft Azure

1. Nel centro per i partner passare alla pagina **Customers (clienti** ).

2. Individuare il cliente per cui si desidera verificare lo sconto e l'utilizzo della prenotazione, quindi selezionare la freccia rivolta verso il basso per espandere le informazioni del cliente. Selezionare **portale di gestione di Microsoft Azure** per aprire il record del cliente nella portale di Azure.
3. Seleziona **Prenotazioni** dal menu del portale, quindi seleziona la prenotazione di cui desideri verificare l'utilizzo.
4. Nella pagina **Panoramica** controllare il grafico di utilizzo della prenotazione, che mostra la quantità di prenotazione applicata alle macchine virtuali.

    >[!NOTE]
    >I dati di utilizzo possono essere ritardati fino a 8 ore.

    a. Se l'utilizzo della prenotazione è pari al 100%, il cliente è in grado di ottenere tutti i risparmi possibili che possono essere forniti dall'acquisto della prenotazione.
    b. Se l'utilizzo della prenotazione è 0%, lo sconto non viene applicato a nessuna macchina virtuale.
    c. Se l'utilizzo della prenotazione è compreso tra 1% e 99%, i vantaggi non vengono usati.

5. Per evitare questa situazione, determinare la VM di dimensioni corrette per supportare le esigenze di calcolo del cliente prima di effettuare l'acquisto.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verificare l'utilizzo della prenotazione del cliente con l'API di utilizzo di Azure

>[!NOTE]
>Solo l'API di utilizzo di Azure mostra a quale macchina virtuale è applicato lo sconto.  

Puoi ottenere i dati di utilizzo della prenotazione con l'API di utilizzo di Azure per verificare che il cliente riceva lo sconto prenotazione e per vedere a quali macchine virtuali è applicato lo sconto. Confrontare l'esempio a all'esempio B per vedere come verificare l'utilizzo della prenotazione di un cliente.

![Esempi di utilizzo della prenotazione](images/usage5.png)

- reservationId identifica la prenotazione di Azure utilizzata per applicare lo sconto alla macchina virtuale.
- consumptionMeter è il MeterId per la macchina virtuale a cui è applicato lo sconto della prenotazione.
- ReservationMeter mostra un costo di $ 0 perché è stato applicato lo sconto prenotazione.

Per altre informazioni, vedere [ottenere i record di utilizzo di un cliente per Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) nell' [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

>[!IMPORTANT]
>I costi relativi al software, ad esempio Microsoft Windows Server, non sono attualmente inclusi nel prezzo di una prenotazione di macchina virtuale e verranno visualizzati come voci separate nel record dell'ordine e nella fattura. Tuttavia, se un cliente ha il Vantaggio Azure Hybrid Use, i costi del software non verranno applicati. Per ulteriori informazioni, vedi [I costi del software Windows non sono inclusi nelle istanze riservate](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure

|**Per informazioni su**   |**Leggi**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendere Microsoft Azure istanze di VM riservate](azure-reservations.md)
|Acquisto di prenotazioni di Azure per i clienti nel centro per i partner   |[Acquista prenotazioni di Azure](azure-reservations-buying.md)
|Gestione delle prenotazioni di Azure nel centro per i partner | [Gestione delle prenotazioni di Azure nel centro per i partner](azure-reservations-manage.md)
|Acquisto di prenotazioni di Azure nel portale di Azure | [Pagare in anticipo per macchine virtuali con istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure |
|Gestione di prenotazioni di Azure nel portale di Azure   |[Gestire le istanze di macchina virtuale riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure  |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner
