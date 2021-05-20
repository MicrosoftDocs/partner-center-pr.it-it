---
title: Annunci di aprile 2021
description: Annunci di aprile 2021 per Microsoft Partner Center nuove funzionalità, promozioni, offerte, mercati o modifiche alle offerte esistenti.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 13b8ec9ddd82b38a265606809b8c39c07436e548
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150132"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="c75cc-103">Annunci di aprile 2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-103">April 2021 announcements</span></span>

<span data-ttu-id="c75cc-104">Questa pagina fornisce gli annunci per Microsoft Partner Center per aprile 2021.</span><span class="sxs-lookup"><span data-stu-id="c75cc-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="c75cc-105">Conformità: aggiornamento dell'API di convalida dell'indirizzo del cliente CSP in corso di validità a giugno; Funzionalità di test ora disponibile</span><span class="sxs-lookup"><span data-stu-id="c75cc-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-106">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-106">Categories</span></span>

- <span data-ttu-id="c75cc-107">Data: 2021-04-30</span><span class="sxs-lookup"><span data-stu-id="c75cc-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="c75cc-108">Preparazione</span><span class="sxs-lookup"><span data-stu-id="c75cc-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-109">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-109">Summary</span></span>

<span data-ttu-id="c75cc-110">Per consentire a partner e clienti di eseguire la propria attività in base alla fiducia, invitiamo i partner a testare le modifiche apportate all'API Convalida indirizzo per tutti i paesi di tutto il mondo.</span><span class="sxs-lookup"><span data-stu-id="c75cc-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-111">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-111">Impacted audience</span></span>

<span data-ttu-id="c75cc-112">Partner di fatturazione diretta CSP e provider indiretti che creano nuovi o aggiornano i dettagli dell'indirizzo dei clienti esistenti</span><span class="sxs-lookup"><span data-stu-id="c75cc-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-113">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-113">Details</span></span>

<span data-ttu-id="c75cc-114">Microsoft</span><span class="sxs-lookup"><span data-stu-id="c75cc-114">Microsoft runs on trust.</span></span> <span data-ttu-id="c75cc-115">Microsoft si impegna a fornire un metodo conforme, sicuro e sicuro per la convalida degli indirizzi dei clienti per la transazione delle sottoscrizioni dei clienti nel programma CSP.</span><span class="sxs-lookup"><span data-stu-id="c75cc-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="c75cc-116">A partire dal 31 marzo 2021 sono state introdotte modifiche all'API Convalida indirizzo.</span><span class="sxs-lookup"><span data-stu-id="c75cc-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="c75cc-117">I partner sono invitati a testare l'API prima del go-live alla fine di giugno 2021.</span><span class="sxs-lookup"><span data-stu-id="c75cc-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="c75cc-118">Si noti che queste modifiche influiscono solo sull'API Convalida indirizzo.</span><span class="sxs-lookup"><span data-stu-id="c75cc-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="c75cc-119">Le API Crea cliente e Aggiorna profilo di fatturazione non sono interessate.</span><span class="sxs-lookup"><span data-stu-id="c75cc-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="c75cc-120">Anche se l'indirizzo suggerito non deve attualmente essere usato con l'API Crea cliente, è altamente consigliato.</span><span class="sxs-lookup"><span data-stu-id="c75cc-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="c75cc-121">La risposta restituirà uno dei messaggi di stato seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="c75cc-122">Stato</span><span class="sxs-lookup"><span data-stu-id="c75cc-122">Status</span></span>     | <span data-ttu-id="c75cc-123">Descrizione</span><span class="sxs-lookup"><span data-stu-id="c75cc-123">Description</span></span> |    <span data-ttu-id="c75cc-124">Numero di indirizzi suggeriti restituiti</span><span class="sxs-lookup"><span data-stu-id="c75cc-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="c75cc-125">Shippable verificato</span><span class="sxs-lookup"><span data-stu-id="c75cc-125">Verified shippable</span></span> | <span data-ttu-id="c75cc-126">L'indirizzo viene verificato e può essere spedito.</span><span class="sxs-lookup"><span data-stu-id="c75cc-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="c75cc-127">Single</span><span class="sxs-lookup"><span data-stu-id="c75cc-127">Single</span></span> |
|<span data-ttu-id="c75cc-128">Verified</span><span class="sxs-lookup"><span data-stu-id="c75cc-128">Verified</span></span> | <span data-ttu-id="c75cc-129">L'indirizzo viene verificato.</span><span class="sxs-lookup"><span data-stu-id="c75cc-129">Address is verified.</span></span> | <span data-ttu-id="c75cc-130">Single</span><span class="sxs-lookup"><span data-stu-id="c75cc-130">Single</span></span> |
|<span data-ttu-id="c75cc-131">Interazione richiesta</span><span class="sxs-lookup"><span data-stu-id="c75cc-131">Interaction required</span></span> | <span data-ttu-id="c75cc-132">L'indirizzo suggerito è stato modificato in modo significativo e richiede la conferma dell'utente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="c75cc-133">Single</span><span class="sxs-lookup"><span data-stu-id="c75cc-133">Single</span></span> |
|<span data-ttu-id="c75cc-134">Via parziale</span><span class="sxs-lookup"><span data-stu-id="c75cc-134">Street partial</span></span> | <span data-ttu-id="c75cc-135">La via specificata nell'indirizzo è parziale e richiede altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="c75cc-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="c75cc-136">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="c75cc-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="c75cc-137">Locale parziale</span><span class="sxs-lookup"><span data-stu-id="c75cc-137">Premises partial</span></span> | <span data-ttu-id="c75cc-138">I locali (numero di edificio, numero di suite e altri) sono parziali e necessitano di altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="c75cc-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="c75cc-139">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="c75cc-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="c75cc-140">Multipli</span><span class="sxs-lookup"><span data-stu-id="c75cc-140">Multiple</span></span> | <span data-ttu-id="c75cc-141">Esistono più campi che sono parziali nell'indirizzo (potenzialmente includendo anche parziale strada e parziale locale).</span><span class="sxs-lookup"><span data-stu-id="c75cc-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="c75cc-142">Multiplo: massimo tre</span><span class="sxs-lookup"><span data-stu-id="c75cc-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="c75cc-143">Nessuno</span><span class="sxs-lookup"><span data-stu-id="c75cc-143">None</span></span> | <span data-ttu-id="c75cc-144">L'indirizzo non è corretto.</span><span class="sxs-lookup"><span data-stu-id="c75cc-144">Address is incorrect.</span></span> | <span data-ttu-id="c75cc-145">Nessuno</span><span class="sxs-lookup"><span data-stu-id="c75cc-145">None</span></span> |
|<span data-ttu-id="c75cc-146">Non convalidato</span><span class="sxs-lookup"><span data-stu-id="c75cc-146">Not validated</span></span> | <span data-ttu-id="c75cc-147">Impossibile inviare l'indirizzo tramite il processo di convalida.</span><span class="sxs-lookup"><span data-stu-id="c75cc-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="c75cc-148">Nessuno</span><span class="sxs-lookup"><span data-stu-id="c75cc-148">None</span></span> |

