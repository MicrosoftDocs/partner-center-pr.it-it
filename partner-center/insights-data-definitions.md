---
title: Definizioni dei dati di Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Il documento elenca vari report e le relative definizioni di dati, che è possibile scaricare dalla pagina Insights scarica report.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c77f5eb97771c4768f76b8d35c0d4493c5070ff2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375650"
---
# <a name="export--data-definitions"></a>Esportazione : definizioni dei dati 

**Ruoli appropriati:** Visualizzatore di report | Visualizzatore di report executive

## <a name="introduction"></a>Introduzione 

Usando l'hub Scarica report nel dashboard Insights, è possibile esportare i set di dati non elaborati. 

I vari report, che è possibile scaricare insieme alle relative definizioni di dati, sono elencati nelle tabelle seguenti: 

### <a name="partner-profile-report"></a>**Report del profilo partner**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| MPNId | ID Microsoft Partner Network (MPN)| 
| PartnerName | Nome del partner | 
| PGA_MPNId | Identificatore dell'account globale del partner MPN | 
| PGA_PartnerName | Nome dell'account globale del partner | 
| City | Località della città del partner | 
| Paese | Località del paese del partner | 
| HierarchyLevel | Indica se si tratta di un ID MPN globale o di un ID MPN della posizione | 

### <a name="customer-details-report"></a>**Report dettagli cliente**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | Identificatore del tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento di clienti | 
| CustomerMarket | Mercato geografico del cliente | 
| CustomerStatus | Stato del cliente (attivo o inattivo) | 
| Prodotto | Prodotto venduto al cliente da MPN: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI o Microsoft Azure | 
| SKU | SKU di prodotto | 
| Month | Mese per il quale vengono segnalati l'utilizzo e i ricavi | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 
| SalesChannel | Canale di vendita | 
| AvailableSeats | Postazioni disponibili | 
| RevenueUSD | Ricavi in dollari STATUNITENSI | 

### <a name="reseller-performance-report"></a>**Report sulle prestazioni del rivenditore**

> [!Note]
> I dati relativi ai ricavi e ai ricavi utilizzati da Azure sono disponibili solo per gli utenti che sono visualizzatori di report executive.

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ResellerMPNid | Identificatore Microsoft Partner Network rivenditore | 
| ResellerName | Nome del rivenditore | 
| ResellerMarket | Paese di mercato dei rivenditori | 
| IndirectProviderMPNId | Identificatore del provider indiretto Microsoft Partner Network | 
| IndirectProviderName | Nome del provider indiretto | 
| Month | Mese per il quale vengono segnalati l'utilizzo e i ricavi | 
| Prodotto | Nome prodotto | 
| SubscriptionID | Identificatore della sottoscrizione | 
| AvailableSeats | Numero di postazioni disponibili | 
| AssignedSeats | Numero di postazioni assegnate | 
| BilledRevenueUSD | Ricavi fatturati in dollari USA | 
| CustomerName | Nome del cliente | 
| CustomerTPid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento di clienti | 
| CustomerMarket | Mercato geografico del cliente | 
| ResellerStatus | Stato rivenditore | 

### <a name="subscription-details-report"></a>**Report dettagli sottoscrizione**

>[!Note]
>I dati relativi a ricavi e ACR sono disponibili solo per gli utenti che sono visualizzatori di report executive.

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionState | Stato della sottoscrizione (attivo o in stato di varianza) | 
| Month | Mese per il quale vengono segnalati l'utilizzo e i ricavi | 
| IsAutoRenew | Indica se la sottoscrizione viene nuovata (Sì o No) | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | GUID del cliente | 
| CustomerTpid | Identificatore padre principale del cliente | 
| CustomerSegment | Segmento di mercato del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| Prodotto | Prodotto venduto al cliente dal partner | 
| SKU | SKU del prodotto | 
| MPNId | Microsoft Partner Network'ID del partner | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione per la sottoscrizione | 
| SalesChannel | Canale delle vendite - Direct, Cloud Solution Provider (CSP) e così via | 
| AvailableSeats | Postazione attualmente disponibile | 
| RevenueUSD | Ricavi in dollari statunitensi | 
| ID registrazione | ID registrazione della sottoscrizione | 

