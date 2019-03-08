---
title: Eseguire la migrazione di Dynamics 365 e si prevede di Engagement dei clienti da Basic (offerte completo) per le versioni più recenti | Centro per i partner
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales / Customer Engagement pianificare dalle sottoscrizioni Basic (offre completo) non può essere rinnovato.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offre, rinnovare le offerte, nuovi SKU di Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586944"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti

**Si applica a**

-  Centro per i partner

I clienti il 1 gennaio 2019 efficaci con Dynamics 365 for Sales / Customer Engagement pianificare dalle sottoscrizioni Basic (offre completo) non effettuare il rinnovo non è più queste offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà per "Expires su [date]" da "Rinnova automaticamente in [date]". 


Per garantire continuità aziendale per i clienti, è necessario eseguire la transizione quelli con le sottoscrizioni in scadenza un'opzione supportata, elencati di seguito. Si consiglia di far passare i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento, al fine di evitare eventuali interruzioni del servizio.

Se si usa l'API (CREST o centro per i Partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione con l'automobile vengono rinnovate = False proprietà. Le sottoscrizioni in questione verranno impostate su auto rinnovare = False su 1 gennaio 2019. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Di Dynamics 365 offre in fase di ritiro

- Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo)
- Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo) per istituti di istruzione
- Dynamics 365 per vendita Enterprise Edition CRMOL Basic (offerta completo) per gli studenti
- Dynamics 365 per vendita Enterprise Edition (prezzo per enti pubblici) CRMOL Basic (offerta completo)
- Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo)
- Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo) per istituti di istruzione
- Dynamics 365 per l'edizione Enterprise di vendita da software Assurance per CRM Basic (offerta completo) per gli studenti
- Dynamics 365 per vendita Enterprise Edition (prezzo per enti pubblici) da software Assurance per CRM Basic (offerta completo)
- Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo)
- Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo) per istituti di istruzione
- Dynamics 365 per il componente aggiuntivo di edizione Enterprise di vendite per CRM Basic (offerta completo) per gli studenti
- Dynamics 365 per il componente aggiuntivo di vendita Enterprise Edition (prezzo per enti pubblici) per CRM Basic (offerta completo)
- Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo)
- Dynamics 365 Customer Engagement piano Enterprise Edition (prezzo per enti pubblici) CRMOL Basic (offerta completo)
- Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo) per gli studenti
- Dynamics 365 Customer Engagement piano Enterprise Edition CRMOL Basic (offerta completo) per istituti di istruzione
- Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo)
- Dynamics 365 Customer Engagement piano Enterprise Edition (prezzo per enti pubblici) da software Assurance per CRM Basic (offerta completo)
- Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo) per gli studenti
- Dynamics 365 Customer Engagement piano Enterprise Edition da software Assurance per CRM Basic (offerta completo) per istituti di istruzione
- Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo)
- Dynamics 365 Customer Engagement Enterprise Edition (prezzo per enti pubblici) componente aggiuntivo del piano Basic CRM (offerta completo)
- Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo) per gli studenti
- Dynamics 365 Customer Engagement Enterprise Edition componente aggiuntivo del piano Basic CRM (offerta completo) per istituti di istruzione



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales / piani di Customer Engagement piano dalla sostituzione Basic (offre completo)

**Offerte ritirate**   

- Dynamics 365 for Sales da CRM Basic o CRMOL Basic (offerta completo)
- Dynamics 365 Customer Engagement piano da CRM Basic o CRMOL Basic (offerta completo)

**Opzioni di sostituzione**
- Dynamics 365 for Sales Professional (nuovo)
- Dynamics 365 for Sales Professional (nuovo)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement piano o
- Membri del Team Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

I clienti lo spostamento dal ritirati SKU quelli più recenti richiede i passaggi seguenti nell'ordine indicato:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Il nuovo piano di acquisto per il cliente

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente che si desidera spostare la nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione**.
3. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**. 

Il cliente avrà la sottoscrizione precedente sia quello nuovo. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.
2. Seleziona **Utenti e licenze**.
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **gestire le licenze**. 
4. Nel **gestire le licenze** pagina, cancellare il di Dynamics 365 for Sales / piano di Engagement dei clienti da Basic (completi dell'offerta) casella di controllo di licenza e selezionare un nuovo piano di servizio per la sottoscrizione cliente stia passando ad. 
5. Seleziona **Invia**. Si eseguirà questa operazione per ogni utente che necessita la nuova licenza. 

Dopo aver spostato le licenze alla nuova sottoscrizione è possibile annullare la sottoscrizione precedente. 

1. Selezionare **clienti** da di spostamento a sinistra e quindi selezionare il cliente si stanno spostando.
2. Nella pagina di dettagli della sottoscrizione, impostare la sottoscrizione precedente **degli elementi sospesi** e selezionare **Submit**.

La sottoscrizione precedente a questo punto viene sospeso e la nuova sottoscrizione è attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non incorrerà costi aggiuntivi per la sottoscrizione precedente.
 

 



