---
title: Aggiungere altri tenant all'account del centro per i partner
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant di Azure AD nell'account del centro per i partner. Altre informazioni su alcuni dei motivi per cui si potrebbe voler eseguire questa operazione.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175159"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="745e7-104">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="745e7-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="745e7-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="745e7-105">**Applies to**</span></span>

- <span data-ttu-id="745e7-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="745e7-106">Partner Center</span></span>

<span data-ttu-id="745e7-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="745e7-107">**Appropriate roles**</span></span>

- <span data-ttu-id="745e7-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="745e7-108">Global admin</span></span>

<span data-ttu-id="745e7-109">Questa funzionalità consente all'utente di gestire più tenant per la propria azienda e di consolidarli nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="745e7-110">Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="745e7-111">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="745e7-111">For example:</span></span>

- <span data-ttu-id="745e7-112">L'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="745e7-113">Tuttavia, si vuole che le due società rimangano separate.</span><span class="sxs-lookup"><span data-stu-id="745e7-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="745e7-114">In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="745e7-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="745e7-115">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="745e7-116">Se si dispone di più tenant per l'esecuzione dell'attività, ad esempio contoso.com, contoso.uk, contoso.in, è possibile usare il multi-tenant per collegarli con lo stesso account del computer.</span><span class="sxs-lookup"><span data-stu-id="745e7-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="745e7-117">Per le fusioni e le acquisizioni è necessario usare più di un tenant (ad esempio, se contoso acquisisce Fabrikam, è necessario poter usare sia Constoso.com che Fabrikam.com rispettivi tenant).</span><span class="sxs-lookup"><span data-stu-id="745e7-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="745e7-118">È necessario che gli utenti di uno dei tenant siano in grado di:</span><span class="sxs-lookup"><span data-stu-id="745e7-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="745e7-119">Accedi al centro per i partner per corsi di formazione, download digitali, associazione MCP</span><span class="sxs-lookup"><span data-stu-id="745e7-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="745e7-120">Sono assegnati ruoli del centro per i partner, ad esempio MPN admin, incentives admin e così via.</span><span class="sxs-lookup"><span data-stu-id="745e7-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="745e7-121">Aggiungere un altro tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="745e7-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="745e7-122">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="745e7-123">Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="745e7-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associa tenant"::: 

3. <span data-ttu-id="745e7-125">Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="745e7-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="745e7-126">Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="745e7-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="associa tenant"::: 

5. <span data-ttu-id="745e7-128">Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="745e7-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="745e7-129">Selezionare **Torna a gestione tenant per** visualizzare l'elenco dei tenant appena aggiunti.</span><span class="sxs-lookup"><span data-stu-id="745e7-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="745e7-130">Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="745e7-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="745e7-131">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="745e7-131">Next steps</span></span>

- [<span data-ttu-id="745e7-132">Aggiungere utenti</span><span class="sxs-lookup"><span data-stu-id="745e7-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
