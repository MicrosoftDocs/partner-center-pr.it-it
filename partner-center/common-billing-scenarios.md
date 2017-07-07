---
title: Scenari di fatturazione comuni | Centro per i partner
description: "Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 92805672975e319b53c2cd89063442df2feb1267
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/01/2017
---
# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di licenze per una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## <a name="in-this-section"></a>Contenuto della sezione


-   [Fatturazione in base all'uso](#usagebased)

-   [Fatturazione in base alle licenze](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione in base all'uso


Vengono fatturati solo i servizi usati nel periodo di fatturazione precedente. Nella fattura comparirà qualsiasi applicazione o servizio di Azure abilitato e usato durante il periodo di fatturazione.

-   Le tariffe per i servizi a consumo possono variare durante il ciclo di fatturazione.
    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni
    -   Le diminuzioni di prezzo sono riportate il giorno in cui vengono rese effettive.
    -   Le sottoscrizioni esistenti vengono fatturate in base alle tariffe in vigore all'inizio del ciclo di fatturazione.
    -   Le nuove sottoscrizioni (quelle create durante il ciclo di fatturazione) vengono fatturate in base alle tariffe in vigore quando sono state aggiunte.
-   Se annulli una sottoscrizione durante il primo ciclo di fatturazione, i costi di utilizzo saranno indicati nel file di riconciliazione per il periodo in cui la sottoscrizione era attiva.

## <a href="" id="licensebased"></a>Fatturazione in base alle licenze

Per i mesi senza modifiche alle sottoscrizioni in base alle licenze, nella fattura vedrai una sola voce per ogni sottoscrizione. Corrisponde all'anticipo per il mese successivo.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Scenario</td>
<td>Descrizione</td>
<td>Esempio</td>
</tr>
<tr class="even">
<td>Nuova sottoscrizione aggiunta</td>
<td><p>Il periodo tra la data di inizio della sottoscrizione e la prima data di fatturazione è SENZA COSTI AGGIUNTIVI.</p>
<p>Il file di riconciliazione conterrà una sola voce:</p>
<ul>
<li>addebito dell'anticipo per il mese successivo</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nuova sottoscrizione con annullamento prima della scadenza di fatturazione</td>
<td>Non verrà effettuato alcun addebito sull'account. La sottoscrizione non comparirà nel file di riconciliazione. Questa opzione è utile se desideri eseguire test senza sostenere le spese della sottoscrizione.</td>
<td></td>
</tr>
<tr class="even">
<td>Nuova sottoscrizione con rettifiche della quantità di licenze durante il periodo gratuito</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>modifiche alla quantità di licenze, con prezzo unitario 0 (per le modifiche di licenze apportate durante il periodo gratuito non vengono effettuati addebiti).</li>
<li>addebito dell'anticipo per il mese successivo, in base alla nuova quantità.</li>
</ul></td>
<td>Uso ripartito:
<ul>
<li>Dal 3 giugno al 7 giugno per 10 licenze = addebito ZERO</li>
<li>Dall'8 giugno all'11 giugno per 20 licenze = addebito ZERO</li>
<li>Dal 12 giugno al 14 giugno per 15 licenze = addebito ZERO</li>
</ul>
<p>Scadenza di fatturazione: anticipo per il periodo mensile completo dal 15 giugno al 14 luglio per 15 licenze. Supponendo che l'addebito mensile per la sottoscrizione sia di 10 USD, l'addebito sarebbe 10 USD x 15 licenze = 150 USD.</p></td>
</tr>
<tr class="odd">
<td>Sottoscrizioni esistenti: aumento o riduzione della quantità di licenze</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>lo storno dell'anticipo</li>
<li>l'addebito per l'uso ripartito</li>
<li>l'addebito dell'anticipo per il mese successivo</li>
</ul></td>
<td><p>Uso ripartito:</p>
<ul>
<li>Dal 15 luglio al 19 luglio per 15 licenze = 26,61 USD</li>
<li>Dal 20 luglio al 30 luglio per 12 licenze = 46,84 USD</li>
<li>Dal 31 luglio al 9 agosto per 18 licenze = 63,87 USD</li>
<li>Dal 10 agosto al 14 agosto per 10 licenze = 17,74 USD</li>
</ul>
Storno dell'anticipo per il periodo mensile completo dal 15 luglio al 14 agosto = 165 USD.
<p>Scadenza di fatturazione: anticipo per il periodo mensile completo dal 15 agosto al 14 settembre per 10 licenze = 110 USD.</p></td>
</tr>
<tr class="even">
<td>Annullamento senza modifiche precedenti delle licenze</td>
<td><p>Il file di riconciliazione conterrà una sola voce:</p>
<ul>
<li>Un credito per i giorni inutilizzati, poiché l'intero periodo è stato addebitato in anticipo nell'ultima distinta di fatturazione. Viene calcolato in base alla data di fine della sottoscrizione.</li>
</ul></td>
<td>Anticipo fatturato in precedenza: dal 15 agosto al 14 settembre per 10 licenze = 100 USD.
<p>Parte usata dell'anticipo dal 15 agosto al 24 agosto.</p>
<p>Credito per i giorni inutilizzati: dal 25 agosto al 14 settembre per 10 licenze = -74,51 USD.</p></td>
</tr>
<tr class="odd">
<td>Annullamento con modifiche precedenti delle licenze</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>lo storno dell'anticipo</li>
<li>l'addebito per l'uso ripartito</li>
<li>un credito per eventuali giorni inutilizzati</li>
</ul></td>
<td>Anticipo fatturato in precedenza: dal 15 agosto al 14 settembre per 10 licenze = 100 USD.
<p>Uso ripartito:</p>
<ul>
<li>Dal 15 agosto al 24 agosto per 10 licenze</li>
<li>Dal 25 agosto al 14 settembre per 5 licenze</li>
</ul>
<p>Credito per i giorni inutilizzati: dall'1 settembre al 14 settembre per 5 licenze.</p>
<p>Storno dell'anticipo per il periodo mensile completo dal 15 agosto al 14 settembre = -100 USD.</p></td>
</tr>
</tbody>
</table>




 



