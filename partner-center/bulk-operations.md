---
title: Esportazione e importazione bulk di opportunità di co-selling tramite file Excel/CSV nelle segnalazioni
description: Informazioni su come scaricare, creare o aggiornare opportunità di co-selling usando file di Excel (CSV) in Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149163"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Operazioni bulk per le opportunità di co-selling usando file con valori delimitati da virgole (CSV)

**Ruoli appropriati:** amministrazione delle segnalazioni | Utente delle segnalazioni

Le operazioni bulk in Partner Center consentono all'azienda di esportare e importare i dati delle opportunità di co-selling. Passare alla pagina **delle opportunità di co-selling** per trovare **i** collegamenti di importazione **ed** esportazione in alto a destra nel banner del titolo della pagina. Gli utenti con **autorizzazioni di amministratore di Referrals** e **Referrals Utente** possono usare questa funzionalità.

> [!IMPORTANT]
> Le azioni di creazione/aggiornamento eseguite tramite l'importazione bulk non sono reversibili. Prestare attenzione quando si modifica o si crea un numero elevato di record. Dopo aver creato un accordo, è possibile modificare solo un subset di campi. **Non sarà consentita alcuna azione quando un'operazione raggiunge uno stato del terminale, ad esempio Rifiutato/Scaduto/Vinto/Perso.**

## <a name="export-co-sell-opportunities"></a>Esportare opportunità di co-selling

Le informazioni seguenti descrivono la funzionalità di esportazione:

