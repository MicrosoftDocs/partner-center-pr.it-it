---
title: Creare sottoscrizioni clienti nel centro per i partner
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come vendere le sottoscrizioni dei clienti ai prodotti pubblicati da Microsoft e ai prodotti SaaS pubblicati da ISV di terze parti.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: sottoscrizione, crea nuovo, Aggiungi sottoscrizione, Sospendi, Annulla, sospensione, Sospendi, SaaS, licenza, ISV, terze parti
ms.localizationpriority: medium
ms.openlocfilehash: 969093b1ce3ba6936800ea91fd066d73b51701c7
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394147"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Creare, sospendere o annullare le sottoscrizioni dei clienti

**Si applica a**

- Centro per i partner
- Centro per i partner per Microsoft Cloud for US Government
- Partner CSP

**Ruoli appropriati**

- Agente amministratore
- Amministratore fatturazione
- Amministratore globale
- Agente di supporto tecnico
- Agente di vendita

Dopo aver creato un record del cliente nel Centro per i partner, puoi vendere loro sottoscrizioni per i prodotti nel catalogo. Sono inclusi i prodotti pubblicati da Microsoft, oltre ai prodotti SaaS (software as a Service) pubblicati da fornitori di software indipendenti (ISV) di terze parti nel [Marketplace commerciale](https://azuremarketplace.microsoft.com/marketplace).

Alcune offerte sono limitate a una sottoscrizione per cliente. Per vedere l'elenco delle offerte limitate, visita la pagina Prezzi e offerte del Centro per i partner.

> [!IMPORTANT]
> Come partner del programma CSP, è possibile acquistare solo sottoscrizioni Saas **basate su licenza** dagli editori ISV all'interno del centro per i partner. Ciò significa che è possibile acquistare qualsiasi offerta SaaS **basata su licenze** che l'editore ISV ha reso disponibile, incluse le [offerte esclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a cui si ha accesso. Per acquistare o gestire altre offerte del Marketplace commerciale dagli ISV, ad esempio offerte basate **sull'utilizzo**, a consumo o a consumo che coinvolgono applicazioni, contenitori o macchine virtuali di Azure, è necessario accedere al portale di [gestione di Azure](https://portal.azure.com/). Per ulteriori informazioni, vedere [acquistare prodotti Marketplace commerciali](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Creare una nuova sottoscrizione

1. Accedere al [Dashboard del centro](https://partner.microsoft.com/dashboard)per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Selezionare **Aggiungi sottoscrizione**. La scheda **Online Services** mostrerà tutte le offerte SaaS del Marketplace disponibili.

4. Per visualizzare solo determinati tipi di sottoscrizioni, effettua le selezioni nei filtri disponibili:
   - **Autore**: scegliere **Microsoft** per visualizzare solo le offerte di Microsoft o il **partner** per vedere i prodotti commerciali del Marketplace pubblicati dagli ISV.
   - **Tipo di fatturazione**: selezionare il tipo di fatturazione per la sottoscrizione che si vuole usare: **licenza** o **utilizzo**. Vedi [Domande frequenti sulle nuove funzionalità di fatturazione](faq-about-new-billing-features.md) per informazioni che ti aiuteranno a decidere tra la frequenza di fatturazione mensile e annuale.
   - **Categoria**: scegliere **Enterprise**, **Small Business**o **Trial**. Per informazioni sulle sottoscrizioni di versioni di valutazione, vedi [Offrire ai clienti le versioni di valutazione dei prodotti Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Selezionare le sottoscrizioni di prodotto che si desidera acquistare per il cliente. I prodotti visualizzati dipendono dal tipo di segmento dei clienti (Education, Government e così via) e dai filtri applicati. Alcune offerte visualizzate sul Marketplace potrebbero non essere sempre disponibili per un cliente specifico o per un partner CSP specifico. Il motivo può essere il seguente:

   - Il cliente dispone già di una sottoscrizione a tale prodotto e ne è consentito solo uno

   - La sottoscrizione del cliente potrebbe essere stata sospesa. in questo caso, è possibile riattivare la sottoscrizione anziché acquistarne una nuova.

   - Per le offerte SaaS ISV, potrebbero esserci alcuni motivi per cui l'offerta non è disponibile per l'acquisto: l'ISV potrebbe non supportare il paese o l'area di fatturazione del cliente; l'ISV potrebbe aver scelto di non rendere disponibile l'offerta tramite il programma CSP; in alternativa, l'ISV potrebbe avere reso l'offerta [esclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo per determinati partner CSP. L'offerta ISV potrebbe anche non essere transazionale tramite il centro per i partner, ad esempio i contenitori o alcune offerte basate sull'utilizzo.  

6. Per ogni sottoscrizione che si vuole aggiungere, immettere il numero di licenze (se necessario) e selezionare **Aggiungi al carrello**.

7. Al termine dell'aggiunta delle sottoscrizioni, selezionare **Revisione** ed esaminare l'ordine.

8. Dopo aver esaminato gli ordini ed è possibile acquistare tali sottoscrizioni, selezionare **Acquista**.

9. Dopo aver acquistato una sottoscrizione per un cliente, si verificherà quanto segue:

    - È possibile esaminare o modificare la sottoscrizione selezionando il nome della sottoscrizione dalla pagina **sottoscrizioni** del cliente. In tale pagina puoi selezionare licenze per componenti aggiuntivi (se disponibili), modificare la quantità di licenze o sospendere la sottoscrizione.

    **Per le sottoscrizioni SaaS (basate su licenza) ISV:**
    - Si riceverà un collegamento al sito dell'editore ISV. Questo collegamento dovrebbe aiutare a completare la distribuzione o la configurazione dell'account della sottoscrizione del cliente. Si noti che il cliente non riceverà un messaggio di posta elettronica con le istruzioni per completare la configurazione e il provisioning dell'account per questo tipo di sottoscrizione ISV.

    - Se la sottoscrizione viene fornita con una versione di valutazione gratuita di 30 giorni, il periodo di valutazione gratuito verrà applicato automaticamente. I partner del programma CSP non possono rinunciare al periodo di valutazione gratuito sulle offerte acquistate per i clienti. Una volta terminato il periodo di valutazione gratuita, viene avviato il periodo di validità della sottoscrizione e la sottoscrizione viene convertita in stato a pagamento. La sottoscrizione verrà quindi rinnovata in base alla stessa pianificazione.

## <a name="suspend-or-cancel-a-subscription"></a>Sospendere o annullare una sottoscrizione

I partner possono sospendere o annullare una sottoscrizione se richiesto dal cliente o in caso di insolvenza o frode.

### <a name="suspend-a-subscription"></a>Sospendere una sottoscrizione

Quando cambi lo stato di una sottoscrizione in **Sospesa**, gli utenti non possono accedere alla sottoscrizione o ai servizi.

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Scegli la sottoscrizione che vuoi gestire.

4. Nella sezione **Stato**, scegliere **Sospesa**. **Inviare** quindi le modifiche.

5. Verranno eliminati tutti i dati, tranne nel caso in cui la sottoscrizione venga riattivata entro 90 giorni o 90 giorni più il numero di giorni tra il momento in cui l'account è stato aperto e il primo periodo di fatturazione (massimo 120 giorni).

Quando sospendi una sottoscrizione, la data visualizzata sotto il pulsante **Sospesa** indica quando la sottoscrizione scadrà automaticamente se non la riattivi. Per altre informazioni, vedere [domande frequenti sulle nuove funzionalità di fatturazione](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>Annullare una sottoscrizione

È possibile scegliere di annullare le sottoscrizioni SaaS basate su licenza da autori ISV di terze parti all'interno del [Marketplace commerciale](csp-commercial-marketplace-overview.md)del centro per i partner. Fino a quando l'annullamento viene annullato entro il periodo di annullamento, si riceverà un rimborso completo.

Per le offerte ISV fatturate mensilmente:

- Se si annulla meno di 24 ore dopo aver effettuato l'ordine, si riceverà un credito completo per la fattura successiva.

- Se si annulla l'annullamento in seguito a 24 ore dopo l'esecuzione dell'ordine, l'annullamento verrà pianificato per il rinnovo.

Per le offerte fatturate annualmente:

- Se si annulla meno di 14 giorni dopo aver effettuato l'ordine, si riceverà un credito completo per la fattura successiva.

- Se si annulla dopo 14 giorni dopo aver inserito l'ordine, l'annullamento verrà pianificato per il rinnovo.

Al termine di questi periodi, non verrà più visualizzata l'opzione per annullare la sottoscrizione.

> [!NOTE]
> I servizi ISV di terze parti basati sull'utilizzo e a consumo (che usano macchine virtuali o contenitori, ad esempio) non sono idonei per la restituzione. Il deprovisioning dei servizi basati sull'utilizzo può essere effettuato come un metodo di annullamento. Poiché i costi vengono addebitati dopo l'utilizzo, questi servizi non sono idonei per un rimborso.

Per annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV, seguire questa procedura:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Individuare la sottoscrizione che si vuole annullare.

4. Nella colonna **stato** selezionare **Annulla**. **Inviare** quindi le modifiche.

5. Se viene visualizzata una finestra di dialogo, compilare eventuali dettagli rilevanti, quindi selezionare **Invia**.

6. Per confermare l'annullamento, selezionare **Sì, Annulla**.

> [!NOTE]
> È anche possibile scegliere di annullare una sottoscrizione di Azure Marketplace usando le API. A tale scopo, vedere [annullare una sottoscrizione di Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Scegliere se rinnovare automaticamente una sottoscrizione del Marketplace commerciale

Per impostazione predefinita, le sottoscrizioni attive sono impostate in modo da essere rinnovate automaticamente al termine del periodo di sottoscrizione. Nel caso di [sottoscrizioni per prodotti del Marketplace commerciale](csp-commercial-marketplace-overview.md), puoi scegliere di non rinnovare automaticamente la sottoscrizione.

Per arrestare una sottoscrizione del Marketplace commerciale attiva dal rinnovo automatico:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Selezionare **sottoscrizioni**. Verranno elencate tutte le sottoscrizioni basate sulle licenze acquistate per il cliente.

4. Nella colonna **sottoscrizione** selezionare la sottoscrizione che si desidera modificare.

5. Nella pagina Dettagli sottoscrizione individuare la sezione **stato** e deselezionare la casella **rinnovo automatico** .

6. Selezionare **Invia**.

## <a name="next-steps"></a>Passaggi successivi

- [Acquistare prodotti del Marketplace commerciale per i clienti](csp-commercial-marketplace-purchase.md)

- [Gestione dei prodotti del Marketplace commerciale per i clienti](csp-commercial-marketplace-manage.md)

- [Panoramica del marketplace commerciale](csp-commercial-marketplace-overview.md)
