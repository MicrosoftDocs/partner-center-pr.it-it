---
title: Installare Partner Center Analytics per Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seguire la procedura descritta in questo articolo per installare e visualizzare in anteprima il app Analisi del Centro per i Partner per Power BI (per i partner diretti in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854486"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI


**Ruoli appropriati:** amministratore globale | Amministratore gestione utenti | Agente di vendita | Agente amministratore

## <a name="before-you-begin"></a>Prima di iniziare

Selezionare l'applicazione più rilevante per l'azienda dall'elenco seguente di app Power BI disponibili:

- [Provider diretto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Provider indiretto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Rivenditore indiretto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Prima di installare la versione Partner Center anteprima dell'app Analytics, assicurarsi di soddisfare i requisiti seguenti.

- Scegliere l'app Power BI corretta per l'azienda.

- Si ha una licenza Power BI Pro.

- Si dispone delle autorizzazioni per installare le app modello nel tenant.

- È possibile accedere a Power BI.

- È possibile accedere come amministratore globale, agente amministratore o amministratore fatturazione al tenant di Azure Active Directory [aziendale (Azure AD).](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Per installare l'app

1. Selezionare il collegamento all'origine dell'app specificato (Provider diretto/Provider indiretto/Rivenditore indiretto) nella sezione precedente.

2. Selezionare **SCARICA ADESSO**. 

3. Accettare termini e condizioni selezionando **Continua.**

4. In Hai già un account? Selezionare **Accedi.**

5. Nella pagina successiva immettere il nome utente e Power BI password e quindi selezionare **Accedi.**

6. Installare l'area di lavoro specificando il nome dell'area di lavoro.

7. È possibile trovare le app modello installate nella sezione App.

8. Selezionare **App** e scegliere le app installate.

9. Viene visualizzata la schermata Introduzione alla nuova app.

10. Per connettersi ai dati, selezionare **Connetti**.

11. Nella finestra popup Connetti **a Partner Center Analytics** verificare  che il metodo di autenticazione sia impostato su **oAuth2** o selezionare **oAuth2** nell'elenco, in caso contrario. 

> [!NOTE]  
>  La visualizzazione di questa finestra potrebbe richiedere alcuni minuti.

12. Nella pagina **Partner Center Analytics Connector** accedere con le credenziali di amministratore globale, agente amministratore o amministratore della fatturazione per il tenant Azure AD aziendale e quindi selezionare Accedi . 
 
13. Quando viene richiesto l'accesso, selezionare **Accetta**. 

Quando il Partner Center Analytics è connesso a Power BI, i dati inizieranno a essere caricati. A seconda della quantità di dati, questa operazione può richiedere fino a 10 minuti. 

Al termine del caricamento dei dati, è possibile iniziare a usare il dashboard dell'app Partner Center Analytics e i report in Power BI.

## <a name="next-steps"></a>Passaggi successivi

[Visualizzare i dati aziendali con l'app Partner Center Analytics per Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
