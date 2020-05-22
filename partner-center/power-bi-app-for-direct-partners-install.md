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
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795869"
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
- [Partner diretto](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Partner indiretto](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Rivenditore indiretto](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Prima di installare la versione di anteprima dell'app partner Center Analytics, assicurarsi di soddisfare i requisiti seguenti.

- Si sceglie l'app Power BI corretta per l'azienda.

- Si dispone di una sottoscrizione attiva a Microsoft Power BI Professional o Microsoft Power BI Premium.

- È possibile accedere a Power BI.

- È possibile accedere come amministratore globale, agente di amministrazione o amministratore della fatturazione al [tenant di Azure Active Directory (Azure ad) dell'azienda](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Per installare l'app

1. Avviare [il processo di installazione](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. In **avere già un account?** selezionare **Accedi**. 

3. Nella pagina successiva immettere il nome utente e la password Power BI e quindi selezionare **Accedi**. 

4. Nella finestra popup **Connetti a partner Center Analytics** verificare che il **metodo di autenticazione** sia impostato su **OAuth2** o selezionare **OAuth2** nell'elenco, se non lo è. 

> [!NOTE]  
>  La visualizzazione di questa finestra potrebbe richiedere alcuni minuti.

5. Nella pagina del **connettore di analisi dei partner** , accedere con le credenziali di amministratore globale, agente di amministrazione o amministratore fatturazione per il tenant Azure ad della società e quindi selezionare **Accedi**.
 
6. Quando viene richiesto di accedere, selezionare **Accetto**. 

Quando il servizio di analisi dei partner Center è connesso alla Power BI, i dati inizieranno a essere caricati. A seconda della quantità di dati, l'operazione può richiedere fino a 10 minuti. 

Al termine del caricamento dei dati, è possibile iniziare a usare il dashboard dell'app partner Analytics e i report in Power BI.

## <a name="next-steps"></a>Passaggi successivi

[Visualizzare i dati aziendali con l'app partner Center Analytics per Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
