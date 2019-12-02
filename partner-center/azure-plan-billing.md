---
title: Fatturazione del piano di Azure | Centro per i partner
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come accedere e ottieni informazioni sulla struttura dei file di fatturazione e di riconciliazione correlata alla fatturazione per il piano di Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: b52030f4956f8b3f86eec5aad72628dc64099729
ms.sourcegitcommit: f5dbf96c1dece9c766e9b4c1527e599872e2ab14
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/26/2019
ms.locfileid: "74536444"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="53712-103">Nuova esperienza commerciale in CSP - Fatturazione di Azure</span><span class="sxs-lookup"><span data-stu-id="53712-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="53712-104">**Ruoli appropriati:**</span><span class="sxs-lookup"><span data-stu-id="53712-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="53712-105">Amministratore fatturazione</span><span class="sxs-lookup"><span data-stu-id="53712-105">Billing admin</span></span>
- <span data-ttu-id="53712-106">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="53712-106">Admin agent</span></span>
- <span data-ttu-id="53712-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="53712-107">Global admin</span></span>


<span data-ttu-id="53712-108">La fatturazione in base al piano di Azure è un'esperienza semplificata che prevede l'uso di una singola data di fatturazione allineata e di un periodo di fatturazione basato sul mese di calendario.</span><span class="sxs-lookup"><span data-stu-id="53712-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="53712-109">Per informazioni sulla piattaforma di fatturazione, leggi [Panoramica della fatturazione](billing-basics.md).</span><span class="sxs-lookup"><span data-stu-id="53712-109">For information on the billing platform, read [Billing overview](billing-basics.md).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="53712-110">Riepilogo dei dati essenziali della fatturazione</span><span class="sxs-lookup"><span data-stu-id="53712-110">Summary of billing essentials</span></span>

- <span data-ttu-id="53712-111">**Data della fattura**: la fattura e il file di riconciliazione saranno disponibili nell'API o nel dashboard Centro per i partner entro il giorno 8 (mezzanotte UTC).</span><span class="sxs-lookup"><span data-stu-id="53712-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="53712-112">**Periodo di fatturazione**: il periodo di fatturazione è allineato al mese di calendario, ad esempio 01/10-31/10, 01/11-30/11.</span><span class="sxs-lookup"><span data-stu-id="53712-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="53712-113">**Addebiti per i periodi di servizio**: gli addebiti sono allineati al mese di calendario.</span><span class="sxs-lookup"><span data-stu-id="53712-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="53712-114">Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10.</span><span class="sxs-lookup"><span data-stu-id="53712-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="53712-115">La fattura del mese successivo che verrà generata il giorno 08/12 conterrà tutti gli addebiti per il periodo di servizio 01/11-31/11.</span><span class="sxs-lookup"><span data-stu-id="53712-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="53712-116">**Termine di pagamento della fattura**: netto a 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="53712-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="53712-117">**Valuta della fattura**: i partner continueranno a ricevere la fattura nella valuta assegnata del paese del cliente.</span><span class="sxs-lookup"><span data-stu-id="53712-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="53712-118">Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.</span><span class="sxs-lookup"><span data-stu-id="53712-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="53712-119">**Incentivi per i partner**: pagamento a 45 giorni dalla fine del mese della fattura.</span><span class="sxs-lookup"><span data-stu-id="53712-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="53712-120">Accedere alle fatture e ai file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="53712-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="53712-121">L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="53712-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="53712-122">**Per accedere alla fattura e al file di riconciliazione**</span><span class="sxs-lookup"><span data-stu-id="53712-122">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="53712-123">Accedi al [dashboard](https://partner.microsoft.com/en-us/dashboard/) Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="53712-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="53712-124">Dal menu del Centro per i partner seleziona **Fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="53712-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="53712-125">Seleziona la scheda per **Ricorrente** e **Occasionale** e la valuta di tuo interesse.</span><span class="sxs-lookup"><span data-stu-id="53712-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![fatturazione](images/azure/billing1.png)

