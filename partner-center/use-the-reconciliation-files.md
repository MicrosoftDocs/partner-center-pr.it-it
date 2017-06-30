---
title: Usare i file di riconciliazione | Centro per i partner
description: Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 61e71d4207d9e8ac68ee4fcfc1f0d04282474032
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/19/2017
---
# <a name="use-the-reconciliation-files"></a>Usare i file di riconciliazione

**Si applica a**

-  Centro per i partner
-  Centro per i partner per Microsoft Cloud per il governo statunitense
-  Centro per i partner per Microsoft Cloud Germania

Per una visualizzazione delle voci relative a ogni addebito in un ciclo di fatturazione, scarica i file di riconciliazione dal dashboard del Centro per i partner. I dettagli includono gli addebiti per le sottoscrizioni di ogni singolo cliente e gli eventi dettagliati, ad esempio un'aggiunta di postazioni a una sottoscrizione in corso.

## <a href="" id="itemizebypartner"></a>Eseguire la scomposizione dei dati in base al partner


I partner nel modello indiretto possono usare questi campi aggiuntivi sia nei file di riconciliazione in base alle licenze che nei file di riconciliazione in base all'uso per eseguire la scomposizione dei dati per ogni rivenditore.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>ID MPN</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>ID MPN</td>
<td><p>ID Microsoft Partner Network (MPN) del partner CSP (diretto o indiretto).</p></td>
</tr>
<tr class="even">
<td>ID MPN rivenditore</td>
<td><p>Viene visualizzato solo nei file di riconciliazione per i partner nel modello indiretto.</p>
<p>ID MPN del rivenditore nel record per la sottoscrizione. Corrisponde all'ID rivenditore elencato per la sottoscrizione specifica nel Centro per i partner.</p>
<p>Per visualizzare o aggiornare il rivenditore, nel menu del Centro per i partner seleziona <strong>Clienti</strong> e quindi scegli il cliente nell'elenco. Nel menu del cliente seleziona <strong>Sottoscrizioni</strong> e quindi scegli la sottoscrizione nell'elenco. Seleziona <strong>Aggiorna</strong> per modificare il valore <strong>Rivenditore (ID MPN)</strong>.</p>
<p>Se un partner CSP ha venduto la sottoscrizione direttamente al cliente, il relativo ID MPN è elencato due volte, sia come ID MPN che come ID MPN del rivenditore.</p>
<p>Se per un partner CSP è presente un rivenditore senza ID MPN, il valore viene impostato sull'ID MPN del partner.</p>
<p>Se il partner CSP rimuove un ID rivenditore, il valore verrà impostato su -1.</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licencebasedfiles"></a> Campi dei file in base alle licenze


