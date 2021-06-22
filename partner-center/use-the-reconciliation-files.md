---
title: Usare i file di riconciliazione
ms.topic: article
ms.date: 03/26/2021
description: Informazioni sui file di riconciliazione Partner Center e su come interpretare le visualizzazioni dettagliate degli addebiti per voci per un determinato ciclo di fatturazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431563"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="966de-103">Informazioni su come leggere le voci nei file di Partner Center di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="966de-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="966de-104">**Ruoli appropriati:** Amministratore fatturazione | Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="966de-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="966de-105">È possibile scaricare i file di riconciliazione Partner Center per una visualizzazione dettagliata delle voci di ogni addebito in un ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="966de-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="966de-106">I dettagli delle voci includono gli addebiti per le sottoscrizioni di ogni cliente e gli eventi dettagliati, ad esempio l'aggiunta di licenze a medio termine a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="966de-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="966de-107">Per informazioni su come leggere la **fattura,** vedere [Leggere la fattura.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="966de-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="966de-108">Comprendere i campi del file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="966de-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="966de-109">Campi del file di riconciliazione basato su licenza</span><span class="sxs-lookup"><span data-stu-id="966de-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="966de-110">Campi del file di riconciliazione basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="966de-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="966de-111">Campi del file di riconciliazione per l'uso quotidiano</span><span class="sxs-lookup"><span data-stu-id="966de-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="966de-112">Campi del file di riconciliazione CSP per l'acquisto una sola volta</span><span class="sxs-lookup"><span data-stu-id="966de-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="966de-113">Comprendere i tipi di addebito nei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="966de-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="966de-114">Per comprendere i tipi di addebiti nei file di riconciliazione (colonna **ChargeType),** vedere [Tipi di addebiti per i file di riconciliazione.](recon-file-charge-types.md)</span><span class="sxs-lookup"><span data-stu-id="966de-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="966de-115">Risolvere i problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="966de-115">Fix formatting issues</span></span>

<span data-ttu-id="966de-116">In alcuni casi, un file di riconciliazione potrebbe contenere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="966de-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="966de-117">Ad esempio, questo problema può verificarsi se non vengono usate le impostazioni locali en-US.</span><span class="sxs-lookup"><span data-stu-id="966de-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="966de-118">Per risolvere eventuali problemi di formattazione nei file di riconciliazione, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="966de-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="966de-119">Aprire il file di riconciliazione (in .csv) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="966de-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="966de-120">Selezionare la prima colonna nel file.</span><span class="sxs-lookup"><span data-stu-id="966de-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="966de-121">Aprire la **Conversione guidata testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="966de-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="966de-122">Sulla barra multifunzione selezionare **Dati** e quindi selezionare **Da testo a colonne.**</span><span class="sxs-lookup"><span data-stu-id="966de-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="966de-123">Nella procedura guidata selezionare **Tipo di file delimitato**.</span><span class="sxs-lookup"><span data-stu-id="966de-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="966de-124">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="966de-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="966de-125">Nel campo **Delimitatori** selezionare **Virgola.**</span><span class="sxs-lookup"><span data-stu-id="966de-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="966de-126">Se **l'opzione Scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Selezionare quindi **Avanti.**</span><span class="sxs-lookup"><span data-stu-id="966de-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="966de-127">Nel campo **Formato dati colonna** selezionare **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="966de-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="966de-128">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="966de-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="966de-129">Nel campo **Formato dati colonna** selezionare Testo per tutte le colonne quantità. </span><span class="sxs-lookup"><span data-stu-id="966de-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="966de-130">quindi fare clic su **Fine**.</span><span class="sxs-lookup"><span data-stu-id="966de-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="966de-131">Scaricare i file di riconciliazione a livello di codice</span><span class="sxs-lookup"><span data-stu-id="966de-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="966de-132">I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="966de-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="966de-133">Per scaricare i file di riconciliazione a livello di codice, vedere [Ottenere le voci della fattura.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="966de-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="966de-134">Se il file supera il limite di righe in Excel</span><span class="sxs-lookup"><span data-stu-id="966de-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="966de-135">Se è possibile scaricare un file di riconciliazione ma non aprirlo in Microsoft Excel, è probabile che il file contenga più righe di quelle consentite da Excel.</span><span class="sxs-lookup"><span data-stu-id="966de-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="966de-136">In questo caso, è possibile usare una delle procedure seguenti per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="966de-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="966de-137">Aprire un file di ricognizione in Power BI</span><span class="sxs-lookup"><span data-stu-id="966de-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="966de-138">Scaricare il file di riconciliazione come di consueto.</span><span class="sxs-lookup"><span data-stu-id="966de-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="966de-139">Scaricare, installare e aprire un'istanza di Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="966de-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="966de-140">Nella scheda Power BI **Home** selezionare **Ottieni dati.**</span><span class="sxs-lookup"><span data-stu-id="966de-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="966de-141">Nell'elenco Origini **dati comuni** selezionare **Testo/CSV.**</span><span class="sxs-lookup"><span data-stu-id="966de-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="966de-142">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="966de-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="966de-143">Aprire un file di ricognizione in una tabella pivot di Excel</span><span class="sxs-lookup"><span data-stu-id="966de-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="966de-144">Scaricare il file di riconciliazione come di consueto.</span><span class="sxs-lookup"><span data-stu-id="966de-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="966de-145">Aprire un nuovo file in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="966de-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="966de-146">Nella scheda **Dati** **selezionare Ottieni** dati, selezionare Da **file** e quindi selezionare **Testo/CSV.**</span><span class="sxs-lookup"><span data-stu-id="966de-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="966de-147">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="966de-147">When prompted, open your recon file.</span></span> <span data-ttu-id="966de-148">Verranno visualizzati i dati.</span><span class="sxs-lookup"><span data-stu-id="966de-148">Your data will appear.</span></span>
5. <span data-ttu-id="966de-149">Nel menu **a** discesa Carica selezionare **Carica in** e quindi selezionare **OK.**</span><span class="sxs-lookup"><span data-stu-id="966de-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="966de-150">Nella finestra **di dialogo Importa** dati selezionare Rapporto di tabella **pivot** per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="966de-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="966de-151">Importo negativo visualizzato</span><span class="sxs-lookup"><span data-stu-id="966de-151">Negative amount displayed</span></span>

