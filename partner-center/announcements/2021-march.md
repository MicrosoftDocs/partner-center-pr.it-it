---
title: Annunci 2021 di marzo
description: 2021 annunci per il centro per i partner Microsoft, incluse nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374389"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="56f03-103">Annunci 2021 di marzo</span><span class="sxs-lookup"><span data-stu-id="56f03-103">March 2021 announcements</span></span>

<span data-ttu-id="56f03-104">Questa pagina fornisce gli annunci per Microsoft Partner Center per il 2021 marzo.</span><span class="sxs-lookup"><span data-stu-id="56f03-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="56f03-105">API di convalida degli indirizzi dei clienti CSP aggiornata ora disponibile per il test</span><span class="sxs-lookup"><span data-stu-id="56f03-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-106">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-106">Categories</span></span>

- <span data-ttu-id="56f03-107">Data: 2021-03-31</span><span class="sxs-lookup"><span data-stu-id="56f03-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="56f03-108">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-109">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-109">Summary</span></span>

<span data-ttu-id="56f03-110">Nell'ambito del nostro impegno per aiutare i partner e i clienti a svolgere la propria attività in base alla fiducia, verranno invitati i partner in tutto il mondo per testare le modifiche apportate all'API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="56f03-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-111">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-111">Impacted audience</span></span>

<span data-ttu-id="56f03-112">Tutti i partner di fatturazione diretta CSP e i provider indiretti che creano o aggiornano i dettagli di un indirizzo cliente esistente</span><span class="sxs-lookup"><span data-stu-id="56f03-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="56f03-113">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-113">Details</span></span>

<span data-ttu-id="56f03-114">Microsoft</span><span class="sxs-lookup"><span data-stu-id="56f03-114">Microsoft runs on trust.</span></span> <span data-ttu-id="56f03-115">Ci impegniamo a fornire un metodo conforme, sicuro e sicuro per l'invio della convalida degli indirizzi dei clienti per la transazione degli abbonamenti ai clienti nel programma CSP.</span><span class="sxs-lookup"><span data-stu-id="56f03-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="56f03-116">Attualmente, il 31 marzo 2021 abbiamo introdotto modifiche all'API ValidateAddress che vorremmo invitare a testare, prima di continuare a vivere con le modifiche apportate a giugno 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="56f03-117">Si noti che queste modifiche influiscono solo sull'API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="56f03-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="56f03-118">Le API CreateCustomer e UpdateBillingProfile non sono interessate.</span><span class="sxs-lookup"><span data-stu-id="56f03-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="56f03-119">La risposta restituirà uno dei messaggi di stato seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="56f03-120">Stato</span><span class="sxs-lookup"><span data-stu-id="56f03-120">Status</span></span> | <span data-ttu-id="56f03-121">Descrizione</span><span class="sxs-lookup"><span data-stu-id="56f03-121">Description</span></span> | <span data-ttu-id="56f03-122">Numero di indirizzi suggeriti restituiti</span><span class="sxs-lookup"><span data-stu-id="56f03-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="56f03-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="56f03-123">VerifiedShippable</span></span> | <span data-ttu-id="56f03-124">L'indirizzo viene verificato e può essere spedito a.</span><span class="sxs-lookup"><span data-stu-id="56f03-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="56f03-125">Single</span><span class="sxs-lookup"><span data-stu-id="56f03-125">Single</span></span> |
| <span data-ttu-id="56f03-126">Verified</span><span class="sxs-lookup"><span data-stu-id="56f03-126">Verified</span></span> | <span data-ttu-id="56f03-127">L'indirizzo è verificato.</span><span class="sxs-lookup"><span data-stu-id="56f03-127">Address is verified.</span></span> | <span data-ttu-id="56f03-128">Single</span><span class="sxs-lookup"><span data-stu-id="56f03-128">Single</span></span> |
| <span data-ttu-id="56f03-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="56f03-129">InteractionRequired</span></span> | <span data-ttu-id="56f03-130">Gli indirizzi suggeriti sono stati modificati in modo significativo e richiedono la conferma dell'utente.</span><span class="sxs-lookup"><span data-stu-id="56f03-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="56f03-131">Single</span><span class="sxs-lookup"><span data-stu-id="56f03-131">Single</span></span> |
| <span data-ttu-id="56f03-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="56f03-132">StreetPartial</span></span> | <span data-ttu-id="56f03-133">La via specificata nell'indirizzo è parziale e necessita di altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="56f03-134">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="56f03-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="56f03-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="56f03-135">PremisesPartial</span></span> | <span data-ttu-id="56f03-136">I dati locali (numero di edificio, numero di gruppo e così via) sono parziali e richiedono altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="56f03-137">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="56f03-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="56f03-138">Più elementi</span><span class="sxs-lookup"><span data-stu-id="56f03-138">Multiple</span></span> | <span data-ttu-id="56f03-139">Sono presenti più campi parziali nell'indirizzo, che includono potenzialmente anche StreetPartial e PremisesPartial.</span><span class="sxs-lookup"><span data-stu-id="56f03-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="56f03-140">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="56f03-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="56f03-141">nessuno</span><span class="sxs-lookup"><span data-stu-id="56f03-141">None</span></span> | <span data-ttu-id="56f03-142">L'indirizzo non è corretto.</span><span class="sxs-lookup"><span data-stu-id="56f03-142">Address is incorrect.</span></span> | <span data-ttu-id="56f03-143">nessuno</span><span class="sxs-lookup"><span data-stu-id="56f03-143">None</span></span> |
| <span data-ttu-id="56f03-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="56f03-144">NotValidated</span></span> | <span data-ttu-id="56f03-145">Non è stato possibile inviare l'indirizzo durante il processo di convalida.</span><span class="sxs-lookup"><span data-stu-id="56f03-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="56f03-146">nessuno</span><span class="sxs-lookup"><span data-stu-id="56f03-146">None</span></span> |

<span data-ttu-id="56f03-147">Una volta che un indirizzo è stato inviato per essere convalidato tramite l'API ValidateAddress, verrà restituito il seguente schema di risposta:</span><span class="sxs-lookup"><span data-stu-id="56f03-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="56f03-148">Esaminare questa risposta di esempio.</span><span class="sxs-lookup"><span data-stu-id="56f03-148">Take a look at this sample response.</span></span> <span data-ttu-id="56f03-149">Si noti che per gli Stati Uniti, la risposta restituirà un suffisso di quattro cifre aggiuntivo per la riga di codice postale se si immettono solo cinque cifre per il codice postale.</span><span class="sxs-lookup"><span data-stu-id="56f03-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="56f03-150">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-150">Next steps</span></span>

- <span data-ttu-id="56f03-151">Condividi il tuo ID tenant sandbox con il nostro esperto in materia (PMI), Ali khaki, da includere nel test Flight, in modo che tu possa iniziare la preparazione per l'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="56f03-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="56f03-152">Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.</span><span class="sxs-lookup"><span data-stu-id="56f03-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-153">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-153">Questions?</span></span>

<span data-ttu-id="56f03-154">In caso di domande o se è necessario supporto per le operazioni con Microsoft, contattare il gruppo Yammer del supporto partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="56f03-155">Nuova esperienza dell'interfaccia di amministrazione di Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="56f03-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-156">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-156">Categories</span></span>

- <span data-ttu-id="56f03-157">Data: 2021-03-29</span><span class="sxs-lookup"><span data-stu-id="56f03-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="56f03-158">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-159">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-159">Summary</span></span>

<span data-ttu-id="56f03-160">A partire dal 27 aprile 2021, l'interfaccia di amministrazione di Exchange fornirà una nuova esperienza che consente di migliorare l'efficienza quotidiana per gli utenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-161">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-161">Impacted audience</span></span>

<span data-ttu-id="56f03-162">Amministratori delegati che accedono a Exchange tramite il centro per i partner</span><span class="sxs-lookup"><span data-stu-id="56f03-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="56f03-163">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-163">Details</span></span>

