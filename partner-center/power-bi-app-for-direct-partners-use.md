---
title: Usare il centro per i partner Analytics per Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come visualizzare i dati aziendali usando l'app di analisi del centro per i partner per Power BI (per i partner diretti in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215748"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visualizzare i dati aziendali con l'app partner Center Analytics per Microsoft Power BI



**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Agente di vendita
- Agente amministratore

## <a name="view-your-business-data"></a>Visualizza i dati aziendali

Ottieni una rappresentazione visiva dei dati aziendali con l'app di analisi del centro per i partner per Power BI, tra cui:

- Crescita della base clienti, delle sottoscrizioni e delle licenze

- L'utilizzo dei prodotti Office 365, Microsoft Dynamics e Microsoft Azure

- Le unità di consumo giornaliere per ogni risorsa a consumo negli abbonamenti di Azure per gli ultimi 60 giorni

- Costo stimato (in base all'ultima scheda tariffaria)

- Possibilità di esportare set di impostazioni e creare report personalizzati, inclusi i singoli clienti.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informazioni sulla versione di anteprima dell'app partner Center Analytics

- Questa app è destinata solo ai partner diretti nel programma Cloud Solution Provider. Altri partner in CSP (rivenditori indiretti, ad esempio) non saranno in grado di eseguire l'accesso.

- I costi stimati sono i dati di fatturazione/fattura pre-fiscali e non sono legalmente vincolanti. I costi stimati devono essere usati solo per le informazioni dettagliate sui dati.

- Le informazioni sul cliente si basano sulle sottoscrizioni. I clienti di cui sono stati creati di recente gli account, ma che non dispongono ancora di sottoscrizioni, non sono inclusi nei conteggi.

- Il costo stimato è basato sull'ultima scheda tariffaria, basata sui prezzi di CSP.

- I giorni sono giorni di calendario.

### <a name="business-insights-report"></a>Report di business Insights

- **Tenant del cliente**: numero di tenant Azure ad distinti dei clienti che hanno acquistato sottoscrizioni

- **Nuovi (ultimi 30 giorni)**: i nuovi clienti che acquistano almeno una sottoscrizione negli ultimi 30 giorni

- **Varianza (ultimi 30 giorni)**: clienti senza sottoscrizioni "attive", "in Grace" o "disabilitate"

- **Nuove (ultime 24 ore)**: i nuovi clienti che acquistano almeno una sottoscrizione nelle ultime 24 ore

- **Costo mensile stimato negli ultimi 12 mesi**: tendenza del mese in base all'importo stimato per la fattura pre-imposte in dollari aggregati mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato per prodotto negli ultimi 12 mesi**: i prodotti venduti ordinati in base all'importo stimato per la fattura pre-imposta sono aggregati nel periodo degli ultimi 12 mesi. Questo stato indica i primi prodotti che portano la maggior parte dei ricavi.

- **Clienti negli ultimi 12 mesi**: tendenza del mese rispetto al mese dei nuovi clienti e dei clienti con varianza aggregata mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato per cliente negli ultimi 12 mesi**: i clienti ordinati in base all'importo stimato per la fattura pre-imposta è aggregato nel periodo degli ultimi 12 mesi. Questo stato indica i clienti principali che riportano la maggior parte dei profitti.

- **Conteggio clienti per prodotto**: prodotti venduti ordinati per clienti associati. Questo stato indica i prodotti principali venduti alla maggior parte dei clienti.

### <a name="subscription-insights-report"></a>Report informazioni dettagliate sottoscrizione

- **Stato sottoscrizione**:

- Attivo: le sottoscrizioni appartenenti a uno stato "attivo" o "in tolleranza"

  - Sospeso: le sottoscrizioni appartenenti allo stato "disabilitato"

  - Deprovisioning eseguito: sottoscrizioni appartenenti allo stato "deprovisioned" o "expired"

- **Stato scadenza**:

  - Scaduto: sottoscrizioni già scadute (in cui la data di fine della sottoscrizione è passata)

  - Scadenza dopo 30 giorni: sottoscrizioni che scadono dopo 30 giorni (dove la data di fine della sottoscrizione è successiva a 30 giorni)

  - Scadenza tra 30 giorni: le sottoscrizioni scadranno entro i prossimi 30 giorni (dove la data di fine della sottoscrizione è compresa tra oggi e i successivi 30 giorni)

- **Totale sottoscrizioni**: sottoscrizioni in stato "attivo", "in Grace" o "disabilitato"

- **Nuovi (ultimi 30 giorni)**: nuove sottoscrizioni acquistate dai clienti negli ultimi 30 giorni

- **Nuove (ultime 24 ore)**: nuove sottoscrizioni acquistate dai clienti nelle ultime 24 ore

- **Scadenza tra 30 giorni**: sottoscrizioni che scadranno entro i prossimi 30 giorni

- **Varianza (ultimi 30 giorni)**: sottoscrizioni di cui è stato effettuato il deprovisioning o sospese (disabilitate) negli ultimi 30 giorni

- **Distribuzione per tipi di sottoscrizione**:% distribuzione delle sottoscrizioni totali per tipo di sottoscrizione basata sulle licenze e utilizzo

- **Numero di sottoscrizioni attive per prodotto**: i prodotti venduti ordinati per numero di sottoscrizioni attive

- **Sottoscrizioni negli ultimi 12 mesi**: tendenza rispetto al mese precedente di nuove sottoscrizioni e sottoscrizioni varianza aggregate mensilmente nel periodo degli ultimi 12 mesi

- **Dettagli sull'abbonamento clienti**: visualizzazione dettagliata dei clienti, delle sottoscrizioni e delle offerte

### <a name="license-insights-report"></a>Report informazioni sulle licenze:

- **Totale licenze**: numero totale di licenze aggregate in tutte le sottoscrizioni basate su licenze

- **Nuovi (ultimi 30 giorni)**: addizione della licenza negli ultimi 30 giorni

- **Varianza (ultimi 30 giorni)**: riduzione della licenza negli ultimi 30 giorni

- **Nuove (ultime 24 ore)**: addizione delle licenze nelle ultime 24 ore

- **Licenze negli ultimi 90 giorni**: tendenza del mese rispetto al mese delle aggiunte e delle riduzioni delle licenze aggregate mensilmente nel periodo degli ultimi 90 giorni

- **Conteggio licenze attive per prodotto**: prodotti venduti ordinati per numero di licenze attive

- **Conteggio licenze attive per cliente**: clienti ordinati per numero di licenze attive

- **Dettagli dell'evento di licenza del cliente negli ultimi 90 giorni**: visualizzazione dettagliata dei clienti, delle sottoscrizioni e degli eventi di sottoscrizione, tra cui la data dell'evento, il nome dell'evento, la quantità e la modifica della quantità.

### <a name="licenses-usage-report"></a>Report utilizzo licenze:

- **Licenze assegnate dal prodotto**: prodotti venduti ordinati per numero di assegnazioni di licenze

- **Licenze utilizzate dal prodotto**: prodotti venduti ordinati per numero di utilizzo delle licenze

- **Distribuzione del cliente delle licenze assegnate**:% distribuzione dei clienti totali suddivisi in bucket del 20% di intervallo per assegnazione della licenza%

- **Distribuzione dei clienti delle licenze in uso**:% distribuzione dei clienti totali suddivisi in bucket del 20% di intervallo per utilizzo licenza%

- **Licenze assegnate dal cliente**: visualizzazione dettagliata delle licenze vendute e licenze assegnate da clienti e prodotti

- **Licenze in uso da** parte del cliente: visualizzazione dettagliata delle licenze vendute e licenze utilizzate da clienti e prodotti

### <a name="azure-insights-report"></a>Report di Azure Insights:

- **Clienti basati sull'utilizzo negli ultimi 12 mesi**: tendenza al mese rispetto ai nuovi clienti basati sull'utilizzo e ai clienti basati sull'utilizzo con varianza aggregata mensilmente nel periodo degli ultimi 12 mesi

- **Sottoscrizioni basate sull'utilizzo negli ultimi 12 mesi**: tendenza rispetto al mese precedente di nuove sottoscrizioni basate sull'utilizzo e sottoscrizioni basate sull'utilizzo varianza aggregate mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato dell'utilizzo da parte del cliente negli ultimi 60 giorni**: i clienti basati sull'utilizzo sono ordinati in base all'importo stimato per la fattura pre-imposta, aggregato nel periodo degli ultimi 60 giorni. Questo stato indica clienti principali basati sull'utilizzo che riportano la maggior parte dei ricavi

- **Costo stimato dell'utilizzo in base alla categoria negli ultimi 60 giorni**: categorie di contatori delle sottoscrizioni basate sull'utilizzo ordinate in base all'importo stimato per la fattura pre-imposta, aggregato per il periodo degli ultimi 60 giorni.

- **Costo stimato dell'utilizzo da parte della sottoscrizione negli ultimi 60 giorni**: sottoscrizioni basate sull'utilizzo in base all'importo stimato per la fattura pre-imposta in dollari aggregati nel periodo degli ultimi 60 giorni.

- **Costo di utilizzo stimato del cliente per budget di spesa**: i clienti ordinati per percentuale del budget di spesa di utilizzo corrente supera la soglia (100%).

### <a name="azure-resource-usage-report"></a>Report sull'utilizzo delle risorse di Azure:

- **Utilizzo delle risorse di Azure per giorno per il periodo selezionato**: unità consumo giornaliero per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni.

- **Costo di utilizzo stimato delle risorse di Azure per il periodo selezionato**: costo stimato basato sull'ultima scheda tariffaria per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni. 

## <a name="next-steps"></a>Passaggi successivi

- [Panoramica di partner Center Analytics per app Power BI](power-bi-app-for-direct-partners.md)

- [Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
