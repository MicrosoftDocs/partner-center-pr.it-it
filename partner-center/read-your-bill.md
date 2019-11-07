---
title: Leggere la fattura | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel centro per i partner.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione abbonamenti, fatturazione, fatturazione nel centro per i partner, centri per i partner fatturazione, leggere la fattura, fattura, fattura del centro per i partner, fattura CSP, dove è la fattura?
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652177"
---
# <a name="read-your-bill"></a>Leggere la fattura

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government


Per la fattura, accedere al menu del centro per i **partner** , quindi selezionare **fatturazione** per visualizzare la cronologia e le tendenze di fatturazione, i collegamenti alla fattura e al file di riconciliazione e il pagamento più recente.

I partner del programma Cloud Solution Provider che hanno scelto la fatturazione mensile pagheranno Microsoft per gli abbonamenti dei clienti (sia in base a licenza che in base all'uso) in via posticipata, dopo 60 giorni.

> [!NOTE]  
> La fattura è un riepilogo di tutti gli addebiti, per il programma, i prodotti e i clienti, per il periodo di fatturazione corrente ed è disponibile entro due (2) giorni dalla data di fatturazione selezionata in ora UTC. Se, ad esempio, si dispone di una data di fatturazione del 12 settembre, il processo di generazione della fattura inizierà alle 12.00 UTC della tredicesima e completerà entro le 12.00 UTC del 14 °. Se la fattura non viene visualizzata entro 11:59PM UTC al 15, il Contratto di servizio e dovrebbe presentare una richiesta di servizio. 

Riceverai una fattura per gli addebiti basati sulla licenza (Office365) e basati sull'utilizzo (Azure) e una fattura separata per addebiti una tantum (istanze di macchina virtuale riservate di Azure).

Per i dettagli sugli addebiti, consulta i file di riconciliazione associati. I file di riconciliazione includono gli ID dei clienti e gli ID delle sottoscrizioni che userai per creare le fatture per i clienti. Per altre informazioni, vedi [Come usare i file di riconciliazione](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definizioni del file di fatturazione


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Campo</strong></td>
<td><strong>Descrizione</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>Numero ID fiscale federale.</td>
</tr>
<tr class="odd">
<td>Numero cliente</td>
<td>Codice del cliente.</td>
</tr>
<tr class="even">
<td>Indirizzo fatturazione</td>
<td>Indirizzo a cui inviare la fattura. Per modificare il nome o l'indirizzo della società, modificare il profilo di fatturazione del centro per i partner. </td>
</tr>
<tr class="odd">
<td>Addebiti in base alle licenze</td>
<td>Gli addebiti fissi mensili o annuali per le licenze basate sull'utilizzo acquistate, fatturati prima del servizio. Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</td>
</tr>
<tr class="even">
<td>Addebiti basati sull'utilizzo</td>
<td>Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il mese di fatturazione. Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</td>
</tr>
<tr class="odd">
<td>Sconti</td>
<td>Ad esempio lo sconto che il cliente riceve sul prezzo normale della sottoscrizione. Lo sconto viene indicato come importo unico, non come prezzo per unità o licenza.</td>
</tr>
<tr class="odd">
<td>Crediti</td>
<td>Crediti o rettifiche per modifiche apportate alle sottoscrizioni, ad esempio aumento o riduzione delle postazioni.</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>Totale al lordo delle imposte e crediti e addebiti netti.</td>
</tr>
<td>Imposta</td>
<td>Imposta totale per gli addebiti correnti calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti che fanno riferimento a:
<ul>
<li>la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</li>
<li>la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Altri crediti</td>
<td>Crediti netti.</td>
</tr>
<tr class="even">
<td>Costi attuali totali</td>
<td>L'importo dovuto nella valuta della fattura per il periodo fatturato, da pagare entro la data di scadenza.</td>
</tr>
<tr class="odd">
<td>Istruzioni per il pagamento</td>
<td>Descrive come pagare la fattura, in base all'area geografica. Includi sempre il numero di fattura quando effettui un pagamento.</td>
</tr>
<tr class="even">
<td>N. fattura</td>
<td>Numero della fattura.</td>
</tr>
<tr class="odd">
<td>Periodo di fatturazione</td>
<td>Il periodo mensile che precede la data della fattura. Si tratta del periodo di tempo durante il quale vengono utilizzati i servizi basati sull'utilizzo e i servizi basati su licenze vengono riconciliati per eventuali rettifiche di credito o modifiche al numero di licenze.</td>
</tr>
<tr class="even">
<td>Data fattura</td>
<td>Data di fatturazione o data di anniversario in cui la fattura viene generata ogni mese.</td>
</tr>
<tr class="odd">
<td>Condizioni di pagamento</td>
<td>Per gli acquisti una tantum sarà sempre 60 giorni.</td>
</tr>
<tr class="even">
<td>Data scadenza pagamento</td>
<td>Data entro cui effettuare il pagamento.</td>
</tr>
<tr class="odd">
<td>Ordine d'acquisto del cliente</td>
<td>Il numero del tuo ordine di acquisto.</td>
</tr>
<tr class="even">
<td>Servizio clienti</td>
<td>Indirizzo del sito Web per accedere al servizio clienti.</td>
</tr>
<tr class="odd">
<td>Destinatario del servizio</td>
<td>Indirizzo in cui viene usato il servizio. Si tratta dell'indirizzo aziendale legale associato al vagliatura aziendale.</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Elenco dettagliato dei costi una tantum

|**Campo** |**Definizione**|
|:----------------|:-----------------------------|
|Data |Data di acquisto. |
|Descrizione |Nome del prodotto. |
|Quantità |Numero di prodotti (prenotazioni, ad esempio) acquistati. |
|Prezzo unitario |Prezzo per prodotto (prenotazione, ad esempio). |
|Sconti |Eventuali sconti applicabili. |
|Importo pre-imposta |Totale parziale degli acquisti prima delle imposte. |
|Imposta sulle vendite |Importo dell'imposta. |
|Totale |Totale da pagare. |
 



