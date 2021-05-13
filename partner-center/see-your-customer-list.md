---
title: Gestire l'elenco dei clienti
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I record dei clienti sono tra gli asset di informazioni più importanti. Informazioni su come visualizzare, cercare, aggiornare e & le informazioni sull'Partner Center dei clienti.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854503"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gestire l'elenco dei clienti: cercare, aggiornare o esportare clienti in Partner Center

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** Agente di amministrazione | Amministratore globale

I record dei clienti sono tra le informazioni più importanti nel Centro per i partner. Puoi eseguire una ricerca nel database degli account dei clienti, esportare l'intero database dei clienti o esportarne un sottoinsieme, in un formato di file con valori delimitati da virgole (CSV) compatibile con Excel. Puoi anche esportare le informazioni sulle sottoscrizioni del cliente in un file CSV.

Anche i log attività offrono dati esportabili sulle transazioni e le operazioni di gestione per i clienti. Per altre informazioni, vedi [Visualizzare i log attività dei clienti](activity-logs.md).

## <a name="search-for-a-customer"></a>Cercare un cliente

1. Dal menu **Partner Center** selezionare **Clienti**.
2. Per cercare un cliente, immettere il nome del cliente o un nome di dominio nella casella di ricerca.
3. Seleziona la **freccia in giù** alla fine della riga di un cliente per visualizzare l'ID Microsoft oltre ai link rapidi per le sottoscrizioni e i servizi associati.

## <a name="update-a-customers-company-name"></a>Aggiornare il nome della società del cliente

Dal menu **Partner Center** selezionare **Clienti**.
2. Per cercare un cliente, immettere il nome del cliente o un nome di dominio nella casella di ricerca.
3. Seleziona la **freccia in giù** alla fine della riga di un cliente per visualizzare l'ID Microsoft oltre ai link rapidi per le sottoscrizioni e i servizi associati.
4. Nelle informazioni di fatturazione **del cliente** aggiornare il nome della società. Quando salvi il nuovo valore, questo sarà riportato nell'elenco dei clienti. Questa operazione modificherà solo il nome della società di fatturazione e il valore nell'elenco dei clienti. Non sarà applicata altrove.

## <a name="export-your-customer-list"></a>Esportare l'elenco dei clienti

1. Dal menu **Partner Center** selezionare **Clienti**.
2. Seleziona **Esporta clienti**.

   Il Centro per i partner converte l'elenco completo dei clienti in un file CSV e lo carica nella cartella di download predefinita nel tuo computer. Puoi anche esportare sottoinsiemi dei dati dei clienti. Le colonne di dati includono:

   - **ID Microsoft**;
   - **Nome società**;
   - **Nome di dominio primario**;
   - **Relazione** - Relazione di business del partner con ogni cliente elencato.

    Per impostazione predefinita, il Centro per i partner esporta l'intero elenco dei clienti, indipendentemente dalla lunghezza. Puoi anche eseguire una ricerca nell'elenco dei clienti in base al nome dell'azienda o del dominio e quindi esportare il sottoinsieme di dati corrispondente.

3. Se si è un provider indiretto, è possibile filtrare l'elenco dei clienti in base al rivenditore indiretto. Selezionare **Filtra per rivenditore indiretto** nell'elenco e quindi scegliere un rivenditore.


## <a name="export-customer-subscription-information"></a>Esportare le informazioni sulla sottoscrizione del cliente

1. Dal menu **Partner Center** selezionare **Clienti**.

2. Seleziona **Nome azienda** per qualsiasi cliente. Viene aperta la pagina **Sottoscrizioni** del cliente con l'elenco completo delle sottoscrizioni di prodotti.

3. Seleziona **Esporta sottoscrizioni**. Il Centro per i partner converte i dati relativi alle sottoscrizioni del cliente in un file CSV e lo carica nella cartella di download predefinita nel tuo computer. Le colonne di dati includono:
   - **ID sottoscrizione**;
   - **Sottoscrizione** - nome del prodotto per la sottoscrizione;
   - **Quantità** - numero delle licenze acquistate;
   - **Stato**;
   - **Rivenditore** - ID del rivenditore che possiede e gestisce la sottoscrizione.

> [!NOTE]  
> Per altre informazioni sulla gestione delle sottoscrizioni, vedere [Sottoscrizioni dei clienti.](customer-subscriptions.md)
