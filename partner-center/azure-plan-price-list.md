---
title: Listino prezzi per il piano di Azure | Centro per i partner
ms.topic: article
ms.date: 11/01/2019
description: Come visualizzare il listino prezzi per le sottoscrizioni in base al piano di Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 53e5327b505de1c1860e44b477aca21b5aef2d2b
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428542"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Listino prezzi per la nuova esperienza commerciale di Azure in CSP 

Il listino prezzi per la nuova esperienza commerciale di Azure in CSP viene pubblicato nel Centro per i partner. Il listino prezzi viene distribuito in modo dinamico in un file dettagliato costantemente aggiornato e i prezzi sono riportati solo in USD. La fatturazione, tuttavia, viene eseguita nella valuta supportata applicabile alla località della valuta del cliente. Per altre informazioni sulla fatturazione nella località della valuta del cliente, vedi [Piano di Azure - fatturazione](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Visualizzare il listino prezzi per le sottoscrizioni in base ai prezzi del piano di Azure

1. Dal menu del Centro per i partner a sinistra seleziona **Vendita** e quindi **Marketplace**.

2. Accanto a **Tipo di esportazione** seleziona **Azure plan consumption pricing** (Prezzi per l'utilizzo del piano di Azure).

3. Accanto a **Prezzi per data** seleziona la data desiderata, ad esempio **Corrente**. Nota: puoi anche selezionare **FX rates** (Tassi di cambio) per esportare i tassi di cambio correnti.

![prezzi di Azure 2](images/azure/pricelist2.jpg)

4. In **Marketplace** seleziona i valori di **Tipo** e **Categoria** per il prodotto oppure cerca un prodotto. Verranno visualizzati i prodotti disponibili in base alla ricerca.

![pricing](images/azure/Azurepricelist1.jpg)

5. Seleziona quindi **Esporta listino prezzi del piano di Azure** per scaricare i prezzi del piano di Azure per i prodotti selezionati.


![esportare il listino prezzi](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Specifiche del listino prezzi di Azure

- Il listino prezzi di Azure sarà disponibile dalla pagina Marketplace del Centro per i partner, nell'area **Vendita**.

- La funzionalità di esportazione dei dati sarà disponibile per i servizi di utilizzo del piano di Azure, le prenotazioni di Azure e i tassi di cambio.

- Le opzioni di esportazione includono:

    - **Today’s pricing** (Prezzi correnti): sono inclusi tutti i contatori e i prezzi dal primo giorno del mese alla data corrente del mese corrente. Sono inoltre specificati i prezzi nuovi, modificati o rimossi. Tutti i prezzi avranno date di inizio e di fine valide per indicare se sono nuovi o rimossi.

    - **Previous month's pricing** (Prezzi del mese precedente): il download di ogni tipo di risorsa verrà eseguito su base mensile. Per i file dei prezzi, saranno inclusi tutti i contatori disponibili durante il mese specificato. Se a metà del mese viene introdotto un nuovo contatore, verrà visualizzato con una data di validità definita in base alla disponibilità. In modo analogo, i prezzi sospesi vengono visualizzati con una data di fine validità per indicare quando non sono più disponibili.

    - **FX Rates** (Tassi di cambio): i tassi di cambio saranno disponibili per il download il giorno precedente il primo del mese, alle ore 18.00 PST. Se, ad esempio, vuoi visualizzare i tassi per il mese di novembre, scaricali il 31 ottobre. Saranno disponibili anche i tassi di cambio relativi al mese precedente.

- I prezzi riportati nei listini sono prezzi diretti. Alcuni partner potrebbero essere idonei a ricevere dei crediti. Per informazioni sul modo in cui viene calcolato il credito ottenuto da un partner, vedi [Come viene calcolato e pagato il credito ottenuto dai partner](partner-earned-credit-explanation.md).

- **Eligible services** (Servizi idonei): il credito ottenuto dai partner è applicabile ai servizi elencati nei **prezzi per l'utilizzo del piano di Azure** che i partner possono esportare dalla pagina dei [prezzi del piano di Azure](https://partner.microsoft.com/commerce/sales). Si noti che esistono eccezioni, tra cui i prodotti di terze parti identificati come "Terze parti" nella colonna Tags del listino prezzi relativo ai consumi del piano di Azure e le prenotazioni del piano di Azure.

## <a name="price-list-data"></a>Dati del listino prezzi

|**Campo**   |**Descrizione**   |
|--------------------------|:---------------------------|
|ProductTitle  |Titolo o nome del prodotto|
|ProductID   |ID del prodotto|
|SKuId|ID dello SKU|
|SkuTitle|Titolo o nome dello SKU|
|Autore|La parte principale sarà sempre Microsoft|
|SkuDescription|Descrizione dello SKU|
|UnitOfMeasure|Unità che verranno addebitate o fatturate|
|TermDuration|Per i prodotti a termine, durata del periodo, applicabile alle prenotazioni|
|Mercato|Mercato di applicazione dei prezzi|
|Valuta|Valuta dei prezzi|
|UnitPrice|Prezzo per unità|
|PricingTierRangeMin|Per i prezzi a livelli, viene applicato il prezzo minimo|
|PricingTierRangeMax|Per i prezzi a livelli, viene applicato il prezzo massimo|
|EffectiveStartDate|Data di inizio dei prezzi|
|EffectiveEndDate|Data di fine dei prezzi|
|MeterIds|ID contatore dello SKU del prodotto|
|MeterType|Tipo di contatore|
|Tag|Proprietà relative all'elemento, che per i prezzi relativi al piano di Azure saranno Azure oppure Azure e Reservations (per le prenotazioni)|

Per i dettagli, vedi le [informazioni sul listino prezzi](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
