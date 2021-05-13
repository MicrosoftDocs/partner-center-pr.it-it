---
title: Non è possibile accedere a Partner Center
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 'Risolvere le possibili cause e ottenere informazioni sulle soluzioni per quando non è possibile accedere a Partner Center: altre informazioni sulla reimpostazione delle password, sul controllo dei ruoli e sul controllo delle credenziali.'
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818797"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="c8230-103">Risolvere i problemi di accesso per Partner Center</span><span class="sxs-lookup"><span data-stu-id="c8230-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="c8230-104">**Ruoli appropriati:** tutti i partner interessati a Partner Center</span><span class="sxs-lookup"><span data-stu-id="c8230-104">**Appropriate roles**: All partners interested in Partner Center</span></span>

<span data-ttu-id="c8230-105">Questo articolo contiene soluzioni per problemi di accesso comuni per Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c8230-105">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="c8230-106">È stata dimenticata la password per Partner Center</span><span class="sxs-lookup"><span data-stu-id="c8230-106">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="c8230-107">Se si dimentica la password e non è possibile accedere Partner Center, contattare il supporto tecnico.</span><span class="sxs-lookup"><span data-stu-id="c8230-107">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="c8230-108">Trovare il contatto appropriato in [Supporto per i prodotti aziendali.](/microsoft-365/admin/contact-support-for-business-products)</span><span class="sxs-lookup"><span data-stu-id="c8230-108">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="c8230-109">I partner MPN possono chiedere all'amministratore globale di creare una nuova password.</span><span class="sxs-lookup"><span data-stu-id="c8230-109">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="c8230-110">I rivenditori indiretti CSP possono chiedere al provider indiretto di creare un nuovo amministratore globale nel tenant di Azure AD o di creare una nuova password usando i privilegi di amministratore con delega.</span><span class="sxs-lookup"><span data-stu-id="c8230-110">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="c8230-111">Per altre informazioni su come reimpostare la password e ottenere nuovamente l'accesso all'account aziendale, vedere Reimpostare la password aziendale o dell'istituto di [istruzione usando le informazioni di sicurezza.](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="c8230-111">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="c8230-112">Non è possibile visualizzare o gestire le pagine o le funzionalità previste in Partner Center</span><span class="sxs-lookup"><span data-stu-id="c8230-112">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="c8230-113">L'accesso alle Partner Center è controllato dai ruoli assegnati.</span><span class="sxs-lookup"><span data-stu-id="c8230-113">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="c8230-114">Per controllare i ruoli assegnati, in Partner Center l'icona Impostazioni, selezionare **Impostazioni** account e quindi in Impostazioni account selezionare **Gestione utenti.**</span><span class="sxs-lookup"><span data-stu-id="c8230-114">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="c8230-115">In Cerca digitare il nome e quindi visualizzare i risultati.</span><span class="sxs-lookup"><span data-stu-id="c8230-115">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="c8230-116">Se non è possibile visualizzare o gestire le competenze, i clienti, gli incentivi o gli utenti previsti, provare le soluzioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="c8230-116">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="c8230-117">Per accedere alle funzionalità di MPN, CSP e segnalazioni, contattare l'amministratore globale o l'amministratore account. Per altre informazioni sui ruoli e sulle attività che abilitano in Partner Center, vedere Assegnare ruoli & [autorizzazioni agli utenti.](permissions-overview.md)</span><span class="sxs-lookup"><span data-stu-id="c8230-117">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="c8230-118">Per accedere alle funzionalità del Marketplace commerciale e dei programmi per sviluppatori Windows & Xbox, Office Store, Microsoft Edge e Hardware, contattare la persona nel ruolo Proprietario o Manager dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="c8230-118">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="c8230-119">Per altre informazioni su ruoli e autorizzazioni, vedere [Come gestire un account del marketplace](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)commerciale in Microsoft Partner Center .</span><span class="sxs-lookup"><span data-stu-id="c8230-119">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="c8230-120">Non è possibile visualizzare l'offerta o i vantaggi in Partner Center</span><span class="sxs-lookup"><span data-stu-id="c8230-120">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="c8230-121">Verificare di usare le credenziali corrette per l'accesso.</span><span class="sxs-lookup"><span data-stu-id="c8230-121">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="c8230-122">Ad esempio, gli account aziendali e personali possono avere lo stesso aspetto ( ad esempio ), ma uno può essere un account personale creato e un altro può essere un account aziendale configurato per abc@contoso.com conto dell'utente.</span><span class="sxs-lookup"><span data-stu-id="c8230-122">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="c8230-123">In questo caso, se è stato eseguito l'accesso, ma non è possibile visualizzare le funzionalità previste correlate a MPN, CSP, Marketplace commerciale, provare a selezionare l'account aziendale.</span><span class="sxs-lookup"><span data-stu-id="c8230-123">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c8230-124">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="c8230-124">Next steps</span></span>

- [<span data-ttu-id="c8230-125">Verificare le informazioni sull'account</span><span class="sxs-lookup"><span data-stu-id="c8230-125">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="c8230-126">Reimpostare la password personale</span><span class="sxs-lookup"><span data-stu-id="c8230-126">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="c8230-127">Reimpostare una password utente</span><span class="sxs-lookup"><span data-stu-id="c8230-127">Reset a user password</span></span>](reset-a-user-password.md)