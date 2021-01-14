---
title: Aggiungere altri tenant all'account del centro per i partner
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant di Azure AD nell'account del centro per i partner. Altre informazioni su alcuni dei motivi per cui si potrebbe voler eseguire questa operazione.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182435"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="91329-104">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="91329-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="91329-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="91329-105">**Appropriate roles**</span></span>

- <span data-ttu-id="91329-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="91329-106">Global admin</span></span>
- <span data-ttu-id="91329-107">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="91329-107">Account admin</span></span>

<span data-ttu-id="91329-108">Questa funzionalità consente all'utente di gestire più tenant per la propria azienda e di consolidarli nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="91329-109">Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="91329-110">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="91329-110">For example:</span></span>

- <span data-ttu-id="91329-111">L'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="91329-112">Tuttavia, si vuole che le due società rimangano separate.</span><span class="sxs-lookup"><span data-stu-id="91329-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="91329-113">In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="91329-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="91329-114">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="91329-115">Se si dispone di più tenant per l'esecuzione dell'attività, ad esempio contoso.com, contoso.uk, contoso.in, è possibile usare il multi-tenant per collegarli con lo stesso account del computer.</span><span class="sxs-lookup"><span data-stu-id="91329-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="91329-116">Per le fusioni e le acquisizioni è necessario usare più di un tenant (ad esempio, se contoso acquisisce Fabrikam, è necessario poter usare sia Constoso.com che Fabrikam.com rispettivi tenant).</span><span class="sxs-lookup"><span data-stu-id="91329-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="91329-117">È necessario che gli utenti di uno dei tenant siano in grado di:</span><span class="sxs-lookup"><span data-stu-id="91329-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="91329-118">Accedi al centro per i partner per corsi di formazione, download digitali, associazione MCP</span><span class="sxs-lookup"><span data-stu-id="91329-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="91329-119">Sono assegnati ruoli del centro per i partner, ad esempio MPN admin, incentives admin e così via.</span><span class="sxs-lookup"><span data-stu-id="91329-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="91329-120">Aggiungere un altro tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="91329-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="91329-121">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="91329-122">Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="91329-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associa tenant"::: 

3. <span data-ttu-id="91329-124">Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="91329-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="91329-125">Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="91329-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="conferma associazione tenant"::: 

5. <span data-ttu-id="91329-127">Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="91329-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="91329-128">Selezionare **Torna a gestione tenant per** visualizzare il tenant appena aggiunto.</span><span class="sxs-lookup"><span data-stu-id="91329-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="91329-129">Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="91329-130">Rimuovere un tenant dall'account</span><span class="sxs-lookup"><span data-stu-id="91329-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="91329-131">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="91329-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="91329-132">Nell'icona **Impostazioni** selezionare **impostazioni account** -> tenant e fare clic sulla scheda **partner** .</span><span class="sxs-lookup"><span data-stu-id="91329-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="91329-133">Fare clic su **Rimuovi** per il tenant a cui si desidera eseguire l'associazione.</span><span class="sxs-lookup"><span data-stu-id="91329-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="91329-134">L'annullamento dell'associazione di un tenant implica che gli utenti di tale tenant non avranno più accesso all'account del centro per i partner e questo potrebbe avere un effetto sulle competenze.</span><span class="sxs-lookup"><span data-stu-id="91329-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="91329-135">Il pulsante **Rimuovi** è abilitato per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi.</span><span class="sxs-lookup"><span data-stu-id="91329-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="tenant con il pulsante Rimuovi":::
 

## <a name="next-steps"></a><span data-ttu-id="91329-137">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="91329-137">Next steps</span></span>

- [<span data-ttu-id="91329-138">Aggiungere utenti</span><span class="sxs-lookup"><span data-stu-id="91329-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






