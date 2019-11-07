---
title: Vendere sottoscrizioni per prodotti del Marketplace commerciale | Centro per i partner
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Puoi usare il Centro per i partner per vendere le sottoscrizioni dei clienti per prodotti SaaS (Software as a Service) pubblicati nel Marketplace commerciale da fornitori di software indipendenti (ISV).
author: JnHs
ms.author: jenhayes
keywords: sottoscrizioni, Marketplace, terze parti, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651634"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>Vendere sottoscrizioni per prodotti del Marketplace commerciale

**Si applica a**

- Centro per i partner

Puoi usare il Centro per i partner per vendere le sottoscrizioni dei clienti per prodotti SaaS (Software as a Service) pubblicati nel Marketplace commerciale ([Microsoft AppSource](https://appsource.microsoft.com/) e [Azure Marketplace](https://azuremarketplace.microsoft.com/)) da fornitori di software indipendenti (ISV). Questo consente di distinguere la propria azienda e fornire ai clienti bundle di software che permettono di soddisfare le loro esigenze aziendali specifiche. Puoi gestire le licenze e le sottoscrizioni per questi prodotti SaaS del Marketplace come per i prodotti Microsoft.

Per altre informazioni sul Marketplace commerciale, vedi [Domande frequenti sul Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

> [!IMPORTANT]
> Nel Centro per i partner possono essere acquistate solo sottoscrizioni SaaS (Software as a Service) del Marketplace commerciale. Altri tipi di offerte del Marketplace commerciale (ad esempio applicazioni, contenitori o macchine virtuali di Azure) vengono gestiti tramite il portale di Azure e fatturati in base all'uso. Una sottoscrizione di Azure esistente è necessaria per abilitare soluzioni con pagamento in base al consumo tramite il portale di Azure.

## <a name="view-marketplace-offers-and-pricing"></a>Visualizzare le offerte e i prezzi del Marketplace

Per visualizzare tutte le offerte disponibili del Marketplace commerciale, scegli **Marketplace** dal menu di spostamento a sinistra. Per impostazione predefinita, verranno visualizzati i prodotti di tutti i tipi e le categorie. È possibile filtrare in base al tipo e/o alla categoria oppure usare la casella di ricerca per individuare parole chiave specifiche. Selezionare un prodotto per visualizzare le informazioni sull'editore e gli SKU disponibili, ad esempio se è disponibile un periodo di prova gratuito.

> [!NOTE]
> Alcuni prodotti disponibili nel Marketplace commerciale potrebbero non essere visualizzati qui. Gli ISV possono decidere se offrire o meno i propri prodotti ai partner Cloud Solution Provider (CSP) nel Centro per i partner. Se viene visualizzato un prodotto nel Marketplace commerciale che si vuole offrire ai clienti tramite il centro per i partner, trovare le informazioni di contatto dell'editore nella lista dei prodotti e indicare che si è interessati.

I prezzi per i prodotti del Marketplace commerciale possono variare di frequente. Per ottenere informazioni sui prezzi correnti di tutti i prodotti del Marketplace commerciale, seleziona **Esporta listino prezzi** nell'angolo superiore destro della pagina del **Marketplace**. Verrà generato un foglio di calcolo con tutti i dati relativi ai prezzi. Tali informazioni sui prezzi vengono aggiornate ogni giorno, pertanto potrai controllarle con la stessa frequenza con cui vuoi ottenere i prezzi correnti.

> [!TIP]
> Se un prodotto in questo elenco offre una versione di valutazione gratuita, nel foglio di calcolo saranno incluse due righe per quel prodotto. Una riga indicherà un prezzo pari a zero, ciò significa che è disponibile una versione di valutazione gratuita. Nell'altra riga verranno inclusi il prezzo e le condizioni che verranno applicati al termine del periodo di prova.
>
> Se un prodotto in questo elenco usa la [fatturazione a consumo](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing), il campo della condizione sarà vuoto.

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>Acquistare prodotti del Marketplace commerciale per i clienti

L'acquisto di sottoscrizioni per i prodotti SaaS del Marketplace commerciale segue lo stesso processo previsto per l'acquisto di sottoscrizioni per i prodotti Microsoft. Prima di acquistare una sottoscrizione, devi selezionare un cliente già esistente o aggiungerne uno nuovo.

Quando si aggiunge una sottoscrizione per un cliente, è possibile scegliere di visualizzare solo le offerte del Marketplace dagli ISV selezionando **partner** nel filtro dell'**Editore**. Per altre informazioni, vedere [Crea una nuova sottoscrizione](create-a-new-subscription.md).

Si noti che alcune offerte visualizzate nella pagina **Marketplace** potrebbero non essere disponibili per un cliente specifico. La disponibilità può essere interessata da diversi fattori, ad esempio se l'ISV supporta il paese di fatturazione del cliente.

> [!TIP]
> Puoi anche possibile usare le [API del Centro per i partner](https://docs.microsoft.com/partner-center/develop/) per creare sottoscrizioni del Marketplace commerciale per i clienti. Per altre informazioni, vedi [Creare una sottoscrizione per i prodotti del Marketplace commerciale](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Nel caso di sottoscrizioni per prodotti del Marketplace commerciale, puoi [annullare la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) entro il periodo di annullamento (24 ore per le sottoscrizioni mensili o 14 giorni per le sottoscrizioni annuali). È anche possibile [scegliere se rinnovare automaticamente la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-commercial-marketplace-products"></a>Attivazione delle licenze per i prodotti del Marketplace commerciale

Per i tipi di offerta SaaS (Software as a Service), l'assegnazione e l'attivazione delle licenze vengono gestite tramite il fornitore di software indipendente (ISV) che ha pubblicato il prodotto. Per completare questo processo, è necessario visitare il sito dell'editore, usando un collegamento personalizzato con un codice di autorizzazione che consente all'autore di identificare l'acquisto specifico. Questo collegamento è disponibile nella pagina di conferma visualizzata dopo l'acquisto di un'offerta SaaS e nella pagina **Sottoscrizioni** (nella riga relativa a tale offerta). Per recuperare il [collegamento, è anche possibile usare le API del Centro per i partner](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Quando si visita il sito dell'editore usando questo collegamento, verranno visualizzate le informazioni aggiuntive o l'azione necessaria per il provisioning e l'assegnazione delle licenze o il completamento del processo di installazione. I passaggi necessari possono variare a seconda dell'autore e dell'offerta. L'utente è responsabile dell'invio di eventuali informazioni necessarie (o dell'invio dell'URL al cliente per fornire direttamente queste informazioni). Dopo essere state fornite le informazioni necessarie, il server di pubblicazione effettuerà il provisioning e l'assegnazione delle licenze appropriate. La fatturazione della sottoscrizione avrà inizio solo dopo la corretta assegnazione delle licenze.

## <a name="access-billing-info-for-commercial-marketplace-products"></a>Accedere alle informazioni di fatturazione per i prodotti del Marketplace commerciale

Per i prodotti del Marketplace commerciale, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. La fattura sarà disponibile l'ottavo giorno del mese successivo. È possibile accedere a queste fatture nel Centro per i partner o usando le API del Centro per i partner.

Per altre informazioni, vedere [Informazioni sui tipi di fatturazione nel Centro per i partner](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>Fornire supporto ai clienti che usano prodotti del Marketplace commerciale

Esattamente come con i prodotti Microsoft, l'utente dovrebbe continuare a essere il primo contatto per il cliente per altre informazioni sulla gestione della fatturazione e della sottoscrizione. Per ottenere supporto tecnico, è necessario contattare l'editore. Microsoft non fornisce supporto per i prodotti commerciali del Marketplace, ma fornirà le informazioni di contatto per il supporto dell'editore.

Per altre informazioni, vedi [Supporto per i prodotti del Marketplace commerciale](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products) e [Fornire supporto ai clienti](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gestire le sottoscrizioni usando le API del Centro per i partner

Puoi creare una sottoscrizione per i prodotti del Marketplace commerciale usando le API del Centro per i partner. A tale scopo, devi innanzitutto ottenere un elenco di offerte per un mercato, quindi creare e inviare un ordine per una sottoscrizione specifica del Marketplace commerciale. Devi infine recuperare un collegamento di attivazione per la sottoscrizione.

È anche possibile usare le API del Centro per i partner per eseguire la gestione del ciclo di vita e gestire le fatture per queste sottoscrizioni.

Per altre informazioni, vedi [Creare una sottoscrizione per i prodotti del Marketplace commerciale](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).