---
title: Usare i file di riconciliazione
ms.topic: article
ms.date: 06/08/2020
description: Informazioni sui file di riconciliazione nel centro per i partner e su come interpretare le visualizzazioni dettagliate degli articoli di linea degli addebiti per un determinato ciclo di fatturazione.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a53a0f3d37183c67d5d1d44472192ed15f6ed62e
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/09/2020
ms.locfileid: "84603800"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="86df1-103">Informazioni su come leggere le voci nei file di riconciliazione del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="86df1-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="86df1-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="86df1-104">Applies to:</span></span>

- <span data-ttu-id="86df1-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="86df1-105">Partner Center</span></span>
- <span data-ttu-id="86df1-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="86df1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="86df1-107">È possibile scaricare i file di riconciliazione dal centro per i partner per una visualizzazione dettagliata di ogni addebito in un ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="86df1-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="86df1-108">I dettagli dell'elemento di riga includono gli addebiti per le sottoscrizioni di ogni cliente ed eventi dettagliati, ad esempio l'aggiunta a metà del periodo di postazioni a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="86df1-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="86df1-109">Ruoli appropriati:</span><span class="sxs-lookup"><span data-stu-id="86df1-109">Appropriate roles:</span></span>

- <span data-ttu-id="86df1-110">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="86df1-110">Billing admin</span></span>
- <span data-ttu-id="86df1-111">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="86df1-111">Global admin</span></span>

<span data-ttu-id="86df1-112">Per informazioni su come leggere la **fattura**, vedere [leggere la fattura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="86df1-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="86df1-113">Informazioni sui campi del file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="86df1-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="86df1-114">Campi del file di riconciliazione basato su licenza</span><span class="sxs-lookup"><span data-stu-id="86df1-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="86df1-115">Campi del file di riconciliazione basata sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="86df1-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="86df1-116">Campi di un file di riconciliazione monouso e ricorrente</span><span class="sxs-lookup"><span data-stu-id="86df1-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="86df1-117">Campi del file di riconciliazione dell'utilizzo con classificazione giornaliera</span><span class="sxs-lookup"><span data-stu-id="86df1-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="86df1-118">Informazioni sui tipi di addebito nei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="86df1-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="86df1-119">Per informazioni sui tipi di addebiti nei file di riconciliazione (colonna **ChargeType** ), vedere [tipi di addebiti per i file di riconciliazione](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="86df1-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="86df1-120">Correzione dei problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="86df1-120">Fix formatting issues</span></span>

<span data-ttu-id="86df1-121">Occasionalmente, un file di riconciliazione potrebbe contenere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="86df1-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="86df1-122">Ad esempio, questo problema può verificarsi se le impostazioni locali en-US non vengono usate.</span><span class="sxs-lookup"><span data-stu-id="86df1-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="86df1-123">Per correggere eventuali problemi di formattazione nei file di riconciliazione, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="86df1-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="86df1-124">Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="86df1-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="86df1-125">Consente di selezionare la prima colonna del file.</span><span class="sxs-lookup"><span data-stu-id="86df1-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="86df1-126">Aprire la **procedura guidata Converti testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="86df1-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="86df1-127">Sulla barra multifunzione selezionare **dati**, quindi selezionare **testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="86df1-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="86df1-128">Nella procedura guidata selezionare **tipo di file delimitato**.</span><span class="sxs-lookup"><span data-stu-id="86df1-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="86df1-129">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="86df1-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="86df1-130">Nel campo **delimitatori** selezionare **virgola**.</span><span class="sxs-lookup"><span data-stu-id="86df1-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="86df1-131">Se la **scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="86df1-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="86df1-132">Nel campo **formato dati colonna** selezionare **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="86df1-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="86df1-133">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="86df1-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="86df1-134">Nel campo **formato dati colonna** selezionare **testo** per tutte le colonne Amount.</span><span class="sxs-lookup"><span data-stu-id="86df1-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="86df1-135">Quindi selezionare **Fine**.</span><span class="sxs-lookup"><span data-stu-id="86df1-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="86df1-136">Scarica i file di riconciliazione a livello di codice</span><span class="sxs-lookup"><span data-stu-id="86df1-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="86df1-137">I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="86df1-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="86df1-138">Per scaricare i file di riconciliazione a livello di codice, vedere [ottenere le voci di riga della fattura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="86df1-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="86df1-139">Tasse per la mappa o IVA</span><span class="sxs-lookup"><span data-stu-id="86df1-139">Map taxes or VAT</span></span>

<span data-ttu-id="86df1-140">Per mappare le imposte o le imposte a valore aggiunto (IVA) alla fattura:</span><span class="sxs-lookup"><span data-stu-id="86df1-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="86df1-141">Sommare la colonna **Tax** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="86df1-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="86df1-142">Sommare la colonna **TaxAmount** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="86df1-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="86df1-143">Descrivere i file di riconciliazione per partner</span><span class="sxs-lookup"><span data-stu-id="86df1-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="86df1-144">I partner del **modello indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenze e utilizzo per descrivere i file in base al rivenditore.</span><span class="sxs-lookup"><span data-stu-id="86df1-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="86df1-145">ID MPN</span><span class="sxs-lookup"><span data-stu-id="86df1-145">MPN ID</span></span> | <span data-ttu-id="86df1-146">Descrizione</span><span class="sxs-lookup"><span data-stu-id="86df1-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="86df1-147">ID MPN</span><span class="sxs-lookup"><span data-stu-id="86df1-147">MPN ID</span></span> | <span data-ttu-id="86df1-148">Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="86df1-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="86df1-149">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="86df1-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="86df1-150">[Identificatore MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="86df1-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="86df1-151">Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="86df1-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="86df1-152">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="86df1-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="86df1-153">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="86df1-153">Reseller MPN ID</span></span>

<span data-ttu-id="86df1-154">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, l' **ID MPN** viene elencato due volte, sia come **ID MPN** sia come **ID MPN rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="86df1-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="86df1-155">Se un partner CSP ha un rivenditore senza **ID MPN**, questo valore viene impostato invece sull' **ID MPN** del partner.</span><span class="sxs-lookup"><span data-stu-id="86df1-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="86df1-156">Se il partner CSP rimuove un **ID MPN rivenditore**, questo valore viene impostato su *-1*.</span><span class="sxs-lookup"><span data-stu-id="86df1-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="86df1-157">Per visualizzare o aggiornare l' **ID MPN del rivenditore**:</span><span class="sxs-lookup"><span data-stu-id="86df1-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="86df1-158">Accedere al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="86df1-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="86df1-159">Nel menu del Centro per i partner scegli **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="86df1-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="86df1-160">Scegliere il cliente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="86df1-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="86df1-161">Nel menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="86df1-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="86df1-162">Scegliere la sottoscrizione dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="86df1-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="86df1-163">Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)**.</span><span class="sxs-lookup"><span data-stu-id="86df1-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
