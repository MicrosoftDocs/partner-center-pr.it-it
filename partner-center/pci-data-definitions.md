---
title: Definizioni dei dati di Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Il documento fornisce l'elenco dei vari report e le definizioni dei dati di ogni report, che possono essere scaricati dalla pagina del report di download di Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501749"
---
# <a name="export--data-definitions"></a>Export-definizioni dei dati 

 **Ruoli appropriati** 

- Visualizzatore di report 
- Visualizzatore di report esecutivi 

## <a name="introduction"></a>Introduzione 

L'hub Download Reports nel dashboard Insights consente di esportare i set di dati non elaborati.  

I vari report, che possono essere scaricati insieme alla definizione dei dati, sono i seguenti: 

**Profilo partner**: le definizioni dei dati dei diversi campi del report del profilo sono: 


| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|MPNId|ID Microsoft Partner Network|
|PartnerName|Nome del partner |
|PGA_MPNId|ID MPN dell'account globale partner|
|PGA_PartnerName|Nome dell'account globale del partner|
|City|Località della città del partner |
|Paese|Località del paese del partner |
|Livello gerarchia|Indica se si tratta di un ID MPN globale o di un ID MPN della località|

**Dettagli cliente**: le definizioni dei dati dei diversi campi del report Dettagli cliente sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerName|Nome del cliente |
|CustomerTenantId|ID tenant del cliente |
|CustomerTpid|Identificatore padre principale del cliente |
|CustomerSegment|Segmento Customer |
|CustomerMarket|Mercato geografico del cliente  |
|CustomerStatus|Stato del cliente (/inactive attivo) |
|Prodotto|Prodotto venduto al cliente dal MPN. Si tratta di uno dei O365, d365, Enterprise Mobility, Power BI Microsoft Azure.|
|SKU|   SKU di prodotto|
|Month| Mese per cui viene segnalato l'utilizzo e i ricavi|
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Nome del partner|
|PartnerLocation|   Posizione geografica del partner|
|PartnerAttributionType|    Tipo di attribuzione del partner|
|SalesChannel|  Sales Channel|
|AvailableSeats|    Postazioni disponibili| 
|RevenueUSD|    Ricavi in USD|

**Prestazioni rivenditore**: le definizioni dei dati dei diversi campi dei report sulle prestazioni dei rivenditori sono:

> [!Note]
> I dati ricavi e ACR sono disponibili solo per gli utenti che sono visualizzatori di report esecutivi.

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|ResellerMpnid|Identificatore Microsoft Partner Network rivenditore| 
|ResellerName|Reseller Name|
|ResellerMarket|Paese rivenditore del mercato| 
|IndirectProviderMPNId|Identificatore Microsoft Partner Network provider indiretto|
|IndirectProviderName|Nome provider indiretto|
|Month|Mese per cui viene segnalato l'utilizzo e i ricavi|
|Prodotto|Nome prodotto|
|SubscriptionID|Identificatore sottoscrizione|
|AvailableSeats|Numero di postazioni disponibili|
|AssignedSeats|Numero di postazioni assegnate|
|BilledRevenueUSD|Ricavi fatturati (in $)|
|CustomerName|Nome del cliente| 
|CustomerTPid|Identificatore padre principale del cliente| 
|CustomerSegment|Segmento Customer |
|CustomerMarket|Mercato geografico del cliente |
|ResellerStatus|Stato rivenditore| 

**Dettagli sottoscrizioni**: le definizioni dei dati dei diversi campi del report Dettagli sottoscrizione sono:

>[!Note]
>I dati ricavi e ACR sono disponibili solo per gli utenti che sono visualizzatori di report Executive

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|SubscriptionId|    GUID della sottoscrizione|
|SubscriptionStartDate| Data di inizio della sottoscrizione|
|SubscriptionEndDate|   Data di fine della sottoscrizione|
|SubscriptionState| Stato della sottoscrizione (attiva o con varianza)|
|Month| Mese per cui viene segnalato l'utilizzo e i ricavi|
|IsAutoRenew|   Indica se la sottoscrizione è a rinnovo automatico (Y/N)|
|CustomerName|  Nome del cliente| 
|CustomerTenantId|  GUID cliente|
|CustomerTpid|  Identificatore padre principale del cliente| 
|CustomerSegment|   Segmento di mercato del cliente| 
|CustomerMarket|    Mercato geografico del cliente|
|Prodotto|   Prodotto venduto al cliente dal partner| 
|SKU|   SKU del prodotto |
|MPNId| ID Microsoft Partner Network del partner |
|PartnerName|   Nome del partner |
|PartnerLocation|   Posizione geografica del partner |
|PartnerAttributionType|    Tipo di attribuzione per la sottoscrizione|
|SalesChannel|  Canale delle vendite (Direct/CSP e così via) |
|AvailableSeats|    Postazione disponibile corrente|
|RevenueUSD|    Ricavi in USD|
|ID registrazione| ID di registrazione della sottoscrizione|

