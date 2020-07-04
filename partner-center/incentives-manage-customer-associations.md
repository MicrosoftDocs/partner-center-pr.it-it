---
title: Gestire le associazioni del cliente
description: Informazioni sui processi e le sequenze temporali importanti per la gestione delle associazioni clienti di CPOR (partner di record).
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.topic: article
author: kim-davis
ms.author: kimnich
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: 97871089ad7614be47a65bb41dfb8dc4f871b54b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949505"
---
# <a name="manage-customer-associations"></a>Gestire le associazioni del cliente

Si applica a:

- Centro per i partner

La piattaforma CPOR (partner of record) rivendicata viene usata per i partner per associarsi ai clienti finali per i quali influiscono sull'uso o sull'acquisto di prodotti Microsoft. Attualmente la piattaforma CPOR supporta i prodotti Business Applications e Microsoft 365. I partner usano questo metodo di associazione per ottenere informazioni sulle prestazioni dei clienti, ricevere incentivi tramite i programmi OSU e OSA e ottenere l'associazione di ricavi come influencer aziendale.  

Ruoli appropriati:

- Amministratore fatturazione
- Amministratore globale
- Amministratore degli incentivi

## <a name="how-your-cpor-association-claim-relates-to-incentives"></a>Relazione tra l'attestazione di associazione CPOR e gli incentivi

Se è stata creata un'attestazione di associazione CPOR ed è stata approvata, l'utente è ora associato al cliente. Non significa che l'attestazione è stata approvata per incentivare guadagni o pagamenti. La guida del programma incentive descrive i requisiti di idoneità per gli incentivi da pagare in base alle attestazioni approvate.

