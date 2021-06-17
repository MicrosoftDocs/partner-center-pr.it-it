---
title: Unire l'account partner con un altro account partner
description: Informazioni su come unire l'account partner a un altro account partner in Partner Center, per le aziende che sono partner Microsoft attivi in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276638"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="d2e2b-103">Unire l'account partner con un altro account partner</span><span class="sxs-lookup"><span data-stu-id="d2e2b-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="d2e2b-104">**Ruoli appropriati:** Amministratore account</span><span class="sxs-lookup"><span data-stu-id="d2e2b-104">**Appropriate roles**: Account admin</span></span>

<span data-ttu-id="d2e2b-105">Due o più aziende che sono partner Microsoft attivi e hanno account in Partner Center possibile scegliere di unire i propri account.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-105">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="d2e2b-106">Cosa accade quando due partner sceglie di unire i propri account Partner Center partner</span><span class="sxs-lookup"><span data-stu-id="d2e2b-106">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="d2e2b-107">L'organizzazione partner che avvia l'unione sarà l'account globale del partner.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-107">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="d2e2b-108">Il PGA dell'organizzazione invitata diventa la posizione dell'azienda che ha iniziato.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-108">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="d2e2b-109">Tutte le posizioni dell'account di unione diventano posizioni nel PGA.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-109">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="d2e2b-110">Al termine della fusione dell'account, verranno visualizzati i dettagli dell'account, ad esempio le posizioni e gli utenti all'interno del profilo PGA.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-110">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="d2e2b-111">Non è possibile invertire questo processo.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-111">You can't reverse this process.</span></span>