4. <span data-ttu-id="53712-127">Seleziona **Fattura** o il file **Reconciliation** (Riconciliazione).</span><span class="sxs-lookup"><span data-stu-id="53712-127">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="53712-128">Per visualizzare i dati della cronologia relativa alle fatture e ai file di riconciliazione, espandi la riga della cronologia di fatturazione sottostante.</span><span class="sxs-lookup"><span data-stu-id="53712-128">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="53712-129">Informazioni sui dati di utilizzo</span><span class="sxs-lookup"><span data-stu-id="53712-129">Understanding usage data</span></span> 

1. <span data-ttu-id="53712-130">Il piano di Azure è il contenitore radice o di primo livello per l'utilizzo.</span><span class="sxs-lookup"><span data-stu-id="53712-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="53712-131">Tutti gli utilizzi sono associati a un singolo piano di Azure.</span><span class="sxs-lookup"><span data-stu-id="53712-131">All usage is tied back to a single azure plan.</span></span> 

2. <span data-ttu-id="53712-132">All'interno di un piano saranno presenti una o più sottoscrizioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="53712-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="53712-133">Si tratta di contenitori usati per la gestione e la distribuzione delle risorse.</span><span class="sxs-lookup"><span data-stu-id="53712-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="53712-134">All'interno di una sottoscrizione, gruppi di risorse vengono aggiunti a risorse di gruppo.</span><span class="sxs-lookup"><span data-stu-id="53712-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="53712-135">Ogni risorsa viene distribuita a un solo gruppo di risorse.</span><span class="sxs-lookup"><span data-stu-id="53712-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="53712-136">Esempi di risorse sono le macchine virtuali e gli account di archiviazione.</span><span class="sxs-lookup"><span data-stu-id="53712-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="53712-137">Le risorse generano contatori, che sono misurazioni del consumo di una risorsa. Una risorsa può generare l'utilizzo di più contatori.</span><span class="sxs-lookup"><span data-stu-id="53712-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="53712-138">I contatori sono identificati da ProductId, SKUId e AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="53712-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="heirarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="53712-139">Gerarchia della misurazione e dei gruppi di risorse di sottoscrizione</span><span class="sxs-lookup"><span data-stu-id="53712-139">Heirarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="53712-140">**Account di Azure (tenant)**</span><span class="sxs-lookup"><span data-stu-id="53712-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="53712-141">Sottoscrizione A</span><span class="sxs-lookup"><span data-stu-id="53712-141">Subscription A</span></span>
    - <span data-ttu-id="53712-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="53712-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="53712-143">Macchina virtuale (risorsa)</span><span class="sxs-lookup"><span data-stu-id="53712-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="53712-144">Contatore di calcolo</span><span class="sxs-lookup"><span data-stu-id="53712-144">Compute meter</span></span>
        - <span data-ttu-id="53712-145">Rete virtuale (risorsa)</span><span class="sxs-lookup"><span data-stu-id="53712-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="53712-146">Nessun contatore di fatturazione</span><span class="sxs-lookup"><span data-stu-id="53712-146">No billing meter</span></span>

    - <span data-ttu-id="53712-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="53712-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="53712-148">Macchina virtuale (risorsa)</span><span class="sxs-lookup"><span data-stu-id="53712-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="53712-149">Contatore di calcolo</span><span class="sxs-lookup"><span data-stu-id="53712-149">Computer meter</span></span>
        - <span data-ttu-id="53712-150">Disco gestito SSD Premium (risorsa)</span><span class="sxs-lookup"><span data-stu-id="53712-150">Premium SSD managed disk (resource)</span></span>
            - <span data-ttu-id="53712-151">Contatore della capacità di archiviazione</span><span class="sxs-lookup"><span data-stu-id="53712-151">Storage capacity meter</span></span>
            - <span data-ttu-id="53712-152">Contatore delle operazioni di archiviazione</span><span class="sxs-lookup"><span data-stu-id="53712-152">Storage operations meter</span></span>

- <span data-ttu-id="53712-153">Sottoscrizione B   -ResourceGroup 1       - Azure SQL (risorsa)           - Contatore DTU       - Gateway VPN (risorsa)           - Contatore gateway VPN</span><span class="sxs-lookup"><span data-stu-id="53712-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="53712-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="53712-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="53712-155">Interfaccia di rete virtuale (risorsa)</span><span class="sxs-lookup"><span data-stu-id="53712-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="53712-156">Nessun contatore di fatturazione</span><span class="sxs-lookup"><span data-stu-id="53712-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="53712-157">Leggere la fattura</span><span class="sxs-lookup"><span data-stu-id="53712-157">Read the invoice</span></span>

