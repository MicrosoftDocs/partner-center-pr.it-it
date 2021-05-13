---
title: Usare Partner Center Analytics per Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informazioni su come visualizzare i dati aziendali usando il app Analisi del Centro per i Partner per Power BI (per i partner diretti in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855030"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visualizzare i dati aziendali con l'app Partner Center Analytics per Microsoft Power BI



**Ruoli appropriati:** Amministratore globale | Amministratore di gestione utenti | Agente di vendita | Agente amministratore

## <a name="view-your-business-data"></a>Visualizzare i dati aziendali

Ottenere una rappresentazione visiva dei dati aziendali con app Analisi del Centro per i Partner per Power BI, tra cui:

- Crescita della base clienti, delle sottoscrizioni e delle licenze

- L'utilizzo dei prodotti Office 365, Microsoft Dynamics e Microsoft Azure

- Le unità di consumo giornaliere per ogni risorsa a consumo negli abbonamenti di Azure per gli ultimi 60 giorni

- Costo stimato (in base alla scheda tariffa più recente)

- Possibilità di esportare set di dati e creare report personalizzati, incluso per cliente.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informazioni sulla versione Partner Center di anteprima dell'app Di Analytics

- Questa app è solo per i partner diretti Cloud Solution Provider programma. Altri partner in CSP (rivenditori indiretti, ad esempio) non saranno in grado di accedere.

- Tutti i costi stimati sono dati di fatturazione/fattura pre-imposta e non sono legalmente vincolanti. I costi stimati devono essere usati solo per le informazioni dettagliate sui dati.

- Le informazioni sui clienti si basano sulle sottoscrizioni. Tutti i clienti per cui sono stati creati di recente gli account, ma che non hanno ancora sottoscrizioni, non vengono inclusi nei conteggi.

- Il costo stimato si basa sulla scheda tariffa più recente, basata sui prezzi CSP.

- I giorni sono giorni di calendario.

### <a name="business-insights-report"></a>Approfondimento azienda report

- **Tenant dei clienti:** numero di tenant Azure AD tenant dei clienti che hanno acquistato sottoscrizioni

- **Nuovo (ultimi 30 giorni):** nuovi clienti che acquistano almeno una sottoscrizione negli ultimi 30 giorni

- **Varianza (ultimi 30 giorni):** clienti senza sottoscrizioni "attive", "in tolleranza" o "disabilitate"

- **Nuovo (ultime 24 ore):** nuovi clienti che acquistano almeno una sottoscrizione nelle ultime 24 ore

- **Costo mensile stimato negli ultimi 12 mesi:** tendenza mensile dell'importo stimato in dollari della fattura pre-imposta aggregato mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato per prodotto negli ultimi 12** mesi: prodotti venduti ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 12 mesi. Questo stato indica che i prodotti principali hanno prodotto la maggior parte dei ricavi.

- **Clienti negli ultimi 12 mesi:** tendenza mensile dei nuovi clienti e clienti di varianza aggregata mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato per cliente negli ultimi 12** mesi: clienti ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 12 mesi. Questo stato indica che i principali clienti hanno portato la maggior parte dei ricavi.

- **Numero di clienti per prodotto:** prodotti venduti ordinati in base ai clienti associati. Questo stato indica i prodotti più venduti alla maggior parte dei clienti.

### <a name="subscription-insights-report"></a>Report informazioni dettagliate sulla sottoscrizione

- **Stato della sottoscrizione:**

- Attivo: sottoscrizioni appartenenti allo stato "attivo" o "in stato di tolleranza"

  - Sospeso: sottoscrizioni appartenenti allo stato "disabilitato"

  - De-provisioning: sottoscrizioni appartenenti allo stato "De-provisioning" o "Scaduto"

- **Stato di scadenza:**

  - Scaduto: sottoscrizioni già scadute (in cui la data di fine della sottoscrizione è passata)

  - Scadenza dopo 30 giorni: sottoscrizioni che scadono dopo 30 giorni (in cui la data di fine della sottoscrizione è successiva ai 30 giorni successivi)

  - Scadenza entro 30 giorni: sottoscrizioni che scadranno entro i 30 giorni successivi (dove la data di fine della sottoscrizione è compresa tra oggi e i 30 giorni successivi)

- **Totale sottoscrizioni:** sottoscrizioni con stato "attivo", "in stato di tolleranza" o "disabilitato"

- **Nuovo (ultimi 30 giorni):** nuove sottoscrizioni acquistate dai clienti negli ultimi 30 giorni

- **Nuovo (ultime 24 ore):** nuove sottoscrizioni acquistate dai clienti nelle ultime 24 ore

- **Scadenza tra 30 giorni:** sottoscrizioni che scadranno entro i prossimi 30 giorni

- **Varianza (ultimi 30 giorni):** sottoscrizioni di cui è stato eseguito il de-provisioning o sospese (disabilitate) negli ultimi 30 giorni

- **Distribuzione in base ai tipi di sottoscrizione:**% distribuzione delle sottoscrizioni totali in base alla licenza e al tipo di sottoscrizione basata sull'utilizzo

- **Conteggio sottoscrizioni attive per prodotto:** prodotti venduti ordinati in base al numero di sottoscrizioni attive

- **Sottoscrizioni negli ultimi 12 mesi:** tendenza mensile delle nuove sottoscrizioni e delle sottoscrizioni di varianza aggregate mensilmente nel periodo degli ultimi 12 mesi

- **Dettagli della sottoscrizione del** cliente: visualizzazione dettagliata di clienti, sottoscrizioni e offerte

### <a name="license-insights-report"></a>Report di Informazioni dettagliate sulle licenze:

- **Totale licenze:** numero totale di licenze aggregate in tutte le sottoscrizioni basate su licenza

- **Nuovo (ultimi 30 giorni):** aggiunta della licenza negli ultimi 30 giorni

- **Varianza (ultimi 30 giorni):** riduzione delle licenze negli ultimi 30 giorni

- **Nuovo (ultime 24 ore):** aggiunta della licenza nelle ultime 24 ore

- **Licenze negli ultimi 90 giorni:** tendenza mensile delle aggiunte e delle riduzioni delle licenze aggregate mensilmente nel periodo degli ultimi 90 giorni

- **Numero di licenze attive per prodotto:** prodotti venduti ordinati in base al numero di licenze attive

- **Numero di licenze attive per cliente:** clienti ordinati in base al numero di licenze attive

- **Dettagli dell'evento** di licenza del cliente negli ultimi 90 giorni: visualizzazione dettagliata dei clienti, delle sottoscrizioni e degli eventi di sottoscrizione, tra cui la data dell'evento, il nome dell'evento, la quantità e la modifica della quantità.

### <a name="licenses-usage-report"></a>Report utilizzo licenze:

- **Licenze assegnate per prodotto:** prodotti venduti ordinati in base al numero di assegnazioni di licenze

- **Licenze in uso per prodotto:** prodotti venduti ordinati in base al numero di utilizzo delle licenze

- **Distribuzione delle licenze assegnate dal cliente:**% di distribuzione dei clienti totali suddivisa in bucket dell'intervallo del 20% in base alla % di assegnazione delle licenze

- **Distribuzione delle licenze in uso da parte** dei clienti: % di distribuzione del totale dei clienti suddivisa in bucket dell'intervallo del 20% in base alla % di utilizzo delle licenze

- **Licenze assegnate dal cliente:** visualizzazione dettagliata delle licenze vendute e delle licenze assegnate da clienti e prodotti

- **Licenze in uso dal cliente:** visualizzazione dettagliata delle licenze vendute e delle licenze usate da clienti e prodotti

### <a name="azure-insights-report"></a>Report di Azure Insights:

- Clienti basati sull'utilizzo negli ultimi **12** mesi: tendenza mensile dei nuovi clienti basati sull'utilizzo e dei clienti basati sull'utilizzo variati aggregati mensilmente nel periodo degli ultimi 12 mesi

- Sottoscrizioni basate sull'utilizzo negli ultimi **12** mesi: tendenza mensile delle nuove sottoscrizioni basate sull'utilizzo e delle sottoscrizioni basate sull'utilizzo variate aggregate mensilmente nel periodo degli ultimi 12 mesi

- **Costo stimato dell'utilizzo** per cliente negli ultimi 60 giorni: clienti basati sull'utilizzo ordinati in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 60 giorni. Questo stato indica che i principali clienti basati sull'utilizzo hanno portato la maggior parte dei ricavi

- Costo stimato dell'utilizzo per categoria negli ultimi **60** giorni: categorie del contatore delle sottoscrizioni basate sull'utilizzo ordinate in base all'importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 60 giorni.

- Costo stimato di utilizzo per sottoscrizione negli ultimi **60** giorni: sottoscrizioni basate sull'utilizzo per importo stimato in dollari della fattura pre-imposta aggregato nel periodo degli ultimi 60 giorni.

- **Costo di utilizzo stimato dal cliente per budget** di spesa: i clienti ordinati per percentuale del budget di spesa per l'utilizzo corrente superano la soglia (100%).

### <a name="azure-resource-usage-report"></a>Report Utilizzo risorse di Azure:

- **Utilizzo delle risorse di Azure** per giorno per il periodo selezionato: unità di consumo giornaliere per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni.

- **Costo di utilizzo stimato** delle risorse di Azure per il periodo selezionato: costo stimato in base alla tariffa più recente per ogni risorsa a consumo in ogni sottoscrizione basata sull'utilizzo per il periodo selezionato negli ultimi 60 giorni. 

## <a name="next-steps"></a>Passaggi successivi

- [Partner Center Di Analytics per Power BI'app](power-bi-app-for-direct-partners.md)

- [Installare e visualizzare in anteprima l'app Analisi del Centro per i Partner per Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
