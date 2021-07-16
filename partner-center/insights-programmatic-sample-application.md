---
title: Applicazione di esempio
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare l'applicazione di esempio per compilare un'applicazione per accedere a livello di codice ai dati di informazioni dettagliate dei partner.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375343"
---
# <a name="sample-application"></a><span data-ttu-id="d8a36-103">Applicazione di esempio</span><span class="sxs-lookup"><span data-stu-id="d8a36-103">Sample Application</span></span>

<span data-ttu-id="d8a36-104">Le applicazioni di esempio vengono create nei linguaggi C# e JAVA e sono disponibili in [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="d8a36-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="d8a36-105">Applicazione di esempio C#</span><span class="sxs-lookup"><span data-stu-id="d8a36-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="d8a36-106">Applicazione di esempio JAVA</span><span class="sxs-lookup"><span data-stu-id="d8a36-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="d8a36-107">È possibile scegliere di ispirarsi all'applicazione di esempio e creare un'applicazione in qualsiasi linguaggio.</span><span class="sxs-lookup"><span data-stu-id="d8a36-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="d8a36-108">L'applicazione di esempio raggiunge gli obiettivi seguenti:</span><span class="sxs-lookup"><span data-stu-id="d8a36-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="d8a36-109">Genera un token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d8a36-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="d8a36-110">Ottiene i set di dati disponibili.</span><span class="sxs-lookup"><span data-stu-id="d8a36-110">Gets available datasets.</span></span>
- <span data-ttu-id="d8a36-111">Crea query definite dall'utente.</span><span class="sxs-lookup"><span data-stu-id="d8a36-111">Creates user defined queries.</span></span>
- <span data-ttu-id="d8a36-112">Ottiene query definite dall'utente e di sistema.</span><span class="sxs-lookup"><span data-stu-id="d8a36-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="d8a36-113">Pianifica un report.</span><span class="sxs-lookup"><span data-stu-id="d8a36-113">Schedules a report.</span></span>

<span data-ttu-id="d8a36-114">L'applicazione di esempio non tratta il metodo di chiamata delle API per altre funzionalità.</span><span class="sxs-lookup"><span data-stu-id="d8a36-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="d8a36-115">Tuttavia, il processo di chiamata di altre API rimane lo stesso descritto in precedenza.</span><span class="sxs-lookup"><span data-stu-id="d8a36-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="d8a36-116">Come eseguire l'applicazione</span><span class="sxs-lookup"><span data-stu-id="d8a36-116">How to run the application</span></span>

- <span data-ttu-id="d8a36-117">Clonare il repository in un sistema locale usando questo comando:</span><span class="sxs-lookup"><span data-stu-id="d8a36-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="d8a36-118">Per altre istruzioni, vedere il file ProgrammaticExportSampleAppMPN/README.md nel [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub .</span><span class="sxs-lookup"><span data-stu-id="d8a36-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="d8a36-119">Per eseguire rapidamente l'app, aggiornare l'ID client e il segreto client nelappsettings.Development.js **su**</span><span class="sxs-lookup"><span data-stu-id="d8a36-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustrazione del codice JSON di sviluppo di appsetting":::

<span data-ttu-id="d8a36-121">L'esecuzione dell'app avvia un server Web locale e viene aperta una pagina ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="d8a36-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustrazione dell'interfaccia utente dell'applicazione di esempio":::

<span data-ttu-id="d8a36-123">Questa pagina esegue chiamate API al server Web in esecuzione nel computer locale, che a sua volta effettua le chiamate API di accesso a livello di codice effettive.</span><span class="sxs-lookup"><span data-stu-id="d8a36-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="d8a36-124">Frammenti di codice</span><span class="sxs-lookup"><span data-stu-id="d8a36-124">Code Snippets</span></span>

<span data-ttu-id="d8a36-125">La struttura di base del codice C# per l'esecuzione delle chiamate API di accesso a livello di codice è la seguente:</span><span class="sxs-lookup"><span data-stu-id="d8a36-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustrazione del frammento di codice":::

## <a name="next-steps"></a><span data-ttu-id="d8a36-127">Passaggi successivi</span><span class="sxs-lookup"><span data-stu-id="d8a36-127">Next steps</span></span>

[<span data-ttu-id="d8a36-128">API per l'accesso ai dati di analisi delle informazioni dettagliate dei partner</span><span class="sxs-lookup"><span data-stu-id="d8a36-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
