---
title: Informazioni dettagliate sul centro per i partner-CloudAscent
description: Informazioni sui report di proCloudAscentzione del centro per i partner. Sono incluse informazioni sulla propensione del cliente per l'acquisto di prodotti Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 2cdb63c8f7e29fc8a56e920b587e47c382c6eacb
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086958"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent i report di propensione disponibili dal dashboard del centro per i partner

**Ruoli appropriati**

- Visualizzatore di report esecutivi
- Visualizzatore di report

Il dashboard del centro per i partner fornisce dati di propensione scaricabili dal programma CloudAscent. I dati mostrano la propensità dei clienti per l'acquisto di prodotti Microsoft.  Questo articolo descrive la suddivisione di questi dati, le modalità di utilizzo dei punteggi e il significato.

## <a name="summary-definitions"></a>Definizioni di riepilogo

- **Clienti SMC**: questo è il numero totale di clienti nei download di propensione.  I clienti sono identificati dal partner del record.
- **Scadenza dei contratti**: nell'anno fiscale corrente viene fornito il numero di contratti in scadenza.
- **Scadenza dei ricavi**: il ricavo associato ai contratti in scadenza.
- **Apertura dei ricavi in scadenza**: il ricavo associato ai contratti aperti in scadenza.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Screenshot del dashboard di riepilogo delle opportunità dei clienti.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentazione SMB CloudAscent

Il segmento small to Medium Business (SMB) viene diviso ulteriormente in tre sottosegmenti distinti.

1. **Top unmanaged** include i maggiori clienti SMB con la massima opportunità per Microsoft. I clienti principali non gestiti più comuni condividono caratteristiche simili a quelle degli account gestiti, con un numero elevato di dipendenti, budget IT di grandi dimensioni e spesa e grandi quantità di potenziali ricavi per Microsoft.

   Vengono definiti i due modi principali non gestiti:

   - **Top non gestito basato su utenti**: include account con 300 o più dipendenti. User-Based gli account sono ottimi obiettivi per l'acquisto iniziale o l'espansione di prodotti di sottoscrizione basati sugli utenti, ad esempio Microsoft 365, Dynamics 365 o Surface.
   - **Top non gestito basato su calcolo** : include account con potenziali Azure maggiori di $10.000. Gli account basati su calcolo includono Azure esistente. account con potenziali anni e account futuri significativi che hanno ancora acquistato Azure, ma che hanno un potenziale di Azure superiore a $10.000.

2. **Media Business** include clienti esistenti e account Prospect con 25 a 300 dipendenti.

3. **Small Business** include tutte le aziende rimanenti con meno di 25 dipendenti.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Tipo Customer by SMC.":::

I principali sottosegmenti aziendali **non gestiti** e **medi** rappresentano i clienti LTV (High Life-Time) per Microsoft e i partner Microsoft. Per questo motivo, si tratta delle aree principali di interesse per la crescita in questo segmento. In questi due sottosegmenti, possiamo acquisire il socket con Microsoft 365, monetizzare ulteriormente con le app line-of-business (LOB) d365/Azure e realizzare un LTV elevato per Microsoft.

Oggi sono disponibili due aree principali di opportunità: 1. il cliente aggiunge la crescita; 2. anche se stiamo acquisendo un'ottima opportunità di acquisizione dei socket cloud con Microsoft 365, abbiamo una grande opportunità in d365 e in Azure.

Lo screenshot seguente rappresenta i tre sottosegmenti SMB e le route ottimizzate per il mercato. CloudAscent assegna la priorità alla profilatura, al punteggio e alla modellazione di tutti gli account aziendali principali non gestiti e medi.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Screenshot dei sottosegmenti SMB.":::

## <a name="cloudascent-machine-learning"></a>Machine Learning CloudAscent

SMB utilizza la tecnologia di machine learning per promuovere le stime dei clienti di vendite e marketing all'interno dei principali segmenti aziendali non gestiti e medi. In che modo i segnali vengono raccolti e trasformati in raccomandazioni di propensità?

- **Raccolta dati**: i Web crawler analizzano e raccolgono miliardi di segnali dei clienti eseguendo il ping dei domini aziendali e monitorando: post di Blog, comunicati stampa, flussi sociali e forum tecnici.  Oltre ai segnali raccolti, le informazioni di firmographics vengono raccolte da origini interne ed esterne quali D&B, sottoscrizione interna Microsoft e dati transazionali.