<span data-ttu-id="c75cc-149">I codici postali degli Stati Uniti restituiranno altre quattro cifre + trattino, ad esempio 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="c75cc-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-150">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-150">Next steps</span></span>

- <span data-ttu-id="c75cc-151">Per indicazioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella raccolta [partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dedicata.</span><span class="sxs-lookup"><span data-stu-id="c75cc-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="c75cc-152">Prepararsi a incorporare le modifiche usando l'API Partner Center e l'esperienza utente Web.</span><span class="sxs-lookup"><span data-stu-id="c75cc-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="c75cc-153">Condividere l'ID tenant della sandbox con l'esperto in materia (Ali Kpiki) da includere nel test, in modo da poter iniziare la preparazione per l'aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="c75cc-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="c75cc-154">Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.</span><span class="sxs-lookup"><span data-stu-id="c75cc-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-155">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-155">Questions?</span></span>

<span data-ttu-id="c75cc-156">Se è necessario supporto per le operazioni con Microsoft, contattare il gruppo yammer di supporto partner o aprire una richiesta [di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="c75cc-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="c75cc-157">Nuova posizione per la Partner Center di Swagger dell'API</span><span class="sxs-lookup"><span data-stu-id="c75cc-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-158">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-158">Categories</span></span>

- <span data-ttu-id="c75cc-159">Data: 26/04/2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="c75cc-160">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-161">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-161">Summary</span></span>

<span data-ttu-id="c75cc-162">Partner Center dei documenti Swagger dell'API sono stati migrati dal sito della [documentazione di Swagger](https://apidocs.microsoft.com/services/partnercenter) precedente a un [nuovo sito della documentazione di Swagger.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="c75cc-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-163">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-163">Impacted audience</span></span>

<span data-ttu-id="c75cc-164">Partner con fatturazione diretta e provider indiretti che partecipano al programma Cloud Solution Provider (CSP) che usano Partner Center API</span><span class="sxs-lookup"><span data-stu-id="c75cc-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-165">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-165">Details</span></span>

<span data-ttu-id="c75cc-166">A partire dal 26 aprile 2021 la documentazione di Swagger dell'API Partner Center, incluso il contenuto dell'API Rest, si trova in un [nuovo sito.](/rest/api/partner-center-rest/)</span><span class="sxs-lookup"><span data-stu-id="c75cc-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="c75cc-167">Il sito precedente sarà inaccessibile dopo diverse settimane.</span><span class="sxs-lookup"><span data-stu-id="c75cc-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="c75cc-168">Vantaggi</span><span class="sxs-lookup"><span data-stu-id="c75cc-168">Benefits</span></span>

<span data-ttu-id="c75cc-169">La documentazione Partner Center'API Swagger fornirà una **funzione Try It.**</span><span class="sxs-lookup"><span data-stu-id="c75cc-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="c75cc-170">Per usare questa funzione, è necessario disporre di un token di bearer, che è possibile generare seguendo i passaggi elencati in Partner Center [Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span><span class="sxs-lookup"><span data-stu-id="c75cc-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-171">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-171">Next steps</span></span>

<span data-ttu-id="c75cc-172">Condividere queste informazioni all'interno dell'organizzazione in modo che il team appropriato possa esaminare e aggiornare i processi.</span><span class="sxs-lookup"><span data-stu-id="c75cc-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-173">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-173">Questions?</span></span>

<span data-ttu-id="c75cc-174">Per domande su queste offerte, controllare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="c75cc-175">Cloud Solution Provider criteri del periodo di restituzione software (CSP) e avviso di scadenza del collegamento di download</span><span class="sxs-lookup"><span data-stu-id="c75cc-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-176">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-176">Categories</span></span>

- <span data-ttu-id="c75cc-177">Data: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="c75cc-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="c75cc-178">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-179">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-179">Summary</span></span>

<span data-ttu-id="c75cc-180">Sono state apportate modifiche ai criteri del periodo di restituzione del software CSP e alla scadenza del collegamento di download.</span><span class="sxs-lookup"><span data-stu-id="c75cc-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-181">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-181">Impacted audience</span></span>

<span data-ttu-id="c75cc-182">Partner che eselezionano offerte di sottoscrizione software o software perpetue in CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-183">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-183">Details</span></span>

<span data-ttu-id="c75cc-184">Si notino le notifiche importanti seguenti relative agli acquisti di sottoscrizioni software e software perpetue tramite Partner Center:</span><span class="sxs-lookup"><span data-stu-id="c75cc-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="c75cc-185">Criteri del periodo di restituzione software</span><span class="sxs-lookup"><span data-stu-id="c75cc-185">Software return period policy</span></span>

<span data-ttu-id="c75cc-186">A partire dal 1° giugno 2021, il periodo di restituzione delle offerte software in CSP, come indicato nel Contratto Microsoft Partner (MPA), cambierà da 60 giorni dalla data dell'ordine a 30 giorni dalla data dell'ordine.</span><span class="sxs-lookup"><span data-stu-id="c75cc-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="c75cc-187">Dopo l'invio di un ordine per un'offerta software, i partner avranno 30 giorni dalla data dell'ordine per inviare eventuali revisioni a tale ordine:</span><span class="sxs-lookup"><span data-stu-id="c75cc-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="c75cc-188">Qualsiasi licenza software perpetua restituita entro il periodo di restituzione di 30 giorni riceverà un credito completo del prezzo di acquisto a pagamento.</span><span class="sxs-lookup"><span data-stu-id="c75cc-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="c75cc-189">Qualsiasi prodotto di sottoscrizione software restituito entro il periodo di restituzione di 30 giorni riceverà un credito prorato del prezzo di acquisto a pagamento.</span><span class="sxs-lookup"><span data-stu-id="c75cc-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="c75cc-190">Questo messaggio è un follow-up delle comunicazioni di posta elettronica inviate il dicembre 2020 e aprile 2021 a tutti i partner CSP relativi al periodo di restituzione e ad altri aggiornamenti all'MPA.</span><span class="sxs-lookup"><span data-stu-id="c75cc-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="c75cc-191">Fare riferimento a tali avvisi per informazioni dettagliate complete sulle modifiche che interessano l'MPA.</span><span class="sxs-lookup"><span data-stu-id="c75cc-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="c75cc-192">Scadenza del collegamento di download software</span><span class="sxs-lookup"><span data-stu-id="c75cc-192">Software download link expiry</span></span>

<span data-ttu-id="c75cc-193">A partire dal 3 giugno 2021, i collegamenti di download software per gli acquisti di prodotti in sottoscrizione software e software perpetui tramite Partner Center avranno una data di scadenza di cinque giorni dal download iniziale.</span><span class="sxs-lookup"><span data-stu-id="c75cc-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="c75cc-194">Il periodo di scadenza verrà applicato a tutti gli acquisti prima del 3 giugno 2021, nonché il 3 giugno 2021 o dopo il 3 giugno 2021.</span><span class="sxs-lookup"><span data-stu-id="c75cc-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-195">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-195">Next steps</span></span>

<span data-ttu-id="c75cc-196">Esaminare il [periodo di restituzione CSP e le domande frequenti](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)sulla scadenza del collegamento di download e informare tutti i team appropriati all'interno dell'organizzazione delle modifiche seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-197">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-197">Questions?</span></span>

<span data-ttu-id="c75cc-198">Per domande su queste offerte, controllare le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="c75cc-199">Programma open licensing: transizione dei rivenditori al programma Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="c75cc-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-200">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-200">Categories</span></span>

- <span data-ttu-id="c75cc-201">Data: 2021-04-19</span><span class="sxs-lookup"><span data-stu-id="c75cc-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="c75cc-202">Far crescere l'azienda</span><span class="sxs-lookup"><span data-stu-id="c75cc-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-203">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-203">Summary</span></span>

<span data-ttu-id="c75cc-204">Questa comunicazione illustra in dettaglio come prepararsi per le modifiche che saranno presto disponibili nel programma Open Licensing.</span><span class="sxs-lookup"><span data-stu-id="c75cc-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-205">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-205">Impacted audience</span></span>

<span data-ttu-id="c75cc-206">Partner CSP e Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-207">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-207">Details</span></span>

<span data-ttu-id="c75cc-208">Nel 2020 [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) ha annunciato che le licenze software perpetue saranno disponibili a livello generale per partner e clienti tramite il programma Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="c75cc-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="c75cc-209">La prima attività cardine è stata raggiunta nel gennaio 2021, quando sono disponibili offerte software perpetue commerciali.</span><span class="sxs-lookup"><span data-stu-id="c75cc-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="c75cc-210">L'attività cardine successiva si avrà a luglio 2021, quando saranno disponibili [le](https://aka.ms/openlicensepublicsector) offerte del settore pubblico.</span><span class="sxs-lookup"><span data-stu-id="c75cc-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="c75cc-211">È [](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) stato anche comunicato che a partire dal 1° gennaio 2022 non è possibile effettuare nuovi acquisti o rinnovi di licenze software di Software Assurance o Servizi online tramite il programma Open License.</span><span class="sxs-lookup"><span data-stu-id="c75cc-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="c75cc-212">La transizione del software perpetuo al programma CSP nella nuova esperienza commerciale aiuterà i partner ad espandere le opportunità di offrire soluzioni e servizi gestiti diversi.</span><span class="sxs-lookup"><span data-stu-id="c75cc-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="c75cc-213">Ciò accelererà anche la transizione dei clienti al cloud.</span><span class="sxs-lookup"><span data-stu-id="c75cc-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="c75cc-214">Per garantire una transizione senza problemi sia per i partner che per i clienti, sono stati apportati questi adattamenti e materiali per accelerare questa trasformazione digitale:</span><span class="sxs-lookup"><span data-stu-id="c75cc-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="c75cc-215">Aprile 2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-215">April 2021</span></span>

<span data-ttu-id="c75cc-216">[Ora disponibile:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Materiali di transizione Open License-to-CSP per rivenditori</span><span class="sxs-lookup"><span data-stu-id="c75cc-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="c75cc-217">Luglio 2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="c75cc-218">CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-218">CSP</span></span>

- <span data-ttu-id="c75cc-219">1° luglio: licenze software perpetue disponibili per i clienti del settore pubblico</span><span class="sxs-lookup"><span data-stu-id="c75cc-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="c75cc-220">7 luglio: Visual Studio licenze software perpetue pro e get genuine del Contratto Windows disponibili per tutti i segmenti</span><span class="sxs-lookup"><span data-stu-id="c75cc-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="c75cc-221">Apri valore</span><span class="sxs-lookup"><span data-stu-id="c75cc-221">Open Value</span></span>

- <span data-ttu-id="c75cc-222">1 luglio: SKU aggiuntivi disponibili nel programma Open Value per la formazione e le organizzazioni no profit, offrendo offerte simili al programma Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="c75cc-223">Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-223">Open License</span></span>

- <span data-ttu-id="c75cc-224">1 luglio: Microsoft non avvierà più nuove offerte nel programma Open License.</span><span class="sxs-lookup"><span data-stu-id="c75cc-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="c75cc-225">Gennaio 2022</span><span class="sxs-lookup"><span data-stu-id="c75cc-225">January 2022</span></span>

- <span data-ttu-id="c75cc-226">1 gennaio: non è possibile effettuare nuovi acquisti o rinnovi tramite il programma Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-227">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="c75cc-228">Provider indiretti CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-228">CSP indirect providers</span></span>

<span data-ttu-id="c75cc-229">Usare i prossimi mesi per aiutare i rivenditori Open License a orientarsi nel programma CSP partecipando agli eventi della community dei partner e usando i materiali di transizione Open License-to-CSP per i rivenditori:</span><span class="sxs-lookup"><span data-stu-id="c75cc-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="c75cc-230">Open [License-to-CSP transition](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)materials for resellers (Materiale per la transizione da licenza a CSP aperta per i rivenditori): presentazione panoramica personalizzabile, modello di posta elettronica, guida all'onboarding dei rivenditori indiretti CSP e altro ancora per facilitare l'adozione per i rivenditori su larga scala.</span><span class="sxs-lookup"><span data-stu-id="c75cc-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="c75cc-231">[Eventi della community dei partner CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) ospitati da Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="c75cc-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="c75cc-232">Partecipare alle varie sessioni per apprendere le nozioni di base di CSP (Nozioni fondamentali su CSP) o rimanere aggiornati e porre domande relative al software in CSP (Q&A Sessions).</span><span class="sxs-lookup"><span data-stu-id="c75cc-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="c75cc-233">(Presto disponibili) Sessione di formazione incentrata sui rivenditori indiretti CSP ospitata da Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="c75cc-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="c75cc-234">Rivenditori Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-234">Open License resellers</span></span>

- <span data-ttu-id="c75cc-235">Se l'organizzazione non è attualmente iscritta al programma CSP, contattare il distributore per informazioni su come iniziare.</span><span class="sxs-lookup"><span data-stu-id="c75cc-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="c75cc-236">Connettersi con un provider indiretto [qui](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="c75cc-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="c75cc-237">Se l'organizzazione è già iscritta al programma CSP, vedere qui per altre informazioni sul software perpetuo in [CSP.](https://partner.microsoft.com/resources/collection/software-in-csp)</span><span class="sxs-lookup"><span data-stu-id="c75cc-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-238">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-238">Questions?</span></span>

<span data-ttu-id="c75cc-239">Per altre domande su queste offerte, vedere le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="c75cc-240">Now live: Global promo readiness guide (Guida all'idoneità per le promo globali)</span><span class="sxs-lookup"><span data-stu-id="c75cc-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-241">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-241">Categories</span></span>

- <span data-ttu-id="c75cc-242">Data: 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="c75cc-243">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-244">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-244">Summary</span></span>

<span data-ttu-id="c75cc-245">Launch Readiness ha pubblicato una nuova [guida all'idoneità per la promo globale](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) nella raccolta di risorse per l'idoneità per le operazioni.</span><span class="sxs-lookup"><span data-stu-id="c75cc-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="c75cc-246">Questa guida offre una visualizzazione consolidata di tutte le [promozioni globali attive.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)</span><span class="sxs-lookup"><span data-stu-id="c75cc-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-247">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-247">Impacted audience</span></span>

<span data-ttu-id="c75cc-248">Tutti i partner volume licensing (VL), Dynamics Price List (DPL) e Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="c75cc-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-249">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-249">Details</span></span>

<span data-ttu-id="c75cc-250">I partner Microsoft hanno condiviso con Microsoft la necessità di fornire una visualizzazione consolidata di tutte le promozioni globali con i dettagli di supporto.</span><span class="sxs-lookup"><span data-stu-id="c75cc-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="c75cc-251">Si desiderava che questa guida consolidata aiuta a usare le promozioni con la certezza che tutte le informazioni disponibili saranno facilmente accessibili in una posizione centrale e comoda.</span><span class="sxs-lookup"><span data-stu-id="c75cc-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="c75cc-252">A partire da aprile 2021, Microsoft aggiornerà questa guida su base mensile e sarà disponibile in una raccolta di guide alla preparazione della terapia globale dedicata nella raccolta di risorse preparazione operazioni.</span><span class="sxs-lookup"><span data-stu-id="c75cc-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="c75cc-253">I collegamenti a questa guida verranno inclusi anche nelle raccolte seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="c75cc-254">[Avviare la raccolta di](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)calendari , che offre una visualizzazione centralizzata delle modifiche e dei lanci imminenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="c75cc-255">[Raccolte della](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)community, che contengono materiale di supporto per le chiamate mensili dei partner, evidenziando le modifiche imminenti e gli argomenti di interesse operativo.</span><span class="sxs-lookup"><span data-stu-id="c75cc-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="c75cc-256">[Newsletter per i partner,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)ad esempio l'aggiornamento mensile CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="c75cc-257">Come promemoria mensile, pubblicheremo anche un annuncio Partner Center con ogni nuovo numero della guida alla preparazione della descrizione globale.</span><span class="sxs-lookup"><span data-stu-id="c75cc-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-258">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-258">Next steps</span></span>

<span data-ttu-id="c75cc-259">All'inizio di ogni mese, è possibile trovare la guida più recente alla preparazione [delle promo](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) globali nella raccolta di risorse [di Conformità alle operazioni](https://partner.microsoft.com/resources).</span><span class="sxs-lookup"><span data-stu-id="c75cc-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="c75cc-260">Condividere queste informazioni con i contatti appropriati all'interno dell'organizzazione e indicarci quanto sia utile la guida tramite il messaggio "Questa pagina è stata utile?"</span><span class="sxs-lookup"><span data-stu-id="c75cc-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="c75cc-261">alla fine di ogni pagina.</span><span class="sxs-lookup"><span data-stu-id="c75cc-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="c75cc-262">Aggiornamento e promemoria della community di Cloud Solution Provider (CSP) di aprile</span><span class="sxs-lookup"><span data-stu-id="c75cc-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-263">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-263">Categories</span></span>

- <span data-ttu-id="c75cc-264">Data: 2021-04-16</span><span class="sxs-lookup"><span data-stu-id="c75cc-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="c75cc-265">Community | Inviti e promemoria</span><span class="sxs-lookup"><span data-stu-id="c75cc-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-266">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-266">Summary</span></span>

<span data-ttu-id="c75cc-267">Le risorse della community CSP sono disponibili su richiesta e aggiornate mensilmente per tenervi informati e preparati per il cambiamento nel programma CSP.</span><span class="sxs-lookup"><span data-stu-id="c75cc-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-268">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-268">Impacted audience</span></span>

<span data-ttu-id="c75cc-269">Partner di fatturazione diretta CSP e provider indiretti</span><span class="sxs-lookup"><span data-stu-id="c75cc-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-270">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-270">Details</span></span>

<span data-ttu-id="c75cc-271">Questo mese, le risorse includono gli argomenti chiave seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="c75cc-272">Aggiornamento all'evoluzione del programma CSP e modifiche al programma Open License</span><span class="sxs-lookup"><span data-stu-id="c75cc-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="c75cc-273">Modifiche ai requisiti di onboarding dei clienti CSP in determinate aree</span><span class="sxs-lookup"><span data-stu-id="c75cc-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="c75cc-274">Nuovo formato per la nuova fattura pdf commerciale nel programma CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="c75cc-275">[All'interno della raccolta della community CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)sono presenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="c75cc-276">La newsletter di aggiornamento mensile [CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)scaricabile, che aggrega annunci, aggiornamenti, eventi e promemoria CSP recenti in un documento di facile lettura.</span><span class="sxs-lookup"><span data-stu-id="c75cc-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="c75cc-277">Calendario [degli annunci CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)che offre una visualizzazione temporale delle modifiche imminenti che interessano il programma.</span><span class="sxs-lookup"><span data-stu-id="c75cc-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="c75cc-278">Il nuovo [calendario di lancio del](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)prodotto, in cui è possibile visualizzare i prossimi lanci di prodotti e offerte.</span><span class="sxs-lookup"><span data-stu-id="c75cc-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="c75cc-279">[Il provider di servizi di configurazione avvia le](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) risorse di aggiornamento con contenuti facili da usare in base alle principali modifiche operative.</span><span class="sxs-lookup"><span data-stu-id="c75cc-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="c75cc-280">[Aggiornamenti e promemoria su](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) argomenti CSP chiave che ricevono interesse e query.</span><span class="sxs-lookup"><span data-stu-id="c75cc-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="c75cc-281">CSP Community Call Q&As</span><span class="sxs-lookup"><span data-stu-id="c75cc-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="c75cc-282">Sono disponibili&domande frequenti sulla chiamata della community per rispondere alle domande relative alle modifiche imminenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="c75cc-283">Registrarsi ora per il programma CSP Community Call Q&che si stanno verificando nei mesi di aprile, maggio e giugno.</span><span class="sxs-lookup"><span data-stu-id="c75cc-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="c75cc-284">Queste informazioni saranno incentrate sui lanci più recenti, sugli aggiornamenti importanti e sui promemoria.</span><span class="sxs-lookup"><span data-stu-id="c75cc-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="c75cc-285">[Registrarsi qui](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span><span class="sxs-lookup"><span data-stu-id="c75cc-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-286">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-286">Next steps</span></span>

<span data-ttu-id="c75cc-287">Esaminare le risorse della community e registrarsi per la chiamata alla community Q&A.</span><span class="sxs-lookup"><span data-stu-id="c75cc-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="c75cc-288">Per ottenere il massimo dalla chiamata alla community Q&A, esaminare il contenuto della community su richiesta e inviare le domande fino a 48 ore prima della chiamata.</span><span class="sxs-lookup"><span data-stu-id="c75cc-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-289">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-289">Questions?</span></span>

<span data-ttu-id="c75cc-290">Il piano mensile CSP Community Call Q&A è il posto migliore per le domande relative alle modifiche apportate al programma CSP.</span><span class="sxs-lookup"><span data-stu-id="c75cc-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="c75cc-291">Ogni mese esaminare il materiale e inviare le domande in anticipo in modo da poter dedicare la sessione agli argomenti più importanti per l'utente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="c75cc-292">Per altre informazioni, contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span><span class="sxs-lookup"><span data-stu-id="c75cc-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="c75cc-293">Promemoria finale: Deprecazione della qualificazione GET il 6 maggio 2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-294">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-294">Categories</span></span>

- <span data-ttu-id="c75cc-295">Data: 04/05/2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="c75cc-296">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-297">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-297">Impacted audience</span></span>

<span data-ttu-id="c75cc-298">Partner che vendono offerte Academic, No profit e Government Community Cloud (GCC) tramite il programma Cloud Solution Provider usando l'API Partner Center</span><span class="sxs-lookup"><span data-stu-id="c75cc-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-299">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-299">Details</span></span>

<span data-ttu-id="c75cc-300">Questo annuncio è un follow-up delle Partner Center [miglioramenti rilasciati a dicembre.](./2020-december.md#1)</span><span class="sxs-lookup"><span data-stu-id="c75cc-300">This announcement is a follow-up to the Partner Center [enhancements released in December](./2020-december.md#1).</span></span> <span data-ttu-id="c75cc-301">Come parte di tale versione, sono state distribuite nuove API di qualifica GET e POST e, di conseguenza, la qualifica GET esistente verrà ritirata il 6 maggio **2021.**</span><span class="sxs-lookup"><span data-stu-id="c75cc-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="c75cc-302">A questo punto, sarà necessario eseguire la transizione all'uso del nuovo POST Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="c75cc-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="c75cc-303">Le nuove API POST consentono di acquistare offerte Education, mentre le nuove API GET consentono di acquistare offerte non profit e GCC pre-qualificate.</span><span class="sxs-lookup"><span data-stu-id="c75cc-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-304">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-304">Next steps</span></span>

- <span data-ttu-id="c75cc-305">**Eseguire l'aggiornamento alle nuove API per** una transizione corretta e temporale.</span><span class="sxs-lookup"><span data-stu-id="c75cc-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="c75cc-306">**Esaminare le nuove modifiche Partner Center'API** e la Guida nelle risorse conformità alle operazioni: Partner Center miglioramenti del processo di convalida dei clienti [di Education.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)</span><span class="sxs-lookup"><span data-stu-id="c75cc-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="c75cc-307">Condividere queste informazioni con i team appropriati all'interno dell'organizzazione e con i rivenditori per prepararsi a queste modifiche.</span><span class="sxs-lookup"><span data-stu-id="c75cc-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-308">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-308">Questions?</span></span>

<span data-ttu-id="c75cc-309">Per eventuali domande correlate a questa notifica, contattare il [supporto Partner Center .](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)</span><span class="sxs-lookup"><span data-stu-id="c75cc-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="c75cc-310">Registro delle modifiche</span><span class="sxs-lookup"><span data-stu-id="c75cc-310">Change log</span></span>

- <span data-ttu-id="c75cc-311">4 maggio 2021: promemoria finale dell'imminente deprecazione della qualifica GET</span><span class="sxs-lookup"><span data-stu-id="c75cc-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="c75cc-312">9 aprile 2021: promemoria dell'imminente deprecazione della qualifica GET</span><span class="sxs-lookup"><span data-stu-id="c75cc-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="c75cc-313">Febbraio: sono state aggiornate le sequenze temporali per la deprecazione delle & PUT GET</span><span class="sxs-lookup"><span data-stu-id="c75cc-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="c75cc-314">Gennaio: promemoria delle prossime deprecazioni delle & PUT GET</span><span class="sxs-lookup"><span data-stu-id="c75cc-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="c75cc-315">Nuovo formato per la nuova fattura PDF commerciale in CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-316">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-316">Categories</span></span>

- <span data-ttu-id="c75cc-317">Data: 2021-04-05</span><span class="sxs-lookup"><span data-stu-id="c75cc-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="c75cc-318">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-319">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-319">Summary</span></span>

<span data-ttu-id="c75cc-320">Microsoft sta introducendo un nuovo formato per la nuova fattura PDF commerciale nel programma Cloud Solution Provider (CSP) per visualizzare i dettagli di fatturazione in base ai dettagli del prodotto anziché alla descrizione dello SKU.</span><span class="sxs-lookup"><span data-stu-id="c75cc-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-321">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-321">Impacted audience</span></span>

<span data-ttu-id="c75cc-322">Partner che eseguono transazioni tramite il programma CSP</span><span class="sxs-lookup"><span data-stu-id="c75cc-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-323">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-323">Details</span></span>

<span data-ttu-id="c75cc-324">A partire da maggio 2021, Microsoft introduce un nuovo formato per la nuova fattura PDF commerciale nel programma CSP per visualizzare i dettagli di fatturazione in base ai dettagli del prodotto anziché alla descrizione dello SKU.</span><span class="sxs-lookup"><span data-stu-id="c75cc-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="c75cc-325">Con questo nuovo aggiornamento, le voci verranno aggregate per tipo di prodotto, visualizzando ogni prodotto in una singola riga.</span><span class="sxs-lookup"><span data-stu-id="c75cc-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="c75cc-326">I partner noteranno che questa modifica sarà effettiva nella fattura di maggio per il periodo di fatturazione compreso tra il 1° aprile 2021 e il 30 aprile 2021.</span><span class="sxs-lookup"><span data-stu-id="c75cc-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="c75cc-327">Le offerte interessate sono Microsoft Azure,sottoscrizioni di Azure (piano di Azure) e Marketplace.</span><span class="sxs-lookup"><span data-stu-id="c75cc-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="c75cc-328">Tutte le richieste di nuova fattura effettuate dopo l'aggiornamento del formato della fattura verranno generate nel nuovo formato.</span><span class="sxs-lookup"><span data-stu-id="c75cc-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="c75cc-329">Vantaggi per i partner</span><span class="sxs-lookup"><span data-stu-id="c75cc-329">Partner benefits</span></span>

<span data-ttu-id="c75cc-330">Questo aggiornamento offrirà i miglioramenti seguenti all'esperienza di fatturazione per i partner:</span><span class="sxs-lookup"><span data-stu-id="c75cc-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="c75cc-331">Riduzione delle dimensioni della fattura mantenendo i dati critici</span><span class="sxs-lookup"><span data-stu-id="c75cc-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="c75cc-332">Allineamento del formato agli standard del settore per le fatture compatte e di facile utilizzo</span><span class="sxs-lookup"><span data-stu-id="c75cc-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="c75cc-333">Gli elementi seguenti non saranno interessati:</span><span class="sxs-lookup"><span data-stu-id="c75cc-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="c75cc-334">Pagina di riepilogo della fatturazione nel PDF della fattura</span><span class="sxs-lookup"><span data-stu-id="c75cc-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="c75cc-335">API di fatturazione esistenti</span><span class="sxs-lookup"><span data-stu-id="c75cc-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="c75cc-336">File di riconciliazione (i file di riconciliazione possono essere usati per il recupero di dati granulari).</span><span class="sxs-lookup"><span data-stu-id="c75cc-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="c75cc-337">Fatture per l'utilizzo e gli addebiti basati su licenza</span><span class="sxs-lookup"><span data-stu-id="c75cc-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-338">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-338">Next steps</span></span>

<span data-ttu-id="c75cc-339">Esaminare le informazioni su questo argomento nella raccolta di risorse [per l'idoneità per le](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) operazioni nel sito Web dei partner Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c75cc-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="c75cc-340">Per altre informazioni su fatturazione e imposte, tra cui risorse di fatturazione, fatture, fatturazione CSP e imposte, vedere la sezione [Fatturazione](../billing.md) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c75cc-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](../billing.md) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="c75cc-341">Modifiche apportate ai requisiti di onboarding dei clienti Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="c75cc-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-342">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-342">Categories</span></span>

- <span data-ttu-id="c75cc-343">Data: 02/04/2021</span><span class="sxs-lookup"><span data-stu-id="c75cc-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="c75cc-344">Offerte/mercati</span><span class="sxs-lookup"><span data-stu-id="c75cc-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="c75cc-345">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-345">Summary</span></span>

<span data-ttu-id="c75cc-346">Nell'ambito dell'impegno per aiutare partner e clienti a eseguire la propria attività in base alla fiducia, microsoft richiederà informazioni aggiuntive sui clienti a partire dal 25 marzo 2021.</span><span class="sxs-lookup"><span data-stu-id="c75cc-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-347">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-347">Impacted audience</span></span>

<span data-ttu-id="c75cc-348">I provider indiretti e i partner con fatturazione diretta CSP con clienti nuovi o esistenti nei paesi elencati nella sezione successiva</span><span class="sxs-lookup"><span data-stu-id="c75cc-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-349">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-349">Details</span></span>

<span data-ttu-id="c75cc-350">Microsoft</span><span class="sxs-lookup"><span data-stu-id="c75cc-350">Microsoft runs on trust.</span></span> <span data-ttu-id="c75cc-351">si impegna a fornire un metodo di convalida dei clienti conforme e sicuro per la vendita di sottoscrizioni cliente nel programma CSP.</span><span class="sxs-lookup"><span data-stu-id="c75cc-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="c75cc-352">Il 25 marzo 2021 verranno introdotti miglioramenti all'API Partner Center e all'interfaccia utente che influiranno sui partner che soddisfano entrambi i criteri seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="c75cc-353">Il partner ha una relazione di fatturazione diretta con Microsoft (ovvero, è un partner con fatturazione diretta o un provider indiretto).</span><span class="sxs-lookup"><span data-stu-id="c75cc-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="c75cc-354">Il partner opera con clienti nuovi o esistenti nei paesi seguenti:</span><span class="sxs-lookup"><span data-stu-id="c75cc-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="c75cc-355">Thailandia</span><span class="sxs-lookup"><span data-stu-id="c75cc-355">Thailand</span></span>
    - <span data-ttu-id="c75cc-356">Vietnam</span><span class="sxs-lookup"><span data-stu-id="c75cc-356">Vietnam</span></span>
    - <span data-ttu-id="c75cc-357">Turchia</span><span class="sxs-lookup"><span data-stu-id="c75cc-357">Turkey</span></span>
    - <span data-ttu-id="c75cc-358">Polonia</span><span class="sxs-lookup"><span data-stu-id="c75cc-358">Poland</span></span>
    - <span data-ttu-id="c75cc-359">Sud Africa</span><span class="sxs-lookup"><span data-stu-id="c75cc-359">South Africa</span></span>
    - <span data-ttu-id="c75cc-360">India</span><span class="sxs-lookup"><span data-stu-id="c75cc-360">India</span></span>
    - <span data-ttu-id="c75cc-361">Brasile</span><span class="sxs-lookup"><span data-stu-id="c75cc-361">Brazil</span></span>
    - <span data-ttu-id="c75cc-362">Iraq</span><span class="sxs-lookup"><span data-stu-id="c75cc-362">Iraq</span></span>
    - <span data-ttu-id="c75cc-363">Myanmar</span><span class="sxs-lookup"><span data-stu-id="c75cc-363">Myanmar</span></span>
    - <span data-ttu-id="c75cc-364">Sud Sudan</span><span class="sxs-lookup"><span data-stu-id="c75cc-364">South Sudan</span></span>
    - <span data-ttu-id="c75cc-365">Arabia Saudita</span><span class="sxs-lookup"><span data-stu-id="c75cc-365">Saudi Arabia</span></span>
    - <span data-ttu-id="c75cc-366">Emirati Arabi Uniti</span><span class="sxs-lookup"><span data-stu-id="c75cc-366">United Arab Emirates</span></span>
    - <span data-ttu-id="c75cc-367">Venezuela</span><span class="sxs-lookup"><span data-stu-id="c75cc-367">Venezuela</span></span>

<span data-ttu-id="c75cc-368">I partner che soddisfano i criteri doranno inviare l'ID registrazione aziendale di un cliente (noto anche come INN dell'organizzazione del cliente) e il numero di telefono al successivo aggiornamento o creazione di una sottoscrizione per tale cliente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="c75cc-369">I partner possono anche immettere un secondo nome facoltativo per il cliente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="c75cc-370">Si noti che quando si aggiunge l'ID registrazione aziendale, è necessario usare l'ID imposta aziendale e non l'ID personale del cliente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="c75cc-371">I partner che svolgono attività con clienti nuovi o esistenti nei paesi seguenti hanno già eseguito l'onboarding di una versione precedente a novembre 2020.</span><span class="sxs-lookup"><span data-stu-id="c75cc-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="c75cc-372">Armenia</span><span class="sxs-lookup"><span data-stu-id="c75cc-372">Armenia</span></span>
- <span data-ttu-id="c75cc-373">Azerbaigian</span><span class="sxs-lookup"><span data-stu-id="c75cc-373">Azerbaijan</span></span>
- <span data-ttu-id="c75cc-374">Bielorussia</span><span class="sxs-lookup"><span data-stu-id="c75cc-374">Belarus</span></span>
- <span data-ttu-id="c75cc-375">Ungheria</span><span class="sxs-lookup"><span data-stu-id="c75cc-375">Hungary</span></span>
- <span data-ttu-id="c75cc-376">Kazakhstan</span><span class="sxs-lookup"><span data-stu-id="c75cc-376">Kazakhstan</span></span>
- <span data-ttu-id="c75cc-377">Kirghizistan</span><span class="sxs-lookup"><span data-stu-id="c75cc-377">Kyrgyzstan</span></span>
- <span data-ttu-id="c75cc-378">Moldova</span><span class="sxs-lookup"><span data-stu-id="c75cc-378">Moldova</span></span>
- <span data-ttu-id="c75cc-379">Russia</span><span class="sxs-lookup"><span data-stu-id="c75cc-379">Russia</span></span>
- <span data-ttu-id="c75cc-380">Tagikistan</span><span class="sxs-lookup"><span data-stu-id="c75cc-380">Tajikistan</span></span>
- <span data-ttu-id="c75cc-381">Ucraina</span><span class="sxs-lookup"><span data-stu-id="c75cc-381">Ukraine</span></span>
- <span data-ttu-id="c75cc-382">Uzbekistan</span><span class="sxs-lookup"><span data-stu-id="c75cc-382">Uzbekistan</span></span>

<span data-ttu-id="c75cc-383">I partner con clienti nel resto del mondo avranno la possibilità di immettere l'ID di registrazione della società, il numero di telefono e il secondo nome per i clienti come dettagli facoltativi.</span><span class="sxs-lookup"><span data-stu-id="c75cc-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-384">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-384">Next steps</span></span>

- <span data-ttu-id="c75cc-385">Per istruzioni più dettagliate, vedere la documentazione tecnica e le domande frequenti nella [raccolta dedicata ai partner](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/).</span><span class="sxs-lookup"><span data-stu-id="c75cc-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="c75cc-386">Prepararsi ad adottare le modifiche usando l'API del Centro per i partner e l'esperienza utente Web.</span><span class="sxs-lookup"><span data-stu-id="c75cc-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="c75cc-387">Saranno disponibili API e SDK a scopo di test.</span><span class="sxs-lookup"><span data-stu-id="c75cc-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="c75cc-388">Assicurarsi di inviare i dati aggiuntivi quando si caricano nuovi clienti o si modificano i dettagli del cliente esistente.</span><span class="sxs-lookup"><span data-stu-id="c75cc-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="c75cc-389">Se si usa la soluzione di un fornitore del pannello di controllo (CPV), rivolgersi a tale fornitore.</span><span class="sxs-lookup"><span data-stu-id="c75cc-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="c75cc-390">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-390">Questions?</span></span>

<span data-ttu-id="c75cc-391">Contattare l'assistente fiscale o l'ufficio fiscale locale per eventuali domande relative all'ID di registrazione dell'azienda (detto anche INN o TIN).</span><span class="sxs-lookup"><span data-stu-id="c75cc-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="c75cc-392">Microsoft non è in grado di fornire indicazioni sulle imposte.</span><span class="sxs-lookup"><span data-stu-id="c75cc-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="c75cc-393">Se è necessario supporto per le operazioni con Microsoft, aprire una richiesta [di servizio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="c75cc-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="c75cc-394">Visualizzare i lanci e le offerte del prodotto di questo mese</span><span class="sxs-lookup"><span data-stu-id="c75cc-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="c75cc-395">Categorie</span><span class="sxs-lookup"><span data-stu-id="c75cc-395">Categories</span></span>

- <span data-ttu-id="c75cc-396">Data: 2021-04-01</span><span class="sxs-lookup"><span data-stu-id="c75cc-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="c75cc-397">Funzionalità</span><span class="sxs-lookup"><span data-stu-id="c75cc-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="c75cc-398">Riepilogo</span><span class="sxs-lookup"><span data-stu-id="c75cc-398">Summary</span></span>

<span data-ttu-id="c75cc-399">Il calendario di lancio del prodotto di aprile 2021 è ora pubblicato.</span><span class="sxs-lookup"><span data-stu-id="c75cc-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="c75cc-400">Destinatari interessati</span><span class="sxs-lookup"><span data-stu-id="c75cc-400">Impacted audience</span></span>

<span data-ttu-id="c75cc-401">Tutti i partner che eseguono transazioni tramite il programma Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="c75cc-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="c75cc-402">Dettagli</span><span class="sxs-lookup"><span data-stu-id="c75cc-402">Details</span></span>

<span data-ttu-id="c75cc-403">Il calendario di lancio del prodotto [di](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) aprile 2021 è ora disponibile nella raccolta di risorse conformità alle operazioni.</span><span class="sxs-lookup"><span data-stu-id="c75cc-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="c75cc-404">Vedere i prossimi lanci e offerte del prodotto qui.</span><span class="sxs-lookup"><span data-stu-id="c75cc-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="c75cc-405">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c75cc-405">Next steps</span></span>

<span data-ttu-id="c75cc-406">Esaminare il [calendario di lancio del](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)prodotto e condividere le informazioni con gli stakeholder appropriati nell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="c75cc-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="c75cc-407">Domande?</span><span class="sxs-lookup"><span data-stu-id="c75cc-407">Questions?</span></span>

<span data-ttu-id="c75cc-408">Per altre domande su queste offerte, vedere le community Yammer pertinenti.</span><span class="sxs-lookup"><span data-stu-id="c75cc-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>