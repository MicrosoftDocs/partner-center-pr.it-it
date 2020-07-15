---
title: Gestione dei costi di Azure di Cloudyn per CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come registrare l'app Web Cloudyn e usare una chiave privata per l'app nel centro per i partner, in modo da poter usare l'app per tenere traccia dell'utilizzo e dei costi di Azure per i clienti.
author: aparnagkrishnan
ms.author: aparnag
Keywords: App gestione costi di Azure, Gestisci costi, app Web
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 521501f9a979c0993d299ab30443168408656a44
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390448"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Tieni traccia dell'utilizzo e dei costi di Azure per i clienti con l'app gestione costi di Azure per i partner CSP  

**Si applica a**

- Centro per i partner
- Partner del programma Cloud Solution Provider

**Ruoli appropriati**

- Amministratore globale
- Agente amministratore

[Ottenere altre informazioni su gestione costi di Azure](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Prima di iniziare
Prima di poter usare gestione costi di Azure, assicurarsi di soddisfare i requisiti seguenti:

- Si è partner del programma Cloud Solution Provider.
- Si ha la possibilità di creare un'app Web per le API del centro per i partner.

## <a name="overview"></a>Panoramica

Cloudyn è un'app Web che consente di tenere traccia e gestire la quantità di utilizzo di Azure da parte dei clienti e i costi dell'utilizzo. Viene usato tramite l'API del centro per i partner.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrare l'app Web nel centro per i partner
Quando si registra un'app Web Azure Active Directory nel centro per i partner, si Abilita l'accesso all'API del centro per i partner. 
1.  Accedere [al centro per i partner](https://partnercenter.microsoft.com/pcv/dashboard/overview) usando un [account di amministratore globale o di amministratore](create-user-accounts-and-set-permissions.md).
2.  Dal centro per i **partner**selezionare **Impostazioni account** &gt; **[gestione app](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  Nella sezione **app Web** fare clic su **Aggiungi nuova app Web**.
<br> **Nota**: se in precedenza è stata creata un'app Web, è possibile ignorare il passaggio 3.
4.  Copiare e salvare il GUID **ID Commerce** e il GUID **ID app** per l'app Web. Sono necessari entrambi gli ID per usare la versione di valutazione gratuita di 30 giorni dell'app gestione costi di Azure.

## <a name="add-a-secret-key-to-your-app"></a>Aggiungere una chiave privata all'app
1. Nell'elenco a discesa accanto al pulsante **Aggiungi chiave** selezionare una durata di 1 o 2 anni.
2. Fare clic su **Aggiungi chiave**. 
3. Copiare e salvare il valore della chiave privata. Questa operazione sarà necessaria per la versione di valutazione gratuita di 30 giorni.<br>
   > [!NOTE]  
   > Le chiavi segrete dell'applicazione sono simili alle password con date di scadenza più lunghe. Salvare il valore della chiave in un percorso sicuro per un uso futuro.

## <a name="next-steps"></a>Passaggi successivi
Avviare una [versione di valutazione gratuita di 30 giorni](https://go.microsoft.com/fwlink/?linkid=857895).
Per avviare la versione di valutazione sono necessari i dettagli seguenti:
- Credenziali di accesso al centro per i partner
- GUID ID Commerce
- GUID ID app
- Valore della chiave privata dell'applicazione
