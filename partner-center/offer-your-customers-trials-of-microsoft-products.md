---
title: Offrire ai clienti le versioni di valutazione dei prodotti Microsoft | Centro per i partner
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: I tuoi clienti possono testare i prodotti a sottoscrizione Microsoft per 30 giorni. Iscriversi a queste versioni di valutazione nel catalogo proprio come molti altri Servizi online.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: a0f511ad2275866552e9646cf433351ae4fc3be3
ms.sourcegitcommit: a80838c0e79f66c28b958165e910871dd37d39f0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/18/2019
ms.locfileid: "75185541"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Offrire ai clienti le versioni di valutazione dei prodotti Microsoft

**Si applica a**

- Centro per i partner

**Ruoli appropriati**
-   Amministratore globale 
-   Amministratore utenti
-   Agente di vendita

Un buon metodo per presentare ai clienti i nuovi prodotti Microsoft è offrire versioni di valutazione gratuite di 30 giorni. Puoi registrarti per le versioni di valutazione nel catalogo esattamente come per molti altri servizi online. Tutti i partner.

## <a name="available-trial-offers"></a>Offerte di valutazione disponibili

Tutte le offerte di valutazione in attesa sono disponibili nella pagina del **cliente** . Questa pagina elenca tutte le sottoscrizioni, incluse le versioni di valutazione gratuite e quelle a pagamento. Questa funzionalità non è attualmente disponibile in Cina.

Ogni cliente ha diritto a una versione di valutazione gratuita per ogni offerta disponibile. Possono ad esempio ottenere una versione di valutazione gratuita per Office 365 Business Premium e un'altra per Office 365 E3. Tuttavia, se il cliente è già proprietario dell'offerta, non potrà usare una versione di valutazione gratuita per l'offerta.

### <a name="available-products"></a>Prodotti disponibili

Sono disponibili versioni di valutazione gratuite per i seguenti prodotti:

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 con PSTN
- Office 365 E5 senza PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Piano 1
- Dynamics 365 Business Central
- Microsoft 365 Business

Offriamo versioni di valutazione gratuite per questi prodotti perché sono le offerte aziendali più complete e popolari. È possibile che in futuro siano disponibili altre offerte di versioni di valutazione gratuite.

Attualmente non sono disponibili **versioni di valutazione gratuite** per offerte per enti pubblici, offerte di formazione o offerte di componenti aggiuntivi.

## <a name="licenses-for-free-trial-offers"></a>Licenze per le offerte della versione di valutazione gratuita

Tutte le versioni di valutazione gratuite forniscono 25 licenze. Non è possibile modificare questo numero durante la versione di valutazione. Non è possibile aggiungere o rimuovere le postazioni nella versione di valutazione gratuita. Dopo che la versione di valutazione è stata convertita in una sottoscrizione a pagamento, è possibile aggiungere altre licenze alla sottoscrizione.

È consigliabile assegnare le licenze e le postazioni di valutazione esattamente come per un servizio a pagamento nel centro per i partner.

## <a name="sign-customers-up-for-trials"></a>Accedi ai clienti per le versioni di valutazione

Per firmare il cliente per una versione di valutazione tramite il centro per i partner:

1. Da **sell** nel centro per i partner passare a **Catalog**. 
2. Nel catalogo fai clic su **Trial offer** in **Frequenza fatturazione**. Questa operazione consente di abilitare solo le versioni di valutazione gratuite e disabilitare altre offerte non gratuite. Le versioni di valutazione verranno visualizzate nella scheda **Versioni di valutazione** del catalogo.
3. Seleziona la versione di valutazione gratuita che desideri offrire, quindi seleziona **Invia**. Tutte le versioni di valutazione sono valide per 30 giorni e durante questo periodo non ti verrà addebitato alcun costo. Inoltre puoi convertirla in una sottoscrizione a pagamento in qualsiasi momento durante il periodo della versione di valutazione.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversione di versioni di valutazione in sottoscrizioni a pagamento

