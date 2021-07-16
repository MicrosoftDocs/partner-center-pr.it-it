---
title: Prerequisiti per accedere ai dati di analisi a livello di codice
description: Prerequisiti per accedere ai dati di analisi a livello di codice
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375352"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Prerequisiti per accedere ai dati di analisi a livello di codice

**Ruoli appropriati:** Amministratore globale | Amministratore MPN

Prima di poter accedere a livello di codice ai dati di analisi delle informazioni dettagliate dei partner, è necessario soddisfare i requisiti seguenti.

## <a name="mpn-program-enrollment"></a>Registrazione al programma MPN

Per accedere ai dati di analisi delle informazioni dettagliate dei partner a livello di codice, è necessario essere registrati nel programma MPN e avere un account Partner Center partner. Per informazioni, vedere [Creare un account MPN in Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Creare Azure Active Directory (AAD)

Le normali credenziali utente non possono essere usate per l'accesso a livello di codice ai dati di Analisi Insights partner. Per accedere alle API di accesso a livello di codice, è necessario creare un'applicazione Azure Active Directory (AAD) insieme a un segreto (applicazione e accesso utente). Per informazioni su come creare un'applicazione AAD e un segreto, vedere [Avvio rapido: Registrare un'applicazione](/azure/active-directory/develop/quickstart-register-app) con il Microsoft Identity Platform.   L'autorizzazione è necessaria per accedere a Microsoft API Partner. Per informazioni su come aggiungere autorizzazioni, vedere Autenticazione [API Partner - Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Assegnare il ruolo Executive Report Viewer (ERV) all'utente

Per accedere ai dati di analisi delle informazioni dettagliate dei partner a livello di codice, è necessario disporre di Executive Report Viewer (ERV). Per informazioni su come assegnare il ruolo ERV all'utente, [Partner Center Insights'accesso in](insights-roles.md) base al ruolo - Partner Center

## <a name="generate-an-aad-token"></a>Generare un token AAD

È necessario generare un token AAD usando l'ID applicazione (client), il segreto client, l'ID utente e la password.   [Vedere qui](insights-programmatic-first-api-call.md#token-generation) per la procedura per generare il token AAD.

> [!Note]
> Il token è valido per un'ora.

## <a name="next-steps"></a>Passaggi successivi
[Paradigma di accesso a livello di codice](insights-programmatic-access-paradigm.md)