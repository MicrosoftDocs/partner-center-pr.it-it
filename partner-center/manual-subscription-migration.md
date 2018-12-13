---
title: Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Enterprise Plan dalle sottoscrizioni di base (offre qualificati) non è più può essere rinnovato.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968271"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti

**Si applica a**

-  Centro per i partner

Effettivi 1 gennaio 2019, i clienti con Dynamics 365 for Sales / Enterprise Plan dalle sottoscrizioni di base (offre qualificati) più possibile rinnovare le offerte legacy; le sottoscrizioni esistenti non verranno rinnovati automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà a "Data di scadenza [Data]" da "Rinnovo automatico il [Data]". 


Per garantire la continuità, è opportuno trasferire quelli con sottoscrizioni in scadenza a delle opzioni supportate elencati di seguito. Ti consigliamo di far sottoscrivere ai clienti nuove sottoscrizioni prima della data di scadenza annuale della sottoscrizione, al fine di evitare eventuali interruzioni del servizio.

Se si utilizza l'API (CREST o centro per i Partner), puoi trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme automatico = False proprietà. Le sottoscrizioni in questione verranno impostate su auto renew = False il 1 gennaio 2019. Puoi trasferire i clienti a un nuovo piano in qualsiasi momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Il Dynamics 365 offre viene ritirato

- Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (qualificato offerta)
- Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (offerta qualificato) per istituti di istruzione
- Dynamics 365 per la vendita Enterprise Edition CRMOL Basic (offerta qualificato) per studenti
- Dynamics 365 per la vendita Enterprise Edition (enti pubblici sui prezzi) CRMOL Basic (qualificato offerta)
- Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (qualificato offerta)
- Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (offerta qualificato) per istituti di istruzione
- Dynamics 365 per l'edizione Enterprise di vendita da SA per Basic CRM (offerta qualificato) per studenti
- Dynamics 365 per la vendita Enterprise Edition (enti pubblici sui prezzi) da SA per Basic CRM (qualificato offerta)
- Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (qualificato offerta)
- Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (offerta qualificato) per istituti di istruzione
- Dynamics 365 per componente aggiuntivo edizione Enterprise di vendita per Basic CRM (offerta qualificato) per studenti
- Dynamics 365 per componente aggiuntivo di vendita Enterprise Edition (enti pubblici sui prezzi) per Basic CRM (qualificato offerta)
- Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (qualificato offerta)
- Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) CRMOL Basic (qualificato offerta)
- Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (offerta qualificato) per gli studenti
- Dynamics 365 cliente Engagement piano Enterprise Edition CRMOL Basic (offerta qualificato) per istituti di istruzione
- Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (qualificato offerta)
- Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) da SA per Basic CRM (qualificato offerta)
- Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (offerta qualificato) per gli studenti
- Dynamics 365 Customer coinvolgimento piano Enterprise Edition da SA per Basic CRM (offerta qualificato) per istituti di istruzione
- Dynamics 365 cliente Engagement piano Enterprise Edition un componente aggiuntivo per Basic CRM (qualificato offerta)
- Dynamics 365 cliente Engagement piano Enterprise Edition (enti pubblici sui prezzi) un componente aggiuntivo per Basic CRM (qualificato offerta)
- Dynamics 365 Customer coinvolgimento piano Enterprise Edition un componente aggiuntivo per Basic CRM (offerta qualificato) per gli studenti
- Dynamics 365 Customer coinvolgimento piano Enterprise Edition un componente aggiuntivo per Basic CRM (offerta qualificato) per istituti di istruzione



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / Enterprise Plan da sostituzione Basic (offre qualificati) piani

**Offerte ritirate**   

- Dynamics 365 for Sales da CRM Basic o CRMOL Basic (qualificato offerta)
- Piano Dynamics 365 Customer Engagement da CRM Basic o CRMOL Basic (qualificato offerta)

**Opzioni di sostituzione**
- Dynamics 365 per la vendita Professional (novità)
- Dynamics 365 per la vendita Professional (novità)
- Dynamics 365 for Customer Service
- Piano Dynamics 365 Customer Engagement oppure
- Membri del Team Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Spostare i clienti da SKU ritirati a quelli più recenti richiede la procedura seguente in questo ordine:

- Acquistare il nuovo abbonamento
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Il nuovo piano di acquisto per il cliente

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente da trasferire alla nuova sottoscrizione.
2. Seleziona **Aggiungi sottoscrizione**.
3. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**. 

Il cliente verrà ora avere sia la sottoscrizione precedente e quello nuovo. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.
2. Seleziona **Utenti e licenze**.
3. Per riassegnare una licenza a un utente, seleziona l'utente e quindi seleziona **Gestisci licenze**. 
4. Nella pagina **Gestisci licenze** , cancellare il Dynamics 365 for Sales / piano di coinvolgimento dei clienti da Basic (offrire qualificati) casella di controllo della licenza e seleziona un nuovo piano di servizio per l'abbonamento a cui sta passando il cliente. 
5. Seleziona **Invia**. Lo farai per ogni utente che richiede la nuova licenza. 

Dopo avere spostato le licenze alla nuova sottoscrizione puoi annullare la sottoscrizione precedente. 

1. Seleziona **i clienti** di spostamento a sinistra e quindi seleziona il cliente che si stanno spostando.
2. Nella pagina dei dettagli della sottoscrizione imposta la sottoscrizione precedente in **sospeso** e seleziona **Invia**.

La sottoscrizione precedente viene ora sospesa e la nuova sottoscrizione diventa attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non incorrere costi aggiuntivi necessari per la sottoscrizione precedente.
 

 



