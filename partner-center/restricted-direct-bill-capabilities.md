---
title: Funzionalità di fatturazione diretta con restrizioni
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I partner diretti per la fatturazione che non soddisfano il nuovo requisito avranno funzionalità di fatturazione diretta limitate
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: fatturazione diretta, limitazione
ms.openlocfilehash: ae2a1a66f1a93e8b8183a307eca395e9781a00df
ms.sourcegitcommit: 3849d49261f4f652bd7c0537ebe31558af427c5c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2020
ms.locfileid: "83362429"
---
# <a name="restricted-direct-bill-capabilities"></a>Funzionalità di fatturazione diretta con restrizioni  

## <a name="overview"></a>Panoramica

I partner diretti per la fatturazione devono soddisfare i nuovi [requisiti](direct-partner-new-requirements.md) per restare nel programma per i partner Direct Bill CSP. In caso contrario, l'accesso alle funzionalità di fatturazione diretta verrà limitato e non sarà più possibile eseguire attività specifiche, ad esempio effettuare nuovi acquisti per i clienti.

> [!Note]
> I partner diretti per la fatturazione che non soddisfano i nuovi requisiti per CSP Direct Bill Partner Program verranno informati da Microsoft quando le relative funzionalità di fatturazione diretta saranno limitate. Questa condizione si applica a tutti i partner diretti di fatturazione, indipendentemente dal fatto che abbiano optato per la [transizione dal partner Direct Bill a rivenditori indiretti](transition-direct-to-indirect.md) .  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Come stabilire se le funzionalità di fatturazione diretta sono state limitate

Per verificare se l'accesso dal tenant partner diretto a fatturazione diretta è stato limitato, attenersi alla seguente procedura.

1. Accedere al dashboard del [centro](https://partner.microsoft.com/dashboard)per i partner.

2. Passare a **Impostazioni partner**  ->  **profilo partner**.

3. In **informazioni sul programma**cercare **Microsoft Cloud stato provider soluzione**.

4. Se lo stato del programma dispone di un valore **limitato**, significa che l'accesso al tenant del partner Direct Bill per le funzionalità di fatturazione diretta è stato limitato.

## <a name="affected-direct-bill-capabilities"></a>Funzionalità di fatturazione diretta interessate

Se le funzionalità di fatturazione diretta sono state limitate, non è più possibile effettuare nuovi acquisti per i clienti nel centro per i partner. Questa restrizione include:

- Sottoscrizioni Azure
- Sottoscrizioni basate su Seat
- Aggiungere nuovi componenti aggiuntivi alle sottoscrizioni esistenti basate su postazioni.
- Effettuare acquisti monouso di prodotti software e di prenotazione (ad esempio, sottoscrizioni software, software perpetuo e istanze di macchine virtuali riservate di Azure).

Non è inoltre possibile acquistare nuove sottoscrizioni di Azure per uso personale usando l' [offerta servizi condivisi di Azure partner](shared-services.md) nel programma CSP.

Le sottoscrizioni di fatturazione diretta esistenti non sono interessate. Rimangono validi e vengono rinnovati. Si continuerà a essere addebitati direttamente da Microsoft fino a quando non vengono annullati. È comunque possibile gestire le sottoscrizioni esistenti nei modi seguenti:

- Sospendi sottoscrizioni esistenti
- Modificare il numero di postazioni esistenti per le sottoscrizioni basate su postazione
- Modificare il numero di postazioni dei componenti aggiuntivi esistenti in una sottoscrizione. Nota: non è possibile aggiungere nuovi componenti aggiuntivi alle sottoscrizioni esistenti perché vengono considerati come nuovi acquisti.
- Distribuisci nuove risorse di Azure e Gestisci le risorse di Azure esistenti in sottoscrizioni di Azure esistenti. Sono incluse le risorse disponibili tramite Azure Marketplace e le sottoscrizioni di Visual Studio.

Oltre ai nuovi acquisti, non è possibile accedere alle seguenti funzionalità di fatturazione diretta nel centro per i partner:

- Non è possibile creare nuovi tenant del cliente. L'opzione **Crea cliente** nella pagina clienti del centro per **i** partner non sarà disponibile.
- Non è possibile generare un invito al cliente che richiede la relazione diretta del rivenditore. L'opzione **Richiedi relazione rivenditore** nella pagina clienti del centro per **i** partner non sarà disponibile.

    >[!Note]
    >Nell'ambito della transizione da Direct Bill partner a Reseller indirect, se è già stato registrato il tenant Direct Bill partner come rivenditore indiretto, è possibile generare un invito al cliente che richiede la relazione indiretta del rivenditore.

- Non è possibile creare un nuovo tenant sandbox. Ogni tenant Direct Bill partner può creare un tenant sandbox ai fini dell'integrazione dell'API Direct Bill. Se non è stato creato in precedenza, non è possibile eseguire questa operazione dopo aver limitato la funzionalità di fatturazione partner.  

## <a name="next-steps"></a>Passaggi successivi

- [Altre informazioni su come diventare rivenditore indiretto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nuovi requisiti dei partner diretti in CSP](direct-partner-new-requirements.md)