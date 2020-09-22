---
title: Usare i file di riconciliazione
ms.topic: article
ms.date: 06/08/2020
description: Informazioni sui file di riconciliazione nel centro per i partner e su come interpretare le visualizzazioni dettagliate degli articoli di linea degli addebiti per un determinato ciclo di fatturazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999705"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Informazioni su come leggere le voci nei file di riconciliazione del centro per i partner

Si applica a:

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government

È possibile scaricare i file di riconciliazione dal centro per i partner per una visualizzazione dettagliata di ogni addebito in un ciclo di fatturazione. I dettagli dell'elemento di riga includono gli addebiti per le sottoscrizioni di ogni cliente ed eventi dettagliati, ad esempio l'aggiunta a metà del periodo di licenze a una sottoscrizione.

Ruoli appropriati:

- Amministratore fatturazione
- Amministratore globale

Per informazioni su come leggere la **fattura**, vedere [leggere la fattura](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Informazioni sui campi del file di riconciliazione

- [Campi del file di riconciliazione basato su licenza](license-based-recon-files.md)
- [Campi del file di riconciliazione basata sull'utilizzo](usage-based-recon-files.md)
- [Campi del file di riconciliazione dell'utilizzo con classificazione giornaliera](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Informazioni sui tipi di addebito nei file di riconciliazione

Per informazioni sui tipi di addebiti nei file di riconciliazione (colonna **ChargeType** ), vedere [tipi di addebiti per i file di riconciliazione](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Correzione dei problemi di formattazione

Occasionalmente, un file di riconciliazione potrebbe contenere problemi di formattazione. Ad esempio, questo problema può verificarsi se le impostazioni locali en-US non vengono usate.

Per correggere eventuali problemi di formattazione nei file di riconciliazione, attenersi alla procedura seguente:

1. Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.
2. Consente di selezionare la prima colonna del file.
3. Aprire la **procedura guidata Converti testo in colonne**. Sulla barra multifunzione selezionare **dati**, quindi selezionare **testo in colonne**.
4. Nella procedura guidata selezionare **tipo di file delimitato**. Quindi selezionare **Avanti**.
5. Nel campo **delimitatori** selezionare **virgola**. Se la **scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Quindi selezionare **Avanti**.
6. Nel campo **formato dati colonna** selezionare **Data: MDY**. Quindi selezionare **Avanti**.
7. Nel campo **formato dati colonna** selezionare **testo** per tutte le colonne Amount. Quindi selezionare **Fine**.

## <a name="download-reconciliation-files-programmatically"></a>Scarica i file di riconciliazione a livello di codice

I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare. Per scaricare i file di riconciliazione a livello di codice, vedere [ottenere le voci di riga della fattura](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Tasse per la mappa o IVA

Per mappare le imposte o le imposte a valore aggiunto (IVA) alla fattura:

- Sommare la colonna **Tax** dal file basato sulle licenze.
- Sommare la colonna **TaxAmount** dal file basato sull'utilizzo.

## <a name="itemize-reconciliation-files-by-partner"></a>Descrivere i file di riconciliazione per partner

I partner del **modello indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenze e utilizzo per descrivere i file in base al rivenditore.

| ID MPN | Descrizione |
| ------ | ----------- |
| ID MPN | Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto). |
| [ID MPN rivenditore](#reseller-mpn-id) | [Identificatore MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id). Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel centro per i partner. Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto. |

### <a name="reseller-mpn-id"></a>ID MPN rivenditore

Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, l' **ID MPN** viene elencato due volte, sia come **ID MPN** sia come **ID MPN rivenditore**.

Se un partner CSP ha un rivenditore senza **ID MPN**, questo valore viene impostato invece sull' **ID MPN** del partner.

Se il partner CSP rimuove un **ID MPN rivenditore**, questo valore viene impostato su *-1*.

Per visualizzare o aggiornare l' **ID MPN del rivenditore**:

1. Accedere al Centro per i partner.
2. Nel menu del Centro per i partner scegli **Clienti**.
3. Scegliere il cliente dall'elenco.
4. Nel menu cliente selezionare **sottoscrizioni**.
5. Scegliere la sottoscrizione dall'elenco.
6. Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.