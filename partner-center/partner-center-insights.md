---
title: Insights del Centro per i partner
description: Esplorare questo dashboard Partner Center report unificato. Informazioni sulle prestazioni degli indicatori KPI per le vendite e la distribuzione, lo sviluppo dei clienti e altro ancora.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 6661fb013b25e55785dac9156e5f3561f5b50c97
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151016"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Insights: dashboard che mostra le attività di un partner commerciale Microsoft

**Ruoli appropriati:** amministratore globale | Account admin | Visualizzatore di report | Visualizzatore di report

## <a name="introduction"></a>Introduzione

Il dashboard di Insights è un dashboard di report unificato in Partner Center per i partner commerciali Microsoft registrati al programma Microsoft Partner Network (MPN). Il dashboard insights offre una visualizzazione a 360 gradi degli indicatori di prestazioni chiave (KPI) in prodotti cloud come Office, Azure, Dynamics e modelli di licenza come CSP ed EA. Espone un set ricco di report KPI che consentono di prendere decisioni guidate sui dati per l'organizzazione. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Controllo degli accessi in base al ruolo nel dashboard di Insights

Sono disponibili due nuovi ruoli in Partner Center specificamente per l'accesso a Insights: **Visualizzatore** report e **Executive Report Viewer.** Gli utenti con il ruolo Executive Report Viewer hanno accesso a tutti i set di dati di report, mentre gli utenti con il ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i ricavi e i dati personali di clienti/dipendenti. 

L'amministratore globale o l'amministratore account può assegnare questi ruoli agli utenti e vengono assegnati per l'intera azienda o per una posizione MPN specifica.  

>[!Note] 
>Gli utenti che erano amministratori MPN dal 20 gennaio 2020 sono stati aggiunti automaticamente al ruolo visualizzatore di report a livello aziendale. Possono accedere ai report come visualizzatore di report senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore account. Se necessario, gli amministratori globali o gli amministratori dell'account possono eseguire l'override di queste assegnazioni. 

## <a name="reports-available"></a>Report disponibili

I report seguenti sono disponibili come parte del dashboard informazioni dettagliate.

**Panoramica:** il report Panoramica presenta una visualizzazione snapshot dei vari indicatori KPI di interesse, ad esempio il numero di clienti, il numero di sottoscrizioni attive, i ricavi a consumo di Azure, le licenze attive e così via.

**Customer**(Cliente): il report Customer (Cliente) presenta analisi per i clienti, ad esempio i dati di acquisizione dei clienti, i clienti attivi e così via.

**Prodotto - Sottoscrizioni:** il report Sottoscrizioni presenta l'analisi di acquisizione e utilizzo per le sottoscrizioni cloud,ad esempio Office 365, Azure, Dynamics e così via.

**Prodotto - Licenze:** il dashboard Licenze presenta l'analisi delle licenze per i prodotti cloud basati su licenza, ad esempio Office 365, Dynamics, Power BI e così via.

**Prodotto - Utilizzo di Azure:** il report Utilizzo di Azure presenta le metriche correlate alle sottoscrizioni di Azure dei clienti, inclusi i ricavi a consumo di Azure e l'utilizzo per categorie di contatori.

**Competenze:** il report Competenze presenta le metriche sulle competenze attive, qualificate e a rischio.

**Vantaggi:** il report Vantaggi presenta l'analisi dei vantaggi dei partner ottenuti e utilizzati.

## <a name="navigating-the-insights-reports"></a>Esplorazione dei report di Insights

**Filtri per intervalli di** date: è possibile trovare una selezione dell'intervallo di date nell'angolo superiore destro di ogni pagina. L'output dei grafici della pagina di panoramica può essere personalizzato selezionando un intervallo di date basato sugli ultimi 3, 6 o 12 mesi oppure selezionando un intervallo di date personalizzato. L'intervallo di date predefinito è 12 mesi. 

:::image type="content" source="images/pci/intro1.png" alt-text="Mappa introduttiva":::

**Pulsante Commenti e** suggerimenti: ogni grafico/controllo in tutti i report di Insights è incorporato con un pulsante di feedback per consentire di fornire commenti e suggerimenti sulle istanze su una funzionalità del report. 

 
**Filtri a livello di** pagina: ad eccezione dei report Panoramica, Vantaggi e Competenze, tutti i report di Insights consentono di applicare filtri a livello di pagina. 

- I filtri selezionati saranno applicabili per tutti i grafici e le metriche in una pagina, inclusa la sezione di riepilogo. Se sono presenti dati all'interno di tali criteri di filtro, sarà disponibile un elemento filtro. 

- La selezione predefinita di ogni elenco di filtri **è .** Ad esempio, se non è stato selezionato un prodotto specifico nel filtro dei prodotti, la selezione predefinita sarà tutti i prodotti.

- I filtri selezionati verranno visualizzati nella parte superiore della pagina. 

:::image type="content" source="images/pci/filters.png" alt-text="Screenshot parziale che mostra la barra Filtri applicati con le selezioni di filtro per Prodotti, Mercati dei clienti, Attribuzioni partner e Canali di vendita.":::

### <a name="filters-definitions"></a>Definizioni dei filtri:

- Prodotti: elenco di tutti i prodotti Microsoft Cloud venduti/gestiti dall'organizzazione, ad esempio Office 365, Azure, D365, EMS, Power BI e così via.
- Mercati dei clienti: elenco dei paesi dei clienti
- Attribuzioni dei partner: il tipo di associazione con le sottoscrizioni dei clienti, ad esempio Partner digitale di record (DPOR), Privilegi di amministratore delegato (DAP) e Collegamento amministratore partner (PAL). 
- Località dei partner: elenco di tutte le località MPN dell'organizzazione.
- Canali di vendita: tutti i canali di vendita/prezzi tramite i quali si acquistano/e provisioning prodotti e servizi, ovvero CSP, EA, CSP indiretto, diretto, advisor, aperto, altri
- Segmenti dei clienti: elenco dei segmenti di clienti nella base di clienti dei partner.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Informazioni su ogni dashboard e report:

- [Partner Center Insights - Dashboard Panoramica](pci-overview-report.md)

- [Partner Center Insights - Dashboard clienti](pci-customer-report.md)

- [Partner Center Insights - Report Sottoscrizioni](pci-product-subscriptions-report.md)

- [Partner Center Insights - Report licenze](pci-product-licenses-report.md)

- [Partner Center Insights - Report sull'utilizzo di Azure](pci-azure-usage-report.md)

- [Partner Center Insights - Report competenze](pci-competencies-report.md)

- [Partner Center Insights - Report vantaggi](pci-benefits-report.md)
