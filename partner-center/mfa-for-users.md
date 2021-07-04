---
title: Configurare gli utenti con l'autenticazione a più fattori
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come configurare i dipendenti con MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450807"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="a4a66-103">Configurare gli utenti con l'autenticazione a più fattori</span><span class="sxs-lookup"><span data-stu-id="a4a66-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="a4a66-104">**Ruoli appropriati:** Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="a4a66-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="a4a66-105">Le misure di sicurezza e la protezione della privacy sono alcune tra le nostre priorità più importanti.</span><span class="sxs-lookup"><span data-stu-id="a4a66-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="a4a66-106">Sappiamo che la migliore difesa è la prevenzione e di essere al sicuro quanto lo sono i nostri punti più deboli.</span><span class="sxs-lookup"><span data-stu-id="a4a66-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="a4a66-107">Questo è il motivo per cui è necessario che tutti nell'ecosistema agiscano e si assicurino che vengano adottate le protezioni di sicurezza appropriate.</span><span class="sxs-lookup"><span data-stu-id="a4a66-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="a4a66-108">È consigliabile che tutti i partner abilitino l'autenticazione a più fattori (MFA) per gli utenti nel tenant partner.</span><span class="sxs-lookup"><span data-stu-id="a4a66-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="a4a66-109">Aggiungere l'autenticazione a più fattori per gli utenti</span><span class="sxs-lookup"><span data-stu-id="a4a66-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="a4a66-110">Per completare questa attività, è necessario essere l'amministratore globale della società.</span><span class="sxs-lookup"><span data-stu-id="a4a66-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="a4a66-111">È possibile abilitare l'autenticazione a più fattori per gli utenti con la massima facilità quando tali utenti vengono aggiunti al tenant di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a4a66-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="a4a66-112">Accedere al [portale di Azure](https://portal.azure.com) e quindi passare a **Gestione utenti**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="a4a66-113">Selezionare **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="a4a66-114">Selezionare l'utente che si vuole abilitare e quindi selezionare **Abilita**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="a4a66-115">Verrà abilitata l'autenticazione a più fattori per l'utente.</span><span class="sxs-lookup"><span data-stu-id="a4a66-115">This will enable MFA for this user.</span></span> <span data-ttu-id="a4a66-116">L'opzione Abilitato indica che all'utente verrà chiesto di impostare la verifica dell'autenticazione a più fattori al primo accesso.</span><span class="sxs-lookup"><span data-stu-id="a4a66-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="a4a66-117">Successivamente, al momento dell'accesso, verrà chiesto di fornire un codice ricevuto tramite posta elettronica o SMS, a seconda dell'impostazione fornita.</span><span class="sxs-lookup"><span data-stu-id="a4a66-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Specificare la modalità di verifica.":::

>[!NOTE]
><span data-ttu-id="a4a66-119">Per consentire agli utenti di usare l'autenticazione a più fattori, è possibile usare l'opzione **Applica** seguendo la stessa procedura illustrata in precedenza e selezionando **Applica**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="a4a66-120">Per altre informazioni, vedere [Abilitare Azure Multi-Factor Authentication per singolo utente per proteggere gli eventi di accesso](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="a4a66-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="a4a66-121">Lo stato iniziale di tutti gli utenti è  **Disabilitato**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-121">All users start out **Disabled**.</span></span> <span data-ttu-id="a4a66-122">Quando si registrano utenti in Azure Active Directory Multi-Factor Authentication, il relativo stato viene modificato in **Abilitato**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="a4a66-123">Quando gli utenti abilitati eseguono l'accesso e completano il processo di registrazione, il relativo stato viene modificato in  **Applicato**.</span><span class="sxs-lookup"><span data-stu-id="a4a66-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="a4a66-124">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="a4a66-124">Next steps</span></span>

- [<span data-ttu-id="a4a66-125">Assegnare ruoli e autorizzazioni agli utenti</span><span class="sxs-lookup"><span data-stu-id="a4a66-125">Assign roles and permissions to users</span></span>](permissions-overview.md)