### <a name="azure-usage-report"></a>**Report sull'utilizzo di Azure**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionState | Stato corrente della sottoscrizione (Aperto, Chiuso, Attivo o In periodo di tolleranza) | 
| Month | Data aggregata per mese | 
| ServiceName | Nome del servizio di Azure | 
| MeterCategory | Nome della categoria del contatore | 
| UsageUnits | Numero di unità usate durante il ciclo di fatturazione | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID padre principale del cliente | 
| CustomerSegment | Segmento del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| MPNId | Microsoft Partner Network'ID del cliente | 
| PartnerName | Nome del partner | 
| PartnerLocation | Località geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 
| SalesChannel | Canale delle vendite (Direct/CSP, Indiretto/CSP, Diretto e così via) | 
| ACR_USD | Ricavi consumati di Azure (ACR) in dollari statunitensi | 
| ID registrazione | ID registrazione della sottoscrizione di Azure | 

### <a name="office-365-license-usage-report"></a>**Office 365 di utilizzo delle licenze**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID padre principale del cliente | 
| WorkloadName | Skype for Business, Teams, Exchange Online | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| PaidAvailableUnits | Numero di unità disponibili a pagamento | 
| MonthlyActiveUsers | Numero di utenti attivi mensili | 
| CustomerName | Nome del cliente | 
| CustomerMarket | Località geografica del mercato del cliente | 
| CustomerSegment | Segmento del cliente | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Report sull'utilizzo delle licenze di Mobilità**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID padre principale del cliente | 
| WorkloadName | Nome del carico Enterprise Mobility + Security (EMS) | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| PaidAvailableUnits | Numero di unità disponibili a pagamento | 
| MonthlyActiveUsers | Numero di utenti attivi mensili | 
| CustomerName | Nome del cliente | 
| CustomerMarket | Località geografica del mercato del cliente | 
| CustomerSegment | Segmento del cliente | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Posizione geografica del partner | 
| PartnerAttributionType | Tipo di attribuzione del partner | 

### <a name="dynamics-365-license-usage-report"></a>**Report sull'utilizzo delle licenze di Dynamics 365**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionStatus | Stato della sottoscrizione | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| RevSumDivisionName | Nome della divisione rev sum | 
| RevSumCategoryName | Nome della categoria di somma dellev | 
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
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Località geografica del partner | 
| PartnerAttachType | Tipo di attribuzione per la sottoscrizione | 
| AvailableSeats | Postazione attualmente disponibile | 
| AssignedSeats | Postazione assegnata corrente | 
| ActiveSeats | Postazioni attive correnti | 
| DeploymentOpportunity | Opportunità di distribuzione corrente | 
| ActiveUsagePercent | Percentuale di utilizzo attiva corrente | 

### <a name="power-bi-license-usage-report"></a>**Power BI report sull'utilizzo delle licenze**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| SubscriptionId | GUID della sottoscrizione | 
| SubscriptionStartDate | Data di inizio della sottoscrizione | 
| SubscriptionEndDate | Data di fine della sottoscrizione | 
| SubscriptionStatus | Stato della sottoscrizione (attivo, inattivo o in periodo di tolleranza) | 
| Month | Data aggregata per mese | 
| SKU | SKU del prodotto | 
| SKUId | ID SKU del prodotto | 
| FreeVsPaidSKU | Differenziatore SKU gratuito o a pagamento | 
| SalesModel | Modello di vendita usato per vendere la sottoscrizione | 
| DetailedSalesModel | Modello di vendita dettagliato per la sottoscrizione | 
| CustomerName | Nome del cliente | 
| CustomerTenantId | GUID del tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| CustomerSegment | Segmento di mercato del cliente | 
| CustomerMarket | Mercato geografico del cliente | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerLocation | Località geografica del partner | 
| PartnerAttachType | Tipo di attribuzione per la sottoscrizione | 
| AvailableSeats | Postazioni attualmente disponibili | 
| AssignedSeats | Postazioni assegnate correnti | 
| ActiveSeats | Postazioni attive correnti | 
| DeploymentOpportunity | Opportunità di distribuzione corrente | 
| ActiveUsagePercent | Percentuale di utilizzo attiva corrente | 

### <a name="teams-meetings-and-calls-report"></a>**Teams report riunioni e chiamate**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Carico di lavoro secondario | Carico di lavoro secondario per cui viene segnalato l'utilizzo (riunioni, chiamate o sistemi telefonici) | 
| Conteggio riunioni | Numero di riunioni | 
| Durata della riunione | Durata totale della riunione in ore | 

