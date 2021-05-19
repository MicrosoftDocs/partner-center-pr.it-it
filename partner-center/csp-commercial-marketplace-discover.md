---
title: Scoprire le offerte - Marketplace commerciale
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come i partner CSP possono usare Partner Center per visualizzare o cercare nel marketplace offerte SaaS o prezzi da fornitori di software indipendenti (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147973"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Scoprire offerte e prezzi nel marketplace Partner Center commerciale

**Ruoli appropriati:** amministratore globale | Agente amministratore

Quando i fornitori di software indipendenti (ISV) scelgono di pubblicare un'offerta nel marketplace commerciale, possono anche decidere se l'offerta deve essere resa disponibile nel programma CSP. Se scelgono di vendere l'offerta tramite il programma CSP, i partner CSP dovrebbero vedere l'offerta Partner Center Marketplace.

Se un'offerta ISV non viene visualizzata come previsto Partner Center, è possibile che:

- L'ISV ha deciso di non vendere l'offerta tramite il programma CSP. Ad esempio, alcuni prodotti ISV potrebbero essere stati resi disponibili in altre aree del marketplace commerciale (ad esempio [in Microsoft AppSource](https://appsource.microsoft.com/) e [Azure Marketplace),](https://azuremarketplace.microsoft.com/)ma potrebbero non essere visualizzati per i partner nel programma CSP in Partner Center Marketplace.

- L'ISV ha deciso di rendere l'offerta esclusiva solo a un numero selezionato di partner CSP. Per altre informazioni sulle offerte esclusive, vedere più avanti in questo argomento della Guida.

- Il tipo di offerta potrebbe non essere transazionabile tramite Partner Center o portale di Azure (ad esempio, contenitori o alcune offerte basate sull'utilizzo).

- Il paese di fatturazione dei clienti associati potrebbe non essere supportato per questa offerta ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Visualizzare le offerte del Marketplace in Partner Center

Per visualizzare le offerte del marketplace commerciale disponibili nel programma CSP:

1. Accedere Partner Center [dashboard](https://partner.microsoft.com/dashboard)e quindi selezionare **CSP** dal menu di spostamento a sinistra.

2. Selezionare **Sell (Vendi),** quindi **Marketplace.** Per impostazione predefinita, verranno visualizzati prodotti di tutti i tipi e categorie.

3. Selezionare un filtro per tipo o categoria. È anche possibile usare **La ricerca per** trovare parole chiave specifiche, nomi di offerte o nomi di editori ISV.

4. Selezionare un'offerta di prodotto specifica dall'elenco. Verrà visualizzato una scheda Panoramica del prodotto in cui è possibile ottenere altre informazioni sull'offerta. Le informazioni in questa scheda possono includere: 

    - Descrizione del prodotto o dell'offerta

    - Altre informazioni sul server di pubblicazione ISV

    - Collegamenti alla documentazione o ai materiali di marketing caricati dall'editore ISV

    - Altri possibili contatti ISV per l'assistenza clienti, il reparto tecnico o un contatto per il programma CSP

5. Per visualizzare altre informazioni sui piani, sugli SKU o sui prezzi disponibili di un'offerta, selezionare la **scheda Piani e** prezzi. Questa scheda mostrerà:

    - I mercati in cui questa offerta è disponibile

    - Elenco di SKU o piani disponibili per l'offerta

    - Prezzi per ogni SKU o piano disponibile

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Visualizzare le offerte del Marketplace Partner Center API

I partner del programma CSP possono anche usare le API per restituire un elenco di offerte idonee. Le offerte idonee saranno solo le offerte ISV SaaS disponibili per la vendita da parte del partner Partner Center marketplace. Per i partner che usano le API per identificare le offerte nel catalogo, vedere le linee guida per ottenere un [elenco di offerte per un mercato.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Visualizzare i prezzi più recenti dell'offerta marketplace in Partner Center

Seguire questa procedura per i dettagli più recenti sui prezzi associati a un'offerta:

1. Accedere Partner Center [dashboard](https://partner.microsoft.com/dashboard)e quindi selezionare **CSP** dal menu di spostamento a sinistra.

2. Selezionare **Sell (Vendi),** quindi **Pricing and offers (Prezzi e offerte).**

3. Scorrere verso il basso fino **alla sezione Marketplace,** selezionare un percorso e scaricare **i prezzi del Marketplace.** Verrà generato un foglio di calcolo con i dati più recenti sui prezzi per SaaS, le offerte basate su licenza e le offerte a consumo disponibili dagli editori ISV. Alcuni prezzi delle applicazioni Azure possono essere visualizzati anche qui. Queste informazioni vengono aggiornate ogni giorno, quindi è possibile controllarvi i prezzi correnti con la frequenza scelta.

4. Se un prodotto ISV include un periodo di valutazione gratuito, nel foglio di calcolo verranno visualizzate due righe per il prodotto:

    - Una riga mostra il prezzo della versione di valutazione gratuita pari a zero. Ciò significa che è disponibile un periodo di valutazione gratuito.

    - L'altra riga mostra il prezzo e i termini che verranno applicati al termine del periodo di valutazione gratuita.

I partner del programma CSP possono essere idonei per altri incentivi associati a determinate offerte del marketplace commerciale. Per altre informazioni su altri incentivi, vedere la guida [agli incentivi CSP](https://aka.ms/partnerincentives) (richiede l'accesso CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Informazioni sulle offerte esclusive del marketplace

Gli ISV hanno la possibilità di rendere le offerte disponibili solo a partner specifici nel programma CSP. Questa operazione è nota come offerta esclusiva. Tutti i partner del programma CSP possono comunque visualizzare tutte le offerte ISV Partner Center marketplace commerciale, incluse quelle contrassegnate come esclusive.

Se un'offerta non **è** contrassegnata come Esclusiva, tutti i partner possono acquistare l'offerta (presupponendo che il paese di fatturazione del cliente selezionato corrisponda alla disponibilità del paese dell'offerta dell'ISV).

Per qualsiasi offerta contrassegnata come Esclusiva, tuttavia, solo i partner selezionati dall'ISV potranno acquistare l'offerta.

> [!NOTE]
> Se viene visualizzata un'offerta contrassegnata come Esclusiva che si vuole vendere ai clienti, contattare direttamente l'ISV e chiedere l'autorizzazione per vendere l'offerta esclusiva. Quando si visualizzano i dettagli di un'offerta esclusiva, è possibile che venga visualizzato un collegamento **Contatta ISV** che è possibile selezionare.

Per altre informazioni sull'esperienza isv nel marketplace commerciale, vedere [Cloud Solution Provider.](/azure/marketplace/cloud-solution-providers)

Per altre informazioni sull'esperienza CSP nel marketplace, vedere [Panoramica del marketplace commerciale.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Passaggi successivi

- [Acquistare offerte del marketplace commerciale](csp-commercial-marketplace-purchase.md)