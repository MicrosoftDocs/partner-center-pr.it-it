---
title: Iscriversi come CPV (Control Panel Vendor)
description: Informazioni su come eseguire la registrazione come un produttore del pannello di controllo (CPV) nel centro per i partner per integrare meglio i sistemi partner CSP con le API del centro per i partner.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: 5fd2267d53641fe4a0b6181217a35f0470e5bbe5
ms.sourcegitcommit: 7681c6fc51e78cba106c46a52f6bb27e1a5c1c6b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "98560511"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="708d9-103">Iscriversi come fornitore del pannello di controllo per integrare i sistemi di partner CSP con le API del Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="708d9-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="708d9-104">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="708d9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="708d9-105">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="708d9-105">Global admin</span></span>

<span data-ttu-id="708d9-106">Un produttore del pannello di controllo (CPV) è un fornitore di software indipendente che sviluppa applicazioni per l'uso da parte dei partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="708d9-106">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="708d9-107">Un fornitore del pannello di controllo non è un partner CSP con accesso diretto al dashboard del centro per i partner o alle API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="708d9-107">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="708d9-108">Se si è un fornitore del pannello di controllo (CPV) o un nuovo CPV che vuole collaborare con i partner Microsoft, ora Microsoft richiede di iscriversi a partner Center per registrare le applicazioni e supportare i partner Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="708d9-108">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="708d9-109">Per creare un account, un partner CPV può usare un tenant del partner CSP esistente o un tenant CPV esistente oppure può creare un nuovo tenant come parte del processo di onboarding.</span><span class="sxs-lookup"><span data-stu-id="708d9-109">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="708d9-110">Se il partner CPV sceglie di usare il tenant CSP esistente, sarà necessario creare applicazioni multi-tenant separate e registrarle nel centro per i partner per le attività CPV.</span><span class="sxs-lookup"><span data-stu-id="708d9-110">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="708d9-111">Un'applicazione non può essere registrata come applicazione CSP e CPV.</span><span class="sxs-lookup"><span data-stu-id="708d9-111">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="708d9-112">Dopo aver eseguito la registrazione nel centro per i partner e aver registrato le applicazioni, sarà possibile accedere alle API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="708d9-112">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="708d9-113">Se è necessario un account sandbox, contattare Microsoft tramite una richiesta supporto tecnico Microsoft.</span><span class="sxs-lookup"><span data-stu-id="708d9-113">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="708d9-114">Se si dispone già di un account sandbox, continuare a usarlo.</span><span class="sxs-lookup"><span data-stu-id="708d9-114">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="708d9-115">Non è necessario un nuovo sandbox</span><span class="sxs-lookup"><span data-stu-id="708d9-115">You won't need a new sandbox</span></span>

<span data-ttu-id="708d9-116">Esaminare il [contratto del fornitore del pannello di controllo Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="708d9-116">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="708d9-117">Lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="708d9-117">Working in Partner Center</span></span>

<span data-ttu-id="708d9-118">Dopo aver eseguito la registrazione nell'esperienza CPV del centro per i partner e aver accettato il contratto CPV, è possibile:</span><span class="sxs-lookup"><span data-stu-id="708d9-118">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="708d9-119">Consente di gestire applicazioni multi-tenant (aggiungere applicazioni per portale di Azure, registrare e annullare la registrazione delle applicazioni nel centro per i partner).</span><span class="sxs-lookup"><span data-stu-id="708d9-119">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="708d9-120">CPVs deve registrare le proprie applicazioni nel centro per i partner per ottenere l'autorizzazione per le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="708d9-120">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="708d9-121">La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="708d9-121">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="708d9-122">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="708d9-122">View and manage your CPV profile</span></span> 

- <span data-ttu-id="708d9-123">Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo.</span><span class="sxs-lookup"><span data-stu-id="708d9-123">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="708d9-124">L'amministratore globale è l'unico ruolo che un CPV può avere.</span><span class="sxs-lookup"><span data-stu-id="708d9-124">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="708d9-125">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="708d9-125">Next steps</span></span>

<span data-ttu-id="708d9-126">-[Aggiungere altri tenant all'account del centro per i partner](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="708d9-126">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>