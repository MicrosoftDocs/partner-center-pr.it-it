---
title: Risolvere i problemi di configurazione dell'account del centro per i partner o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi relativi alla registrazione nel centro per i partner
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848935"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="7204f-103">Risolvere i problemi di configurazione dell'account o di rinnovo MPN</span><span class="sxs-lookup"><span data-stu-id="7204f-103">Troubleshoot account setup or MPN renewal issues</span></span>

### <a name="applies-to"></a><span data-ttu-id="7204f-104">Si applica a</span><span class="sxs-lookup"><span data-stu-id="7204f-104">Applies to</span></span>

- <span data-ttu-id="7204f-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="7204f-105">Partner Center</span></span>
 
### <a name="appropriate-roles"></a><span data-ttu-id="7204f-106">Ruoli appropriati</span><span class="sxs-lookup"><span data-stu-id="7204f-106">Appropriate roles</span></span>

- <span data-ttu-id="7204f-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="7204f-107">Global admin</span></span>
- <span data-ttu-id="7204f-108">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="7204f-108">MPN partner admin</span></span> 
 

<span data-ttu-id="7204f-109">Ecco alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="7204f-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="7204f-110">Cosa accade se si esegue la migrazione da partner Membership Center e non è possibile modificare i campi di informazioni aziendali</span><span class="sxs-lookup"><span data-stu-id="7204f-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="7204f-111">Questa situazione si verifica nei casi in cui la società dispone già di una presenza nel centro per i partner (ad esempio, l'account CSP). verrà visualizzata una schermata di sola lettura in cui verranno visualizzate tutte le informazioni sull'azienda così come esistono nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="7204f-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="7204f-112">Non è possibile modificare i dettagli in questa schermata.</span><span class="sxs-lookup"><span data-stu-id="7204f-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="7204f-113">Si tratta di un errore di progettazione.</span><span class="sxs-lookup"><span data-stu-id="7204f-113">This is by design and not an error.</span></span>

<span data-ttu-id="7204f-114">Selezionare **Accetto** e **continuare** per procedere.</span><span class="sxs-lookup"><span data-stu-id="7204f-114">Select **Accept** and **Continue** to proceed.</span></span>

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="7204f-115">Si sta tentando di eseguire la registrazione o di eseguire la migrazione da partner Membership Center e viene visualizzato un messaggio di errore che informa che il reparto IT ha disattivato l' **iscrizione per il centro per i partner**.</span><span class="sxs-lookup"><span data-stu-id="7204f-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span> 

<span data-ttu-id="7204f-116">Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o l'iscrizione virale è disabilitata nel tenant del Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7204f-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="7204f-117">L'amministratore globale dell'account di Azure AD può abilitare le funzionalità necessarie eseguendo il comando PowerShell seguente:</span><span class="sxs-lookup"><span data-stu-id="7204f-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="7204f-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="7204f-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="7204f-119">Per altre informazioni, vedere [iscrizione self-service](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="7204f-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

### <a name="you-forgot-your-password"></a><span data-ttu-id="7204f-120">Password dimenticata</span><span class="sxs-lookup"><span data-stu-id="7204f-120">You forgot your password</span></span>

<span data-ttu-id="7204f-121">Se si dimentica la password, selezionare il collegamento **non è possibile accedere all'account?** nella pagina di accesso per reimpostare la password o chiedere all'amministratore globale di assegnare le nuove credenziali.</span><span class="sxs-lookup"><span data-stu-id="7204f-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="7204f-122">Nella schermata "informazioni sull'azienda" viene visualizzato un errore che indica che si è verificato un problema</span><span class="sxs-lookup"><span data-stu-id="7204f-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="7204f-123">Questo problema si verifica in genere se si usano inavvertitamente caratteri speciali, spazi o codici paese nel numero di telefono dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="7204f-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="7204f-124">Il valore immesso nel campo numero di telefono può contenere un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="7204f-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="7204f-125">Si sta provando a completare l'acquisto tramite carta di credito, ma si riceve un messaggio di errore che informa che l'ordine è stato rifiutato.</span><span class="sxs-lookup"><span data-stu-id="7204f-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="7204f-126">Verificare le informazioni "</span><span class="sxs-lookup"><span data-stu-id="7204f-126">Please verify your information”</span></span>

<span data-ttu-id="7204f-127">È sempre necessario inserire l'indirizzo corrispondente alla carta di credito e non corrispondente all'entità legale.</span><span class="sxs-lookup"><span data-stu-id="7204f-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="7204f-128">Verificare inoltre che il codice postale sia corretto e corrisponda all'indirizzo utilizzato.</span><span class="sxs-lookup"><span data-stu-id="7204f-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="7204f-129">Si desidera passare dal pagamento offline al metodo di pagamento online</span><span class="sxs-lookup"><span data-stu-id="7204f-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="7204f-130">È necessario annullare l'ordine originale e riacquistare usando il metodo di pagamento preferito.</span><span class="sxs-lookup"><span data-stu-id="7204f-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="7204f-131">Per annullare un ordine:</span><span class="sxs-lookup"><span data-stu-id="7204f-131">To cancel an order:</span></span>

1. <span data-ttu-id="7204f-132">Selezionare la scheda **offerte di appartenenza** nel dashboard.</span><span class="sxs-lookup"><span data-stu-id="7204f-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="7204f-133">Seleziona **ordine di annullamento**</span><span class="sxs-lookup"><span data-stu-id="7204f-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="7204f-134">Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.</span><span class="sxs-lookup"><span data-stu-id="7204f-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