**Azure Usage**: le definizioni dei dati dei diversi campi del report utilizzo di Azure sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|SubscriptionId|    GUID della sottoscrizione|
|SubscriptionStartDate| Data di inizio della sottoscrizione.|
|SubscriptionEndDate|   Data di fine della sottoscrizione.|
|SubscriptionState| Stato corrente della sottoscrizione (periodo di apertura/chiusura/attivo/intolleranza)|
|Month| Data aggregata per mese |
|ServiceName|   Nome del servizio di Azure|
|MeterCategory| Nome della categoria del contatore|
|UsageUnits|    Il numero di unità usate durante il ciclo di fatturazione |
|CustomerName|  Nome del cliente |
|CustomerTenantId|  ID tenant del cliente |
|CustomerTpid|  ID principale del cliente |
|CustomerSegment|   Segmento del cliente |
|CustomerMarket|    Mercato geografico del cliente |
|MPNId  |ID Microsoft Partner Network del cliente |
|PartnerName|   Nome del partner |
|PartnerLocation    |Posizione geografica del partner |
|PartnerAttributionType |Tipo di attribuzione del partner|
|SalesChannel|  Canale delle vendite (diretto/CSP indiretto/CSP diretto e così via) |
|ACR_USD|   Ricavi usati da Azure in USD|
|ID registrazione| ID di registrazione della sottoscrizione di Azure|

**Office 365-uso della licenza**: le definizioni dei dati dei diversi campi del report di utilizzo delle licenze di Office 365:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerTenantId|  ID tenant del cliente| 
|CustomerTpid|  ID principale del cliente |
|Carico di lavoro|  SFB, teams, EXO |
|Month| Mese per cui viene segnalato l'utilizzo|
|PaidAvailableUnits|    Numero di unità a pagamento disponibili|
|MonthlyActiveUsers|    Numero di utenti attivi mensili|
|CustomerName|  Nome del cliente|
|CustomerMarket|    Area geografica del mercato del cliente |
|CustomerSegment|   Segmento Customer |
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Nome del partner|
|PartnerLocation|   Posizione geografica del partner|
|PartnerAttributionType|    Tipo di attribuzione del partner|

**Enterprise Mobility-uso della licenza**: la definizione dei dati dei diversi campi del report EMS – Usage License è la seguente:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerTenantId|  ID tenant del cliente| 
|CustomerTpid|  ID principale del cliente |
|Carico di lavoro|  Nome del carico di lavoro EMS |
|Month| Mese per cui viene segnalato l'utilizzo|
|PaidAvailableUnits|    Numero di unità a pagamento disponibili|
|MonthlyActiveUsers|    Numero di utenti attivi mensili|
|CustomerName|  Nome del cliente|
|CustomerMarket|Area geografica del mercato del cliente |
|CustomerSegment|   Segmento Customer |
|MPNId| ID Microsoft Partner Network|
|PartnerName|   Nome del partner|
|PartnerLocation|   Posizione geografica del partner|
|PartnerAttributionType|    Tipo di attribuzione del partner|

**Dynamics 365 – uso della licenza**: la definizione dei dati dei diversi campi del report Dynamics 365 – Usage License è:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|SubscriptionId|GUID della sottoscrizione|
|SubscriptionStartDate| Data di inizio della sottoscrizione|
|SubscriptionEndDate|   Data di fine della sottoscrizione|
|SubscriptionStatus|    Stato della sottoscrizione |
|Month| Mese per cui viene segnalato l'utilizzo|
|RevSumDivisionName|    Nome della divisione Rev Sum|
|RevSumCategoryName|    Nome della categoria Rev Sum|
|SKU|   SKU del prodotto |
|SKUId| ID SKU del prodotto |
|FreeVsPaidSKU| Indica se si tratta di uno SKU gratuito o a pagamento |
|SalesModel|    Canale di vendita usato per la vendita della sottoscrizione|
|DetailedSalesModel|    Modello di vendita dettagliato per la sottoscrizione|
|CustomerName|  Nome del cliente |
|CustomerTenantId|  GUID del tenant del cliente |
|CustomerTpid|  Identificatore padre principale del cliente |
|CustomerSegment|   Segmento di mercato del cliente |
|CustomerMarket|    Mercato geografico del cliente |
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Nome del partner |
|PartnerLocation|   Posizione geografica del partner |
|PartnerAttachType| Tipo di attribuzione per la sottoscrizione|
|AvailableSeats|    Postazione disponibile corrente|
|AssignedSeats| Sede assegnata corrente |
|ActiveSeats|   Postazioni attive correnti |
|DeploymentOpportunity| Opportunità di distribuzione corrente|
|ActiveUsagePercent|    Percentuale utilizzo attivo corrente|
 
