---
title: Eseguire la migrazione di alcune sottoscrizioni di Skype for business
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Informazioni su come e quando migrare determinati clienti con sottoscrizioni del piano 1 di Skype for business online in scadenza alle nuove versioni di Office 365.
author: BrentSerbus
ms.author: brserbus
keywords: Piani di Skype for business, ritiro di Skype, Office 365
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4202e146a470e2231ac33df9878be91e19fcddf3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949617"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Eseguire la migrazione di sottoscrizioni di Skype for Business Online piano 1 alla versione più recente di Office 365

**Si applica a**

- Centro per i partner

Il piano 1 di Skype for business online verrà ritirato, a partire dal 1 ° agosto 2018. Dopo tale data, i clienti non potranno più acquistare nuove sottoscrizioni di Skype for business piano 1 e le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza e non forniranno un'opzione di rinnovo. Nella pagina dei dettagli della sottoscrizione, lo stato della sottoscrizione del piano 1 di Skype for business online è stato modificato in "scade in data [DATE]" da "auto renews on [DATE]".  

Per garantire la continuità per i clienti, è consigliabile eseguire la transizione dei clienti con sottoscrizioni di Skype for business online piano 1 in scadenza a un'opzione SKU supportata, elencate di seguito. È consigliabile trasferire i clienti a nuove sottoscrizioni prima della data di fine annuale della sottoscrizione, in modo da evitare eventuali interruzioni del servizio per i clienti. 

>[!NOTE]
>Gli SKU commerciali e governativi del piano 1 di Skype for business online sono stati ritirati.

Se si usa l'API (CREST o centro per i partner), trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto Renew = false. Le sottoscrizioni del piano 1 di Skype for business online verranno impostate su rinnovo automatico = false il 1 ° settembre 2018. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Piani di sostituzione del piano 1 di Skype for business online

Con i nuovi piani, i clienti possono sfruttare le funzionalità e le funzionalità più recenti di Office 365. I dettagli relativi ai prezzi sono disponibili nell'elenco prezzi e nella matrice elenco offerte del centro per i partner. 

- Opzione 1: Office 365 Enterprise F1
- Opzione 2: Microsoft 365 Enterprise F1
- Opzione 3: altri piani di Office 365

|**Funzionalità**    |**Opzione 1**   |**Opzione 2**   |**Opzione 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Ottenere tutte le funzionalità incluse nel piano 1 di Skype for business online|Sì   |Sì   |Sì   |
|Messaggistica immediata e presenza |Sì   |Sì   |Sì   |
|Audio e video peer-to-peer su IP|Sì   |Sì   |Sì   
|Unisciti a riunioni come utente autenticato| Sì   |Sì   |Sì   |

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai nostri partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione delle sottoscrizioni da SKU che verranno arrestate. Per la migrazione dei clienti da SKU ritirati a quelli più recenti sono necessari i passaggi seguenti:

- Acquistare la nuova sottoscrizione
- Riassegna licenze utente correnti
- Annulla sottoscrizione precedente

### <a name="migrate-your-customers-to-new-plans"></a>Esegui la migrazione dei clienti ai nuovi piani

1. Per acquistare la nuova sottoscrizione, scegliere **Customers**dal **menu centro**per i partner, selezionare il cliente che si desidera spostare e quindi selezionare **Aggiungi sottoscrizioni**.

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Submit (Invia**). 

Il cliente deve avere ora sottoscrizioni sia precedenti che nuove, la sottoscrizione precedente del piano 1 di Skype for business online e la nuova sottoscrizione di destinazione, ad esempio l'opzione 1-Office 365 Enterprise F1.

3. Per riassegnare le licenze degli utenti del cliente, dal menu **centro** per i partner selezionare **clienti**, selezionare il cliente da trasferire, quindi selezionare **utenti e licenze**. Verrà visualizzata la pagina utenti e licenze del cliente.

4. Per riassegnare la licenza utente, selezionare l'utente da riassegnare, quindi selezionare **Gestisci licenze.**

5. Nella pagina **Gestisci licenze** deselezionare la casella di controllo licenza di Skype for business online piano 1 e selezionare un nuovo piano di servizio per la sottoscrizione a cui il cliente si sta muovendo.

6. Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma. Continuare lo stesso processo per gli altri utenti che necessitano di assegnazioni di licenze.

Dopo aver spostato la licenza utente nel nuovo servizio, è possibile annullare tranquillamente la sottoscrizione ritirata a livello di cliente.

7. Scegliere **clienti**dal menu **centro partner** . Selezionare il cliente di cui annullare la sottoscrizione.

8. Nella pagina Dettagli sottoscrizione impostare la sottoscrizione su **sospesa**.

9. Selezionare **Invia.**

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Il deprovisioning della sottoscrizione sospesa verrà effettuato automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.