- **Machine Learning**: i segnali vengono inseriti nel modello di Machine Learning che restituisce un set di dati strutturato di stime di vendite e marketing per ogni cliente dal prodotto e dal cluster cloud.  A ogni cliente viene assegnato un punteggio usando un modello simile a SMB principale di Microsoft che determina l'idoneità del cliente e gli algoritmi di Machine Learning che integrano il comportamento online del cliente definito come finalità. Il Punteggio viene unito in cluster che mostrano la propensità di un cliente per l'acquisto di prodotti Microsoft Cloud.

- **Ottimizzazione**: il sistema di Machine Learning ottimizza i modelli tramite l'utilizzo dei dati delle transazioni mensili e i dati di sottoscrizione trimestrali.  Usando i dati di win/loss, il Machine Learning regola gli algoritmi e verifica che i modelli funzionino come previsto confrontando le raccomandazioni del cluster con le opportunità eseguite nel server MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot di SMB Machine Learning.":::

## <a name="cloudascent-propensity"></a>Propensità CloudAscent

Come vengono create le raccomandazioni relative alla propensione?

Usando i segnali raccolti tramite i crawler web e i dati forniti da varie origini, i dati firmographics e i segnali dei social media del cliente vengono consolidati.  Il Punteggio usa questi segnali e dati nei modelli di confronto per adattarli e assegnare punteggi ai modelli per finalità.

1. Adattamento dell'account cliente

   - Punti dati interni ed esterni che definiscono firmographics.

   - Adatta punteggio usa un modello di aspetto simile al nostro SMB migliore per confrontare i clienti e verificare se sono idonei per Microsoft Cloud prodotti.

   - Il Punteggio Fit è stato aggiornato trimestralmente

2. Finalità dell'account cliente

   - I segnali correlati ai social media e al comportamento online di un cliente definiscono lo scopo.

   - Il Punteggio preventivo è sovrapposto alla soluzione adatta per definire i cluster.

   - Il Punteggio preventivo viene aggiornato ogni mese.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelli predittivi SMB CloudAscent.":::

3. Clustering

   I segnali per Fit e Intent sono consolidati in un punteggio di clustering. CloudAscent dispone di quattro cluster:

      - Agire ora-clienti pronti per le vendite
      - Valutazione-clienti pronti al marketing
      - Campagne di sensibilizzazione sulle unità
      - Istruire-educare e monitorare le finalità

   Il clustering consente agli utenti di rivolgersi a clienti specifici per iniziative di vendita e marketing in base a fattori di segmento, ad esempio: prodotto, Geo, settore e verticale.

   La scheda **modello di propensione** nelle cartelle di lavoro di CloudAscent condivide la propensità e il ricavo dello spazio vuoto stimato. Per definire il clustering di Fit e Intent, seguire questa procedura:

      1. Usando i modelli ML, viene innanzitutto calcolato il Punteggio fit del cliente e il Punteggio preventivo su una scala di 100.  I punteggi esatti variano in base ai modelli ML.  Punteggi di esempio seguenti:

         |**Classificazione**|**Punteggio**|
         |---------|:---------|
         |Alto|75-100|
         |Medio|55-74|
         |Basso|30 - 54|
         |Molto bassa|0 - 29|

      2. Utilizzando la regola precedente, le aziende vengono classificate come alta, media, bassa e molto bassa per i segnali di adattamento dei clienti e finalità.

      3. Si tracciano i segnali di adattamento dei clienti e finalità su una matrice 2D con ogni intersezione che rappresenta la propensione. Ad esempio, High Fit + High Intent = a1, che rappresenta la propensità più elevata.

      4. Infine, questi segmenti raggruppano per formare i cluster.  Ad esempio, a1, a2, a3 e A4 formano il cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelli CloudAscent.":::

   Per questi clienti, è consigliabile scegliere come destinazione Act Now e valutare i clienti.

## <a name="cloudascent-products--models"></a>Modelli di & di prodotti CloudAscent

Il grafico seguente offre una visualizzazione di ogni modello di propensione all'interno di CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent modello di propensione.":::

I modelli di spazi vuoti sono costituiti da stime per i clienti Microsoft esistenti in cui non dispongono di un prodotto e/o sono clienti NET New Prospect.

I modelli di upsell usano i dati delle transazioni per stimare il potenziale per la vendita in Azure e Microsoft 365 SKU.

EOS condivide i clienti finali dei servizi per Windows 7, Office 2010, SQL Server e Windows Server. I dati EOS vengono estratti dalle vendite MS e sovrapposti alla modellazione della propensione CloudAscent, se disponibile. I dati EOS si trovano nel lavoro moderno e nelle vendite di Azure.