**Power bi uso della licenza**: la definizione dei dati dei diversi campi del report di utilizzo delle licenze Power bi:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|SubscriptionId|    GUID della sottoscrizione|
|SubscriptionStartDate| Data di inizio della sottoscrizione|
|SubscriptionEndDate|   Data di fine della sottoscrizione|
|SubscriptionStatus|    Stato della sottoscrizione (periodo attivo o In-Active o in-Grace)|
|Month| Data aggregata per mese |
|SKU|   SKU del prodotto |
|SKUId| ID SKU del prodotto |
|FreeVsPaidSKU| Differenziatore SKU gratuito o a pagamento |
|SalesModel|    Modello Sales usato per vendere la sottoscrizione|
|DetailedSalesModel|    Modello di vendita dettagliato per la sottoscrizione|
|CustomerName|  Nome del cliente |
|CustomerTenantId|  GUID del tenant del cliente |
|CustomerTpid|  Identificatore padre principale del cliente| 
|CustomerSegment|   Segmento di mercato del cliente |
|CustomerMarket|    Mercato geografico del cliente |
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Nome del partner |
|PartnerLocation|   Posizione geografica del partner |
|PartnerAttachType| Tipo di attribuzione per la sottoscrizione|
|AvailableSeats|    Postazioni disponibili correnti|
|AssignedSeats| Postazioni assegnate correnti|
|ActiveSeats|   Postazioni attive correnti|
|DeploymentOpportunity| Opportunità di distribuzione corrente|
|ActiveUsagePercent|    Percentuale utilizzo attivo corrente|

**Utilizzo dei team-riunioni e chiamate**: le definizioni dei dati dei diversi campi sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerTenantId|  ID tenant del cliente |
|CustomerTpid|  ID principale del cliente |
|Month| Mese per cui viene segnalato l'utilizzo|
|Sottocarico di lavoro|   Carico di lavoro secondario per il quale viene segnalato l'utilizzo (riunioni, chiamate, sistemi telefonici)|
|Conteggio riunioni| Numero di riunioni|
|Durata della riunione|  Durata totale riunione in ore|

**Teams-dettagli sull'utilizzo mensile**: le definizioni dei dati dei diversi campi sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerTenantId|  ID tenant del cliente |
|CustomerTpid|  ID principale del cliente |
|Month| Mese per cui viene segnalato l'utilizzo|
|Sottocarico di lavoro|   Carico di lavoro secondario per il quale viene segnalato l'utilizzo (riunioni, chiamate, sistemi telefonici)|
|Utenti desktop| Numero di utenti che usano i team sul desktop|
|Utenti mobili|  Numero di utenti che usano i team in dispositivi mobili|
|Utenti Web| Numero di utenti che usano i team sul Web|
|AllUpParticipants| Numero di utenti distinti di team per il mese|

**Uso dei team-app 3P**: le definizioni dei dati dei diversi campi sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|CustomerTenantId|  ID tenant del cliente| 
|CustomerTpid|  ID principale del cliente |
|Month| Mese per cui viene segnalato l'utilizzo|
|Nome dell'app 3P|   Nome dell'app Teams|
|Numero utenti|    Numero di utenti per l'app|


**Dettagli di training**: le definizioni dei dati dei diversi campi del report dettagli di training sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|TrainingActivityId|    Identificatore del training |
|TrainingTitle| Titolo della formazione |
|TrainingType|  Tipo di training (certificazione/esame)|
|IndividualFirstName|   Nome del cliente| 
|IndividualLastName|    Cognome del cliente| 
|E-mail| ID di posta elettronica personale del cliente|
|CorpEmail| ID di posta elettronica dell'ufficio del cliente|
|TrainingCompletionDate|    Data di completamento del training |
|Month| Mese per cui vengono segnalati i dati|
|IcMCP| Indica se l'utente è Microsoft Certified Professional|
|MCPID| ID MCP dell'utente|
|MPNId| ID Microsoft Partner Network |
|PartnerName|   Nome del partner |
|PartnerCityLocation|   Posizione geografica della città del partner |
|PartnerCountryLocation|    Posizione geografica del partner |

