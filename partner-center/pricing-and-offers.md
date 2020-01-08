---
title: Prezzi e offerte | Centro per i partner
ms.topic: article
ms.date: 09/26/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: L'elenco delle offerte include le diverse famiglie di prodotti che possono essere acquistate tramite il centro per i partner e le relative informazioni sui prezzi.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca270413291ba0d09ca03d9b8b270a65f77a46b1
ms.sourcegitcommit: 2ba40700aeb94c38ba850973dd7ff3330c577937
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/03/2020
ms.locfileid: "75631825"
---
# <a name="pricing-and-offers"></a>Prezzi e offerte

**Si applica a**

-  Centro per i partner

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente amministratore
-   Amministratore dei partner MPN
-   Agente di vendita
-   Amministratore fatturazione

Per vedere i listini prezzi e le offerte più recenti del programma Cloud Solution Provider, vai a **Vendi > Prezzi e offerte**. Troverai listini prezzi separati per i servizi basati su licenza, come Office 365, Microsoft Dynamics CRM ed Enterprise Mobility Suite, e per i servizi basati sull'uso, come Azure. 

L'elenco delle offerte include le diverse famiglie di prodotti che possono essere acquistate tramite il centro per i partner. Queste includono attualmente Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM e Microsoft Azure. L'elenco è destinato ad aumentare.

All'interno di ciascuna di queste famiglie di prodotti sono disponibili per la vendita SKU e aggregazioni di prodotti differenti, a seconda della tua attività. Puoi sempre accedere ai dettagli più recenti su ognuna di queste utilizzando la matrice delle offerte per i rivenditori cloud, disponibile nella pagina Prezzi e offerte.

## <a name="pricelist-preview-and-change-frequency"></a>Anteprima e frequenza di modifica dei listini prezzi 

I servizi basati su licenza includono un'anteprima del listino prezzi, fornita 30 giorni prima delle modifiche. Per visualizzare l'anteprima del listino prezzi, vai a **Vendi > Prezzi e offerte**. Non esiste alcuna anteprima di prezzo per i servizi basati sull'utilizzo, poiché questi servizi sono dinamici. Nella tabella seguente viene illustrato come leggere la tabella dei listini prezzi.

|**Item**        |**Definizione**      |
|:-----------   |:-----------   |
|AD   |Un nuovo elemento nel listino prezzi|
|CHG   |Modifiche al prezzo di listino dal mese al mese. Potrebbero verificarsi altre modifiche non correlate al prezzo di listino. i partner dovrebbero confrontare altre proprietà da mesi a mese per determinare altre modifiche.|
|DEL   |Un elemento rimosso dal listino prezzi|
|UNC   |Prezzo di listino senza modifiche rispetto ai prezzi del mese precedente  |
|Data di inizio validità   |La prima data in cui può essere ordinata un'offerta    |
|Data di fine validità   |L'ultima data in cui può essere ordinata un'offerta   |
|Nome visualizzato offerta   |Nome dell'offerta come visualizzato dai clienti   |
|ID offerta   |Identificatore interno dell'offerta   |
|Tipo di contratto di licenza   |Può essere aziendale, per la pubblica amministrazione o per scuola o università e determina i tipi di clienti a cui l'offerta può essere venduta.|
|Unità di acquisto   |La durata dell'offerta da acquistare. In genere un mese.   |
|Tipo di licenza secondario   |Sarà non specifico, componente aggiuntivo o versione di valutazione. Componente aggiuntivo indica che sono presenti prodotti prerequisiti che il cliente deve acquistare prima del componente aggiuntivo.|
|Tipo di cliente finale   |Si riferisce al tipo di contratto di licenza: licenza aziendale - rivenditore cloud aziendale, licenza per la pubblica amministrazione - rivenditore cloud per la pubblica amministrazione, licenza per scuola o università - rivenditore cloud per istituti di istruzione o rivenditore cloud per studenti   |
|Prezzo di listino   |Il prezzo che il partner pagherà   |
|Prezzo stimato al dettaglio   |Il prezzo al dettaglio stimato o consigliato per il cliente   |

## <a name="price-changes"></a>Modifiche ai prezzi

Le modifiche ai prezzi sono un'occorrenza comune. I partner possono anticipare le variazioni dei prezzi per le offerte basate sulle licenze esaminando l'anteprima dell'elenco prezzi nella pagina prezzi e offerte del dashboard del centro per i partner. I prezzi basati sull'utilizzo di Azure non hanno un'anteprima. I partner possono restare al passo con le variazioni dei prezzi di consumo di Azure usando l'API di tariffario che restituisce i prezzi del contatore di tale giorno.

|**Tipo di prodotto**   |**Esempi di prodotti**  |**Anteprima disponibile** |**Modificare i dettagli**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basato su licenza|Office, Dynamics, Intune, Windows Enterprise|30 giorni|Elenco delle modifiche al prezzo contrassegnate come CHNG negli elenchi prezzi di anteprima|
|Basato sull'utilizzo|Risorse di Azure|Non disponibile|Log delle modifiche disponibile nella scheda **cronologia modifiche** dell'elenco prezzi del mese precedente|
|Software||Non disponibile|Confrontare elenchi prezzi manualmente da un mese a un mese|
|Prenotazioni|Macchine virtuali, pre-pagate|Non disponibile|Confrontare elenchi prezzi manualmente da un mese a un mese|

