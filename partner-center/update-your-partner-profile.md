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
ms.openlocfilehash: f65de1bb115ba8108720429974622bf1a6afcc7b
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276349"
---
# <a name="verify-or-update-your-company-profile-information"></a>Verificare o aggiornare le informazioni del profilo aziendale 

**Ruoli appropriati:** Amministratore globale | Amministratore dell'account MPN

Al primo accesso al Centro per i partner come amministratore globale, devi verificare che tutti i dettagli aziendali siano corretti. Tra cui, contatto principale, indirizzo, ragione sociale e informazioni sul programma. Se la società ha più di una località, verificare l'accuratezza dei dati della località. Come amministratore globale, amministratore fatturazione o agente di amministrazione, sarà possibile visualizzare e aggiornare le informazioni di fatturazione e fiscali.

Il profilo partner è costituito dalle informazioni aziendali legali, dal nome del contatto principale e dall'indirizzo di posta elettronica, dai programmi a cui la società partecipa e, se pertinente, dalle altre società fuse con l'azienda legale. Verificare che il nome e l'indirizzo della società nel profilo aziendale legale siano privi di errori di ortografia e abbreviazioni e che corrispondano esattamente ai record ufficiali di iscrizione al registro delle imprese. Se si opera come impresa individuale, è necessario usare come ragione sociale il nome della società.


## <a name="locate-the-legal-business-profile"></a>Individuare il profilo aziendale legale

1. Passare all’icona **Impostazioni** e selezionare **Impostazioni account**.
 
1. Selezionare **Profilo organizzazione**. 

2. Verificare il **Legal business profile** (Profilo aziendale legale), le **Primary contact info** (Informazioni sul contatto principale) e le **Program info** (Informazioni sul programma).

Se le altre società sono state unite nell'azienda legale, è possibile verificare anche le informazioni relative a tali società. 

## <a name="update-your-legal-business-profile"></a>Aggiornare il profilo aziendale legale 

Aggiornare il nome o l'indirizzo dell'azienda legale Partner Center.

>[!Important]
>- Per gli account MPN, la ragione sociale può essere aggiornata sia dall'amministratore globale sia dall'amministratore degli account.
>- Per gli account rivenditore indiretti CSP, solo l'amministratore globale può aggiornare il nome della società legale. 
>- I partner con fatturazione diretta e i provider indiretti non possono modificare il nome legale della società se lo stato di verifica dell'account è **Autorizzato.** Se è necessario modificare il nome, è necessario creare un [ticket di supporto](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772).



1. Passare a **Impostazioni**, **Impostazioni account e** selezionare Profilo **organizzazione**.

2. Selezionare **Legale**  e quindi selezionare il profilo aziendale legale (partner o rivenditore) da aggiornare.

1. Fare clic **su Aggiorna**  accanto a nome/indirizzo della società e modificare i dettagli.
 
1. Quando si seleziona **Invia**, l'identità legale verrà nuovamente valutata. Viene nuovamente riassato solo ciò che è stato modificato.

1. Se la verifica non riesce, informazioni su come [risolvere il problema.](verification-responses.md)

>[!Important]
>Se si è un partner Cloud Solution Provider (CSP), non è possibile modificare il paese associato all'indirizzo legale. Il paese dell'indirizzo legale è associato al tenant e ai servizi, nonché alla valuta con cui si fanno affari. Per informazioni sugli aggiornamenti del paese MPN, vedere  [Aggiornamenti del paese MPN](manage-locations.md#change-country-of-partner-global-account).


### <a name="who-can-update-legal-business-name-and-when"></a>Chi può aggiornare il nome dell'azienda legale e quando

|**Programma**|**Chi può aggiornare il nome della società**|**Quando (stato) può essere aggiornato**|**È consentito**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Amministratore globale; Amministratore dell'account|Autorizzato; in sospeso; Rifiutato| Consentito|
|CSP: rivenditore indiretto|Amministratore globale|Autorizzato; in sospeso; Rifiutato| Consentito|


## <a name="update-your-mpn-global-business-account"></a>Aggiornare l'account aziendale globale MPN

Se, durante la migrazione da Partner Membership Center a Partner Center, l'account aziendale errato è stato identificato come azienda legale, è possibile modificarlo nell'account aziendale legale corretto.

Per apportare questi aggiornamenti, è necessario essere l'amministratore globale o l'amministratore account. Informazioni su come gestire gli account della posizione [globale MPN](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Aggiornare l'ID MPN associato all'account CSP

Per aggiornare l'ID MPN associato all'account CSP:

1. Accedere al dashboard Partner Center [come](https://partner.microsoft.com/dashboard/home) amministratore globale con le credenziali dell'account CSP e quindi selezionare **Impostazioni**. Le credenziali MPN e CSP possono essere diverse.
 
1. Selezionare **Identificatori** da **Impostazioni account**.

1. Nella sezione **CSP** usare il collegamento **Aggiorna** per aggiornare l'ID MPN associato all'account CSP. 


## <a name="update-your-csp-legal-billing-address"></a>Aggiornare l'indirizzo di fatturazione legale CSP

Gli amministratori globali, gli amministratori di fatturazione o gli agenti di amministrazione possono modificare l'indirizzo visualizzato nella fattura in **Profili di pagamento e fiscali**. Tuttavia, non è possibile modificare il nome della società nella fattura a causa di una limitazione del sistema di fatturazione.

:::image type="content" source="images/billing-profile.png" alt-text="Acquisizione dello schermo dell'area in cui vengono aggiunte le informazioni di fatturazione.":::

|**Campo**  |**Descrizione**|  
|---------------------|:------------------|
|Fatturare a Nome società|Nome della società visualizzato nel Bill-To informazioni sulla fattura CSP.  Non è modificabile nel Centro per i partner.  Per eseguire l'aggiornamento, creare un ticket di supporto.|
|Indirizzo di fatturazione|Indirizzo di fatturazione visualizzato nella fattura CSP. Possibilità di aggiornamento dal [profilo di fatturazione](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Contatto di fatturazione|I dettagli di contatto della fatturazione (nome, cognome, numero primario) per l'account CSP.  Possibilità di aggiornamento dal [profilo di fatturazione](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Numero dell'ordine fornitore|Numero dell'ordine di acquisto visualizzato nella fattura del partner.  Possibilità di aggiornamento dal [profilo di fatturazione](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|ID imposta società|Le aziende in alcuni paesi possono fornire il proprio numero di imposta sul valore aggiunto [(IVA) o equivalente locale.](./organization-tax-info.md) Per aggiornare l'ID fiscale o la partita IVA, è necessario essere amministratore globale, amministratore di fatturazione o un agente di amministrazione.|
|Valuta di fatturazione|La valuta di fatturazione per l'account CSP è determinata dal paese legale dell'account CSP.  Non è possibile modificare questa impostazione dopo la creazione dell'account CSP.|

## <a name="next-steps"></a>Passaggi successivi

- [Controllare lo stato di verifica](verification-responses.md)

- [Gestire le sedi MPN](manage-locations.md)