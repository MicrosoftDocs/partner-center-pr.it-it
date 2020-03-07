---
title: Usare i file di riconciliazione | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
description: Usare i file di riconciliazione per ottenere informazioni dettagliate sulle visualizzazioni di elementi lineari degli addebiti per i centri partner.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340219"
---
# <a name="use-your-reconciliation-files"></a><span data-ttu-id="f9cfc-103">Usare i file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-103">Use your reconciliation files</span></span>

<span data-ttu-id="f9cfc-104">Si applica a:</span><span class="sxs-lookup"><span data-stu-id="f9cfc-104">Applies to:</span></span>

- <span data-ttu-id="f9cfc-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="f9cfc-105">Partner Center</span></span>
- <span data-ttu-id="f9cfc-106">Centro per i partner per Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f9cfc-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f9cfc-107">È possibile scaricare i file di riconciliazione dal centro per i partner per una visualizzazione dettagliata di ogni addebito in un ciclo di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="f9cfc-108">I dettagli dell'elemento di riga includono gli addebiti per le sottoscrizioni di ogni cliente ed eventi dettagliati, ad esempio l'aggiunta a metà del periodo di postazioni a una sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="f9cfc-109">Ruoli appropriati:</span><span class="sxs-lookup"><span data-stu-id="f9cfc-109">Appropriate roles:</span></span>

- <span data-ttu-id="f9cfc-110">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-110">Billing admin</span></span>
- <span data-ttu-id="f9cfc-111">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="f9cfc-111">Global admin</span></span>

<span data-ttu-id="f9cfc-112">Per informazioni su come leggere la **fattura**, vedere [leggere la fattura](read-your-bill.md).</span><span class="sxs-lookup"><span data-stu-id="f9cfc-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="f9cfc-113">Informazioni sui campi del file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="f9cfc-114">Campi del file di riconciliazione basato su licenza</span><span class="sxs-lookup"><span data-stu-id="f9cfc-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="f9cfc-115">Campi del file di riconciliazione basata sull'utilizzo</span><span class="sxs-lookup"><span data-stu-id="f9cfc-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="f9cfc-116">Campi di un file di riconciliazione monouso e ricorrente</span><span class="sxs-lookup"><span data-stu-id="f9cfc-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="f9cfc-117">Campi del file di riconciliazione dell'utilizzo con classificazione giornaliera</span><span class="sxs-lookup"><span data-stu-id="f9cfc-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="f9cfc-118">Informazioni sui tipi di addebito nei file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="f9cfc-119">Per informazioni sui tipi di addebiti nei file di riconciliazione (colonna **ChargeType** ), vedere [tipi di addebiti per i file di riconciliazione](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="f9cfc-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="f9cfc-120">Correzione dei problemi di formattazione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-120">Fix formatting issues</span></span>

<span data-ttu-id="f9cfc-121">Occasionalmente, un file di riconciliazione potrebbe contenere problemi di formattazione.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="f9cfc-122">Ad esempio, questo problema può verificarsi se le impostazioni locali en-US non vengono usate.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="f9cfc-123">Per correggere eventuali problemi di formattazione nei file di riconciliazione, attenersi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="f9cfc-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="f9cfc-124">Aprire il file di riconciliazione (in formato CSV) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="f9cfc-125">Consente di selezionare la prima colonna del file.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="f9cfc-126">Aprire la **procedura guidata Converti testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="f9cfc-127">Sulla barra multifunzione selezionare **dati**, quindi selezionare **testo in colonne**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="f9cfc-128">Nella procedura guidata selezionare **tipo di file delimitato**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="f9cfc-129">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="f9cfc-130">Nel campo **delimitatori** selezionare **virgola**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="f9cfc-131">Se la **scheda** è già selezionata, è possibile lasciare selezionata questa opzione. Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="f9cfc-132">Nel campo **formato dati colonna** selezionare **Data: MDY**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="f9cfc-133">Quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="f9cfc-134">Nel campo **formato dati colonna** selezionare **testo** per tutte le colonne Amount.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="f9cfc-135">Selezionare quindi **fine**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="f9cfc-136">Scarica i file di riconciliazione a livello di codice</span><span class="sxs-lookup"><span data-stu-id="f9cfc-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="f9cfc-137">I file di riconciliazione possono essere molto grandi e talvolta difficili da scaricare.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="f9cfc-138">Per scaricare i file di riconciliazione a livello di codice, vedere [ottenere le voci di riga della fattura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="f9cfc-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="f9cfc-139">Tasse per la mappa o IVA</span><span class="sxs-lookup"><span data-stu-id="f9cfc-139">Map taxes or VAT</span></span>

<span data-ttu-id="f9cfc-140">Per mappare le imposte o le imposte a valore aggiunto (IVA) alla fattura:</span><span class="sxs-lookup"><span data-stu-id="f9cfc-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="f9cfc-141">Sommare la colonna **Tax** dal file basato sulle licenze.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="f9cfc-142">Sommare la colonna **TaxAmount** dal file basato sull'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="f9cfc-143">Descrivere i file di riconciliazione per partner</span><span class="sxs-lookup"><span data-stu-id="f9cfc-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="f9cfc-144">I partner del **modello indiretto** possono usare questi campi aggiuntivi nei file di riconciliazione basati su licenze e utilizzo per descrivere i file in base al rivenditore.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="f9cfc-145">ID MPN</span><span class="sxs-lookup"><span data-stu-id="f9cfc-145">MPN ID</span></span> | <span data-ttu-id="f9cfc-146">Descrizione</span><span class="sxs-lookup"><span data-stu-id="f9cfc-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="f9cfc-147">ID MPN</span><span class="sxs-lookup"><span data-stu-id="f9cfc-147">MPN ID</span></span> | <span data-ttu-id="f9cfc-148">Identificatore Microsoft Partner Network (MPN) del partner Cloud Solution Provider (CSP) (diretto o indiretto).</span><span class="sxs-lookup"><span data-stu-id="f9cfc-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="f9cfc-149">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="f9cfc-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="f9cfc-150">[Identificatore MPN del rivenditore del record per la sottoscrizione](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="f9cfc-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="f9cfc-151">Questo campo corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="f9cfc-152">Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="f9cfc-153">ID MPN rivenditore</span><span class="sxs-lookup"><span data-stu-id="f9cfc-153">Reseller MPN ID</span></span>

<span data-ttu-id="f9cfc-154">Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, l' **ID MPN** viene elencato due volte, sia come **ID MPN** sia come **ID MPN rivenditore**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="f9cfc-155">Se un partner CSP ha un rivenditore senza **ID MPN**, questo valore viene impostato invece sull' **ID MPN** del partner.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="f9cfc-156">Se il partner CSP rimuove un **ID MPN rivenditore**, questo valore viene impostato su *-1*.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="f9cfc-157">Per visualizzare o aggiornare l' **ID MPN del rivenditore**:</span><span class="sxs-lookup"><span data-stu-id="f9cfc-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="f9cfc-158">Accedi al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f9cfc-159">Nel menu del Centro per i partner scegli **Clienti**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="f9cfc-160">Scegli il cliente nell'elenco.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="f9cfc-161">Nel menu cliente selezionare **sottoscrizioni**.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="f9cfc-162">Scegliere la sottoscrizione dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="f9cfc-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="f9cfc-163">Seleziona **Aggiorna** per modificare il valore **Rivenditore (ID MPN)** .</span><span class="sxs-lookup"><span data-stu-id="f9cfc-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