I prezzi basati sull'utilizzo possono variare in un mese. Per ottenere i prezzi giornalieri "correnti" per queste risorse di Azure, i partner devono chiamare l'API tariffario. 

>[!Note] 
>Le modifiche ai prezzi della sottoscrizione si applicano solo durante il rinnovo. Il costo mensile di un partner è determinato dal prezzo di acquisto o dal prezzo al momento della creazione di una sottoscrizione. Se un prezzo aumenta o diminuisce dopo l'acquisizione del periodo annuale, al partner non viene addebitato il prezzo modificato fino al rinnovo, in genere in corrispondenza del periodo di 12 mesi.

## <a name="pricing-and-special-segments"></a>Prezzi e segmenti speciali

CSP offre alcuni servizi a segmenti di mercato speciali, ad esempio Education, no profit e Government community Cloud. Non tutti i servizi sono disponibili in tutti i canali. Nessun segmento predefinito è quello che viene chiamato segmento "commerciale". Tutti i prezzi basati sulle licenze sono disponibili nell'elenco prezzi basato su licenza della pagina prezzi e offerte. I prezzi di Azure gov sono disponibili nell'elenco prezzi basato sull'utilizzo quando sono connessi al tenant CSP abilitato per Azure gov.

|**Segmento**   |**utenti che devono qualificarsi**   |**Partner idoneo per i clienti**|**Tipi di prodotto abilitati**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Istruzione|Cliente|No, la qualifica del cliente verrà eseguita da Microsoft |Solo basato su licenza|
|No profit|Cliente|No, il cliente si qualifica all'esterno del centro per i partner|Solo basato su licenza|
|Government Community Cloud (GCC) (Cloud della community per enti pubblici)|Partner e cliente|Una volta abilitata la funzionalità GCC, il partner può creare clienti GCC| Solo basato su licenza|
|Azure gov|Partner|Una volta qualificato, il partner opera in un tenant CSP specifico di Azure gov|Risorse di Azure|

I margini dei partner, la differenza tra il prezzo di listino e i prezzi di vendita al dettaglio stimati, possono variare da segmento a segmento. In genere, la formazione e la mancata redditività tendono a avere margini inferiori o senza margini per i partner CSP. Per i valori esatti, vedere l'elenco dei prezzi basato sulle licenze.  
## <a name="pricing-between-azure-and-non-azure"></a>Prezzi tra Azure e non Azure

I prezzi variano in base ai diversi tipi di offerte. I prezzi basati sulle licenze sono in genere la quantità per postazione (licenza) per un determinato mese. I prezzi basati sull'utilizzo sono determinati dall'uso di una determinata risorsa, con un ID contatore associato. Ai partner non viene addebitato l'acquisto della sottoscrizione di Azure, ma vengono addebitate le risorse utilizzate da diverse distribuzioni nella sottoscrizione. I prezzi nell'elenco prezzi basato sull'utilizzo sono organizzati in base a diversi ID del contatore delle risorse in Azure.

Le prenotazioni di Azure sono acquisti basati su termini per il tipo di risorsa specifico, ovvero macchine virtuali. L'acquisto di una prenotazione di Azure consente a un partner di pagare in anticipo (uno o tre anni) e di riservare una determinata macchina virtuale. In questo modo il denaro del partner viene salvato e si garantisce che la macchina virtuale sia sempre disponibile per tutta la durata del periodo di validità. Un partner può allineare la prenotazione che desidera per gli ID del contatore delle risorse basate sull'utilizzo. Gli ID del contatore sono coerenti tra le risorse, se il partner Acquista una macchina virtuale o semplicemente distribuisce la macchina virtuale come risorsa basata sull'utilizzo. 


## <a name="offers-matrix"></a>Matrice delle offerte

Consulta la matrice delle offerte per i rivenditori cloud nella pagina Prezzi e offerte per visualizzare le differenti SKU e aggregazioni di prodotti disponibili per le tue attività di vendita. La matrice delle offerte include le offerte disponibili per ognuna delle impostazioni locali. Se un elemento si trova nel listino prezzi ma non ancora nella matrice, significa che i prodotti non possono ancora essere ordinati. Non appena sono disponibili per essere ordinati, la matrice delle offerte viene aggiornata.

Per i partner CSP che usano il Software Development Kit (SDK) del centro per i partner. Inoltre, Microsoft pubblica un elenco dei servizi di Azure in CSP nella pagina Prezzi e offerte.

### <a name="offers-matrix-and-pricelist-questions"></a>Domande relative alla matrice delle offerte e al listino prezzi

Per domande sui prezzi o sulla matrice di offerte, inviare una richiesta di assistenza tramite il centro per i partner.
