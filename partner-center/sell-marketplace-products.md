---
title: Vendere sottoscrizioni ai prodotti Azure Marketplace | Centro per i partner
ms.topic: article
ms.date: 07/12/2019
description: È possibile usare il centro per i partner per vendere le sottoscrizioni dei clienti ai prodotti SaaS (software as a Service) pubblicati in Azure Marketplace da fornitori di software indipendenti (ISV).
author: JnHs
ms.author: jenhayes
keywords: sottoscrizioni, Marketplace, terze parti, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 4dda776e7ebdece3a8a15c3576b64d93d3e4158c
ms.sourcegitcommit: dd961f85bc790e56c70479a5926177454dd8e855
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/12/2019
ms.locfileid: "67854507"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vendere sottoscrizioni di prodotti di Azure Marketplace

**Si applica a**

- Centro per i partner

È possibile usare il centro per i partner per vendere le sottoscrizioni dei clienti ai prodotti SaaS (software as a Service) pubblicati in [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) da fornitori di software indipendenti (ISV). In questo modo è possibile distinguere la propria azienda e fornire ai clienti bundle software che risolvono le specifiche esigenze aziendali. È possibile gestire le licenze e le sottoscrizioni per questi prodotti SaaS di Azure Marketplace come per i prodotti Microsoft.

