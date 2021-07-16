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
# <a name="sample-application"></a>Applicazione di esempio

Le applicazioni di esempio vengono create nei linguaggi C# e JAVA e sono disponibili in [GitHub](https://github.com/partneranalytics)

- [Applicazione di esempio C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Applicazione di esempio JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

È possibile scegliere di ispirarsi all'applicazione di esempio e creare un'applicazione in qualsiasi linguaggio.

L'applicazione di esempio raggiunge gli obiettivi seguenti:

- Genera un token Azure Active Directory (Azure AD).
- Ottiene i set di dati disponibili.
- Crea query definite dall'utente.
- Ottiene query definite dall'utente e di sistema.
- Pianifica un report.

L'applicazione di esempio non tratta il metodo di chiamata delle API per altre funzionalità. Tuttavia, il processo di chiamata di altre API rimane lo stesso descritto in precedenza.

## <a name="how-to-run-the-application"></a>Come eseguire l'applicazione

- Clonare il repository in un sistema locale usando questo comando:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Per altre istruzioni, vedere il file ProgrammaticExportSampleAppMPN/README.md nel [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub .

- Per eseguire rapidamente l'app, aggiornare l'ID client e il segreto client nelappsettings.Development.js **su**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Illustrazione del codice JSON di sviluppo di appsetting":::

L'esecuzione dell'app avvia un server Web locale e viene aperta una pagina ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Illustrazione dell'interfaccia utente dell'applicazione di esempio":::

Questa pagina esegue chiamate API al server Web in esecuzione nel computer locale, che a sua volta effettua le chiamate API di accesso a livello di codice effettive.

## <a name="code-snippets"></a>Frammenti di codice

La struttura di base del codice C# per l'esecuzione delle chiamate API di accesso a livello di codice è la seguente:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Illustrazione del frammento di codice":::

## <a name="next-steps"></a>Passaggi successivi

[API per l'accesso ai dati di analisi delle informazioni dettagliate dei partner](insights-programmatic-analytics-available-api.md)