1. <span data-ttu-id="53712-158">La fattura sarà disponibile entro il giorno 8 di ogni mese.</span><span class="sxs-lookup"><span data-stu-id="53712-158">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="53712-159">I partner hanno 60 giorni per effettuare il pagamento.</span><span class="sxs-lookup"><span data-stu-id="53712-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="53712-160">Il periodo di fatturazione riguarderà un determinato mese di calendario, ad esempio 01/10-31/10.</span><span class="sxs-lookup"><span data-stu-id="53712-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="53712-161">Gli addebiti sono al netto delle rettifiche (l'importo è al netto del "credito ottenuto dai partner per i servizi gestiti").</span><span class="sxs-lookup"><span data-stu-id="53712-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="53712-162">Per altri dettagli sulla fatturazione, esamina il file di riconciliazione della fattura e il file sull'utilizzo valutato su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="53712-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![fattura](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="53712-164">Leggere il file di riconciliazione della fattura</span><span class="sxs-lookup"><span data-stu-id="53712-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="53712-165">Per ogni combinazione di piano di Azure e contatore possono essere presenti al massimo due righe di fatturazione nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="53712-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="53712-166">Se il contatore è idoneo a un qualsiasi tipo di sconto o credito (ad esempio, agli sconti in base al livello o al credito ottenuto dai partner per i servizi gestiti) durante l'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53712-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="53712-167">La colonna **PriceAdjusmentDescription** farà riferimento allo sconto o al credito ottenuto.</span><span class="sxs-lookup"><span data-stu-id="53712-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="53712-168">Se non sono presenti risorse per un determinato contatore idoneo allo sconto o al credito ottenuto dai partner, il file di riconciliazione conterrà una sola riga di fatturazione e il prezzo unitario effettivo sarà il prezzo al dettaglio, ovvero il prezzo unitario.</span><span class="sxs-lookup"><span data-stu-id="53712-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="53712-169">Se il contatore, o qualsiasi risorsa che genera tale contatore, è idoneo al **credito ottenuto dai partner per i servizi gestiti** per una parte del mese, il file di riconciliazione conterrà due righe di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53712-169">If the meter, or any resources emitting that meter,qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="53712-170">Una riga rappresenterà i giorni per i quali il contatore è idoneo e la seconda rappresenterà i giorni per i quali non lo è.</span><span class="sxs-lookup"><span data-stu-id="53712-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="53712-171">Leggere il file sull'utilizzo giornaliero</span><span class="sxs-lookup"><span data-stu-id="53712-171">Read the daily usage file</span></span>

- <span data-ttu-id="53712-172">I contatori delle sottoscrizioni in un piano di Azure vengono valutati e cumulati su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="53712-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="53712-173">Il **credito ottenuto dai partner per i servizi gestiti** viene determinato e applicato su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="53712-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="53712-174">Ogni contatore della sottoscrizione avrà una riga per ogni giorno del mese di utilizzo.</span><span class="sxs-lookup"><span data-stu-id="53712-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="53712-175">Nell'esempio seguente:</span><span class="sxs-lookup"><span data-stu-id="53712-175">In the example below:</span></span>

  - <span data-ttu-id="53712-176">Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 01/07-03/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="53712-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="53712-177">Il contatore non è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 04/07-07/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio.</span><span class="sxs-lookup"><span data-stu-id="53712-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="53712-178">Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 08/07-31/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="53712-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![riconciliazione2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="53712-180">Fattura nella valuta del cliente</span><span class="sxs-lookup"><span data-stu-id="53712-180">Invoice in customer currency</span></span> 

<span data-ttu-id="53712-181">I prezzi per i servizi di Azure forniti tramite un piano di Azure verranno addebitati in USD e fatturati in base alla valuta assegnata al paese del cliente.</span><span class="sxs-lookup"><span data-stu-id="53712-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="53712-182">Se la valuta di fatturazione è diversa da USD, il tasso di cambio (FX) usato verrà visualizzato nell'ultima pagina della fattura.</span><span class="sxs-lookup"><span data-stu-id="53712-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="53712-183">I tassi di cambio vengono determinati mensilmente e applicati alla fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="53712-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="53712-184">Per un elenco completo delle valute dei paesi, vedi la [nuova matrice di disponibilità delle offerte commerciali nelle varie aree geografiche e valute dei clienti](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="53712-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span> 

<span data-ttu-id="53712-185">Microsoft userà [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) per determinare i tassi di cambio usati per la conversione della valuta dei prezzi nella valuta di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="53712-185">Microsoft will use [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="53712-186">I tassi di cambio verranno aggiornati e saranno disponibili il giorno precedente il primo giorno del mese in cui verranno applicati.</span><span class="sxs-lookup"><span data-stu-id="53712-186">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="53712-187">**Esempio**:  gli addebiti relativi all'utilizzo per il periodo di servizio compreso tra il 1° e il 31 agosto verranno fatturati in base al tasso di cambio pubblicato il 31 luglio.</span><span class="sxs-lookup"><span data-stu-id="53712-187">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="53712-188">Questi addebiti verranno riportati nella fattura di settembre e il tasso di cambio sarà indicato nell'ultima pagina della fattura.</span><span class="sxs-lookup"><span data-stu-id="53712-188">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="53712-189">Prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="53712-189">Azure reservations</span></span> 

<span data-ttu-id="53712-190">Se vengono acquistate [prenotazioni di Azure](https://docs.microsoft.com/partner-center/azure-reservations) tramite un piano di Azure, inizialmente nel Centro per i partner sarà possibile scegliere solo la fatturazione una tantum.</span><span class="sxs-lookup"><span data-stu-id="53712-190">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="53712-191">La fatturazione mensile è disponibile nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="53712-191">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="53712-192">Nel Centro per i partner sarà disponibile in una data successiva.</span><span class="sxs-lookup"><span data-stu-id="53712-192">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="53712-193">Spese di Azure</span><span class="sxs-lookup"><span data-stu-id="53712-193">Azure spending</span></span> 

<span data-ttu-id="53712-194">L'esperienza di spesa di Azure è stata aggiornata per supportare la nuova fatturazione del piano di Azure nel Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="53712-194">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="53712-195">Tale meccanismo consente ai partner di:</span><span class="sxs-lookup"><span data-stu-id="53712-195">This enables partners to:</span></span>

- <span data-ttu-id="53712-196">Visualizzare, gestire e ricevere avvisi per il budget impostato a livello di cliente</span><span class="sxs-lookup"><span data-stu-id="53712-196">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="53712-197">Visualizzare la spesa stimata totale per un piano di Azure (ripartita in base al livello di risorsa e contatore)</span><span class="sxs-lookup"><span data-stu-id="53712-197">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="53712-198">Poiché il modello di fatturazione per i servizi di Azure tramite un piano di Azure riguarda un tipo di utilizzo con pagamento posticipato, per evitare di ricevere una fattura di importo maggiore del previsto, i partner possono definire un budget mensile e tenere traccia della percentuale di utilizzo.</span><span class="sxs-lookup"><span data-stu-id="53712-198">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="53712-199">Un budget può essere applicato a un solo cliente o contemporaneamente a più clienti.</span><span class="sxs-lookup"><span data-stu-id="53712-199">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Spese di Azure](images/azure/azurespend.png)

<span data-ttu-id="53712-201">**Per altre informazioni**</span><span class="sxs-lookup"><span data-stu-id="53712-201">**For more information**</span></span>

-  <span data-ttu-id="53712-202">La modalità di calcolo del credito ottenuto dal partner (PEC) è indicata nel listino prezzi disponibile tramite il [dashboard](https://partner.microsoft.com/en-us/dashboard/) Centro per i partner (è richiesto l'accesso).</span><span class="sxs-lookup"><span data-stu-id="53712-202">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="53712-203">Acquistare il piano di Azure</span><span class="sxs-lookup"><span data-stu-id="53712-203">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="53712-204">Listino prezzi per la nuova esperienza commerciale di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="53712-204">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