### <a name="teams-monthly-usage-report"></a>**Teams report sull'utilizzo mensile**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | Identificatore dell'elemento padre principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Carico di lavoro secondario | Carico di lavoro secondario per cui viene segnalato l'utilizzo (riunioni, chiamate o sistemi telefonici) | 
| Utenti desktop | Numero di utenti che usano Teams desktop | 
| Utenti mobili | Numero di utenti che usano Teams dispositivi mobili | 
| Utenti Web | Numero di utenti che usano Teams sul Web | 
| AllUpParticipants | Numero di utenti univoci Teams per il mese | 

### <a name="teams-usage-3p-apps-report"></a>**Teams report sull'utilizzo delle app 3P**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CustomerTenantId | ID tenant del cliente | 
| CustomerTpid | ID padre principale del cliente | 
| Month | Mese per cui viene segnalato l'utilizzo | 
| Nome app 3P | Nome dell'app Teams app | 
| Conteggio utenti | Numero di utenti per l'app | 


### <a name="training-details-report"></a>**Report dei dettagli del training**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| TrainingActivityId | Identificatore del training | 
| TrainingTitle | Titolo del training | 
| Tipo di training | Tipo di training (certificazione o esame) | 
| IndividualFirstName | Nome del cliente | 
| IndividualLastName | Cognome del cliente | 
| E-mail | ID di posta elettronica personale del cliente | 
| CorpEmail | Office'ID di posta elettronica del cliente | 
| TrainingCompletionDate | Data di completamento del training | 
| Month | Mese per cui vengono segnalati i dati | 
| IcMCP | Indica se l'utente è un microsoft certified Professional (MCP) | 
| MCPID | ID MCP dell'utente | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| PartnerCityLocation | Posizione geografica della città del partner | 
| PartnerCountryLocation | Località geografica del partner | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn report**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| Nome utente | Nome dell'utente | 
| UserId | GUID dell'utente | 
| TrainingName | Nome del training | 
| Tipo di training | Tipo di training (modulo o percorso di apprendimento) | 
| Prodotti | Prodotto per cui è applicabile il modulo di apprendimento | 
| Ruoli | Ruoli applicabili del training | 
| CompletionDate | Data di completamento del training | 
| MPNId | Identificatore della Microsoft Partner Network | 
| PartnerName | Nome del partner | 
| Paese | Località geografica del partner | 

### <a name="competency-summary-and-history-report"></a>**Riepilogo delle competenze e report cronologia**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CompetencyName | Nome della competenza | 
| CompetencyLevel | Livello di competenza (Gold o Silver) | 
| CompetencyStatus | Stato corrente della competenza (Attivo, Inattivo o In periodo di tolleranza) | 
| CompetencyStartDate | Data di inizio della competenza | 
| CompetencyEndDate | Data di fine della competenza | 