<span data-ttu-id="966de-152">È possibile che venga visualizzato un importo negativo nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="966de-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="966de-153">Questo problema è probabilmente dovuto a una delle cause seguenti:</span><span class="sxs-lookup"><span data-stu-id="966de-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="966de-154">Il numero di licenze è stato annullato o ridotto di recente</span><span class="sxs-lookup"><span data-stu-id="966de-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="966de-155">Si è ricevuto il credito per un contratto di licenza del servizio o per l'utilizzo di Azure</span><span class="sxs-lookup"><span data-stu-id="966de-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="966de-156">Per ottenere altre informazioni su questa transazione, verificare il rispettivo attributo relativo al tipo di addebito nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="966de-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="966de-157">Mappare le imposte o l'IVA</span><span class="sxs-lookup"><span data-stu-id="966de-157">Map taxes or VAT</span></span>

<span data-ttu-id="966de-158">Per eseguire il mapping delle imposte o delle imposte sul valore aggiunto (IVA) alla fattura:</span><span class="sxs-lookup"><span data-stu-id="966de-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="966de-159">Sommare **la colonna** Tax dal file basato su licenza.</span><span class="sxs-lookup"><span data-stu-id="966de-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="966de-160">Sommare **la colonna TaxAmount** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="966de-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="966de-161">Visualizzare i file di riconciliazione in base al partner</span><span class="sxs-lookup"><span data-stu-id="966de-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="966de-162">I partner nel **modello indiretto possono** usare questi campi aggiuntivi sia nei file di riconciliazione basati su licenza che in base all'utilizzo per specificare i file in base al rivenditore.</span><span class="sxs-lookup"><span data-stu-id="966de-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="966de-163">ID MPN</span><span class="sxs-lookup"><span data-stu-id="966de-163">MPN ID</span></span> | <span data-ttu-id="966de-164">Descrizione</span><span class="sxs-lookup"><span data-stu-id="966de-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="966de-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="966de-165">MPN ID</span></span> | <span data-ttu-id="966de-166">Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="966de-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="966de-167">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="966de-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="966de-168">Identificatore [MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="966de-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="966de-169">Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="966de-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="966de-170">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="966de-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="966de-171">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="966de-171">Reseller MPN ID</span></span>

<span data-ttu-id="966de-172">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo **ID MPN** viene elencato due volte, sia come **ID MPN** che come **ID MPN rivenditore.**</span><span class="sxs-lookup"><span data-stu-id="966de-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="966de-173">Se un partner CSP ha un rivenditore senza **ID MPN,** questo valore viene impostato sull'ID **MPN del** partner.</span><span class="sxs-lookup"><span data-stu-id="966de-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="966de-174">Se il partner CSP rimuove un **ID MPN rivenditore,** questo valore verrà impostato su *-1.*</span><span class="sxs-lookup"><span data-stu-id="966de-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="966de-175">Per visualizzare o aggiornare **l'ID MPN del rivenditore:**</span><span class="sxs-lookup"><span data-stu-id="966de-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="966de-176">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="966de-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="966de-177">Nel menu del Centro per i partner scegli **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="966de-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="966de-178">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="966de-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="966de-179">Nel menu del cliente selezionare **Sottoscrizioni.**</span><span class="sxs-lookup"><span data-stu-id="966de-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="966de-180">Scegliere la sottoscrizione dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="966de-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="966de-181">Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.</span><span class="sxs-lookup"><span data-stu-id="966de-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="966de-182">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="966de-182">Next steps</span></span>

- [<span data-ttu-id="966de-183">Come leggere il file di ricognizione & fattura</span><span class="sxs-lookup"><span data-stu-id="966de-183">How to read your bill & recon file</span></span>](read-your-bill.md) 