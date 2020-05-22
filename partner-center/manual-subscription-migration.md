---
title: Eseguire la migrazione di sottoscrizioni Dynamics 365 qualificate
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione da sottoscrizioni di base dinamiche 365 qualificate a una nuova sottoscrizione prima della scadenza delle sottoscrizioni esistenti.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 offers, Renew offers, New Dynamics 365 SKU
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795997"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti

**Si applica a**

-  Centro per i partner

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente amministratore
-   Agente di vendita

A partire dal 1 ° gennaio 2019, i clienti con Dynamics 365 per il piano Sales/Customer Engagement dalle sottoscrizioni Basic (offerte qualificate) non possono più rinnovare tali offerte legacy; le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione cambierà in "scade in data [DATE]" da "auto renews on [DATE]". 

Per garantire la continuità per i clienti, è necessario eseguire la transizione con le sottoscrizioni in scadenza a un'opzione supportata, elencate di seguito. È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.

Se si usa l'API (CREST o centro per i partner), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false. Le sottoscrizioni in questione verranno impostate su rinnovo automatico = false il 1 ° gennaio 2019. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Le offerte di Dynamics 365 sono state ritirate

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (offerta qualificata) per studenti
- Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)
- Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata)
- Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti
- Dynamics 365 for Sales Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti
- Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)
- Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata)
- Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per i docenti
- Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition per CRM Basic (offerta qualificata) per studenti
- Componente aggiuntivo Dynamics 365 for Sales Enterprise Edition (prezzi per enti pubblici) per CRM Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) CRMOL Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per studenti
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (offerta qualificata) per i docenti
- Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) di SA per CRM Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per studenti
- Dynamics 365 Customer Engagement Plan Enterprise Edition di SA per CRM Basic (offerta qualificata) per i docenti
- Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (prezzi per enti pubblici) componente aggiuntivo per CRM Basic (offerta qualificata)
- Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per studenti
- Componente aggiuntivo Dynamics 365 Customer Engagement Plan Enterprise Edition per CRM Basic (offerta qualificata) per i docenti



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 per Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)

**Offerte ritirate**   

- Dynamics 365 per le vendite di CRM Basic o CRMOL Basic (offerta qualificata)
- Piano di engagement per i clienti di Dynamics 365 da CRM Basic o CRMOL Basic (offerta qualificata)

**Opzioni di sostituzione**
- Dynamics 365 per Sales Professional (nuovo)
- Dynamics 365 per Sales Professional (nuovo)
- Dynamics 365 for Customer Service
- Piano di coinvolgimento dei clienti di Dynamics 365 o
- Membri del Team Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Il trasferimento dei clienti da SKU ritirati a quelli più recenti richiede i passaggi seguenti nell'ordine indicato:

- Acquistare la nuova sottoscrizione
- Riassegna licenze utente correnti
- Annulla sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Acquistare il nuovo piano per il cliente

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente che si desidera spostare nella nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione**.
3. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**). 

Il cliente avrà ora la sottoscrizione precedente e quella nuova. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.
2. Selezionare **utenti e licenze**.
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi selezionare **Gestisci licenze**. 
4. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Dynamics 365 per il piano Sales/Customer Engagement dalla licenza Basic (offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta migrando. 
5. Selezionare **Invia**. Questa operazione verrà eseguita per ogni utente che richiede la nuova licenza. 

Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente. 

1. Selezionare **Customers (clienti** ) dal NAV a sinistra e quindi selezionare il cliente da trasferire.
2. Nella pagina Dettagli sottoscrizione impostare la sottoscrizione precedente su **sospesa** e selezionare **Invia**.

La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva. Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni. Il cliente non comporterà costi aggiuntivi per la sottoscrizione precedente.
 

 



