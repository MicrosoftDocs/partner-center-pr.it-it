---
title: Offrire ai clienti versioni di valutazione dei prodotti Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consentire ai clienti di provare i prodotti in sottoscrizione Microsoft per 30 giorni. Iscriversi a queste versioni di valutazione gratuite nel catalogo come molte altre Servizi online.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151135"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Offrire ai clienti versioni di valutazione gratuite di 30 giorni dei prodotti Microsoft

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente di vendita

Un buon modo per presentare i clienti ai nuovi prodotti Microsoft è offrire versioni di valutazione gratuite di 30 giorni. È possibile iscriversi alle versioni di valutazione nel catalogo come molte altre Servizi online. Tutti i partner.

## <a name="available-trial-offers"></a>Offerte di valutazione disponibili

Tutte le offerte di valutazione in sospeso sono disponibili nella **pagina Cliente.** Questa pagina elenca tutte le sottoscrizioni, incluse le versioni di valutazione gratuite e le sottoscrizioni a pagamento. Questa funzionalità non è attualmente disponibile in Cina.

Ogni cliente ha diritto a una versione di valutazione gratuita per ogni offerta disponibile. Ad esempio, possono ottenere una versione di valutazione gratuita per Microsoft 365 Business Standard e una versione di valutazione gratuita per Office 365 E3. Tuttavia, se il cliente è già proprietario dell'offerta, non può usare una versione di valutazione gratuita per tale offerta.

### <a name="available-products"></a>Prodotti disponibili

Le versioni di valutazione gratuite sono disponibili per le offerte più complete e più popolari basate su licenza. Le nuove offerte di valutazione possono essere introdotte su base mensile.

I partner possono trovare le versioni di valutazione nel listino prezzi mensile nella pagina **prezzi e** offerte in Partner Center. Le offerte di valutazione avranno "TRIAL" elencate nella colonna Price list **Secondary License Type (Tipo di licenza secondaria).**

Attualmente non sono **disponibili versioni di valutazione gratuite per** offerte per enti pubblici, offerte di formazione o offerte di componenti aggiuntivi.

## <a name="licenses-for-free-trial-offers"></a>Licenze per le offerte di valutazione gratuite

Tutte le versioni di valutazione gratuite offrono 25 licenze. Non è possibile modificare questo numero durante la versione di valutazione. Non è possibile aggiungere o rimuovere licenze nella versione di valutazione gratuita. Dopo aver convertito la versione di valutazione in una sottoscrizione a pagamento, è possibile aggiungere altre licenze alla sottoscrizione.

Le licenze di valutazione devono essere assegnate agli utenti nello stesso modo in cui vengono assegnate le licenze dei servizi a pagamento.

## <a name="sign-customers-up-for-trials"></a>Iscriversi ai clienti per le versioni di valutazione

Ottenere una versione di valutazione per il cliente in Partner Center:

1. In **Sell** on the Partner Center (Partner Center vendita) passare a **Catalog (Catalogo).** 
2. Nel catalogo, in **Frequenza di fatturazione** selezionare Offerta **di valutazione.** In questo modo vengono visualizzate solo le versioni di valutazione gratuite e vengono disabilitate altre offerte non gratuite. Le versioni di valutazione verranno mostrate nella scheda Versioni **di** valutazione del catalogo.
3. Selezionare la versione di valutazione gratuita che si vuole offrire e quindi selezionare **Invia.** Tutte le versioni di valutazione sono per 30 giorni durante i quali non verrà fatturato. È anche possibile convertirlo in una sottoscrizione a pagamento in qualsiasi momento durante la versione di valutazione.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversione delle versioni di valutazione in sottoscrizioni a pagamento

