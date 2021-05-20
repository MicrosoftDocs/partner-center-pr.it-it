---
title: Partner Center Insights - Report di tendenza di CloudAscent
description: Informazioni sui report di CloudAscent Propensity in Partner Center. Include informazioni sulla propensione di un cliente ad acquistare prodotti Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153039"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Report di tendenza di CloudAscent disponibili Partner Center dashboard

**Ruoli appropriati:** Visualizzatore di report | Visualizzatore di report

Il dashboard Partner Center dashboard fornisce dati scaricabili sulla propensione dal programma CloudAscent. I dati mostrano la probabilità dei clienti di acquistare prodotti Microsoft.  Questo articolo descrive la suddivisione di questi dati, come usare l'assegnazione dei punteggi e cosa significa.

## <a name="summary-definitions"></a>Definizioni di riepilogo

- **Clienti SMC:** numero totale di clienti nei download di propensione.  I clienti vengono identificati dal partner di record.
- **Contratti di scadenza:** entro l'anno fiscale corrente viene fornito il numero di contratti in scadenza.
- **Ricavi in scadenza aperti:** ricavi associati ai contratti di scadenza aperti.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Screenshot del dashboard Riepilogo opportunità clienti.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentazione SMB cloudAscent

Il segmento small-medium business (SMB) è suddiviso in tre sotto segmenti distinti.

1. **Top Unmanaged include** i clienti SMB più grandi con il maggior numero di opportunità per Microsoft. I clienti top unmanaged tipici condividono caratteristiche simili agli account gestiti, con un numero elevato di dipendenti, budget IT di grandi dimensioni e spesa e grandi quantità di potenziali ricavi per Microsoft.

   Si definisce Top Unmanaged in due modi:

   - **Principali utenti non gestiti:** include gli account con 300 o più dipendenti. User-Based sono ottimi obiettivi per il primo acquisto o l'espansione di prodotti di sottoscrizione basati sull'utente, ad esempio Microsoft 365, Dynamics 365 o Surface.
   - **Top Unmanaged Compute Based :include** account con un potenziale di Azure superiore a $ 10.000. Gli account basati sul calcolo includono Azure esistente. account con potenzialità significative per l'anno futuro e account che non hanno ancora acquistato Azure, ma hanno un potenziale per Azure superiore a $ 10.000.

2. **Medium Business** include clienti esistenti e account potenziali con 25-300 dipendenti.

3. **Le piccole imprese** includono aziende con 10-25 dipendenti.

4. **Very Small Business** include aziende con 1-9 dipendenti.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente per tipo SMC.":::

**I principali**  sottosegmenti non gestiti e di media attività rappresentano clienti con valore di durata elevato per Microsoft e partner Microsoft. Per questo, sono le principali aree di interesse per la crescita in questo segmento. In questi due sottosegmenti è possibile acquisire il socket con Microsoft 365, monetizzare ulteriormente con le app line-of-business (LOB) D365/Azure e realizzare un'elevata LTV per Microsoft.

Oggi sono disponibili due aree chiave di opportunità: 1. il cliente aggiunge crescita; 2. Anche se l'acquisizione di socket cloud è all'Microsoft 365, è possibile avere grandi opportunità in Dynamics 365 e Azure.

Lo screenshot seguente rappresenta i quattro sottosegmenti SMB. CloudAscent classifica in ordine di priorità la profilatura, l'assegnazione dei punteggi e la modellazione di tutti gli account top unmanaged e medium business.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Screenshot dei sottosegmenti SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB usa la tecnologia di Machine Learning per guidare le stime dei clienti di vendite e marketing all'interno dei segmenti Top Unmanaged e Medium Business. In che modo i segnali vengono raccolti e trasformati in raccomandazioni di tendenza?

- **Raccolta dati:** i crawler Web analizzano e raccolgono miliardi di segnali dei clienti eseguendo il ping dei domini aziendali e monitorando post di blog, comunicati stampa, flussi social e forum tecnici.  Oltre ai segnali raccolti, le informazioni firmographics vengono raccolte sia da origini interne che esterne, ad esempio D&B, sottoscrizione interna Microsoft e dati transazionali.

- **Machine Learning:** i segnali vengono immessi nel modello di Machine Learning che restituisce un set di dati strutturati di stime di vendite e marketing per ogni cliente in base al prodotto cloud e al cluster.  Ogni cliente viene classificato usando un modello simile al primo SMB di Microsoft che determina l'idoneità del cliente e gli algoritmi di Machine Learning che integrano il comportamento online del cliente definiscono come Finalità. L'assegnazione dei punteggi viene unita a cluster che mostrano la propensione di un cliente ad acquistare prodotti Cloud Microsoft.

