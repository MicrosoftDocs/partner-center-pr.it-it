---
title: Scenari comuni di fatturazione (centro per i Partner gestito da 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l'annullamento di una sottoscrizione.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132341"
---
# <a name="common-billing-scenarios"></a>Scenari di fatturazione comuni

**Si applica a**

-   Centro per i partner gestito da 21Vianet


Questo argomento descrive ciò che compare sulla fattura dopo l'aggiunta di nuove sottoscrizioni, la modifica del numero di postazioni in una sottoscrizione o l'annullamento di una sottoscrizione. 


## <a name="licence-based-billing"></a>Fatturazione in base alle licenze


Per i mesi senza apportare modifiche alle sottoscrizioni in base al titolo, si noterà una singola voce per ogni sottoscrizione nel file di riconciliazione e fattura per l'addebito di avanzamento per il mese prossimo.

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
<p>Taglia la fatturazione: Passare l'addebito per il periodo di tutto il mese dal 15 giugno al 14 luglio per 15 postazioni. Supponendo che l'addebito mensile per la sottoscrizione sia di 10 euro, l'addebito sarebbe 10 euro x 15 postazioni = 150 euro.</p></td>
</tr>
<tr class="odd">
<td>Sottoscrizione esistente: Aumentare o ridurre una quantità licenze</td>
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
<p>Taglia la fatturazione: Passare l'addebito per il periodo di tutto il mese da 15 agosto al 14 settembre per 10 postazioni = USD 110.</p></td>
</tr>
<tr class="even">
<td>Annullamento senza modifiche precedenti delle postazioni</td>
<td><p>Il file di riconciliazione conterrà una sola voce:</p>
<ul>
<li>Un credito per i giorni inutilizzati, poiché l'intero periodo è stato addebitato in anticipo nell'ultima distinta di fatturazione. Viene calcolato in base alla data di fine della sottoscrizione.</li>
</ul></td>
<td>In precedenza fatturati in anticipo addebito: Postazioni 15 agosto a 14 settembre per 10 = 100 USD.
<p>Parte usata dell'anticipo dal 15 agosto al 24 agosto.</p>
<p>Carta di credito per i giorni non utilizzati: 25 agosto a 14 settembre per 10 postazioni =-74.51.</p></td>
</tr>
<tr class="odd">
<td>Annullamento con modifiche precedenti delle postazioni</td>
<td><p>Il file di riconciliazione conterrà più voci:</p>
<ul>
<li>lo storno dell'anticipo</li>
<li>l'addebito per l'uso ripartito</li>
<li>un credito per eventuali giorni inutilizzati</li>
</ul></td>
<td>In precedenza fatturati in anticipo addebito: Postazioni 15 agosto a 14 settembre per 10 = 100 USD.
<p>Uso ripartito:</p>
<ul>
<li>Dal 15 agosto al 24 agosto per 10 postazioni</li>
<li>Dal 25 agosto al 14 settembre per 5 postazioni</li>
</ul>
<p>Carta di credito per i giorni non utilizzati: Il 1 ° settembre a 14 settembre per 5 postazioni.</p>
<p>Storno dell'anticipo per il periodo mensile completo dal 15 agosto al 14 settembre = 100 euro.</p></td>
</tr>
</tbody>
</table>