**Microsoft Learn**: le definizioni dei dati dei diversi campi del report Microsoft Learn sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|Nome utente|Nome dell'utente| 
|UserId|GUID utente |
|Trainingname|Nome del training |
|TrainingType|Tipo di training (percorso/Learning del modulo)|
|Prodotti|Prodotto per cui è applicabile il modulo Learning|
|Ruoli|Ruoli applicabili del training |
|CompletionDate|Data di completamento del training |
|MPNId|ID Microsoft Partner Network |
|PartnerName|Nome del partner |
|Paese|Posizione geografica del partner |

**Riepilogo e cronologia delle competenze**: la definizione dei dati dei diversi campi del report di riepilogo delle competenze e della cronologia è la seguente:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|Competenzaname|Nome della competenza |
|CompetencyLevel|Livello di competenza (Gold/Silver)|
|CompetencyStatus|Stato corrente della competenza (attivo/inattivo/nel periodo di tolleranza)|
|CompetencyStartDate|Data di inizio della competenza specificata| 
|CompetencyEndDate|Data di fine della competenza specificata |

**Prestazioni delle competenze**: le definizioni dei dati dei diversi campi del report sulle prestazioni delle competenze sono:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|Competenzaname|    Nome della competenza |
|CompetencyAttainmentOptionName|    Nome dell'opzione di raggiungimento delle competenze|
|Month| Mese per cui vengono segnalate le metriche|
|MetricName|    Nome della metrica pertinente per la competenza|
|MetricMonthlyContribution| Contributo mensile della metrica|
|TTMAggregate|  Metrica aggregata per i 12 mesi finali|
|AnniversaryYearAggregate|  Metrica aggregata per l'anno di anniversario corrente|
|GoldThreshold| Requisiti di prestazioni per soddisfare le competenze Gold|
|SilverThreshold|   Requisiti di prestazioni per soddisfare le competenze Silver|

**Scalabilità del cloud-M365 propensiity**: le definizioni dei dati dei diversi campi del report di propensanza M365 del cloud:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Nome partner|  Nome del partner|
|Customer ID|   Numero Identificativo cliente |
|Numero DUNS|   Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione|
|Nome account|  Nome dell'account |
|Dominio|    Dominio dell'account|
|Dimensioni dell'organizzazione|  Dimensioni dell'organizzazione|
|Settore|  Settore  |
|Vertical|  Verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft e da altri standard del settore (D&B)|
|Area|  Area geografica della località|
|Affiliata|    La filiale del cliente a cui viene assegnato il punteggio per la propensione|
|Area di vendita|   Territorio di vendita del cliente per cui è stato eseguito il punteggio per la propensione|
|City|  Posizione geografica della città |
|State| Posizione dello stato geografico|
|CAP|   CAP|
|Paese|   Posizione geografica del paese |
|Segment|   Segmento di mercato |
|Segmento secondario|   Segmento secondario Market |
|Riepilogo del tipo SMC|  Tipo SMC |
|Top non gestito-base di calcolo|  Clienti non gestiti principali-calcolo|
|Base utente non gestita principale| Clienti non gestiti principali-utente|
|IsNonProfit|   Se non profit o profit (Yes/No)|
|Abilita Exchange Online per la destinazione di lavoro|   Clienti con una sottoscrizione di Exchange Online attiva, da vendere a M365|
|Abilitare l'acquisizione di lavoro locale (versione corrente) con CLAS propensiity-+ 10 licenses|Cliente che dispone di una sede locale o di un client Win, ovvero versioni successive ai prodotti EOS. Il cliente dispone di 10 o più licenze. Cliente con punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilitare l'acquisizione di lavoro locale (versione corrente) con CLAS propensiity-<10 licenze|Cliente che dispone di una sede locale o di un client Win, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 10 licenze. Cliente con punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilita l'acquisizione di lavoro in locale (versione corrente) senza la propensità CLAS-+ 10 licenze| Cliente che dispone di una sede locale o di un client Win, ovvero versioni successive ai prodotti EOS. Il cliente dispone di 10 o più licenze. Il cliente non ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilitare l'acquisizione di lavoro in locale (versione corrente) senza la propensità CLAS-<10 licenze| Cliente che dispone di una sede locale o di un client Win, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilita l'acquisizione di lavoro locale (EOS) remota con CLAS propensiity-+ 10 licenze|Cliente che dispone di un client o di un client Premium EOS (ovvero versioni precedenti a e inclusi i prodotti EOS). Il cliente dispone di 10 o più licenze. Il cliente ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilitare l'acquisizione di lavoro locale (EOS) remota con CLAS propensiity-<10 licenze|Cliente che dispone di un client o di un client Premium EOS (ovvero versioni precedenti a e inclusi i prodotti EOS). Il cliente ha meno di 10 licenze. Il cliente ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilita l'acquisizione di lavoro locale (EOS) remota senza la propensanza CLAS-+ 10 licenze| Cliente che dispone di una sede locale o di un client Win, ovvero versioni precedenti e inclusi i prodotti EOS. Il cliente dispone di 10 o più licenze. Il cliente non ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilitare l'acquisizione di lavoro locale (EOS) remota senza la propensità di CLAS-<10 licenze| Cliente che dispone di una sede locale o di un client Win, ovvero versioni precedenti e inclusi i prodotti EOS. Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. I partner devono essere destinati alla conversione in M365.|
|Abilita lavoro remoto-prospettiva di propensione elevata per M365 (Act Now/Evaluate)| Prospect Customer con elevata propensione per M365.|
|Abilita lavoro remoto-competi (zoom) con M365| Clienti con zoom e M365, destinazione per la conversione ai team|
|Abilita lavoro remoto-competi (zoom) senza M365|  Clienti con zoom, destinazione per la conversione ai team|
|Riduzione dei costi e della gestione-M365 E3 destinati a M365 E5| Customer esistente con M365 E3, target per M365 E5|
|Ridurre i costi e gestire i clienti M365 BB e BS destinati a M365 BP|    Clienti M365 BB e BS esistenti per M365 BP|
|Trasformare la produttività organizzativa-propensità della superficie|    Il cliente Mostra la propensione per Surface.|
|M365Cluster|Identifica la propensità del cliente per l'acquisto di M365.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|M365Fit|   Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|M365Intent|    I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|SurfaceCluster|    In questo modo si identifica la propensità del cliente per l'acquisto di superficie consolidando le raccomandazioni Fit e Intent in un cluster.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|SurfaceFit|    Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|SurfaceIntent| I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|O365Cluster|   Questo identifica la propensità del cliente per l'acquisto di O365.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|O365Fit|   Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|O365Intent|    I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|M365UpsellCustomer|    Indica se il cliente Visualizza la propensione per M365|
|Con Google|    Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti Google posseduti|
|Con AWS|   Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti AWS proprietari|
|Con EA|    Indica se un rinnovo è un contratto Enterprise Agreement (EA) o una sottoscrizione EA|
|Con apertura|  Indica se un rinnovo è un contratto Open o Open Value|

