---
title: Leggere la fattura | Centro per i partner
ms.topic: article
ms.date: 10/29/2018
description: La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel centro per i Partner.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: fatturazione abbonamenti, fatturazione, fatturazione nel centro per i partner, centri per i partner fatturazione, leggere la fattura, fattura, fattura del centro per i partner, fattura CSP, dove è la fattura?
ms.localizationpriority: medium
ms.openlocfilehash: aec344eb7e4ed6e0a4d5e7e506c9bcf195654293
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584544"
---
# <a name="read-your-bill"></a>Leggere la fattura

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud for US Government


Per la fattura, visitare il **Centro per i Partner** menu e quindi selezionare **fatturazione** per visualizzare la cronologia di fatturazione e le tendenze, collegamenti a file di riconciliazione e fatturazione e il pagamento più recente.

I partner del programma Cloud Solution Provider che hanno scelto la fatturazione mensile pagheranno Microsoft per gli abbonamenti dei clienti (sia in base a licenza che in base all'uso) in via posticipata, dopo 60 giorni.

> [!NOTE]  
> La fattura è riportato un riepilogo di tutti gli addebiti, attraverso il programma, i prodotti e clienti, per il periodo di fatturazione corrente ed è disponibile entro due (2) della data di fatturazione selezionata in formato UTC. Ad esempio, se hai il 12 settembre data di fatturazione, il processo di generazione della fattura verrà iniziano alle 12:00 AM UTC nel 13 e completare da 12:00 AM UTC su 14. Se non è possibile visualizzare la fattura da 11 alle 23.59.59 UTC il giorno 15, vengono all'esterno del contratto di servizio, che deve inviare una richiesta di servizio. 

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
<td>ID fiscale federale.</td>
</tr>
<tr class="odd">
<td>Numero cliente</td>
<td>Codice del cliente.</td>
</tr>
<tr class="even">
<td>Indirizzo fatturazione</td>
<td>Indirizzo a cui inviare la fattura. Per modificare il nome della società o l'indirizzo, modificare il centro per i Partner del profilo di fatturazione. </td>
</tr>
<tr class="odd">
<td>Addebiti in base alle licenze</td>
<td>Gli addebiti fissi mensili o annuali per le licenze in base all'uso acquistate, fatturati prima del servizio. Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</td>
</tr>
<tr class="even">
<td>Addebiti basati sull'utilizzo</td>
<td>Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il periodo di fatturazione. Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</td>
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
<td>Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti che fanno riferimento a:
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
<td>Il periodo mensile conducono alla data di fatturazione. Questo è il periodo durante il quale vengono utilizzati i servizi basati sull'utilizzo e servizi basati su licenza vengono riconciliati le regolazioni di carta di credito o la modifica di nel conteggio delle licenze.</td>
</tr>
<tr class="even">
<td>Data fattura</td>
<td>La data di fatturazione o data di ricorrenza in cui la fattura viene generata ogni mese.</td>
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
<td>Indirizzo in cui viene usato il servizio. (Questo è l'indirizzo ragione sociale della società associato all'azienda consultazione).</td>
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
 



