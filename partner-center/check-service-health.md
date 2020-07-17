---
title: Controllare l'integrità dei servizi per un cliente
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come usare il centro per i partner per verificare l'integrità dei servizi per un cliente quando si verifica un problema con un servizio.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 11ec4cfcfc9326c1e9d6598dce528410c0e02542
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435480"
---
# <a name="check-service-health-for-a-customer-reporting-a-potential-service-problem-or-outage"></a><span data-ttu-id="ffd9d-103">Verificare l'integrità dei servizi per un cliente che ha segnalato un potenziale problema o un'interruzione del servizio</span><span class="sxs-lookup"><span data-stu-id="ffd9d-103">Check service health for a customer reporting a potential service problem or outage</span></span>

<span data-ttu-id="ffd9d-104">**Si applica a**</span><span class="sxs-lookup"><span data-stu-id="ffd9d-104">**Applies to**</span></span>

- <span data-ttu-id="ffd9d-105">Centro per i partner</span><span class="sxs-lookup"><span data-stu-id="ffd9d-105">Partner Center</span></span>

<span data-ttu-id="ffd9d-106">**Ruoli appropriati**</span><span class="sxs-lookup"><span data-stu-id="ffd9d-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ffd9d-107">Agente amministratore</span><span class="sxs-lookup"><span data-stu-id="ffd9d-107">Admin agent</span></span>
- <span data-ttu-id="ffd9d-108">Amministratore globale</span><span class="sxs-lookup"><span data-stu-id="ffd9d-108">Global admin</span></span>
- <span data-ttu-id="ffd9d-109">Agente di supporto tecnico</span><span class="sxs-lookup"><span data-stu-id="ffd9d-109">Helpdesk agent</span></span>
- <span data-ttu-id="ffd9d-110">Agente di vendita</span><span class="sxs-lookup"><span data-stu-id="ffd9d-110">Sales agent</span></span>

<span data-ttu-id="ffd9d-111">Una delle prime cose che è possibile fare quando un cliente segnala problemi con un servizio è controllare l'integrità del servizio.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-111">One of the first things you can do when a customer is experiencing problems with a service is to check the service health.</span></span> 

## <a name="check-service-health"></a><span data-ttu-id="ffd9d-112">Controllare l'integrità del servizio</span><span class="sxs-lookup"><span data-stu-id="ffd9d-112">Check service health</span></span>

1. <span data-ttu-id="ffd9d-113">Selezionare il **cliente** che presenta il problema dall'elenco dei **clienti**.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-113">Select the **Customer** that is having the issue from the **Customer list**.</span></span>

2. <span data-ttu-id="ffd9d-114">Selezionare **Gestione servizi** dal menu a sinistra.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-114">Select **Service management** from the left menu.</span></span> <span data-ttu-id="ffd9d-115">In questo elenco vengono elencati i servizi di cui è stato effettuato il provisioning per il cliente e l'integrità del servizio per ognuno.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-115">This will list the services provisioned for the customer and the service health for each.</span></span> <span data-ttu-id="ffd9d-116">I partner possono fare clic sul servizio a cui sono interessati per ottenere altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-116">Partners can click the service they are interested in to get more information.</span></span> 

>[!NOTE] 
> <span data-ttu-id="ffd9d-117">I collegamenti per l'integrità dei servizi nelle pagine di **gestione dei servizi** porteranno il partner all'interfaccia di amministrazione di M365 o all'portale di Azure come **amministratore delegato**. Quando il partner raggiunge una destinazione, il partner può passare alle pagine di integrità del servizio in uno dei due portale per ulteriori dettagli sull'interruzione.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-117">Service health links on the **Service management** pages will take the partner to either the M365 admin center or the Azure portal as **delegated admin**. Once the partner gets to either destination, the partner can navigate to the service health pages in either portal for more details about the outage.</span></span>
 
<span data-ttu-id="ffd9d-118">Durante un'interruzione del servizio, Microsoft fornisce aggiornamenti periodici man mano che lavora per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-118">During a service outage, Microsoft provides regular updates as we work to address the problem.</span></span> <span data-ttu-id="ffd9d-119">Queste notifiche vengono visualizzate anche nel centro di amministrazione di portale di Microsoft Azure o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-119">These notifications are also displayed on either the Microsoft Azure portal or the Microsoft 365 admin Center.</span></span>

<span data-ttu-id="ffd9d-120">Se il problema persiste dopo la fine dell'interruzione del servizio, inviare una richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-120">If the problem persists after the end of the service outage, submit a service request.</span></span> <span data-ttu-id="ffd9d-121">Vedi [Segnalare problemi per conto di un cliente](report-problems-on-behalf-of-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="ffd9d-121">See [Report problems on behalf of a customer](report-problems-on-behalf-of-a-customer.md).</span></span>

<span data-ttu-id="ffd9d-122">Microsoft 365 e Microsoft Azure forniscono ogni [API che i partner possono utilizzare per recuperare l'integrità del servizio in tempo reale](get-automated-service-notifications-with-our-apis.md), le comunicazioni del centro messaggi e gli eventi di manutenzione pianificata.</span><span class="sxs-lookup"><span data-stu-id="ffd9d-122">Microsoft 365 and Microsoft Azure each provide [APIs that partners can use to retrieve real-time service health](get-automated-service-notifications-with-our-apis.md), message center communications, and planned maintenance events.</span></span>

 