**Scalabilità del cloud-d365 propensiity**: le definizioni dei dati dei diversi campi del report di propensanza d365 del cloud:

| **Nome colonna** | **Descrizione dati** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Nome partner|  Nome del partner|
|Customer ID|   Numero Identificativo cliente |
|Numero DUNS|   Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione|
|Nome account|  Nome dell'account |
|Dominio|    Dominio dell'account|
|Dimensioni dell'organizzazione|  Dimensioni dell'organizzazione|
|Settore|  Settore  |
|Vertical|  Verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft e da altri standard del settore (D&B)
|Area|  Area geografica della località|
|Affiliata|    La filiale del cliente a cui viene assegnato il punteggio per la propensione|
|Area di vendita|   Area di vendita|
|City|  Posizione geografica della città |
|State| Posizione dello stato geografico|
|CAP|   CAP|
|Paese|   Posizione geografica del paese |
|Segment|   Segmento di mercato |
|Segmento secondario|   Segmento secondario Market |
|Riepilogo del tipo SMC|  La categorizzazione di un cliente: le principali basi utente non gestite sono i clienti con 300 dipendenti, la base di calcolo non gestita più elevata è costituita dai clienti con $10.000 in Azure 3 year potenziali, le aziende di medie dimensioni sono clienti con 25 dipendenti o superiore, le piccole imprese sono clienti con meno di 25 dipendenti|
|Top non gestito-base di calcolo   |Clienti non gestiti principali-calcolo|
|Base utente non gestita principale| Clienti non gestiti principali: utenti|
|IsNonProfit|   Se non profit o profit (Yes/No)|
|Activate Digital selling-M365-Seat size >= 25 postazioni (modello di propensione SalesPro)|   Cliente senza d365. Dimensioni postazione: 25 +. I partner devono essere destinati a cross-selling di d365 SalesPro|
|Attivare la vendita digitale-d365 SalesPro Propensity (Act Now/Evaluate) |Clienti ad alta propensione senza d365.  I partner devono avere come destinazione d365 SalesPro.|
|Gestione dei rischi finanziari & frode-Dynamics on-premi install base-Navision (modello di propensione BC)|Cliente esistente con OnPrem Navision.  Il partner deve essere destinato a d365 BC|
|Gestione dei rischi finanziari & frode-Dynamics on-premi install base-AX (F&O modello di propensione)    |Cliente esistente con OnPrem AX.  Il partner deve essere destinato a d365 F&O|
|Gestione dei rischi finanziari & frode-Dynamics on-premi install base-Plain Plains (modello di propensione BC)|  Cliente esistente con una grande pianura.  Il partner deve essere destinato a d365 BC|
|Gestione dei rischi finanziari & frode-Dynamics on-premi install base-Solomon (modello di propensione BC)|Cliente esistente con OnPrem Solomon.  Il partner deve essere destinato a d365 BC|
|Gestione dei rischi finanziari & frode: base di installazione di Dynamics locale-altri (modello di propensione BC) |Cliente esistente con altre soluzioni locali non elencate in precedenza.  Il partner deve essere destinato a d365 BC|
|Creazione di processi di business agile-Dynamics on-premi install base-AX/GP/SL/NAV/other (modello di propensione d365)|   Creazione di processi di business agile-Dynamics on-premi install base-AX/GP/SL/NAV/other (modello di propensione d365)|
|Creazione di processi di business agile-Dynamics compete base-mendix/Outsystems/Salesforce (modello di propensione d365)| Creazione di processi di business agile-Dynamics compete base-mendix/Outsystems/Salesforce (modello di propensione d365)|
|Creazione di processi di business agile-d365 F&O install base |Clienti d365 F&O esistenti.  Partner per le app Power Apps.|
|Creazione di processi di business agile-d365 BC install base| Clienti d365 BC esistenti. Partner per le app Power Apps.|
|Creazione di processi di business agile-d365 CE install base| Clienti esistenti di d365 CE. Partner per le app Power Apps.|
|Creazione di una catena di approvvigionamento resiliente: vincere e attivare il primo carico di lavoro d365 come supply chain di d365 con clienti non Oracle/SAP ERP|  Clienti di destinazione per la supply chain d365.|
|Creazione di una catena di fornitura resiliente, cross-sell d365 supply chain e/o vendite al dettaglio/commerciale ai clienti d365 CE esistenti |Clienti esistenti di d365 CE a destinazione per la supply chain di cross-selling d365|
|Creazione di una catena di alimentazione resiliente: cross-sell d365 sup. Chain e/o retail/commerce per d365 CE e (Oracle o SAP)| Clienti esistenti di d365 CE con Oracle o SAP come destinazione per la supply chain di d365|
|D365BCCluster| Questo identifica la propensità del cliente per l'acquisto di d365 business Central.  I clienti che mostrano la propensità per BC si troveranno nella categoria media e piccola.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|D365BCFit| Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|D365BCIntent|  I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|D365FOCluster| Questo identifica la propensità del cliente per l'acquisto di operazioni e finanza d365.  I clienti che mostrano la propensità per F&O si troveranno nelle categorie non gestite principali. I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|D365FOFit| Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|D365FOIntent|  I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|D365CECluster| Questo identifica la propensità del cliente per l'acquisto del coinvolgimento del cliente d365.  I clienti che mostrano la propensione per la CE saranno nelle categorie media e piccola.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|D365CEFit| Adatta per d365 CE|
|D365CEIntent|  Finalità per d365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Questa operazione identifica se un cliente ha un rinnovo aperto per Dynamics locale AX o CRM.|
|M365UpsellCustomer|    Indica se il cliente Visualizza la propensione per M365|
|Con Google|    Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti Google posseduti|
|Con AWS|   Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti AWS proprietari|
|Con EA |Indica se un rinnovo è un contratto Enterprise Agreement (EA) o una sottoscrizione EA|
|Con apertura|  Indica se un rinnovo è un contratto Open o Open Value|

