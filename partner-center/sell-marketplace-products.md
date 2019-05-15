---
title: Vendi le sottoscrizioni a prodotti di Azure Marketplace | Centro per i partner
ms.topic: article
ms.date: 04/04/2019
description: È possibile usare Partner Center per vendere i clienti di sottoscrizioni per il Software come servizio (SaaS) prodotti pubblicati in Azure Marketplace da fornitori di Software indipendenti (ISV).
author: JnHs
ms.author: jenhayes
keywords: le sottoscrizioni, Marketplace, terze parti, ISV
ms.localizationpriority: medium
ms.openlocfilehash: a086ab3a58e926d33c118690e7b171ba4f0fd18b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133831"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vendere sottoscrizioni di prodotti di Azure Marketplace

**Si applica a**

- Centro per i partner

È possibile usare Partner Center per vendere le sottoscrizioni per il Software ai clienti come i prodotti di un servizio (SaaS) pubblicati [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) da fornitori di Software indipendenti (ISV). Ciò consente di differenziare il business e fornire ai propri clienti con le suite di software che consentono di risolvere le proprie esigenze aziendali specifiche. Gestire licenze e le sottoscrizioni per questi prodotti SaaS di Azure Marketplace, come avviene per i prodotti Microsoft.

Per altre informazioni su Azure Marketplace, vedi [domande frequenti sul Marketplace di Azure](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Visualizza Marketplace offerte e prezzi

Per visualizzare tutte le offerte disponibili, selezionare **Marketplace** dal menu di spostamento a sinistra. Per impostazione predefinita, vedrai i prodotti di tutti i tipi e le categorie. È possibile filtrare in base al tipo e/o categoria, o usare la casella di ricerca per cercare parole chiave specifiche. Selezionare un prodotto per visualizzare informazioni sui server di pubblicazione e gli SKU disponibili.

> [!NOTE]
> Alcuni prodotti che sono disponibili in Azure Marketplace potrebbero non essere visualizzati qui. Fornitori di software indipendenti possono decidere se offrire prodotti per i partner nel centro per i Partner Cloud Solution Provider (CSP) o meno. Se viene visualizzato un prodotto in Azure Marketplace che si desidera offrire ai tuoi clienti tramite Centro per i Partner, trovare le informazioni di contatto dell'editore in Azure Marketplace e informarne i membri che si è interessati.

I prezzi per i prodotti di Azure Marketplace possono cambiare di frequente. Per ottenere le informazioni sui prezzi corrente per tutti i prodotti di Marketplace, selezionare **esportazione listino** nell'angolo superiore destro delle **Marketplace** pagina. Verrà generato un foglio di calcolo con tutti i dati sui prezzi. Informazioni sui prezzi viene aggiornata ogni giorno, pertanto è possibile controllare le volte che si desidera ottenere i prezzi correnti.

## <a name="purchase-marketplace-products-for-your-customers"></a>Acquistare prodotti di Marketplace per i clienti

Acquisto di sottoscrizioni per i prodotti di Azure Marketplace SaaS segue lo stesso processo come l'acquisto di sottoscrizioni per i prodotti Microsoft. Quando si aggiunge una sottoscrizione per un cliente, è possibile scegliere di vedere solo Marketplace delle offerte da parte degli ISV selezionando **Partner** nel **server di pubblicazione** filtro. Per altre informazioni, vedi [creare una nuova sottoscrizione](create-a-new-subscription.md).

> [!IMPORTANT]
> È possibile acquistare solo Software sotto forma di sottoscrizioni di prodotto un servizio (SaaS) nel centro per i Partner. Altri tipi di offerta (ad esempio, le applicazioni Azure, contenitori o le macchine virtuali) vengono gestiti tramite il portale di Azure e fatturati in base al consumo. Per abilitare soluzioni con pagamento a consumo tramite il portale di Azure è necessaria una sottoscrizione di Azure esistente.

Si noti che alcune offerte che presenti il **Marketplace** pagina potrebbe non essere disponibile a un cliente specifico. Disponibilità potrebbe essere interessata da numerosi fattori, ad esempio se gli ISV supporta la fatturazione paese/area geografica del cliente.

> [!TIP]
> È anche possibile usare [Partner Center API](https://docs.microsoft.com/partner-center/develop/) creare sottoscrizioni di Azure Marketplace per i clienti. Per altre informazioni, vedi [creare una sottoscrizione per i prodotti di Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Con le sottoscrizioni a prodotti di Azure Marketplace, si ha la possibilità [annullare la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) entro il periodo di annullamento (24 ore per le sottoscrizioni mensili o 14 giorni per le sottoscrizioni annuali). È anche possibile [scegliere se visualizzare o meno rinnovare automaticamente la sottoscrizione](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="access-billing-info-for-marketplace-products"></a>Accedere alle info di fatturazione per i prodotti di Marketplace

Per i prodotti di Marketplace, il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. Si renderà la fattura disponibile su 8 giorni del mese successivo. È possibile accedere a tali fatture nel centro per i Partner o tramite Partner Center API.

Per altre informazioni, vedi [comprendere i tipi di fatturazione nel centro per i Partner](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Fornire il supporto per i clienti che usano i prodotti di Marketplace

Come con i prodotti Microsoft, dovrebbe essere il primo punto di contatto per il cliente per domande su fatturazione e gestione delle sottoscrizioni. Per il supporto tecnico, è necessario contattare il server di pubblicazione. Microsoft non fornisce supporto per i prodotti di Marketplace, ma verranno fornite informazioni di contatto dell'editore per il supporto all'utente.

Per altre informazioni, vedi [supporto per i prodotti di Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) e [fornire supporto ai clienti](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Gestire le sottoscrizioni tramite Partner Center API

È possibile creare una sottoscrizione per i prodotti di Azure Marketplace usando Partner Center API per ottenere un elenco di offerte per un mercato, creare e inviare un ordine per una sottoscrizione di Azure Marketplace, quindi il recupero di un collegamento di attivazione. È anche possibile usare Partner Center API per eseguire la gestione del ciclo di vita e gestire le fatture per le sottoscrizioni.

Per altre informazioni, vedi [creare una sottoscrizione per i prodotti di Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).