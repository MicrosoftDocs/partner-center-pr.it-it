---
title: Iscriversi come CPV (Control Panel Vendor)
description: Informazioni su come eseguire la registrazione come fornitore Pannello di controllo (CPV) in Partner Center in modo da poter integrare meglio i sistemi partner CSP con Partner Center API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147140"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="e1040-103">Iscriversi come fornitore del pannello di controllo per integrare i sistemi di partner CSP con le API del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="e1040-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="e1040-104">**Ruoli appropriati**: Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="e1040-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e1040-105">Un Pannello di controllo Vendor (CPV) è un fornitore di software indipendente che sviluppa applicazioni per l'uso da parte di partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="e1040-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="e1040-106">Un Pannello di controllo fornitore non è un partner CSP con accesso diretto al dashboard Partner Center o alle API Partner Center client.</span><span class="sxs-lookup"><span data-stu-id="e1040-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="e1040-107">Sia che si sia un fornitore di Pannello di controllo (CPV) o un nuovo CPV che vuole collaborare con i partner Microsoft, Microsoft richiede ora la registrazione a Partner Center per registrare le applicazioni e supportare i partner Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="e1040-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="e1040-108">Per creare un account, un partner CPV può usare un tenant partner CSP esistente o un tenant CPV esistente oppure creare un nuovo tenant come parte del processo di onboarding.</span><span class="sxs-lookup"><span data-stu-id="e1040-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="e1040-109">Se il partner CPV sceglie di usare il tenant CSP esistente, dovrà creare applicazioni multi-tenant separate e registrarle in Partner Center per le attività CPV.</span><span class="sxs-lookup"><span data-stu-id="e1040-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="e1040-110">Un'applicazione non può essere registrata come applicazione CSP e CPV.</span><span class="sxs-lookup"><span data-stu-id="e1040-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="e1040-111">Dopo aver registrato in Partner Center e registrato le applicazioni, si avrà accesso alle API Partner Center applicazioni.</span><span class="sxs-lookup"><span data-stu-id="e1040-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="e1040-112">Contattare Microsoft tramite una Supporto tecnico Microsoft richiesta se è necessario un account sandbox.</span><span class="sxs-lookup"><span data-stu-id="e1040-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="e1040-113">Se si ha già un account sandbox, continuare a usarlo.</span><span class="sxs-lookup"><span data-stu-id="e1040-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="e1040-114">Non sarà necessaria una nuova sandbox</span><span class="sxs-lookup"><span data-stu-id="e1040-114">You won't need a new sandbox</span></span>

<span data-ttu-id="e1040-115">Esaminare il [contratto microsoft Pannello di controllo vendor](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="e1040-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="e1040-116">Lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="e1040-116">Working in Partner Center</span></span>

<span data-ttu-id="e1040-117">Dopo aver registrato l'esperienza Partner Center CPV e aver accettato il contratto CPV, è possibile:</span><span class="sxs-lookup"><span data-stu-id="e1040-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="e1040-118">Gestire applicazioni multi-tenant (aggiungere applicazioni per portale di Azure, registrare e annullare la registrazione delle applicazioni in Partner Center).</span><span class="sxs-lookup"><span data-stu-id="e1040-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="e1040-119">I CPV devono registrare le applicazioni in Partner Center per ottenere l'autorizzazione per Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="e1040-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="e1040-120">La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="e1040-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="e1040-121">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="e1040-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="e1040-122">Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo.</span><span class="sxs-lookup"><span data-stu-id="e1040-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="e1040-123">L'amministratore globale è l'unico ruolo che un CPV può avere.</span><span class="sxs-lookup"><span data-stu-id="e1040-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e1040-124">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="e1040-124">Next steps</span></span>

<span data-ttu-id="e1040-125">-[Aggiungere altri tenant all'account Partner Center locale](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="e1040-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>