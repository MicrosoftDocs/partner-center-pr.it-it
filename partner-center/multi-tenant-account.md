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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389516"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="622de-103">Aggiungere e gestire più tenant nell'account del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="622de-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="622de-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="622de-104">**Applies to**</span></span>

- <span data-ttu-id="622de-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="622de-105">Partner Center</span></span>

<span data-ttu-id="622de-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="622de-106">**Appropriate roles**</span></span>

- <span data-ttu-id="622de-107">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="622de-107">Global admin</span></span>

<span data-ttu-id="622de-108">Esistono molti motivi per cui potrebbe essere necessario gestire più tenant Azure AD nell'account del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="622de-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="622de-109">Ad esempio, l'azienda può acquistare un'altra società e si vuole che i dipendenti della nuova azienda possano usare il centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="622de-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="622de-110">Tuttavia, si vuole che le due società rimangano separate.</span><span class="sxs-lookup"><span data-stu-id="622de-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="622de-111">In questo caso, è necessario associare il tenant di Azure AD della nuova società con l'account globale del partner (PNG).</span><span class="sxs-lookup"><span data-stu-id="622de-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="622de-112">Questa associazione consente agli utenti di entrambe le aziende di lavorare nel centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="622de-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="622de-113">Aggiungere un altro tenant Azure AD all'account</span><span class="sxs-lookup"><span data-stu-id="622de-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="622de-114">Come amministratore globale, accedere al [Dashboard](https://partner.microsoft.com/dashboard)del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="622de-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="622de-115">Nell'icona **Impostazioni** selezionare **Impostazioni account** , quindi selezionare **tenant**.</span><span class="sxs-lookup"><span data-stu-id="622de-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="associa tenant"::: 

3. <span data-ttu-id="622de-117">Selezionare **associa un altro tenant di Active Directory** e indicare il tenant che si vuole associare.</span><span class="sxs-lookup"><span data-stu-id="622de-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="622de-118">Come amministratore globale, accedere al tenant che si vuole associare e confermare l'associazione.</span><span class="sxs-lookup"><span data-stu-id="622de-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="conferma associazione tenant"::: 

5. <span data-ttu-id="622de-120">Dopo la conferma, viene visualizzato un avviso relativo a **tutti i set** .</span><span class="sxs-lookup"><span data-stu-id="622de-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="622de-121">Selezionare **Torna a gestione tenant per** visualizzare l'elenco dei tenant appena aggiunti.</span><span class="sxs-lookup"><span data-stu-id="622de-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="622de-122">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="622de-122">Next steps</span></span>

- [<span data-ttu-id="622de-123">Aggiungere utenti</span><span class="sxs-lookup"><span data-stu-id="622de-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
