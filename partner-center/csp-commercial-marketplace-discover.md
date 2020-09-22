---
title: Scopri le offerte-Marketplace commerciale
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri in che modo i partner CSP possono usare il centro per i partner per visualizzare o cercare offerte SaaS o prezzi di Marketplace da fornitori di software indipendenti (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000415"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Scopri le offerte e i prezzi nel Marketplace commerciale del centro per i partner

**Si applica a**

- Centro per i partner
- Partner aderenti al programma CSP

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

Quando fornitori di software indipendenti (ISV) scelgono di pubblicare un'offerta nel Marketplace commerciale, possono anche decidere se desiderano rendere disponibile l'offerta nel programma CSP. Se scelgono di vendere l'offerta tramite il programma CSP, i partner CSP dovrebbero vedere l'offerta nell'area del Marketplace del centro per i partner.

Se un'offerta ISV non viene visualizzata come previsto nel centro per i partner, è possibile che:

- L'ISV ha deciso di non vendere l'offerta tramite il programma CSP. Ad esempio, alcuni prodotti ISV potrebbero essere stati resi disponibili in altre aree del Marketplace commerciale, ad esempio in [Microsoft AppSource](https://appsource.microsoft.com/) e in [Azure Marketplace](https://azuremarketplace.microsoft.com/), ma potrebbero non essere visualizzati per i CSP nel Marketplace del centro per i partner.

- L'ISV ha deciso di rendere l'offerta esclusiva solo a un numero selezionato di partner CSP. Per ulteriori informazioni sulle offerte esclusive, vedere più avanti in questo argomento della guida.

- Il tipo di offerta potrebbe non essere transazionale tramite il centro per i partner o portale di Azure, ad esempio contenitori o alcune offerte basate sull'utilizzo.

- Il paese di fatturazione dei clienti associati potrebbe non essere supportato per questa offerta ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Visualizzare le offerte del Marketplace nel centro per i partner

Per visualizzare le offerte di Marketplace commerciali disponibili nel programma CSP: 

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **CSP** dal menu di spostamento a sinistra.

2. Selezionare **Vendi**, seguito da **Marketplace**. Per impostazione predefinita, vengono visualizzati i prodotti di tutti i tipi e le categorie.

3. Selezionare un filtro in base al tipo o alla categoria. È anche possibile usare la **ricerca** per trovare parole chiave, nomi di offerte o nomi di editori ISV specifici.

4. Selezionare l'offerta di un prodotto specifico dall'elenco. Verrà visualizzata una scheda Panoramica del prodotto in cui è possibile ottenere altre informazioni sull'offerta. Le informazioni su questa scheda possono includere: 

    - Descrizione del prodotto o dell'offerta

    - Ulteriori informazioni sul server di pubblicazione ISV

    - Collegamenti alla documentazione o ai materiali di marketing caricati dall'editore ISV

    - Altri contatti ISV possibili per il supporto tecnico, la progettazione o un contatto per il programma CSP

5. Per visualizzare altre informazioni sui piani disponibili, gli SKU o i prezzi di un'offerta, selezionare la scheda **piani e prezzi** . In questa scheda viene visualizzato:

    - I mercati in cui questa offerta è disponibile

    - Elenco di SKU o piani disponibili per l'offerta

    - Prezzi per ogni SKU o piano disponibile

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Visualizzare le offerte del Marketplace tramite le API del centro

I partner del programma CSP possono anche usare le API per restituire un elenco di offerte idonee. Le offerte idonee saranno solo le offerte ISV SaaS disponibili per il partner per la vendita tramite il Marketplace del partner Center. Per i partner che usano le API per identificare le offerte nel catalogo, vedere le indicazioni per [ottenere un elenco di offerte per un mercato](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Visualizza i prezzi più recenti dell'offerta Marketplace nel centro per i partner

Per i dettagli più recenti sui prezzi associati a un'offerta, seguire questa procedura:

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner, quindi selezionare **CSP** dal menu di spostamento a sinistra.

2. Selezionare **Vendi**, seguito da **prezzi e offerte**.

3. Scorrere verso il basso fino alla sezione **Marketplace** , selezionare una località e scaricare **prezzi per Marketplace**. Viene generato un foglio di calcolo con i dati più recenti sui prezzi per le offerte SaaS, basate sulle licenze disponibili dagli editori ISV. Alcuni prezzi per le applicazioni Azure possono essere visualizzati anche qui. Queste informazioni vengono aggiornate ogni giorno, in modo che sia possibile controllarle per i prezzi correnti con la frequenza di scelta.

4. Se un prodotto ISV include un periodo di valutazione gratuito, nel foglio di calcolo vengono visualizzate due righe per il prodotto:

    - Una riga Visualizza il prezzo della versione di valutazione gratuita di zero. Questo significa che è disponibile un periodo di valutazione gratuito.

    - L'altra riga indica il prezzo e le condizioni che verranno applicate al termine del periodo di valutazione gratuita.

Un partner del programma CSP può essere idoneo per altri incentivi associati a determinate offerte di Marketplace commerciali. Per ulteriori informazioni su altri incentivi, vedere la guida per gli [incentivi CSP](https://aka.ms/partnerincentives) (richiede l'accesso CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Informazioni sulle offerte esclusive del Marketplace

Gli ISV hanno la possibilità di rendere disponibili le loro offerte solo a partner specifici nel programma CSP. Questa operazione è nota come offerta esclusiva. Tutti i partner del programma CSP possono comunque visualizzare tutte le offerte ISV nel Marketplace commerciale del centro per i partner, incluse quelle offerte contrassegnate come esclusive.

Se un'offerta **non** è contrassegnata come esclusiva, tutti i partner possono acquistare tale offerta (presupponendo che il paese di fatturazione del cliente selezionato corrisponda alla disponibilità del paese dell'offerta ISV).

Per ogni offerta contrassegnata come esclusiva, tuttavia, solo i partner selezionati dall'ISV saranno in grado di acquistare l'offerta.

> [!NOTE]
> Se viene visualizzata un'offerta contrassegnata come esclusiva che si vuole vendere ai clienti, contattare direttamente l'ISV e richiedere l'autorizzazione a vendere l'offerta esclusiva. Quando si visualizzano i dettagli di un'offerta esclusiva, è possibile che venga visualizzato un collegamento **Contatta ISV** che è possibile selezionare.

Per ulteriori informazioni sull'esperienza ISV nel Marketplace commerciale, vedere provider di [soluzioni cloud](/azure/marketplace/cloud-solution-providers).

Per altre informazioni sull'esperienza CSP nel Marketplace, vedere Panoramica del [Marketplace commerciale](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Passaggi successivi

- [Acquista offerte per Marketplace commerciali](csp-commercial-marketplace-purchase.md)