### <a name="competency-performance-report"></a>**Report sulle prestazioni delle competenze**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| CompetencyName | Nome della competenza | 
| CompetencyAttainmentOptionName | Nome dell'opzione di contenimento delle competenze | 
| Month | Mese per cui vengono segnalate le metriche | 
| MetricName | Nome della metrica pertinente per la competenza | 
| MetricMonthlyContribution | Contributo mensile della metrica | 
| TTMAggregate | Metrica aggregata per i 12 mesi finali | 
| AnniversaryYearAggregate | Metrica aggregata per l'anno dell'anniversario corrente | 
| GoldThreshold | Requisito di prestazioni per soddisfare le competenze Gold | 
| SilverThreshold | Requisito di prestazioni per soddisfare le competenze Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent - report Microsoft 365 la tendenza**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Nome partner | Nome del partner | 
| Customer ID | Numero di identificatore del cliente | 
| Numero DUNS | Il numero & Dun&(D&B) del cliente a cui viene in corso l'assegnazione dei punteggi per la tendenza | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore a cui appartiene l'organizzazione | 
| Vertical | Verticale del cliente a cui viene classificata la propensione, come identificato da Microsoft, D&B e altri standard del settore | 
| Ad aree | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene segnati i punteggi per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene ottenuto il punteggio di propensione | 
| City | Posizione geografica della città dell'organizzazione | 
| State | Posizione geografica dello stato dell'organizzazione | 
| CAP | Codice postale dell'organizzazione | 
| Paese | Località geografica del paese dell'organizzazione | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principali clienti non gestiti : calcolo | 
| Top Unmanaged - User Base | Principali clienti non gestiti - utente | 
| IsNonProfit | Indica se l'organizzazione è no profit (Sì o No) | 
| Abilitare il lavoro remoto - Destinazione Exchange Online | Clienti che hanno una sottoscrizione Exchange Online, upsell a Microsoft 365 | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione corrente) con la propensione di Cloud Ascent - +10 licenze | Cliente che dispone di un client Office o Windows locale corrente. Ovvero, la versione del client è successiva a una versione end-of-life (EOL). Il cliente ha 10 o più licenze. Cliente con un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione corrente) con la propensione di Cloud Ascent - <10 licenze | Cliente che dispone di un client Office o Windows locale (ovvero una versione successiva a EOL). Il cliente ha meno di 10 licenze. Cliente con un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione corrente) senza propensione di Cloud Ascent - +10 licenze | Cliente che dispone di un client Office o Windows locale (ovvero una versione successiva a EOL). Il cliente ha 10 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione corrente) senza propensione di Cloud Ascent - <10 licenze | Cliente che dispone di un client Office o Windows locale (ovvero una versione successiva a EOL). Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione EOL) con propensione di Cloud Ascent - +10 licenze | Cliente che dispone di un client EOL Office o Windows ,ovvero una versione di EOL o una versione precedente. Il cliente ha 10 o più licenze. Il cliente ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare il lavoro remoto - acquisizione locale (versione EOL) con propensione di Cloud Ascent - <10 licenze | Cliente che dispone di un client EOL Office o Windows ,ovvero una versione di EOL o una versione precedente. Il cliente ha meno di 10 licenze. Il cliente ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare Il lavoro remoto - Acquisizione locale (versione EOL) senza propensione di Cloud Ascent - +10 licenze | Cliente che dispone di un client Office o Windows locale (ovvero una versione EOL o una versione precedente). Il cliente ha 10 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare il lavoro remoto - acquisizione locale (versione EOL) senza propensione di Cloud Ascent - <10 licenze | Cliente che dispone di un client Office o Windows locale (ovvero una versione EOL o una versione precedente). Il cliente ha meno di 10 licenze. Il cliente non ha un punteggio di propensione. Il partner deve essere la destinazione per la conversione in Microsoft 365. | 
| Abilitare il lavoro remoto - prospettiva ad alta propensione per Microsoft 365 (Act NowithEvaluate) | Cliente potenziale con elevata propensione per Microsoft 365 | 
| Abilitare il lavoro remoto - Compete (Zoom) con Microsoft 365 | Customer with Zoom and Microsoft 365, target for conversion to Teams | 
| Abilitare il lavoro remoto - Compete (Zoom) senza Microsoft 365 | Cliente con Zoom, destinazione per la conversione in Teams | 
| Ridurre i costi e la gestione: Microsoft 365 E3 per l'Microsoft 365 E5 | Cliente esistente con Microsoft 365 E3, destinazione per Microsoft 365 E5 | 
| Ridurre i costi e la gestione: Microsoft 365 Business Basic e Business Standard destinati a Microsoft 365 Business Premium | Clienti Microsoft 365 Business Basic e Business Standard esistenti, come destinazione per Microsoft 365 Business Premium | 
| Trasformare la produttività aziendale - Propensione alla superficie | Il cliente mostra una propensione per Surface | 
| M365Cluster | Identifica la propensione di un cliente ad acquistare Microsoft 365. Target Act Now e Evaluate clusters perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted(Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted). | 
| M365Fit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile alle migliori piccole o medie imprese (SMB) per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| M365Intent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| SurfaceCluster | Identifica la propensione di un cliente ad acquistare Surface consolidando le raccomandazioni fit e intent in un cluster. Target Act Now e Evaluate clusters perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted(Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted). | 
| SurfaceFit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile alle migliori piccole e medie imprese per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| SurfaceIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| O365Cluster | Identifica la propensione del cliente ad acquistare Office 365. Target Act Now e Evaluate clusters perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted(Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted). | 
| O365Fit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile alle migliori piccole e medie imprese per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| O365Intent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| M365UpsellCustomer | Identifica se il cliente mostra la propensione all'upsell per Microsoft 365 | 
| Google ha | Identifica se il cliente mostra segnali competitivi per la proprietà di prodotti Google | 
| Dispone di AWS | Identifica se il cliente mostra segnali competitivi per la proprietà di Amazon Web Services (AWS) | 
| Ha EA | Identifica se un rinnovo è un contratto Enterprise (EA) o una sottoscrizione EA | 
| Ha aperto | Identifica se un rinnovo è un contratto Open o Open Value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent - Dynamics 365 propensione report**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network (MPN) | 
| Nome partner | Nome del partner | 
| Customer ID | Numero di identificatore del cliente | 
| Numero DUNS | Il numero & Di Dun del cliente a cui viene segnati i punteggi per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore a cui appartiene l'organizzazione | 
| Vertical | Verticale del cliente a cui viene classificata la propensione, come identificato da Microsoft, D&B e altri standard del settore
| Ad aree | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene segnati i punteggi per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene ottenuto il punteggio di propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | Codice postale dell'organizzazione | 
| Paese | Località geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Categorizzazione di un cliente: le principali basi di utenti non gestiti sono clienti con più di 300 dipendenti, le principali basi di calcolo non gestite sono clienti con un potenziale triennale di USD 10.000, le aziende medie sono clienti con almeno 25 dipendenti e le piccole imprese sono clienti con meno di 25 dipendenti. | 
| Top Unmanaged - Compute Base | Principali clienti non gestiti : calcolo | 
| Top Unmanaged - User Base | Principali clienti non gestiti : utenti | 
| IsNonProfit | Indica se l'organizzazione è no profit (Sì o No) | 
| Attivare la vendita digitale - Microsoft 365 - dimensioni dei >= 25 posti (modello di propensione SalesPro) | Cliente senza Dynamics 365. Dimensioni del posto: 25+. Il partner deve essere l'obiettivo del cross-selling di Dynamics 365 SalesPro. | 
| Attivare la vendita digitale - Dynamics 365 SalesPro propensione (agire ora o valutare) | Clienti ad alta propensione senza Dynamics 365. Il partner deve avere come destinazione Dynamics 365 SalesPro. | 
| Gestione delle frodi & rischio finanziario - Base di installazione locale di Dynamics - Navision (modello di propensione di Business Central) | Cliente esistente con Navision locale. Il partner deve essere l'obiettivo di Dynamics 365 Business Central. | 
| Gestione dei rischi finanziari & frode - Base di installazione locale di Dynamics - Dynamics AX (dynamics 365 Finance + modello di propensione alle operazioni) | Cliente esistente con AX locale. Il partner deve essere l'obiettivo di Dynamics 365 Finance + Operations. | 
| Gestione delle frodi & rischio finanziario - Base di installazione locale di Dynamics - Great Plains (modello di propensione di Business Central) | Cliente esistente con Great Plains locale. Il partner deve essere l'obiettivo di Dynamics 365 Business Central. | 
| Gestione delle frodi & rischio finanziario - Base di installazione locale di Dynamics - Solomon (modello di propensione di Business Central) | Cliente esistente con Solomon locale. Il partner deve essere l'obiettivo di Dynamics 365 Business Central. | 
| Gestione delle frodi & rischio finanziario - Base di installazione locale di Dynamics - Altri (modello di propensione di Business Central) | Cliente esistente con altre soluzioni locali non elencate in precedenza. Il partner deve essere l'obiettivo di Dynamics 365 Business Central. | 
| Build Agile Business Processes - Dynamics on-premises install base - AX/GP/SL/NAV/Other (Modello di propensione dynamics 365) | Build Agile Business Processes - Dynamics on-premises install base - AX/GP/SL/NAV/Other (Modello di propensione dynamics 365) | 
| Creare processi aziendali Agile - Base di competenze dynamics - Mendix/OutSystems/Salesforce (modello di propensione dynamics 365) | Creare processi aziendali agile - Dynamics compete base - Mendix/OutSystems/Salesforce (modello di propensione dynamics 365) | 
| Creare processi aziendali Agile - Base di installazione di Dynamics 365 Finance + Operations | Clienti Dynamics 365 Finance + Operations esistenti. Partner per la destinazione Power Apps. | 
| Creare processi aziendali Agile - Base di installazione di Dynamics 365 Business Central | Clienti di Dynamics 365 Business Central esistenti. Partner per la destinazione Power Apps. | 
| Creare processi aziendali Agile - Base di installazione di Dynamics 365 Customer Engagement | Clienti di Dynamics 365 Customer Engagement esistenti. Partner per la destinazione Power Apps. | 
| Creare una supply chain resiliente - Windows e attivare il primo carico di lavoro Dynamics 365 come Dynamics 365 Supply Chain Management con clienti non Oracle o SAP ERP (enterprise resource planning) | Clienti di destinazione per la gestione della supply chain di Dynamics 365 | 
| Creare una supply chain resiliente: cross-selling di Dynamics 365 Supply Chain Management e/o Retail o Commerce ai clienti di Dynamics 365 Customer Engagement esistenti | Clienti di Dynamics 365 Customer Engagement esistenti per il cross-selling di Dynamics 365 Supply Chain Management. | 
| Creare una supply chain resiliente: cross-selling di Dynamics 365 Supply Chain Management e/o Retail o Commerce a Dynamics 365 Customer Engagement e Oracle o SAP | Clienti di Dynamics 365 Customer Engagement esistenti con Oracle o SAP per la gestione della supply chain di Dynamics 365 | 
| D365BCCluster | Identifica la propensione del cliente ad acquistare Dynamics 365 Business Central. I clienti che mostrano una propensione per Business Central saranno nelle categorie Medie e Piccole. Target Act Now e Evaluate clusters, perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers (Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers). | 
| D365BCFit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| D365BCIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| D365FOCluster | Identifica la propensione del cliente ad acquistare Dynamics 365 Finance and Operations. I clienti che mostrano una propensione per Finance + Operations saranno nelle prime categorie non gestite. Target Act Now e Evaluate clusters, perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers (Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers). | 
| D365FOFit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| D365FOIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| D365CECluster | Identifica la propensione del cliente ad acquistare Dynamics 365 Customer Engagement. I clienti che mostrano una propensione per Customer Engagement saranno nelle categorie Medio e Piccolo. Target Act Now e Evaluate clusters, perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers (Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers). | 
| D365CEFit | Indica l'adattamento per Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica la finalità per Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica se il cliente ha un rinnovo aperto per Dynamics in locale AX o CRM | 
| M365UpsellCustomer | Identifica se il cliente mostra la propensione all'upsell per Microsoft 365 | 
| Google ha | Identifica se il cliente mostra segnali competitivi per la proprietà di prodotti Google | 
| Dispone di AWS | Identifica se il cliente mostra segnali competitivi per la proprietà di prodotti AWS | 
| Ha EA | Identifica se un rinnovo è una sottoscrizione EA o EA | 
| Ha aperto | Identifica se un rinnovo è un contratto Open o Open Value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent - Report sulla propensione di Azure**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | ID Microsoft Partner Network (MPN) | 
| Nome partner | Nome del partner | 
| Customer ID | Numero di identificatore del cliente | 
| Numero DUNS | Il numero & Di Dun del cliente a cui viene segnati i punteggi per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore | 
| Vertical | Verticale del cliente a cui viene classificata la propensione, come identificato da Microsoft, D&B e altri standard del settore | 
| Ad aree | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene segnati i punteggi per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene ottenuto il punteggio di propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | Codice postale dell'organizzazione | 
| Paese | Località geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principali clienti non gestiti : calcolo | 
| Top Unmanaged - User Base | Principali clienti non gestiti : utenti | 
| IsNonProfit | Indica se l'organizzazione è no profit (Sì o No) | 
| Eseguire la migrazione - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - 5+ licenses | Cliente che ha un server EOL Windows locale, ovvero una versione di EOL o una versione precedente. Il cliente ha 5 o più licenze. Cliente con un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - <5 licenses | Cliente che ha un server EOL Windows locale, ovvero una versione di EOL o una versione precedente. Il cliente ha meno di 5 licenze. Cliente con un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL Windows Server - EOL Windows Server IB senza propensione all'ascensione cloud - 5+ licenze | Cliente che ha un server EOL Windows locale, ovvero una versione di EOL o una versione precedente. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL Windows Server - EOL Windows Server IB senza propensione all'ascensione cloud - <5 licenze | Cliente che ha un server EOL Windows locale, ovvero una versione di EOL o una versione precedente. Ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL SQL - EOL SQL Server IB with Cloud Ascent propensity - 5+ licenses | Cliente che ha un'istanza di EOL SQL Server locale,ovvero una versione EOL o una versione precedente. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL SQL - EOL SQL Server IB with Cloud Ascent propensity - <5 licenses | Cliente che ha un'istanza di EOL SQL Server locale,ovvero una versione EOL o una versione precedente. Ha meno di 5 licenze. Cliente con un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL SQL - EOL SQL Server IB senza propensione di Cloud Ascent - Oltre 5 licenze | Cliente che ha un'istanza di EOL SQL Server locale,ovvero una versione EOL o una versione precedente. Il cliente ha 5 o più licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - EOL SQL - EOL SQL Server IB senza la propensione di Cloud Ascent - <5 licenze | Cliente che ha un'istanza di EOL SQL Server locale,ovvero una versione EOL o una versione precedente. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione di Windows Server locale - Windows Server IB con propensione di Cloud Ascent - 5+ licenze | Cliente con un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione di Windows Server locale - IB Windows Server corrente con propensione di Cloud Ascent - <5 licenze | Cliente con un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione per Azure. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione di Windows Server locale : Windows Server IB senza propensione all'ascensione cloud - 5+ licenze | Cliente con un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione di Windows Server locale - Windows Server IB senza propensione all'ascensione cloud - <5 licenze | Cliente con un server Windows locale corrente, ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione ad Azure SQL o SQL macchine virtuali ( VM) - SQL Server IB con propensione di Cloud Ascent - 5+ licenze | Cliente che dispone di un'istanza locale SQL Server ,ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione alle macchine virtuali SQL o SQL Azure - SQL Server IB con la propensione di Cloud Ascent - <5 licenze | Cliente che dispone di un'istanza locale SQL Server ,ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione alle macchine virtuali SQL o SQL Azure - SQL Server IB senza propensione per l'asce cloud - 5+ licenze | Cliente che dispone di un'istanza locale SQL Server ,ovvero una versione successiva a EOL. Il cliente ha più di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Eseguire la migrazione alle macchine virtuali SQL o SQL Azure - IB SQL Server corrente senza propensione di Cloud Ascent - <5 licenze | Cliente che dispone di un'istanza locale SQL Server ,ovvero una versione successiva a EOL. Il cliente ha meno di 5 licenze. Il cliente non ha un punteggio di propensione. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - OSS - Eseguire la migrazione al database Open Source di Shakespeare (OSS) | Cliente esistente con uno dei prodotti di concorrenza seguenti: PostgreSQL, MySQL, MariaDB. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - OSS - Linux in Azure | Cliente esistente con Linux. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - SAP - SAP in Azure | Cliente esistente con SAP. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Windows Desktop virtuale - Servizi Desktop remoto IB | Identifica i clienti con le Windows Servizi Desktop remoto. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Windows desktop virtuale - Cross Selling Modern Work to Azure/WVD | Identifica i clienti con Microsoft 365 e non dispone di Azure. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - VMware IB | Cliente esistente con il prodotto: VMware. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Eseguire la migrazione - Citrix IB | Cliente esistente con il prodotto: Citrix Systems. Il partner deve avere come destinazione questo cliente per la migrazione ad Azure. | 
| Innovazione - Analisi : Power BI IB con elevata propensione di Azure | Clienti con sottoscrizione e Active Power BI tra cui: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Abilitare - DevOps con GitHub - Visual Studio/MSDN IB | Identifica i clienti con versioni Visual Studio attive | 
| Windows Versione Standard del server | Consente di visualizzare la versione Windows acquisti di Server Standard dal cliente | 
| Windows Licenza Server Standard | Visualizza il tipo di licenza Windows acquisti server Standard dal cliente | 
| Windows Versione del data center del server | Visualizza la versione del Windows di data center acquistati dal cliente | 
| Windows Licenza del data center del server | Visualizza il tipo di licenza Windows di data center acquistati dal cliente | 
| AzureFit | Punti dati interni ed esterni che definiscono firmographics. L'assegnazione dei punteggi di adattamento usa un modello simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti cloud Microsoft. L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre. | 
| AzureIntent | I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità. L'assegnazione dei punteggi delle finalità viene sovrapposta a Fit per definire i cluster. L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente. | 
| AzureCluster | Identifica la propensione del cliente ad acquistare Azure consolidando le raccomandazioni fit e intent in un cluster. Target Act Now e Evaluate clusters, perché produrranno un rendimento superiore. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers (Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers). | 
| WindowsServerDataCenter_HasOpenRenewal | Identifica se il cliente ha un rinnovo aperto per Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identifica se il cliente ha un rinnovo aperto per Windows Server Standard | 
| AzureUpsellCustomer | Identifica se il cliente mostra la propensione all'upsell per Azure | 
| Google ha | Identifica se il cliente mostra segnali competitivi per la proprietà di prodotti Google | 
| Dispone di AWS | Identifica se il cliente mostra segnali competitivi per la proprietà di prodotti AWS | 
| Ha EA | Identifica se un rinnovo è una sottoscrizione EA o EA | 
| Ha aperto | Identifica se un rinnovo è un contratto Open o Open Value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent - Report sulla propensione al rinnovo dell'accordo**

