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
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730084"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="c3ca4-103">Informazioni su come leggere le voci nei file di riconciliazione del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="c3ca4-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="c3ca4-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="c3ca4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c3ca4-105">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="c3ca4-105">Billing admin</span></span>
- <span data-ttu-id="c3ca4-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="c3ca4-106">Global admin</span></span>

<span data-ttu-id="c3ca4-107">È possibile scaricare i file di riconciliazione dal centro per i partner per una visualizzazione dettagliata di ogni addebito in un ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="c3ca4-108">I dettagli dell'elemento di riga includono gli addebiti per le sottoscrizioni di ogni cliente ed eventi dettagliati, ad esempio l'aggiunta a metà del periodo di licenze a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="c3ca4-109">Per informazioni su come leggere la **fattura**, vedere [leggere la fattura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="c3ca4-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="c3ca4-110">Informazioni sui campi del file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="c3ca4-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="c3ca4-111">Campi del file di riconciliazione basato su licenza</span><span class="sxs-lookup"><span data-stu-id="c3ca4-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="c3ca4-112">Campi del file di riconciliazione basato sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="c3ca4-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="c3ca4-113">Campi del file di riconciliazione per l'uso quotidiano</span><span class="sxs-lookup"><span data-stu-id="c3ca4-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="c3ca4-114">Campi del file di riconciliazione del CSP di acquisto monouso</span><span class="sxs-lookup"><span data-stu-id="c3ca4-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="c3ca4-115">Informazioni sui tipi di addebito nei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="c3ca4-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="c3ca4-116">Per informazioni sui tipi di addebiti nei file di riconciliazione (colonna **ChargeType** ), vedere [tipi di addebiti per i file di riconciliazione](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="c3ca4-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="c3ca4-117">Correzione dei problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="c3ca4-117">Fix formatting issues</span></span>

<span data-ttu-id="c3ca4-118">Occasionalmente, un file di riconciliazione potrebbe contenere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="c3ca4-119">Ad esempio, questo problema può verificarsi se le impostazioni locali en-US non vengono usate.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="c3ca4-120">Per correggere eventuali problemi di formattazione nei file di riconciliazione, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="c3ca4-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="c3ca4-121">Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="c3ca4-122">Consente di selezionare la prima colonna del file.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="c3ca4-123">Aprire la **procedura guidata Converti testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="c3ca4-124">Sulla barra multifunzione selezionare **dati**, quindi selezionare **testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="c3ca4-125">Nella procedura guidata selezionare **tipo di file delimitato**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="c3ca4-126">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="c3ca4-127">Nel campo **delimitatori** selezionare **virgola**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="c3ca4-128">Se la **scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="c3ca4-129">Nel campo **formato dati colonna** selezionare **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="c3ca4-130">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="c3ca4-131">Nel campo **formato dati colonna** selezionare **testo** per tutte le colonne Amount.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="c3ca4-132">quindi fare clic su **Fine**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="c3ca4-133">Scarica i file di riconciliazione a livello di codice</span><span class="sxs-lookup"><span data-stu-id="c3ca4-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="c3ca4-134">I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="c3ca4-135">Per scaricare i file di riconciliazione a livello di codice, vedere [ottenere le voci di riga della fattura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="c3ca4-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="c3ca4-136">Se il file supera il limite di righe in Excel</span><span class="sxs-lookup"><span data-stu-id="c3ca4-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="c3ca4-137">Se si è in grado di scaricare un file di riconciliazione ma non di aprirlo in Microsoft Excel, significa probabilmente che il file contiene più righe di quelle consentite da Excel.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="c3ca4-138">In tal caso, è possibile utilizzare una delle procedure riportate di seguito per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="c3ca4-139">Aprire un file di ricognizione in Power BI</span><span class="sxs-lookup"><span data-stu-id="c3ca4-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="c3ca4-140">Scaricare il file di riconciliazione normalmente.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c3ca4-141">Scaricare, installare e aprire un'istanza di Power BI.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="c3ca4-142">Nella scheda **Home** Power bi selezionare **recuperare i dati**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="c3ca4-143">Nell'elenco delle **origini dati comuni** selezionare **testo/CSV**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="c3ca4-144">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="c3ca4-145">Aprire un file di ricognizione in una tabella pivot di Excel</span><span class="sxs-lookup"><span data-stu-id="c3ca4-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="c3ca4-146">Scaricare il file di riconciliazione normalmente.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="c3ca4-147">Aprire un nuovo file in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="c3ca4-148">Nella scheda **dati** selezionare **Ottieni dati**, selezionare **da file**, quindi selezionare **testo/CSV**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="c3ca4-149">Quando richiesto, aprire il file di ricognizione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-149">When prompted, open your recon file.</span></span> <span data-ttu-id="c3ca4-150">Verranno visualizzati i dati.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-150">Your data will appear.</span></span>
5. <span data-ttu-id="c3ca4-151">Nel menu a discesa **carica** selezionare **carica in** e quindi **OK**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="c3ca4-152">Nella finestra di dialogo **Importa dati** selezionare **rapporto di tabella pivot** per aprire il file.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="c3ca4-153">Quantità negativa visualizzata</span><span class="sxs-lookup"><span data-stu-id="c3ca4-153">Negative amount displayed</span></span>

<span data-ttu-id="c3ca4-154">È possibile che venga visualizzato un valore negativo nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-154">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="c3ca4-155">Questa situazione è probabilmente causata da una delle operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c3ca4-155">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="c3ca4-156">Il numero di licenze è stato annullato o ridotto di recente</span><span class="sxs-lookup"><span data-stu-id="c3ca4-156">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="c3ca4-157">Il credito è stato ricevuto per un contratto di licenza con il servizio o per il consumo di Azure</span><span class="sxs-lookup"><span data-stu-id="c3ca4-157">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="c3ca4-158">Per ottenere ulteriori informazioni su questa transazione, esaminare l'attributo di tipo addebito nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-158">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="c3ca4-159">Tasse per la mappa o IVA</span><span class="sxs-lookup"><span data-stu-id="c3ca4-159">Map taxes or VAT</span></span>

<span data-ttu-id="c3ca4-160">Per mappare le imposte o le imposte a valore aggiunto (IVA) alla fattura:</span><span class="sxs-lookup"><span data-stu-id="c3ca4-160">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="c3ca4-161">Sommare la colonna **Tax** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-161">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="c3ca4-162">Sommare la colonna **TaxAmount** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-162">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="c3ca4-163">Descrivere i file di riconciliazione per partner</span><span class="sxs-lookup"><span data-stu-id="c3ca4-163">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="c3ca4-164">I partner del **modello indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenze e utilizzo per descrivere i file in base al rivenditore.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-164">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="c3ca4-165">ID MPN</span><span class="sxs-lookup"><span data-stu-id="c3ca4-165">MPN ID</span></span> | <span data-ttu-id="c3ca4-166">Descrizione</span><span class="sxs-lookup"><span data-stu-id="c3ca4-166">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="c3ca4-167">ID MPN</span><span class="sxs-lookup"><span data-stu-id="c3ca4-167">MPN ID</span></span> | <span data-ttu-id="c3ca4-168">Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="c3ca4-168">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="c3ca4-169">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="c3ca4-169">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="c3ca4-170">[Identificatore MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="c3ca4-170">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="c3ca4-171">Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-171">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="c3ca4-172">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-172">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="c3ca4-173">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="c3ca4-173">Reseller MPN ID</span></span>

<span data-ttu-id="c3ca4-174">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, l' **ID MPN** viene elencato due volte, sia come **ID MPN** sia come **ID MPN rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-174">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="c3ca4-175">Se un partner CSP ha un rivenditore senza **ID MPN**, questo valore viene impostato invece sull' **ID MPN** del partner.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-175">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="c3ca4-176">Se il partner CSP rimuove un **ID MPN rivenditore**, questo valore viene impostato su *-1*.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-176">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="c3ca4-177">Per visualizzare o aggiornare l' **ID MPN del rivenditore**:</span><span class="sxs-lookup"><span data-stu-id="c3ca4-177">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="c3ca4-178">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-178">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="c3ca4-179">Nel menu del Centro per i partner scegli **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-179">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="c3ca4-180">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-180">Choose the customer from the list.</span></span>
4. <span data-ttu-id="c3ca4-181">Nel menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-181">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="c3ca4-182">Scegliere la sottoscrizione dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-182">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="c3ca4-183">Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.</span><span class="sxs-lookup"><span data-stu-id="c3ca4-183">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c3ca4-184">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c3ca4-184">Next steps</span></span>

- [<span data-ttu-id="c3ca4-185">Come leggere il file di fatturazione & Recon</span><span class="sxs-lookup"><span data-stu-id="c3ca4-185">How to read your bill & recon file</span></span>](read-your-bill.md) 