<span data-ttu-id="56f03-164">A partire dal 27 aprile 2021, i partner che passano a Exchange tramite il centro per i partner verranno reindirizzati al nuovo EAC.</span><span class="sxs-lookup"><span data-stu-id="56f03-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="56f03-165">Questa nuova esperienza è attualmente disponibile come anteprima e gli amministratori possono attivare questa esperienza selezionando l'interruttore nell'angolo superiore destro all'interno dell'interfaccia di amministrazione classica.</span><span class="sxs-lookup"><span data-stu-id="56f03-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="56f03-166">È anche possibile passare al nuovo EAC selezionando il banner "try it Now" visualizzato in tutte le pagine.</span><span class="sxs-lookup"><span data-stu-id="56f03-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="56f03-167">I vantaggi del nuovo EAC sono i seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="56f03-168">Aggiunta di informazioni dettagliate, report e meccanismi di avviso per i problemi relativi al flusso di posta.</span><span class="sxs-lookup"><span data-stu-id="56f03-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="56f03-169">Dashboard personalizzati per aumentare la produttività.</span><span class="sxs-lookup"><span data-stu-id="56f03-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="56f03-170">Per facilitare l'esplorazione della nuova esperienza, i video sono disponibili nella sezione **Training & guide** della nuova esperienza di Exchange.</span><span class="sxs-lookup"><span data-stu-id="56f03-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="56f03-171">Questi forniranno una panoramica di come usare al meglio il nuovo portale.</span><span class="sxs-lookup"><span data-stu-id="56f03-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="56f03-172">Con questa modifica, l'esperienza classica di EAC non sarà deprecata.</span><span class="sxs-lookup"><span data-stu-id="56f03-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="56f03-173">L'utente riceverà una notifica in anticipo prima dell'implementazione di qualsiasi modifica.</span><span class="sxs-lookup"><span data-stu-id="56f03-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-174">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-174">Next steps</span></span>

- <span data-ttu-id="56f03-175">Vedere le [risorse relative a questo argomento](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), in cui è possibile visualizzare le schermate della nuova esperienza.</span><span class="sxs-lookup"><span data-stu-id="56f03-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="56f03-176">Condividere queste informazioni con le parti interessate appropriate nella propria organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="56f03-177">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-177">Questions?</span></span>

<span data-ttu-id="56f03-178">Per eventuali domande su queste modifiche, verificare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="56f03-179">Microsoft Operations: Introduzione al calendario di avvio del prodotto</span><span class="sxs-lookup"><span data-stu-id="56f03-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-180">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-180">Categories</span></span>

- <span data-ttu-id="56f03-181">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="56f03-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="56f03-182">Offerte | Area di lavoro moderna</span><span class="sxs-lookup"><span data-stu-id="56f03-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-183">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-183">Summary</span></span>

<span data-ttu-id="56f03-184">In risposta ai commenti dei partner, Microsoft Operations semplifica le comunicazioni per i lanci di prodotti.</span><span class="sxs-lookup"><span data-stu-id="56f03-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-185">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-185">Impacted audience</span></span>

<span data-ttu-id="56f03-186">Partner Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="56f03-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="56f03-187">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-187">Details</span></span>

<span data-ttu-id="56f03-188">Microsoft si impegna a migliorare continuamente le esperienze del partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="56f03-189">Ci sono stati commenti e suggerimenti ricevuti da un numero eccessivo di comunicazioni da Microsoft, inclusi gli annunci duplicati per i lanci di prodotti.</span><span class="sxs-lookup"><span data-stu-id="56f03-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="56f03-190">In risposta ai commenti e suggerimenti, Microsoft ha semplificato l'esperienza di conformità per i lanci di prodotti per offerte nuove ed esistenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="56f03-191">È ora disponibile una singola visualizzazione mensile dei lanci di prodotti, pubblicati nella raccolta di risorse per la preparazione delle operazioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="56f03-192">La [visualizzazione del calendario](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) per il lancio mensile dei prodotti sostituirà le comunicazioni di avvio dei singoli prodotti nella raccolta di risorse per la preparazione delle operazioni e negli annunci del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="56f03-193">È anche possibile accedere a [questo calendario di avvio del prodotto](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) da [raccolte della community](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [visualizzazioni del calendario](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)e [newsletter CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="56f03-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="56f03-194">Ti invieremo una notifica quando pubblichiamo il calendario di lancio del prodotto di ogni mese con un annuncio nella raccolta di risorse per la preparazione delle operazioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="56f03-195">È comunque possibile trovare informazioni sulle offerte nuove ed esistenti nei log di anteprima e prezzi dell'elenco prezzi, oltre che nei Blog del prodotto, nelle guide alle licenze e nelle pagine di marketing del prodotto.</span><span class="sxs-lookup"><span data-stu-id="56f03-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="56f03-196">La modifica verrà applicata agli avvii per i prodotti seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="56f03-197">Dynamics locale</span><span class="sxs-lookup"><span data-stu-id="56f03-197">Dynamics on-premises</span></span>
- <span data-ttu-id="56f03-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="56f03-198">Microsoft 365</span></span>
- <span data-ttu-id="56f03-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="56f03-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="56f03-200">Windows</span><span class="sxs-lookup"><span data-stu-id="56f03-200">Windows</span></span>
- <span data-ttu-id="56f03-201">Server</span><span class="sxs-lookup"><span data-stu-id="56f03-201">Server</span></span>  
- <span data-ttu-id="56f03-202">Strumenti</span><span class="sxs-lookup"><span data-stu-id="56f03-202">Tools</span></span>
- <span data-ttu-id="56f03-203">Team e Telco</span><span class="sxs-lookup"><span data-stu-id="56f03-203">Teams and Telco</span></span>

<span data-ttu-id="56f03-204">Si continuerà a inviare annunci specifici per i lanci di prodotti che richiedono dettagli sulla conformità delle operazioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-205">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-205">Next steps</span></span>

<span data-ttu-id="56f03-206">Esaminare le risorse relative a questo argomento e condividere queste informazioni con le parti interessate appropriate all'interno dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-207">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-207">Questions?</span></span>

<span data-ttu-id="56f03-208">Per altre domande su queste offerte, vedere le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="56f03-209">Modifiche ai requisiti di onboarding dei clienti CSP</span><span class="sxs-lookup"><span data-stu-id="56f03-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-210">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-210">Categories</span></span>

- <span data-ttu-id="56f03-211">Data: 2021-03-25</span><span class="sxs-lookup"><span data-stu-id="56f03-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="56f03-212">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-213">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-213">Summary</span></span>

<span data-ttu-id="56f03-214">Nell'ambito del nostro impegno per aiutare i partner e i clienti a svolgere la propria attività in base alla fiducia, Microsoft richiederà ulteriori informazioni sui clienti, a partire dal 25 marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-215">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-215">Impacted audience</span></span>

<span data-ttu-id="56f03-216">Provider di soluzioni cloud (CSP) Direct Bill partner e provider indiretti con clienti nuovi o esistenti nei paesi elencati nella sezione successiva</span><span class="sxs-lookup"><span data-stu-id="56f03-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="56f03-217">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-217">Details</span></span>

<span data-ttu-id="56f03-218">Microsoft</span><span class="sxs-lookup"><span data-stu-id="56f03-218">Microsoft runs on trust.</span></span> <span data-ttu-id="56f03-219">si impegna a fornire un metodo di convalida dei clienti conforme e sicuro per la vendita di sottoscrizioni cliente nel programma CSP.</span><span class="sxs-lookup"><span data-stu-id="56f03-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="56f03-220">Il 25 marzo 2021 verranno introdotti i miglioramenti apportati all'interfaccia utente e alle API del centro per i partner che influiranno sui partner che soddisfano entrambi i criteri seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="56f03-221">Il partner ha una relazione di fatturazione diretta con Microsoft (ovvero, è un partner con fatturazione diretta o un provider indiretto).</span><span class="sxs-lookup"><span data-stu-id="56f03-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="56f03-222">Il partner opera con clienti nuovi o esistenti nei paesi seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="56f03-223">Thailandia</span><span class="sxs-lookup"><span data-stu-id="56f03-223">Thailand</span></span>
    - <span data-ttu-id="56f03-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="56f03-224">Vietnam</span></span>
    - <span data-ttu-id="56f03-225">Turchia</span><span class="sxs-lookup"><span data-stu-id="56f03-225">Turkey</span></span>
    - <span data-ttu-id="56f03-226">Polonia</span><span class="sxs-lookup"><span data-stu-id="56f03-226">Poland</span></span>
    - <span data-ttu-id="56f03-227">Sud Africa</span><span class="sxs-lookup"><span data-stu-id="56f03-227">South Africa</span></span>
    - <span data-ttu-id="56f03-228">India</span><span class="sxs-lookup"><span data-stu-id="56f03-228">India</span></span>
    - <span data-ttu-id="56f03-229">Brasile</span><span class="sxs-lookup"><span data-stu-id="56f03-229">Brazil</span></span>
    - <span data-ttu-id="56f03-230">Iraq</span><span class="sxs-lookup"><span data-stu-id="56f03-230">Iraq</span></span>
    - <span data-ttu-id="56f03-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="56f03-231">Myanmar</span></span>
    - <span data-ttu-id="56f03-232">Sud Sudan</span><span class="sxs-lookup"><span data-stu-id="56f03-232">South Sudan</span></span>
    - <span data-ttu-id="56f03-233">Arabia Saudita</span><span class="sxs-lookup"><span data-stu-id="56f03-233">Saudi Arabia</span></span>
    - <span data-ttu-id="56f03-234">Emirati Arabi Uniti</span><span class="sxs-lookup"><span data-stu-id="56f03-234">United Arab Emirates</span></span>
    - <span data-ttu-id="56f03-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="56f03-235">Venezuela</span></span>

