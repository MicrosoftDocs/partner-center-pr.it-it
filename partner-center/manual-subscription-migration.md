---
title: Eseguire la migrazione di sottoscrizioni qualificate di Dynamics 365
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come eseguire la migrazione da sottoscrizioni dynamics 365 di base qualificate a una nuova sottoscrizione prima della scadenza delle sottoscrizioni esistenti.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151645"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Eseguire la migrazione di Dynamics 365 ed Enterprise Plan da Basic (qualificate offerte) alle versioni più recenti

**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente amministratore | Agente di vendita

A partire dal 1° gennaio 2019, i clienti con Dynamics 365 for Sales/Customer Engagement Plan delle sottoscrizioni Basic (Offerte qualificate) non possono più rinnovare queste offerte legacy; Le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza. Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione verrà modificato in "Scadenza alla [data]" da "Rinnovo automatico il [data]". 

Per garantire la continuità per i clienti, è necessario eseguire la transizione di quelli con sottoscrizioni in scadenza a un'opzione supportata, elencata di seguito. È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.

Se si usa l'API (STEMM o Partner Center), è possibile trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà rinnovo automatico = False. Le sottoscrizioni in questione verranno impostate su auto renew=False il 1° gennaio 2019. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Le offerte dynamics 365 vengono ritirate

- Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata)
- Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata) per docenti
- Dynamics 365 for Sales edizione Enterprise CRMOL Basic (offerta qualificata) per studenti
- Dynamics 365 for Sales edizione Enterprise (government pricing) CRMOL Basic (offerta qualificata)
- Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer)
- Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) for Faculty (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 for Sales edizione Enterprise from SA for CRM Basic (Qualified Offer) for Students (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students (Dynamics 365 for Sales edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 for Sales edizione Enterprise (prezzi per enti pubblici) Dalla sa per CRM Basic (offerta qualificata)
- Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Offerta qualificata)
- Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 for Sales edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Students
- Dynamics 365 for Sales edizione Enterprise (government pricing) Add-On for CRM Basic (Qualified Offer)
- Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) CRMOL Basic (Qualified Offer)
- Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata) per studenti
- Piano Dynamics 365 Customer Engagement edizione Enterprise CRMOL Basic (offerta qualificata) per docenti
- Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) From SA for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan edizione Enterprise From SA for CRM Basic (Qualified Offer) for Faculty
- Piano Dynamics 365 Customer Engagement edizione Enterprise Add-On per CRM Basic (offerta qualificata)
- Dynamics 365 Customer Engagement Plan edizione Enterprise (government pricing) Add-On for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan edizione Enterprise Add-On for CRM Basic (Qualified Offer) for Faculty



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement Plan da piani di sostituzione Basic (offerte qualificate)

**Offerte ritirate**   

- Dynamics 365 for Sales da CRM Basic o CRMOL Basic (offerta qualificata)
- Piano Dynamics 365 Customer Engagement di CRM Basic o CRMOL Basic (offerta qualificata)

**Opzioni di sostituzione**
- Dynamics 365 for Sales Professional (NUOVO)
- Dynamics 365 for Sales Professional (NUOVO)
- Dynamics 365 for Customer Service
- Piano di Dynamics 365 Customer Engagement o
- Membri del team di Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Per spostare i clienti da SKU ritirati a SKU più recenti, è necessario eseguire i passaggi seguenti in questo ordine:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

## <a name="purchase-the-new-plan-for-your-customer"></a>Acquistare il nuovo piano per il cliente

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente da spostare nella nuova sottoscrizione.
2. Selezionare **Aggiungi sottoscrizione.**
3. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.** 

Il cliente avrà ora sia la sottoscrizione precedente che quella nuova. Il passaggio successivo consiste nel riassegnare le licenze agli utenti del cliente.

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.
2. Selezionare **Utenti e licenze.**
3. Per riassegnare una licenza a un utente, selezionare l'utente e quindi **selezionare Gestisci licenze.** 
4. Nella  pagina Gestisci licenze deselezionare la casella di controllo Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Piano Dynamics 365 for Sales/Customer Engagement dalla licenza Basic - Offerta qualificata) e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente. 
5. Selezionare **Submit** (Invia). Questa operazione verrà creata per ogni utente che necessita della nuova licenza. 

Dopo aver spostato le licenze nella nuova sottoscrizione, è possibile annullare la sottoscrizione precedente. 

1. Selezionare **Clienti** nel riquadro di spostamento a sinistra e quindi selezionare il cliente che si sta spostando.
2. Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione precedente su **Sospeso** e selezionare **Invia**.

La sottoscrizione precedente è ora sospesa e la nuova sottoscrizione è attiva. Il provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni. Il cliente non incorrerà in costi aggiuntivi per la sottoscrizione precedente.
 

 



