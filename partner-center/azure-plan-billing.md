---
title: Piano di Azure - Fatturazione | Centro per i partner
ms.topic: article
ms.date: 10/04/2019
description: Descrive la struttura della fattura e del file di riconciliazione
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171298"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="11ecb-103">Nuova esperienza commerciale in CSP - Fatturazione di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="11ecb-104">La fatturazione in base al piano di Azure è un'esperienza di fatturazione semplificata che prevede l'uso di una singola data di fatturazione allineata e di un periodo di fatturazione definito in base al mese di calendario.</span><span class="sxs-lookup"><span data-stu-id="11ecb-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="11ecb-105">Per informazioni sulla piattaforma di fatturazione, leggi la [Guida operativa al commercio moderno del Centro per i partner](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span><span class="sxs-lookup"><span data-stu-id="11ecb-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="11ecb-106">Riepilogo dei dati essenziali della fatturazione</span><span class="sxs-lookup"><span data-stu-id="11ecb-106">Summary of billing essentials</span></span>

- <span data-ttu-id="11ecb-107">**Data della fattura**: la fattura e il file di riconciliazione saranno disponibili nell'API o nel dashboard Centro per i partner entro il giorno 8 (mezzanotte UTC).</span><span class="sxs-lookup"><span data-stu-id="11ecb-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="11ecb-108">**Periodo di fatturazione**: il periodo di fatturazione è allineato al mese di calendario, ad esempio 01/10-31/10, 01/11-30/11.</span><span class="sxs-lookup"><span data-stu-id="11ecb-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="11ecb-109">**Addebiti per i periodi di servizio**: gli addebiti sono allineati al mese di calendario.</span><span class="sxs-lookup"><span data-stu-id="11ecb-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="11ecb-110">Se, ad esempio, il partner a cui è stata emessa la fattura aggiunge servizi di Azure tramite un piano di Azure il 15/10 e il cliente inizia a utilizzare i servizi di Azure il 15/10, il partner riceverà la fattura/riconciliazione il giorno 08/11 per l'utilizzo del servizio da parte del cliente per il periodo 15/10-31/10.</span><span class="sxs-lookup"><span data-stu-id="11ecb-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="11ecb-111">La fattura del mese successivo che verrà generata il giorno 08/12 conterrà tutti gli addebiti per il periodo di servizio 01/11-31/11.</span><span class="sxs-lookup"><span data-stu-id="11ecb-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="11ecb-112">**Termine di pagamento della fattura**: netto a 60 giorni.</span><span class="sxs-lookup"><span data-stu-id="11ecb-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="11ecb-113">**Valuta della fattura**: i partner continueranno a ricevere la fattura nella valuta assegnata del paese del cliente.</span><span class="sxs-lookup"><span data-stu-id="11ecb-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="11ecb-114">Se, ad esempio, il partner a cui viene emessa la fattura si trova in Irlanda e ha clienti nel Regno Unito, in Norvegia e in Germania, il partner riceverà una fattura/riconciliazione in GBP, NOK ed EUR.</span><span class="sxs-lookup"><span data-stu-id="11ecb-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="11ecb-115">**Incentivi per i partner**: pagamento a 45 giorni dalla fine del mese della fattura.</span><span class="sxs-lookup"><span data-stu-id="11ecb-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="11ecb-116">Accedere alle fatture e ai file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="11ecb-116">Access your invoices and recon files</span></span>

<span data-ttu-id="11ecb-117">L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione.</span><span class="sxs-lookup"><span data-stu-id="11ecb-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="11ecb-118">**Per accedere alla fattura e al file di riconciliazione**</span><span class="sxs-lookup"><span data-stu-id="11ecb-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="11ecb-119">Accedi al Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="11ecb-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="11ecb-120">Dal menu del Centro per i partner seleziona **Fatturazione**.</span><span class="sxs-lookup"><span data-stu-id="11ecb-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="11ecb-121">Seleziona la scheda per il periodo **Calendar-based** (Basato su calendario) e la valuta a cui sei interessato.</span><span class="sxs-lookup"><span data-stu-id="11ecb-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![fatturazione](images/azure/billing1.png)

4. <span data-ttu-id="11ecb-123">Seleziona **Invoice and Recon file** (Fattura e file di riconciliazione).</span><span class="sxs-lookup"><span data-stu-id="11ecb-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="11ecb-124">Per visualizzare i dati della cronologia relativa alle fatture e ai file di riconciliazione, espandi la riga della cronologia di fatturazione sottostante.</span><span class="sxs-lookup"><span data-stu-id="11ecb-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="11ecb-125">Leggere la fattura</span><span class="sxs-lookup"><span data-stu-id="11ecb-125">Read the invoice</span></span>

1. <span data-ttu-id="11ecb-126">La fattura sarà disponibile entro il giorno 8 di ogni mese.</span><span class="sxs-lookup"><span data-stu-id="11ecb-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="11ecb-127">I partner hanno 60 giorni per effettuare il pagamento.</span><span class="sxs-lookup"><span data-stu-id="11ecb-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="11ecb-128">Il periodo di fatturazione riguarderà un determinato mese di calendario, ad esempio 01/10-31/10.</span><span class="sxs-lookup"><span data-stu-id="11ecb-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="11ecb-129">Gli addebiti sono al netto delle rettifiche (l'importo è al netto del "Credito ottenuto dai partner per i servizi gestiti").</span><span class="sxs-lookup"><span data-stu-id="11ecb-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="11ecb-130">Per altri dettagli sulla fatturazione, esamina il file di riconciliazione della fattura e il file sull'utilizzo valutato su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="11ecb-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![fattura](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="11ecb-132">Leggere il file di riconciliazione</span><span class="sxs-lookup"><span data-stu-id="11ecb-132">Read the recon file</span></span>

1. <span data-ttu-id="11ecb-133">Ogni contatore della sottoscrizione di Azure può avere al massimo due righe di fatturazione nel file di riconciliazione.</span><span class="sxs-lookup"><span data-stu-id="11ecb-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="11ecb-134">Se il contatore è idoneo a un tipo di sconto o di credito (ad esempio, gli sconti di livello 1 o il credito ottenuto dai partner per i servizi gestiti) durante l'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="11ecb-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="11ecb-135">La colonna **PriceAdjustmentDescription** farà riferimento allo sconto o al credito ottenuto. Il prezzo unitario effettivo sarà il prezzo al dettaglio meno il credito ottenuto dai partner o eventuali altri sconti.</span><span class="sxs-lookup"><span data-stu-id="11ecb-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="11ecb-136">Se il contatore non è idoneo al credito ottenuto dai partner per i servizi gestiti nell'intero mese di calendario, il file di riconciliazione conterrà una sola riga di fatturazione e il prezzo unitario effettivo sarà il prezzo al dettaglio, ovvero il prezzo unitario.</span><span class="sxs-lookup"><span data-stu-id="11ecb-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="11ecb-137">Se il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** per una parte del mese, il file di riconciliazione conterrà due righe di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="11ecb-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="11ecb-138">Una riga rappresenterà i giorni per i quali il contatore è idoneo e la seconda rappresenterà i giorni per i quali non lo è.</span><span class="sxs-lookup"><span data-stu-id="11ecb-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="11ecb-139">Leggere il file sull'utilizzo giornaliero</span><span class="sxs-lookup"><span data-stu-id="11ecb-139">Read the daily usage file</span></span>

- <span data-ttu-id="11ecb-140">I contatori delle sottoscrizioni in un piano di Azure vengono valutati e cumulati su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="11ecb-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="11ecb-141">Il **credito ottenuto dai partner per i servizi gestiti** viene determinato e applicato su base giornaliera.</span><span class="sxs-lookup"><span data-stu-id="11ecb-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="11ecb-142">Ogni contatore della sottoscrizione avrà una riga per ogni giorno del mese di utilizzo.</span><span class="sxs-lookup"><span data-stu-id="11ecb-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="11ecb-143">Nell'esempio seguente:</span><span class="sxs-lookup"><span data-stu-id="11ecb-143">In the example below:</span></span>

  - <span data-ttu-id="11ecb-144">Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 01/07-03/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="11ecb-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="11ecb-145">Il contatore non è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 04/07-07/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio.</span><span class="sxs-lookup"><span data-stu-id="11ecb-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="11ecb-146">Il contatore è idoneo al **credito ottenuto dai partner per i servizi gestiti** nel periodo 08/07-31/07. Si noti che il prezzo unitario effettivo equivale al prezzo al dettaglio meno il credito ottenuto dai partner.</span><span class="sxs-lookup"><span data-stu-id="11ecb-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![riconciliazione2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="11ecb-148">Fattura nella valuta del cliente</span><span class="sxs-lookup"><span data-stu-id="11ecb-148">Invoice in customer currency</span></span> 

<span data-ttu-id="11ecb-149">I prezzi per i servizi di Azure forniti tramite un piano di Azure verranno addebitati in USD e fatturati in base alla valuta assegnata al paese del cliente.</span><span class="sxs-lookup"><span data-stu-id="11ecb-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="11ecb-150">Se la valuta di fatturazione è diversa da USD, il tasso di cambio usato verrà visualizzato nell'ultima pagina della fattura.</span><span class="sxs-lookup"><span data-stu-id="11ecb-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="11ecb-151">I tassi di cambio vengono determinati mensilmente e applicati alla fattura successiva.</span><span class="sxs-lookup"><span data-stu-id="11ecb-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="11ecb-152">Per l'elenco completo delle valute dei paesi, vedi la [nuova matrice di disponibilità delle offerte commerciali nelle varie aree geografiche e valute dei clienti](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span><span class="sxs-lookup"><span data-stu-id="11ecb-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="11ecb-153">Microsoft userà [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) per determinare il tasso di cambio usato per la conversione della valuta dei prezzi nella valuta della fattura.</span><span class="sxs-lookup"><span data-stu-id="11ecb-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="11ecb-154">Il tasso di cambio verrà aggiornato e sarà disponibile il giorno precedente il primo giorno del mese in cui verrà applicato.</span><span class="sxs-lookup"><span data-stu-id="11ecb-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="11ecb-155">**Esempio**:  gli addebiti relativi all'utilizzo per il periodo di servizio compreso tra il 1° agosto e il 31 agosto verranno fatturati in base al tasso di cambio pubblicato il 1° agosto.</span><span class="sxs-lookup"><span data-stu-id="11ecb-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="11ecb-156">Questi addebiti verranno riportati nella fattura di settembre e il tasso di cambio sarà indicato nell'ultima pagina della fattura.</span><span class="sxs-lookup"><span data-stu-id="11ecb-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="11ecb-157">Gli utenti del tenant del partner continueranno a visualizzare le informazioni correlate specifiche dei ruoli riguardanti tutti i clienti e tutti gli ordini, indipendentemente dalla valuta di fatturazione.</span><span class="sxs-lookup"><span data-stu-id="11ecb-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="11ecb-158">Inoltre, l'utente potrà visualizzare tutte le fatture in tutte le valute.</span><span class="sxs-lookup"><span data-stu-id="11ecb-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="11ecb-159">Prenotazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-159">Azure reservations</span></span> 

<span data-ttu-id="11ecb-160">Se vengono acquistate [prenotazioni di Azure](https://docs.microsoft.com/partner-center/azure-reservations) tramite un piano di Azure, inizialmente nel Centro per i partner sarà possibile scegliere solo la fatturazione una tantum.</span><span class="sxs-lookup"><span data-stu-id="11ecb-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="11ecb-161">La fatturazione mensile è disponibile nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="11ecb-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="11ecb-162">Nel Centro per i partner sarà disponibile in una data successiva.</span><span class="sxs-lookup"><span data-stu-id="11ecb-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="11ecb-163">Gestione costi di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-163">Azure cost management</span></span> 

<span data-ttu-id="11ecb-164">Gli strumenti di Gestione costi di Azure consentono alle organizzazioni di visualizzare, gestire e ottimizzare i costi in Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="11ecb-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="11ecb-165">Questa funzionalità sarà disponibile nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="11ecb-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="11ecb-166">I partner avranno a disposizione una soluzione sempre attiva, a bassa latenza, con le seguenti funzionalità:</span><span class="sxs-lookup"><span data-stu-id="11ecb-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="11ecb-167">Analisi avanzata e avvisi relativi al budget</span><span class="sxs-lookup"><span data-stu-id="11ecb-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="11ecb-168">API e connettori di Power BI</span><span class="sxs-lookup"><span data-stu-id="11ecb-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="11ecb-169">Visualizzazione di più clienti</span><span class="sxs-lookup"><span data-stu-id="11ecb-169">Multi-customer view</span></span> 
- <span data-ttu-id="11ecb-170">Gestione gratuita dei costi di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="11ecb-171">Espansione di ruoli/utenti</span><span class="sxs-lookup"><span data-stu-id="11ecb-171">Expansion of roles/users</span></span> 

<span data-ttu-id="11ecb-172">Visita la pagina [Gestione dei costi e fatturazione di Azure](https://azure.microsoft.com/services/cost-management) per altre informazioni su questa funzionalità, disponibile per i contratti Enterprise Agreement dal mese di febbraio 2019.</span><span class="sxs-lookup"><span data-stu-id="11ecb-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="11ecb-173">La funzionalità è disponibile solo con i servizi di Azure acquistati nell'ambito di questa nuova esperienza commerciale di Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="11ecb-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="11ecb-174">Spese di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-174">Azure spending</span></span> 

<span data-ttu-id="11ecb-175">Nel Centro per i partner sarà disponibile uno strumento di calcolo delle spese di Azure per la nuova esperienza commerciale in CSP.</span><span class="sxs-lookup"><span data-stu-id="11ecb-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="11ecb-176">Quando applicata, questa funzionalità consentirà ai partner di visualizzare i dati seguenti:</span><span class="sxs-lookup"><span data-stu-id="11ecb-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="11ecb-177">Budget totale per un cliente</span><span class="sxs-lookup"><span data-stu-id="11ecb-177">Total budget on a customer</span></span> 
- <span data-ttu-id="11ecb-178">Spese stimate totali per un piano di Azure esistente</span><span class="sxs-lookup"><span data-stu-id="11ecb-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="11ecb-179">Percentuale di utilizzo dei clienti in ogni periodo di fatturazione</span><span class="sxs-lookup"><span data-stu-id="11ecb-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="11ecb-180">Poiché il modello di fatturazione per i servizi di Azure tramite un piano di Azure riguarda un tipo di utilizzo con pagamento posticipato, per evitare di ricevere una fattura di importo maggiore del previsto, i partner possono definire un budget mensile e tenere traccia della percentuale di utilizzo.</span><span class="sxs-lookup"><span data-stu-id="11ecb-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="11ecb-181">Un budget può essere applicato a un solo cliente o contemporaneamente a più clienti.</span><span class="sxs-lookup"><span data-stu-id="11ecb-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Spese di Azure](images/azure/azurespend.png)

<span data-ttu-id="11ecb-183">**Per altre informazioni**</span><span class="sxs-lookup"><span data-stu-id="11ecb-183">**For more information**</span></span>

-  <span data-ttu-id="11ecb-184">La modalità di calcolo del credito guadagnato dal partner (PEC) è indicata nel listino prezzi disponibile tramite il dashboard Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="11ecb-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="11ecb-185">Acquistare il piano di Azure</span><span class="sxs-lookup"><span data-stu-id="11ecb-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="11ecb-186">Listino prezzi per la nuova esperienza commerciale di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="11ecb-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