- **Ottimizzazione:** il Machine Learning ottimizza i modelli usando i dati delle transazioni mensilmente e i dati della sottoscrizione ogni trimestre.  Usando i dati di win/loss, il Machine Learning regola gli algoritmi e verifica che i modelli funzionino come previsto confrontando le raccomandazioni del cluster con le opportunità su cui si è lavorato in MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Screenshot di Machine Learning SMB.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Come vengono create le raccomandazioni sulla propensione?

Usando i segnali raccolti tramite web crawler e i dati forniti da diverse origini, i dati firmographics e i segnali dei social media dei clienti vengono consolidati.  L'assegnazione dei punteggi usa questi segnali e dati nei modelli di confronto per i modelli di adattamento e assegnazione dei punteggi per Finalità.

1. Idoneo per l'account del cliente

   - Punti dati interni ed esterni che definiscono firmographics.

   - L'assegnazione dei punteggi di adattamento usa un modello simile a quello del nostro SMB migliore per confrontare i clienti e verificare se sono idonei per i prodotti Cloud Microsoft.

   - L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre

2. Finalità dell'account del cliente

   - I segnali correlati ai social media e al comportamento online di un cliente definiscono finalità.

   - L'assegnazione dei punteggi delle finalità viene sovrapposta all'adattamento per definire i cluster.

   - L'assegnazione dei punteggi delle finalità viene aggiornata mensilmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelli predittivi SMB cloudAscent.":::

3. Clustering

   I segnali di idoneità e finalità vengono consolidati in un punteggio di clustering. CloudAscent ha quattro cluster:

      - Act Now : clienti pronti per le vendite
      - Valuta - Clienti pronti per il marketing
      - Promuovere campagne di sensibilizzazione
      - Istruire: istruire e monitorare la finalità

   Il clustering consente agli utenti di scegliere come target clienti specifici per le iniziative di vendita e marketing in base a fattori di segmento, ad esempio prodotto, geo, settore e verticale.

   La **scheda Modello di propensione** nelle cartelle di lavoro cloudAscent condivide la propensione e i ricavi stimati per gli spazi vuoti. Per definire il clustering di Fit and Intent, seguire questa procedura:

      1. Usando i modelli ml, si calcolano prima il punteggio di idoneità del cliente e il punteggio di finalità su una scala di 100.  I punteggi esatti variano in base ai modelli di Machine Learning.  Punteggi di esempio seguenti:

         |**Classificazione**|**Punteggio**|
         |---------|:---------|
         |Alto|75 - 100|
         |Medio|55 - 74|
         |Basso|30 - 54|
         |Molto bassa|0 - 29|

      2. Usando la regola precedente, le aziende vengono classificate come High, Medium, Low e Very Low sia per Customer Fit che per Intent Signals.

      3. Tracciare i segnali di idoneità e finalità del cliente su una matrice 2D con ogni intersezione che rappresenta la propensione. Ad esempio, High Fit + High Intent = A1, che rappresenta la più alta propensione.

      4. Infine, questi segmenti vengono raggruppati per formare cluster.  Ad esempio, A1, A2, A3, A4 formano il cluster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelli CloudAscent.":::

   Per questi clienti, è consigliabile scegliere come destinazione i clienti Act Now e Evaluate.

## <a name="cloudascent-products--models"></a>Modelli di & CloudAscent

La figura seguente offre una visualizzazione di ogni modello di propensione all'interno di CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modello di propensione CloudAscent.":::

I modelli di spazi vuoti sono costituiti da stime per i clienti Microsoft esistenti in cui non hanno un prodotto e/o sono nuovi clienti potenziali.

I modelli upsell usano i dati delle transazioni per stimare il potenziale di upsell in Azure e Microsoft 365 SKU.

Questi clienti avranno già Azure o Microsoft 365 e il modello upsell mostra che è probabile che acquistino più dello SKU esistente.

EOS condivide i clienti di fine servizio (EOS) per Win 7, Office 2010, SQL Server e Windows Server. I dati EOS vengono estratti da MS Sales e sovrapposti con la modellazione della propensione CloudAscent, se disponibile. I dati EOS si mandono nel lavoro moderno e nelle attività di Vendita di Azure.
