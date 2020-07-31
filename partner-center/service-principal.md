---
title: Entità servizio di Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come aggiungere un'entità servizio al tenant di Azure AD. Si tratta di aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365757"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale

Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nell'account del Centro per i partner. Questa operazione in precedenza veniva eseguita nell'account del portale Cloud Partner (CPP). Ora che è stata eseguita la migrazione al Centro per i partner, l'account CPP è di sola lettura.
 
>[!Note] 
>Entità servizio è sinonimo di applicazione Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Aggiungere un'applicazione Azure AD (entità servizio)

1. Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.

2. Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.

3. Selezionare un'applicazione Azure AD esistente o crearne una nuova.

4. Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:  

   - **URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD.

   - **URI ID app**: un identificatore logico per l'applicazione Azure AD che viene presentato quando invia una richiesta Single Sign-On ad Azure AD.

   - **Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.  

## <a name="next-steps"></a>Passaggi successivi

- [Panoramica del marketplace commerciale nel Centro per i partner](csp-commercial-marketplace-overview.md)