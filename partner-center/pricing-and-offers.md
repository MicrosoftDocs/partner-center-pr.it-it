---
title: Prezzi e offerte
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'elenco delle offerte include le diverse famiglie di prodotti che possono essere acquistate tramite il centro per i partner e le relative informazioni sui prezzi.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 19e935122d1223c87714ca8c3a3f4fd212f2cf3c
ms.sourcegitcommit: 4731d6647db34cf214f781f9e002074210fcfc29
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/21/2020
ms.locfileid: "81664289"
---
# <a name="pricing-and-offers"></a>Prezzi e offerte

**Si applica a**

- Centro per i partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Agente amministratore
- Amministratore dei partner MPN
- Agente di vendita
- Amministratore fatturazione

Per visualizzare i programmi e le offerte del provider di soluzioni cloud più recenti, dal portale per i partner, vai a **vendere > prezzi e offerte**. Sono disponibili elenchi prezzi distinti per i servizi basati su licenza, tra cui Office 365, Microsoft Dynamics CRM ed Enterprise Mobility Suite, e per i servizi basati sull'utilizzo che includono Azure.

L'elenco delle offerte include le diverse famiglie di prodotti che possono essere acquistate tramite il centro per i partner. Attualmente includono Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM e Microsoft Azure. Questo elenco continuerà ad espandersi Man mano che nuovi prodotti diventano disponibili.

All'interno di ognuna di queste famiglie di prodotti sono disponibili diversi SKU e bundle di prodotti da vendere a seconda dell'azienda. È sempre possibile accedere ai dettagli più recenti su questi prodotti usando la matrice di offerte del rivenditore cloud, disponibile nella pagina prezzi e offerte.

## <a name="price-list-preview-and-change-frequency"></a>Anteprima dell'elenco prezzi e frequenza di modifica 

I servizi basati su licenze includono un'anteprima di listino prezzi, che fornisce 30 giorni prima di qualsiasi modifica. Per visualizzare l'anteprima dell'elenco prezzi, vai a **vendi > prezzi e offerte**. Non sono disponibili anteprime dei prezzi per i servizi basati sull'utilizzo poiché questi servizi sono dinamici. Nella tabella seguente viene illustrato come leggere la tabella Listino prezzi.

|**Item**        |**Definizione**      |
|:-----------   |:-----------   |
|ADD   |Un nuovo elemento all'elenco prezzi|
|CHG   |Modifiche al prezzo di listino dal mese al mese. Potrebbero verificarsi altre modifiche non correlate al prezzo di listino. i partner dovrebbero confrontare gli elenchi prezzi tra i mesi per determinare le modifiche apportate ad altre proprietà.|
|DEL   |Elemento rimosso dall'elenco prezzi|
|UNC   |Prezzo di listino non modificato rispetto all'elenco prezzi del mese precedente  |
|Data di inizio validità   |Prima data è possibile ordinare l'offerta    |
|Data di inizio validità   |Ultima data in cui è possibile ordinare un'offerta   |
|Nome visualizzato dell'offerta   |Nome del cliente per l'offerta   |
|Offer ID (ID offerta)   |Identificatore interno per l'offerta   |
|Tipo di contratto di licenza   |I tipi di contratto di licenza possono essere aziendali, governativi o accademici. Il tipo di contratto determina i tipi di clienti a cui è possibile vendere l'offerta.|
|Unità di acquisto   |Durata dell'acquisto dell'offerta. Le unità di acquisto sono in genere di un mese.   |
|Tipo di licenza secondaria   |I tipi di licenza secondari saranno non specifici, componente aggiuntivo o versione di valutazione. Il componente aggiuntivo indica che sono presenti prodotti prerequisiti che il cliente deve acquistare prima di acquistare il componente aggiuntivo.|
|Tipo di cliente finale   |Si riferisce al tipo di contratto di licenza: Corporate License-cloud Reseller Corporate, Government License-cloud Reseller Government o Academic License-cloud Reseller Student o cloud Reseller Student   |
|Prezzo di listino   |Prezzo pagato dal partner   |
|Prezzo ERP   |Prezzo al dettaglio stimato o consigliato per il cliente   |

