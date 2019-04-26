---
title: Fatturazione di prenotazioni di Azure | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
Description: Informazioni sulla fatturazione per le prenotazioni di Azure.
author: LauraBrenner
ms.author: v-petand
keywords: istanze riservate azure, istanze prenotate azure, prenotazioni, vm, gestire, fatturazione, acquisto
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b99cb2a72d69cd33f9267a956f921aa65dedd482
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135421"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Fatturazione di istanze di macchina virtuale riservate di Microsoft Azure

**Si applica a**

-  Centro per i partner
-  Portale di Microsoft Azure
-  Partner di CSP

I partner del programma Cloud Solution Provider (CSP) possono offrire istanze prenotate ai clienti sulle macchine virtuali di Microsoft Azure. I clienti possono prenotare le macchine virtuali in anticipo, per uno o tre anni, e ottenere risparmi significativi sull'uso di Azure.   

I clienti pagano anticipatamente le istanze di macchina virtuale riservate di Azure. Quando acquisti istanze di macchina virtuale riservate di Azure per conto di un cliente, riceverai le fatture e i file di riconciliazione per questi addebiti una tantum. 

>[!IMPORTANT]
>Se acquisti istanze di macchina virtuale riservate di Azure per un cliente in un mercato con una valuta diversa dalla tua, la valuta di fatturazione predefinita corrisponderà a quella del mercato del cliente e non del tuo. Se disponi di clienti in più mercati, riceverai fatture e file di riconciliazione separati per ogni valuta in cui i clienti necessitano della fatturazione, consentendoti così di fatturare nella valuta appropriata. 

Per accedere a un costo una tantum fatture e i file di riconciliazione, selezionare **fatturazione** dal centro per i Partner e quindi selezionare **una volta**. 