| Nome colonna | Descrizione dei dati | 
| :--------- | :--------- | 
| ID MPN | Microsoft Partner Network ID | 
| Nome partner | Nome del partner | 
| Customer ID | Numero di identificatore del cliente | 
| Numero DUNS | Il numero & Di Dun del cliente a cui viene segnati i punteggi per la propensione | 
| Nome account | Nome dell'account | 
| Dominio | Dominio dell'account | 
| Dimensioni dell'organizzazione | Dimensioni dell'organizzazione | 
| Settore | Settore | 
| Vertical | Verticale del cliente a cui viene classificata la propensione, come identificato da Microsoft, D&B e altri standard del settore | 
| Ad aree | Area geografica della località | 
| Affiliata | La filiale del cliente a cui viene segnati i punteggi per la propensione | 
| Area di vendita | Territorio di vendita del cliente a cui viene ottenuto il punteggio di propensione | 
| City | Posizione geografica della città | 
| State | Posizione dello stato geografico | 
| CAP | Codice postale dell'organizzazione | 
| Paese | Località geografica del paese | 
| Segment | Segmento di mercato | 
| Segmento secondario | Sottosegmento di mercato | 
| Riepilogo del tipo SMC | Tipo SMC | 
| Top Unmanaged - Compute Base | Principali clienti non gestiti : calcolo | 
| Top Unmanaged - User Base | Principali clienti non gestiti : utenti | 
| IsNonProfit | Indica se l'organizzazione è no profit (Sì o No) | 
| Ha Google | Identifica se il cliente mostra segnali competitivi per i prodotti AWS proprietari | 
| Dispone di AWS | Identifica se il cliente mostra segnali competitivi per i prodotti AWS proprietari | 
| Azure Cluster | Identifica la tendenza del cliente ad acquistare Azure. Target Act Now e Evaluate clusters, perché produrranno un rendimento più elevato. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers. | 
| D365 Finance + Operations Cluster | Identifica la tendenza del cliente ad acquistare Dynamics 365 Finance and Operations. I clienti che mostrano una tendenza a Finance + Operations saranno nelle prime categorie non gestite. Target Act Now e Evaluate clusters, perché produrranno un rendimento più elevato. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers. | 
| D365 CE Cluster | Identifica la tendenza del cliente ad acquistare Dynamics 365 Customer Engagement. I clienti che mostrano un'arietà per Customer Engagement saranno nelle categorie Medio e Piccolo. Target Act Now e Evaluate clusters, perché produrranno un rendimento più elevato. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers. | 
| D365 BC Cluster | Identifica la tendenza del cliente ad acquistare Dynamics 365 Business Central. I clienti che mostrano una tendenza per Business Central saranno nelle categorie Medio e Piccolo. Target Act Now e Evaluate clusters, perché produrranno un rendimento più elevato. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers. | 
| Microsoft 365 grappolo | Identifica la tendenza del cliente ad acquistare Microsoft 365. Target Act Now e Evaluate clusters, perché produrranno un rendimento più elevato. Target Nurture and Educate customers only if there is still capacity after you target Act Now and Evaluate customers. | 
| Programma di licenza | Identifica il tipo di programma di licenza per il rinnovo | 
| Agreement ID | Identificatore del contratto | 
| Data di fine contratto | Data di fine del contratto | 
| Tipo di scadenza | Tipo di scadenza | 
| Ricavi in scadenza | Ricavi associati alle sottoscrizioni in scadenza | 
| Ha EA | Identifica se un rinnovo è un contratto EA o una sottoscrizione EA | 
| Ha aperto | Identifica se un rinnovo è un contratto Open Value o Open Value | 
| Cliente di Azure Upsell | Identifica se il cliente mostra l'autenticità dell'upsell per Azure | 
| Microsoft 365 Cliente upselling | Identifica se il cliente visualizza la tendenza dell'Microsoft 365 | 
| RevSumDivisionName | Identifica il prodotto che è in tempo di rinnovo | 

## <a name="next-steps"></a>Passaggi successivi

Per altre informazioni, vedere [Scaricare i report.](insights-download-reports.md)
