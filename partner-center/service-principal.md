---
title: Entità servizio di Azure AD | Centro per i partner
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aggiungere un'entità servizio al tenant di Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, piano di Azure, entità servizio, applicazione Azure AD
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010382"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Aggiungere un'applicazione Azure AD (entità servizio) nel Centro per i partner

Nel programma Commercial Marketplace del Centro per i partner è ora possibile aggiungere un'applicazione Azure AD (entità servizio) come utente nel tenant di Azure AD. Questa operazione era possibile in precedenza nell'account del portale Cloud Partner, ma dopo la migrazione al Centro per i partner, tale account è diventato di sola lettura. Si noti che entità servizio è sinonimo di applicazione Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Aggiungere un'applicazione Azure AD (entità servizio)

1. Nel dashboard Centro per i partner selezionare **Impostazioni** e quindi **Impostazioni sviluppatore**.

2. Selezionare **Utenti** e quindi **Aggiungi applicazioni Azure AD**.

3. Selezionare un'applicazione Azure AD esistente o crearne una nuova.

4. Se si crea una nuova applicazione Azure AD, includere le informazioni seguenti:  
  
**Nome**: è simile al campo 'nome descrittivo' del portale Cloud Partner.

**URL di risposta**: l'URL a cui gli utenti possono accedere per usare l'applicazione Azure AD. 

**URI ID app**: Questo è un identificatore logico per l'applicazione Azure AD presentato quando invia una richiesta Single Sign-On ad Azure AD. 

**Ruoli di sicurezza**: i ruoli **Manager** (uguale al ruolo 'Proprietario' nel portale Cloud Partner) e **Sviluppatore** (uguale al ruolo 'Collaboratore' nel portale Cloud Partner) si applicano al programma Commercial Marketplace nel Centro per i partner e possono essere associati a questa applicazione Azure AD.  

Quando si seleziona **Salva**, per creare questa applicazione nel Centro per i partner, le informazioni vengono anche sincronizzate nel sistema del portale Cloud Partner.  
