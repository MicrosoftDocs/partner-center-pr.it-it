---
title: Usare i file di riconciliazione
ms.topic: article
ms.date: 03/26/2021
description: Informazioni sui file di riconciliazione nel centro per i partner e su come interpretare le visualizzazioni dettagliate degli articoli di linea degli addebiti per un determinato ciclo di fatturazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633897"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="c1cab-103">Informazioni su come leggere le voci nei file di riconciliazione del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="c1cab-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="c1cab-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="c1cab-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c1cab-105">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="c1cab-105">Billing admin</span></span>
- <span data-ttu-id="c1cab-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c1cab-106">Global admin</span></span>

<span data-ttu-id="c1cab-107">È possibile scaricare i file di riconciliazione dal centro per i partner per una visualizzazione dettagliata di ogni addebito in un ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="c1cab-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="c1cab-108">I dettagli dell'elemento di riga includono gli addebiti per le sottoscrizioni di ogni cliente ed eventi dettagliati, ad esempio l'aggiunta a metà del periodo di licenze a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c1cab-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="c1cab-109">Per informazioni su come leggere la **fattura**, vedere [leggere la fattura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="c1cab-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="c1cab-110">Informazioni sui campi del file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="c1cab-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="c1cab-111">Campi del file di riconciliazione basato su licenza</span><span class="sxs-lookup"><span data-stu-id="c1cab-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="c1cab-112">Campi del file di riconciliazione basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="c1cab-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="c1cab-113">Campi del file di riconciliazione per l'uso quotidiano</span><span class="sxs-lookup"><span data-stu-id="c1cab-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="c1cab-114">Campi del file di riconciliazione del CSP di acquisto monouso</span><span class="sxs-lookup"><span data-stu-id="c1cab-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="c1cab-115">Informazioni sui tipi di addebito nei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="c1cab-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="c1cab-116">Per informazioni sui tipi di addebiti nei file di riconciliazione (colonna **ChargeType** ), vedere [tipi di addebiti per i file di riconciliazione](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="c1cab-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="c1cab-117">Correzione dei problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="c1cab-117">Fix formatting issues</span></span>

<span data-ttu-id="c1cab-118">Occasionalmente, un file di riconciliazione potrebbe contenere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="c1cab-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="c1cab-119">Ad esempio, questo problema può verificarsi se le impostazioni locali en-US non vengono usate.</span><span class="sxs-lookup"><span data-stu-id="c1cab-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="c1cab-120">Per correggere eventuali problemi di formattazione nei file di riconciliazione, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="c1cab-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="c1cab-121">Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="c1cab-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="c1cab-122">Consente di selezionare la prima colonna del file.</span><span class="sxs-lookup"><span data-stu-id="c1cab-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="c1cab-123">Aprire la **procedura guidata Converti testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="c1cab-124">Sulla barra multifunzione selezionare **dati**, quindi selezionare **testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="c1cab-125">Nella procedura guidata selezionare **tipo di file delimitato**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="c1cab-126">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="c1cab-127">Nel campo **delimitatori** selezionare **virgola**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="c1cab-128">Se la **scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="c1cab-129">Nel campo **formato dati colonna** selezionare **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="c1cab-130">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="c1cab-131">Nel campo **formato dati colonna** selezionare **testo** per tutte le colonne Amount.</span><span class="sxs-lookup"><span data-stu-id="c1cab-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="c1cab-132">quindi fare clic su **Fine**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="c1cab-133">Scarica i file di riconciliazione a livello di codice</span><span class="sxs-lookup"><span data-stu-id="c1cab-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="c1cab-134">I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="c1cab-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="c1cab-135">Per scaricare i file di riconciliazione a livello di codice, vedere [ottenere le voci di riga della fattura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="c1cab-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="c1cab-136">Se il file supera il limite di righe in Excel</span><span class="sxs-lookup"><span data-stu-id="c1cab-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="c1cab-137">Se si è in grado di scaricare un file di riconciliazione ma non di aprirlo in Microsoft Excel, significa probabilmente che il file contiene più righe di quelle consentite da Excel.</span><span class="sxs-lookup"><span data-stu-id="c1cab-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="c1cab-138">In tal caso, è possibile utilizzare una delle procedure riportate di seguito per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="c1cab-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="c1cab-139">Aprire un file di ricognizione in Power BI</span><span class="sxs-lookup"><span data-stu-id="c1cab-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="c1cab-140">Scaricare il file di riconciliazione normalmente.</span><span class="sxs-lookup"><span data-stu-id="c1cab-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c1cab-141">Scaricare, installare e aprire un'istanza di Power BI.</span><span class="sxs-lookup"><span data-stu-id="c1cab-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="c1cab-142">Nella scheda **Home** Power bi selezionare **recuperare i dati**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="c1cab-143">Nell'elenco delle **origini dati comuni** selezionare **testo/CSV**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="c1cab-144">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="c1cab-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="c1cab-145">Aprire un file di ricognizione in una tabella pivot di Excel</span><span class="sxs-lookup"><span data-stu-id="c1cab-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="c1cab-146">Scaricare il file di riconciliazione normalmente.</span><span class="sxs-lookup"><span data-stu-id="c1cab-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c1cab-147">Aprire un nuovo file in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="c1cab-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="c1cab-148">Nella scheda **dati** selezionare **Ottieni dati**, selezionare **da file**, quindi selezionare **testo/CSV**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="c1cab-149">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="c1cab-149">When prompted, open your recon file.</span></span> <span data-ttu-id="c1cab-150">Verranno visualizzati i dati.</span><span class="sxs-lookup"><span data-stu-id="c1cab-150">Your data will appear.</span></span>
5. <span data-ttu-id="c1cab-151">Nel menu a discesa **carica** selezionare **carica in** e quindi **OK**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="c1cab-152">Nella finestra di dialogo **Importa dati** selezionare **rapporto di tabella pivot** per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="c1cab-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="c1cab-153">Tasse per la mappa o IVA</span><span class="sxs-lookup"><span data-stu-id="c1cab-153">Map taxes or VAT</span></span>

<span data-ttu-id="c1cab-154">Per mappare le imposte o le imposte a valore aggiunto (IVA) alla fattura:</span><span class="sxs-lookup"><span data-stu-id="c1cab-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="c1cab-155">Sommare la colonna **Tax** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="c1cab-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="c1cab-156">Sommare la colonna **TaxAmount** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="c1cab-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="c1cab-157">Descrivere i file di riconciliazione per partner</span><span class="sxs-lookup"><span data-stu-id="c1cab-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="c1cab-158">I partner del **modello indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenze e utilizzo per descrivere i file in base al rivenditore.</span><span class="sxs-lookup"><span data-stu-id="c1cab-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="c1cab-159">ID MPN</span><span class="sxs-lookup"><span data-stu-id="c1cab-159">MPN ID</span></span> | <span data-ttu-id="c1cab-160">Descrizione</span><span class="sxs-lookup"><span data-stu-id="c1cab-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="c1cab-161">ID MPN</span><span class="sxs-lookup"><span data-stu-id="c1cab-161">MPN ID</span></span> | <span data-ttu-id="c1cab-162">Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="c1cab-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="c1cab-163">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="c1cab-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="c1cab-164">[Identificatore MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="c1cab-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="c1cab-165">Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1cab-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="c1cab-166">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="c1cab-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="c1cab-167">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="c1cab-167">Reseller MPN ID</span></span>

<span data-ttu-id="c1cab-168">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, l' **ID MPN** viene elencato due volte, sia come **ID MPN** sia come **ID MPN rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="c1cab-169">Se un partner CSP ha un rivenditore senza **ID MPN**, questo valore viene impostato invece sull' **ID MPN** del partner.</span><span class="sxs-lookup"><span data-stu-id="c1cab-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="c1cab-170">Se il partner CSP rimuove un **ID MPN rivenditore**, questo valore viene impostato su *-1*.</span><span class="sxs-lookup"><span data-stu-id="c1cab-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="c1cab-171">Per visualizzare o aggiornare l' **ID MPN del rivenditore**:</span><span class="sxs-lookup"><span data-stu-id="c1cab-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="c1cab-172">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c1cab-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="c1cab-173">Nel menu del Centro per i partner scegli **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="c1cab-174">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c1cab-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="c1cab-175">Nel menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="c1cab-176">Scegliere la sottoscrizione dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c1cab-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="c1cab-177">Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.</span><span class="sxs-lookup"><span data-stu-id="c1cab-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c1cab-178">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c1cab-178">Next steps</span></span>

- [<span data-ttu-id="c1cab-179">Come leggere il file di fatturazione & Recon</span><span class="sxs-lookup"><span data-stu-id="c1cab-179">How to read your bill & recon file</span></span>](read-your-bill.md) 