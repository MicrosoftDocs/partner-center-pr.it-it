---
title: Risolvere i problemi di configurazione dell'account del centro per i partner o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi durante il tentativo di registrazione nel centro per i partner. Le risposte rispondono a problemi con i metodi di pagamento, dimenticando le password e altro ancora.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381410"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="3b793-104">Risolvere i problemi di configurazione dell'account o di rinnovo MPN</span><span class="sxs-lookup"><span data-stu-id="3b793-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="3b793-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="3b793-105">**Applies to**</span></span>

- <span data-ttu-id="3b793-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="3b793-106">Partner Center</span></span>
 
<span data-ttu-id="3b793-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="3b793-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3b793-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="3b793-108">Global admin</span></span>
- <span data-ttu-id="3b793-109">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="3b793-109">MPN partner admin</span></span> 
 
<span data-ttu-id="3b793-110">Ecco alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="3b793-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="3b793-111">Cosa accade se si esegue la migrazione da partner Membership Center e non è possibile modificare i campi di informazioni aziendali</span><span class="sxs-lookup"><span data-stu-id="3b793-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="3b793-112">Nei casi in cui la società dispone già di una presenza nel centro per i partner (ad indicare un account CSP), verrà visualizzata una schermata di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="3b793-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="3b793-113">In questa schermata vengono visualizzate tutte le informazioni sull'azienda così come esistono nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="3b793-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="3b793-114">Non è possibile modificare i dettagli in questa schermata.</span><span class="sxs-lookup"><span data-stu-id="3b793-114">You can't change the details on this screen.</span></span> <span data-ttu-id="3b793-115">Si tratta di un errore di progettazione.</span><span class="sxs-lookup"><span data-stu-id="3b793-115">This is by design and not an error.</span></span>

<span data-ttu-id="3b793-116">Selezionare **Accetto** e **continuare** per procedere.</span><span class="sxs-lookup"><span data-stu-id="3b793-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="3b793-117">Se il reparto IT ha disattivato l' **iscrizione per il centro per i partner**.</span><span class="sxs-lookup"><span data-stu-id="3b793-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="3b793-118">Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o perché l'iscrizione virale è disabilitata nel tenant Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b793-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="3b793-119">L'amministratore globale dell'account di Azure AD può abilitare le funzionalità necessarie eseguendo il comando PowerShell seguente:</span><span class="sxs-lookup"><span data-stu-id="3b793-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="3b793-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="3b793-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="3b793-121">Per altre informazioni, vedere [iscrizione self-service](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="3b793-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="3b793-122">Password dimenticata</span><span class="sxs-lookup"><span data-stu-id="3b793-122">You forgot your password</span></span>

<span data-ttu-id="3b793-123">Se si dimentica la password, selezionare il collegamento **non è possibile accedere all'account?** nella pagina di accesso.</span><span class="sxs-lookup"><span data-stu-id="3b793-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="3b793-124">Questa opzione consente di reimpostare la password o di richiedere all'amministratore globale di assegnare le nuove credenziali.</span><span class="sxs-lookup"><span data-stu-id="3b793-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="3b793-125">Nella schermata "informazioni sull'azienda" viene visualizzato un errore che indica che si è verificato un problema</span><span class="sxs-lookup"><span data-stu-id="3b793-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="3b793-126">Questo messaggio di errore viene in genere visualizzato se si usano inavvertitamente caratteri speciali, spazi o codice paese nel numero di telefono dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="3b793-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="3b793-127">Il valore immesso nel campo numero di telefono può contenere un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="3b793-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="3b793-128">L'acquisto della carta di credito riceve un messaggio di errore che informa che l'ordine è stato rifiutato.</span><span class="sxs-lookup"><span data-stu-id="3b793-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="3b793-129">Verificare le informazioni "</span><span class="sxs-lookup"><span data-stu-id="3b793-129">Please verify your information”</span></span>


<span data-ttu-id="3b793-130">Usare sempre l'indirizzo corrispondente alla carta di credito invece che all'entità legale.</span><span class="sxs-lookup"><span data-stu-id="3b793-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="3b793-131">Verificare inoltre che il codice postale sia corretto e corrisponda all'indirizzo utilizzato.</span><span class="sxs-lookup"><span data-stu-id="3b793-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="3b793-132">Si desidera passare dal pagamento offline al metodo di pagamento online</span><span class="sxs-lookup"><span data-stu-id="3b793-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="3b793-133">È necessario annullare l'ordine originale e riacquistare usando il metodo di pagamento preferito.</span><span class="sxs-lookup"><span data-stu-id="3b793-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="3b793-134">Per annullare un ordine:</span><span class="sxs-lookup"><span data-stu-id="3b793-134">To cancel an order:</span></span>

1. <span data-ttu-id="3b793-135">Selezionare la scheda **offerte di appartenenza** nel dashboard.</span><span class="sxs-lookup"><span data-stu-id="3b793-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="3b793-136">Seleziona **ordine di annullamento**</span><span class="sxs-lookup"><span data-stu-id="3b793-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="3b793-137">Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.</span><span class="sxs-lookup"><span data-stu-id="3b793-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b793-138">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="3b793-138">Next steps</span></span>

- [<span data-ttu-id="3b793-139">Gestire l'account per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="3b793-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="3b793-140">Come leggere il file di fatturazione e di ricognizione</span><span class="sxs-lookup"><span data-stu-id="3b793-140">How to read your bill and recon file</span></span>](read-your-bill.md)