Una versione di valutazione gratuita non viene convertita automaticamente in una sottoscrizione a pagamento. Dopo trenta giorni, una versione di valutazione gratuita deve essere convertita in una sottoscrizione a pagamento o [scadrà](#expiring-offers). Non è possibile estendere le versioni di valutazione gratuite.

Dovrai convertire la versione di valutazione in una sottoscrizione a pagamento. Questa operazione può essere eseguita [tramite il centro](#convert-trials-using-partner-center) per i partner o [tramite le API del centro per i partner](#convert-trials-using-apis).

> [!NOTE]
> Le versioni di valutazione gratuite del cliente per il programma Cloud Solution Provider (CSP) non possono essere convertite in un altro tenant del programma (ad esempio EA, Open o MOSP).

### <a name="convert-trials-using-partner-center"></a>Converti le versioni di valutazione con il centro per i partner

È possibile convertire le versioni di valutazione in sottoscrizioni a pagamento usando il dashboard del centro per i partner come segue:

1. Vai alla pagina della sottoscrizione del cliente e seleziona la versione di valutazione gratuita.
2. Seleziona **Convertire una versione di valutazione in sottoscrizione a pagamento**
3. Immetti il numero di licenze desiderato e la frequenza di fatturazione, quindi seleziona **Applica**.
4. La fatturazione per la sottoscrizione a pagamento inizia alla data di conversione e la sottoscrizione si rinnova automaticamente dopo 12 mesi dalla data di conversione. 

### <a name="convert-trials-using-apis"></a>Convertire le versioni di valutazione usando le API

Potrebbe essere necessario modificare le API per adattarla alla conversione di una versione di valutazione gratuita a una sottoscrizione a pagamento. Per ulteriori informazioni, vedere la seguente documentazione per gli sviluppatori:

- [Convertire un abbonamento di valutazione in uno a pagamento](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Ottenere un elenco delle offerte di conversione della copia di valutazione](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Offerte in scadenza

L'utente non riceverà alcuna notifica delle offerte in scadenza. È possibile tenere traccia delle date di scadenza future usando la visualizzazione clienti nel centro per i partner o eseguendo una query sull'API. È consigliabile monitorare queste date di frequente in modo da poter intraprendere le azioni appropriate quando si avvicinano i momenti critici in cui i clienti devono prendere una decisione.

Dopo la scadenza di una versione di valutazione, un cliente che tenta di accedere a tale versione di valutazione visualizzerà un messaggio di scadenza. Tuttavia, i dati vengono archiviati in linea con gli standard di conservazione dei dati. Dopo l'acquisto di una nuova sottoscrizione con gli stessi piani di servizio, è possibile accedere nuovamente alle informazioni del cliente dalla sottoscrizione appena attivata.

## <a name="billing"></a>Fatturazione

La fatturazione annuale e le versioni di valutazione gratuite sono le stesse nei cloud sovrani e nel cloud pubblico. L'unica differenza è rappresentata dagli SKU di valutazione disponibili al momento dell'avvio.

## <a name="billing-for-free-trials"></a>Fatturazione per le versioni di valutazione gratuite

Le versioni di valutazione gratuite possono essere utilizzate sia per le sottoscrizioni mensili che annuali. È possibile selezionare la frequenza di fatturazione quando si converte la versione di valutazione in una sottoscrizione a pagamento.

La data di inizio della sottoscrizione è basata sulla data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione annuale, la data di rinnovo dell'abbonamento cade 12 mesi dopo la data di conversione. Se la versione di valutazione gratuita viene convertita in un'offerta a pagamento con fatturazione mensile, la data di rinnovo dell'abbonamento cade 12 mesi dopo la data di fatturazione successiva alla data di conversione.

### <a name="invoices"></a>Fatture

Non verranno visualizzate le versioni di valutazione gratuite elencate nel file di riconciliazione della fattura o della licenza. Le versioni di valutazione gratuite verranno visualizzate solo nel file di riconciliazione delle fatture e delle licenze dopo la conversione di una versione di valutazione gratuita in una sottoscrizione a pagamento. La sottoscrizione convertita verrà visualizzata allo stesso modo di qualsiasi nuova sottoscrizione.

### <a name="incentives"></a>Incentivi

Le versioni di valutazione gratuite non influiscano sugli incentivi.

## <a name="support"></a>Supporto tecnico

Per il supporto delle versioni di valutazione gratuite, inviare una richiesta di assistenza tramite il centro per i partner.
