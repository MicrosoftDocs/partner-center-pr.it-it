---
title: Aggiungere altri tenant all'account del centro per i partner
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gestire più tenant tramite l'account del centro per i partner
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846961"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="2a81e-103">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2a81e-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="2a81e-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="2a81e-104">**Applies to**</span></span>

- <span data-ttu-id="2a81e-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2a81e-105">Partner Center</span></span>

<span data-ttu-id="2a81e-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="2a81e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2a81e-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="2a81e-107">Global admin</span></span>

<span data-ttu-id="2a81e-108">Questa funzionalità consente all'utente di gestire più tenant per la propria azienda e di consolidarli nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="2a81e-109">Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="2a81e-110">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="2a81e-110">For example:</span></span>

- <span data-ttu-id="2a81e-111">L'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="2a81e-112">Tuttavia, si vuole che le due società rimangano separate.</span><span class="sxs-lookup"><span data-stu-id="2a81e-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="2a81e-113">In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="2a81e-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="2a81e-114">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="2a81e-115">Se si dispone di più tenant per l'esecuzione dell'attività, ad esempio contoso.com, contoso.uk, contoso.in, è possibile usare il multi-tenant per collegarli con lo stesso account del computer.</span><span class="sxs-lookup"><span data-stu-id="2a81e-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="2a81e-116">Per le fusioni e le acquisizioni è necessario usare più di un tenant (ad esempio, se contoso acquisisce Fabrikam, è necessario poter usare sia Constoso.com che Fabrikam.com rispettivi tenant).</span><span class="sxs-lookup"><span data-stu-id="2a81e-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="2a81e-117">È necessario che gli utenti di uno dei tenant siano in grado di:</span><span class="sxs-lookup"><span data-stu-id="2a81e-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="2a81e-118">Accedi al centro per i partner per corsi di formazione, download digitali, associazione MCP</span><span class="sxs-lookup"><span data-stu-id="2a81e-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="2a81e-119">Sono assegnati ruoli del centro per i partner, ad esempio MPN admin, incentives admin e così via.</span><span class="sxs-lookup"><span data-stu-id="2a81e-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="2a81e-120">Aggiungere un altro tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="2a81e-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="2a81e-121">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="2a81e-122">Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="2a81e-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associa tenant"::: 

3. <span data-ttu-id="2a81e-124">Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="2a81e-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="2a81e-125">Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="2a81e-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="conferma associazione tenant"::: 

5. <span data-ttu-id="2a81e-127">Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="2a81e-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="2a81e-128">Selezionare **Torna a gestione tenant per** visualizzare l'elenco dei tenant appena aggiunti.</span><span class="sxs-lookup"><span data-stu-id="2a81e-128">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="2a81e-129">Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2a81e-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="2a81e-130">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="2a81e-130">Next steps</span></span>

- [<span data-ttu-id="2a81e-131">Aggiungere utenti</span><span class="sxs-lookup"><span data-stu-id="2a81e-131">Add users</span></span>](create-user-accounts-and-set-permissions.md)
