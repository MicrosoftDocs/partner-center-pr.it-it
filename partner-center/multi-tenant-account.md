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
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105554"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="2df39-104">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="2df39-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="2df39-105">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="2df39-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2df39-106">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="2df39-106">Global admin</span></span>

<span data-ttu-id="2df39-107">Questa funzionalità consente all'utente di gestire più tenant per la propria azienda e di consolidarli nell'account del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="2df39-108">Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="2df39-109">Esempio:</span><span class="sxs-lookup"><span data-stu-id="2df39-109">For example:</span></span>

- <span data-ttu-id="2df39-110">L'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="2df39-111">Tuttavia, si vuole che le due società rimangano separate.</span><span class="sxs-lookup"><span data-stu-id="2df39-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="2df39-112">In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="2df39-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="2df39-113">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="2df39-114">Se si dispone di più tenant per l'esecuzione dell'attività, ad esempio contoso.com, contoso.uk, contoso.in, è possibile usare il multi-tenant per collegarli con lo stesso account del computer.</span><span class="sxs-lookup"><span data-stu-id="2df39-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="2df39-115">Per le fusioni e le acquisizioni è necessario usare più di un tenant (ad esempio, se contoso acquisisce Fabrikam, è necessario poter usare sia Constoso.com che Fabrikam.com rispettivi tenant).</span><span class="sxs-lookup"><span data-stu-id="2df39-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="2df39-116">È necessario che gli utenti di uno dei tenant siano in grado di:</span><span class="sxs-lookup"><span data-stu-id="2df39-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="2df39-117">Accedi al centro per i partner per corsi di formazione, download digitali, associazione MCP</span><span class="sxs-lookup"><span data-stu-id="2df39-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="2df39-118">Sono assegnati ruoli del centro per i partner, ad esempio MPN admin, incentives admin e così via.</span><span class="sxs-lookup"><span data-stu-id="2df39-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="2df39-119">Aggiungere un altro tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="2df39-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="2df39-120">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="2df39-121">Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="2df39-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="associa tenant"::: 

3. <span data-ttu-id="2df39-123">Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="2df39-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="2df39-124">Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="2df39-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="conferma associazione tenant"::: 

5. <span data-ttu-id="2df39-126">Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="2df39-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="2df39-127">Selezionare **Torna a gestione tenant per** visualizzare il tenant appena aggiunto.</span><span class="sxs-lookup"><span data-stu-id="2df39-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="2df39-128">Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="2df39-129">Rimuovere un tenant dall'account</span><span class="sxs-lookup"><span data-stu-id="2df39-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="2df39-130">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="2df39-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="2df39-131">Nell'icona **Impostazioni** selezionare **impostazioni account** -> tenant e fare clic sulla scheda **partner** .</span><span class="sxs-lookup"><span data-stu-id="2df39-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="2df39-132">Fare clic su **Rimuovi** per il tenant a cui si desidera eseguire l'associazione.</span><span class="sxs-lookup"><span data-stu-id="2df39-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="2df39-133">L'annullamento dell'associazione di un tenant implica che gli utenti di tale tenant non avranno più accesso all'account del centro per i partner e questo potrebbe avere un effetto sulle competenze.</span><span class="sxs-lookup"><span data-stu-id="2df39-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="2df39-134">Il pulsante **Rimuovi** è abilitato per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi.</span><span class="sxs-lookup"><span data-stu-id="2df39-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="tenant con il pulsante Rimuovi":::
 

## <a name="next-steps"></a><span data-ttu-id="2df39-136">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="2df39-136">Next steps</span></span>

- [<span data-ttu-id="2df39-137">Aggiungere utenti</span><span class="sxs-lookup"><span data-stu-id="2df39-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






