---
title: Definizioni dei dati di Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Il documento elenca i vari report e le relative definizioni dei dati, che è possibile scaricare dalla pagina del report di download di Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861394"
---
# <a name="export--data-definitions"></a>Export-definizioni dei dati 

 **Ruoli appropriati** 

- Visualizzatore di report 
- Visualizzatore di report esecutivi 

## <a name="introduction"></a>Introduzione 

Usando l'hub Download Reports nel dashboard Insights, è possibile esportare i set di dati non elaborati. 

I vari report, che è possibile scaricare insieme alle relative definizioni dei dati, sono elencati nelle tabelle seguenti: 

### <a name="partner-profile-report"></a>**Report profilo partner**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| MPNId | Identificatore di Microsoft Partner Network (MPN) | 
| PartnerName | Nome del partner | 
| PGA_MPNId | Identificatore dell'account globale partner MPN | 
| PGA_PartnerName | Nome dell'account globale del partner | 
| City | Località della città del partner | 
| Paese | Località del paese del partner | 
| Livello gerarchia | Indica se si tratta di un ID MPN globale o di un ID MPN della località | 

### <a name="customer-details-report"></a>**Report Dettagli cliente**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | Identificatore del tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento Customer | 
| CustomerMarket | Mercato geografico del cliente | 
| CustomerStatus | Stato del cliente (attivo o inattivo) | 
| Prodotto | Prodotto venduto al cliente da MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI o Microsoft Azure | 
| SKU | SKU di prodotto | 
| Month | Mese per cui vengono segnalati l'utilizzo e i ricavi | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 
| SalesChannel | Canale di vendita | 
| AvailableSeats | Postazioni disponibili | 
| RevenueUSD | Ricavi in dollari statunitensi | 

### <a name="reseller-performance-report"></a>**Report prestazioni rivenditore**

> [!Note]
> I dati ricavi e ACR sono disponibili solo per gli utenti che sono visualizzatori di report esecutivi.

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ResellerMPNid | Identificatore Microsoft Partner Network rivenditore | 
| ResellerName | Nome del rivenditore | 
| ResellerMarket | Paese rivenditore del mercato | 
| IndirectProviderMPNId | Identificatore del provider indiretto Microsoft Partner Network | 
| IndirectProviderName | Nome provider indiretto | 
| Month | Mese per cui viene segnalato l'utilizzo e i ricavi | 
| Prodotto | Nome prodotto | 
| SubscriptionID | Identificatore della sottoscrizione | 
| AvailableSeats | Numero di postazioni disponibili | 
| AssignedSeats | Numero di postazioni assegnate | 
| BilledRevenueUSD | Ricavi fatturati in dollari statunitensi | 
| CustomerName | Nome del cliente | 
| CustomerTPid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento Customer | 
| CustomerMarket | Mercato geografico del cliente | 
| ResellerStatus | Stato rivenditore | 

### <a name="subscription-details-report"></a>**Report Dettagli sottoscrizione**

>[!Note]
>I dati ricavi e ACR sono disponibili solo per gli utenti che sono visualizzatori di report esecutivi.

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionState | Stato della sottoscrizione (attiva o con varianza) | 
| Month | Mese per cui vengono segnalati l'utilizzo e i ricavi | 
| IsAutoRenew | Indica se la sottoscrizione è di rinnovo (Sì o no) | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | GUID del cliente | 
| CustomerTpid | Identificatore padre principale del cliente | 
| CustomerSegment | Segmento di mercato del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| Prodotto | Prodotto venduto al cliente dal partner | 
| SKU | SKU del prodotto | 
| MPNId | ID Microsoft Partner Network del partner | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione per la sottoscrizione | 
| SalesChannel | Canale delle vendite-diretto, CSP (Cloud Solution Provider) e così via | 
| AvailableSeats | Postazione disponibile corrente | 
| RevenueUSD | Ricavi in dollari statunitensi | 
| ID registrazione | ID di registrazione della sottoscrizione | 

