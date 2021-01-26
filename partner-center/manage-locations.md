---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773436"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="16d43-103">Gestire le sedi dell'account MPN e aggiungere una nuova sede</span><span class="sxs-lookup"><span data-stu-id="16d43-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="16d43-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="16d43-104">**Appropriate roles**</span></span>

- <span data-ttu-id="16d43-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="16d43-105">Global admin</span></span>
- <span data-ttu-id="16d43-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="16d43-106">Account admin</span></span>

<span data-ttu-id="16d43-107">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="16d43-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="16d43-108">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="16d43-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="16d43-109">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="16d43-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="16d43-110">Di seguito è riportato uno scenario tipico:</span><span class="sxs-lookup"><span data-stu-id="16d43-110">The following is a typical scenario:</span></span>

<span data-ttu-id="16d43-111">Contoso ha registrato il proprio account globale partner nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="16d43-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="16d43-112">Si tratta della sede legale dell'azienda e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="16d43-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="16d43-113">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="16d43-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="16d43-114">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="16d43-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="16d43-115">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="16d43-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="16d43-116">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="16d43-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="16d43-117">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="16d43-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="16d43-119">Prerequisiti per l'aggiunta di un nuovo percorso dell'account per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="16d43-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="16d43-120">Per aggiungere una nuova sede aziendale CSP, è necessario soddisfare alcuni prerequisiti:</span><span class="sxs-lookup"><span data-stu-id="16d43-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="16d43-121">È necessario avere un ID MPN di sede nel paese in cui si vuole svolgere le attività aziendali.</span><span class="sxs-lookup"><span data-stu-id="16d43-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="16d43-122">È necessario un nuovo tenant Azure AD nell'[area geografica di attività](regional-authorization-overview.md) non ancora iscritta a CSP.</span><span class="sxs-lookup"><span data-stu-id="16d43-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="16d43-123">Creare questo tenant quando si effettua l'iscrizione a CSP.</span><span class="sxs-lookup"><span data-stu-id="16d43-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="16d43-124">Usare il nuovo tenant di AAD per l'iscrizione al programma CSP nell'area geografica.</span><span class="sxs-lookup"><span data-stu-id="16d43-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="16d43-125">Fornire i dettagli legali dell'azienda, inclusi la ragione sociale, l'indirizzo e i dettagli del contatto principale.</span><span class="sxs-lookup"><span data-stu-id="16d43-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="16d43-126">L'account verrà sottoposto a verifica, quindi assicurarsi di aggiungere informazioni valide.</span><span class="sxs-lookup"><span data-stu-id="16d43-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="16d43-127">Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="16d43-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="16d43-128">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="16d43-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="16d43-129">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="16d43-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="16d43-130">Aggiungere una sede MPN</span><span class="sxs-lookup"><span data-stu-id="16d43-130">Add an MPN location</span></span>

1. <span data-ttu-id="16d43-131">Accedere al Centro per i partner con l'account MPN.</span><span class="sxs-lookup"><span data-stu-id="16d43-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="16d43-132">L'account MPN deve avere i privilegi di amministratore globale o amministratore account.</span><span class="sxs-lookup"><span data-stu-id="16d43-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="16d43-133">Nell'icona **Impostazioni** selezionare **Impostazioni dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="16d43-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="16d43-134">Selezionare **Note legali** quindi **Posizioni**.</span><span class="sxs-lookup"><span data-stu-id="16d43-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="16d43-135">Selezionare **Aggiungere una sede** e inserire i dettagli dell'indirizzo della sede che si vuole aggiungere alla società, nonché un contatto principale per la sede.</span><span class="sxs-lookup"><span data-stu-id="16d43-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="16d43-136">dopo aver aggiunto una posizione nel Centro per i partner, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="16d43-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="16d43-137">Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="16d43-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="16d43-138">Modificare la sede dell'account partner globale</span><span class="sxs-lookup"><span data-stu-id="16d43-138">Change Global partner account location</span></span>

1. <span data-ttu-id="16d43-139">Nella pagina **[Località società](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** verificare che la sede desiderata come entità legale sia inclusa nell'elenco delle sedi.</span><span class="sxs-lookup"><span data-stu-id="16d43-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="16d43-140">In caso contrario, aggiungerla.</span><span class="sxs-lookup"><span data-stu-id="16d43-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot della pagina delle posizioni dell'account del Centro per i partner con l'elenco di tutte le posizioni correnti.":::

2. <span data-ttu-id="16d43-142">Selezionare **Note legali** quindi **aggiornare il profilo legale dell'azienda**</span><span class="sxs-lookup"><span data-stu-id="16d43-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="16d43-143">Seleziona l'area e la persona giuridica e quindi **Invia**.</span><span class="sxs-lookup"><span data-stu-id="16d43-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="16d43-144">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="16d43-144">Next steps</span></span>

- <span data-ttu-id="16d43-145">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="16d43-145">Learn about the [verification process](verification-responses.md).</span></span>