Una versione di valutazione gratuita non viene convertita automaticamente in una sottoscrizione a pagamento. Dopo 30 giorni, una versione di valutazione gratuita deve essere convertita in una sottoscrizione a pagamento o [scadrà](#expiring-offers). Le versioni di valutazione gratuite non possono essere estese.

È necessario convertire la versione di valutazione in una sottoscrizione a pagamento. È possibile eseguire questa [operazione usando Partner Center](#convert-trials-using-partner-center) o tramite le API Partner Center [.](#convert-trials-using-apis)

> [!NOTE]
> Le versioni di valutazione gratuite dei clienti per il programma Cloud Solution Provider (CSP) non possono essere convertite in un altro tenant del programma, ad esempio EA, Open o MOSP.

### <a name="convert-trials-using-partner-center"></a>Convertire le versioni di valutazione usando Partner Center

È possibile convertire le versioni di valutazione in sottoscrizioni a pagamento usando Partner Center:

1. Passare alla pagina della sottoscrizione del cliente e selezionare la versione di valutazione gratuita.
2. Selezionare **Convert trial to paid subscription (Converti versione di valutazione in sottoscrizione a pagamento).**
3. Immettere la quantità di licenza e la frequenza di fatturazione desiderate e selezionare **Applica**.
4. La fatturazione per la sottoscrizione a pagamento inizia alla data di conversione e la sottoscrizione viene rinnovata automaticamente 12 mesi dalla data di conversione. 

### <a name="convert-trials-using-apis"></a>Convertire le versioni di valutazione con le API

Potrebbe essere necessario modificare le API per supportare la conversione di una versione di valutazione gratuita in una sottoscrizione a pagamento. Per altre informazioni, vedere la documentazione per sviluppatori seguente:

- [Convertire un abbonamento di valutazione in uno a pagamento](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Ottenere un elenco delle offerte di conversione della copia di valutazione](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Versioni di valutazione senza conversioni

Non tutte le versioni di valutazione possono essere convertite in sottoscrizioni a pagamento. I partner possono usare una versione di valutazione senza conversioni fino alla data di scadenza. I partner possono acquistare offerte compatibili che supportano gli stessi servizi dell'offerta di valutazione.  Questa operazione deve essere eseguita prima della scadenza della versione di valutazione per garantire che i servizi delle offerte appena acquistate siano allineati ai servizi della versione di valutazione. 

|**Versione di valutazione**   |**Offerte di piccole imprese compatibili**   |**Offerte Enterprise compatibili**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Versione di valutazione di Microsoft Teams Commercial Cloud (avviata dall'utente)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (in precedenza F1), Office 365 for Enterprise (E1, E3 ed E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Le offerte precedenti hanno piani di servizio simili con funzionalità simili, tuttavia potrebbero esserci alcune differenze tra le offerte.

### <a name="expiring-offers"></a>Offerte in scadenza

Non verrà notificata la scadenza delle offerte. È possibile tenere traccia delle prossime date di scadenza usando la visualizzazione del cliente Partner Center o tramite query sull'API. È consigliabile monitorare queste date di frequente in modo da poter intraprendere le azioni appropriate quando si avvicinano i momenti critici in cui i clienti devono prendere una decisione.

Dopo la scadenza di una versione di valutazione, un cliente che tenta di accedere a tale versione di valutazione visualizza un messaggio di scadenza. Tuttavia, i dati vengono archiviati in base agli standard di conservazione dei dati. Dopo aver acquistato una nuova sottoscrizione con gli stessi piani di servizio, è possibile accedere di nuovo alle informazioni del cliente dalla sottoscrizione appena attivata.

## <a name="billing"></a>Fatturazione

La fatturazione annuale e le versioni di valutazione gratuite sono le stesse nei cloud sovrani e nel cloud pubblico. L'unica differenza è che gli SKU di valutazione sono disponibili al momento dell'avvio.

## <a name="billing-for-free-trials"></a>Fatturazione per le versioni di valutazione gratuite

Le versioni di valutazione gratuite possono essere usate sia per le sottoscrizioni mensili che per le sottoscrizioni fatturate annualmente. È possibile selezionare la frequenza di fatturazione quando si converte la versione di valutazione in una sottoscrizione a pagamento.

La data di inizio della sottoscrizione è basata sulla data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione annuale, la data di rinnovo della sottoscrizione sarà di 12 mesi dalla data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione mensile, la data di rinnovo dell'abbonamento cade 12 mesi dopo la data di fatturazione successiva alla data di conversione.

### <a name="invoices"></a>Fatture

Le versioni di valutazione gratuite non saranno elencate nella fattura o nel file di riconciliazione basato su licenza. Le versioni di valutazione gratuite verranno visualizzate nella fattura e nel file di riconciliazione basato su licenza solo dopo la conversione di una versione di valutazione gratuita in una sottoscrizione a pagamento. La sottoscrizione convertita verrà visualizzata nello stesso modo di qualsiasi nuova sottoscrizione.

### <a name="incentives"></a>Incentivi

Le versioni di valutazione gratuite non influiscono sugli incentivi.

## <a name="support"></a>Supporto

Per il supporto nelle versioni di valutazione gratuite, inviare una richiesta di servizio tramite Partner Center.