È possibile trovare le guide ai programmi per incentivare il [Microsoft Partner Network](https://aka.ms/partnerincentives).

Se l'attestazione di associazione CPOR è approvata e idonea per gli incentivi, è possibile convalidare la sottoscrizione o l'ID tenant nei report guadagni e pagamenti. 

## <a name="cpor-association-claims-timeline"></a>Sequenza temporale delle attestazioni di associazione CPOR

- Inviato: lo stato verrà inviato per un massimo di cinque giorni lavorativi fino a quando Microsoft non avvia il processo di approvazione.
- In fase di Revisione: Microsoft ha cinque giorni lavorativi per prendere una decisione in base alla prova dell'esecuzione fornita.
- Azione del partner necessaria: se un revisore invia commenti e una richiesta di informazioni aggiuntive, è necessario rispondere a cinque giorni lavorativi. È necessario prendere una decisione sull'attestazione dell'associazione CPOR entro 10 giorni, in base al contratto di servizi del revisore, oltre alla quantità di tempo necessaria per fornire ai revisori PoE informazioni aggiuntive.
- Approvato: l'attestazione di associazione CPOR è stata approvata. Una volta approvata l'associazione, viene inviata una notifica al cliente che offre la possibilità di negare l'associazione. Il cliente avrà quindi sette giorni per rifiutare esplicitamente. Una volta trascorso il periodo di consenso, l'attestazione verrà inviata per valutare l'idoneità per i programmi incentive.

## <a name="view-the-status-of-your-cpor-association-claim"></a>Visualizzare lo stato dell'attestazione di associazione CPOR

È possibile controllare lo stato dell'attestazione dell'associazione di CPOR in qualsiasi momento usando il [Dashboard associazioni clienti](https://partner.microsoft.com/dashboard/incentives/claims/associations).

Ecco gli Stati e i relativi significati:

| Stato attestazione | Viene visualizzato quando |
| ------ | ----------- | 
|  In fase di modifica  | L'attestazione di associazione CPOR è stata creata. Rimane in questo stato fino a quando non si carica il documento di prova dell'esecuzione e si invia l'attestazione per l'approvazione.   |
|  Inviato  | Il partner ha inviato correttamente la richiesta di associazione CPOR, ma Microsoft non ha ancora avviato il processo di revisione.   |
|  In fase di revisione  | Microsoft ha iniziato a convalidare la documentazione di PoE. Per ulteriori informazioni, è possibile contattare l'utente. Il contratto di lavoro per il processo di revisione è di cinque giorni lavorativi.  |
|  Rifiutato  | Il PoE è insufficiente o non è stato risposto entro cinque giorni lavorativi per le linee guida di revisione di PoE e l'attestazione è stata negata.   |
|  Approved  | L'attestazione è stata approvata. Dopo l'approvazione di Microsoft, il cliente ha avuto la possibilità di negare l'associazione. Il cliente ha sette giorni per rifiutare l'approvazione a Microsoft. Anche se l'attestazione verrà visualizzata come approvata, verrà inviata per la valutazione degli incentivi solo dopo che il periodo di consenso è scaduto.   |
|  Azione partner obbligatoria  | Microsoft ha esaminato la richiesta di associazione CPOR PoE e necessita di altre informazioni relative al PoE per i prodotti e i carichi di lavoro richiesti. Ci sono cinque giorni lavorativi per fornire le informazioni richieste e inviare nuovamente l'attestazione o verrà rifiutato. Di seguito sono riportati i possibili motivi per cui potrebbero essere necessarie informazioni aggiuntive:

- Mancano tutti i PoE: i PoE sono mancanti a causa del caricamento di un file non corretto o non pertinente alla richiesta di associazione CPOR

- Firma del cliente per il riconoscimento dei clienti mancante non presente in PoE

- Date mancanti oppure obsolete: le date nel PoE sono mancanti oppure obsolete rispetto all'attestazione

- Soluzione o servizio del partner mancante: la descrizione delle operazioni completate non è sufficiente o non è inclusa nel documento

- Prodotti mancanti: il PoE non include il prodotto o il carico di lavoro richiesto 

## <a name="dispute-the-status-of-a-cpor-association-claim"></a>Disputare lo stato di un'attestazione di associazione CPOR

Se l'attestazione di associazione CPOR viene rifiutata, si avranno 30 giorni per disputare il rifiuto. Il messaggio di posta elettronica ricevuto per informare l'utente del rifiuto indica anche dove è possibile visualizzare il motivo del rifiuto e come contestarlo.  

Se sono trascorsi 30 giorni e si vuole comunque disputare un'attestazione rifiutata, è necessario inviare una nuova associazione con la prova di esecuzione (PoE) aggiornata. 

### <a name="to-dispute-a-rejected-claim"></a>Per disputare un'attestazione rifiutata

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Aprire l'attestazione che si desidera disputare.
3. Nella pagina attestazione selezionare **contenzioso**.
4. Immettere una giustificazione aziendale e/o un PoE aggiornato per spiegare il motivo per cui deve essere ripreso in considerazione il rifiuto.
5. Al termine dell'aggiunta delle informazioni, selezionare **contenzioso**. I revisori dovranno contattare l'utente con i risultati entro 5 giorni lavorativi.

## <a name="reasons-a-cpor-association-claim-is-rejected"></a>Motivi per cui un'attestazione di associazione CPOR viene rifiutata

Esistono tre motivi principali per cui un'attestazione di associazione CPOR viene rifiutata.

**Richiesta partner:** I partner possono richiedere che l'associazione sia stata rifiutata. Questa operazione viene usata principalmente quando il partner ha creato un'attestazione di associazione CPOR per errore usando un MPN errato, ha scelto un'attività non corretta (ad esempio... È stata scelta l'associazione di ricavi anziché le vendite preliminari oppure non è più possibile utilizzare il cliente.

**Rifiuto del cliente:** Una volta che l'attestazione di associazione CPOR è stata eseguita correttamente, il processo di approvazione di PoE è stato modificato in approved, mentre al cliente viene offerta la possibilità di negare il consenso dell'associazione. Se il cliente nega il consenso, l'associazione verrà rifiutata.

**Prova di esecuzione insufficiente:** La prova di esecuzione è obbligatoria per ogni associazione di CPOR. Una volta inviata l'attestazione di associazione CPOR, i revisori di Microsoft richiederanno fino a 5 giorni per esaminare il PoE e richiedere eventuali informazioni aggiuntive necessarie usando la sezione dei commenti nell'attestazione. Se le informazioni non sono sufficienti, l'attestazione dell'associazione CPOR verrà rifiutata.

Altri possibili motivi per il rifiuto:

- Manca il consenso del cliente su PoE
- Prodotti mancanti
- Nessuna risposta partner
- PoE non disponibile 

## <a name="edit-your-cpor-association-claim"></a>Modificare l'attestazione di associazione CPOR

L'utente può modificare campi specifici nella richiesta di associazione CPOR. È possibile che venga richiesto di rimuovere uno o più prodotti o carichi di lavoro se i revisori indicano che il PoE inviato è insufficiente. Per apportare modifiche, la richiesta di associazione CPOR deve avere lo stato Inviata o Richiesta azione del partner.

Campi che è possibile modificare:

- MPN
- Products
- Informazioni di contatto del clienti e del partner
- Aggiungere altre informazioni al PoE e commenti

## <a name="customer-consent-notification"></a>Notifica di consenso del cliente

Una volta approvata l'attestazione di associazione CPOR, viene inviata una notifica al cliente che offre la possibilità di negare l'associazione. Il cliente avrà quindi 7 giorni per rifiutare esplicitamente. Lo stato di questo periodo viene visualizzato come approvato. Se il cliente nega il consenso, l'associazione verrà rifiutata. Una volta trascorso il periodo di consenso e il cliente non ha negato il consenso, l'attestazione verrà inviata per valutare l'idoneità per i programmi incentive.

## <a name="how-to-communicate-with-poe-reviewers"></a>Come comunicare con i revisori PoE

Dopo che i revisori hanno attraversato il PoE, possono determinare che sono necessarie informazioni aggiuntive. In tal caso, verranno contattati tramite la sezione relativa ai commenti dell'attestazione. È anche possibile rispondere a questi elementi nella sezione dei commenti.

## <a name="view-claim-history"></a>Visualizza cronologia attestazioni

Nell'attestazione di associazione CPOR, sul lato superiore destro, è disponibile un pulsante **cronologia** che consente di visualizzare tutte le modifiche, i commenti e le azioni intraprese dall'attestazione da un partner e da una prospettiva revisore.