### <a name="azure-usage-report"></a>**Report sull'utilizzo di Azure**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data della fine della sottoscrizione | 
| SubscriptionState | Stato corrente della sottoscrizione (aperto, chiuso, attivo o nel periodo di tolleranza) | 
| Month | Data aggregata per mese | 
| ServiceName | Nome del servizio di Azure | 
| MeterCategory | Nome della categoria del contatore | 
| UsageUnits | Numero di unità usate durante il ciclo di fatturazione | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID principale del cliente | 
| CustomerSegment | Segmento del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| MPNId | ID Microsoft Partner Network del cliente | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 
| SalesChannel | Canale delle vendite (Direct/CSP, indirect/CSP, Direct e così via) | 
| ACR_USD | Ricavi usati da Azure (ACR) in dollari statunitensi | 
| ID registrazione | ID di registrazione della sottoscrizione di Azure | 

### <a name="office-365-license-usage-report"></a>**Report utilizzo licenze Office 365**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID principale del cliente | 
| Carico di lavoro | Skype for business, teams, Exchange Online | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| PaidAvailableUnits | Numero di unità a pagamento disponibili | 
| MonthlyActiveUsers | Numero di utenti attivi mensili | 
| CustomerName | Nome del cliente | 
| CustomerMarket | Area geografica del mercato del cliente | 
| CustomerSegment | Segmento Customer | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 

### <a name="enterprise-mobility-license-usage-report"></a>**Report sull'utilizzo delle licenze Enterprise Mobility**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID principale del cliente | 
| Carico di lavoro | Nome del carico di lavoro di Enterprise Mobility + Security (EMS) | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| PaidAvailableUnits | Numero di unità a pagamento disponibili | 
| MonthlyActiveUsers | Numero di utenti attivi mensili | 
| CustomerName | Nome del cliente | 
| CustomerMarket | Area geografica del mercato del cliente | 
| CustomerSegment | Segmento Customer | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 

### <a name="dynamics-365-license-usage-report"></a>**Report utilizzo licenze Dynamics 365**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionStatus | Stato della sottoscrizione | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| RevSumDivisionName | Nome della divisione Rev Sum | 
| RevSumCategoryName | Nome della categoria Rev Sum | 
| SKU | SKU del prodotto | 
| SKUId | ID SKU del prodotto | 
| FreeVsPaidSKU | Indica se si tratta di uno SKU gratuito o a pagamento | 
| SalesModel | Canale di vendita usato per la vendita della sottoscrizione | 
| DetailedSalesModel | Modello di vendita dettagliato per la sottoscrizione | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | GUID del tenant del cliente | 
| CustomerTpid | Identificatore padre principale del cliente | 
| CustomerSegment | Segmento di mercato del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttachType | Tipo di attribuzione per la sottoscrizione | 
| AvailableSeats | Postazione disponibile corrente | 
| AssignedSeats | Sede assegnata corrente | 
| ActiveSeats | Postazioni attive correnti | 
| DeploymentOpportunity | Opportunità di distribuzione corrente | 
| ActiveUsagePercent | Percentuale di utilizzo attivo corrente | 

### <a name="power-bi-license-usage-report"></a>**Report utilizzo licenze Power BI**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionStatus | Stato della sottoscrizione (attivo, inattivo o periodo di tolleranza) | 
| Month | Data aggregata per mese | 
| SKU | SKU del prodotto | 
| SKUId | ID SKU del prodotto | 
| FreeVsPaidSKU | Differenziatore SKU gratuito o a pagamento | 
| SalesModel | Modello Sales usato per vendere la sottoscrizione | 
| DetailedSalesModel | Modello di vendita dettagliato per la sottoscrizione | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | GUID del tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento di mercato del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttachType | Tipo di attribuzione per la sottoscrizione | 
| AvailableSeats | Postazioni disponibili correnti | 
| AssignedSeats | Postazioni assegnate correnti | 
| ActiveSeats | Postazioni attive correnti | 
| DeploymentOpportunity | Opportunità di distribuzione corrente | 
| ActiveUsagePercent | Percentuale di utilizzo attivo corrente | 

