---
title: Installare Partner Center Analytics per Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Eseguire la procedura descritta in questo articolo per installare e visualizzare in anteprima l'app partner Center Analytics per Power BI (per i partner diretti in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e2a1d17a7520cca1a6e1da540cc58d2d365d8cb
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679308"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI

**Si applica a**

- Centro per i partner

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente di vendita
-   Agente amministratore

## <a name="before-you-begin"></a>Prima di iniziare

Selezionare l'applicazione più pertinente per l'azienda dal seguente elenco di app Power BI disponibili:
- [Provider diretto](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Provider indiretto](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Rivenditore indiretto](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Prima di installare la versione di anteprima dell'app partner Center Analytics, assicurarsi di soddisfare i requisiti seguenti.

- Si sceglie l'app Power BI corretta per l'azienda.

- Si dispone di una licenza di Power BI Pro.

- Si dispone delle autorizzazioni per installare le app modello nel tenant.

- È possibile accedere a Power BI.

- È possibile accedere come amministratore globale, agente di amministrazione o amministratore della fatturazione al [tenant di Azure Active Directory (Azure ad) dell'azienda](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Per installare l'app

1. Fare clic sul collegamento dell'origine app specificato (provider diretto/provider indiretto/rivenditore indiretto) nella sezione precedente.

2. Fare clic su **Ottieni ora**. 

3. Per accettare i termini e le condizioni, fare clic su **continua**.

4. In è già presente un account? Selezionare **Sign in (accedi**).

5. Nella pagina successiva immettere il nome utente e la password Power BI e quindi selezionare Accedi.

6. Installare l'area di lavoro fornendo l'area di lavoro.

7. È possibile trovare le app modello installate nella sezione app.

8. Fare clic su app e scegliere le app installate.

9. Viene visualizzata la schermata inizia con la nuova app.

10. Per connettersi ai dati, fare clic su **Connetti**.

11. Nella finestra popup **Connetti a partner Center Analytics** verificare che il **metodo di autenticazione** sia impostato su **OAuth2** o selezionare **OAuth2** nell'elenco, se non lo è. 

> [!NOTE]  
>  La visualizzazione di questa finestra potrebbe richiedere alcuni minuti.

12. Nella pagina del **connettore di analisi dei partner** , accedere con le credenziali di amministratore globale, agente di amministrazione o amministratore fatturazione per il tenant Azure ad della società e quindi selezionare **Accedi**.
 
13. Quando viene richiesto di accedere, selezionare **Accetto**. 

Quando il servizio di analisi dei partner Center è connesso alla Power BI, i dati inizieranno a essere caricati. A seconda della quantità di dati, l'operazione può richiedere fino a 10 minuti. 

Al termine del caricamento dei dati, è possibile iniziare a usare il dashboard dell'app partner Analytics e i report in Power BI.

## <a name="next-steps"></a>Passaggi successivi

[Visualizzare i dati aziendali con l'app partner Center Analytics per Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