## <a name="price-changes"></a>Modifiche ai prezzi

Le modifiche ai prezzi sono un'occorrenza comune. I partner possono anticipare le variazioni dei prezzi per le offerte basate sulle licenze esaminando l'anteprima Listino prezzi. Nel dashboard del centro per i partner aprire la pagina prezzi e offerte per visualizzare l'anteprima dell'elenco prezzi.

Tuttavia, i prezzi basati sull'utilizzo di Azure non hanno un'anteprima. I partner possono restare al passo con le variazioni dei prezzi di consumo di Azure usando l'API di tariffario, che restituisce i prezzi del contatore di tale giorno.

|**Tipo di prodotto**   |**Esempi di prodotti**  |**Anteprima disponibile** |**Dettagli modifiche**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basato su licenza|Office, Dynamics, Intune, Windows Enterprise|30 giorni|Elenco delle modifiche al prezzo contrassegnate come CHNG negli elenchi prezzi di anteprima|
|Basato sull'utilizzo|Risorse di Azure|Non disponibile|Log delle modifiche disponibile nella scheda **cronologia modifiche** dell'elenco prezzi del mese precedente|
|Software||Non disponibile|Confrontare elenchi prezzi manualmente da un mese a un mese|
|Prenotazioni|Macchine virtuali, pre-pagate|Non disponibile|Confrontare elenchi prezzi manualmente da un mese a un mese|

I prezzi basati sull'utilizzo possono variare in un mese. Per ottenere i prezzi giornalieri "correnti" per queste risorse di Azure, i partner devono chiamare l'API tariffario. 

> [!Note] 
> Le modifiche ai prezzi della sottoscrizione si applicano solo durante il rinnovo. Il costo mensile di un partner è determinato dal prezzo di acquisto o dal prezzo al momento della creazione di una sottoscrizione. Se un prezzo aumenta o diminuisce dopo l'acquisizione del periodo annuale, al partner non viene addebitato il prezzo modificato fino al rinnovo, in genere in corrispondenza del periodo di 12 mesi.

## <a name="pricing-and-special-segments"></a>Prezzi e segmenti speciali

CSP offre alcuni servizi a segmenti di mercato speciali, ad esempio Education, no profit e Government community Cloud. Non tutti i servizi sono disponibili in ogni canale. Nessun segmento predefinito è quello che viene chiamato segmento "commerciale". Tutti i prezzi basati sulle licenze sono disponibili nell'elenco prezzi basato su licenza della pagina prezzi e offerte. I prezzi di Azure per enti pubblici sono disponibili nell'elenco prezzi basato sull'utilizzo quando sono connessi al tenant CSP abilitato per Azure per enti pubblici.

|**Segment**   |**utenti che devono qualificarsi**   |**Partner idoneo per i clienti**|**Tipi di prodotto abilitati**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Customer|No, la qualifica del cliente verrà eseguita da Microsoft |Solo basato su licenza|
|Senza scopo di lucro|Customer|No, il cliente si qualifica all'esterno del centro per i partner|Solo basato su licenza|
|Government Community Cloud (GCC) (Cloud della community per enti pubblici)|Partner e cliente|Una volta abilitata la funzionalità GCC, il partner può creare clienti GCC| Solo basato su licenza|
|Azure Government|Partner|Una volta qualificato, il partner opera in un tenant CSP specifico di Azure per enti pubblici|Risorse di Azure|

I margini dei partner, la differenza tra il prezzo di listino e i prezzi di vendita al dettaglio stimati, possono variare da segmento a segmento. In genere, la formazione e la mancata redditività tendono a avere margini inferiori o senza margini per i partner CSP. Per i valori esatti, vedere l'elenco dei prezzi basato sulle licenze.  
## <a name="pricing-between-azure-and-non-azure"></a>Confronto prezzi tra Azure e non Azure

