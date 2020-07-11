---
title: Iscriversi come CPV (Control Panel Vendor)
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come eseguire la registrazione come un produttore del pannello di controllo (CPV) nel centro per i partner.
author: kbangalore
ms.author: kiranban
keywords: Fornitore del pannello di controllo, registrazione delle app CPV, gestione delle app CPV
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 819c814333878efc882749a1597e993eb9002545
ms.sourcegitcommit: 13b0e1358dc306f896190088d31a0d883644850f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/10/2020
ms.locfileid: "86219609"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="d9f26-104">Eseguire la registrazione come fornitore del pannello di controllo per integrare i sistemi partner CSP con le API del centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9f26-104">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="d9f26-105">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="d9f26-105">**Applies to**</span></span>

- <span data-ttu-id="d9f26-106">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9f26-106">Partner Center</span></span>

<span data-ttu-id="d9f26-107">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="d9f26-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d9f26-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="d9f26-108">Global admin</span></span>

<span data-ttu-id="d9f26-109">Un produttore del pannello di controllo (CPV) è un fornitore di software indipendente che sviluppa applicazioni per l'uso da parte dei partner Cloud Solution Provider (CSP) per consentire loro di integrare i propri sistemi con le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9f26-109">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="d9f26-110">Un fornitore del pannello di controllo non è un partner CSP con accesso diretto al dashboard del centro per i partner o alle API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9f26-110">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="d9f26-111">Se si è un fornitore del pannello di controllo (CPV) o un nuovo CPV che vuole collaborare con i partner Microsoft, ora Microsoft richiede di iscriversi a partner Center per registrare le applicazioni e supportare i partner Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="d9f26-111">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="d9f26-112">Per creare un account, un partner CPV può usare un tenant del partner CSP esistente o un tenant CPV esistente oppure può creare un nuovo tenant come parte del processo di onboarding.</span><span class="sxs-lookup"><span data-stu-id="d9f26-112">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="d9f26-113">Se il partner CPV sceglie di usare il tenant CSP esistente, sarà necessario creare applicazioni multi-tenant separate e registrarle nel centro per i partner per le attività CPV.</span><span class="sxs-lookup"><span data-stu-id="d9f26-113">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="d9f26-114">Un'applicazione non può essere registrata come applicazione CSP e CPV.</span><span class="sxs-lookup"><span data-stu-id="d9f26-114">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="d9f26-115">Dopo aver eseguito la registrazione nel centro per i partner e aver registrato le applicazioni, sarà possibile accedere alle API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9f26-115">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="d9f26-116">Microsoft contatterà l'utente tramite una notifica del centro per i partner con le informazioni sulla sandbox.</span><span class="sxs-lookup"><span data-stu-id="d9f26-116">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="d9f26-117">Se si dispone già di un account sandbox, continuare a usarlo.</span><span class="sxs-lookup"><span data-stu-id="d9f26-117">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="d9f26-118">Non è necessario un nuovo sandbox.</span><span class="sxs-lookup"><span data-stu-id="d9f26-118">You won't need a new sandbox.</span></span>

<span data-ttu-id="d9f26-119">Esaminare il [contratto del fornitore del pannello di controllo Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="d9f26-119">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="d9f26-120">Lavorare nel Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="d9f26-120">Working in Partner Center</span></span>
<span data-ttu-id="d9f26-121">Dopo aver eseguito la registrazione nell'esperienza CPV del centro per i partner e aver accettato il contratto CPV, è possibile:</span><span class="sxs-lookup"><span data-stu-id="d9f26-121">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="d9f26-122">Consente di gestire applicazioni multi-tenant (aggiungere applicazioni per portale di Azure, registrare e annullare la registrazione delle applicazioni nel centro per i partner).</span><span class="sxs-lookup"><span data-stu-id="d9f26-122">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="d9f26-123">CPVs deve registrare le proprie applicazioni nel centro per i partner per ottenere l'autorizzazione per le API del centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9f26-123">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="d9f26-124">La semplice aggiunta di applicazioni al portale di Azure non fornisce alle applicazioni dei fornitori di pannelli di controllo l'autorizzazione ad accedere alle API del Centro per i partner.</span><span class="sxs-lookup"><span data-stu-id="d9f26-124">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="d9f26-125">Visualizzazione e gestione del profilo dei fornitori di pannelli di controllo</span><span class="sxs-lookup"><span data-stu-id="d9f26-125">View and manage your CPV profile</span></span> 

- <span data-ttu-id="d9f26-126">Visualizzare e gestire gli utenti che devono accedere alle funzionalità dei fornitori di pannelli di controllo.</span><span class="sxs-lookup"><span data-stu-id="d9f26-126">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="d9f26-127">L'amministratore globale è l'unico ruolo che un CPV può avere.</span><span class="sxs-lookup"><span data-stu-id="d9f26-127">Global admin is the only role a CPV can have.</span></span>


