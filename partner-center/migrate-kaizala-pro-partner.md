---
title: Eseguire la migrazione di sottoscrizioni Kaizala Pro a Microsoft365
description: Informazioni su come eseguire la migrazione di sottoscrizioni Kaizala Pro a Microsoft365 o versioni di Office 365. Leggere questo articolo per altre informazioni sulla transizione dei clienti.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175173"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Eseguire la migrazione di sottoscrizioni Kaizala Pro autonome a Microsoft365 o versioni di Office 365

A partire dal 1 ° luglio 2020, Microsoft sta terminando le vendite del servizio Kaizala Pro autonomo. I clienti non saranno più in grado di acquistare nuove sottoscrizioni Kaizala Pro dopo questa data e le sottoscrizioni Kaizala Pro esistenti non verranno rinnovate automaticamente alla scadenza.

Per garantire la continuità per i clienti, è necessario eseguire la transizione dei clienti con sottoscrizioni Kaizala Pro autonome in scadenza a un'opzione SKU supportata, elencate di seguito. È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti.

Se si usa l'API (CREST o centro per i partner), è possibile individuare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà rinnovo automatico impostata su false: `auto renew = False` .

Le sottoscrizioni E4 verranno impostate `auto renew=False` su il 1 ° luglio 2020. È possibile spostare i clienti in un nuovo piano in qualsiasi momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Piani di sostituzione Kaizala Pro autonomo

Con i nuovi piani, i clienti possono sfruttare le funzionalità e le funzionalità più recenti in Microsoft 365. I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner.

- [**Microsoft 365 per le aziende**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), tra cui:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 per Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), tra cui:
   - Microsoft 365 F3 (in precedenza Microsoft 365 F1) e Office 365 F3
    
- [**Microsoft 365 per Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), tra cui: 
   - Office 365 E1
   - Microsoft 365 E3 e Office 365 E3
   - Microsoft 365 E5 e Office 365 E5

- [**Microsoft 365 per la formazione**](https://www.microsoft.com/education/buy-license/microsoft365), tra cui: 
    - Microsoft 365 A1 e Office 365 A1
    - Microsoft 365 A3 e Office 365 A3
    - Microsoft 365 A5 e Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate. Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:

R. Acquistare la nuova sottoscrizione

B. Riassegna licenze utente correnti

C. Annulla sottoscrizione precedente


## <a name="migrate-your-customers-to-new-plans"></a>Esegui la migrazione dei clienti ai nuovi piani

### <a name="a-purchase-the-new-subscription"></a>R. Acquistare la nuova sottoscrizione

1. Per acquistare la nuova sottoscrizione, scegliere **Customers**dal menu centro per i **partner** , selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**).

Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la vecchia sottoscrizione Kaizala Pro autonoma e la nuova sottoscrizione di destinazione, ad esempio, l'opzione 1-Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Riassegna licenze utente correnti

1. Per riassegnare le licenze degli utenti del cliente, dal menu **centro** per i partner selezionare **clienti**, selezionare il cliente da trasferire, quindi selezionare **utenti e licenze**. Verrà visualizzata la pagina utenti e licenze del cliente.

2. Per riassegnare la licenza utente, selezionare l'utente da riassegnare, quindi selezionare **Gestisci licenze**.

3. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Kaizala Pro standalone License e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta muovendo il cliente.

4.  Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma. Continuare lo stesso processo per gli altri utenti che necessitano di assegnazioni di licenze.

### <a name="c-cancel-old-subscription"></a>C. Annulla sottoscrizione precedente

Dopo aver spostato la licenza utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata a livello di cliente.

1.  Scegliere **clienti**dal menu **centro partner** . Selezionare il cliente di cui annullare la sottoscrizione.

2.  Nella pagina Dettagli sottoscrizione impostare la sottoscrizione su **sospesa**.

3.  Selezionare **Submit** (Invia).

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.