Per riconciliare i tuoi addebiti rispetto agli ordini dei clienti, confronta la voce Syndication\_Partner\_Subscription\_Number del file di riconciliazione con l'ID sottoscrizione del Centro per i partner.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonna</strong></td>
<td><strong>Descrizione</strong></td>
<td><strong>Valore di esempio</strong></td>
</tr>
<tr class="even">
<td>OperatingUnit</td>
<td><p>Identificatore univoco per un'entità di fatturazione specifica, in formato GUID. Non è necessario per la riconciliazione, ma può risultare utile. È lo stesso per tutte le righe.</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare l'ordine quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p>
<p>Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner. Vedi Syndication_Partner_Subscription_Number.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>Identificatore univoco per le sottoscrizioni. Un cliente può avere più sottoscrizioni per lo stesso piano, quindi questa informazione è importante per l'analisi di un file di riconciliazione.</p>
<p>Questo campo è associato all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>ID univoco dell'offerta. ID dell'offerta standard in base al listino prezzi.</p>
<p><b>Nota</b>: questo valore non corrisponde all'ID dell'offerta dal listino prezzi. Vedi DurableOfferID di seguito.</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>ID dell'offerta durevole univoco, come definito nel listino prezzi.</p>
<p><b>Nota</b>: questo valore corrisponde all'ID offerta dal listino prezzi.</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi.</p></td>
<td>Microsoft Office 365 (Piano E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>Data di inizio della sottoscrizione, impostata sul giorno successivo a quello in cui è stato inviato l'ordine. Verificando la data di inizio della sottoscrizione insieme alla data di fine, puoi determinare se il cliente è ancora nel primo anno della sottoscrizione o se la sottoscrizione è stata rinnovata per l'anno successivo.</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>Data di fine della sottoscrizione: 12 mesi + x giorni dopo la data di inizio (per allineare con la data di fatturazione del partner) o 12 mesi dalla data di rinnovo.</p>
<p>In fase di rinnovo, i prezzi vengono aggiornati rispetto al listino prezzi corrente. È possibile che venga richiesta una comunicazione con il cliente prima del rinnovo automatico.</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>Giorno di inizio degli addebiti.</p>
<p>Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>Giorno di fine degli addebiti.</p>
<p>Quando un cliente cambia il numero di postazioni, questo valore viene usato per calcolare gli addebiti per giorno (calcolo proporzionale).</p>
<p>L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Tipo di addebito o rettifica. Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
<td><p>Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>Prezzo per postazione. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>Quantity</td>
<td><p>Numero di postazioni. Verifica che corrisponda alle informazioni archiviate nel tuo sistema di fatturazione durante la riconciliazione.</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>Amount</td>
<td><p>Prezzo totale per la quantità. Utile per verificare che il calcolo dell'importo corrisponda al calcolo del prezzo per i clienti.</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>Importo dello sconto applicato a questi addebiti. IUR o le nuove sottoscrizioni idonee per un incentivo contengono anche un importo di sconto in questa colonna.</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>Subtotal</td>
<td><p>Totale al lordo delle imposte. Verifica che il subtotale corrisponda al totale previsto, in caso di sconto.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Tax</td>
<td><p>Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>Totale al netto delle imposte. Verifica se nella fattura sono addebitate imposte.</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>Currency</td>
<td><p>Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</p></td>
<td>EUR</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Nome dell'organizzazione del cliente registrato nel Centro per i partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema.</p></td>
<td>Cliente di prova A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID MPN del partner CSP</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione. Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>Nome di dominio del cliente, usato per identificare il cliente.</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>Nome alternativo della sottoscrizione. Se non viene specificato alcun nome alternativo, il Centro per i partner usa l'OfferName.</p></td>
<td>PROGETTO ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>Nome dell'offerta di servizio acquistata dal cliente, come definito nel listino prezzi. Questo è un campo identico a Nome offerta.</p></td>
<td>PROGETTO PREMIUM ONLINE SENZA CLIENTE PROGETTO</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>Campi dei file in base all'uso


Per riconciliare i tuoi addebiti in base all'uso da parte dei clienti, confronta i campi ResellerID/ResellerName/ResellerBillableAccount del file di riconciliazione con il nome del cliente e l'ID sottoscrizione del Centro per i partner.

I campi seguenti illustrano quali servizi sono stati usati e la tariffa.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Colonna</strong></td>
<td><strong>Descrizione</strong></td>
<td><strong>Valore di esempio</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>ID del partner, in formato GUID.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>Nome partner.</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>ID account partner.</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>Nome dell'organizzazione del cliente registrato nel Centro per i partner. Molto importante per la riconciliazione della fattura con le informazioni di sistema.</p></td>
<td>Cliente di prova A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>ID MPN del partner CSP.</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>ID MPN del rivenditore nel record per la sottoscrizione. Vedi [Eseguire la scomposizione dei dati in base al partner](#itemizebypartner).</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>Numero di fattura in cui viene visualizzata la transazione specificata.</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>Data di inizio del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</p>
<p>L'ora indicata è sempre l'inizio della giornata, le 0:00.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>Data di fine del ciclo di fatturazione, ad eccezione di quando sono presenti date riferite a dati di utilizzo latenti non addebitati in precedenza (dal ciclo di fatturazione precedente).</p>
<p>L'ora indicata è sempre la fine della giornata, le 23:59.</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>Identificatore univoco di una sottoscrizione nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p>
<p>Non corrisponde all'ID sottoscrizione nella console di amministrazione dei partner.</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>Nome alternativo dell'offerta di servizio.</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>Line-of-business dell'offerta di servizio</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>Identificatore univoco di un ordine nella piattaforma di fatturazione Microsoft. Può essere utile per identificare la sottoscrizione quando viene contattato il supporto tecnico, ma non per la riconciliazione.</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>Nome del servizio di Azure in questione.</p></td>
<td>MACCHINE VIRTUALI</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Tipo specifico di servizio di Microsoft Azure.</p></td>
<td><ul>
<li>Service Bus – Individual o Pack</li>
<li>SQL Azure database – Business o Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>Identificatore univoco specifico per l'intera struttura di prezzi e dati di servizio.</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Resource Name</td>
<td><p>Nome della risorsa Azure.</p></td>
<td><ul>
<li>Data Transfer In (GB)</li>
<li>Data Transfer Out (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>Region</td>
<td><p>Area geografica a cui si applica l'uso. Usata principalmente per assegnare le tariffe ai trasferimenti di dati, che variano in base all'area geografica.</p></td>
<td>Asia Pacifico, Europa, America Latina, America del Nord</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>Identificatore univoco MSFT per l'offerta</p></td>
<td>7UD-00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>ID e quantità per specificare nel dettaglio le diverse tariffe relative a un servizio o una risorsa in un determinato periodo di fatturazione. Per le tariffe suddivise in livelli di Azure, potrebbe essere applicata una tariffa fino a una determinata quantità di unità fatturabili e una tariffa diversa da lì in poi.</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>La quantità di servizio usata (ore, GB e così via) durante il periodo di reporting.</p>
<p>Include anche gli utilizzi non fatturati relativi a periodi di reporting precedenti.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>Unità incluse nell'ambito dell'offerta. In genere non presente in CSP.</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>Unità non incluse nell'ambito dell'offerta, che devono essere corrisposte dal partner.</p>
<p>Uguale a ConsumedQuantity - IncludedQuantity.</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>Prezzo di offerta in vigore alla data di inizio della sottoscrizione.</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrice moltiplicato per OverageQuantity, arrotondato al centesimo più vicino.</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>Importo totale delle imposte, in base alle leggi vigenti a livello locale e alle circostanze specifiche.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>Totale al netto delle imposte, se le imposte sono applicabili.</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>Currency</td>
<td><p>Tipo di valuta. Ogni entità di fatturazione ha una sola valuta. Verifica quando viene emessa la prima fattura e dopo qualsiasi aggiornamento importante della piattaforma di fatturazione.</p></td>
<td>EUR</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>Prezzo unitario prima dell'applicazione delle imposte. Uguale a PretaxCharges / OverageQuantity, arrotondato al centesimo successivo.</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>Prezzo unitario dopo l'applicazione delle imposte. Uguale a PostTaxTotal / OverageQuantity o PretaxEffectiveRate + aliquota d’imposta per unità, arrotondato al centesimo successivo.</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>Tipo di addebito o rettifica. Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
<td><p>Vedi <a href="#charge_types">Mapping degli addebiti tra una fattura e il file di riconciliazione</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>ID account univoco nella piattaforma di fatturazione MSFT.</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>Data di distribuzione del servizio.</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>Questa colonna identifica la posizione del data center nell'area geografica dei servizi dove applicabile e popolato.</p></td>
<td>East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>Questa colonna viene usata per tenere traccia del servizio Microsoft Azure singolo che può non essere identificato in modo specifico nella colonna Service Name. I trasferimenti di dati sono ad esempio indicati come &quot;Microsoft Azure - All Services&quot; nella colonna Service Name. La colonna MeteredService indica a quale servizio specifico si riferisce l'utilizzo.</p></td>
<td>AccessControl, CDN, Compute, Database, ServiceBus, Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>Un sottotitolo che definisce ulteriormente il singolo servizio Microsoft Azure oltre il livello specificato dal campo MeteredService.</p></td>
<td>EXTERNAL</td>
</tr>
<tr class="even">
<td>Project</td>
<td><p>Nome definito dal cliente per l'istanza del servizio</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>Numero di connessioni ServiceBus di cui è stato eseguito il provisioning e usate in un determinato giorno.</p></td>
<td>Ad esempio, con una connessione fornita a livello singolo per un periodo di un mese di 30 giorni, Service Info 1 è "1.000000 Connections / 30 days". Se hai un pacchetto da 25 connessioni ServiceBus e ne hai utilizzata 1 per quel giorno, l'uso giornaliero registrato sarà "25 Connections / 30 Days – Used: 1.000000".</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>ID Microsoft univoco, in formato GUID, usato per identificare il cliente.</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>Nome di dominio del cliente, usato per identificare il cliente.</p></td>
<td>example.onmicrosoft.com</td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a>Mapping degli addebiti tra una fattura e il file di riconciliazione

La fattura fornisce un riepilogo degli addebiti, mentre il file di riconciliazione fornisce una descrizione dettagliata delle transazioni di voce, inclusi i tipi di addebito.

Per effettuare il riferimento incrociato degli importi di addebito tra la fattura e il file di riconciliazione, puoi utilizzare le opzioni di filtro di Microsoft Excel per filtrare per tipi di addebito nel file di riconciliazione per eseguire il mapping degli addebiti in fattura a un set di suddivisioni dettagliate nel file di riconciliazione.

Nella tabella seguente sono illustrati i mapping tra una sezione della fattura e i tipi di addebito associati che possono apparire nei file di riconciliazione. 

<table>
<tbody>
<tr>
<td>
<p><strong>Descrizione dell'addebito in fattura</strong></p>
</td>
<td>
<p><strong>Descrizione dell'addebito nel file di riconciliazione (colonna ChargeType)</strong></p>
</td>
<td>
<p><strong>Descrizione dell'addebito</strong></p>
</td>
<td>
<p><strong>Modalità di mapping di questi tipi di addebito alla fattura</strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong>Addebiti periodici</strong></p>
</td>
<td>
<p>Istanza di annullamento rateizzata</p>
</td>
<td>
<p>Addebiti rateizzati rimborsati al cliente in caso di modifica delle postazioni associate</p>
</td>
<td rowspan="8">
<p>Dal file in base alle licenze, somma la colonna <strong>Amount</strong></p>
</td>
</tr>
<tr>
<td>
<p>Tariffa periodica</p>
</td>
<td>
<p>Addebiti periodici per una sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Istanza del ciclo rateizzata</p>
</td>
<td>
<p>Tariffe rateizzate calcolate dal cliente in caso di modifica delle postazioni associate</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza le tariffe in caso di annullamento</p>
</td>
<td>
<p>Rimborso rateizzato per servizio parzialmente inutilizzato all'annullamento</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza le tariffe all'acquisto</p>
</td>
<td>
<p>Tariffe rateizzate all'acquisto</p>
</td>
</tr>
<tr>
<td>
<p>Tariffa di acquisto</p>
</td>
<td>
<p>Addebito iniziale per una sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Rateizza la tariffa al rinnovo</p>
</td>
<td>
<p>Tariffe rateizzate al rinnovo della sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p>Tariffa di rinnovo</p>
</td>
<td>
<p>Addebito per il rinnovo di una sottoscrizione</p>
</td>
</tr>
<tr>
<td>
<p><strong>Altri prodotti e servizi</strong></p>
</td>
<td>
<p>Rateizza le tariffe all'attivazione</p>
</td>
<td>
<p>Tariffe rateizzate dall'attivazione fino alla fine del periodo di fatturazione</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>Amount</strong></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>Costi di utilizzo</strong></p>
</td>
<td>
<p>Valuta la tariffa di utilizzo all'annullamento</p>
</td>
<td>
<p>Tariffa di utilizzo per l'accesso all'annullamento per utilizzo non pagato durante il periodo di fatturazione corrente</p>
</td>
<td rowspan="2">
<p>Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Valuta la tariffa di utilizzo per il ciclo corrente</p>
</td>
<td>
<p>Tariffa di utilizzo per l'accesso per il periodo di fatturazione corrente</p>
</td>
</tr>
<tr>
<td>
<p><strong>Crediti e rettifiche</strong></p>
</td>
<td>
<p>Compensa una voce</p>
</td>
<td>
<p>Rimborso parziale o totale per una voce, comprese le imposte</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>TotalForCustomer</strong></p>
<p>Dal file in base all'uso, somma la colonna <strong>PostTaxTotal</strong></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong>Altri sconti</strong></br>
<em>(in base all'uso)</em></p>
</td>
<td>
<p>Sconto attivazione</p>
</td>
<td>
<p>Sconto applicato all'attivazione della sottoscrizione</p>
</td>
<td rowspan="4">
<p>Dal file in base all'uso, somma la colonna <strong>PretaxCharges</strong></p>
</td>
</tr>
<tr>
<td>
<p>Sconto ciclo</p>
</td>
<td>
<p>Sconto applicato su addebiti periodici</p>
</td>
</tr><tr>
<td>
<p>Sconto rinnovo</p>
</td>
<td>
<p>Sconto applicato al rinnovo della sottoscrizione</p>
</td>
</tr><tr>
<td>
<p>Annulla sconto</p>
</td>
<td>
<p>Addebiti applicati all'annullamento degli sconti</p>
</td>
</tr>
<tr>
<td>
<p><strong>Altri sconti</strong></br>
<em>(in base alle licenze)</em></p>
</td>
<td>
<p><em>Possono essere applicati a più tipi di addebito</em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>TotalOtherDiscount</strong></p>
</td>
</tr>
<tr>
<td>
<p><strong>Imposte</strong>&nbsp;o&nbsp;<strong>IVA</strong></p>
</td>
<td>
<p><em>Possono essere applicate a più tipi di addebito</em></p>
<p><em>Eccezione: "Compensa una voce" include già le imposte. Vedi Crediti e rettifiche, sopra.</em></p>
</td>
<td>
<p>Imposte o imposte sul valore aggiunto (IVA)</p>
</td>
<td>
<p>Dal file in base alle licenze, somma la colonna <strong>Tax</strong></p>
<p>Dal file in base all'uso, somma la colonna <strong>TaxAmount</strong></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
