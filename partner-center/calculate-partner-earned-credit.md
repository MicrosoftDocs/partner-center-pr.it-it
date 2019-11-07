---
title: Come viene calcolato il credito guadagnato dal partner | Centro per i partner
ms.topic: article
ms.date: 09/17/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Calcolo dell'aspetto del credito del partner del piano Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 402ee0e2084191c7d4f592dd91480be8e1bd0341
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653714"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="6c5cc-103">Come viene calcolato il credito guadagnato dal partner (PEC)</span><span class="sxs-lookup"><span data-stu-id="6c5cc-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="6c5cc-104">I partner che possiedono la gestione operativa delle attività IT di 24 ore su 7 o l'intero ambiente Azure dei clienti in CSP sono ricompensati con PEC.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="6c5cc-105">Il PEC viene fornito come parte della fattura al partner che ha una relazione di fatturazione diretta con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="6c5cc-106">Il credito viene calcolato quotidianamente e riportato nella fattura mensile.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="6c5cc-107">Per impostazione predefinita, in CSP, ai partner vengono concessi i diritti di accesso necessari per la sottoscrizione del cliente che consente loro di disporre di gestione e controllo 24X7 delle risorse nella sottoscrizione.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-107">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="6c5cc-108">Nella sezione seguente sono descritti altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="6c5cc-109">Importanti requisiti di idoneità e calcolo:</span><span class="sxs-lookup"><span data-stu-id="6c5cc-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="6c5cc-110">Un partner deve avere un contratto MPN attivo e un ruolo di account C (RBAC) valido basato su regole per ricevere il credito guadagnato per le risorse di Azure che gestiscono.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="6c5cc-111">Altre informazioni su [ruoli RBAC validi]</span><span class="sxs-lookup"><span data-stu-id="6c5cc-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="6c5cc-112">Il provider indiretto sarà idoneo per PEC se l'utente o il rivenditore indiretto o entrambi hanno il controllo operativo e la gestione di 24x7 per le risorse di Azure del cliente in CSP.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="6c5cc-113">PEC è associato al consumo fatturato (addebitabile) delle proprietà di Azure del cliente in CSP gestito dal partner.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-113">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="6c5cc-114">PEC è disponibile solo per i partner in CSP fatturati da Microsoft (provider indiretto e Direct Bill partner).</span><span class="sxs-lookup"><span data-stu-id="6c5cc-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="6c5cc-115">Servizi idonei: il credito guadagnato dal partner è applicabile a tutti i consumi di Azure 1PP di Azure indicati nell'elenco prezzi.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="6c5cc-116">Sono presenti eccezioni tra cui, ma non limitate, 3PP e le prenotazioni di Azure.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="6c5cc-117">PEC viene calcolato quotidianamente e può essere visualizzato nel file di ricognizione giornaliero.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="6c5cc-118">Un partner (provider o rivenditore (tramite il provider) deve avere accesso per l'intero giorno (24x7) per assicurarsi che guadagni PEC.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="6c5cc-119">Il PEC viene raggiunto a livello di risorse di Azure.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="6c5cc-120">Se il partner dispone di un accesso valido a livello di sottoscrizione o di gruppo di risorse, ogni risorsa che fa parte dell'entità superiore guadagnerà PEC.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="6c5cc-121">PEC verrà incluso nella fattura mensile del partner.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="6c5cc-122">La fattura è il costo netto.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-122">The invoice is net of charges.</span></span> <span data-ttu-id="6c5cc-123">I dettagli vengono visualizzati nel file di ricognizione della fattura.</span><span class="sxs-lookup"><span data-stu-id="6c5cc-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="6c5cc-124">Per informazioni su come ottenere l'accesso per gestire le sottoscrizioni di Azure e su come collegare l'ID MPN ai ruoli RBAC, vedere [gestire sottoscrizioni e risorse nel piano Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="6c5cc-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="6c5cc-125">Ulteriori informazioni</span><span class="sxs-lookup"><span data-stu-id="6c5cc-125">For more information</span></span>

- [<span data-ttu-id="6c5cc-126">Piano di Azure-fatturazione</span><span class="sxs-lookup"><span data-stu-id="6c5cc-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="6c5cc-127">Listino prezzi per la nuova esperienza commerciale di Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="6c5cc-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)