---
title: Funzionalità di fatturazione diretta con restrizioni
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sui Cloud Solution Provider dei partner con fatturazione diretta (CSP) e su cosa fare per evitare che le funzionalità vengano limitate. Verificare se le funzionalità sono state limitate.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551419"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Funzionalità di fatturazione diretta con restrizioni e requisiti necessari per i partner con fatturazione diretta CSP

**Ruoli appropriati:** Amministratore globale

## <a name="overview"></a>Panoramica

I partner con fatturazione diretta devono [soddisfare](direct-partner-new-requirements.md) i nuovi requisiti per rimanere nel programma Cloud Solution Provider (CSP) per i partner con fatturazione diretta. In caso contrario, l'accesso alle funzionalità di fatturazione diretta verrà limitato e non sarà più possibile eseguire attività specifiche, ad esempio effettuare nuovi acquisti per i clienti.

> [!Note]
> I partner con fatturazione diretta che non soddisfano i nuovi requisiti per il programma CSP per i partner con fatturazione diretta verranno informati da Microsoft quando le funzionalità di fatturazione diretta saranno limitate. Questo vale per tutti i partner con fatturazione diretta, indipendentemente dal fatto che abbia scelto o meno la transizione da partner con fatturazione diretta [a rivenditori](transition-direct-to-indirect.md) indiretti.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Come determinare se le funzionalità di fatturazione diretta sono state limitate

Per verificare se l'accesso dal tenant partner con fatturazione diretta alle funzionalità di fatturazione diretta è stato limitato, seguire questa procedura.

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).

2. Passare a **Impostazioni account**  >  **Profilo legale.**

3. In **Program info (Informazioni** programma) **cercare Microsoft Cloud Solution Provider stato .**

4. Se lo stato del programma ha un valore **limitato,** significa che l'accesso del tenant del partner con fatturazione diretta alle funzionalità di fatturazione diretta è stato limitato.

## <a name="affected-direct-bill-capabilities"></a>Funzionalità di fatturazione diretta interessate

Se le funzionalità di fatturazione diretta sono state limitate, non è più possibile effettuare nuovi acquisti per i clienti in Partner Center. Questa restrizione include:

- Sottoscrizioni Azure

- Abbonamenti in base alle licenze

- Aggiungere nuovi componenti aggiuntivi alle sottoscrizioni esistenti basate su licenza.

- Effettuare acquisti una sola volta di prodotti software e di prenotazione, ad esempio sottoscrizioni software, software perpetuo e istanze di macchine virtuali riservate di Azure.

Non è inoltre possibile usare [l'offerta di servizi condivisi dei partner di Azure](shared-services.md) nel programma CSP per acquistare nuove sottoscrizioni di Azure per uso personale.

Le sottoscrizioni con fatturazione diretta esistenti non sono interessate. Rimangono validi e vengono rinuovati. L'addebito continuerà a essere addebitato direttamente da Microsoft fino a quando non vengono annullati. È comunque possibile gestire le sottoscrizioni esistenti nei modi seguenti:

- Sospendere le sottoscrizioni esistenti

- Modificare il numero di licenze delle sottoscrizioni esistenti basate su licenza

- Modificare il numero di licenze dei componenti aggiuntivi esistenti in una sottoscrizione. 

    >[!Note]
    >Non è possibile aggiungere nuovi componenti aggiuntivi alle sottoscrizioni esistenti perché vengono considerati come nuovi acquisti.

- Distribuire nuove risorse di Azure e gestire le risorse di Azure esistenti nelle sottoscrizioni di Azure esistenti. Sono incluse le risorse disponibili tramite sottoscrizioni Azure Marketplace e Visual Studio sottoscrizione.

Oltre ai nuovi acquisti, non è possibile accedere alle funzionalità di fatturazione diretta seguenti in Partner Center:

- Non è possibile creare nuovi tenant del cliente. **L'opzione Crea** cliente **nella pagina** Clienti Partner Center non sarà disponibile.

- Non è possibile generare l'invito al cliente che richiede una relazione come rivenditore diretto. **L'opzione Richiedi una relazione come** rivenditore nella **pagina** Clienti Partner Center non sarà disponibile.

    >[!NOTE]
    >Nell'ambito della transizione dal partner con fatturazione diretta al rivenditore indiretto, se è già stato registrato il tenant del partner con fatturazione diretta come rivenditore indiretto, è possibile generare l'invito al cliente che richiede una relazione come rivenditore indiretto.

- Non è possibile creare un nuovo tenant sandbox. Ogni tenant partner con fatturazione diretta può creare un tenant sandbox per l'integrazione dell'API di fatturazione diretta. Se non è stato creato in precedenza, non è consentito farlo dopo che la funzionalità del partner con fatturazione diretta è stata limitata.  

## <a name="next-steps"></a>Passaggi successivi

- [Altre informazioni su come diventare rivenditore indiretto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nuovi requisiti dei partner diretti in CSP](direct-partner-new-requirements.md)
