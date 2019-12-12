---
title: App Analisi del Centro per i Partner per Power BI   | Centro per i partner
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usare l'app Analisi del Centro per i Partner per Power BI (per i partner diretti in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a2a20ce2c2d73381121f210e5cf41e7405c6840d
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004870"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visualizzare i dati aziendali con l'app Analisi del Centro per i Partner per Microsoft Power BI

**Si applica a**

-   Centro per i partner

**Ruoli appropriati**
-   Amministratore globale
-   Amministratore utenti
-   Agente di vendita
-   Agente amministratore

## <a name="view-your-business-data"></a>Visualizzare i dati aziendali

Con l'app Analisi del Centro per i Partner per Power BI è disponibile una rappresentazione visiva dei dati aziendali che include:

- Aumento della base di clienti, delle sottoscrizioni e delle licenze

- Utilizzo dei prodotti Office 365, Microsoft Dynamics e Microsoft Azure

- Unità di consumo giornaliere per ciascuna risorsa a consumo in ogni sottoscrizione di Azure per gli ultimi 60 giorni

- Costo stimato (in base al tariffario più recente)

- Possibilità di esportare set di dati e creare report personalizzati, anche per cliente 

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informazioni sulla versione di anteprima dell'app Analisi del Centro per i Partner

 - Questa app è riservata solo all'uso da parte dei partner diretti nel programma Cloud Solution Provider Altri partner nel CSP (ad esempio rivenditori indiretti) non saranno in grado di accedere.

- Tutti i costi stimati sono calcolati in base a dati di fatturazione al lordo delle imposte e non sono legalmente vincolanti. I costi stimati sono destinati esclusivamente per l'analisi dei dati.

- Le informazioni sui clienti si basano sulle loro sottoscrizioni. I clienti per cui sono stati recentemente creati account, ma non dispongono ancora di sottoscrizioni, non sono inclusi nei conteggi. 

- Il costo stimato si basa sul tariffario più recente, a sua volta basato sui prezzi CSP. 

- I giorni sono giorni di calendario. 


### <a name="business-insights-report"></a>Report Approfondimento azienda

-  **Tenant cliente**: numero di tenant Azure AD distinti per i clienti che hanno acquistato sottoscrizioni

-  **Nuovi (ultimi 30 giorni)** : nuovi clienti che hanno acquistato almeno una sottoscrizione negli ultimi 30 giorni

-  **Varianza (ultimi 30 giorni)** : clienti senza sottoscrizioni "attive", "in Grace" o "disabilitate"

- **Nuovi (ultime 24 ore)** : nuovi clienti che hanno acquistato almeno una sottoscrizione nelle ultime 24 ore

- **Costo mensile stimato negli ultimi 12 mesi**: tendenza mensile dell'importo stimato in dollari di fatturazione al lordo delle imposte aggregato mensilmente su un periodo che copre gli ultimi 12 mesi

- **Costo stimato per prodotto negli ultimi 12 mesi**: prodotti venduti ordinati per importo stimato in dollari di fatturazione al lordo delle imposte aggregato su un periodo che copre gli ultimi 12 mesi Fornirà indicazioni sui prodotti principali che generano la maggior parte dei ricavi.

- **Clienti negli ultimi 12 mesi**: tendenza mensile dei nuovi clienti e dei clienti persi aggregata mensilmente su un periodo che copre gli ultimi 12 mesi

- **Costo stimato per cliente negli ultimi 12 mesi**: clienti ordinati per importo stimato in dollari di fatturazione al lordo delle imposte aggregato su un periodo che copre gli ultimi 12 mesi Fornirà indicazioni sui clienti principali che generano la maggior parte dei ricavi.

- **Conteggio clienti per prodotto**: prodotti venduti ordinati in base ai clienti associati. Fornirà indicazioni sui prodotti principali venduti alla maggior parte dei clienti. 


### <a name="subscription-insights-report"></a>Report Approfondimento sottoscrizioni 

- **Stato sottoscrizione**:

    - Attivo: le sottoscrizioni appartenenti a uno stato "attivo" o "in tolleranza"

    - Sospeso: le sottoscrizioni appartenenti allo stato "disabilitato"

    - Deprovisioning eseguito: sottoscrizioni appartenenti allo stato "deprovisioned" o "expired"

- **Stato scadenza**:

    - Scadute: sottoscrizioni già scadute (per cui la data di fine della sottoscrizione è nel passato)

    - In scadenza dopo 30 giorni: sottoscrizioni che scadranno dopo 30 giorni (per cui la data di fine della sottoscrizione è dopo 30 giorni)

    - In scadenza tra 30 giorni: sottoscrizioni che scadranno entro i successivi 30 giorni (per cui la data di fine della sottoscrizione è tra la data odierna e i successivi 30 giorni)

-  **Totale sottoscrizioni**: sottoscrizioni in stato "attivo", "in Grace" o "disabilitato"

- **Nuove (ultimi 30 giorni)** : nuove sottoscrizioni acquistate dai clienti negli ultimi 30 giorni

- **Nuove (ultime 24 ore)** : nuove sottoscrizioni acquistate dai clienti nelle ultime 24 ore

- **In scadenza tra 30 giorni**: sottoscrizioni che scadranno entro i successivi 30 giorni

