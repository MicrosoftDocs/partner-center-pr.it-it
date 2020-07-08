---
title: Listino prezzi del piano di Azure per i partner CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come i partner del programma CSP possono usare il Centro per i partner per visualizzare il listino prezzi delle sottoscrizioni in base al piano di Azure.
author: dineshvu
ms.author: dineshvu
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ecfd86d41f550bc4f124b371d87c59e928dd4253
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948404"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Listino prezzi per la nuova esperienza commerciale di Azure in CSP

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale
- Agente di supporto tecnico
- Agente di vendita
- Amministratore gestione utenti

Il listino prezzi per la nuova esperienza commerciale di Azure in CSP viene pubblicato nel Centro per i partner. Il listino prezzi viene distribuito in modo dinamico in un file dettagliato costantemente aggiornato e i prezzi sono riportati solo in USD. La fatturazione, tuttavia, viene eseguita nella valuta supportata applicabile alla località della valuta del cliente. Per altre informazioni sulla fatturazione nella località della valuta del cliente, vedi [Piano di Azure - fatturazione](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Visualizzare il listino prezzi per le sottoscrizioni in base ai prezzi del piano di Azure

1. Dal menu del Centro per i partner a sinistra seleziona **Vendita** e quindi **Marketplace**.

2. In Prezzi del piano di Azure seleziona il paese per cui vuoi ottenere i prezzi.

3. Accanto a **Tipo di esportazione** seleziona **Prezzi a consumo del piano di Azure**, **Prezzi delle prenotazioni del piano di Azure** o **Tariffe fisse** (nel caso dei tassi di cambio). 

>[!NOTE] 
>i valori **Tariffe fisse** (ovvero i tassi di cambio) non sono specifici del paese.

4. Accanto a **Prezzi per data** seleziona la data desiderata, ad esempio **Corrente**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="Specifici del paese":::

>[!NOTE] 
>puoi esportare due listini prezzi diversi, ovvero i prezzi del piano di Azure e i prezzi di terze parti del Marketplace.

## <a name="azure-price-list-specifics"></a>Specifiche del listino prezzi di Azure

- Il listino prezzi di Azure sarà disponibile dalla pagina Marketplace del Centro per i partner, nell'area **Vendita**.

- La funzionalità di esportazione dei dati sarà disponibile per i servizi di utilizzo del piano di Azure, le prenotazioni di Azure e i tassi di cambio.

- Le opzioni di esportazione includono:

  - **Today's pricing** (Prezzi correnti): sono inclusi tutti i contatori e i prezzi dal primo giorno del mese alla data corrente del mese corrente. Sono inoltre specificati i prezzi nuovi, modificati o rimossi. Tutti i prezzi avranno date di inizio e di fine valide per indicare se sono nuovi o rimossi.

  - **Previous month's pricing** (Prezzi del mese precedente): il download di ogni tipo di risorsa verrà eseguito su base mensile. Per i file dei prezzi, saranno inclusi tutti i contatori disponibili durante il mese specificato. Se a metà del mese viene introdotto un nuovo contatore, verrà visualizzato con una data di validità definita in base alla disponibilità. In modo analogo, i prezzi sospesi vengono visualizzati con una data di fine validità per indicare quando non sono più disponibili.

  - **FX Rates** (Tassi di cambio): i tassi di cambio saranno disponibili per il download il giorno precedente il primo del mese, alle ore 18.00 PST. Se, ad esempio, vuoi visualizzare i tassi per il mese di novembre, scaricali il 31 ottobre. Saranno disponibili anche i tassi di cambio relativi al mese precedente.

- I prezzi riportati nei listini sono prezzi diretti. Alcuni partner potrebbero essere idonei a ricevere dei crediti. Per informazioni sul modo in cui viene calcolato il credito ottenuto da un partner, vedi [Come viene calcolato e pagato il credito ottenuto dai partner](partner-earned-credit-explanation.md).

- **Eligible services** (Servizi idonei): il credito ottenuto dai partner è applicabile ai servizi elencati nei **prezzi per l'utilizzo del piano di Azure** che i partner possono esportare dalla pagina dei [prezzi del piano di Azure](https://partner.microsoft.com/commerce/sales). Tieni presente che esistono eccezioni, tra cui i prodotti di terze parti identificati come "Terze parti" nella colonna dei tag del listino prezzi relativo ai consumi del piano di Azure e le prenotazioni del piano di Azure.

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

È possibile esportare i listini prezzi del piano di Azure dalla [pagina Prezzi del piano di Azure e marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any).

## <a name="pricing-api-for-azure-plan"></a>API dei prezzi per il piano di Azure

Per recuperare i prezzi del piano Azure relativi ai consumi e alle prenotazioni a livello di codice, puoi usare l'[API dei prezzi](https://docs.microsoft.com/partner/develop/pricing). Puoi anche recuperare i tassi di cambio esteri.

L'API dei prezzi si trova in un endpoint diverso rispetto alle altre API del Centro per i partner. Le informazioni sui prezzi includono i prezzi dei contatori in USD relativi alle risorse e alle prenotazioni del piano di Azure, applicati alle sottoscrizioni del piano di Azure.

Questa API consente ai partner anche di recuperare i tassi di cambio mensili perché i prezzi del piano di Azure sono indicati solo in USD. Puoi usare le API per recuperare sia i prezzi sia i tassi di cambio esteri relativi al mese corrente o ai mesi precedenti.

>[!NOTE]
> L'API dei prezzi è specifica per i prezzi del piano di Azure. Per le risorse e le prenotazioni di Azure distribuite in sottoscrizioni diverse dal piano di Azure, devi continuare a usare l'API RateCard esistente e i listini prezzi pubblicati nella pagina Prezzi e offerte del Centro per i partner. L'API dei prezzi del piano di Azure non supporta i prezzi di software, marketplace o basati su postazione come Microsoft 365 o Dynamics 365.

Per altre informazioni sulle API dei prezzi del piano di Azure e dei tassi di cambio esteri, vedi tutta la [documentazione relativa all'API dei prezzi](https://docs.microsoft.com/partner/develop/pricing).
