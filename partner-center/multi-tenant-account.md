---
title: Aggiungere tenant all'account Partner Center
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere, consolidare o gestire più tenant Azure AD nell'account Partner Center e sui motivi per cui è consigliabile farlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151203"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="b2226-103">Aggiungere e gestire più tenant nell'account Partner Center</span><span class="sxs-lookup"><span data-stu-id="b2226-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="b2226-104">**Ruoli appropriati:** amministratore globale | Amministratore account</span><span class="sxs-lookup"><span data-stu-id="b2226-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="b2226-105">Questo articolo illustra come consolidare più tenant Azure Active Directory (Azure AD) per l'azienda e quindi aggiungerli e gestirli nell'account Partner Center aziendale.</span><span class="sxs-lookup"><span data-stu-id="b2226-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="b2226-106">Esistono molti motivi per farlo.</span><span class="sxs-lookup"><span data-stu-id="b2226-106">There are many reasons to do so.</span></span> <span data-ttu-id="b2226-107">Esempio:</span><span class="sxs-lookup"><span data-stu-id="b2226-107">For example:</span></span>

- <span data-ttu-id="b2226-108">Si supponiamo che l'azienda Contoso abbia acquisito un'altra società, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="b2226-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="b2226-109">Si vuole che le due società rimangano separate, ma si vuole che i nuovi dipendenti possano usare Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b2226-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="b2226-110">In questo caso, si associa il tenant del Azure AD aziendale all'account globale del partner.</span><span class="sxs-lookup"><span data-stu-id="b2226-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="b2226-111">Questa associazione consente agli utenti di entrambe le società di lavorare in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="b2226-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="b2226-112">Se si esegue l'azienda con più tenant (ad esempio, *contoso.com*, *contoso.uk* e *contoso.in*), è possibile usare la multi-tenant per raggrupparli nello stesso account PC.</span><span class="sxs-lookup"><span data-stu-id="b2226-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="b2226-113">Se le linee guida per fusioni e acquisizioni richiedono l'uso  di tenant di entrambe le società, è necessario usare i tenant constoso.com e *fabrikam.com* tenant.</span><span class="sxs-lookup"><span data-stu-id="b2226-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="b2226-114">Gli utenti di uno dei tenant devono essere in grado di:</span><span class="sxs-lookup"><span data-stu-id="b2226-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="b2226-115">Accesso Partner Center per il training, i download digitali o l'associazione Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="b2226-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="b2226-116">Essere assegnati Partner Center ruoli, ad esempio amministratore Microsoft Partner Network (MPN) o amministratore incentivi.</span><span class="sxs-lookup"><span data-stu-id="b2226-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="b2226-117">Aggiungere un tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="b2226-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="b2226-118">Accedere come amministratore globale a [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b2226-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="b2226-119">In alto a destra selezionare **Impostazioni,** quindi **Impostazioni account** e infine **Tenant.**</span><span class="sxs-lookup"><span data-stu-id="b2226-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Screenshot del pulsante Associa nel riquadro Azure AD profilo."::: 

1. <span data-ttu-id="b2226-121">Selezionare **Associa** e quindi indicare il tenant da associare.</span><span class="sxs-lookup"><span data-stu-id="b2226-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="b2226-122">Al prompt accedere come amministratore globale al tenant che si vuole associare e quindi selezionare **Conferma**.</span><span class="sxs-lookup"><span data-stu-id="b2226-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Screenshot del pulsante Conferma nel riquadro Conferma nuova Azure AD associazione."::: 

   <span data-ttu-id="b2226-124">Dopo aver confermato l'associazione, viene visualizzato un messaggio Tutti **i** set.</span><span class="sxs-lookup"><span data-stu-id="b2226-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="b2226-125">Per visualizzare il tenant appena aggiunto, selezionare **Torna alla gestione del tenant.**</span><span class="sxs-lookup"><span data-stu-id="b2226-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="b2226-126">Non è possibile associare un tenant a un account se è già associato a un altro Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="b2226-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="b2226-127">Rimuovere un tenant dall'account</span><span class="sxs-lookup"><span data-stu-id="b2226-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="b2226-128">Accedere come amministratore globale a [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b2226-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="b2226-129">In alto a destra selezionare **l'icona Impostazioni** e quindi Selezionare **Impostazioni account**.</span><span class="sxs-lookup"><span data-stu-id="b2226-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="b2226-130">Nel riquadro sinistro selezionare **Tenant**.</span><span class="sxs-lookup"><span data-stu-id="b2226-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="b2226-131">In **Gestisci Azure AD tenant** selezionare la scheda **Partner.**</span><span class="sxs-lookup"><span data-stu-id="b2226-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="b2226-132">Selezionare **Rimuovi** accanto al tenant di cui si vuole rimuovere l'associazione.</span><span class="sxs-lookup"><span data-stu-id="b2226-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Screenshot delle associazioni di tenant correnti e dei relativi collegamenti Rimuovi.":::

   <span data-ttu-id="b2226-134">Come illustrato nello screenshot precedente, i collegamenti Rimuovi sono abilitati per tutti i tenant associati, ad eccezione del tenant primario e del tenant a cui si è attualmente connessi. </span><span class="sxs-lookup"><span data-stu-id="b2226-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="b2226-135">Quando si rimuove un tenant, gli utenti in tale tenant non hanno più accesso all'account Partner Center e la rimozione potrebbe avere un impatto sulle competenze.</span><span class="sxs-lookup"><span data-stu-id="b2226-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="b2226-136">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="b2226-136">Next steps</span></span>

- [<span data-ttu-id="b2226-137">Creare account utente</span><span class="sxs-lookup"><span data-stu-id="b2226-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