Per altre informazioni su Azure Marketplace, vedere [domande frequenti su Azure Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Visualizza le offerte e i prezzi del Marketplace

Per visualizzare tutte le offerte disponibili, scegliere **Marketplace** dal menu di spostamento a sinistra. Per impostazione predefinita, verranno visualizzati i prodotti di tutti i tipi e le categorie. È possibile filtrare in base al tipo e/o alla categoria oppure utilizzare la casella di ricerca per cercare parole chiave specifiche. Selezionare un prodotto per visualizzare le informazioni sull'editore e gli SKU disponibili, ad esempio se è disponibile un periodo di valutazione gratuito.

> [!NOTE]
> Alcuni prodotti disponibili in Azure Marketplace potrebbero non essere visualizzati qui. Gli ISV possono decidere se offrire o meno i propri prodotti ai partner Cloud Solution Provider (CSP) nel centro per i partner. Se viene visualizzato un prodotto in Azure Marketplace che si vuole offrire ai clienti tramite il centro per i partner, trovare le informazioni di contatto dell'editore in Azure Marketplace e indicare che si è interessati.

I prezzi per i prodotti Azure Marketplace possono essere modificati di frequente. Per ottenere informazioni sui prezzi correnti per tutti i prodotti Marketplace, selezionare **Esporta Listino prezzi** nell'angolo superiore destro della pagina del **Marketplace** . Verrà generato un foglio di calcolo con tutti i dati relativi ai prezzi. Le informazioni sui prezzi vengono aggiornate ogni giorno, in modo che sia possibile controllarle con la stessa frequenza con cui si vogliono ottenere i prezzi correnti.

> [!TIP]
> Se un prodotto in questo elenco offre una versione di valutazione gratuita, nel foglio di calcolo sono incluse due righe per quel prodotto. Una riga indicherà un prezzo pari a zero, che indica che è disponibile una versione di valutazione gratuita. Nell'altra riga verranno inclusi il prezzo e il termine che verranno applicati al termine del periodo di valutazione.

## <a name="purchase-marketplace-products-for-your-customers"></a>Acquistare prodotti Marketplace per i clienti

L'acquisto di sottoscrizioni per i prodotti SaaS di Azure Marketplace segue lo stesso processo di acquisto di sottoscrizioni per i prodotti Microsoft. Quando si aggiunge una sottoscrizione per un cliente, è possibile scegliere di visualizzare solo le offerte del Marketplace dagli ISV selezionando **partner** nel filtro dell' **editore** . Per altre informazioni, vedere [creare una nuova sottoscrizione](create-a-new-subscription.md).

> [!IMPORTANT]
> È possibile acquistare solo sottoscrizioni di prodotti SaaS (software as a Service) nel centro per i partner. Altri tipi di offerta, ad esempio applicazioni, contenitori o macchine virtuali di Azure, vengono gestiti tramite il portale di Azure e fatturati in base all'utilizzo. Una sottoscrizione di Azure esistente è necessaria per abilitare soluzioni con pagamento in base al consumo tramite il portale di Azure.

Si noti che alcune offerte visualizzate nella pagina **Marketplace** potrebbero non essere disponibili per un cliente specifico. La disponibilità può essere interessata da diversi fattori, ad esempio se l'ISV supporta il paese di fatturazione del cliente.

> [!TIP]
> È anche possibile usare le [API del centro](https://docs.microsoft.com/partner-center/develop/) per i partner per creare sottoscrizioni di Azure Marketplace per i clienti. Per altre informazioni, vedere [creare una sottoscrizione per i prodotti Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Con le sottoscrizioni ai prodotti Azure Marketplace, è possibile [annullare la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) entro il periodo di annullamento (24 ore per le sottoscrizioni mensili o 14 giorni per le sottoscrizioni annuali). È anche possibile [scegliere se rinnovare automaticamente la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-marketplace-products"></a>Attivazione delle licenze per i prodotti Marketplace

Per i tipi di offerta SaaS (software as a Service), l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto. Per completare questo processo, è necessario visitare il sito dell'editore, usando un collegamento personalizzato con un codice di autorizzazione che consente all'autore di identificare l'acquisto specifico. Questo collegamento è disponibile nella pagina di conferma visualizzata dopo l'acquisto di un'offerta SaaS e nella pagina **sottoscrizioni** (nella riga relativa a tale offerta). [Per recuperare il collegamento](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item), è anche possibile usare le API del centro per i partner.

Quando si visita il sito dell'editore usando questo collegamento, verranno visualizzate le informazioni aggiuntive o l'azione necessaria per il provisioning e l'assegnazione delle licenze o il completamento del processo di installazione. I passaggi necessari possono variare a seconda dell'autore e dell'offerta. L'utente è responsabile dell'invio di eventuali informazioni necessarie (o dell'invio dell'URL al cliente per fornire direttamente queste informazioni). Una volta fornite le informazioni necessarie, il server di pubblicazione effettuerà il provisioning e l'assegnazione delle licenze appropriate. La fatturazione della sottoscrizione avrà inizio solo dopo la corretta assegnazione delle licenze.

## <a name="access-billing-info-for-marketplace-products"></a>Accedi alle informazioni di fatturazione per i prodotti Marketplace

Per i prodotti del Marketplace, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. La fattura sarà disponibile l'ottavo giorno del mese successivo. È possibile accedere a queste fatture nel centro per i partner o usando le API del centro per i partner.

Per altre informazioni, vedere informazioni [sui tipi di fatturazione nel centro per i partner](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fornire supporto per i clienti che usano prodotti Marketplace

Come per i prodotti Microsoft, è necessario essere il primo punto di contatto del cliente per domande sulla gestione delle sottoscrizioni e della fatturazione. Per il supporto tecnico, è necessario contattare l'editore. Microsoft non fornisce supporto per i prodotti Marketplace, ma fornirà le informazioni di contatto per il supporto dell'editore.

Per altre informazioni, vedere [supporto per i prodotti Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) e [fornire supporto ai clienti](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gestire le sottoscrizioni usando le API del centro per i partner

È possibile creare una sottoscrizione per i prodotti Azure Marketplace usando le API del centro per i partner ottenendo un elenco di offerte per un mercato, creando e inviando un ordine per una sottoscrizione di Azure Marketplace e quindi recuperando un collegamento di attivazione. È anche possibile usare le API del centro per i partner per eseguire la gestione del ciclo di vita e gestire le fatture per queste sottoscrizioni.

Per altre informazioni, vedere [creare una sottoscrizione per i prodotti Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).