I prezzi variano in base ai diversi tipi di offerte. I prezzi basati sulle licenze sono in genere la quantità per postazione (licenza) per un determinato mese. I prezzi basati sull'utilizzo sono determinati dall'uso di una determinata risorsa, con un ID contatore associato. Ai partner non viene addebitato l'acquisto della sottoscrizione di Azure. Tuttavia, ai partner vengono addebitate le risorse utilizzate da distribuzioni diverse nella sottoscrizione di Azure. I prezzi nell'elenco prezzi basato sull'utilizzo sono organizzati in base a diversi ID del contatore delle risorse in Azure.

Le prenotazioni di Azure sono acquisti basati su termini per il tipo di risorsa specifico, ovvero macchine virtuali. L'acquisto di una prenotazione di Azure consente a un partner di pagare in anticipo (uno o tre anni) e di riservare una determinata macchina virtuale. Le prenotazioni salvano il denaro del partner e assicurano che la macchina virtuale sia sempre disponibile per tutta la durata del periodo di validità. Un partner può allineare la prenotazione che desidera per gli ID del contatore delle risorse basate sull'utilizzo. Gli ID del contatore sono coerenti tra le risorse, se il partner Acquista una macchina virtuale o semplicemente distribuisce la macchina virtuale come risorsa basata sull'utilizzo.

## <a name="offers-matrix"></a>Matrice delle offerte

Nella pagina prezzi e offerte visualizzare la matrice di offerte del rivenditore cloud per informazioni sui diversi SKU e sui bundle di prodotti disponibili per la vendita. La matrice offers include le offerte disponibili per le impostazioni locali. Se un elemento è elencato nell'elenco prezzi ma non nella matrice dell'offerta, significa che i prodotti non possono essere ancora ordinati. Non appena saranno disponibili per l'ordine, viene aggiornata la matrice delle offerte.

Per i partner CSP che usano il Software Development Kit (SDK) del centro per i partner. Microsoft pubblica inoltre un elenco dei servizi di Azure in CSP nella pagina prezzi e offerte.

### <a name="offers-matrix-and-price-list-questions"></a>Domande sulle offerte di matrici e prezzi

Per domande sull'elenco prezzi o sulla matrice di offerte, inviare una richiesta di assistenza tramite il centro per i partner.

## <a name="offer-limits"></a>Limiti dell'offerta

Alcune offerte basate sulle licenze hanno alcune regole e limitazioni che proibiscono più acquisti per lo stesso cliente. Queste regole si applicano alla maggior parte delle versioni di valutazione e a molte delle piccole offerte aziendali. Le **offerte Small Business** sono definite dalle offerte con un numero massimo di licenze inferiore a 300.

Questi vincoli di acquisto sono definiti come parte della configurazione dell'offerta ed è possibile trovarli cercando nella matrice dell'elenco di offerte. Due colonne di dati interagiscono per definire l'applicazione: 1. Ambito limite offerta e 2. Limite dell'offerta. I vincoli vengono applicati durante l'acquisto. Il catalogo nel centro per i partner impedisce a un partner di acquistare più offerte rispetto a quelle consentite dalle regole. Qualsiasi tentativo di violare i vincoli provocherà un errore.

L'ambito del limite dell'offerta viene registrato come colonna nella matrice dell'elenco di offerte e può avere valori None, Lifetime o Concurrent. 

- Le offerte con **nessuno** possono essere acquistate senza vincoli.
- Le offerte di **durata** possono essere acquistate una sola volta.
- Le offerte **simultanee** possono essere acquistate il numero di volte consentito dal valore **limite offerta** per l'offerta. Per la maggior parte delle versioni di valutazione è previsto un limite per l'offerta di durata pari a "1". Per la maggior parte delle piccole aziende è previsto un ambito di limite di offerte simultanee con un limite di offerta pari a "2".

> [!IMPORTANT]
> I limiti di concorrenza vengono applicati anche se un'offerta viene annullata. È necessario annullare completamente l'offerta e quindi effettuare il deprovisioning per liberare spazio aggiuntivo in modo da consentire un altro acquisto.

### <a name="taxes-and-pricing"></a>Tasse e prezzi

Tutti i prezzi negli elenchi prezzi del centro per i partner CSP sono inclusivi fiscali. Per ulteriori informazioni [, le imposte e le imposte fiscali](tax-and-tax-exemptions.md)dei documenti del centro partner.
