---
title: Leggere la fattura | Centro per i partner
description: "La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel dashboard del Centro per i partner."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 3035ba6f108c9676b1d555147aaa98da24603133
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="read-your-bill"></a>Leggere la fattura

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud Germania

La fattura è un riepilogo di tutti gli addebiti (per il programma, i prodotti e i clienti) per il periodo mensile corrente. È disponibile nel dashboard del Centro per i partner.

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
<td>Indirizzo a cui inviare la fattura. Per cambiare questo indirizzo, modifica il tuo profilo dell'account del Centro per i partner.</td>
</tr>
<tr class="odd">
<td>Addebiti periodici</td>
<td>Gli addebiti fissi mensili o annuali per le licenze in base all'uso acquistate, fatturati prima del servizio. Questo numero è la somma di tutti gli addebiti nella colonna &quot;Subtotal&quot; del file di riconciliazione in base alle licenze (colonna T).</td>
</tr>
<tr class="even">
<td>Costi di utilizzo</td>
<td>Utilizzo di Azure, inclusi le nuove applicazioni e i nuovi servizi abilitati e usati durante il periodo di fatturazione. Questo numero è la somma di tutti gli addebiti nella colonna &quot;PretaxCharges&quot; del file di riconciliazione in base all'uso (colonna Z).</td>
</tr>
<tr class="odd">
<td>Crediti e rettifiche</td>
<td>Crediti o rettifiche per modifiche apportate alle sottoscrizioni, ad esempio aumento o riduzione delle postazioni.</td>
</tr>
<tr class="even">
<td>Altri sconti</td>
<td>Ad esempio lo sconto che il cliente riceve sul prezzo normale della sottoscrizione. Lo sconto viene indicato come importo unico, non come prezzo per unità o licenza.</td>
</tr>
<tr class="odd">
<td>Imposte</td>
<td>Imposta totale per gli addebiti correnti come calcolata complessivamente nella sezione dei dettagli che inizia a pagina 2 della fattura. Questo numero è la somma di tutti gli addebiti che fanno riferimento a:
<ul>
<li>la colonna &quot;TaxAmount&quot; del file di riconciliazione in base all'uso (colonna AA) e</li>
<li>la colonna &quot;Tax&quot; del file in base alle licenze (colonna U).</li>
</ul></td>
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
<td>I partner CSP ricevono una fattura mensile.</td>
</tr>
<tr class="even">
<td>Data fattura</td>
<td>Data in cui ricevi la fattura.</td>
</tr>
<tr class="odd">
<td>Data scadenza pagamento</td>
<td>Data entro cui effettuare il pagamento.</td>
</tr>
<tr class="even">
<td>Ordine d'acquisto del cliente</td>
<td>Il numero del tuo ordine di acquisto.</td>
</tr>
<tr class="odd">
<td>Servizio clienti</td>
<td>Indirizzo del sito Web per accedere al servizio clienti.</td>
</tr>
<tr class="even">
<td>Destinatario del servizio</td>
<td>Indirizzo in cui viene usato il servizio. (Questo è l'indirizzo legale della società associato alla verifica della società e non può essere modificato.)</td>
</tr>
</tbody>
</table>

 

 

 



