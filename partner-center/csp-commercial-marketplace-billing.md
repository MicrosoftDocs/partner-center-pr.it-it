---
title: Fatturazione per i prodotti del marketplace commerciale
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sul funzionamento della fatturazione per i prodotti o le sottoscrizioni SaaS ISV acquistati per i clienti dal marketplace commerciale all'interno Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148024"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Fatturazione per prodotti e sottoscrizioni del marketplace commerciale in Partner Center


**Ruoli appropriati:** Amministratore globale | Amministratore della fatturazione

In qualità di partner nel programma CSP, è possibile usare Partner Center per acquistare prodotti SaaS basati su licenza da editori ISV nel marketplace commerciale. Dopo questa operazione, è possibile accedere a una fattura per questi tipi di acquisti. Il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. Le fatture vengono rese disponibili l'8° giorno del mese successivo.

È possibile accedere alle fatture dal [dashboard](https://partner.microsoft.com/dashboard/) Partner Center o usando Partner Center [API .](/partner-center/develop/)

I partner del programma CSP vengono fatturati per le soluzioni del marketplace commerciale ISV acquistate per un cliente quando acquistano tali prodotti da Partner Center o dal portale di Azure (usando il tenant di Azure acquistato da CSP precedente del cliente).

>[!NOTE]
>Se i clienti usano il proprio tenant Azure AD (non uno acquistato da un partner nel programma CSP), i clienti possono anche scegliere di acquistare la propria soluzione SaaS ISV direttamente da ([Microsoft AppSource](https://appsource.microsoft.com/) [o Azure Marketplace](https://azuremarketplace.microsoft.com/)). In tal caso, riceveranno la fattura direttamente da Microsoft. Analogamente, se un partner nel programma CSP vende una sottoscrizione di Azure o il nuovo piano di [](/azure/role-based-access-control/built-in-roles) Azure al cliente e concede al cliente (o rivenditore indiretto) l'accesso in base al ruolo al tenant (assegnando qualsiasi ruolo al cliente oltre a **Lettore),** tale cliente (o rivenditore indiretto) può anche acquistare offerte del marketplace commerciale senza approvazione o notifica preventiva al partner CSP. In questi casi, Microsoft non invierà direttamente ai partner del programma CSP gli acquisti effettuati dai clienti. Tuttavia, Microsoft offre un meccanismo di [Monitoraggio di Azure](/azure/azure-monitor/platform/alerts-activity-log) facoltativo che è possibile usare per impostare avvisi o notifiche sull'attività in una sottoscrizione di Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Accedere alle informazioni di fatturazione per i prodotti del marketplace commerciale

L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione. Per accedere alla fattura e al file di riconciliazione più recenti per gli acquisti di prodotti del marketplace commerciale:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/) Centro per i partner.

2. Dal menu del Centro per i partner seleziona **Fatturazione**. 

    Nella parte superiore della pagina Fatturazione verranno visualizzate due schede: **Ricorrente** e Ricorrente e Acquisti **una sola volta.** Ogni scheda consente di accedere ai file di fattura e riconciliazione (ricognizione) per prodotti del marketplace diversi:

    - **Scheda Ricorrente:** mostra i file di fattura e riconciliazione per le sottoscrizioni correlate a Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro e Microsoft Azure.

    - **Scheda Acquisti ricorrenti e una sola** volta: mostra i file di fattura e riconciliazione per il piano di Azure, le prenotazioni di Azure, i prodotti del marketplace software e commerciale.
  
3. Selezionare la **scheda Acquisti ricorrenti e una sola** volta. Se sono state acquistate sottoscrizioni per un cliente in una valuta diversa, verrà visualizzata una scheda per ogni valuta. In questa pagina è possibile eseguire alcune operazioni:

    - Per visualizzare la fattura e il file di riconciliazione più recenti, selezionare **Fattura** o **File di riconciliazione**. Se si vuole, è anche possibile accedere alla fattura più recente e riconciliare i dati dei file [usando Partner Center API](/partner-center/develop/).

    - Per visualizzare le fatture e i file di ricognizione precedenti, espandere la **riga Cronologia fatturazione riportata** di seguito.

    - Per controllare il saldo o la fattura stimata dell'account in qualsiasi momento in base all'attività dell'account più recente, selezionare un collegamento sotto **l'intestazione Stime.**  

    >[!NOTE]
    > Quando la fattura viene pubblicata l'8° giorno del mese, verranno incluse le imposte e eventuali altri addebiti e crediti applicabili. Ciò significa che l'importo finale dovuto potrebbe essere diverso da quello visualizzato durante il periodo di fatturazione.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Altre informazioni su fatture e file di ricognizione per i prodotti del marketplace commerciale

Questa sezione offre altre informazioni sui file di fattura e riconciliazione per le sottoscrizioni SaaS del marketplace commerciale acquistate per i clienti di editori ISV di terze parti.

Quando si  seleziona Acquisti ricorrenti e  una sola volta dall'opzione Fatturazione nel menu Partner Center, si ottiene l'accesso alle fatture e ai file di riconciliazione per gli addebiti correlati agli acquisti microsoft (di prima parte) e ISV (di terze parti). Questi acquisti possono essere associati a:

- Sottoscrizioni SaaS (da editori Microsoft o ISV)

- Piano di Azure

- Prenotazioni di Azure

- Altro software basato su sottoscrizione (da editori Microsoft o ISV)

Esempi di questi acquisti possono includere software SUSE Linux (una sottoscrizione software) o una sottoscrizione di prodotto SaaS isv di Azure.

>[!NOTE]
> Per altre informazioni su come leggere i file di fattura e ricognizione, vedere anche Panoramica [della fatturazione.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Suggerimenti per la lettura della fattura

Quando si acquista un prodotto SaaS basato su licenza da un editore ISV di terze parti, nella fattura verranno visualizzati solo gli addebiti per la tariffa di licenza. Questo vale anche quando il prodotto SaaS dell'ISV usa (o usa) le risorse dell'infrastruttura di Azure sottostanti. Ciò è dovuto al fatto che gli addebiti per l'utilizzo dell'infrastruttura di Azure del cliente per un prodotto SaaS di un ISV vengono fatturati direttamente all'ISV. Gli ISV vedranno gli addebiti per il consumo di Azure associati nel proprio file di riconciliazione delle fatture con tariffa giornaliera per l'utilizzo di Azure.

La fattura conterrà diverse pagine:

- **Pagina 1 della fattura:** Contiene una panoramica di riepilogo dei dettagli di fatturazione del partner del programma CSP. Sono inclusi un riepilogo degli addebiti per il periodo di fatturazione, un numero di fattura, le condizioni di pagamento (60 giorni netti) e i metodi di pagamento per il pagamento tramite bonifico o tramite assegno.

- **Pagina 2 (ed eventuali pagine successive) della fattura:** Dettagli degli addebiti sia per gli acquisti Microsoft di terze parti che per gli acquisti isv di terze parti (basati su licenza) dal marketplace commerciale. È possibile identificare gli acquisti basati su licenza ISV dalla riga **Publisher** sotto ogni nome di prodotto. Il file di riconciliazione associato offre altri dettagli di fatturazione per addebiti di fatture specifici.

- **Pagina finale della fattura:** Se sono stati addebitati costi per i prodotti del marketplace basati su licenza di un ISV, in questa pagina finale verranno visualizzati altri dettagli sul nome e sull'indirizzo dell'editore ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Suggerimenti sulla lettura del file di riconciliazione

Il file **di riconciliazione degli** acquisti ricorrenti e una sola volta contiene diverse colonne con dettagli aggiuntivi mappati agli addebiti nella fattura. La **colonna PublisherName** indica se l'acquisto viene acquistato da Microsoft o da un editore ISV di terze parti.

Alcuni addebiti nel file di riconciliazione possono essere visualizzati con un costo di $ 0. Ciò può essere dovuto a un'offerta di "versione di valutazione gratuita" isv (in genere 30 o 60 giorni) o a un'offerta Bring Your Own License.

Nel caso di offerte ISV della versione di valutazione gratuita:

- Il periodo di valutazione gratuito copre il costo del prodotto SaaS basato su licenza dell'ISV durante tale periodo. Non verranno inoltre addebitati costi per l'uso dell'infrastruttura di Azure associata al prodotto SaaS.  Se si usa un'offerta ISV basata sull'utilizzo, tuttavia, la versione di valutazione gratuita non include il costo dell'utilizzo dell'infrastruttura di Azure sottostante. In questo caso, gli addebiti per l'utilizzo dell'infrastruttura di Azure verranno visualizzati in un file di riconciliazione di Azure separato.

- Quando si acquista e si distribuisce un prodotto idoneo per la versione di valutazione gratuita di un ISV per il cliente, il cliente viene automaticamente registrato nella versione di valutazione gratuita dall'editore dell'ISV. Il periodo di valutazione gratuita termina automaticamente dopo il periodo definito dall'editore ISV. Al termine del periodo, verrà addebitato il costo al cliente. Questo significa che il file di riconciliazione può mostrare due righe per un prodotto idoneo per la versione di valutazione: una che tiene traccia del periodo di valutazione e una che tiene traccia dell'offerta a pagamento (che visualizza un costo di $ 0 fino al termine del periodo di valutazione). Al termine della versione di valutazione, la riga che mostra l'offerta a pagamento inizierà a mostrare gli addebiti. 

Per altre informazioni su ciò che ogni colonna rappresenta, vedere [Usare i file di riconciliazione.](use-the-reconciliation-files.md) Vedere anche [Tipi di fatturazione in Partner Center](./billing-basics.md)

## <a name="next-steps"></a>Passaggi successivi

- [Gestire i prodotti del marketplace commerciale per i clienti](csp-commercial-marketplace-manage.md)
- [Informazioni sul supporto per i prodotti del marketplace commerciale](csp-commercial-marketplace-support.md)