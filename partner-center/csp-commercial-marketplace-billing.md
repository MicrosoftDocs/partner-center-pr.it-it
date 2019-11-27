---
title: Fatturazione per prodotti Marketplace commerciali | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni sul funzionamento della fatturazione per i prodotti SaaS ISV o per le sottoscrizioni acquistate per i clienti dal Marketplace commerciale all'interno del centro per i partner.
author: MicheleHope
ms.author: v-mihope
keywords: sottoscrizioni, prodotti, acquisti, Marketplace, terze parti, ISV, fatturazione, fatture, riconciliazione, file di ricognizione
ms.localizationpriority: medium
ms.openlocfilehash: bc4dcca3d8c3d454a17eca676d5fadd1dac202d3
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384916"
---
# <a name="billing-for-commercial-marketplace-products"></a>Fatturazione per prodotti Marketplace commerciali

**Si applica a**

- Centro per i partner
- Partner aderenti al programma CSP

**Ruoli appropriati**

- Amministratore globale
- Amministratore fatturazione

Come partner del programma CSP, è possibile usare il centro per i partner per acquistare prodotti SaaS basati su licenze dagli editori ISV nel Marketplace commerciale. Al termine di questa operazione, è possibile accedere a una fattura per questi tipi di acquisti. Il periodo di fatturazione inizia il primo giorno del mese di calendario e termina l'ultimo giorno del mese di calendario. Le fatture vengono rese disponibili nell'ottavo giorno del mese successivo.