- È possibile esportare **un massimo di 5000 record** facendo clic sul pulsante **esporta.**
- Le offerte scaricate saranno basate sui livelli di accesso. Gli amministratori delle segnalazioni e gli utenti referral possono ottenere risultati diversi in base all'ambito e all'inclusione come membri del team nelle trattative. Altre informazioni sulle [autorizzazioni per le segnalazioni.](permissions-overview.md#manage-referrals)
- La funzione di esportazione tiene conto della scheda corrente nella pagina delle opportunità di co-selling e dei filtri applicati.
- Verrà generato un file CSV con tutti i dati basati sui filtri applicati.
- Il download dei record può richiedere fino a un minuto.
- Non è necessario attendere il completamento dell'azione di download. Anche se si passa ad altre pagine in Partner Center, il file verrà scaricato non appena la funzione di esportazione sarà completa.
- È possibile riutilizzare il file scaricato per modificare i dettagli della trattativa e caricarlo per aggiornare i record.

## <a name="import-co-sell-opportunities"></a>Importare opportunità di co-selling

- È possibile creare o aggiornare un **massimo di 1000 record** usando la funzionalità di importazione.
- È possibile compilare il modello da zero scaricando il modello dalla pagina Importa Partner Center.
- È anche possibile usare la funzionalità Esporta per scaricare i record esistenti e aggiornarli.
- Se il file contiene più di 1000 record, non può essere elaborato.
- Dopo l'elaborazione del file, nell'ultima scheda del file di processo verrà visualizzato un riepilogo con il numero di segnalazioni create, aggiornate e non elaborate.
- È possibile scaricare i dettagli dei record elaborati, correggere eventuali errori e caricare lo stesso file per creare o aggiornare i record non riusciti nell'esecuzione precedente. **Rimuovere tutti i record con esito positivo dal file prima di caricare i record corretti non riusciti nell'esecuzione precedente.**
- Per aggiungere altre soluzioni, aggiungere altre colonne accanto alla soluzione 1 e usare il nome di colonna Soluzione X, dove X rappresenta il numero della soluzione nella trattativa. Ad esempio, Soluzione 2, Soluzione 3.
- È possibile aggiungere fino a 50 soluzioni a una trattativa.
- Per aggiungere altri membri del team, aggiungere altre colonne accanto a Membro del team 1 e usare il nome della colonna come Membro del team X, dove X rappresenta il numero del membro del team nella trattativa. Ad esempio, Membro del team 2, Membro del team 3.
- È possibile aggiungere fino a 50 membri del team a una trattativa.

> [!NOTE]
> Non è necessario attendere il completamento dell'elaborazione. I dettagli dell'ultimo file elaborato saranno disponibili per il download al termine dell'elaborazione. **Se si caricano file con 1000 record, possono essere necessari fino a 10 minuti.**

> [!IMPORTANT]
> Leggere attentamente tutte le istruzioni e controllare il formato di ogni colonna dalla tabella seguente prima di creare o aggiornare offerte usando file CSV in Partner Center.

|**Nome colonna**|**È obbligatorio?**|**Descrizione**|**Valori di esempio**|
|-----|:-----|:---------|:---|
Errors|No|Eventuali errori correlati alle operazioni di creazione/aggiornamento w.r.t alle segnalazioni verranno inclusi in questa colonna. Se sono presenti più errori, verranno elencati tutti separati da un punto e virgola.|Campo obbligatorio Soluzione 1 mancante|
Engagement ID|No|L'ID engagement viene generato dal sistema di segnalazione del Centro per i partner Microsoft. Non obbligatorio per la creazione di nuove segnalazioni. È possibile usare l'ID engagement esistente se si aggiorna un record.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID di riferimento|No|L'ID segnalazione viene generato dal sistema di segnalazione del Centro per i partner Microsoft. Non obbligatorio per la creazione di nuove segnalazioni. Compilarlo con l'ID segnalazione se si sta aggiornando un record esistente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nome dell'offerta|Sì|Nome descrittivo dell'offerta per il riferimento.|Accordo di primavera nel Regno Unito
Nome del cliente|Sì|Nome della società del cliente. Usare il nome legale dell'organizzazione per la corrispondenza rapida sul lato Microsoft.|Contoso Corporation
Riga indirizzo cliente 1|Sì|Indirizzo 1 della società del cliente. |One Contoso Way
Riga indirizzo cliente 2|No|Indirizzo 2 della società del cliente.|NE 148 street
Città del cliente|Sì|Città in cui si trova l'organizzazione del cliente.|Redmond
Customer State|No|Stato in cui si trova l'organizzazione del cliente.|Washington
Customer Postal Code|No|Codice postale dell'area in cui si trova l'organizzazione del cliente.|98052
Customer Country|Sì|Paese/area geografica in cui si trova l'organizzazione del cliente. Usare i codici paese di due lettere come indicato [qui.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|US
ID cliente D-U-N-S|No|Provare a recuperare l'ID DUNS dell'organizzazione del cliente. Ciò consente di velocizzare la corrispondenza dell'organizzazione del cliente sul lato Microsoft, in modo da velocizzare l'assegnazione del venditore. È possibile ottenere GRATUITAMENTE l'ID DUNS da questo [sito Web.](https://www.dnb.com/duns-number/lookup.html)|81466849
Nome del contatto del cliente|Dipende da|Il nome è obbligatorio solo se è necessaria la Guida Microsoft. Nome del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|John
Cognome contatto cliente|Dipende da|Il cognome è obbligatorio solo se è necessaria la Guida Microsoft. Cognome del contatto principale dell'organizzazione del cliente che sta lavorando a questa trattativa.|Cliente
Numero di telefono del contatto del cliente|Dipende da|Il numero di telefono è obbligatorio solo se è necessaria la Guida Microsoft. Numero di telefono del contatto principale dell'organizzazione del cliente che lavora a questa trattativa.|9999999999
Indirizzo di posta elettronica del contatto del cliente|Dipende da|L'indirizzo di posta elettronica è obbligatorio solo se è necessaria assistenza Microsoft. Indirizzo di posta elettronica del contatto principale dell'organizzazione del cliente che sta lavorando a questa trattativa.|john.customer@contoso.com
Stato segnalazione partner|Sì|Indica lo stato dell'offerta dal punto di vista dell'azienda. Obbligatorio se si tenta di creare o modificare una segnalazione. Usare **Nuovo** se si sta tentando di creare un nuovo accordo. I valori accettati sono documentati [qui.](/partner/develop/referral-resources#referralstatus)|Attivo
Stato secondario segnalazione partner|Sì|Indica lo stato esatto dell'operazione. Usare **Accettato** se si sta tentando di creare un nuovo accordo. È necessario anche se si modifica una segnalazione esistente. I valori accettati sono documentati [qui.](/partner/develop/referral-resources#referralsubstatus)|Accettato
Stato segnalazione Microsoft|Dipende da|Indica lo stato della richiesta di co-selling inviata a Microsoft per richiedere assistenza. Questo è un campo di sola lettura. Qualsiasi modifica apportata a questo campo durante l'importazione dei dati verrà ignorata.| In sospeso
Motivo rifiutato/perso|Dipende da| È necessario fornire queste informazioni solo se si modifica lo stato secondario del campo in Rifiutato o Perso. In caso contrario, è possibile ignorare questa colonna. <br/> **Immettere un numero in base alle opzioni seguenti** <br/><br/> **1**- Il budget del progetto non è adeguato  <br/> **2**- Il cliente non ha risposto  <br/> **3**- Il cliente ha scelto un altro fornitore  <br/> **4** - Requisito del cliente non soddisfatto  <br/> **5** - Non un cliente <br/> **6**- Linea temporale proposta troppo breve <br/> **7** - Segnalare abusi, spam o phishing <br/> **8** - Altri |6|
Sales Stage|No|Questo è il campo per indicare la fase di vendita dettagliata della segnalazione. Per altre informazioni sulle fasi di vendita, [vedere qui](./manage-co-sell-opportunities.md)|40
Valore stimato della trattativa|Sì|Valore della trattativa in base alle conversazioni iniziali con il cliente. Questo può essere modificato fino a quando la trattativa non raggiunge uno degli stati terminali **vinti** o **persi.**|12563
Valuta|Sì|Valuta in cui viene immesso il valore dell'operazione. I codici valuta sono disponibili [qui.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Data di chiusura stimata|Sì|Data di chiusura stimata dell'accordo in base alle conversazioni iniziali con il cliente nel formato MM/GG/AAAA. <br/> **La data deve essere nel fuso orario UTC. Tutte le date visualizzate nell'interfaccia Partner Center sono basate sui fusi orario localizzati. Potrebbe esserci una differenza di +/- un giorno nell'interfaccia utente di Partner Center se si sta esaminando la segnalazione per cui è stata specificata la data nel fuso orario UTC.**|1/30/2020
CRM ID|No|Identificatore di questa segnalazione specifica nel sistema CRM, se presente. Si tratta di un campo di immissione di testo in formato libero.|34234324-sdfsdf-345345-sfd
ID campagna di marketing|No|Questo campo indica la campagna di marketing, che ha determinato questa segnalazione specifica. Usato in genere per il calcolo del ROI|BingSummer2020
Note|No|Note dettagliate che indicano gli aggiornamenti correlati alla segnalazione|Si tratta di una nota di esempio
È necessaria la Guida Microsoft?|Sì|Indica se si vuole che Microsoft sia utile per effettuare questa richiesta di co-selling|Sì
Quale aiuto specifico di Microsoft?|Dipende da|Uno dei sei modi in cui Microsoft può essere utile. Questa opzione è applicabile solo se si sceglie Sì per la domanda "Richiesta di assistenza Microsoft? " <br/> **Immettere un numero in base alle opzioni seguenti** <br/><br/> **1**- Carico di lavoro - proposta di valore specifica  <br/> **2**- Architettura tecnica del cliente  <br/> **3**- Modello di verifica /Demo  <br/> **4**- Citazioni e licenze  <br/> **5**- Post - Successo dei clienti delle vendite  <br/> **6**- Generale o altro|1|
Condividere con il team di vendita Microsoft|Sì|Indica se si vogliono condividere o meno i dettagli della trattativa con il team di vendita Microsoft. Questa opzione è applicabile solo se si sceglie No per la domanda "Richiesta di assistenza Microsoft? "|Sì
Note per Microsoft|No|Eventuali note specifiche per Microsoft per ottenere assistenza da Microsoft|Serve aiuto con un modello di acquisto per il cliente Contoso
Consenso per condividere il contatto cliente/partner|Sì|Acconsentire a condividere i dettagli di contatto del cliente e i dati di contatto dei dipendenti aziendali che stanno lavorando alla trattativa. **Le trattative non verranno create o aggiornate se si sceglie No per questa colonna.** |Sì
Soluzione 1|Sì|ID soluzione (obbligatorio), valuta (facoltativa) in cui viene immesso il valore della trattativa. È possibile trovare i codici di [valuta qui,](https://en.wikipedia.org/wiki/ISO_4217)il prezzo dello SKU (facoltativo) e la quantità dello SKU (facoltativo)  |SOL-1234-PQRS, USD, 10, 100
Membro del team 1|Sì|Nome, Cognome, numero di cellulare e ID di posta elettronica del rispettivo membro del team.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Passaggi successivi

È possibile usare questi connettori Partner Center co-selling per co-selling con Microsoft dall'interno dei sistemi CRM.

- [Connettore di co-selling per Dynamics 365 CRM - Panoramica](connector-dynamics.md)
- [Connettore di co-selling per CRM Salesforce - Panoramica](connector-salesforce.md)