Per ulteriori informazioni generali sulla fatturazione in merito al programma Cloud Solution Provider, vedi [Nozioni di base sulla fatturazione](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Definizioni dei file di fatturazione per le istanze di macchina virtuale riservate di Azure

**Informazioni di fatturazione generale**

|**Campo** |**Definizione**|
|:----------------|:-----------------------------|
|US FEIN |ID fiscale federale. |
|Indirizzo fatturazione |Indirizzo legale dell'azienda utilizzato per scopi fiscali. Per modificare questo indirizzo, vai a Impostazioni account > Profilo di fatturazione partner. |
|Addebiti |Tutti gli addebiti correnti. |
|Crediti |Crediti per attività di rimborso dall'acquisto iniziale. |
|Sconti |Sconti applicabili a prenotazioni di Azure o ad altri elementi nell'ordine del cliente. |
|Imposte |Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. |
|Costi attuali totali |L'importo dovuto nella valuta della fattura per il periodo fatturato, da pagare entro la data di scadenza. |
|Istruzioni per il pagamento |Descrive quando e come pagare la fattura, in base all'area geografica. Includi sempre il numero di fattura quando effettui un pagamento. |
|N. fattura |Numero della fattura. |
|Data fattura |Data in cui la fattura è stata generata. |
|Condizioni di pagamento |Per gli acquisti una tantum sarà sempre 60 giorni. |
|Data scadenza pagamento |Data entro cui effettuare il pagamento. |


**Elenco dettagliato delle spese una tantum**

|**Campo** |**Definizione**|
|:----------------|:-----------------------------|
|Data |Data di acquisto. |
|Descrizione |Nome del prodotto. |
|Quantità |Numero di prodotti (prenotazioni, ad esempio) acquistati. |
|Prezzo unitario |Prezzo per prodotto (prenotazione, ad esempio). |
|Sconti |Eventuali sconti applicabili. |
|Importo pre-imposta |Totale parziale degli acquisti prima delle imposte. |
|Imposta sulle vendite |Importo dell'imposta. |
|Totale |Totale da pagare. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Descrizioni dei file di riconciliazione per le istanze di macchina virtuale riservate di Azure

|**Campo** |**Definizione**|
|:----------------|:-----------------------------|
|PartnerId |ID del partner, in formato GUID. |
|CustomerId |ID Microsoft univoco, in formato GUID, usato per identificare il cliente. |
|CustomerName |Nome dell'organizzazione del cliente registrato nel Centro per i partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema. |
|CustomerDomainName |Nome di dominio del cliente. |
|CustomerCountry |Paese in cui si trova il cliente. |
|InvoiceNumber |Numero di fattura in cui viene visualizzata la transazione specificata. |
|MpnId |ID MPN del partner CSP (diretto o indiretto). |
|ID MPN rivenditore |Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto. ID MPN del rivenditore nel record per la prenotazione. Corrisponde all'ID rivenditore elencato per la prenotazione specifica nel Centro per i partner. Se un partner CSP ha venduto la prenotazione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore. Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner. Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1. |
|OrderId |Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la prenotazione di Azure quando viene contattato il supporto tecnico, ma non per la riconciliazione. |
|OrderDate |Data di effettuazione dell'ordine. |
|ProductId |ID del prodotto. |
|SkuId  |ID di una SKU particolare. |
|AvailabilityId |ID di una disponibilità particolare. "Disponibilità" indica se una determinata SKU è disponibile per l'acquisto per il paese, la valuta, il segmento specificato e così via. |
|SkuName  |Titolo di una particolare SKU. |
|ProductName |Nome del prodotto. |
|ChargeType |Tipo di addebito o rettifica. |
|UnitPrice |Prezzo per prodotto ordinato. |
|Quantità |Numero di prodotti ordinati. |
|Subtotal |Totale al lordo delle imposte. Verifica che il subtotale corrisponda al totale previsto, in caso di sconto. |
|TaxTotal |Totale di tutte le imposte applicabili. |
|Totale |Importo totale di questo acquisto. |
|Valuta |Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione. |
|DiscountDetails |Elenco dettagliato di eventuali sconti pertinenti. |


## <a name="manage-your-billing"></a>Gestire la fatturazione

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Visualizzare lo stato della fatturazione corrente, le fatture e i file di riconoscimento

1.  Nel centro per i Partner, selezionare **fatturazione** e quindi **una volta** per visualizzare il tuo stato di fatturazione. 
2.  Seleziona una fattura o un file di riconoscimento per visualizzare informazioni più dettagliate. 

### <a name="view-a-customers-order-history"></a>Visualizzare la cronologia degli ordini di un cliente

1.  Selezionare **clienti** dal menu di scelta Centro per i Partner.
2.  Nella pagina **Clienti** trova il cliente di cui desideri visualizzare la cronologia ordini e seleziona la freccia giù per espandere il record del cliente. 
3.  Seleziona **Visualizza ordini** per visualizzare la cronologia degli ordini.

### <a name="create-a-credit-or-void-note"></a>Creare un accredito o annullare una fattura

In determinate situazioni, potresti avere l'esigenza di annullare una fattura ed emetterne una nuova. Ad esempio, un cliente può cambiare il nome della propria attività e ricevere una fattura in cui figura il vecchio nome. 

Per annullare una fattura ed emetterne una nuova, scarica il modulo dalla pagina di fatturazione in Rettifiche.

## <a name="azure-reservations-resources"></a>Risorse sulle prenotazioni di Azure
|**Per informazioni su**   |**Leggere questo**    |
|:-----------------------------|:-----------------|
|Panoramica delle prenotazioni di Azure in CSP  | [Vendi le istanze di macchina virtuale riservate di Azure di Microsoft](azure-reservations.md)
|Acquisto di istanze riservate di Azure per i clienti nel centro per i Partner   |[Acquisto di prenotazioni di Azure](azure-reservations-buying.md)
| La gestione delle prenotazioni di Azure nel centro per i Partner | [La gestione delle prenotazioni di Azure nel centro per i Partner](azure-reservations-manage.md)
|Acquisto di prenotazioni di Azure nel portale di Azure | [Pagare in anticipo per macchine virtuali con istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) nella Guida di Azure |
|Gestione di prenotazioni di Azure nel portale di Azure   |[Gestire le istanze di macchina virtuale riservate](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) nella Guida di Azure  |
|Acquisto di prenotazioni di Azure mediante l'API del Centro per i partner | [Acquisto di istanze di macchina virtuale riservate di Azure](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) nella documentazione per sviluppatori del Centro per i partner

 