<span data-ttu-id="56f03-236">I partner che soddisfano i criteri dovranno inviare l' **ID registrazione della società** del cliente (noto anche come Locanda dell' **organizzazione** del cliente) e il **numero di telefono** quando caricano nuovi clienti o modificano i dettagli dei clienti esistenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="56f03-237">I partner possono anche immettere un **secondo nome** facoltativo per il cliente.</span><span class="sxs-lookup"><span data-stu-id="56f03-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="56f03-238">Si noti che quando si aggiunge l'ID registrazione aziendale, è necessario usare l'ID dell'imposta aziendale e non l'ID personale del cliente.</span><span class="sxs-lookup"><span data-stu-id="56f03-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="56f03-239">I partner che svolgono attività con clienti nuovi o esistenti nei paesi seguenti hanno già eseguito l'onboarding di una versione precedente a novembre 2020.</span><span class="sxs-lookup"><span data-stu-id="56f03-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="56f03-240">Armenia</span><span class="sxs-lookup"><span data-stu-id="56f03-240">Armenia</span></span>
- <span data-ttu-id="56f03-241">Azerbaigian</span><span class="sxs-lookup"><span data-stu-id="56f03-241">Azerbaijan</span></span>
- <span data-ttu-id="56f03-242">Bielorussia</span><span class="sxs-lookup"><span data-stu-id="56f03-242">Belarus</span></span>
- <span data-ttu-id="56f03-243">Ungheria</span><span class="sxs-lookup"><span data-stu-id="56f03-243">Hungary</span></span>
- <span data-ttu-id="56f03-244">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="56f03-244">Kazakhstan</span></span>
- <span data-ttu-id="56f03-245">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="56f03-245">Kyrgyzstan</span></span>
- <span data-ttu-id="56f03-246">Moldova</span><span class="sxs-lookup"><span data-stu-id="56f03-246">Moldova</span></span>
- <span data-ttu-id="56f03-247">Russia</span><span class="sxs-lookup"><span data-stu-id="56f03-247">Russia</span></span>
- <span data-ttu-id="56f03-248">Tagikistan</span><span class="sxs-lookup"><span data-stu-id="56f03-248">Tajikistan</span></span>
- <span data-ttu-id="56f03-249">Ucraina</span><span class="sxs-lookup"><span data-stu-id="56f03-249">Ukraine</span></span>
- <span data-ttu-id="56f03-250">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="56f03-250">Uzbekistan</span></span>

<span data-ttu-id="56f03-251">I partner con clienti nel resto del mondo avranno la possibilità di usare il 25 marzo 2021 per immettere l' **ID registrazione aziendale**, il **numero di telefono** e il **secondo nome** per i clienti come dettagli facoltativi.</span><span class="sxs-lookup"><span data-stu-id="56f03-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-252">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-252">Next steps</span></span>