**Propensity Ascent-Azure cloud**: le definizioni dei dati dei diversi campi del report di propensione Ascent-Azure cloud sono:

|**Nome colonna** |**Descrizione dati** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Nome partner|  Nome del partner|
|Customer ID|   Numero Identificativo cliente |
|Numero DUNS|   Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione|
|Nome account|  Nome dell'account |
|Dominio|    Dominio dell'account|
|Dimensioni dell'organizzazione|  Dimensioni dell'organizzazione|
|Settore|  Settore  |
|Vertical|  Verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft e da altri standard del settore (D&B)|
|Area|  Area geografica della località|
|Affiliata|    La filiale del cliente a cui viene assegnato il punteggio per la propensione|
|Area di vendita|   Area di vendita|
|City|  Posizione geografica della città |
|State| Posizione dello stato geografico|
|CAP|   CAP|
|Paese|   Posizione geografica del paese |
|Segment|   Segmento di mercato |
|Segmento secondario|   Segmento secondario Market |
|Riepilogo del tipo SMC|  Tipo SMC |
|Top non gestito-base di calcolo|  Clienti non gestiti principali-calcolo|
|Base utente non gestita principale| Clienti non gestiti principali: utenti|
|IsNonProfit|   Se non profit o profit (Yes/No)|
|Migrate-EOS Win Server-EOS Windows Server IB con CLAS propensiity-5 + licenze|   Cliente che dispone di EOS Server Win locale (ovvero versioni precedenti a e inclusi i prodotti EOS). Il cliente dispone di 5 o più licenze. Cliente con punteggio di propensione.  I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB con CLAS propensiity-<5 licenze|   Cliente con EOS (End of Service) il server Win locale (ovvero versioni precedenti a e inclusi i prodotti EOS). Il cliente ha meno di 5 licenze. Cliente con punteggio di propensione.  I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB senza CLAS propensiity-5 + licenze |Cliente che dispone di EOS Server Win locale (ovvero versioni precedenti a e inclusi i prodotti EOS). Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB senza CLAS propensiity-<5 licenze|    Cliente che dispone di EOS Server Win locale (ovvero versioni precedenti a e inclusi i prodotti EOS). Dispone di meno di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS SQL-EOS SQL Server IB con CLAS propensiity-5 + licenze|  Cliente con EOS locale SQL Server, ovvero versioni precedenti a e inclusi i prodotti EOS. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione.  I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS SQL-EOS SQL Server IB con CLAS propensiity-<5 licenze|  Cliente con EOS locale SQL Server, ovvero versioni precedenti a e inclusi i prodotti EOS. Dispone di meno di 5 licenze. Cliente con punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione-EOS SQL-EOS SQL Server IB senza le licenze CLAS propensiity-5 +|   Cliente con EOS locale SQL Server, ovvero versioni precedenti a e inclusi i prodotti EOS. Il cliente dispone di 5 o più licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-EOS SQL-EOS SQL Server IB senza CLAS propensiity-<5 licenze|   Cliente con EOS locale SQL Server, ovvero versioni precedenti a e inclusi i prodotti EOS. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione di un server Win locale-Windows Server corrente IB con CLAS propensiity-5 + licenze|   Cliente con Server Win locale corrente, ovvero versioni successive ai prodotti EOS. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione del server Win locale-Windows Server corrente IB con CLAS propensiity-<5 licenze|   Cliente con Server Win locale corrente, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione per Azure. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione di un server Win locale con Windows Server IB corrente senza CLAS propensiity-5 + licenze|    Cliente con Server Win locale corrente, ovvero versioni successive ai prodotti EOS. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione del server Win locale-Windows Server corrente IB senza CLAS propensiity-<5 licenze |Cliente con Server Win locale corrente, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL-Current SQL Server IB con CLAS propensiity-5 + licenses|  Cliente che ha SQL Server locali correnti, ovvero versioni successive ai prodotti EOS. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL-Current SQL Server IB con CLAS propensiity-<5 licenses|  Cliente che ha SQL Server locali correnti, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL-Current SQL Server IB senza CLAS propensiity-5 + licenses|   Cliente che ha SQL Server locali correnti, ovvero versioni successive ai prodotti EOS. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrare: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL-Current SQL Server IB senza CLAS propensiity-<5 licenze|   Cliente che ha SQL Server locali correnti, ovvero versioni successive ai prodotti EOS. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione-OSS-migrate al database OSS| Cliente esistente con uno dei prodotti di concorrenza seguenti: PostgreSQL, MySQL, MariaDB. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione-OSS-Linux in Azure |Cliente esistente con il prodotto: Linux. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione di SAP-SAP in Azure|  Cliente esistente con il prodotto: SAP. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Migrate-WVD-RDS IB |Identifica i clienti con Servizi Desktop remoto Windows attive. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione di WVD-cross sell Modern work in Azure/WVD|   Identifica i clienti con M365 e non dispone di Azure. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione-VMware IB|   Cliente esistente con il prodotto: VMware. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Eseguire la migrazione-Citrix IB|   Cliente esistente con il prodotto: sistemi Citrix. I partner devono avere come destinazione questi clienti per la migrazione ad Azure.|
|Innovazione-Analytics-Power BI IB w/elevata propensione di Azure|   Clienti con una sottoscrizione Active Power BI inclusa: Power BI-standalone Pro, Power BI-Suite di Azure, Power BI-Suite di Office, Power BI Suites-M365|
|Enable-DevOps con GitHub-VisualStudio/MSDN IB|    Clienti identificati con Visual Studio attivi|
|Versione di Win Server standard|   Viene visualizzata la versione di acquisti standard di Windows Server da parte del cliente|
|Licenza Win Server standard|   Viene visualizzato il tipo di licenza degli acquisti standard di Windows Server da parte del cliente|
|Versione di Win Server Data Center|    Viene visualizzata la versione di Windows Data Center acquistata dal cliente|
|Licenza Win Server Data Center| Indica il tipo di licenza degli acquisti di Windows Data Center da parte del cliente|
|AzureFit|  Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti. Il Punteggio Fit viene aggiornato trimestralmente.|
|AzureIntent|   I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese.|
|AzureCluster|  In questo modo si identifica la propensità del cliente per l'acquisto di Azure consolidando le raccomandazioni Fit e Intent in un cluster.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|WindowsServerDataCenter_HasOpenRenewal|    Indica se un cliente ha un rinnovo aperto per Windows Server data center|
|WindowsServerStandard_HasOpenRenewal|  Indica se un cliente ha un rinnovo aperto per Windows Server standard|
|AzureUpsellCustomer|   Indica se il cliente Visualizza la propensione per Azure|
|Con Google|    Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti Google posseduti|
|Con AWS|   Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti AWS proprietari|
|Con EA |Indica se un rinnovo è un contratto Enterprise Agreement (EA) o una sottoscrizione EA|
|Con apertura|  Indica se un rinnovo è un contratto Open o Open Value|

