---
title: Gestire le posizioni nell'account partner
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663897"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="8dc03-103">Gestire le sedi dell'account MPN e aggiungere una nuova sede</span><span class="sxs-lookup"><span data-stu-id="8dc03-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="8dc03-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="8dc03-104">**Applies to**</span></span>

- <span data-ttu-id="8dc03-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="8dc03-105">Partner Center</span></span>

<span data-ttu-id="8dc03-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="8dc03-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8dc03-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="8dc03-107">Global admin</span></span>
- <span data-ttu-id="8dc03-108">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="8dc03-108">Account admin</span></span>

<span data-ttu-id="8dc03-109">L'ID MPN di sede identifica ogni specifica sede della società.</span><span class="sxs-lookup"><span data-stu-id="8dc03-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="8dc03-110">L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali.</span><span class="sxs-lookup"><span data-stu-id="8dc03-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="8dc03-111">L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.</span><span class="sxs-lookup"><span data-stu-id="8dc03-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="8dc03-112">Di seguito è riportato uno scenario tipico:</span><span class="sxs-lookup"><span data-stu-id="8dc03-112">The following is a typical scenario:</span></span>

<span data-ttu-id="8dc03-113">La sede dell'account globale partner di Contoso è nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="8dc03-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="8dc03-114">Si tratta della sede legale dell'azienda, mentre un ID MPN viene usato per la gestione di tutte le attività non transazionali.</span><span class="sxs-lookup"><span data-stu-id="8dc03-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="8dc03-115">Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti.</span><span class="sxs-lookup"><span data-stu-id="8dc03-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="8dc03-116">Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci.</span><span class="sxs-lookup"><span data-stu-id="8dc03-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="8dc03-117">Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP.</span><span class="sxs-lookup"><span data-stu-id="8dc03-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="8dc03-118">I pagamenti sono collegati a posizioni specifiche.</span><span class="sxs-lookup"><span data-stu-id="8dc03-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="8dc03-119">Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.</span><span class="sxs-lookup"><span data-stu-id="8dc03-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="8dc03-121">Prerequisiti per aggiungere una nuova sede per un'azienda CSP</span><span class="sxs-lookup"><span data-stu-id="8dc03-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="8dc03-122">Per aggiungere una nuova sede aziendale CSP, è necessario soddisfare alcuni prerequisiti:</span><span class="sxs-lookup"><span data-stu-id="8dc03-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="8dc03-123">È necessario avere un ID MPN di sede nel paese in cui si vuole svolgere le attività aziendali.</span><span class="sxs-lookup"><span data-stu-id="8dc03-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="8dc03-124">È necessario un nuovo tenant Azure AD nell'area di attività non ancora iscritta a CSP.</span><span class="sxs-lookup"><span data-stu-id="8dc03-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="8dc03-125">Creare questo tenant quando si effettua l'iscrizione a CSP.</span><span class="sxs-lookup"><span data-stu-id="8dc03-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="8dc03-126">Usare il nuovo tenant di AAD per l'iscrizione al programma CSP nell'area geografica.</span><span class="sxs-lookup"><span data-stu-id="8dc03-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="8dc03-127">Fornire i dettagli legali dell'azienda, inclusi la ragione sociale, l'indirizzo e i dettagli del contatto principale.</span><span class="sxs-lookup"><span data-stu-id="8dc03-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="8dc03-128">L'account verrà sottoposto a verifica, quindi assicurarsi di aggiungere informazioni valide.</span><span class="sxs-lookup"><span data-stu-id="8dc03-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="8dc03-129">Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8dc03-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="8dc03-130">Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.</span><span class="sxs-lookup"><span data-stu-id="8dc03-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="8dc03-131">Accettare il Contratto Microsoft Partner e attivare l'account.</span><span class="sxs-lookup"><span data-stu-id="8dc03-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="8dc03-132">Aggiungere una sede</span><span class="sxs-lookup"><span data-stu-id="8dc03-132">Add a location</span></span>

1. <span data-ttu-id="8dc03-133">Nell'icona **Impostazioni** seleziona **Impostazioni partner**.</span><span class="sxs-lookup"><span data-stu-id="8dc03-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="8dc03-134">Seleziona **Posizione**.</span><span class="sxs-lookup"><span data-stu-id="8dc03-134">Select **Locations.**</span></span>

3. <span data-ttu-id="8dc03-135">Seleziona **Aggiungi una posizione**.</span><span class="sxs-lookup"><span data-stu-id="8dc03-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="8dc03-136">Nella pagina **Aggiungi una posizione** inserisci i dettagli dell'indirizzo della posizione che vuoi aggiungere alla società, nonché un contatto principale per la posizione.</span><span class="sxs-lookup"><span data-stu-id="8dc03-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="8dc03-137">dopo aver aggiunto una posizione nel Centro per i partner, non è possibile rimuoverla.</span><span class="sxs-lookup"><span data-stu-id="8dc03-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="8dc03-138">Modificare la sede dell'account partner globale</span><span class="sxs-lookup"><span data-stu-id="8dc03-138">Change Global partner account location</span></span>

1. <span data-ttu-id="8dc03-139">Nella pagina **Posizione** controlla che nell'elenco delle posizioni sia presente quella desiderata come entità legale.</span><span class="sxs-lookup"><span data-stu-id="8dc03-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="8dc03-140">In caso contrario, aggiungerla.</span><span class="sxs-lookup"><span data-stu-id="8dc03-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Struttura delle sedi MPN":::

2. <span data-ttu-id="8dc03-142">Seleziona **Profilo partner** e quindi **Update legal business profile (Aggiorna profilo aziendale legale)**</span><span class="sxs-lookup"><span data-stu-id="8dc03-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Struttura delle sedi MPN":::

3. <span data-ttu-id="8dc03-144">Seleziona l'area e la persona giuridica e quindi **Invia**.</span><span class="sxs-lookup"><span data-stu-id="8dc03-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Struttura delle sedi MPN":::

## <a name="next-steps"></a><span data-ttu-id="8dc03-146">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="8dc03-146">Next steps</span></span>

- <span data-ttu-id="8dc03-147">Vedere le informazioni sul [processo di verifica](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="8dc03-147">Learn about the [verification process](verification-responses.md).</span></span>
