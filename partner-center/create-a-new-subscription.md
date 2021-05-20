---
title: Creare sottoscrizioni dei clienti in Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come vendere sottoscrizioni ai clienti per prodotti pubblicati da Microsoft e prodotti SaaS pubblicati da ISV di terze parti.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201409"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Creare, sospendere o annullare le sottoscrizioni dei clienti

**Si applica a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Ruoli appropriati:** Agente di amministrazione | Amministratore della fatturazione | Amministratore globale | Supporto per l'agente | Agente di vendita

Dopo aver creato un record del cliente nel Centro per i partner, puoi vendere loro sottoscrizioni per i prodotti nel catalogo. Sono inclusi i prodotti pubblicati da Microsoft e prodotti SaaS (Software as a Service) pubblicati da fornitori di software indipendenti (ISV) di terze parti nel [marketplace commerciale.](https://azuremarketplace.microsoft.com/marketplace)

Alcune offerte sono limitate a una sottoscrizione per cliente. Per vedere l'elenco delle offerte limitate, visita la pagina Prezzi e offerte del Centro per i partner.

>[!IMPORTANT]
> I partner del programma CSP possono  acquistare sottoscrizioni **SaaS** basate su licenza o a consumo da editori ISV all'interno Partner Center. Ciò significa che  è possibile acquistare qualsiasi offerta **SaaS** basata su licenza o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a consumo resa disponibile dall'editore ISV, incluse le offerte esclusive a cui si ha accesso. Per acquistare o gestire altre offerte del marketplace commerciale dagli ISV (ad esempio offerte basate sull'utilizzo che coinvolgono applicazioni di Azure, contenitori o macchine virtuali), è necessario passare al [portale di Azure](https://portal.azure.com/).

>[!NOTE]
>Tutte le date e le ore Partner Center sono specificate nello standard dell'ora UTC (Universal Time Coordinated). Può variare fino a 24 ore rispetto all'ora locale.

## <a name="create-a-new-subscription"></a>Creare una nuova sottoscrizione

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard).

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Selezionare **Aggiungi sottoscrizione**. Nella **scheda Servizi online** verranno mostrate tutte le offerte SaaS del Marketplace disponibili.

4. Per visualizzare solo determinati tipi di sottoscrizioni, effettua le selezioni nei filtri disponibili:
   - **Editore:** scegliere **Microsoft** per visualizzare solo le offerte di Microsoft o **partner** per visualizzare i prodotti del marketplace commerciale pubblicati dagli ISV.
   - **Tipo di fatturazione:** selezionare il tipo di fatturazione della sottoscrizione da usare: **Licenza** o **Utilizzo.** Vedere [Fatturazione basata su licenza](license-based-billing.md) per informazioni che consentono di decidere tra la frequenza di fatturazione mensile e annuale.
   - **Categoria:** scegliere **Enterprise,** **Small Business** o **Trial.** Per informazioni sulle sottoscrizioni di versioni di valutazione, vedi [Offrire ai clienti le versioni di valutazione dei prodotti Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Selezionare le sottoscrizioni al prodotto da acquistare per il cliente. I prodotti visualizzati dipendono dal tipo di segmento di cliente (istruzione, enti pubblici e così via) e dai filtri applicati. Alcune offerte visualizzate nel Marketplace potrebbero non essere sempre disponibili per un cliente specifico o per un partner CSP specifico. Ciò può essere dovuto al seguente:

   - Il cliente ha già una sottoscrizione a tale prodotto e ne è consentita solo una

   - La sottoscrizione del cliente potrebbe essere stata sospesa. In questo caso, è possibile riattivare la sottoscrizione anziché acquistarne una nuova.

   - Per le offerte SaaS ISV, possono esserci alcuni motivi per cui l'offerta non è disponibile per l'acquisto: l'ISV potrebbe non supportare il paese o l'area di fatturazione del cliente; l'ISV potrebbe aver scelto di non rendere disponibile l'offerta tramite il programma CSP; oppure l'ISV potrebbe aver reso l'offerta [esclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo a determinati partner CSP. L'offerta ISV potrebbe anche non essere transazionabile tramite il Partner Center (ad esempio, contenitori o alcune offerte basate sull'utilizzo).  

6. Per ogni sottoscrizione da aggiungere, immettere il numero di licenze (se necessario) e selezionare **Aggiungi al carrello.**

7. Al termine dell'aggiunta delle sottoscrizioni, selezionare **Rivedi** ed esamina l'ordine.

8. Dopo aver esaminato gli ordini e aver pronti per l'acquisto di queste sottoscrizioni, selezionare **Acquista**.

9. Dopo aver acquistato una sottoscrizione per un cliente, si verificheranno le condizioni seguenti:

    - È possibile esaminare o modificare la sottoscrizione selezionando il nome della sottoscrizione dalla pagina **Sottoscrizioni del** cliente. In tale pagina puoi selezionare licenze per componenti aggiuntivi (se disponibili), modificare la quantità di licenze o sospendere la sottoscrizione.

    **Per le sottoscrizioni Isv SaaS (basate su licenza e a consumo):**
    - Si riceverà un collegamento al sito dell'editore ISV. Questo collegamento consente di completare la distribuzione o la configurazione dell'account della sottoscrizione del cliente.
      
    >[!NOTE]
    > Né l'utente né il cliente riceveranno un messaggio di posta elettronica con le istruzioni per completare la configurazione/provisioning dell'account per questo tipo di sottoscrizione ISV.

    - Se la sottoscrizione include una versione di valutazione gratuita di 30 giorni, il periodo di valutazione gratuita verrà applicato automaticamente. I partner del programma CSP non possono rinunciare al periodo di valutazione gratuito per le offerte acquistate per i clienti. Al termine del periodo di valutazione gratuita, il periodo di sottoscrizione inizierà e la sottoscrizione verrà convertita in stato a pagamento. La sottoscrizione verrà quindi rinnovata automaticamente in base alla stessa pianificazione.
   
## <a name="update-subscriptions-with-add-ons"></a>Aggiornare le sottoscrizioni con i componenti aggiuntivi 

Per acquistare un componente aggiuntivo, il cliente deve prima avere una sottoscrizione di base attiva.  Non è possibile acquistare i componenti aggiuntivi tramite il catalogo.

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Scegli la sottoscrizione che vuoi gestire.

4. Sotto la **sezione** Stato è riportato un elenco di componenti aggiuntivi disponibili per la sottoscrizione.  

5. Aggiornare la quantità di licenze per ogni componente aggiuntivo necessario. **Inviare** quindi le modifiche.

La possibilità di acquistare componenti aggiuntivi tramite Partner Center è disponibile solo per i provider di fatturazione diretta e indiretti.
Vengono visualizzati solo i componenti aggiuntivi idonei in base ai requisiti di base e alla disponibilità a livello di regione. Per altre informazioni sui prezzi e sulle offerte, vedere la matrice di offerte cloud reseller. La sospensione della sottoscrizione di base comporta anche la sospensione di tutti i componenti aggiuntivi associati.

Le date di inizio per i componenti aggiuntivi sono allineate alla sottoscrizione di base e gli addebiti vengono calcolati dalla data di inizio e dalla data di fine dell'addebito con addebiti proporzionali nella prima fattura. Per altre informazioni, vedere [Fatturazione basata su licenza.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Sospendere o annullare una sottoscrizione

I partner possono sospendere o annullare una sottoscrizione se richiesto dal cliente o in caso di insolvenza o frode.

### <a name="suspend-a-subscription"></a>Sospendere una sottoscrizione

Quando cambi lo stato di una sottoscrizione in **Sospesa**, gli utenti non possono accedere alla sottoscrizione o ai servizi.

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Scegli la sottoscrizione che vuoi gestire.

4. Nella sezione **Stato**, scegliere **Sospesa**. **Inviare** quindi le modifiche.

5. Verranno eliminati tutti i dati, tranne nel caso in cui la sottoscrizione venga riattivata entro 90 giorni o 90 giorni più il numero di giorni tra il momento in cui l'account è stato aperto e il primo periodo di fatturazione (massimo 120 giorni).

Quando sospendi una sottoscrizione, la data visualizzata sotto il pulsante **Sospesa** indica quando la sottoscrizione scadrà automaticamente se non la riattivi. 

>[!NOTE]
>Le sottoscrizioni CSP non hanno un periodo scaduto (come le sottoscrizioni dirette Web) durante il quale i servizi continuano a funzionare, ma la sottoscrizione non genera alcun addebito per la fatturazione. Le sottoscrizioni CSP sono attive o sospese (o completamente eliminate).

### <a name="cancel-a-subscription"></a>Annullare una sottoscrizione

È possibile annullare sottoscrizioni SaaS basate su licenza da editori ISV di terze parti all'interno Partner Center [marketplace commerciale.](csp-commercial-marketplace-overview.md) Se si annulla entro il periodo di annullamento, si riceverà un rimborso completo.

Per le offerte ISV fatturate mensilmente:

- Se si annulla meno di 24 ore dopo l'ordine, si riceverà un credito completo nella fattura successiva.

- Se si annulla più di 24 ore dopo l'ordine, l'annullamento verrà pianificato al rinnovo.

Per le offerte fatturate annualmente:

- Se si annulla meno di 14 giorni dopo l'ordine, si riceverà un credito completo nella fattura successiva.

- Se si annulla più di 14 giorni dopo l'esecuzione dell'ordine, l'annullamento verrà pianificato al rinnovo.

Al termine di questi periodi, non verrà più visualizzata l'opzione per annullare la sottoscrizione.

> [!NOTE]
> I servizi ISV di terze parti basati sull'utilizzo e a consumo (ad esempio, che usano macchine virtuali o contenitori) non sono idonei per la restituzione. È possibile effettuare il de-provisioning dei servizi basati sull'utilizzo come metodo di annullamento. Poiché gli addebiti vengono fatturati dopo l'uso, questi servizi non sono idonei per un rimborso.

Per annullare una sottoscrizione SaaS basata su licenza da un server di pubblicazione ISV, seguire questa procedura:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Individuare la sottoscrizione da annullare.

4. Nella colonna **Stato** selezionare **Annulla.** **Inviare** quindi le modifiche.

5. Se viene visualizzata una finestra di dialogo, immettere i dettagli pertinenti e quindi selezionare **Invia.**

6. Per confermare l'annullamento, **selezionare Sì, annulla**.

> [!NOTE]
> È anche possibile scegliere di annullare una sottoscrizione Azure Marketplace usando le API. A tale scopo, vedere [Annullare una sottoscrizione Azure Marketplace sottoscrizione.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Scegliere se rinnovare automaticamente una sottoscrizione del Marketplace commerciale

Per impostazione predefinita, le sottoscrizioni attive sono impostate in modo da essere rinnovate automaticamente al termine del periodo di sottoscrizione. Per [le sottoscrizioni ai prodotti del marketplace commerciale,](csp-commercial-marketplace-overview.md)è possibile scegliere di non rinnovare automaticamente la sottoscrizione.

Per impedire il rinnovo automatico di una sottoscrizione attiva del marketplace commerciale:

1. Accedi al [dashboard](https://partner.microsoft.com/dashboard) Centro per i partner.

2. Dal menu Centro per i partner scegli **Clienti** e quindi seleziona un cliente dall'elenco.

3. Selezionare **Sottoscrizioni**. Vengono elencate tutte le sottoscrizioni basate su licenza acquistate per il cliente.

4. Nella **colonna Sottoscrizione** selezionare la sottoscrizione che si vuole modificare.

5. Nella pagina dei dettagli della sottoscrizione individuare la **sezione Stato** e deselezionare la **casella Rinnovo** automatico.

6. Selezionare **Submit** (Invia).

## <a name="next-steps"></a>Passaggi successivi

- [Acquistare prodotti del Marketplace commerciale per i clienti](csp-commercial-marketplace-purchase.md)

- [Gestire i prodotti del marketplace commerciale per i clienti](csp-commercial-marketplace-manage.md)

- [Panoramica del marketplace commerciale](csp-commercial-marketplace-overview.md)