---
title: Eseguire la migrazione delle sottoscrizioni Kaizala Pro a Microsoft 365
description: Informazioni su come eseguire la migrazione delle sottoscrizioni di Kaizala Pro Microsoft 365 versioni di Office 365. Per altre informazioni sulla transizione dei clienti, vedere questo articolo.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172405"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Eseguire la migrazione delle sottoscrizioni autonome di Kaizala Pro Microsoft 365 versioni di Office 365

**Ruoli appropriati**

- Agente di vendita

A partire dal 1° luglio 2020, Microsoft termina le vendite del servizio autonomo Kaizala Pro. I clienti non potranno più acquistare nuove sottoscrizioni Kaizala Pro dopo questa data e le sottoscrizioni Kaizala Pro esistenti non verranno rinnovate automaticamente alla scadenza.

Per garantire la continuità per i clienti, è consigliabile eseguire la transizione dei clienti con sottoscrizioni autonome di Kaizala Pro in scadenza a un'opzione SKU supportata, elencata di seguito. È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti.

Se si usa l'API (STEMM o Partner Center), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà di rinnovo automatico impostata su false: `auto renew = False` .

Le sottoscrizioni E4 verranno impostate su `auto renew=False` il 1° luglio 2020. È possibile spostare i clienti in un nuovo piano in qualsiasi momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Piani di sostituzione autonoma di Kaizala Pro

Con i nuovi piani, i clienti possono sfruttare le funzionalità e le funzionalità più nuove in Microsoft 365. I dettagli dei prezzi sono disponibili nel listino prezzi e nella matrice del listino Partner Center.

- [**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)tra cui:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 per Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)tra cui:
   - Microsoft 365 F3 (in precedenza Microsoft 365 F1) e Office 365 F3
    
- [**Microsoft 365 per Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)tra cui: 
   - Office 365 E1
   - Microsoft 365 E3 e Office 365 E3
   - Microsoft 365 E5 e Office 365 E5

- [**Microsoft 365 per Education,**](https://www.microsoft.com/education/buy-license/microsoft365)tra cui: 
    - Microsoft 365 A1 e Office 365 A1
    - Microsoft 365 A3 e Office 365 A3
    - Microsoft 365 A5 e Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai partner. In questi casi, potrebbe essere necessario aggiornare i clienti a nuovi servizi o eseguire la migrazione delle sottoscrizioni dagli SKU che verranno arrestati. La migrazione dei clienti da SKU ritirati a SKU più recenti richiede i passaggi seguenti:

A. Acquistare la nuova sottoscrizione

B. Riassegnare le licenze utente correnti

C. Annullare la sottoscrizione precedente


## <a name="migrate-your-customers-to-new-plans"></a>Eseguire la migrazione dei clienti a nuovi piani

### <a name="a-purchase-the-new-subscription"></a>A. Acquistare la nuova sottoscrizione

1. Per acquistare la nuova sottoscrizione, dal menu **Partner Center** clienti selezionare **Clienti,** selezionare il cliente che si vuole spostare e quindi selezionare **Aggiungi sottoscrizioni.**

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia.**

Il cliente dovrebbe ora avere sia sottoscrizioni nuove che vecchie, la sottoscrizione kaizala pro autonoma precedente e la nuova sottoscrizione "di destinazione", ad esempio Option 1 - Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Riassegnare le licenze utente correnti

1. Per riassegnare le licenze degli utenti del cliente, dal menu **Partner Center** selezionare **Clienti,** selezionare il cliente che si sta spostando e quindi selezionare **Utenti e licenze.** Verrà visualizzata la pagina Utenti e licenze del cliente.

2. Per riassegnare la licenza utente, selezionare l'utente da riassegnare e quindi selezionare **Gestisci licenze**.

3. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Licenza autonoma Kaizala Pro e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente sta passando.

4.  Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma. Continuare lo stesso processo per altri utenti che necessitano di assegnazioni di licenze.

### <a name="c-cancel-old-subscription"></a>C. Annullare la sottoscrizione precedente

Dopo aver spostata la licenza utente nel nuovo servizio, è possibile annullare in modo sicuro la sottoscrizione ritirata a livello di cliente.

1.  Dal menu **Partner Center** selezionare **Clienti.** Selezionare il cliente di cui si sta annullando la sottoscrizione.

2.  Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione su **Sospeso.**

3.  Selezionare **Submit** (Invia).

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.