- <span data-ttu-id="d2e2b-112">Tutti gli ID MPN per le località vengono mantenuti durante questo consolidamento.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-112">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="d2e2b-113">Vengono assegnati i ruoli dell'utente.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-113">User's roles are brought over.</span></span> <span data-ttu-id="d2e2b-114">Ad esempio, se un utente fosse stato l'amministratore di incentivi per una località specifica, avrebbe ancora quel ruolo dopo la fusione e sarebbe in grado di visualizzare gli incentivi visti prima della fusione.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-114">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="d2e2b-115">Azure AD tenant e gli account CSP non vengono uniti e non hanno alcun effetto.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-115">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="d2e2b-116">Le offerte pubblicate e i dati della pipeline di co-selling associati a entrambe le aziende vengono conservati</span><span class="sxs-lookup"><span data-stu-id="d2e2b-116">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="d2e2b-117">Visualizzazione degli account uniti</span><span class="sxs-lookup"><span data-stu-id="d2e2b-117">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fusione di account.":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="d2e2b-119">Cosa aspettarsi se si è stati invitati a unire l'account Partner Center con un altro account Partner Center</span><span class="sxs-lookup"><span data-stu-id="d2e2b-119">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="d2e2b-120">Se si decide di accettare l'invito a unire gli account: · Gli ID MPN e le località verranno uniti nell'account PGA dell'account partner che ha invitato l'utente.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-120">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="d2e2b-121">Gli utenti verranno portati nell'account unito con i relativi ruoli intatti.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-121">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="d2e2b-122">I vantaggi e le competenze esistenti verranno mantenuti per entrambe le società dopo la fusione fino al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-122">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="d2e2b-123">Al momento del rinnovo, gli account verranno considerati come una società e verranno applicate le regole di rinnovo standard.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-123">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="d2e2b-124">Comprendere l'impatto sui programmi e sui vantaggi quando i partner decidono di unire gli account</span><span class="sxs-lookup"><span data-stu-id="d2e2b-124">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="d2e2b-125">Tutte le competenze esistenti (Gold/Silver), gli acquisti (ad esempio Microsoft Action Pack) e i vantaggi associati vengono mantenuti durante il consolidamento.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-125">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="d2e2b-126">Se entrambe le aziende hanno la stessa competenza, ma una è gold e l'altra silver, la competenza con il livello di competenza più elevato verrà assegnata e i partner avranno un set di vantaggi Silver e un set di vantaggi Gold per tale competenza fino al successivo rinnovo.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-126">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="d2e2b-127">La data di ricorrenza più elevata Action Pack Microsoft verrà mantenuta dopo la fusione.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-127">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="d2e2b-128">Ad esempio, se la data dell'anniversario per la società 1 è giugno 2020 per il rinnovo del Action Pack e la data dell'anniversario per il rinnovo della società Action Pack 2 è ottobre 2020, Microsoft userà la data di ottobre 2020 come nuova data di anniversario per la società unita.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-128">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="d2e2b-129">Durante la fusione dell'account e fino al successivo rinnovo, ogni account manterrà i Action Pack e/o i vantaggi di competenza.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-129">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="d2e2b-130">Al momento del rinnovo, si applicano le Action Pack standard e di rinnovo delle competenze.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-130">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="d2e2b-131">Al momento del rinnovo, i vantaggi inclusi con il conseguimento delle competenze e Action Pack vengono implementati per l'account globale partner della società partner:</span><span class="sxs-lookup"><span data-stu-id="d2e2b-131">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="d2e2b-132">Microsoft Action Pack: la società partner sarà in grado di acquistare una Action Pack per ogni account globale partner.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-132">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="d2e2b-133">Competenza: la società partner riceverà un pacchetto di vantaggi di base, associati al massimo livello di competenza, oltre ai vantaggi specifici delle competenze per cui il partner è idoneo per ogni account globale del partner.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-133">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="d2e2b-134">Tutti i vantaggi sono soggetti alla guida [all Microsoft Partner Network sull'utilizzo dei vantaggi.](https://aka.ms/partner-benefits-use-guide)</span><span class="sxs-lookup"><span data-stu-id="d2e2b-134">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="d2e2b-135">Ad esempio: un token di O365 E3 attivato funziona per 12 mesi dopo l'attivazione.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-135">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="d2e2b-136">Dopo che un token è stato attivato per le licenze in un tenant, tali licenze potrebbero non essere spostate in un altro tenant.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-136">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="d2e2b-137">Le associazioni ID MCP per entrambe le società verranno mantenute e associate all'ID MPN PGA.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-137">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="d2e2b-138">I vantaggi tecnici e go-to-market vengono offerti come vantaggio principale per le competenze.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-138">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="d2e2b-139">Dopo la unione, è consigliabile controllare le informazioni bancarie e fiscali per garantire l'accuratezza.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-139">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="d2e2b-140">Se la società è in programma Azure Expert MSP, i vantaggi vengono mantenuti fino al rinnovo.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-140">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="d2e2b-141">Se l'azienda ha ottenuto specializzazioni avanzate, vengono mantenute in entrambi gli account.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-141">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="d2e2b-142">Tutti i voucher Software Assurance vengono conservati in entrambi gli account.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-142">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="d2e2b-143">Non esiste alcun effetto sull'associazione DPOR o PAL.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-143">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="d2e2b-144">Tutti i contributi ai ricavi associati inizieranno a confluire nel nuovo account globale del partner</span><span class="sxs-lookup"><span data-stu-id="d2e2b-144">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="d2e2b-145">Invitare un'azienda a unire il proprio account Partner Center con l'account Partner Center aziendale</span><span class="sxs-lookup"><span data-stu-id="d2e2b-145">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="d2e2b-146">Per eseguire la fusione degli account, è necessario essere **l'amministratore account** della società.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-146">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="d2e2b-147">Selezionare **Impostazioni** nel dashboard Partner Center dati.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-147">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="d2e2b-148">Selezionare **Account merge**.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-148">Select **Account merge**.</span></span>

3. <span data-ttu-id="d2e2b-149">Aggiungere l'ID MPN che si trova nel **profilo partner** dell'account che si vuole invitare a unire con l'utente.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-149">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="d2e2b-150">È necessario usare l'ID MPN globale del partner.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-150">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="d2e2b-151">Non è possibile usare un ID MPN della posizione.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-151">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="d2e2b-152">Quando si seleziona **Unisci**, viene inviato un invito alla società partner.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-152">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="d2e2b-153">Quando accettano la richiesta, è possibile avviare l'unione dell'account all'interno Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-153">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="d2e2b-154">Se la società rifiuta la richiesta di unione degli account, può spiegare perché ha rifiutato la richiesta.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-154">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="d2e2b-155">Un elenco di tutte le unioni di account è disponibile in **Cronologia unione**.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-155">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="d2e2b-156">Esempio di due società che uniscono account</span><span class="sxs-lookup"><span data-stu-id="d2e2b-156">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="d2e2b-157">Contoso, Ltd. ha</span><span class="sxs-lookup"><span data-stu-id="d2e2b-157">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="d2e2b-158">a.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-158">a.</span></span> <span data-ttu-id="d2e2b-159">un [ID MPN globale 1111111 e](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) un ID MPN di posizione subordinata di [2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span><span class="sxs-lookup"><span data-stu-id="d2e2b-159">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="d2e2b-160">b.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-160">b.</span></span> <span data-ttu-id="d2e2b-161">un tenant Azure AD = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="d2e2b-161">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="d2e2b-162">c.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-162">c.</span></span> <span data-ttu-id="d2e2b-163">una competenza Gold che scade il 1° ottobre 2020</span><span class="sxs-lookup"><span data-stu-id="d2e2b-163">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="d2e2b-164">Fabrikam, Inc. ha</span><span class="sxs-lookup"><span data-stu-id="d2e2b-164">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="d2e2b-165">a.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-165">a.</span></span>  <span data-ttu-id="d2e2b-166">un ID MPN globale di 3333333 e due ID MPN della posizione subordinata 4444444 e 5555555</span><span class="sxs-lookup"><span data-stu-id="d2e2b-166">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="d2e2b-167">b.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-167">b.</span></span>  <span data-ttu-id="d2e2b-168">un tenant Azure AD = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="d2e2b-168">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="d2e2b-169">c.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-169">c.</span></span>  <span data-ttu-id="d2e2b-170">due competenze Gold che scadono il 1° dicembre 2020</span><span class="sxs-lookup"><span data-stu-id="d2e2b-170">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="d2e2b-171">Contoso acquista Fabrikam e viene qui [per](https://partner.microsoft.com/dashboard/account/merger) avviare una richiesta di merge.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-171">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="d2e2b-172">Fabrikam accede Partner Center e passa alla stessa pagina di Contoso nel passaggio #3, per approvare la richiesta di Contoso.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-172">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="d2e2b-173">Contoso esamina i dettagli dell'unione nella stessa pagina e fornisce una conferma per procedere con la fusione dell'account.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-173">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="d2e2b-174">Dopo la fusione, l'account aziendale verrà visualizzato come:</span><span class="sxs-lookup"><span data-stu-id="d2e2b-174">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="d2e2b-175">a.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-175">a.</span></span>  <span data-ttu-id="d2e2b-176">Una società denominata Contoso con ID MPN globale 1111111 e 4 ID MPN di posizione subordinata 2222222, 33333333, 44444444 e 5555555</span><span class="sxs-lookup"><span data-stu-id="d2e2b-176">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="d2e2b-177">b.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-177">b.</span></span>  <span data-ttu-id="d2e2b-178">Avrà due tenant Azure AD ( + ) che hanno @contoso.com accesso allo stesso account @fabrikam.com Partner Center</span><span class="sxs-lookup"><span data-stu-id="d2e2b-178">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="d2e2b-179">c.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-179">c.</span></span>  <span data-ttu-id="d2e2b-180">Avrà due pacchetti di vantaggi per le competenze, uno con scadenza il 1° ottobre 2020 e l'altro con scadenza il 1° dicembre 2020.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-180">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="d2e2b-181">Il 1° dicembre 2020 sarà possibile eseguire il rinnovo come singolo pacchetto di vantaggi per le competenze.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-181">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="d2e2b-182">Al momento del rinnovo, Contoso manterrà tutte e tre le competenze anche se può gestire un solo pacchetto di vantaggi.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-182">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="d2e2b-183">Gli amministratori di Contoso continueranno a gestire i Partner Center per @contoso.com gli utenti di .</span><span class="sxs-lookup"><span data-stu-id="d2e2b-183">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="d2e2b-184">Gli amministratori di Fabrikam continueranno a gestire i Partner Center per @fabrikam.com gli utenti di .</span><span class="sxs-lookup"><span data-stu-id="d2e2b-184">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="d2e2b-185">Gli amministratori di Contoso possono amministrare gli utenti di Fabrikam solo se vengono invitati come guest nel tenant di Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-185">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="d2e2b-186">Contoso potrebbe decidere di ignorare il tenant e riemettere le nuove credenziali ai dipendenti @fabrikam.com fabrikam con nuovi ruoli e @contoso.com autorizzazioni.</span><span class="sxs-lookup"><span data-stu-id="d2e2b-186">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d2e2b-187">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d2e2b-187">Next steps</span></span>

- [<span data-ttu-id="d2e2b-188">Assegnare autorizzazioni e ruoli utente</span><span class="sxs-lookup"><span data-stu-id="d2e2b-188">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="d2e2b-189">Verificare le informazioni del profilo partner</span><span class="sxs-lookup"><span data-stu-id="d2e2b-189">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="d2e2b-190">Aggiungere Servizi condivisi per partner di Azure in modo che i partner possano acquistare sottoscrizioni di Azure per uso personale</span><span class="sxs-lookup"><span data-stu-id="d2e2b-190">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