È possibile accedere alle fatture dal [Dashboard](https://partner.microsoft.com/dashboard/) del centro per i partner o usando le [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

I partner del programma CSP vengono fatturati per le soluzioni di Marketplace commerciale ISV acquistate per un cliente quando acquistano i prodotti dal centro per i partner o dalla portale di Azure (usando il tenant di Azure precedente, acquistato da CSP).

>[!NOTE]
>Se i clienti usano il proprio tenant Azure AD (non uno acquistato da un partner nel programma CSP), i clienti possono anche scegliere di acquistare la propria soluzione SaaS ISV direttamente da ([Microsoft AppSource](https://appsource.microsoft.com/) o [Azure Marketplace](https://azuremarketplace.microsoft.com/)). In tal caso, riceveranno la propria fattura direttamente da Microsoft. Analogamente, se un partner del programma CSP vende un tenant di Azure AD al cliente e concede l' [accesso in base al ruolo](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) del cliente a tale tenant (assegnando un ruolo al cliente oltre a **Reader**), il cliente potrà acquistare anche offerte di Marketplace commerciali senza previa approvazione o notifica al partner CSP. In questi casi, Microsoft non invierà direttamente una notifica ai partner del programma CSP sugli acquisti effettuati dai clienti. Tuttavia, Microsoft offre un meccanismo di [monitoraggio di Azure](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) facoltativo che è possibile usare per impostare avvisi o notifiche sulle attività in una sottoscrizione di Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Accedi alle informazioni di fatturazione per i prodotti commerciali del Marketplace

L'amministratore globale o l'amministratore della fatturazione per l'azienda riceverà un messaggio di posta elettronica quando una fattura è pronta per la visualizzazione. Per accedere alla fattura e al file di riconciliazione più recenti per gli acquisti di prodotti Marketplace commerciali:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard/) Centro per i partner.

2. Dal menu del Centro per i partner seleziona **Fatturazione**. 

    Nella parte superiore della pagina di fatturazione vengono visualizzate due schede: **ricorrenti** e **ricorrenti e acquisti**monouso. Ogni scheda consente di accedere ai file di fatturazione e riconciliazione (Recon) per diversi prodotti Marketplace:

    - Scheda **ricorrente** : Mostra la fattura e i file di riconciliazione per le sottoscrizioni relative a Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power bi Pro e Microsoft Azure.

    - Scheda **ricorrenza e acquisti** monouso: Mostra i file di Invoice e di riconciliazione per piano di Azure, prenotazioni di Azure, software e prodotti Marketplace commerciali.
  
3. Selezionare la scheda **ricorrenza e acquisti** monouso. Se sono state acquistate sottoscrizioni per un cliente in una valuta diversa, viene visualizzata una scheda per ogni valuta. È possibile eseguire alcune operazioni in fr: om questa pagina:

    - Per visualizzare la fattura e il file di riconciliazione più recenti, selezionare **fattura** o **file di riconciliazione**. Se si vuole, è anche possibile accedere ai dati più recenti relativi a fattura e file di ricognizione usando le [API del centro](https://docs.microsoft.com/partner-center/develop/)per i partner.

    - Per visualizzare le fatture e i file di ricognizione precedenti, espandere la riga **cronologia di fatturazione** riportata di seguito.

    - Per controllare il saldo stimato o la fatturazione in qualsiasi momento in base all'attività dell'account più recente, selezionare un collegamento sotto l'intestazione **stime** .  

    >[!NOTE]
    > Quando pubblichi la fattura nell'ottavo giorno del mese, saranno incluse le imposte e gli eventuali altri costi e crediti applicabili. Ciò significa che l'importo finale può essere diverso rispetto a quello visualizzato durante il periodo di fatturazione.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Altre informazioni sulle fatture e i file di ricognizione per i prodotti commerciali del Marketplace

Questa sezione offre ulteriori informazioni sui file di fatturazione e di riconciliazione per le sottoscrizioni SaaS del Marketplace commerciale acquistate per i clienti di editori ISV di terze parti.

Quando si selezionano gli **acquisti ricorrenti e** monouso dall'opzione di **fatturazione** nel menu centro partner, si ottiene l'accesso alle fatture e ai file di riconciliazione per i costi correlati agli acquisti sia Microsoft (First-Party) che ISV (di terze parti). Questi acquisti possono essere associati a:

- Sottoscrizioni SaaS (da autori Microsoft o ISV)

- Piano di Azure

- Prenotazioni di Azure

- Altri software basati su sottoscrizioni (di autori Microsoft o ISV)

Esempi di questi acquisti possono includere il software SUSE Linux (sottoscrizione software) o una sottoscrizione di prodotti SaaS di Azure ISV.

>[!NOTE]
> Per altre informazioni su come leggere i file di fattura e di ricognizione, vedere anche [Panoramica della fatturazione](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Suggerimenti per la lettura della fattura

Quando si acquista un prodotto SaaS basato su licenza da un editore ISV di terze parti, si vedranno solo gli addebiti per il costo della licenza per la fattura. Questo vale anche quando il prodotto SaaS del ISV USA o utilizza le risorse dell'infrastruttura di Azure sottostanti. Ciò è dovuto al fatto che i costi di utilizzo dell'infrastruttura di Azure del cliente per un prodotto SaaS di un ISV vengono fatturati direttamente all'ISV. Gli ISV visualizzeranno gli addebiti per il consumo di Azure associati nel proprio file di riconciliazione della fattura giornaliero di utilizzo di Azure.

La fattura conterrà diverse pagine:

- **Pagina 1 della fattura:** Contiene una panoramica di riepilogo dei dettagli di fatturazione del partner del programma CSP. Sono inclusi un riepilogo degli addebiti per il periodo di fatturazione, un numero di fattura, i termini di pagamento (NET 60 giorni) e i metodi di pagamento per la fatturazione per il pagamento tramite bonifico o per verifica.

- **Pagina 2 (e tutte le pagine successive) della fattura:** Dettagli addebiti per gli acquisti Microsoft di terze parti e per gli acquisti di terze parti (basati su licenza) del Marketplace commerciale. È possibile identificare gli acquisti basati su licenze ISV dalla riga del **server di pubblicazione** sotto ogni nome di prodotto. Il file di riconciliazione associato offre più dettagli di fatturazione per i costi di fatturazione specifici.

- **Pagina finale della fattura:** Se sono stati addebitati i prodotti Marketplace basati su licenza di un ISV, nella pagina finale saranno visualizzati ulteriori dettagli sul nome e sull'indirizzo dell'editore ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Suggerimenti per la lettura del file di riconciliazione

Il file di riconciliazione degli **acquisti ricorrenti e** monouso contiene diverse colonne con dettagli aggiuntivi che vengono mappati agli addebiti nella fattura. La colonna **PublisherName** indica se l'acquisto è stato acquistato da Microsoft o da un server di pubblicazione ISV di terze parti.

Alcuni addebiti nel file di riconciliazione possono essere visualizzati con un costo pari a $0. Questo problema può essere dovuto a un'offerta di "versione di valutazione gratuita" ISV (in genere 30 o 60 giorni) o a un'offerta Bring your own License.

Nel caso di una versione di valutazione gratuita, ISV offre:

- Il periodo della versione di valutazione gratuita copre il costo del prodotto SaaS basato sulle licenze ISV durante tale periodo di tempo. Inoltre, non verrà addebitato l'utilizzo dell'infrastruttura di Azure associata al prodotto SaaS.  Se si usa un'offerta ISV basata sull'utilizzo, tuttavia, la versione di valutazione gratuita non include il costo dell'utilizzo dell'infrastruttura di Azure sottostante. In questo caso, gli addebiti per l'utilizzo dell'infrastruttura di Azure verranno visualizzati in un file di riconciliazione Azure separato.

- Quando si acquista e si distribuisce la versione di valutazione gratuita di un ISV per il cliente, il cliente viene registrato automaticamente nella versione di valutazione gratuita dall'editore ISV. Il periodo di valutazione gratuita termina automaticamente dopo il periodo definito dall'editore ISV. Al termine del periodo, il cliente verrà addebitato. Questo significa che il file di riconciliazione può mostrare due righe per un prodotto idoneo alla versione di valutazione: una che tiene traccia del periodo di valutazione e una che tiene traccia dell'offerta a pagamento (che visualizzerà un costo di $0 fino al termine del periodo di valutazione). Una volta terminata la versione di valutazione, la riga che mostra l'offerta a pagamento inizierà a visualizzare gli addebiti. 

Per altre informazioni su ciò che ogni colonna rappresenta, vedere [usare i file di riconciliazione](use-the-reconciliation-files.md). Vedere anche [tipi di fatturazione nel centro per i partner](billing-different-types.md)

## <a name="next-steps"></a>Passaggi successivi

- [Gestione dei prodotti del Marketplace commerciale per i clienti](csp-commercial-marketplace-manage.md)
- [Informazioni sul supporto per i prodotti commerciali del Marketplace](csp-commercial-marketplace-support.md)
