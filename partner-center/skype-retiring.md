---
title: Eseguire la migrazione di alcune sottoscrizioni di Skype for Business
description: Informazioni su come e quando eseguire la migrazione di determinati clienti con sottoscrizioni skype for business online in scadenza piano 1 alle nuove versioni di Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854826"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Eseguire la migrazione di sottoscrizioni di Skype for Business Online piano 1 alla versione più recente di Office 365

**Ruoli appropriati:** Agente di vendita

Skype for Business Online Piano 1 verrà ritirato a partire dal 1° agosto 2018. Dopo tale data i clienti non potranno più acquistare nuove sottoscrizioni di Skype for Business Piano 1 e le sottoscrizioni esistenti non verranno rinnovate automaticamente alla scadenza e non offriranno un'opzione di rinnovo. Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione di Skype for Business Online Piano 1 è stato modificato in "Scadenza [data]" da "Rinnovo automatico il [data]".  

Per garantire la continuità per i clienti, è consigliabile eseguire la transizione dei clienti con sottoscrizioni skype for business online in scadenza piano 1 a un'opzione SKU supportata, elencata di seguito. È consigliabile spostare i clienti in nuove sottoscrizioni prima della data di fine annuale della sottoscrizione per evitare interruzioni del servizio per i clienti. 

>[!NOTE]
>Sia gli SKU commerciali che gli SKU per enti pubblici di Skype for Business Online Piano 1 sono stati ritirati.

Se si usa l'API (EITHER o Partner Center), trovare le sottoscrizioni in scadenza valutando la data di fine della sottoscrizione insieme alla proprietà auto renew = False. Le sottoscrizioni di Skype for Business Online Piano 1 verranno impostate su Rinnovo automatico=False il 1° settembre 2018. È possibile spostare i clienti in un nuovo piano in qualsiasi momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Piani di sostituzione di Skype for Business Online Piano 1

Con i nuovi piani, i clienti possono sfruttare le funzionalità più nuove di Office 365. I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice del listino Partner Center. 

- Opzione 1: Office 365 Enterprise F1
- Opzione 2: Microsoft 365 Enterprise F1
- Opzione 3: Altri piani di Office 365

|**Funzionalità**    |**Opzione 1**   |**Opzione 2**   |**Opzione 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Ottenere tutte le funzionalità incluse in Skype for Business Online Piano 1|Sì   |Sì   |Sì   |
|Messaggistica istantanea e presenza |Sì   |Sì   |Sì   |
|Audio e video peer-to-peer su IP|Sì   |Sì   |Sì   
|Partecipare alle riunioni come utente autenticato| Sì   |Sì   |Sì   |

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai partner. In questi casi, potrebbe essere necessario aggiornare i clienti a nuovi servizi o eseguire la migrazione delle sottoscrizioni dagli SKU che verranno arrestati. La migrazione dei clienti da SKU ritirati a SKU più recenti richiede i passaggi seguenti:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

### <a name="migrate-your-customers-to-new-plans"></a>Eseguire la migrazione dei clienti a nuovi piani

1. Per acquistare la nuova sottoscrizione, **scegliere** Clienti dal menu **Partner Center,** selezionare il cliente da spostare e quindi aggiungi **sottoscrizioni.**

2. Selezionare la sottoscrizione che si vuole acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immettere il numero di licenze e quindi selezionare **Invia**. 

Il cliente deve ora avere sottoscrizioni sia nuove che vecchie, la sottoscrizione Skype for Business Online piano 1 precedente e la nuova sottoscrizione di "destinazione", ad esempio Opzione 1 - Office 365 Enterprise F1.

3. Per riassegnare le licenze degli utenti del cliente, scegliere **Clienti** dal menu **Partner Center,** selezionare il cliente che si sta spostando e quindi selezionare Utenti **e licenze**. Verrà visualizzata la pagina Utenti e licenze del cliente.

4. Per riassegnare la licenza utente, selezionare l'utente da riassegnare e quindi **selezionare Gestisci licenze.**

5. Nella pagina **Gestisci licenze** deselezionare la casella di controllo Licenza Skype for Business Online Piano 1 e selezionare un nuovo piano di servizio per la sottoscrizione a cui si sta spostando il cliente.

6. Selezionare **Submit** (Invia). Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma. Continuare lo stesso processo per altri utenti che necessitano di assegnazioni di licenza.

Dopo aver spostata la licenza utente nel nuovo servizio, è possibile annullare la sottoscrizione ritirata a livello di cliente.

7. Dal menu **Partner Center** selezionare **Clienti**. Selezionare il cliente di cui si sta annullando la sottoscrizione.

8. Nella pagina dei dettagli della sottoscrizione impostare la sottoscrizione su **Sospeso.**

9. Selezionare **Invia.**

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Il de provisioning della sottoscrizione sospesa verrà eseguito automaticamente dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.

## <a name="next-steps"></a>Passaggi successivi

- [Advisor: creare e inviare un invito alla versione di valutazione per i client a provare Office 365](advisors-create-a-trial-invitation.md)
- [Advisor: creare la base client con inviti alla versione di valutazione di Office 365 e offerte di acquisto](advisors-build-your-business.md)
- [Advisor: creare un'offerta di acquisto](advisor-create-a-purchase-offer.md)
