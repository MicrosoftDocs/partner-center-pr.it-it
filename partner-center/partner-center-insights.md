---
title: Insights del Centro per i partner
description: Esplora il dashboard di report unificato del centro per i partner. Scopri come stai facendo in KPI per le vendite e la distribuzione, lo sviluppo di clienti e altro ancora.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
keywords: PCI, prestazioni, successo dei clienti, misurazioni, dati di report
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 9e56ae1922abee38537d65564781fea3cb0251e7
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949412"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>Partner Center Insights: dashboard che Mostra come opera un partner commerciale Microsoft

**Ruoli appropriati**
- Amministratore globale
- Amministratore degli account
- Visualizzatore di report esecutivi
- Visualizzatore di report

## <a name="introduction"></a>Introduzione

Insights è un dashboard per la creazione di report unificato nel centro per i partner commerciali Microsoft iscritti al programma Microsoft Partner Network (MPN). Il dashboard Insights offre una visualizzazione a 360 gradi degli indicatori di prestazioni chiave (KPI) tra i prodotti cloud, ad esempio i modelli Office, Azure, Dynamics e licensing come CSP ed EA. Espone un set completo di report KPI che consentono di prendere decisioni basate sui dati per l'organizzazione. 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>Controllo degli accessi in base al ruolo per il dashboard Insights

Sono disponibili due nuovi ruoli nel centro per i partner appositamente progettati per l'accesso alle informazioni dettagliate: **Visualizzatore report** e **Visualizzatore report Executive**. Gli utenti nel ruolo di Visualizzatore report Executive possono accedere a tutti i set di dati di report, mentre gli utenti del ruolo Visualizzatore report non avranno accesso a set di dati sensibili, ad esempio i dati personali relativi a ricavi e clienti. 

L'amministratore globale o l'amministratore dell'account può assegnare gli utenti a questi ruoli e viene assegnato per l'intera azienda o per un percorso MPN specifico.  

>[!Note] 
>Gli utenti che erano amministratori MPN a partire dal 20 gennaio 2020 sono stati aggiunti automaticamente al ruolo Visualizzatore report a livello aziendale. Sono in grado di accedere ai report come visualizzatore di report senza alcuna azione esplicita richiesta dall'amministratore globale o dall'amministratore dell'account. Se necessario, l'amministratore globale o l'amministratore dell'account può eseguire l'override di queste assegnazioni. 

## <a name="reports-available"></a>Report disponibili

I report seguenti sono disponibili come parte del dashboard di Insights.

**Panoramica**: il report introduttivo presenta una visualizzazione snapshot dei diversi indicatori KPI di interesse, ad esempio il numero di clienti, il numero di sottoscrizioni attive, i ricavi di consumo di Azure, le licenze attive e così via.

**Customer**: il rapporto del cliente presenta analisi per i clienti, ad esempio i dati di acquisizione dei clienti, i clienti attivi e così via.

**Prodotto-sottoscrizioni**: il report sottoscrizioni presenta l'analisi di acquisizione e utilizzo per le sottoscrizioni cloud, ad esempio O365, Azure, Dynamics e così via.

**Licenze del prodotto**: il Dashboard delle licenze presenta analisi delle licenze per prodotti cloud basati su licenze, ad esempio O365, Dynamics, Power bi e così via.

**Prodotto-Azure Usage**: il report sull'utilizzo di Azure presenta le metriche correlate alle sottoscrizioni di Azure dei clienti, inclusi i ricavi di consumo e l'utilizzo di Azure in base alle categorie del contatore.

**Competenze**: il report sulle competenze presenta le metriche sulle competenze attive, qualificate e a rischio.

**Vantaggi**: il rapporto sui vantaggi presenta analisi sui vantaggi dei partner ottenuti rispetto al consumo.

## <a name="navigating-the-insights-reports"></a>Esplorazione dei report di Insights

**Filtri**per l'intervallo di date: è possibile trovare una selezione dell'intervallo di date nell'angolo superiore destro di ogni pagina. È possibile personalizzare l'output dei grafici della pagina Panoramica selezionando un intervallo di date basato sugli ultimi 3, 6 o 12 mesi oppure selezionando un intervallo di date personalizzato. La selezione dell'intervallo di date predefinito è di 12 mesi. 

:::image type="content" source="images/pci/intro1.png" alt-text="Mappa introduttiva":::

**Pulsante Commenti e suggerimenti**: ogni grafico/controllo in tutti i report di Insights è incorporato con un pulsante Commenti e suggerimenti che consente di fornire commenti sulle istanze in una funzionalità del report. 

 
**Filtri a livello di pagina**: ad eccezione dei report Panoramica, vantaggi e competenze, tutti i report di Insights consentono di applicare filtri a livello di pagina. 

- I filtri selezionati saranno applicabili a tutti i grafici e alle metriche in una pagina, inclusa la sezione di riepilogo. Se sono presenti dati all'interno di questi criteri di filtro, sarà disponibile un elemento filtro. 

- La selezione predefinita di ogni elenco di filtri è **All**. Se, ad esempio, non è stato selezionato un prodotto specifico nel filtro prodotti, la selezione predefinita sarà tutti i prodotti.

- I filtri selezionati verranno visualizzati nella parte superiore della pagina. 

:::image type="content" source="images/pci/filters.png" alt-text="filtri":::

### <a name="filters-definitions"></a>Definizioni dei filtri:

- Prodotti: elenco di tutti i prodotti Microsoft Cloud venduti/gestiti dall'organizzazione, ad esempio O365, Azure, d365, EMS, Power bi e così via.
- Mercati dei clienti: elenco di paesi del cliente
- Attribuzioni partner: tipo di associazione con le sottoscrizioni dei clienti, ad esempio Digital Partner of record (DPOR), Privileged admin Privilege (DAP), partner admin link (PAL) e così via. 
- Località partner: elenco di tutte le località MPN dell'organizzazione.
- Canali di vendita: tutti i canali di vendita/prezzi tramite cui si acquistano/provisioning di prodotti e servizi, ovvero CSP, EA, CSP indirect, Direct, Advisor, Open, others
- Segmenti dei clienti: elenco di segmenti di clienti attraverso la base dei clienti partner.

## <a name="read-about-each-of-the-dashboards-and-reports"></a>Leggi i dashboard e i report:

- [Partner Center Insights-Dashboard panoramica](pci-overview-report.md)

- [Partner Center Insights - Dashboard clienti](pci-customer-report.md)

- [Partner Center Insights-report sottoscrizioni](pci-product-subscriptions-report.md)

- [Partner Center Insights-report licenze](pci-product-licenses-report.md)

- [Partner Center Insights-report sull'utilizzo di Azure](pci-azure-usage-report.md)

- [Partner Center Insights - Report competenze](pci-competencies-report.md)

- [Partner Center Insights - Report vantaggi](pci-benefits-report.md)
