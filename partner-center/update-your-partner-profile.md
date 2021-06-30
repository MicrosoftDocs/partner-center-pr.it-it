---
title: Verificare il profilo aziendale
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descrive come verificare i dettagli della società, ad esempio contatto principale, indirizzo e informazioni sul programma. Puoi anche aggiornare l'indirizzo legale e di fatturazione.
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 9f9a055ce3bfbff568287267b74b04e8f9d03ad1
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080623"
---
# <a name="verify-or-update-your-company-profile-information"></a>Verificare o aggiornare le informazioni del profilo aziendale 

**Ruoli appropriati:** amministratore globale | Amministratore dell'account MPN

La prima volta che si accede Partner Center come amministratore globale, è necessario verificare che tutti i dettagli aziendali siano corretti. Tra cui, contatto principale, indirizzo, ragione sociale e informazioni sul programma. Se la società ha più di una località, verificare l'accuratezza dei dati della località. In quanto amministratore globale, amministratore fatturazione o agente amministratore, sarà anche possibile visualizzare e aggiornare le informazioni di fatturazione e fiscali.

> [!NOTE]
> Per aggiornare l'indirizzo di fatturazione, è necessario essere l'amministratore globale.

Il profilo partner è costituito dalle informazioni aziendali legali, dal nome del contatto principale e dall'indirizzo di posta elettronica, dai programmi a cui la società partecipa e, se pertinente, dalle altre società fuse con l'azienda legale. Assicurarsi che il nome e l'indirizzo della società nel profilo di business legale non siano presenti errori di ortografia e abbreviazioni e che corrispondano esattamente ai record di registrazione aziendale formali dell'azienda. Se si opera come impresa individuale, è necessario usare come ragione sociale il nome della società.


## <a name="locate-the-legal-business-profile"></a>Individuare il profilo aziendale legale

1. In Partner Center selezionare **l'icona Impostazioni** e quindi selezionare **Impostazioni account.**
 
1. Selezionare **Profilo organizzazione**. 

2. Esaminare i valori per **Profilo di business legale,** **Informazioni contatto principale** e **Informazioni programma**.

Se le altre società sono state unite nell'azienda legale, è possibile verificare anche le informazioni relative a tali società. 

## <a name="update-your-legal-business-profile"></a>Aggiornare il profilo aziendale legale 

Aggiornare il nome o l'indirizzo della società legale Partner Center.

>[!Important]
>- Per Microsoft Partner Network (MPN), sia l'amministratore globale che l'amministratore account possono aggiornare il nome della società legale.
>- Per Cloud Solution Provider rivenditori indiretti (CSP), solo l'amministratore globale può aggiornare il nome della società legale. 
>- I partner con fatturazione diretta e i provider indiretti non possono modificare il nome legale della società se lo stato di verifica dell'account è **Autorizzato.** Se è necessario modificare il nome, è necessario creare un [ticket di supporto](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772).



1. In Partner Center impostazioni, **selezionare** **Impostazioni account** e quindi profilo **organizzazione.**

2. Selezionare **Legale** e quindi selezionare il profilo di business legale (partner o rivenditore) che si vuole aggiornare.

1. Selezionare **Aggiorna** accanto al nome/indirizzo della società e modificare i dettagli.
 
1. Quando si seleziona **Invia,** l'identità legale verrà nuovamente valutata. Viene nuovamente rieffezionato solo ciò che è stato modificato.

1. Se la verifica non riesce, vedere come [risolvere il problema](verification-responses.md).

>[!Important]
>I partner CSP non possono modificare il paese associato all'indirizzo legale. Il paese dell'indirizzo legale è associato al tenant e ai servizi, nonché alla valuta con cui si è commerciali. Per informazioni sugli aggiornamenti dei paesi MPN, vedere [Aggiornamenti dei paesi MPN.](manage-locations.md#change-country-of-partner-global-account)


### <a name="who-can-update-legal-business-name-and-when"></a>Chi può aggiornare il nome dell'azienda legale e quando

|**Programma**|**Chi può aggiornare il nome della società**|**Quando (stato) può essere aggiornato**|**È consentito**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Amministratore globale; Amministratore account|Autorizzato; in sospeso; Rifiutato| Consentito|
|CSP: Rivenditore indiretto|Amministratore globale|Autorizzato; in sospeso; Rifiutato| Consentito|


## <a name="update-your-mpn-global-business-account"></a>Aggiornare l'account aziendale globale MPN

Durante la migrazione da Partner Membership Center a Partner Center, se l'account aziendale errato è stato identificato come azienda legale, è possibile modificarlo con l'account aziendale legale corretto.

Per apportare questi aggiornamenti, è necessario essere l'amministratore globale o l'amministratore account. Informazioni su come [gestire gli account di posizione globale MPN](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Aggiornare l'ID MPN associato all'account CSP

Per aggiornare l'ID MPN associato all'account CSP:

1. Accedere al dashboard Partner Center [come](https://partner.microsoft.com/dashboard/home) amministratore globale con le credenziali dell'account CSP e quindi selezionare **Impostazioni.** Le credenziali MPN e CSP possono essere diverse.
 
1. Selezionare **Identificatori** da **Impostazioni account**.

1. Nella sezione **CSP** usare il collegamento **Aggiorna** per aggiornare l'ID MPN associato all'account CSP. 


## <a name="update-your-csp-legal-billing-address"></a>Aggiornare l'indirizzo di fatturazione legale CSP

Se si è l'amministratore globale, è possibile modificare l'indirizzo visualizzato nella fattura nel profilo **di pagamento e fiscale.** Attualmente non è possibile modificare il nome della società nella fattura a causa di una limitazione del sistema di fatturazione.

:::image type="content" source="images/billing-profile.png" alt-text="Acquisizione dello schermo dell'area in cui vengono aggiunte le informazioni di fatturazione.":::

|**Campo**  |**Descrizione**|  
|---------------------|:------------------|
|Nome società di fatturazione|Nome della società visualizzato nel Bill-To informazioni sulla fattura CSP.  Queste informazioni non sono modificabili nel Centro per i partner.  Per eseguire l'aggiornamento, creare un ticket di supporto.|
|Indirizzo di fatturazione|Indirizzo di fatturazione visualizzato nella fattura CSP. Può essere aggiornato da [Profilo di fatturazione.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|Contatto di fatturazione|I dettagli di contatto di fatturazione (nome, cognome, numero primario) per l'account CSP.  Può essere aggiornato da [Profilo di fatturazione.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|Numero ordine di acquisto|Numero dell'ordine di acquisto visualizzato nella fattura del partner. Può essere aggiornato da [Profilo di fatturazione.](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)|
|ID imposta società|Le aziende in alcuni paesi possono fornire il proprio numero di imposta sul valore [aggiunto (IVA) o equivalente locale.](./organization-tax-info.md) Per aggiornare l'ID fiscale o la partita IVA, è necessario essere amministratore globale, amministratore di fatturazione o un agente di amministrazione.|
|Valuta di fatturazione|La valuta di fatturazione per l'account CSP è determinata dal paese legale dell'account CSP.  Queste informazioni non possono essere modificate dopo la creazione dell'account CSP.|

## <a name="next-steps"></a>Passaggi successivi

- [Controllare lo stato di verifica](verification-responses.md)

- [Gestire le sedi MPN](manage-locations.md)
