---
title: Gestire l'elenco dei clienti
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I record dei clienti sono tra le risorse di informazioni più importanti. Informazioni su come visualizzare, cercare, aggiornare & informazioni sull'esportazione nell'elenco dei clienti del centro per i partner.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 865af6a054fc10cddd5422e1ef91ec3df14f69aa
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377745"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gestisci l'elenco dei clienti: Cerca, aggiorna o Esporta clienti nel centro per i partner

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

I record dei clienti sono tra le informazioni più importanti nel Centro per i partner. Puoi eseguire una ricerca nel database degli account dei clienti, esportare l'intero database dei clienti o esportarne un sottoinsieme, in un formato di file con valori delimitati da virgole (CSV) compatibile con Excel. Puoi anche esportare le informazioni sulle sottoscrizioni del cliente in un file CSV.

Anche i log attività offrono dati esportabili sulle transazioni e le operazioni di gestione per i clienti. Per altre informazioni, vedi [Visualizzare i log attività dei clienti](activity-logs.md).

## <a name="search-for-a-customer"></a>Cercare un cliente

1.  Scegliere **clienti**dal menu **centro partner** .
2.  Per cercare un cliente, immettere il nome del cliente o un nome di dominio nella casella di ricerca.
3.  Seleziona la **freccia in giù** alla fine della riga di un cliente per visualizzare l'ID Microsoft oltre ai link rapidi per le sottoscrizioni e i servizi associati.

## <a name="update-a-customers-company-name"></a>Aggiornare il nome della società del cliente

Scegliere **clienti**dal menu **centro partner** .
2.  Per cercare un cliente, immettere il nome del cliente o un nome di dominio nella casella di ricerca.
3.  Seleziona la **freccia in giù** alla fine della riga di un cliente per visualizzare l'ID Microsoft oltre ai link rapidi per le sottoscrizioni e i servizi associati.
4.  In base alle informazioni **fatturate** del cliente, aggiornare il nome della società. Quando salvi il nuovo valore, questo sarà riportato nell'elenco dei clienti. Questa operazione modificherà solo il nome della società di fatturazione e il valore nell'elenco dei clienti. Non sarà applicata altrove.
<sup>1</sup>
## <a name="export-your-customer-list"></a>Esportare l'elenco dei clienti

1. Scegliere **clienti**dal menu **centro partner** .
2. Seleziona **Esporta clienti**.

   Il Centro per i partner converte l'elenco completo dei clienti in un file CSV e lo carica nella cartella di download predefinita nel tuo computer. Puoi anche esportare sottoinsiemi dei dati dei clienti. Le colonne di dati includono:

   - **ID Microsoft**;
   - **Nome della società**;
   - **Nome di dominio primario**;
   - **Relazione** - Relazione di business del partner con ogni cliente elencato.

    Per impostazione predefinita, il Centro per i partner esporta l'intero elenco dei clienti, indipendentemente dalla lunghezza. Puoi anche eseguire una ricerca nell'elenco dei clienti in base al nome dell'azienda o del dominio e quindi esportare il sottoinsieme di dati corrispondente.

3. Se si è un provider indiretto, è possibile filtrare l'elenco dei clienti in base al rivenditore indiretto. Selezionare **Filtra per rivenditore indiretto** dall'elenco e quindi scegliere un rivenditore.
<sup>1</sup>

## <a name="export-customer-subscription-information"></a>Esporta le informazioni sulla sottoscrizione del cliente

1. Scegliere **clienti**dal menu **centro partner** .

2. Seleziona **Nome azienda** per qualsiasi cliente. Viene aperta la pagina **Sottoscrizioni** del cliente con l'elenco completo delle sottoscrizioni di prodotti.

3. Seleziona **Esporta sottoscrizioni**. Il Centro per i partner converte i dati relativi alle sottoscrizioni del cliente in un file CSV e lo carica nella cartella di download predefinita nel tuo computer. Le colonne di dati includono:
   - **ID sottoscrizione**;
   - **Sottoscrizione** - nome del prodotto per la sottoscrizione;
   - **Quantità** - numero delle licenze acquistate;
   - **Stato**;
   - **Rivenditore** - ID del rivenditore che possiede e gestisce la sottoscrizione.

> [!NOTE]  
> Per ulteriori informazioni sulla gestione delle sottoscrizioni, vedere [sottoscrizioni clienti](customer-subscriptions.md).
