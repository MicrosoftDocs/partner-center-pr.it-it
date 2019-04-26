---
title: Migrare le sottoscrizioni di Skype for Business online piano 1 verso versioni più nuove di Office 365 | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
Description: Clienti di transizione con Skype in scadenza per le sottoscrizioni aziendali Online piano 1 di un'opzione supportata dello SKU. È consigliabile spostare i clienti per i nuovi abbonamenti prima data di fine annuali della sottoscrizione.
author: LauraBrenner
ms.author: labrenne
keywords: Piani di Skype for Business, ritiro di Skype, Office 365
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e71e6b05b5ea489b2b6b486f388f5c575dfd02c5
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133918"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrare le sottoscrizioni di Skype for Business online piano 1 verso versioni più nuove di Office 365

**Si applica a**

- Centro per i partner

Skype for Business online piano 1 verrà ritirato a decorrere dal 1° agosto 2018. Dopo tale data i clienti non potranno più acquistare nuove sottoscrizioni di Skype for Business piano 1 e le sottoscrizioni esistenti non verranno rinnovate automaticamente quando scadranno né sarà possibile rinnovarle. Nella pagina dei dettagli della sottoscrizione lo stato della sottoscrizione di Skype for Business online piano 1 è passato da "Rinnovo automatico in [data]" a "Data di scadenza [data]".  

Per garantire la continuità, è opportuno trasferire i clienti con sottoscrizioni di Skype for Business online piano 1 in scadenza a una opzione SKU supportata, indicata di seguito. Si consiglia di far passare i clienti ai nuovi abbonamenti prima della data di scadenza annuale dell'abbonamento, al fine di evitare eventuali interruzioni del servizio. 

>[!NOTE]
>Vengono ritirate sia la SKU commerciale che quella per enti pubblici di Skype for Business online piano 1.

Se usi l'API (CREST o Centro per i partner), puoi trovare le sottoscrizioni in scadenza valutando la data di scadenza della sottoscrizione insieme alla proprietà rinnovo automatico = False. Le sottoscrizioni di Skype for Business online piano 1 verranno impostate su rinnovo automatico=False il 1° settembre 2018. È possibile trasferire i clienti a un nuovo piano in qualsiasi momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Piani per la sostituzione di Skype for Business online (piano 1)

Con i nuovi piani i clienti possono sfruttare le funzioni e le funzionalità più recenti in Office 365. I dettagli sui prezzi sono disponibili nel listino prezzi e nella matrice dell'elenco di offerte nel Centro per i partner. 

- Opzione 1: Office 365 Enterprise F1
- Opzione 2: Microsoft 365 Enterprise F1
- Opzione 3: Altri piani di Office 365

|**Funzionalità**    |**Opzione 1**   |**Opzione 2**   |**Opzione 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Ottenere tutte le funzionalità incluse in Skype for Business online piano 1|Yes   |Yes   |Yes   |
|Messaggistica immediata e presenza |Yes   |Yes   |Yes   |
|Audio peer-to-peer e Video over IP|Yes   |Yes   |Yes   
|Partecipare alle riunioni come utente autenticato| Yes   |Yes   |Yes   |

## <a name="transition-customers-to-new-product-plans"></a>Transizione dei clienti ai nuovi piani per i prodotti

Microsoft offre continuamente nuovi prodotti e servizi ai suoi partner. In questi casi, potrebbe essere necessario aggiornare i clienti ai nuovi servizi o eseguire la migrazione dei loro abbonamenti da SKU destinati a essere ritirati. La migrazione dei clienti da SKU ritirati a quelli più recenti richiede la procedura seguente:

- Acquistare la nuova sottoscrizione
- Riassegnare le licenze utente correnti
- Annullare la sottoscrizione precedente

### <a name="migrate-your-customers-to-new-plans"></a>Eseguire la migrazione dei clienti verso nuovi piani

1. Per acquistare la nuova sottoscrizione, dal **menu Centro per i Partner**, selezionare **clienti**, seleziona il cliente si desidera spostare e quindi selezionare **aggiungere sottoscrizioni**.

2. Seleziona l'abbonamento che vuoi acquistare dal catalogo (in questo caso, una delle opzioni precedenti), immetti il numero di licenze e quindi seleziona **Invia**. 

Il cliente dovrebbe disporre ora di sottoscrizioni sia nuove che precedenti, della precedente sottoscrizione Skype for Business online piano 1 e della nuova sottoscrizione "di destinazione", ad esempio Opzione 1: Office 365 Enterprise F1.

3. Per riassegnare le licenze degli utenti del cliente, dal **Centro per i Partner** dal menu **clienti**, seleziona il cliente si stanno spostando e quindi selezionare **utenti e licenze** . Viene aperta la pagina Utenti e licenze del cliente.

4. Per riassegnare la licenza utente, seleziona l'utente da riassegnare e quindi seleziona **Gestisci licenze**.

5. Nella pagina **Gestisci licenze** deseleziona la casella di controllo della licenza per Skype for Business online piano 1 e seleziona un nuovo piano di servizio per la sottoscrizione alla quale sta passando il cliente.

6. Seleziona **Invia**. Le nuove assegnazioni di licenza vengono visualizzate in una pagina di conferma. Continua nello stesso modo per altri utenti che necessitano le cessioni di licenza.

Dopo aver spostato le licenze utente al nuovo servizio, puoi tranquillamente annullare la sottoscrizione ritirata al livello del cliente.

7. Dal **Centro per i Partner** dal menu **clienti**. Seleziona il cliente di cui stai annullando la sottoscrizione.

8. Nella pagina dei dettagli della sottoscrizione imposta lo stato su **Sospeso**.

9. Seleziona **Invia**.

La sottoscrizione precedente viene sospesa e la nuova sottoscrizione diventa attiva. Per la sottoscrizione sospesa verrà eseguito automaticamente l'annullamento del provisioning dopo 120 giorni. Il cliente non dovrà sostenere alcun costo aggiuntivo per la sottoscrizione precedente.

