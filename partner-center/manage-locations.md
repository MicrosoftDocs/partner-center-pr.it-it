---
title: Gestire le posizioni nell'account partner
ms.topic: how-to
ms.date: 11/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Informazioni su come aggiungere una nuova sede e come usare l'ID MNP di sede in programmi di incentivi, transazioni aziendali CSP, sottoscrizioni e altre transazioni.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03c4fb5a4adeb49602fe3736971e140ac6da6f4f
ms.sourcegitcommit: 245b4792e8221468f781f6effd1c9b23be05499a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/24/2020
ms.locfileid: "95514801"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Gestire le sedi dell'account MPN e aggiungere una nuova sede

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore degli account

L'ID MPN di sede identifica ogni specifica sede della società. L'ID MPN di sede viene usato per l'iscrizione a programmi di incentivi, per transazioni CSP e per altre transazioni aziendali. L'ID MPN globale viene usato per attività non transazionali, ad esempio richieste di supporto.

## <a name="the-following-is-a-typical-scenario"></a>Di seguito è riportato uno scenario tipico:

Contoso ha registrato il proprio account globale partner nel Regno Unito. Si tratta della sede legale dell'azienda e l'ID MPN globale viene usato per la gestione di tutte le attività non transazionali. Contoso ha anche account di sede partner, corrispondenti a filiali o divisioni in un'altra località del Regno Unito, della Francia o degli Stati Uniti. Nella struttura degli account MPN gli account di sede partner sono rappresentati come ID MPN di sede univoci. Gli account di sede partner vengono usati per attività transazionali, ad esempio programmi di incentivi o CSP. I pagamenti sono collegati a posizioni specifiche. 

>[!NOTE]
>Tra un tenant CSP e un ID MPN di sede esiste una relazione 1 a 1.

:::image type="content" source="images/locations/locations1.png" alt-text="Struttura delle sedi MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Prerequisiti per aggiungere una nuova sede per un'azienda CSP

Per aggiungere una nuova sede aziendale CSP, è necessario soddisfare alcuni prerequisiti:

1. È necessario avere un ID MPN di sede nel paese in cui si vuole svolgere le attività aziendali.

1. È necessario un nuovo tenant Azure AD nell'[area geografica di attività](regional-authorization-overview.md) non ancora iscritta a CSP. Creare questo tenant quando si effettua l'iscrizione a CSP.
 
3. Usare il nuovo tenant di AAD per l'iscrizione al programma CSP nell'area geografica.
Fornire i dettagli legali dell'azienda, inclusi la ragione sociale, l'indirizzo e i dettagli del contatto principale. L'account verrà sottoposto a verifica, quindi assicurarsi di aggiungere informazioni valide.

>[!NOTE] 
 >Ricordarsi di eseguire l'accesso con le **nuove** credenziali per il **nuovo** tenant di Azure AD. Non usare le credenziali esistenti perché il Centro per i partner riconoscerà l'utente che ha già un account.

4. Accettare il Contratto Microsoft Partner e attivare l'account.

## <a name="add-an-mpn-location"></a>Aggiungere una sede MPN

1. Accedere al Centro per i partner con l'account MPN. L'account MPN deve avere i privilegi di amministratore globale o amministratore account. 

1. Nell'icona **Impostazioni** selezionare **Impostazioni dell'organizzazione**.

2. Selezionare **Note legali** quindi **Posizioni**.

3. Selezionare **Aggiungere una sede** e inserire i dettagli dell'indirizzo della sede che si vuole aggiungere alla società, nonché un contatto principale per la sede.

> [!NOTE]
> dopo aver aggiunto una posizione nel Centro per i partner, non è possibile rimuoverla. Se l'accesso è stato effettuato con l'account corretto, verrà visualizzato **MPN** nel menu a sinistra del Centro per i partner.

## <a name="change-global-partner-account-location"></a>Modificare la sede dell'account partner globale

1. Nella pagina **[Località società](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** verificare che la sede desiderata come entità legale sia inclusa nell'elenco delle sedi. In caso contrario, aggiungerla.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Screenshot della pagina delle posizioni dell'account del Centro per i partner con l'elenco di tutte le posizioni correnti.":::

2. Selezionare **Note legali** quindi **aggiornare il profilo legale dell'azienda**
  
3. Seleziona l'area e la persona giuridica e quindi **Invia**.

  
## <a name="next-steps"></a>Passaggi successivi

- Vedere le informazioni sul [processo di verifica](verification-responses.md).