**Propensità dei rinnovi di Ascent-Agreement cloud**: le definizioni dei dati dei diversi campi del report di propensanza dei rinnovi del cloud Ascent-Agreement sono:

|**Nome colonna** |**Descrizione dati** |
|---------|:---------|
|ID MPN|    ID Microsoft Partner Network|
|Nome partner|  Nome del partner|
|Customer ID|   Numero Identificativo cliente |
|Numero DUNS|   Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione|
|Nome account|  Nome dell'account |
|Dominio|    Dominio dell'account|
|Dimensioni dell'organizzazione|  Dimensioni dell'organizzazione|
|Settore|  Settore  |
|Vertical|  Verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft e da altri standard del settore (D&B)|
|Area|  Area geografica della località|
|Affiliata|    La filiale del cliente a cui viene assegnato il punteggio per la propensione|
|Area di vendita|   Area di vendita|
|City|  Posizione geografica della città |
|State| Posizione dello stato geografico|
|CAP|   CAP|
|Paese|   Posizione geografica del paese |
|Segment|   Segmento di mercato |
|Segmento secondario|   Segmento secondario Market |
|Riepilogo del tipo SMC|  Tipo SMC |
|Top non gestito-base di calcolo|  Clienti non gestiti principali-calcolo|
|Base utente non gestita principale| Clienti non gestiti principali: utenti|
|IsNonProfit|Se non profit o profit (Yes/No)|
|Con Google|Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti AWS proprietari|
|Con AWS|Questo flag indica se un cliente Visualizza segnali concorrenziali per i prodotti AWS proprietari|
|Cluster di Azure|Questo identifica la propensità del cliente per l'acquisto di Azure.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|D365 F&O cluster|  Questo identifica la propensità del cliente per l'acquisto di operazioni e finanza d365.  I clienti che mostrano la propensità per F&O si troveranno nelle categorie non gestite principali.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|Cluster d365 CE|   Questo identifica la propensità del cliente per l'acquisto del coinvolgimento del cliente d365.  I clienti che mostrano la propensione per la CE saranno nelle categorie media e piccola.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|Cluster d365 BC|   Questo identifica la propensità del cliente per l'acquisto di d365 business Central.  I clienti che mostrano la propensità per BC si troveranno nella categoria media e piccola.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|Cluster M365|  Questo identifica la propensità del cliente per l'acquisto di M365.  I cluster agiscono ora e la valutazione dovrebbe essere mirata perché produrrà un rendimento superiore.  Coltivare e informare i clienti deve essere destinato solo se è ancora disponibile una capacità dopo la destinazione di Act Now e la valutazione dei clienti.|
|Programma di licenza|   Identifica il tipo di programma di licenza per il rinnovo|
|Agreement ID|  Identificatore del contratto|
|Data di fine contratto|    Data di fine contratto |
|Tipo di scadenza|   Tipo di scadenza|
|Ricavi in scadenza|  Ricavi associati alle sottoscrizioni in scadenza|
|Con EA|    Indica se un rinnovo è un contratto Enterprise Agreement (EA) o una sottoscrizione EA|
|Con apertura|  Indica se un rinnovo è un contratto Open o Open Value|
|Cliente per la vendita di Azure| Indica se il cliente Visualizza la propensione per Azure|
|M365-Vendi cliente|  Indica se il cliente Visualizza la propensione per M365|
|RevSumDivisionName|    Identifica il prodotto che è attivo per il rinnovo|

## <a name="next-steps"></a>Passaggi successivi

Per i report, vedere [scaricare i report](pci-download-reports.md).
