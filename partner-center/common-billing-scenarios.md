---
title: Scenari di fatturazione comuni | Centro per i partner
description: "Questo argomento descrive ciò che compare sulla fattura dopo l&quot;aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l&quot;annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all&quot;uso."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 877f2d0e773fc7a42ddb8f62fa320be94b5921a8

---

# Scenari di fatturazione comuni


Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l'annullamento di una sottoscrizione. Le sottoscrizioni in base alle licenze vengono gestite diversamente rispetto a quelle in base all'uso.

## Contenuto della sezione


-   [Fatturazione in base all'uso](#usagebased)

-   [Fatturazione in base alle licenze](#licensebased)

## <a href="" id="usagebased"></a>Fatturazione in base all'uso


Vengono fatturati solo i servizi usati nel periodo di fatturazione precedente. Nella fattura comparirà qualsiasi applicazione o servizio di Azure abilitato e usato durante il periodo di fatturazione.

-   La prima fattura include il periodo iniziale dalla data di inizio della sottoscrizione alla prima data di fatturazione.
-   Le tariffe per i servizi a consumo possono variare all'interno del ciclo di fatturazione.
    -   Aumenti di prezzo: è previsto un preavviso di 30 giorni
    -   Riduzioni del prezzo: attive dal giorno della modifica.
    -   Per le sottoscrizioni esistenti verranno usate le tariffe in vigore all'inizio del ciclo di fatturazione.
    -   Le nuove sottoscrizioni (create all'interno del ciclo di fatturazione) usano le tariffe in vigore alla data di creazione.
-   Se annulli una sottoscrizione prima della prima scadenza per la fatturazione oppure a metà di un ciclo di fatturazione, i costi di utilizzo saranno indicati nel file di riconciliazione per il periodo in cui la sottoscrizione era attiva.

## <a href="" id="licensebased"></a>Fatturazione in base alle licenze


Per i mesi senza modifiche alle sottoscrizioni in base alle licenze, nel file di riconciliazione e nella fattura vedrai una sola voce per ogni sottoscrizione, corrispondente all'anticipo per il mese successivo.

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
<td>Nuova sottoscrizione</td>
<td><p>Il periodo tra la data di inizio della sottoscrizione e la prima data di fatturazione è GRATIS.</p>
<p>Il file di riconciliazione conterrà una sola voce:</p>
<ul>
<li>l'addebito dell'anticipo per il mese successivo</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nuova sottoscrizione con annullamento prima della scadenza di fatturazione</td>
<td>Non verrà effettuato alcun addebito sull'account. La sottoscrizione non comparirà nel file di riconciliazione. Questa opzione è utile se vuoi eseguire test senza sostenere le spese della sottoscrizione.</td>
<td></td>
</tr>
<tr class="even">
<td>Nuova sottoscrizione con rettifiche della quantità di licenze durante il periodo gratuito</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>modifiche alla quantità di licenze, con prezzo unitario 0 (per le modifiche di postazioni apportate durante il periodo gratuito non vengono effettuati addebiti).</li>
<li>addebito dell'anticipo per il mese successivo, in base alla nuova quantità.</li>
</ul></td>
<td>Uso ripartito:
<ul>
<li>Dal 3 giugno al 7 giugno per 10 postazioni = addebito ZERO</li>
<li>Dall'8 giugno all'11 giugno per 20 postazioni = addebito ZERO</li>
<li>Dal 12 giugno al 14 giugno per 15 postazioni = addebito ZERO</li>
</ul>
<p>Scadenza di fatturazione: anticipo per il periodo mensile completo dal 15 giugno al 14 luglio per 15 postazioni. Supponendo che l'addebito mensile per la sottoscrizione sia di 10 euro, l'addebito sarebbe 10 euro x 15 postazioni = 150 euro.</p></td>
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
<li>Dal 15 luglio al 19 luglio per 15 postazioni = 26,61 euro</li>
<li>Dal 20 luglio al 30 luglio per 12 postazioni = 46,84 euro</li>
<li>Dal 31 luglio al 9 agosto per 18 postazioni = 63,87 euro</li>
<li>Dal 10 agosto al 14 agosto per 10 postazioni = 17,74 euro</li>
</ul>
Storno dell'anticipo per il periodo mensile completo dal 15 luglio al 14 agosto = 165 euro.
<p>Scadenza di fatturazione: anticipo per il periodo mensile completo dal 15 agosto al 14 settembre per 10 postazioni = 110 euro.</p></td>
</tr>
<tr class="even">
<td>Annullamento senza modifiche precedenti delle postazioni</td>
<td><p>Il file di riconciliazione conterrà una sola voce:</p>
<ul>
<li>Un credito per i giorni inutilizzati, poiché l'intero periodo è stato addebitato in anticipo nell'ultima distinta di fatturazione. Viene calcolato in base alla data di fine della sottoscrizione.</li>
</ul></td>
<td>Anticipo fatturato in precedenza: dal 15 agosto al 14 settembre per 10 postazioni = 100 euro.
<p>Parte usata dell'anticipo dal 15 agosto al 24 agosto.</p>
<p>Credito per i giorni inutilizzati: dal 25 agosto al 14 settembre per 10 postazioni = -74,51 euro.</p></td>
</tr>
<tr class="odd">
<td>Annullamento con modifiche precedenti delle postazioni</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>lo storno dell'anticipo</li>
<li>l'addebito per l'uso ripartito</li>
<li>un credito per eventuali giorni inutilizzati</li>
</ul></td>
<td>Anticipo fatturato in precedenza: dal 15 agosto al 14 settembre per 10 postazioni = 100 euro.
<p>Uso ripartito:</p>
<ul>
<li>Dal 15 agosto al 24 agosto per 10 postazioni</li>
<li>Dal 25 agosto al 14 settembre per 5 postazioni</li>
</ul>
<p>Credito per i giorni inutilizzati: dall'1 settembre al 14 settembre per 5 postazioni.</p>
<p>Storno dell'anticipo per il periodo mensile completo dal 15 agosto al 14 settembre = 100 euro.</p></td>
</tr>
</tbody>
</table>

 

 

 






<!--HONumber=Nov16_HO4-->


