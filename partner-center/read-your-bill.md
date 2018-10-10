---
title: Leggere la fattura | Centro per i partner
description: La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel centro per i Partner.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: fatturazione abbonamenti, fatturazione, fatturazione nel centro per i partner, centri per i partner fatturazione, leggere la fattura, fattura, fattura del centro per i partner, fattura CSP, dove è la fattura?
ms.localizationpriority: medium
ms.openlocfilehash: 81262c11ab402dcd1748f9f8fde5cdeceac0f4f9
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489407"
---
# <a name="read-your-bill"></a>Leggere la fattura

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Per la fattura, Vai al menu **Centro per i Partner** e quindi seleziona **la fatturazione** per visualizzare la cronologia di fatturazione e tendenze, i collegamenti per la fattura e il file di riconciliazione e il pagamento più recente.

I partner del programma Cloud Solution Provider che hanno scelto la fatturazione mensile pagheranno Microsoft per gli abbonamenti dei clienti (sia in base a licenza che in base all'uso) in via posticipata, dopo 60 giorni.

> [!NOTE]  
> La fattura è un riepilogo di tutti gli addebiti relativi a programma, prodotti e clienti per il periodo di fatturazione corrente ed è disponibile entro quattro (4) giorni dalla data di fatturazione selezionata.

Riceverai una fattura per basate su licenza (Office 365) e gli addebiti (Azure) basati sull'utilizzo e una fattura separata per una tantum (istanze riservate di Azure della macchina virtuale) addebiti.

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
<td>Indirizzo a cui inviare la fattura. Per modificare questo indirizzo, vai a Impostazioni account > Profilo di fatturazione partner. </td>
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
<td>Totale al lordo imposte e addebiti esclusiva fiscali e crediti.</td>
</tr>
<td>Tax</td>
<td>Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti che fanno riferimento a:
<ul>
<li>la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</li>
<li>la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Altri crediti</td>
<td>Crediti fiscali esclusive.</td>
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
<td>I partner CSP ricevono una fattura mensile o annuale.</td>
</tr>
<tr class="even">
<td>Data fattura</td>
<td>Data in cui ricevi la fattura.</td>
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
<td>Indirizzo in cui viene usato il servizio. Questo è l'indirizzo legale della società associato alla verifica della società e non può essere modificato.</td>
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
 



