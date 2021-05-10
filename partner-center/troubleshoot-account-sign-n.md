---
title: Risolvere i problemi di configurazione dell'account Partner Center o del rinnovo MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Risolvere i problemi durante il tentativo di registrazione in Partner Center. Le risposte consentono di risolvere i problemi relativi ai metodi di pagamento, all'eliminazione delle password e altro ancora.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686263"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="8bbe1-104">Risolvere i problemi di configurazione dell'account o di rinnovo MPN</span><span class="sxs-lookup"><span data-stu-id="8bbe1-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="8bbe1-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="8bbe1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="8bbe1-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="8bbe1-106">Global admin</span></span>
- <span data-ttu-id="8bbe1-107">Amministratore dei partner MPN</span><span class="sxs-lookup"><span data-stu-id="8bbe1-107">MPN partner admin</span></span>
 
<span data-ttu-id="8bbe1-108">Di seguito sono riportati alcuni suggerimenti per la risoluzione dei problemi comuni che si verificano durante la configurazione dell Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="8bbe1-109">Cosa accade se si esegue la migrazione da Partner Membership Center e non è possibile modificare i campi di informazioni aziendali</span><span class="sxs-lookup"><span data-stu-id="8bbe1-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="8bbe1-110">Nei casi in cui l'azienda ha già una presenza in Partner Center (ad esempio, un account CSP), verrà visualizzata una schermata di sola lettura.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="8bbe1-111">Questa schermata visualizza tutte le informazioni sull'azienda così come esiste Partner Center.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="8bbe1-112">Non è possibile modificare i dettagli in questa schermata.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-112">You can't change the details on this screen.</span></span> <span data-ttu-id="8bbe1-113">Si tratta di un errore di progettazione e non di un errore.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-113">This is by design and not an error.</span></span>

<span data-ttu-id="8bbe1-114">Selezionare **Accetta** e **continua** per continuare.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="8bbe1-115">Se il reparto IT ha disattivato **l'iscrizione per l'Partner Center**</span><span class="sxs-lookup"><span data-stu-id="8bbe1-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="8bbe1-116">Questo messaggio viene visualizzato perché gli utenti virali sono disabilitati o perché l'iscrizione virale è disabilitata Azure AD tenant.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="8bbe1-117">L'amministratore globale per l'account Azure AD può abilitare le funzionalità necessarie eseguendo il comando di PowerShell seguente:</span><span class="sxs-lookup"><span data-stu-id="8bbe1-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="8bbe1-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="8bbe1-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="8bbe1-119">Per altre informazioni, vedere [Iscrizione self-service.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="8bbe1-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="8bbe1-120">La password è stata dimenticata</span><span class="sxs-lookup"><span data-stu-id="8bbe1-120">You forgot your password</span></span>

<span data-ttu-id="8bbe1-121">Se la password è stata dimenticata, selezionare il collegamento Non è possibile **accedere all'account?** nella pagina di accesso.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="8bbe1-122">Questa opzione consente di reimpostare la password o chiedere all'amministratore globale di assegnare nuove credenziali.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="8bbe1-123">Nella schermata "Informazioni sull'azienda" viene visualizzato un errore "Si è verificato un errore"</span><span class="sxs-lookup"><span data-stu-id="8bbe1-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="8bbe1-124">Questo messaggio di errore viene in genere visualizzato se si usano inavvertitamente caratteri speciali, spazi o codice paese nel numero di telefono dell'azienda.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="8bbe1-125">Il valore immesso nel campo Numero di telefono può contenere solo un massimo di 10 caratteri.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="8bbe1-126">L'acquisto con carta di credito riceve un messaggio di errore che indica che l'ordine è stato rifiutato.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="8bbe1-127">Verificare le informazioni"</span><span class="sxs-lookup"><span data-stu-id="8bbe1-127">Please verify your information”</span></span>


<span data-ttu-id="8bbe1-128">Usare sempre l'indirizzo corrispondente alla carta di credito anziché la persona legale.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="8bbe1-129">Assicurarsi inoltre che il codice postale sia corretto e corrisponda all'indirizzo in uso.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="8bbe1-130">Si vuole passare dal pagamento offline al metodo di pagamento online</span><span class="sxs-lookup"><span data-stu-id="8bbe1-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="8bbe1-131">Sarà necessario annullare l'ordine originale e riacquisirlo usando il metodo di pagamento preferito.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="8bbe1-132">Per annullare un ordine:</span><span class="sxs-lookup"><span data-stu-id="8bbe1-132">To cancel an order:</span></span>

1. <span data-ttu-id="8bbe1-133">Selezionare **la scheda Offerte** di appartenenza nel dashboard.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="8bbe1-134">Selezionare **Annulla ordine**</span><span class="sxs-lookup"><span data-stu-id="8bbe1-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="8bbe1-135">Verrà visualizzata una finestra di conferma ed è necessario confermare per annullare l'ordine iniziale.</span><span class="sxs-lookup"><span data-stu-id="8bbe1-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8bbe1-136">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="8bbe1-136">Next steps</span></span>

- [<span data-ttu-id="8bbe1-137">Gestire l'account per il Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="8bbe1-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="8bbe1-138">Come leggere la fattura e il file di ricognizione</span><span class="sxs-lookup"><span data-stu-id="8bbe1-138">How to read your bill and recon file</span></span>](read-your-bill.md)
