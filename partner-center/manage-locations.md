---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441329"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Gestire i percorsi degli account MPN e aggiungere (eliminare) un percorso


**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

L'ID MPN di sede identifica ogni specifica sede della società. L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali. L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.

## <a name="the-following-scenario-is-typical"></a>Lo scenario seguente è tipico:

Contoso ha registrato il proprio account globale partner nel Regno Unito. Il PGA è il proprio business legale registrato e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali. Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti. Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci. Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP. I pagamenti sono collegati a posizioni specifiche. 

>[!NOTE]
>Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Prerequisiti per l'aggiunta di un nuovo account per un'azienda CSP

Per aggiungere un nuovo account aziendale CSP, iniziare assicurandosi di aver soddisfatto i prerequisiti.

1. È necessario disporre di un ID MPN della località nel paese in cui si desidera eseguire l'attività di CSP. Per creare un nuovo percorso MPN, vedere "aggiungere un percorso MPN" di seguito.
  
1. Per creare una nuova registrazione del rivenditore indiretto CSP, vedere usare i [provider indiretti](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** account CSP. Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.

2. Accettare il Contratto Microsoft Partner e attivare l'account.

1. Se vuoi iscriverti come partner Direct fattura, leggi [i requisiti per la fatturazione diretta dei partner](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>Visualizza le località MPN

1. Accedere al [Dashboard](https://partner.microsoft.com/dashboard/home) del centro per i partner con le credenziali dell'account MPN. (Le credenziali MPN potrebbero essere diverse da quelle del CSP) 
 
1. Nell'icona **Impostazioni** selezionare **Impostazioni account**, **profilo organizzazione**, **legale**. 

1. Nella scheda **partner** verificare che non sia presente un messaggio di errore del banner che chiede di correggere i percorsi migrati da PMC.  Se le località non sono state configurate correttamente in PMC e non sono ancora state passate a PC, è necessario aggiornare tali percorsi.

:::image type="content" source="images/locations/location-two.png" alt-text="Screencap Mostra come aggiornare il percorso.":::
 
4.  Nella schermata **Verifica percorsi di PMC** selezionare **Aggiorna**.
Aggiornare i campi seguenti:

- **Campo nome**: assicurarsi che il nome del percorso aziendale sia corretto. Se viene visualizzato un errore duplicato, provare a modificare da, ad esempio, contoso a contoso, Inc.

- **Campo dell'entità legale**: assicurarsi di aver scelto l'entità legale a cui è associata la località

- **Campi riga indirizzo 1 & 2**: assicurarsi che l'indirizzo sia corretto

- **Campi provincia & stato/provincia**: assicurarsi che la combinazione tra la città e lo stato o la provincia sia corretta. In alcuni paesi viene applicato il menu a discesa per la scelta dello stato e della provincia e in altri paesi sarà necessario inserire manualmente tale campo.

- **Campo CAP**: assicurarsi che il campo CAP corrisponda al paese, all'area, alla città o all'indirizzo indicato.

- **Campi delle informazioni di contatto primarie**: assicurarsi che i campi nome e cognome siano compilati e che l'indirizzo di posta elettronica indicato sia un indirizzo di posta elettronica di lavoro e non uno personale, ad esempio,, e @outlook.com @live.com così via.

- **Campo numero di telefono**: assicurarsi che il numero di telefono non includa caratteri speciali, spazi o codici paese. Il valore immesso nel campo numero di telefono conterrà sempre un massimo di 10 caratteri.

5. Se non è presente un messaggio di errore, da  **Impostazioni** selezionare  **Impostazioni account**, **profilo organizzazione**, **identificatori**.

6. Trovare l'ID MPN con il tipo "location" corrispondente al paese di questo account CSP e usarlo per completare l'associazione.

7. Se non è possibile trovare l'ID MPN della località che corrisponde all'account CSP da usare, è possibile aggiungere un nuovo percorso che creerà un nuovo ID MPN. Vedere **aggiungere un percorso MPN di** seguito.

## <a name="add-an-mpn-location"></a>Aggiungere una sede MPN

1. Accedere con l'account MPN nel centro per i partner. Le credenziali MPN potrebbero essere diverse da quelle del CSP. L'account MPN deve avere i privilegi di amministratore globale o amministratore account. 

1. Nell' **icona Impostazioni** selezionare le impostazioni dell' **account** e quindi selezionare **profilo organizzazione**.

2. Selezionare **Legal** , quindi nella scheda **partner** Selezionare **percorsi aziendali** e fare clic su **Aggiungi un percorso.**

3. Specificare i dettagli richiesti, inclusi il nome dell'azienda, l'indirizzo e il contatto per la località che si desidera aggiungere all'azienda.
 
1. Fare clic su **Aggiungi percorso**. Verrà creato un nuovo ID MPN per la nuova località che è possibile usare per le transazioni e gli incentivi CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Aggiungi una nuova attività legale":::

> [!NOTE]
> Una volta aggiunta una località nel centro per i partner, non è possibile rimuoverla. Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.


## <a name="delete-a-location"></a>Elimina un percorso

Per eliminare un percorso dall'account, sarà necessario contattare il [supporto tecnico](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Assicurarsi di comprendere l'effetto di questa azione. Non è possibile recuperare i percorsi eliminati e qualsiasi elemento associato a tale ID MPN specifico non verrà più riconosciuto o attivo per l'azienda.

## <a name="change-country-of-partner-global-account"></a>Modificare il paese dell'account globale del partner 

1. Accedere con l'account MPN nel centro per i partner. Le credenziali MPN potrebbero essere diverse da quelle del CSP. L'account MPN deve avere i privilegi di amministratore globale o amministratore account. 

2. Nella scheda **partner** passare a **percorsi aziendali** e controllare l'elenco delle località per assicurarsi che la località desiderata come entità legale sia elencata. 
 
1. Per aggiungere un percorso, fare clic su **Aggiungi un percorso** e, in uscita, fornire i dettagli necessari, tra cui il nome dell'azienda, l'indirizzo e il contatto principale per la località che si desidera aggiungere all'azienda. 
 
1. Selezionare **cambia il paese** accanto all'elenco a discesa **paese/area geografica** e seguire i passaggi. 

:::image type="content" source="images/lbp.png" alt-text="Informazioni legali sui dati del profilo aziendale":::

5. Fare clic su **Salva**.

6. Il paese dell'account globale MPN verrà modificato nel nuovo paese legale.
  
## <a name="next-steps"></a>Passaggi successivi

- Vedere le informazioni sul [processo di verifica](verification-responses.md).
