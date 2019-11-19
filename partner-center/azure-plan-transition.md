---
title: Transizioni dei clienti al piano di Azure | Centro per i partner
ms.topic: article
ms.date: 11/01/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Transita i clienti con facilità verso il piano di Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d19648053fefdcd998ad47bde2d68b289f15a10c
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653835"
---
# <a name="transition-your-customers-to-azure-plan"></a>Eseguire la transizione dei clienti al piano di Azure

I provider indiretti e i partner di fatturazione diretti possono passare alla nuova esperienza commerciale disponibile nel programma CSP per Azure. I rivenditori indiretti dovranno passare attraverso i loro provider indiretti. I clienti avranno una soluzione semplificata per l'acquisto di servizi cloud dai partner, dai venditori Microsoft o direttamente sul Web.

La funzionalità di transizione è destinata solo ai clienti che passano alla nuova esperienza commerciale per Azure e che hanno firmato il Contratto per clienti Microsoft e non per altre offerte in CSP, come Office 365 o Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Eseguire la transizione delle offerte CSP esistenti a un piano di Azure

È possibile eseguire la transizione di un cliente da un'offerta CSP per Azure esistente ai servizi di Azure inclusi nel piano per Azure della nuova esperienza commerciale del programma CSP dall'interno del Centro per i partner. Per la transizione è sufficiente che siano soddisfatti i requisiti seguenti:

- Il partner deve avere stabilito una relazione come rivenditore con il cliente finale tramite il Centro per i partner e il cliente deve avere firmato il Contratto per clienti Microsoft.

### <a name="select-transition-to-azure-plan"></a>Selezionare la transizione al piano di Azure

1. Seleziona il piano di Azure per il cliente.

2. Seleziona **Transition Azure subscription billing to Azure plan** (Transizione della fatturazione delle sottoscrizioni di Azure al nuovo piano di Azure).

![transizione](images/azure/transition1.png)

3. Seleziona **Continua**.

![transizione](images/azure/transition2.png)

Verrà visualizzato il portale di Azure in cui si svolgerà la transizione. Il cliente passerà al piano di Azure senza dover eseguire altre operazioni. 

**Durante il flusso della transizione vengono eseguiti automaticamente i passaggi preliminari seguenti**: 

- Acquisto di uno o più piani di Azure 
- Un piano per cliente in scenari CSP diretti  
- Un piano per rivenditore  

Si supponga, ad esempio, che un partner abbia acquistato due offerte Microsoft Azure e abbia incluso due partner registrati distinti nell'acquisto. In questo caso, durante il flusso della transizione verranno acquistati due piani di Azure (uno per rivenditore) e verrà eseguito automaticamente il mapping delle rispettive sottoscrizioni di Azure in base ai piani di Azure.  

**Mapping della sottoscrizione di Azure al piano di Azure**

Dopo aver acquistato uno o più piani di Azure, il sistema eseguirà il mapping delle sottoscrizioni di Azure esistenti ai piani di Azure. Lo stato di avanzamento può essere visualizzato nel portale di Azure e nel Centro per i partner. 

4. Torna alla pagina **Sottoscrizioni** del cliente nel Centro per i partner per aggiornare il relativo limite di budget nella valuta locale. 

![Transizione](images/azure/transition3.png)

>[!NOTE]
>Il budget che imposti nel Centro per i partner non viene trasferito al portale di Azure. Devi quindi impostare il budget e l'avviso nel portale di Azure.

Dopo essere passato al piano di Azure, non potrai più acquistare sottoscrizioni di Azure per questo cliente. Le sottoscrizioni vengono create in base al piano di Azure nel portale di Azure.

>[!NOTE]
> Tutte le sottoscrizioni di Azure acquistate tramite il controllo degli accessi in base al ruolo nel piano di Azure verranno addebitate e fatturate in valuta locale. Non verranno usati i tassi di cambio.

### <a name="track-your-transition-details"></a>Tenere traccia dei dettagli della transizione

Puoi seguire lo stato di avanzamento della transizione sia nel portale di Azure sia nel Centro per i partner.

![Mostra dettagli](images/azure/details1.png)

**Effetti sulla fatturazione per i partner**

Se esegui la transizione di un cliente da un'offerta CSP per Azure esistente, avrai gli effetti seguenti sulla fatturazione:

- Ti verrà addebitato il costo della fattura CSP esistente per tutto l'utilizzo fino al momento della chiusura della sottoscrizione CSP per Azure originale.

- Se disponi dei diritti di accesso di amministratore per la sottoscrizione CSP esistente, continuerai ad avere gli stessi diritti anche dopo la migrazione della sottoscrizione.

Per eseguire la transizione diretta dei contratti Enterprise Agreement a CSP e delle registrazioni SCE (Server and Cloud Enrollment) ai servizi di Azure, leggi [Acquisire la proprietà della fatturazione delle sottoscrizioni di Azure per il Contratto Microsoft Partner](https://docs.microsoft.com/azure/billing/mpa-request-ownership).

**Log di controllo**:

Per riconciliare la fatturazione, visualizza la cronologia delle sottoscrizioni di "Microsoft Azure" (0145P) nella pagina **Sottoscrizioni**. 

La sottoscrizione di "Microsoft Azure" (0145P) è costituita da due parti:
1. Sottoscrizione commerciale 
2. Sottoscrizione di Azure (diritto)

Al termine della transizione, la sottoscrizione di Azure viene spostata nel nuovo piano di Azure e la sottoscrizione commerciale viene sospesa per evitare la registrazione di altro utilizzo.  

>[Nota]: quando la sottoscrizione di Microsoft Azure (0145P) viene acquistata in CSP, la sottoscrizione commerciale e la sottoscrizione di Azure (diritto) hanno lo stesso valore. I valori sono diversi solo nel caso di modifiche o trasferimenti della proprietà della fatturazione. 

**Problemi di transizione**

Non sono previsti problemi durante le transizioni. Se si verifica un errore, verrai aggiornato durante il flusso della transizione. Non vi saranno interferenze con l'utilizzo di Azure.  

**Passaggi successivi**

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)