- **Abbandoni (ultimi 30 giorni)** : sottoscrizioni per cui è stato effettuato il deprovisioning o sospese (disabilitate) negli ultimi 30 giorni

- **Distribuzione per tipi di sottoscrizione**: % di distribuzione delle sottoscrizioni totali in base al tipo di sottoscrizione basata su licenza e basata sull'utilizzo

- **Conteggio sottoscrizioni attive per prodotto**: prodotti venduti ordinati in base al numero di sottoscrizioni attive

- **Sottoscrizioni negli ultimi 12 mesi**: tendenza mensile delle nuove sottoscrizioni e delle sottoscrizioni perse aggregata mensilmente su un periodo che copre gli ultimi 12 mesi

- **Dettagli sottoscrizioni clienti**: visualizzazione dettagliata di clienti, sottoscrizioni e offerte 


### <a name="license-insights-report"></a>Report Approfondimento licenze:

- **Licenze totali**: numero totale di licenze aggregato per tutte le sottoscrizioni basate su licenza

- **Nuove (ultimi 30 giorni)** : licenze aggiunte negli ultimi 30 giorni

- **Nuove (ultimi 30 giorni)** : licenze ritirate negli ultimi 30 giorni

- **Nuove (ultime 24 ore)** : licenze aggiunte nelle ultime 24 ore

- **Licenze negli ultimi 90 giorni**: tendenza mensile delle licenze aggiunte e ritirate aggregata mensilmente su un periodo che copre gli ultimi 90 giorni

- **Conteggio licenze attive per prodotto**: prodotti venduti ordinati in base al numero di licenze attive

- **Conteggio licenze attive per cliente**: clienti ordinati in base al numero di licenze attive

- **Dettagli evento licenze attive negli ultimi 90 giorni**: visualizzazione dettagliata di clienti, sottoscrizioni e eventi di sottoscrizione inclusi data dell'evento, nome dell'evento, quantità e modifiche alla quantità.


### <a name="licenses-usage-report"></a>Report Utilizzo licenze:

- **Licenze assegnate per prodotto**: prodotti venduti ordinati in base al numero di licenze assegnate

- **Licenze in uso per prodotto**: prodotti venduti ordinati in base al numero di licenze in uso

- **Distribuzione clienti di licenze assegnate**: % di distribuzione dei clienti totali suddivisi in bucket di intervallo pari al 20% in base alla percentuale di licenze assegnate

- **Distribuzione clienti di licenze in uso**: % di distribuzione dei clienti totali suddivisi in bucket di intervallo pari al 20% in base alla percentuale di licenze in uso

- **Licenze assegnate per cliente**: visualizzazione dettagliata delle licenze vendute e assegnate in base a clienti e prodotti

- **Licenze in uso per cliente**: visualizzazione dettagliata delle licenze vendute e in uso in base a clienti e prodotti


### <a name="azure-insights-report"></a>Report Approfondimenti di Azure:

- **Clienti basati su utilizzo negli ultimi 12 mesi**: tendenza mensile dei nuovi clienti basati sull'utilizzo e dei clienti persi basati sull'utilizzo aggregata mensilmente su un periodo che copre gli ultimi 12 mesi

- **Sottoscrizioni basate su utilizzo negli ultimi 12 mesi**: tendenza mensile delle nuove sottoscrizioni basate sull'utilizzo e delle sottoscrizioni perse basate sull'utilizzo aggregata mensilmente su un periodo che copre gli ultimi 12 mesi

- **Costo stimato di utilizzo per cliente negli ultimi 60 giorni**: clienti basati sull'utilizzo ordinati per importo stimato in dollari di fatturazione al lordo delle imposte aggregato su un periodo che copre gli ultimi 60 giorni Fornirà indicazioni sui clienti principali basati sull'utilizzo che generano la maggior parte dei ricavi

- **Costo stimato di utilizzo per categoria negli ultimi 60 giorni**: categorie a consumo delle sottoscrizioni basate sull'utilizzo ordinate per importo stimato in dollari di fatturazione al lordo delle imposte aggregato su un periodo che copre gli ultimi 60 giorni

- **Costo stimato di utilizzo per sottoscrizione negli ultimi 60 giorni**: sottoscrizioni basate sull'utilizzo ordinate per importo stimato in dollari di fatturazione al lordo delle imposte aggregato su un periodo che copre gli ultimi 60 giorni

- **Costo di utilizzo stimato clienti per budget di spesa**: clienti ordinati in base alla percentuale del loro budget di spesa per utilizzo corrente che supera la soglia (100%).


### <a name="azure-resource-usage-report"></a>Report Utilizzo risorse di Azure:

- **Utilizzo di risorse di Azure per giorno per il periodo selezionato**: unità di consumo giornaliere per ogni risorsa a consumo in ciascuna sottoscrizione basata sull'utilizzo per un periodo selezionato che copre gli ultimi 60 giorni.

- **Costo utilizzo stimato di risorse di Azure per il periodo selezionato**: costo stimato basato sul tariffario più recente per ogni risorsa a consumo in ciascuna sottoscrizione basata sull'utilizzo per un periodo selezionato che copre gli ultimi 60 giorni. 

## <a name="see-also"></a>Vedi anche

[Panoramica di partner Center Analytics per app Power BI](power-bi-app-for-direct-partners.md)


[Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
