---
title: Esportazione e importazione bulk di opportunità di co-selling tramite file di Excel/CSV in riferimenti
description: Informazioni su come scaricare, creare o aggiornare le opportunità di co-selling usando file di Excel (CSV) nel centro per i partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 39a1370ad4e5da9120c74b46dfb0c20cd93df4e3
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712190"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Operazioni bulk per le opportunità di co-selling con file con valori delimitati da virgole (CSV)

**Ruoli appropriati**

- Amministratore delle segnalazioni
- Utente delle segnalazioni

Le operazioni bulk nel centro per i partner consentono all'azienda di esportare e importare i dati relativi alle opportunità di co-selling. Passare alla pagina **opportunità di co-selling** per trovare i collegamenti **Importa** ed **Esporta** nella parte superiore destra del banner del titolo della pagina. Questa funzionalità può essere utilizzata dagli utenti con autorizzazioni di **amministratore** e di **riferimento** .

> [!IMPORTANT]
> Le azioni di creazione/aggiornamento eseguite mediante l'importazione bulk non sono reversibili. Prestare attenzione quando si modifica o si crea un numero elevato di record. È possibile modificare solo un subset di campi dopo la creazione di una trattativa. **Non saranno consentite azioni quando si raggiunge uno stato terminale come rifiutato/scaduto/vinto/perduto.**

## <a name="export-co-sell-opportunities"></a>Esporta opportunità di co-selling

Le informazioni seguenti descrivono la funzionalità di esportazione:

- È possibile esportare un **massimo di 5000 record** facendo clic sul pulsante **Esporta** .
- Le offerte scaricate verranno basate sui livelli di accesso. Gli amministratori e gli utenti di riferimento possono ottenere risultati diversi in base al relativo ambito e inclusione come membri del team nelle offerte. Altre informazioni sulle [autorizzazioni](permissions-overview.md#manage-referrals)per i riferimenti.
- La funzione Export prende in considerazione la scheda corrente nella pagina opportunità di co-selling e i filtri applicati.
- Verrà generato un file CSV con tutti i dati basati sui filtri applicati.
- Il download dei record può richiedere fino a un minuto.
- Non è necessario attendere il completamento dell'azione di download. Anche se si passa ad altre pagine del centro per i partner, il file verrà scaricato non appena la funzione di esportazione è completa.
- È possibile riutilizzare il file scaricato per modificare i dettagli dell'operazione e caricare per aggiornare i record.

## <a name="import-co-sell-opportunities"></a>Importa opportunità di co-selling

- È possibile creare o aggiornare un **massimo di 1000 record** utilizzando la funzionalità di importazione.
- È possibile compilare il modello da zero scaricando il modello dalla pagina Importa nel centro per i partner.
- È anche possibile usare la funzionalità di esportazione per scaricare i record esistenti e aggiornarli.
- Se il file contiene più di 1000 record, non può essere elaborato.
- Dopo che il file è stato elaborato, un riepilogo con il numero di riferimenti creati, aggiornati e non elaborati verrà visualizzato nell'ultima scheda file di processo.
- È possibile scaricare i dettagli dei record elaborati, correggere eventuali errori e caricare lo stesso file per creare o aggiornare i record non riusciti nell'esecuzione precedente. **Rimuovere tutti i record riusciti dal file prima di caricare i record corretti che non sono riusciti nell'esecuzione precedente.**
- Per aggiungere altre soluzioni, aggiungere colonne aggiuntive accanto alla soluzione 1 e usare il nome della colonna come soluzione X, dove X rappresenta il numero della soluzione nell'affare. Ad esempio, soluzione 2, soluzione 3.
- È possibile aggiungere fino a 50 soluzioni a un problema.
- Per aggiungere altri membri del team, aggiungere colonne aggiuntive accanto al membro del team 1 e usare il nome della colonna come membro del team X, dove X rappresenta il numero del membro del team nell'affare. Ad esempio, il membro del team 2, il membro del team 3.
- È possibile aggiungere fino a un massimo di 50 membri del team a un'operazione.

> [!NOTE]
> Non è necessario attendere il completamento dell'elaborazione. Al termine dell'elaborazione, i dettagli dell'ultimo file elaborato saranno disponibili per il download. **Se si caricano file con record 1000, possono essere necessari fino a 10 minuti.**

> [!IMPORTANT]
> Leggere attentamente tutte le istruzioni e verificare il formato di ogni colonna dalla tabella seguente prima di creare o aggiornare le offerte usando i file CSV nel centro per i partner.

|**Nome colonna**|**È obbligatorio?**|**Descrizione**|**Valore/i di esempio**|
|-----|:-----|:---------|:---|
Errors|No|Gli eventuali errori correlati alle operazioni di creazione/aggiornamento w. r. t nei riferimenti verranno inclusi in questa colonna. Se sono presenti più errori, tutti verranno elencati separati da un punto e virgola.|Manca la soluzione campo obbligatoria 1|
ID Engagement|No|L'ID di engagement viene generato dal sistema di riferimento del centro per i partner Microsoft. Non obbligatorio per la creazione di nuovi riferimenti. Se si sta aggiornando un record, è possibile usare l'ID di engagement esistente.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID di riferimento|No|L'ID di riferimento viene generato dal sistema di riferimento del centro per i partner Microsoft. Non obbligatorio per la creazione di nuovi riferimenti. Inserire l'ID di riferimento se si sta aggiornando un record esistente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nome dell'affare|Sì|Nome descrittivo per l'operazione per il riferimento.|Successo della primavera del Regno Unito
Nome del cliente|Sì|Nome della società del cliente. Usare il nome legale dell'organizzazione per una corrispondenza rapida sul lato Microsoft.|Contoso Corporation
Riga indirizzo cliente 1|Sì|Riga indirizzo 1 della società del cliente. |Un modo contoso
Riga indirizzo cliente 2|No|Indirizzo della riga 2 della società del cliente.|NE 148 Street
Città del cliente|Sì|Città in cui si trova l'organizzazione del cliente.|Redmond
Customer State|No|Stato in cui si trova l'organizzazione del cliente.|Washington
Customer Postal Code|No|CAP della regione in cui si trova l'organizzazione del cliente.|98052
Customer Country|Sì|Paese/area geografica in cui si trova l'organizzazione del cliente. Usare i codici paese a due lettere come indicato [qui]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|US
ID del cliente D-U-N-S|No|Provare a recuperare l'ID DUNS dell'organizzazione del cliente. Ciò consentirà di individuare più rapidamente l'organizzazione del cliente sul lato Microsoft, che facilita l'assegnazione di venditori più veloci. È possibile ottenere l'ID DUNS gratuitamente dal [sito Web](https://www.dnb.com/duns-number/lookup.html).|81466849
Nome contatto cliente|Dipende da|Il primo nome è obbligatorio solo se è necessaria la Guida di Microsoft. Il primo nome del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|John
Cognome contatto cliente|Dipende da|Il cognome è obbligatorio solo se è necessaria la Guida di Microsoft. Il cognome del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|Customer
Numero di telefono di contatto del cliente|Dipende da|Il numero di telefono è obbligatorio solo se è necessaria la Guida di Microsoft. Numero di telefono del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|9999999999
Indirizzo di posta elettronica del contatto del cliente|Dipende da|L'indirizzo di posta elettronica è obbligatorio solo se è necessaria la Guida di Microsoft. Indirizzo di posta elettronica del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|john.customer@contoso.com
Stato del riferimento partner|Sì|Indica lo stato dell'affare dal punto di vista della società. Obbligatorio se si tenta di creare o modificare un riferimento. Usare **New** se si sta provando a creare una nuova operazione. I valori accettati sono descritti [qui](/partner/develop/referral-resources#referralstatus).|Attivo
Stato secondario del riferimento partner|Sì|Indica lo stato esatto dell'operazione. Usare **accettato** se si sta provando a creare una nuova operazione. È anche necessario se si sta modificando un riferimento esistente. I valori accettati sono descritti [qui](/partner/develop/referral-resources#referralsubstatus).|Accettato
Stato Microsoft Referral|Dipende da|Indica lo stato della richiesta di co-selling inviata a Microsoft per chiedere assistenza. Questo è un campo di sola lettura. Qualsiasi modifica apportata a questo campo durante l'importazione dei dati verrà ignorata.| In sospeso
Motivo rifiutato/perso|Dipende da| È necessario fornire queste informazioni solo se si sta modificando lo stato secondario del campo in modo che sia stato rifiutato o perso. In caso contrario, è possibile ignorare questa colonna. <br/> **Immettere un numero basato sulle opzioni seguenti** <br/><br/> **1**-il budget del progetto non è adeguato  <br/> **2**-il cliente non ha risposto  <br/> **3**-il cliente ha scelto un altro fornitore  <br/> **4** -requisito del cliente non soddisfatto  <br/> **5** -non è un cliente <br/> **6**-la riga di tempo proposta è troppo corta <br/> **7** -segnala come abusi, posta indesiderata o phishing <br/> **8** -altri |6|
Sales Stage|No|Questo è il campo per indicare la fase di vendita dettagliata del riferimento. Scopri di più sulle fasi di vendita [qui](./manage-co-sell-opportunities.md)|40
Valore dell'affare stimato|Sì|"Valore dell'affare basato sulle conversazioni iniziali con il cliente. Questo può essere modificato fino a quando l'operazione non raggiunge uno degli stati terminali| vinto o perso ".|12563
Valuta|Sì|La valuta in cui viene immesso il valore dell'operazione. [Qui](https://en.wikipedia.org/wiki/ISO_4217)è possibile trovare i codici di valuta.|USD
Data di chiusura stimata|Sì|Data di chiusura stimata dell'operazione in base alle conversazioni iniziali con il cliente nel formato MM/gg/aaaa. <br/> **La data deve essere nel fuso orario UTC. Tutte le date visualizzate nell'interfaccia utente del centro per i partner sono basate su fusi orari localizzati. Se si sta esaminando il riferimento per il quale è stata specificata la data nel fuso orario UTC, potrebbe essere presente una differenza di +/-un giorno nell'interfaccia utente del centro per i partner.**|1/30/2020
ID CRM|No|Identificatore del riferimento specifico nel sistema CRM, se presente. Si tratta di un campo di immissione di testo in formato libero.|34234324-Greta-345345-SFD
ID campagna di marketing|No|Questo campo indica la campagna di marketing, che ha generato questo riferimento specifico. Usato in genere per il calcolo del ROI|BingSummer2020
Note|No|Note dettagliate che indicano gli aggiornamenti relativi al riferimento|Si tratta di una nota di esempio
La Guida Microsoft è necessaria?|Sì|Per indicare se si vuole che Microsoft consenta di eseguire questa richiesta di co-selling|Sì
Quale guida specifica di Microsoft?|Dipende da|Uno dei sei diversi modi in cui Microsoft può aiutarti. Questa operazione è applicabile solo se si sceglie Sì per la domanda "richiesta di assistenza Microsoft? " <br/> **Immettere un numero basato sulle opzioni seguenti** <br/><br/> **1**-proposta di valore specifico del carico di lavoro  <br/> **2**-architettura tecnica del cliente  <br/> **3**-modello di prova/demo  <br/> **4**-citazioni e licenze  <br/> **5**-successo dei clienti successivi alle vendite  <br/> **6**-generale o altro|1|
Condividi con il team di vendita Microsoft|Sì|Questa operazione consente di indicare se si desidera condividere i dettagli relativi al team di vendita Microsoft. Questa operazione è applicabile solo se si sceglie No per la domanda "richiesta di assistenza Microsoft? "|Sì
Note a Microsoft|No|Eventuali note specifiche su Microsoft per richiedere assistenza da Microsoft|Serve aiuto con un modello di verifica per il cliente Contoso
Consenso alla condivisione del contatto clienti/partner|Sì|Il consenso a condividere i dettagli di contatto dei clienti e i dettagli di contatto dei dipendenti della società che stanno lavorando al problema. **Le offerte non verranno create o aggiornate se si sceglie No per questa colonna.** |Sì
Soluzione 1|Sì|ID soluzione (obbligatorio), valuta (facoltativo) in cui viene immesso il valore dell'operazione. È possibile trovare i codici di valuta [qui](https://en.wikipedia.org/wiki/ISO_4217), il prezzo dello SKU (facoltativo) e la quantità dello SKU (facoltativo)  |SOL-1234-PQRS, USD, 10, 100
Membro del team 1|Sì|Nome, cognome, numero di cellulare e ID di posta elettronica del rispettivo membro del team.| Bob, partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Passaggi successivi

È possibile usare questi connettori di co-selling del centro per i partner per co-selling con Microsoft dall'interno dei sistemi CRM.

- [Co-selling Connector per Dynamics 365 CRM-Panoramica](connector-dynamics.md)
- [Connettore di co-selling per CRM Salesforce - Panoramica](connector-salesforce.md)