- <span data-ttu-id="56f03-253">Per istruzioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella [raccolta di partner dedicati](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .</span><span class="sxs-lookup"><span data-stu-id="56f03-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="56f03-254">Prepararsi a incorporare le modifiche usando l'API del centro per i partner e l'esperienza utente Web.</span><span class="sxs-lookup"><span data-stu-id="56f03-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="56f03-255">Saranno disponibili API e SDK a scopo di test.</span><span class="sxs-lookup"><span data-stu-id="56f03-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="56f03-256">Assicurarsi di inviare i dati aggiuntivi quando si caricano nuovi clienti o si modificano i dettagli del cliente esistente.</span><span class="sxs-lookup"><span data-stu-id="56f03-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="56f03-257">Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.</span><span class="sxs-lookup"><span data-stu-id="56f03-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-258">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-258">Questions?</span></span>

<span data-ttu-id="56f03-259">In caso di domande relative all'identificatore legale (noto anche come INN o codice identificativo del contribuente), contattare il consulente fiscale o l'ufficio fiscale locale.</span><span class="sxs-lookup"><span data-stu-id="56f03-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="56f03-260">Microsoft non è in grado di fornire indicazioni sulle imposte.</span><span class="sxs-lookup"><span data-stu-id="56f03-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="56f03-261">Se è necessario il supporto per le operazioni con Microsoft, [aprire una richiesta di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="56f03-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="56f03-262">Correzioni apportate al 1 ° marzo 2021 elenco prezzi software perpetuo</span><span class="sxs-lookup"><span data-stu-id="56f03-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-263">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-263">Categories</span></span>

- <span data-ttu-id="56f03-264">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="56f03-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="56f03-265">Offerte/mercati</span><span class="sxs-lookup"><span data-stu-id="56f03-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-266">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-266">Impacted audience</span></span>

<span data-ttu-id="56f03-267">Provider indiretti e partner di fatturazione diretta che trasagiscono software perpetuo nel programma Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="56f03-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="56f03-268">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-268">Details</span></span>

<span data-ttu-id="56f03-269">Il listino prezzi per il software perpetuo pubblicato il 1 ° marzo 2021 include i mercati che non dovrebbero essere presenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="56f03-270">Il listino prezzi software perpetuo è stato aggiornato il 17 marzo 2021 con le correzioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="56f03-271">Queste correzioni sono applicabili solo a:</span><span class="sxs-lookup"><span data-stu-id="56f03-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="56f03-272">ID prodotto: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="56f03-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="56f03-273">Nome prodotto: aggiornamento da Windows 10 Home a Pro per Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="56f03-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="56f03-274">Mercati rimossi o non supportati: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LC, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, UR, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="56f03-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="56f03-275">Queste modifiche si applicano solo al prodotto precedente.</span><span class="sxs-lookup"><span data-stu-id="56f03-275">These changes only apply to the above product.</span></span> <span data-ttu-id="56f03-276">Altri prodotti non hanno alcuna correzione.</span><span class="sxs-lookup"><span data-stu-id="56f03-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="56f03-277">Passaggi successivi e risorse</span><span class="sxs-lookup"><span data-stu-id="56f03-277">Next steps and resources</span></span>

- <span data-ttu-id="56f03-278">I partner che eseguono transazioni software perpetue dovrebbero scaricare l'elenco dei prezzi software perpetuo più recente.</span><span class="sxs-lookup"><span data-stu-id="56f03-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="56f03-279">Consultare i [codici paese regione](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) per un mapping descrittivo dell'abbreviazione di due lettere ai paesi.</span><span class="sxs-lookup"><span data-stu-id="56f03-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="56f03-280">Versione SDK in .NET Standard (v 1.17.0)</span><span class="sxs-lookup"><span data-stu-id="56f03-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-281">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-281">Categories</span></span>

- <span data-ttu-id="56f03-282">Data: 2021-03-23</span><span class="sxs-lookup"><span data-stu-id="56f03-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="56f03-283">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="56f03-284">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-284">Impacted audience</span></span>

<span data-ttu-id="56f03-285">Partner di fatturazione diretta e provider indiretti che partecipano al programma CSP e usano .NET SDK del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="56f03-286">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-286">Details</span></span>

<span data-ttu-id="56f03-287">A partire dal 23 2020 marzo, i partner possono iniziare a scaricare la versione di [MicrosoftPartnerCenter. NetSDK (raccolta NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), insieme agli esempi aggiornati di [GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)public Partner Center SDK.</span><span class="sxs-lookup"><span data-stu-id="56f03-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="56f03-288">Questa versione include aggiornamenti ai metodi seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="56f03-289">Controllo aggiornato: nuovi tipi di operazione</span><span class="sxs-lookup"><span data-stu-id="56f03-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="56f03-290">Aggiunta di nuovi [tipi di operazione](https://docs.microsoft.com/partner-center/develop/auditing-resources) per sapere quando il cliente ha approvato e terminato DAP.</span><span class="sxs-lookup"><span data-stu-id="56f03-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="56f03-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="56f03-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="56f03-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="56f03-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="56f03-293">Controllo aggiornato: nuovi tipi di risorse e operazioni</span><span class="sxs-lookup"><span data-stu-id="56f03-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="56f03-294">Aggiunta di nuovi [tipi di risorse e operazioni](https://docs.microsoft.com/partner-center/develop/auditing-resources) per supportare lo scenario del ruolo della directory dei clienti.</span><span class="sxs-lookup"><span data-stu-id="56f03-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="56f03-295">Nuovo tipo di risorsa "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="56f03-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="56f03-296">Tipi di operazione "AddUserMember" e "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="56f03-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="56f03-297">Aggiornamenti dell'SDK per gli account dei clienti</span><span class="sxs-lookup"><span data-stu-id="56f03-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="56f03-298">Supporto per GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="56f03-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="56f03-299">OTTENERE/Customers/{Customer-Tenant-ID}/Qualifications</span><span class="sxs-lookup"><span data-stu-id="56f03-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="56f03-300">POST/Customers/{customer_id}/Qualifications? code = {validationCode}</span><span class="sxs-lookup"><span data-stu-id="56f03-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="56f03-301">Modifiche aggiuntive</span><span class="sxs-lookup"><span data-stu-id="56f03-301">Additional changes</span></span>

<span data-ttu-id="56f03-302">Le modifiche seguenti sono state introdotte come parte del nuovo commercio e sono attualmente disponibili per invito solo ai partner che fanno parte di M365/d365 New Commerce Experience Technical Preview.</span><span class="sxs-lookup"><span data-stu-id="56f03-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="56f03-303">I partner che non fanno parte del nuovo Commerce Technical Preview non devono essere in grado di rilevare gli effetti e dovrebbero essere compatibili con le versioni precedenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="56f03-304">Modifiche al catalogo:</span><span class="sxs-lookup"><span data-stu-id="56f03-304">Catalog Changes:</span></span>

  - <span data-ttu-id="56f03-305">OTTENERE/Products/{Product-ID}/SKUS/{SKU-ID}</span><span class="sxs-lookup"><span data-stu-id="56f03-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="56f03-306">Acquistare e gestire:</span><span class="sxs-lookup"><span data-stu-id="56f03-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="56f03-307">OTTENERE/customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="56f03-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="56f03-308">OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="56f03-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="56f03-309">PATCH/customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="56f03-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="56f03-310">OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="56f03-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="56f03-311">OTTENERE/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="56f03-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="56f03-312">POST/customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="56f03-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-313">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-313">Next Steps</span></span>

- <span data-ttu-id="56f03-314">Scaricare la versione più recente di [MicrosoftPartnerCenter. NetSDK (raccolta NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="56f03-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="56f03-315">Scaricare ed esaminare gli [esempi di GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="56f03-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="56f03-316">Offerta del Marketplace commerciale CSP e incentivi FY21 CSP per le offerte idonee</span><span class="sxs-lookup"><span data-stu-id="56f03-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-317">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-317">Categories</span></span>

- <span data-ttu-id="56f03-318">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="56f03-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="56f03-319">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-320">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-320">Impacted audience</span></span>

<span data-ttu-id="56f03-321">Provider indiretti e partner di fatturazione diretta nel programma Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="56f03-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="56f03-322">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-322">Details</span></span>

<span data-ttu-id="56f03-323">I provider indiretti e i partner di fatturazione diretta nel programma Cloud Solution Provider possono vendere offerte di terze parti e ottenere un incentivo per gli sconti per ogni offerta di terze parti idonea transazionale nel centro per i partner o nel portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="56f03-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="56f03-324">L'incentivo sarà sotto forma di sconto sulle vendite fatturate per le offerte idonee ed è **disponibile fino al 30 giugno 2021**.</span><span class="sxs-lookup"><span data-stu-id="56f03-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="56f03-325">Continua a conoscere questa offerta del Marketplace commerciale CSP di seguito e contatta i clienti oggi stesso per identificare le offerte giuste per consentire la continua riuscita e la trasformazione digitale.</span><span class="sxs-lookup"><span data-stu-id="56f03-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="56f03-326">Collaboriamo con fornitori di software indipendenti (ISV) per offrire al mercato le soluzioni SaaS e IaaS più recenti per i clienti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56f03-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="56f03-327">Gli editori ISV hanno la possibilità di abilitare le vendite delle loro offerte tramite il canale partner Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56f03-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="56f03-328">Le offerte idonee per gli incentivi rientrano in due categorie:</span><span class="sxs-lookup"><span data-stu-id="56f03-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="56f03-329">Selezionare le offerte SaaS e IaaS di terze parti con lo stato incentivate di co-selling IP di Azure.</span><span class="sxs-lookup"><span data-stu-id="56f03-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="56f03-330">Applicazioni SaaS integrate con team o almeno due app per la produttività Microsoft 365, ad esempio PowerPoint, Word, Excel, Outlook o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56f03-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="56f03-331">Passaggi successivi e risorse</span><span class="sxs-lookup"><span data-stu-id="56f03-331">Next steps and resources</span></span>

- <span data-ttu-id="56f03-332">Scopri come guadagnare gli [incentivi](https://partner.microsoft.com/membership/partner-incentives) per i partner per la vendita di app del Marketplace idonee per incentivare le app idonee.</span><span class="sxs-lookup"><span data-stu-id="56f03-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="56f03-333">Le nuove offerte vengono aggiunte ogni mese.</span><span class="sxs-lookup"><span data-stu-id="56f03-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="56f03-334">Risorse di Cloud Solution Provider Direct Bill partner incentive</span><span class="sxs-lookup"><span data-stu-id="56f03-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="56f03-335">Risorse di incentivi per provider indiretto del provider di soluzioni cloud</span><span class="sxs-lookup"><span data-stu-id="56f03-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="56f03-336">Per altre informazioni sulla vendita delle app del Marketplace commerciale, vedere questa [presentazione](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) .</span><span class="sxs-lookup"><span data-stu-id="56f03-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="56f03-337">Vedere risorse aggiuntive [qui](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="56f03-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="56f03-338">Esplorare il catalogo del Marketplace commerciale nel centro per i [partner](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) o [portale di Azure](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="56f03-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="56f03-339">Usare le [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) per integrare le app nel Marketplace aziendale</span><span class="sxs-lookup"><span data-stu-id="56f03-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="56f03-340">Rivolgersi agli ISV a cui si è interessati a lavorare con</span><span class="sxs-lookup"><span data-stu-id="56f03-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="56f03-341">I provider indiretti devono integrarsi usando le API e i rivenditori di guide in cui si vendono le app</span><span class="sxs-lookup"><span data-stu-id="56f03-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-342">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-342">Questions?</span></span>  

<span data-ttu-id="56f03-343">Vedere [questo articolo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) per una panoramica del Marketplace commerciale nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="56f03-344">Se è necessaria assistenza aggiuntiva, è possibile creare una richiesta di supporto nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="56f03-345">Ulteriori informazioni sono disponibili all'indirizzo [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="56f03-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="56f03-346">Nome dell'offerta Power BI Premium e aggiornamento dei prerequisiti</span><span class="sxs-lookup"><span data-stu-id="56f03-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-347">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-347">Categories</span></span>

- <span data-ttu-id="56f03-348">Data: 2021-03-18</span><span class="sxs-lookup"><span data-stu-id="56f03-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="56f03-349">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-350">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-350">Summary</span></span>

<span data-ttu-id="56f03-351">L'elenco dei prezzi finale del 1 ° aprile 2021 verrà aggiornato per aggiungere chiarezza alla denominazione e/o alle informazioni sui prerequisiti per le offerte Power BI Premium per utente.</span><span class="sxs-lookup"><span data-stu-id="56f03-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-352">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-352">Impacted audience</span></span>

<span data-ttu-id="56f03-353">Partner Cloud Solution Provider (CSP) diretti e indiretti</span><span class="sxs-lookup"><span data-stu-id="56f03-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="56f03-354">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-354">Details</span></span>

<span data-ttu-id="56f03-355">L'elenco dei prezzi finale del 1 ° aprile 2021 verrà aggiornato per aggiungere chiarezza alla denominazione e/o alle informazioni sui prerequisiti per le offerte Power BI Premium per utente.</span><span class="sxs-lookup"><span data-stu-id="56f03-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="56f03-356">Fino a quando non viene aggiornato l'elenco dei prezzi finale, utilizzare le informazioni contenute in questa sezione per assicurarsi che venga ordinato il prodotto corretto.</span><span class="sxs-lookup"><span data-stu-id="56f03-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="56f03-357">I dettagli seguenti mostrano lo SKU e i dettagli dei prerequisiti interessati.</span><span class="sxs-lookup"><span data-stu-id="56f03-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="56f03-358">Nome visualizzato dell'offerta il 1 ° marzo elenco prezzi anteprima</span><span class="sxs-lookup"><span data-stu-id="56f03-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="56f03-359">Nome visualizzato dell'offerta aggiornata l'elenco dei prezzi finale del 1 ° aprile</span><span class="sxs-lookup"><span data-stu-id="56f03-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="56f03-360">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="56f03-361">Power BI Premium per Add-On utente (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="56f03-362">Power BI Premium per Add-On utente **(Office)** (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="56f03-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="56f03-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="56f03-364">Per acquistare questa offerta, è necessario che i clienti abbiano uno dei prerequisiti seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="56f03-365">Nome visualizzato dell'offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-365">Offer display name</span></span> | <span data-ttu-id="56f03-366">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="56f03-367">Microsoft 365 E5 (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="56f03-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="56f03-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="56f03-369">Microsoft 365 E5 senza conferenza audio (prezzi del personale no profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="56f03-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="56f03-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="56f03-371">Office 365 E5 (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="56f03-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="56f03-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="56f03-373">Versione di valutazione di Office 365 E5 (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="56f03-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="56f03-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="56f03-375">Office 365 E5 senza conferenza audio (prezzi del personale no profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="56f03-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="56f03-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="56f03-377">Il Power BI Premium offerta seguente ha un prerequisito necessario per l'acquisto:</span><span class="sxs-lookup"><span data-stu-id="56f03-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="56f03-378">Nome visualizzato dell'offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-378">Offer display name</span></span> | <span data-ttu-id="56f03-379">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="56f03-380">Power BI Premium per Add-On utente (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="56f03-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="56f03-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="56f03-382">I clienti devono disporre di questo prerequisito per acquistare questa offerta:</span><span class="sxs-lookup"><span data-stu-id="56f03-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="56f03-383">Nome visualizzato dell'offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-383">Offer display name</span></span> | <span data-ttu-id="56f03-384">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="56f03-385">Power BI Pro (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="56f03-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="56f03-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="56f03-387">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-387">Next steps</span></span>

<span data-ttu-id="56f03-388">Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="56f03-389">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-389">Questions?</span></span>

<span data-ttu-id="56f03-390">Per eventuali domande su queste offerte, consultare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="56f03-391">Aggiornamenti dei prezzi di marzo per Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="56f03-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-392">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-392">Categories</span></span>

- <span data-ttu-id="56f03-393">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="56f03-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="56f03-394">Offerte/mercati</span><span class="sxs-lookup"><span data-stu-id="56f03-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-395">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-395">Summary</span></span>

<span data-ttu-id="56f03-396">I prezzi di marzo 2021 non corretti sono stati corretti per Microsoft 365 F3 British Pound (GBP) ed euro (EUR).</span><span class="sxs-lookup"><span data-stu-id="56f03-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-397">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-397">Impacted audience</span></span>

<span data-ttu-id="56f03-398">Partner che acquistano Microsoft 365 F3 in GBP o EUR tra il 1 ° marzo e il 17 marzo 2021 tramite il programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="56f03-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="56f03-399">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-399">Details</span></span>

<span data-ttu-id="56f03-400">Microsoft ha risolto i prezzi non corretti per Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="56f03-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="56f03-401">I prezzi non corretti erano per GBP ed EUR e solo per le offerte acquistate tra il 1 ° marzo e il 17 marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="56f03-402">Le offerte e le valute interessate sono elencate di seguito.</span><span class="sxs-lookup"><span data-stu-id="56f03-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="56f03-403">Nome offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-403">Offer name</span></span> | <span data-ttu-id="56f03-404">Valuta</span><span class="sxs-lookup"><span data-stu-id="56f03-404">Currency</span></span> | <span data-ttu-id="56f03-405">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-405">Offer ID</span></span> | <span data-ttu-id="56f03-406">ID materiale</span><span class="sxs-lookup"><span data-stu-id="56f03-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="56f03-407">Microsoft 365 F3 (carità)</span><span class="sxs-lookup"><span data-stu-id="56f03-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="56f03-408">GBP</span><span class="sxs-lookup"><span data-stu-id="56f03-408">GBP</span></span> | <span data-ttu-id="56f03-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="56f03-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="56f03-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="56f03-410">AAD-11626</span></span> |
| <span data-ttu-id="56f03-411">Microsoft 365 F3 (commerciale)</span><span class="sxs-lookup"><span data-stu-id="56f03-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="56f03-412">EUR</span><span class="sxs-lookup"><span data-stu-id="56f03-412">EUR</span></span>| <span data-ttu-id="56f03-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="56f03-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="56f03-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="56f03-414">AAA-89898</span></span> |
 
<span data-ttu-id="56f03-415">Gli elenchi prezzi di base per le licenze di marzo e aprile sono stati aggiornati il 16 marzo alle 17.00 ora solare Pacifico.</span><span class="sxs-lookup"><span data-stu-id="56f03-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-416">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-416">Next steps</span></span>

- <span data-ttu-id="56f03-417">I partner devono riscaricare gli elenchi prezzi correnti in base alla licenza, sia marzo sia l'anteprima di aprile, con queste correzioni dei prezzi, se applicabile.</span><span class="sxs-lookup"><span data-stu-id="56f03-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="56f03-418">Microsoft contatterà i partner interessati nelle prossime settimane via posta elettronica per informarli dei passaggi successivi relativi alla correzione delle transazioni interessate.</span><span class="sxs-lookup"><span data-stu-id="56f03-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-419">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-419">Questions?</span></span>

<span data-ttu-id="56f03-420">Per altre domande, consultare le community Yammer CSP pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="56f03-421">Aggiornare un nome di società legale tramite il centro per i partner</span><span class="sxs-lookup"><span data-stu-id="56f03-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-422">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-422">Categories</span></span>

- <span data-ttu-id="56f03-423">Data: 2021-03-16</span><span class="sxs-lookup"><span data-stu-id="56f03-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="56f03-424">Efficienza dell'unità & scalabilità</span><span class="sxs-lookup"><span data-stu-id="56f03-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-425">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-425">Summary</span></span>

<span data-ttu-id="56f03-426">A partire dal 2021 marzo, i partner di Microsoft Partner Network (MPN) e i rivenditori indiretti del provider di soluzioni cloud (CSP) possono aggiornare il nome della società legale tramite il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-427">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-427">Impacted audience</span></span>

<span data-ttu-id="56f03-428">Partner MPN e rivenditori indiretti CSP (non applicabili ai partner per la fatturazione diretta CSP)</span><span class="sxs-lookup"><span data-stu-id="56f03-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="56f03-429">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-429">Details</span></span>

<span data-ttu-id="56f03-430">A partire dal 2021 marzo, i partner MPN e i rivenditori indiretti CSP possono aggiornare il nome della società legale tramite il centro per i partner in modo conforme e autonomo.</span><span class="sxs-lookup"><span data-stu-id="56f03-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="56f03-431">Grazie a questa nuova funzionalità, i partner non dovranno più inviare un ticket di supporto per il centro per i partner per aggiornare il nome della società.</span><span class="sxs-lookup"><span data-stu-id="56f03-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="56f03-432">Ciò consentirà ai partner un notevole risparmio in termini di tempo per l'esecuzione di queste attività.</span><span class="sxs-lookup"><span data-stu-id="56f03-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="56f03-433">Per altre informazioni, vedere [aggiornare il profilo aziendale legale](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="56f03-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="56f03-434">Verificare che il nome della società nel profilo aziendale legale sia privo di errori di ortografia e abbreviazioni e corrisponda esattamente ai record di registrazione aziendali formali.</span><span class="sxs-lookup"><span data-stu-id="56f03-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="56f03-435">Per ulteriori informazioni sull'aggiornamento del profilo dell'organizzazione, fare riferimento a [verificare il profilo dell'organizzazione](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="56f03-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-436">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-436">Next steps</span></span>

<span data-ttu-id="56f03-437">Condividere queste informazioni all'interno dell'organizzazione in modo che il team appropriato possa rivedere e aggiornare i processi.</span><span class="sxs-lookup"><span data-stu-id="56f03-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-438">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-438">Questions?</span></span>

<span data-ttu-id="56f03-439">Per altre domande, consultare le community Yammer CSP pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="56f03-440">Aggiornamento all'evoluzione del programma Cloud Solution Provider (CSP) e alle modifiche al programma Open License</span><span class="sxs-lookup"><span data-stu-id="56f03-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-441">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-441">Categories</span></span>

- <span data-ttu-id="56f03-442">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="56f03-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="56f03-443">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-444">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-444">Summary</span></span>

<span data-ttu-id="56f03-445">Le nuove offerte software perpetue per il settore commerciale e pubblico sono in arrivo al programma Cloud Solution Provider (CSP) insieme alle modifiche apportate al programma di licenza Open.</span><span class="sxs-lookup"><span data-stu-id="56f03-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-446">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-446">Impacted audience</span></span>

<span data-ttu-id="56f03-447">Distributori commerciali e rivenditori gestiti che vendono attraverso il programma di licenza Open, nonché tutti i partner CSP che trasformano software perpetuo</span><span class="sxs-lookup"><span data-stu-id="56f03-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="56f03-448">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-448">Details</span></span>

<span data-ttu-id="56f03-449">Nel settembre 2020, Microsoft [ha annunciato](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) una serie di passaggi del processo di trasformazione digitale per ampliare le opportunità ai partner del programma CSP, inclusa la disponibilità di software locale per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="56f03-450">Queste modifiche consentono ai partner di far crescere la propria azienda ed estendere la propria copertura sfruttando le licenze software in CSP, inserendole in modo da avere successo nel mondo odierno.</span><span class="sxs-lookup"><span data-stu-id="56f03-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="56f03-451">Consentono inoltre di consentire ai clienti di passare al cloud e fornire ai partner la flessibilità necessaria per gli ambienti cloud ibridi del cliente.</span><span class="sxs-lookup"><span data-stu-id="56f03-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="56f03-452">Nella continuazione di questa trasformazione digitale sono state annunciate le modifiche seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="56f03-453">1 ° luglio 2021: non verranno aggiunti nuovi SKU, prodotti o promozioni al listino prezzi del programma Open License.</span><span class="sxs-lookup"><span data-stu-id="56f03-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="56f03-454">7 luglio 2021: due offerte commerciali, ottenere Windows e Visual Studio Professional originali e le offerte di settore pubblico (Government, Education e No [profit) verranno](./2020-december.md#9)aggiunte all'elenco dei prezzi software perpetuo CSP.</span><span class="sxs-lookup"><span data-stu-id="56f03-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="56f03-455">Il listino prezzi è disponibile nella sezione software della pagina [Sell > pricing & offers](https://partnercenter.microsoft.com/pcv/sales) nel centro per i partner e verrà ripubblicato a tale data.</span><span class="sxs-lookup"><span data-stu-id="56f03-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="56f03-456">Per informazioni dettagliate sull'evoluzione del programma CSP e sulle modifiche al programma Open License, vedere i **passaggi successivi** .</span><span class="sxs-lookup"><span data-stu-id="56f03-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-457">Passaggi successivi:</span><span class="sxs-lookup"><span data-stu-id="56f03-457">Next Steps:</span></span>

- <span data-ttu-id="56f03-458">Evoluzione del programma CSP: esaminare il [software perpetuo nei materiali di conformità del programma Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) .</span><span class="sxs-lookup"><span data-stu-id="56f03-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="56f03-459">Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.</span><span class="sxs-lookup"><span data-stu-id="56f03-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="56f03-460">Apri modifiche del programma di licenza: esaminare l' [evoluzione del programma CSP e i materiali di idoneità Open License changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) .</span><span class="sxs-lookup"><span data-stu-id="56f03-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="56f03-461">Usare questa [mappa di preparazione](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) per individuare rapidamente le informazioni adatte per il proprio ruolo.</span><span class="sxs-lookup"><span data-stu-id="56f03-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-462">Domande</span><span class="sxs-lookup"><span data-stu-id="56f03-462">Questions</span></span>

<span data-ttu-id="56f03-463">Per altre domande, consultare le community Yammer CSP pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="56f03-464">Aggiornamento a un annuncio precedente: valutazioni Premium, un componente aggiuntivo per Compliance Manager</span><span class="sxs-lookup"><span data-stu-id="56f03-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-465">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-465">Categories</span></span>

- <span data-ttu-id="56f03-466">Data: 2021-03-15</span><span class="sxs-lookup"><span data-stu-id="56f03-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="56f03-467">Espandi il business</span><span class="sxs-lookup"><span data-stu-id="56f03-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-468">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-468">Summary</span></span>

<span data-ttu-id="56f03-469">Le offerte di valutazione non dovrebbero essere elencate nell'elenco prezzi e verranno rimosse.</span><span class="sxs-lookup"><span data-stu-id="56f03-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-470">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-470">Impacted audience</span></span>

<span data-ttu-id="56f03-471">Partner che trasagiscono tramite Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="56f03-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="56f03-472">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-472">Details</span></span>

<span data-ttu-id="56f03-473">Le offerte di valutazione non dovrebbero essere state incluse nell'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="56f03-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="56f03-474">Questi verranno rimossi dall'elenco dei prezzi del 1 ° maggio 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="56f03-475">L'annuncio originale è [qui](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="56f03-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="56f03-476">Risorse aggiuntive</span><span class="sxs-lookup"><span data-stu-id="56f03-476">Additional resources</span></span>

- [<span data-ttu-id="56f03-477">Sicurezza e conformità di Microsoft 365 E5</span><span class="sxs-lookup"><span data-stu-id="56f03-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="56f03-478">Compilare e gestire valutazioni in Microsoft Compliance Manager-Microsoft 365 conformità</span><span class="sxs-lookup"><span data-stu-id="56f03-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="56f03-479">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-479">Next steps</span></span>

<span data-ttu-id="56f03-480">Vedere le risorse relative a questo argomento e condividerle con gli stakeholder appropriati nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-481">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-481">Questions?</span></span>

<span data-ttu-id="56f03-482">Per domande su queste offerte, consultare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="56f03-483">Esegui la migrazione delle tue soluzioni da un partner commerciale (OCP) go-to-Market (GTM) a Microsoft Commercial Marketplace</span><span class="sxs-lookup"><span data-stu-id="56f03-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-484">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-484">Categories</span></span>

- <span data-ttu-id="56f03-485">Data: 2021-03-12</span><span class="sxs-lookup"><span data-stu-id="56f03-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="56f03-486">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-487">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-487">Summary</span></span>

<span data-ttu-id="56f03-488">Dal 29 marzo 2021, si inizierà a provare a usare le funzionalità limitate di un partner commerciale (GTM).</span><span class="sxs-lookup"><span data-stu-id="56f03-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="56f03-489">Ti invitiamo a eseguire la migrazione delle tue soluzioni al Marketplace commerciale nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-490">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-490">Impacted audience</span></span>

<span data-ttu-id="56f03-491">Co-selling delle organizzazioni con soluzioni in OCP GTM</span><span class="sxs-lookup"><span data-stu-id="56f03-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="56f03-492">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-492">Details</span></span>

<span data-ttu-id="56f03-493">Nel dicembre 2020 abbiamo iniziato il nostro viaggio dallo strumento Microsoft OCP GTM a Microsoft Commercial Marketplace nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="56f03-494">Questa transizione espande le funzionalità del Marketplace commerciale, in cui è possibile presentare le soluzioni a milioni di clienti, condividere in modo bidirezionale le opportunità con altri venditori Microsoft e partner e vendere congiuntamente soluzioni innovative.</span><span class="sxs-lookup"><span data-stu-id="56f03-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="56f03-495">L'attività cardine successiva della transizione verrà eseguita il 29 marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="56f03-496">Questo è il momento in cui si iniziano a provare le funzionalità GTM OCP limitate, con alcuni campi che diventano di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="56f03-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="56f03-497">Se attualmente si condivide con le soluzioni in OCP GTM, si consiglia di eseguire la migrazione delle soluzioni al Marketplace commerciale per sfruttare le funzionalità e semplificare l'esperienza di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="56f03-498">Il passaggio al Marketplace commerciale rende il centro partner la destinazione principale per l'esperienza di pubblicazione di co-selling.</span><span class="sxs-lookup"><span data-stu-id="56f03-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="56f03-499">Puoi continuare a far crescere il tuo business connettendo le tue soluzioni con i nostri clienti condivisi attraverso gli stessi canali e le tue esperienze del prodotto usate per i prodotti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="56f03-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="56f03-500">[Scopri di più sul Marketplace commerciale](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="56f03-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-501">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-501">Next steps</span></span>

- <span data-ttu-id="56f03-502">Se non sono state ancora spostate le soluzioni, seguire le istruzioni riportate nella [Guida alla transizione](/azure/marketplace/co-sell-solution-migration) o visualizzare l'esercitazione dettagliata del [video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) per completare tutte le attività di migrazione e iniziare a pubblicare le soluzioni nel Marketplace commerciale.</span><span class="sxs-lookup"><span data-stu-id="56f03-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="56f03-503">Per domande sull'esperienza limitata in OCP GTM, vedere i [requisiti di co-selling per la pubblicazione nelle domande frequenti su Microsoft Commercial Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="56f03-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="56f03-504">Vedere la sezione "OCP GTM Limited capabilities a partire dal 29 marzo 2021".</span><span class="sxs-lookup"><span data-stu-id="56f03-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-505">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-505">Questions?</span></span>

<span data-ttu-id="56f03-506">Per eventuali domande o per richiedere ulteriori informazioni, contattare il [supporto tecnico](https://partner.microsoft.com/support/?stage=1) .</span><span class="sxs-lookup"><span data-stu-id="56f03-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="56f03-507">Ampliamento della nuova esperienza commerciale nel programma Cloud Solution Provider (CSP) per Azure in Russia</span><span class="sxs-lookup"><span data-stu-id="56f03-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-508">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-508">Categories</span></span>

- <span data-ttu-id="56f03-509">Data: 2021-03-10</span><span class="sxs-lookup"><span data-stu-id="56f03-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="56f03-510">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-511">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-511">Impacted audience</span></span>

<span data-ttu-id="56f03-512">Tutti i partner in Russia che operano attraverso il programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="56f03-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="56f03-513">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-513">Details</span></span>

<span data-ttu-id="56f03-514">A partire da marzo 10 2021, siamo lieti di annunciare la disponibilità della **nuova esperienza commerciale in CSP per Azure in Russia**.</span><span class="sxs-lookup"><span data-stu-id="56f03-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="56f03-515">Questa esperienza semplifica e migliora il modo in cui i clienti acquistano e utilizzano i servizi di Azure.</span><span class="sxs-lookup"><span data-stu-id="56f03-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="56f03-516">Fornirà inoltre ai partner del programma CSP una visualizzazione coerente dei prezzi di Azure tra i movimenti di vendita, i prezzi USD per la coerenza globale, l'allineamento della data di fatturazione e l'accesso a gestione costi di Azure.</span><span class="sxs-lookup"><span data-stu-id="56f03-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-517">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-517">Next steps</span></span>

<span data-ttu-id="56f03-518">Sono disponibili diverse risorse che introducono la nuova esperienza di Azure Commerce e forniscono informazioni aggiuntive.</span><span class="sxs-lookup"><span data-stu-id="56f03-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="56f03-519">Trovare le domande frequenti, i deck, i video e altro ancora più recenti nella [raccolta di risorse aggiornamenti del programma CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="56f03-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="56f03-520">Codice di licenza software per il centro per i partner e evasione del download</span><span class="sxs-lookup"><span data-stu-id="56f03-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-521">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-521">Categories</span></span>

- <span data-ttu-id="56f03-522">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="56f03-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="56f03-523">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-524">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-524">Summary</span></span>

<span data-ttu-id="56f03-525">Il download e la funzionalità di evasione delle chiavi di licenza del centro per i partner sono stati ripristinati.</span><span class="sxs-lookup"><span data-stu-id="56f03-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-526">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-526">Impacted audience</span></span>

<span data-ttu-id="56f03-527">Tutti i partner Cloud Solution Provider (CSP) che tramandano gli ordini software di abbonamento perpetuo e server tramite il centro per i partner</span><span class="sxs-lookup"><span data-stu-id="56f03-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="56f03-528">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-528">Details</span></span>

<span data-ttu-id="56f03-529">In risposta ai commenti dei partner, la funzionalità di evasione del centro per i partner viene ripristinare per ottenere il software e i codici di licenza per gli ordini software di abbonamento perpetuo e server.</span><span class="sxs-lookup"><span data-stu-id="56f03-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="56f03-530">Verrà ripristinato lo stato precedente prima di essere rimosso il 19 gennaio 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="56f03-531">Vedere l' [annuncio](2020-september.md#17).</span><span class="sxs-lookup"><span data-stu-id="56f03-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="56f03-532">Si noti che le chiavi di licenza software e i collegamenti di download sono asset di proprietà intellettuale preziosi e fortemente ricercati.</span><span class="sxs-lookup"><span data-stu-id="56f03-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="56f03-533">Se utenti malintenzionati ne entrassero in possesso, i limiti di attivazione previsti potrebbero venire raggiunti rapidamente, con conseguenti ripercussioni negative sull'esperienza di utilizzo per clienti e partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-534">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-534">Next steps</span></span>

<span data-ttu-id="56f03-535">Esaminare le risorse seguenti per istruzioni sull'utilizzo e indicazioni importanti sulla distribuzione di chiavi software:</span><span class="sxs-lookup"><span data-stu-id="56f03-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="56f03-536">Vendere software locale tramite il programma CSP</span><span class="sxs-lookup"><span data-stu-id="56f03-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="56f03-537">[Guida operativa di New Commerce](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) per il centro per i partner (vedere la sezione **linee guida sulla distribuzione di chiavi software** ).</span><span class="sxs-lookup"><span data-stu-id="56f03-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-538">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-538">Questions?</span></span>

<span data-ttu-id="56f03-539">In caso di ulteriori domande su questa comunicazione, consultare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="56f03-540">Esegui la migrazione delle tue offerte da partner Sales Connect (PSC) al centro per i partner</span><span class="sxs-lookup"><span data-stu-id="56f03-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-541">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-541">Categories</span></span>

- <span data-ttu-id="56f03-542">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="56f03-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="56f03-543">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-544">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-544">Summary</span></span>

<span data-ttu-id="56f03-545">Partner Sales Connect (PSC) passerà all'accesso in sola lettura a partire dal 31 marzo 2021, quindi si consiglia di iniziare la migrazione delle proprie offerte da CPS al centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-546">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-546">Impacted audience</span></span>

<span data-ttu-id="56f03-547">Partner con deals in PSC</span><span class="sxs-lookup"><span data-stu-id="56f03-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="56f03-548">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-548">Details</span></span>

<span data-ttu-id="56f03-549">Nell'ambito del nostro impegno condiviso verso la crescita, la **co-selling con Microsoft** è il percorso che ti permette di individuare **, offrire le tue competenze e ampliare il footprint dei clienti** per ottenere risultati positivi per i clienti.</span><span class="sxs-lookup"><span data-stu-id="56f03-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="56f03-550">Con una media di **3,5 volte più veloce** rispetto al normale, la gestione dell'esperienza di co-selling nel centro per i partner ti permette di vendere attraverso i canali diretti per clienti, partner e venditori Microsoft e di gestire l'intera pipeline di riferimento in un'unica posizione.</span><span class="sxs-lookup"><span data-stu-id="56f03-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="56f03-551">**PSC** passerà all' **accesso** in sola lettura a partire dal **31 marzo 2021**, quindi si consiglia di iniziare il passaggio al centro per i partner e accedere a questi miglioramenti delle funzionalità:</span><span class="sxs-lookup"><span data-stu-id="56f03-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="56f03-552">**Routing più accurato** delle offerte condivise con Microsoft al venditore appropriato, in base al tipo di assistenza necessario.</span><span class="sxs-lookup"><span data-stu-id="56f03-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="56f03-553">Ottenere in **anticipo la convalida dell'idoneità** per soluzioni idonee per gli incentivi e per soddisfare i criteri del programma di connessione ISV, semplificando il processo di approvazione e l'attestazione del certificato di esecuzione (PoE) finale.</span><span class="sxs-lookup"><span data-stu-id="56f03-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="56f03-554">**Esperienza utente trasparente** per gestire tutte le opportunità di co-selling e i lead qualificati per le vendite in un'unica posizione.</span><span class="sxs-lookup"><span data-stu-id="56f03-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="56f03-555">Sono state recentemente aggiunte nuove funzionalità al centro per i partner per facilitare lo spostamento:</span><span class="sxs-lookup"><span data-stu-id="56f03-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="56f03-556">Operazioni bulk per opportunità di co-selling</span><span class="sxs-lookup"><span data-stu-id="56f03-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="56f03-557">[Funzionalità di migrazione di Deal](../psc-to-pc.md) (vedere la sezione relativa alla **migrazione delle offerte di PSC** ).</span><span class="sxs-lookup"><span data-stu-id="56f03-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="56f03-558">Grazie all'esperienza di co-selling nel centro per i partner, i team addetti alle vendite avranno più tempo per concentrarsi sulla gestione di lead e opportunità, sulla chiusura di offerte e sulla creazione di relazioni dei clienti durevoli.</span><span class="sxs-lookup"><span data-stu-id="56f03-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="56f03-559">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-559">Next steps</span></span>

<span data-ttu-id="56f03-560">Usare la guida alla [transizione](../psc-to-pc.md) del centro per i partner per illustrare i passaggi necessari per eseguire la migrazione delle proprie offerte da CPS al centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="56f03-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-561">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-561">Questions?</span></span>

<span data-ttu-id="56f03-562">Per altre domande, contattare il [supporto tecnico](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="56f03-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="56f03-563">Nuovi prodotti e offerte Microsoft Dynamics 365 disponibili il 1 ° aprile 2021</span><span class="sxs-lookup"><span data-stu-id="56f03-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-564">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-564">Categories</span></span>

- <span data-ttu-id="56f03-565">Data: 2021-03-04</span><span class="sxs-lookup"><span data-stu-id="56f03-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="56f03-566">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-567">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-567">Summary</span></span>

<span data-ttu-id="56f03-568">Il 1 ° aprile 2021, Microsoft lancerà diversi nuovi prodotti e offerte per il programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="56f03-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-569">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-569">Impacted audience</span></span>

<span data-ttu-id="56f03-570">Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="56f03-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="56f03-571">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-571">Details</span></span>

<span data-ttu-id="56f03-572">Il 1 ° aprile 2021 Microsoft lancerà i nuovi prodotti e le offerte seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="56f03-573">Power BI Premium per utente</span><span class="sxs-lookup"><span data-stu-id="56f03-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="56f03-574">Area geografica ed espansione del segmento di Customer Voice and marketing USL</span><span class="sxs-lookup"><span data-stu-id="56f03-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="56f03-575">**Power BI Premium per utente**</span><span class="sxs-lookup"><span data-stu-id="56f03-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="56f03-576">Microsoft introdurrà le prime offerte per Power BI Premium per singolo utente.</span><span class="sxs-lookup"><span data-stu-id="56f03-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="56f03-577">Power BI Premium viene attualmente venduto solo in un costrutto di capacità.</span><span class="sxs-lookup"><span data-stu-id="56f03-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="56f03-578">Power BI Premium per utente consente di accedere alle funzionalità di Enterprise business intelligence (BI) e di analisi.</span><span class="sxs-lookup"><span data-stu-id="56f03-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="56f03-579">Le licenze flessibili per le singole postazioni si adattano alle aziende di piccole e medie dimensioni.</span><span class="sxs-lookup"><span data-stu-id="56f03-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="56f03-580">Per ulteriori informazioni su questa offerta, vedere i [Dettagli della versione Power bi](/power-platform-release-plan/2020wave2/power-bi/planned-features) .</span><span class="sxs-lookup"><span data-stu-id="56f03-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="56f03-581">**Dettagli dell'offerta**</span><span class="sxs-lookup"><span data-stu-id="56f03-581">**Offer details**</span></span>

<span data-ttu-id="56f03-582">Si noti che il nome dell'offerta è leggermente diverso dall'anteprima dell'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="56f03-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="56f03-583">Nome offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-583">Offer name</span></span> | <span data-ttu-id="56f03-584">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="56f03-585">Power BI Premium per utente</span><span class="sxs-lookup"><span data-stu-id="56f03-585">Power BI Premium Per User</span></span> | <span data-ttu-id="56f03-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="56f03-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="56f03-587">Power BI Premium per utente per i docenti</span><span class="sxs-lookup"><span data-stu-id="56f03-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="56f03-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="56f03-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="56f03-589">Power BI Premium per utente per studenti</span><span class="sxs-lookup"><span data-stu-id="56f03-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="56f03-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="56f03-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="56f03-591">Power BI Premium per utente (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="56f03-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="56f03-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="56f03-593">Power BI Premium per utente Add-On</span><span class="sxs-lookup"><span data-stu-id="56f03-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="56f03-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="56f03-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="56f03-595">Power BI Premium Add-On per utente per i docenti</span><span class="sxs-lookup"><span data-stu-id="56f03-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="56f03-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="56f03-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="56f03-597">Power BI Premium Add-On per ogni utente per studenti</span><span class="sxs-lookup"><span data-stu-id="56f03-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="56f03-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="56f03-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="56f03-599">Power BI Premium per Add-On utente (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="56f03-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="56f03-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="56f03-601">**Area geografica ed espansione del segmento di Customer Voice and marketing USL**</span><span class="sxs-lookup"><span data-stu-id="56f03-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="56f03-602">In seguito al lancio del dicembre 2020, le offerte di Dynamics 365 Customer Voice and marketing sono state modificate in modo da aggiungere nuovi paesi e SKU di formazione e non profit.</span><span class="sxs-lookup"><span data-stu-id="56f03-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="56f03-603">Nome offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-603">Offer name</span></span> | <span data-ttu-id="56f03-604">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="56f03-605">Dynamics 365 Customer Voice USL (prezzi per il personale non profit)</span><span class="sxs-lookup"><span data-stu-id="56f03-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="56f03-606">7a8642a5-481E-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="56f03-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="56f03-607">Dynamics 365 Customer Voice USL per istituti di facoltà</span><span class="sxs-lookup"><span data-stu-id="56f03-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="56f03-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="56f03-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="56f03-609">Per ulteriori informazioni su queste offerte, visitare le pagine seguenti:</span><span class="sxs-lookup"><span data-stu-id="56f03-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="56f03-610">home page Voice del servizio clienti Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="56f03-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="56f03-611">home page marketing di Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="56f03-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="56f03-612">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-612">Next steps</span></span>

<span data-ttu-id="56f03-613">Esaminare le risorse di questo argomento e condividere queste informazioni con le parti interessate appropriate nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="56f03-614">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-614">Questions?</span></span>

<span data-ttu-id="56f03-615">Per eventuali domande su queste offerte, consultare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="56f03-616">Microsoft Universal Print ora disponibile in alcuni gruppi</span><span class="sxs-lookup"><span data-stu-id="56f03-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="56f03-617">Categorie</span><span class="sxs-lookup"><span data-stu-id="56f03-617">Categories</span></span>

- <span data-ttu-id="56f03-618">Data: 2021-03-33</span><span class="sxs-lookup"><span data-stu-id="56f03-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="56f03-619">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="56f03-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="56f03-620">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="56f03-620">Summary</span></span>

<span data-ttu-id="56f03-621">Microsoft Universal Print sarà disponibile per le transazioni all'interno di Select Microsoft 365 suite e come componente aggiuntivo autonomo a partire dal 1 ° marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="56f03-622">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="56f03-622">Impacted audience</span></span>

<span data-ttu-id="56f03-623">Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="56f03-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="56f03-624">Dettagli</span><span class="sxs-lookup"><span data-stu-id="56f03-624">Details</span></span>

<span data-ttu-id="56f03-625">[Universal Print](https://aka.ms/universalprint) è un servizio di stampa Microsoft 365 che elimina la necessità di server di stampa locali e consente ai dispositivi Windows di stampare le stampanti registrate in Azure.</span><span class="sxs-lookup"><span data-stu-id="56f03-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="56f03-626">Sarà disponibile per le transazioni a partire dall'1 marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="56f03-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="56f03-627">I ruoli di lavoro traggono vantaggio dalla stampa senza driver, dall'individuazione di stampanti basata sulla posizione semplificata e da un'esperienza di stampa intuitiva senza alcuna curva di apprendimento.</span><span class="sxs-lookup"><span data-stu-id="56f03-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="56f03-628">I dispositivi aggiunti a Azure Active Directory (Azure AD) utilizzano le credenziali Azure AD esistenti per la stampa in modo sicuro.</span><span class="sxs-lookup"><span data-stu-id="56f03-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="56f03-629">Gli amministratori gestiscono la stampa tramite il portale di Azure e possono connettere facilmente le stampanti con supporto nativo per la stampa universale.</span><span class="sxs-lookup"><span data-stu-id="56f03-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="56f03-630">La stampa universale può essere distribuita con stampanti non compatibili utilizzando il software connettore di stampa universale.</span><span class="sxs-lookup"><span data-stu-id="56f03-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="56f03-631">La stampa universale verrà ricaricata in fase di avvio a Windows E3, a3, E5 e a5 e Microsoft 365 BP, F3, E3, a3, E5 e a5.</span><span class="sxs-lookup"><span data-stu-id="56f03-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="56f03-632">**Dettagli dell'offerta**</span><span class="sxs-lookup"><span data-stu-id="56f03-632">**Offer details**</span></span>

<span data-ttu-id="56f03-633">Si noti che il nome dell'offerta è leggermente diverso dall'anteprima dell'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="56f03-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="56f03-634">Nome offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-634">Offer name</span></span> | <span data-ttu-id="56f03-635">ID offerta</span><span class="sxs-lookup"><span data-stu-id="56f03-635">Offer ID</span></span> | <span data-ttu-id="56f03-636">ID materiale</span><span class="sxs-lookup"><span data-stu-id="56f03-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="56f03-637">Componente aggiuntivo volume di stampa universale (500 processi)-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="56f03-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="56f03-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="56f03-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="56f03-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="56f03-639">9BI-00004</span></span>   |
| <span data-ttu-id="56f03-640">Componente aggiuntivo volume di stampa universale (500 processi) per i docenti-Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="56f03-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="56f03-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="56f03-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="56f03-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="56f03-642">9BK-00004</span></span>   |
| <span data-ttu-id="56f03-643">Componente aggiuntivo volume di stampa universale (500 processi)-Windows</span><span class="sxs-lookup"><span data-stu-id="56f03-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="56f03-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="56f03-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="56f03-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="56f03-645">9BI-00002</span></span>   |
| <span data-ttu-id="56f03-646">Componente aggiuntivo volume di stampa universale (500 processi) per i docenti-Windows</span><span class="sxs-lookup"><span data-stu-id="56f03-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="56f03-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="56f03-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="56f03-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="56f03-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="56f03-649">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="56f03-649">Next steps</span></span>

<span data-ttu-id="56f03-650">Acquisire familiarità con l'elenco prezzi e la [Panoramica stampa universale](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="56f03-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="56f03-651">Si consiglia di condividere queste informazioni con tutti i contatti appropriati nella propria organizzazione.</span><span class="sxs-lookup"><span data-stu-id="56f03-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="56f03-652">Domande?</span><span class="sxs-lookup"><span data-stu-id="56f03-652">Questions?</span></span>

<span data-ttu-id="56f03-653">Per eventuali domande su queste offerte, consultare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="56f03-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