### <a name="teams-meetings-and-calls-report"></a>**Report riunioni e chiamate del team**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Sottocarico di lavoro | Sottocarico di lavoro per cui viene segnalato l'utilizzo (riunioni, chiamate o sistemi telefonici) | 
| Conteggio riunioni | Numero di riunioni | 
| Durata della riunione | Durata totale riunione in ore | 

### <a name="teams-monthly-usage-report"></a>**Report utilizzo mensile Teams**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Sottocarico di lavoro | Sottocarico di lavoro per cui viene segnalato l'utilizzo (riunioni, chiamate o sistemi telefonici) | 
| Utenti desktop | Numero di utenti che usano i team sul desktop | 
| Utenti mobili | Numero di utenti che usano i team in dispositivi mobili | 
| Utenti Web | Numero di utenti che utilizzano i team sul Web | 
| AllUpParticipants | Numero di utenti univoci dei team per il mese | 

### <a name="teams-usage-3p-apps-report"></a>**Report sulle app di utilizzo di teams 3P**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Nome dell'app 3P | Nome dell'app Teams | 
| Numero utenti | Numero di utenti per l'app | 


### <a name="training-details-report"></a>**Report dettagli di training**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| TrainingActivityId | Identificatore del training | 
| TrainingTitle | Titolo della formazione | 
| TrainingType | Tipo di training (certificazione o esame) | 
| IndividualFirstName | Nome del cliente | 
| IndividualLastName | Cognome del cliente | 
| E-mail | ID di posta elettronica personale del cliente | 
| CorpEmail | ID di posta elettronica dell'ufficio del cliente | 
| TrainingCompletionDate | Data di completamento del training | 
| Month | Mese per cui vengono segnalati i dati | 
| IcMCP | Indica se l'utente è Microsoft Certified Professional (MCP) | 
| MCPID | ID MCP dell'utente | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerCityLocation | Posizione geografica della città del partner | 
| PartnerCountryLocation | Posizione geografica del partner | 

### <a name="microsoft-learn-report"></a>**Report Microsoft Learn**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| UserName | Nome dell'utente | 
| UserId | GUID dell'utente | 
| Trainingname | Nome del training | 
| TrainingType | Tipo di training (modulo o percorso di apprendimento) | 
| Prodotti | Prodotto per cui è applicabile il modulo Learning | 
| Ruoli | Ruoli applicabili del training | 
| CompletionDate | Data di completamento del training | 
| MPNId | Identificatore di Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| Paese | Posizione geografica del partner | 

### <a name="competency-summary-and-history-report"></a>**Riepilogo delle competenze e report della cronologia**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| Competenzaname | Nome della competenza | 
| CompetencyLevel | Livello di competenza (oro o argento) | 
| CompetencyStatus | Stato corrente della competenza (attivo, inattivo o periodo di tolleranza) | 
| CompetencyStartDate | Data di inizio della competenza | 
| CompetencyEndDate | Data di fine della competenza | 

