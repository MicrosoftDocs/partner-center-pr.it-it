---
title: Aggiungere i tenant all'account del centro per i partner
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant di Azure AD nell'account del centro per i partner e per informazioni sul motivo per cui è possibile eseguire questa operazione.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124806"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="d8bab-103">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d8bab-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="d8bab-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="d8bab-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d8bab-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="d8bab-105">Global admin</span></span>
- <span data-ttu-id="d8bab-106">Amministratore degli account</span><span class="sxs-lookup"><span data-stu-id="d8bab-106">Account admin</span></span>

<span data-ttu-id="d8bab-107">Questo articolo illustra come consolidare più tenant di Azure Active Directory (Azure AD) per la società e quindi aggiungerli e gestirli nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d8bab-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="d8bab-108">Esistono diversi motivi per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="d8bab-108">There are many reasons to do so.</span></span> <span data-ttu-id="d8bab-109">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="d8bab-109">For example:</span></span>

- <span data-ttu-id="d8bab-110">Supponiamo che l'azienda, contoso, abbia acquisito un'altra società, fabrikam.</span><span class="sxs-lookup"><span data-stu-id="d8bab-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="d8bab-111">Si vuole che le due società rimangano separate, ma si vuole che i nuovi dipendenti siano in grado di usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d8bab-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="d8bab-112">In questo caso, associare il tenant Azure AD della nuova società con l'account globale del partner (PGA).</span><span class="sxs-lookup"><span data-stu-id="d8bab-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="d8bab-113">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d8bab-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="d8bab-114">Se si esegue l'attività aziendale con più di un tenant, ad esempio *contoso.com*, *contoso.uk* e *contoso.in*, è possibile usare la multitenant per raggrupparli nello stesso account PC.</span><span class="sxs-lookup"><span data-stu-id="d8bab-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="d8bab-115">Se le linee guida per fusioni e acquisizioni richiedono l'uso di tenant di entrambe le società, si useranno entrambi i tenant *constoso.com* e *Fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="d8bab-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="d8bab-116">Gli utenti di qualsiasi tenant devono poter:</span><span class="sxs-lookup"><span data-stu-id="d8bab-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="d8bab-117">Accedi al centro per i partner per corsi di formazione, download digitali o associazione Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="d8bab-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="d8bab-118">Sono assegnati ruoli del centro per i partner, ad esempio l'amministratore di Microsoft Partner Network (MPN) o gli incentivi.</span><span class="sxs-lookup"><span data-stu-id="d8bab-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="d8bab-119">Aggiungere un tenant di Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="d8bab-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="d8bab-120">Accedere come amministratore globale al centro per i [partner Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d8bab-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="d8bab-121">In alto a destra selezionare **Impostazioni**, selezionare **Impostazioni account**, quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="d8bab-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot del pulsante associa nel riquadro del profilo Azure AD."::: 

1. <span data-ttu-id="d8bab-123">Selezionare **associa** e quindi indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="d8bab-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="d8bab-124">Al prompt accedere come amministratore globale al tenant che si vuole associare, quindi selezionare **Confirm (conferma**).</span><span class="sxs-lookup"><span data-stu-id="d8bab-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot del pulsante conferma del riquadro Conferma nuova associazione Azure AD."::: 

   <span data-ttu-id="d8bab-126">Una volta confermata l'associazione, viene visualizzato un messaggio di **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="d8bab-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="d8bab-127">Per visualizzare il tenant appena aggiunto, selezionare **Torna a gestione tenant**.</span><span class="sxs-lookup"><span data-stu-id="d8bab-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="d8bab-128">Non è possibile associare un tenant a un account se è già associato a un altro account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d8bab-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="d8bab-129">Rimuovere un tenant dall'account</span><span class="sxs-lookup"><span data-stu-id="d8bab-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="d8bab-130">Accedere come amministratore globale al centro per i [partner Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d8bab-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="d8bab-131">In alto a destra, selezionare l'icona **delle impostazioni** e quindi selezionare **Impostazioni account**.</span><span class="sxs-lookup"><span data-stu-id="d8bab-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="d8bab-132">Nel riquadro sinistro selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="d8bab-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="d8bab-133">In **gestisci Azure ad tenant** selezionare la scheda **partner** .</span><span class="sxs-lookup"><span data-stu-id="d8bab-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="d8bab-134">Selezionare **Rimuovi** accanto al tenant di cui si vuole rimuovere l'associazione.</span><span class="sxs-lookup"><span data-stu-id="d8bab-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot delle associazioni del tenant corrente e dei relativi collegamenti di rimozione.":::

   <span data-ttu-id="d8bab-136">Come illustrato nella schermata precedente, i collegamenti di **rimozione** sono abilitati per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi.</span><span class="sxs-lookup"><span data-stu-id="d8bab-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="d8bab-137">Quando si rimuove un tenant, gli utenti del tenant non hanno più accesso all'account del centro per i partner e la rimozione potrebbe avere un effetto sulle competenze.</span><span class="sxs-lookup"><span data-stu-id="d8bab-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="d8bab-138">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d8bab-138">Next steps</span></span>

- [<span data-ttu-id="d8bab-139">Creare account utente</span><span class="sxs-lookup"><span data-stu-id="d8bab-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






