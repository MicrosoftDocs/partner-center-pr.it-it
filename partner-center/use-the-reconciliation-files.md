---
title: Usare i file di riconciliazione
ms.topic: article
ms.date: 03/26/2021
description: Informazioni sui file di riconciliazione Partner Center e su come interpretare le visualizzazioni dettagliate degli addebiti per un determinato ciclo di fatturazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794956"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Informazioni su come leggere le voci nei file di Partner Center di riconciliazione

**Ruoli appropriati:** Amministratore fatturazione | Amministratore globale

È possibile scaricare i file di riconciliazione da Partner Center per una visualizzazione dettagliata degli elementi di riga di ogni addebito in un ciclo di fatturazione. I dettagli delle voci includono gli addebiti per le sottoscrizioni di ogni cliente e gli eventi dettagliati, ad esempio un'aggiunta a medio termine di licenze a una sottoscrizione.

Per informazioni su come leggere la **fattura,** vedere [Leggere la fattura.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Comprendere i campi del file di riconciliazione

- [Campi del file di riconciliazione basato su licenza](license-based-recon-files.md)
- [Campi del file di riconciliazione basato sull'utilizzo](usage-based-recon-files.md)
- [Campi del file di riconciliazione per l'uso quotidiano](daily-rated-usage-recon-files.md)
- [Campi del file di riconciliazione CSP per l'acquisto una sola volta](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Informazioni sul tipo di addebito nei file di riconciliazione

Per comprendere i tipi di addebiti nei file di riconciliazione (colonna **ChargeType),** vedere [Tipi di addebito file di riconciliazione](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Risolvere i problemi di formattazione

In alcuni casi, un file di riconciliazione potrebbe contenere problemi di formattazione. Ad esempio, questo problema potrebbe verificarsi se non vengono usate le impostazioni locali en-US.

Seguire questa procedura per risolvere eventuali problemi di formattazione nei file di riconciliazione:

1. Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.
2. Selezionare la prima colonna nel file.
3. Aprire la **Conversione guidata testo in colonne**. Sulla barra multifunzione selezionare **Dati** e quindi Selezionare **Testo in colonne**.
4. Nella procedura guidata selezionare **Tipo di file delimitato**. Quindi selezionare **Avanti**.
5. Nel campo **Delimitatori** selezionare **Virgola.** Se **l'opzione Scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Selezionare quindi **Avanti.**
6. Nel campo **Formato dati colonna** selezionare **Date:MDY**. Quindi selezionare **Avanti**.
7. Nel campo **Formato dati colonna** selezionare Testo per tutte le colonne quantità.  quindi fare clic su **Fine**.

## <a name="download-reconciliation-files-programmatically"></a>Scaricare i file di riconciliazione a livello di codice

I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare. Per scaricare i file di riconciliazione a livello di codice, vedere [Ottenere le voci della fattura.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Se il file supera il limite di righe in Excel

Se è possibile scaricare un file di riconciliazione ma non aprirlo in Microsoft Excel, è probabile che il file contenga più righe di quelle consentite da Excel. In questo caso, è possibile usare una delle procedure seguenti per aprire il file.

### <a name="open-a-recon-file-in-power-bi"></a>Aprire un file di ricognizione in Power BI

1. Scaricare il file di riconciliazione come di consueto.
2. Scaricare, installare e aprire un'istanza di Power BI.
3. Nella scheda Power BI **Home** selezionare **Ottieni dati.**
4. Nell'elenco Origini **dati comuni** selezionare **Testo/CSV.**
5. Quando richiesto, aprire il file di ricognizione.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Aprire un file di ricognizione in una tabella pivot di Excel

1. Scaricare il file di riconciliazione come di consueto.
2. Aprire un nuovo file in Microsoft Excel.
3. Nella scheda **Dati** selezionare Ottieni **dati,** selezionare **Da file** e quindi selezionare **Testo/CSV.**
4. Quando richiesto, aprire il file di ricognizione. Verranno visualizzati i dati.
5. Nel menu a discesa **Carica** selezionare **Carica in** e quindi **OK.**
6. Nella finestra **di dialogo Importa** dati selezionare Rapporto di tabella **pivot** per aprire il file.

## <a name="negative-amount-displayed"></a>Importo negativo visualizzato

È possibile che nel file di riconciliazione venga visualizzato un importo negativo. Questo problema è probabilmente dovuto a una delle cause seguenti:

- Il numero di licenze è stato annullato o ridotto di recente
- È stato ricevuto il credito per un contratto di licenza del servizio o per l'utilizzo di Azure

Per ottenere altre informazioni su questa transazione, verificare il rispettivo attributo relativo al tipo di addebito nel file di riconciliazione.

## <a name="map-taxes-or-vat"></a>Mappare le imposte o l'IVA

Per eseguire il mapping delle imposte o dell'imposta sul valore aggiunto (IVA) alla fattura:

- Sommare **la colonna** Tax dal file basato su licenza.
- Sommare **la colonna TaxAmount** dal file basato sull'utilizzo.

## <a name="itemize-reconciliation-files-by-partner"></a>Visualizzare in modo specifico i file di riconciliazione in base al partner

I partner nel modello **indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenza e basati sull'utilizzo per visualizzare in dettaglio i file in base al rivenditore.

| ID MPN | Descrizione |
| ------ | ----------- |
| ID MPN | Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto). |
| [ID MPN rivenditore](#reseller-mpn-id) | Identificatore [MPN del rivenditore di record per la sottoscrizione](#reseller-mpn-id). Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica in Partner Center. Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto. |

### <a name="reseller-mpn-id"></a>ID MPN rivenditore

Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo **ID MPN** viene elencato due volte come **ID MPN** e ID **MPN rivenditore**.

Se un partner CSP ha un rivenditore senza **ID MPN,** questo valore viene impostato sull'ID **MPN del** partner.

Se il partner CSP rimuove un **ID MPN rivenditore,** questo valore verrà impostato su *-1.*

Per visualizzare o aggiornare **l'ID MPN del rivenditore:**

1. Accedere al Centro per i partner.
2. Nel menu del Centro per i partner scegli **Clienti**.
3. Scegliere il cliente dall'elenco.
4. Nel menu del cliente selezionare **Sottoscrizioni.**
5. Scegliere la sottoscrizione dall'elenco.
6. Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.

## <a name="next-steps"></a>Passaggi successivi

- [Come leggere il file di & fattura](read-your-bill.md) 