### <a name="competency-performance-report"></a>**Report prestazioni competenza**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| Competenzaname | Nome della competenza | 
| CompetencyAttainmentOptionName | Nome dell'opzione di raggiungimento delle competenze | 
| Month | Mese per cui vengono segnalate le metriche | 
| MetricName | Nome della metrica pertinente per la competenza | 
| MetricMonthlyContribution | Contributo mensile della metrica | 
| TTMAggregate | Metrica aggregata per i 12 mesi finali | 
| AnniversaryYearAggregate | Metrica aggregata per l'anno di anniversario corrente | 
| GoldThreshold | Requisiti di prestazioni per soddisfare le competenze Gold | 
| SilverThreshold | Requisiti di prestazioni per soddisfare le competenze Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Scalabilità del cloud-Microsoft 365 report di propensione**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Nome partner | Nome del partner | 
| Customer ID | Numero identificatore del cliente | 
| Numero DUNS | Il numero di Dun & Bradstreet (D&B) del cliente a cui viene assegnato il punteggio per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore a cui appartiene l'organizzazione | 
| Vertical | Il verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft, D&B e altri standard del settore | 
| Area | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene assegnato il punteggio per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene assegnato il punteggio per la propensione | 
| City | Posizione geografica della città dell'organizzazione | 
| State | Posizione dello stato geografico dell'organizzazione | 
| CAP | CAP dell'organizzazione | 
| Paese | Posizione geografica dell'organizzazione | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top non gestito-base di calcolo | Clienti non gestiti principali-calcolo | 
| Base utente non gestita principale | Clienti non gestiti principali-utente | 
| IsNonProfit | Indica se l'organizzazione è senza scopo di lucro (Sì o no) | 
| Abilita Exchange Online per la destinazione di lavoro | I clienti che dispongono di una sottoscrizione di Exchange Online attiva, si vendono a Microsoft 365 | 
| Abilitare l'acquisizione di lavoro remoto locale (versione corrente) con la propensità cloud Ascent-+ 10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente. In altre termini, la versione del client è successiva alla versione di end of Life (EOL). Il cliente dispone di 10 o più licenze. Cliente con punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto locale (versione corrente) con la propensità cloud Ascent-<10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 10 licenze. Cliente con punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilita l'acquisizione di lavoro remoto locale (versione corrente) senza la propensità del cloud Ascent-+ 10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente, ovvero una versione successiva a EOL. Il cliente dispone di 10 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto locale (versione corrente) senza la propensità cloud Ascent-<10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto in locale (versione EOL) con la propensità cloud Ascent-+ 10 licenze | Cliente che dispone di un ufficio locale o di un client Windows, ovvero una versione di EOL o precedente. Il cliente dispone di 10 o più licenze. Il cliente ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto locale (versione EOL) con la propensità cloud Ascent-<10 licenze | Cliente che dispone di un ufficio locale o di un client Windows, ovvero una versione di EOL o precedente. Il cliente ha meno di 10 licenze. Il cliente ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto in locale (versione EOL) senza la propensità del cloud Ascent-+ 10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente (ovvero una versione EOL o precedente). Il cliente dispone di 10 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilitare l'acquisizione di lavoro remoto locale (versione EOL) senza la propensità di cloud Ascent-<10 licenze | Cliente che dispone di un ufficio locale o di un client Windows corrente (ovvero una versione EOL o precedente). Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere destinato alla conversione in Microsoft 365. | 
| Abilita lavoro remoto-propensità elevata per Microsoft 365 (Act NowithEvaluate) | Clienti prospect con elevata propensione per Microsoft 365 | 
| Abilita lavoro remoto-competi (zoom) con Microsoft 365 | Cliente con zoom e Microsoft 365, destinazione per la conversione ai team | 
| Abilita lavoro remoto-competi (zoom) senza Microsoft 365 | Cliente con zoom, destinazione per la conversione ai team | 
| Ridurre i costi e gestire Microsoft 365 E3 destinati a Microsoft 365 E5 | Cliente esistente con Microsoft 365 E3, destinazione per Microsoft 365 E5 | 
| Riduzione dei costi e della gestione: Microsoft 365 Business clienti Basic e business standard destinati a Microsoft 365 Business Premium | Clienti Microsoft 365 Business Basic e business standard esistenti, destinazione per Microsoft 365 Business Premium | 
| Trasformare la produttività organizzativa-propensità della superficie | Il cliente Mostra una propensione per Surface | 
| M365Cluster | Identifica la propensità di un cliente per l'acquisto di Microsoft 365. Esegui subito la valutazione e valuta i cluster perché produrrà un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se la capacità è ancora disponibile dopo Act Now e valutare i clienti come destinazione. | 
| M365Fit | Punti dati interni ed esterni che definiscono firmographics. Il Punteggio Fit usa un modello sosia per le aziende di piccole o medie dimensioni (PMI) migliori per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| M365Intent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| SurfaceCluster | Identifica la propensità della superficie di acquisto di un cliente consolidando le raccomandazioni Fit e Intent in un cluster. Esegui subito la valutazione e valuta i cluster perché produrrà un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se la capacità è ancora disponibile dopo Act Now e valutare i clienti come destinazione. | 
| SurfaceFit | Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello sosia al nostro PMI migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| SurfaceIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| O365Cluster | Identifica la propensità del cliente per l'acquisto di Office 365. Esegui subito la valutazione e valuta i cluster perché produrrà un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se la capacità è ancora disponibile dopo Act Now e valutare i clienti come destinazione. | 
| O365Fit | Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello sosia al nostro PMI migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| O365Intent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| M365UpsellCustomer | Indica se il cliente Mostra la propensione per Microsoft 365 | 
| Con Google | Indica se il cliente Mostra i segnali concorrenziali per i prodotti Google posseduti | 
| Con AWS | Indica se il cliente Mostra i segnali concorrenziali per i prodotti con Amazon Web Services di proprietario (AWS) | 
| Con EA | Indica se un rinnovo è un contratto Enterprise Agreement (EA) o una sottoscrizione EA | 
| Con apertura | Indica se un rinnovo è un accordo Open o Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent-report di propensione Dynamics 365**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Nome partner | Nome del partner | 
| Customer ID | Numero Identificativo cliente | 
| Numero DUNS | Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore a cui appartiene l'organizzazione | 
| Vertical | Il verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft, D&B e altri standard del settore
| Area | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene assegnato il punteggio per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene assegnato il punteggio per la propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | CAP dell'organizzazione | 
| Paese | Posizione geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | La categorizzazione di un cliente: le principali basi utente non gestite sono i clienti con 300 dipendenti, le principali basi di calcolo non gestite sono i clienti con USD10, 000 in un potenziale di tre anni di Azure, le medie imprese sono clienti con 25 dipendenti o superiore e le piccole imprese sono clienti con meno di 25 dipendenti. | 
| Top non gestito-base di calcolo | Clienti non gestiti principali-calcolo | 
| Base utente non gestita principale | Clienti non gestiti principali: utenti | 
| IsNonProfit | Indica se l'organizzazione è senza scopo di lucro (Sì o no) | 
| Attivazione delle dimensioni della vendita digitale-Microsoft 365-Seat >= 25 postazioni (modello di propensione SalesPro) | Cliente senza Dynamics 365. Dimensioni postazione: 25 +. Il partner deve essere destinato a cross-selling di Dynamics 365 SalesPro. | 
| Attivazione della vendita digitale-Dynamics 365 SalesPro Propensity (Act Now o Evaluate) | Clienti ad alta propensione senza Dynamics 365. Il partner deve essere destinato a Dynamics 365 SalesPro. | 
| Gestione dei rischi finanziari & illecito-Dynamics on-premises install base-Navision (modello di propensione business Central) | Cliente esistente con Navision locale. Il partner deve essere destinato a Dynamics 365 business Central. | 
| Gestione dei rischi finanziari & frode-Dynamics on-premises install base-Dynamics AX (Dynamics 365 Finance + Operation Propensity Model) | Cliente esistente con AX locale. Il partner deve avere come destinazione le operazioni di Dynamics 365 Finance +. | 
| Gestione dei rischi finanziari & frode: base di installazione in locale-grandi pianure (modello di propensione business centrale) | Il cliente esistente con una grande pianura locale. Il partner deve essere destinato a Dynamics 365 business Central. | 
| Gestione dei rischi finanziari & illecito-installazione locale base-Solomon (modello di propensione business Central) | Cliente esistente con Solomon locale. Il partner deve essere destinato a Dynamics 365 business Central. | 
| Gestione dei rischi finanziari & illecito-base di installazione di Dynamics locale-altri (modello di propensione business Central) | Cliente esistente con altre soluzioni locali non elencate in precedenza. Il partner deve essere destinato a Dynamics 365 business Central. | 
| Creazione di processi di business agile-Dynamics on-premises install base-AX/GP/SL/NAV/other (modello di propensità Dynamics 365) | Creazione di processi di business agile-Dynamics on-premises install base-AX/GP/SL/NAV/other (modello di propensità Dynamics 365) | 
| Creazione di processi di business agile-Dynamics compete base-mendix/Outsystems/Salesforce (modello di propensione Dynamics 365) | Creazione di processi di business agile-Dynamics compete base-mendix/Outsystems/Salesforce (modello di propensione Dynamics 365) | 
| Creare processi di business agile-Dynamics 365 Finance + Operations install base | Clienti esistenti di Dynamics 365 Finance + Operations. Partner per le app Power Apps. | 
| Creazione di processi di business agile-base di installazione di Dynamics 365 business Central | Clienti di Dynamics 365 business Central esistenti. Partner per le app Power Apps. | 
| Creazione di processi di business agile-base per l'installazione di Dynamics 365 Customer Engagement | Clienti esistenti di Dynamics 365 Customer Engagement. Partner per le app Power Apps. | 
| Creazione di una supply chain elastica-Windows e attivazione del primo carico di lavoro Dynamics 365 come gestione della supply chain di Dynamics 365 con clienti non Oracle o SAP ERP (Enterprise Resource Planning) | Clienti di destinazione per la gestione della supply chain di Dynamics 365 | 
| Creazione di una catena di fornitura resiliente: Gestione cross-selling della supply chain di Dynamics 365 e/o vendita al dettaglio o al commercio per i clienti esistenti di Dynamics 365 Customer Engagement | I clienti di Dynamics 365 Customer Engagement esistenti sono destinati alla gestione della supply chain di Dynamics 365 con cross-selling. | 
| Creazione di una catena di fornitura resiliente: Gestione cross-selling della supply chain di Dynamics 365 e/o vendita al dettaglio o commerciale per Dynamics 365 Customer Engagement e Oracle o SAP | Clienti di Dynamics 365 Customer Engagement esistenti con Oracle o SAP come destinazione per la gestione della supply chain di Dynamics 365 | 
| D365BCCluster | Identifica la propensità del cliente per l'acquisto di Dynamics 365 business Central. I clienti che mostrano una propensione per business Central saranno nelle categorie media e piccola. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| D365BCFit | Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello sosia al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| D365BCIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| D365FOCluster | Identifica la propensità del cliente per l'acquisto di Dynamics 365 Finance and Operations. I clienti che mostrano una propensione per le operazioni Finance + si troveranno nelle categorie non gestite principali. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| D365FOFit | Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello sosia al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| D365FOIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| D365CECluster | Identifica la propensità del cliente per l'acquisto di Dynamics 365 Customer Engagement. I clienti che mostrano una propensione per il coinvolgimento dei clienti saranno in categorie di medie e piccole dimensioni. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| D365CEFit | Indica la idoneità per Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica l'intenzione di Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Indica se il cliente ha un rinnovo aperto per Dynamics locale AX o CRM | 
| M365UpsellCustomer | Indica se il cliente Mostra la propensione per Microsoft 365 | 
| Con Google | Indica se il cliente Mostra i segnali concorrenziali per i prodotti Google posseduti | 
| Con AWS | Indica se il cliente Mostra i segnali concorrenziali per la proprietaria di prodotti AWS | 
| Con EA | Indica se un rinnovo è una sottoscrizione EA o EA | 
| Con apertura | Indica se un rinnovo è un accordo Open o Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Scalabilità cloud-report di propensità di Azure**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Nome partner | Nome del partner | 
| Customer ID | Numero Identificativo cliente | 
| Numero DUNS | Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore | 
| Vertical | Il verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft, D&B e altri standard del settore | 
| Area | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene assegnato il punteggio per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene assegnato il punteggio per la propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | CAP dell'organizzazione | 
| Paese | Posizione geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top non gestito-base di calcolo | Clienti non gestiti principali-calcolo | 
| Base utente non gestita principale | Clienti non gestiti principali: utenti | 
| IsNonProfit | Indica se l'organizzazione è senza scopo di lucro (Sì o no) | 
| Migrate-EOL Windows Server-EOL Windows Server IB con Cloud Ascent Propensity-5 + licenze | Cliente che dispone di un server Windows locale EOL (ovvero una versione EOL o precedente). Il cliente dispone di 5 o più licenze. Cliente con punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB con Cloud Ascent Propensity-<5 licenze | Cliente che dispone di un server Windows locale EOL (ovvero una versione EOL o precedente). Il cliente ha meno di 5 licenze. Cliente con punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB senza il cloud Ascent Propensity-5 + licenze | Cliente che dispone di un server Windows locale EOL (ovvero una versione EOL o precedente). Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB senza la propensità cloud Ascent-<5 licenze | Cliente che dispone di un server Windows locale EOL (ovvero una versione EOL o precedente). Dispone di meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB con le licenze per l'ascesa al cloud-5 + | Il cliente che dispone di un SQL Server locale EOL (ovvero una versione EOL o precedente). Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB con la propensità cloud Ascent-<5 licenze | Il cliente che dispone di un SQL Server locale EOL (ovvero una versione EOL o precedente). Dispone di meno di 5 licenze. Cliente con punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB senza le licenze per l'ascesa del cloud-5 + | Il cliente che dispone di un SQL Server locale EOL (ovvero una versione EOL o precedente). Il cliente dispone di 5 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB senza propensità cloud Ascent-<5 licenze | Il cliente che dispone di un SQL Server locale EOL (ovvero una versione EOL o precedente). Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione di Windows Server corrente Windows Server IB con le licenze per l'ascesa del cloud-5 + | Cliente che dispone di un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione di Windows Server locale-Windows Server IB corrente con la propensità cloud Ascent-<5 licenze | Cliente che dispone di un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione per Azure. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione di Windows Server locale corrente di Windows Server IB senza la propensità cloud Ascent-5 + licenze | Cliente che dispone di un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione di Windows Server locale corrente di Windows Server IB senza la propensità cloud Ascent-<5 licenze | Cliente che dispone di un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL (VM)-Current SQL Server IB con Cloud Ascent Propensity-5 + licenses | Cliente che dispone di un SQL Server locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione a SQL di Azure o alle macchine virtuali SQL-Current SQL Server IB con la propensità cloud Ascent-<5 licenze | Cliente che dispone di un SQL Server locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione ad Azure SQL o alle macchine virtuali SQL-Current SQL Server IB senza il cloud Ascent Propensity-5 + licenses | Cliente che dispone di un SQL Server locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: eseguire la migrazione a SQL di Azure o alle macchine virtuali SQL-Current SQL Server IB senza propensità cloud Ascent-<5 licenze | Cliente che dispone di un SQL Server locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Migrate-OSS-migrate al database open source Shakespeare (OSS) | Cliente esistente con uno dei prodotti di concorrenza seguenti: PostgreSQL, MySQL, MariaDB. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione-OSS-Linux in Azure | Cliente esistente con Linux. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione di SAP-SAP in Azure | Cliente esistente con SAP. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione-desktop virtuale Windows-Servizi Desktop remoto IB | Identifica i clienti con Servizi Desktop remoto Windows attive. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione: desktop virtuale Windows-cross sell Modern work to Azure/WVD | Identifica i clienti con Microsoft 365 e non dispone di Azure. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione-VMware IB | Cliente esistente con il prodotto: VMware. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione-Citrix IB | Cliente esistente con il prodotto: sistemi Citrix. Il partner deve rivolgersi a questo cliente per la migrazione ad Azure. | 
| Innovazione-Analytics-Power BI IB con la propensità di Azure elevata | Clienti con una sottoscrizione Active Power BI inclusa: Power BI-standalone Pro, Power BI-Suite di Azure, Power BI-Suite di Office, Power BI Suites-Microsoft 365 | 
| Enable-DevOps con GitHub-Visual Studio/MSDN IB | Identifica i clienti con le versioni di Visual Studio attive | 
| Versione standard di Windows Server | Visualizza la versione di Windows Server standard purchases da parte del cliente | 
| Licenza Windows Server standard | Visualizza il tipo di licenza degli acquisti standard di Windows Server da parte del cliente | 
| Versione di Windows Server Data Center | Visualizza la versione di Windows Data Center acquistata dal cliente | 
| Licenza di Windows Server Data Center | Visualizza il tipo di licenza degli acquisti di Windows Data Center da parte del cliente | 
| AzureFit | Punti dati interni ed esterni che definiscono firmographics. Adatta punteggio usa un modello sosia al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. Il Punteggio Fit viene aggiornato trimestralmente. | 
| AzureIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo. Il Punteggio preventivo è sovrapposto al Fit per definire i cluster. Il Punteggio preventivo viene aggiornato ogni mese. | 
| AzureCluster | Identifica la propensità del cliente per l'acquisto di Azure consolidando le raccomandazioni Fit e Intent in un cluster. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| WindowsServerDataCenter_HasOpenRenewal | Indica se il cliente ha un rinnovo aperto per Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Indica se il cliente ha un rinnovo aperto per Windows Server standard | 
| AzureUpsellCustomer | Indica se il cliente Mostra la propensione per Azure | 
| Con Google | Indica se il cliente Mostra i segnali concorrenziali per i prodotti Google posseduti | 
| Con AWS | Indica se il cliente Mostra i segnali concorrenziali per la proprietaria di prodotti AWS | 
| Con EA | Indica se un rinnovo è una sottoscrizione EA o EA | 
| Con apertura | Indica se un rinnovo è un accordo Open o Open Value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent-report di propensanza rinnovo contratto**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network | 
| Nome partner | Nome del partner | 
| Customer ID | Numero Identificativo cliente | 
| Numero DUNS | Il numero Dun & Bradstreet del cliente a cui viene assegnato il punteggio per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore | 
| Vertical | Il verticale del cliente a cui viene assegnato il punteggio per la propensione, identificato da Microsoft, D&B e altri standard del settore | 
| Area | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene assegnato il punteggio per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene assegnato il punteggio per la propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | CAP dell'organizzazione | 
| Paese | Posizione geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top non gestito-base di calcolo | Clienti non gestiti principali-calcolo | 
| Base utente non gestita principale | Clienti non gestiti principali: utenti | 
| IsNonProfit | Indica se l'organizzazione è senza scopo di lucro (Sì o no) | 
| Con Google | Indica se il cliente Mostra i segnali concorrenziali per la proprietaria di prodotti AWS | 
| Con AWS | Indica se il cliente Mostra i segnali concorrenziali per la proprietaria di prodotti AWS | 
| Cluster di Azure | Identifica la propensità del cliente per l'acquisto di Azure. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| D365 Finance + cluster operativo | Identifica la propensità del cliente per l'acquisto di Dynamics 365 Finance and Operations. I clienti che mostrano una propensione per le operazioni Finance + si troveranno nelle categorie non gestite principali. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| Cluster d365 CE | Identifica la propensità del cliente per l'acquisto di Dynamics 365 Customer Engagement. I clienti che mostrano una propensione per il coinvolgimento dei clienti saranno in categorie di medie e piccole dimensioni. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| Cluster d365 BC | Identifica la propensità del cliente per l'acquisto di Dynamics 365 business Central. I clienti che mostrano una propensione per business Central saranno nelle categorie media e piccola. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| Cluster Microsoft 365 | Identifica la propensità del cliente per l'acquisto di Microsoft 365. Destinazione agire ora e valutare i cluster, perché produrranno un rendimento superiore. Destinare i clienti a coltivare e informare i clienti solo se è ancora disponibile una capacità dopo la destinazione di Act e la valutazione dei clienti. | 
| Programma di licenza | Identifica il tipo di programma di licenza per il rinnovo | 
| Agreement ID | Identificatore del contratto | 
| Data di fine contratto | Data di fine del contratto | 
| Tipo di scadenza | Tipo di scadenza | 
| Ricavi in scadenza | Ricavi associati alle sottoscrizioni in scadenza | 
| Con EA | Indica se un rinnovo è una sottoscrizione EA o EA | 
| Con apertura | Indica se un rinnovo è un accordo Open o Open Value | 
| Cliente per la vendita di Azure | Indica se il cliente Mostra la propensione per Azure | 
| Microsoft 365 vendere il cliente | Indica se il cliente Mostra la propensione per Microsoft 365 | 
| RevSumDivisionName | Identifica il prodotto che è attivo per il rinnovo | 

## <a name="next-steps"></a>Passaggi successivi

Per altre informazioni, vedere [scaricare i report](pci-download-reports.md).
