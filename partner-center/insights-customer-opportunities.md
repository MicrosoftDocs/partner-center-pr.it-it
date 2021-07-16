---
title: Partner Center Insights - Report di CloudAscent Segnalazione dell'autenticità
description: Informazioni sui report di CloudAscent Disascent in Partner Center. Include informazioni sulla tendenza di un cliente ad acquistare prodotti Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 6916d44e3f028fbfd788d3bee54671dbadd874d1
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375692"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Report di CloudAscent Tendenza disponibili Partner Center dashboard

**Ruoli appropriati:** visualizzatore di report | Visualizzatore report

Il dashboard Partner Center offre dati scaricabili sulla riservatezza dal programma CloudAscent. I dati mostrano la probabilità che i clienti acquistino prodotti Microsoft.  Questo articolo descrive la suddivisione di questi dati, come usare l'assegnazione dei punteggi e cosa significa.

## <a name="summary-definitions"></a>Definizioni di riepilogo

- **Clienti SMC:** numero totale di clienti nei download di clienti.  I clienti sono identificati dal partner del record.
- **Contratti di scadenza:** nell'anno fiscale corrente viene fornito il numero di contratti in scadenza.
- **Ricavi in scadenza aperti:** ricavi associati ai contratti in scadenza aperti.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Screenshot del dashboard di riepilogo delle opportunità dei clienti.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentazione SMB cloudAscent

Il segmento small-medium business (SMB) è suddiviso in tre segmenti secondari distinti.

1. **Top Unmanaged include** i principali clienti SMB con la massima opportunità per Microsoft. I clienti principali non gestiti tipici condividono caratteristiche simili agli account gestiti, con un numero elevato di dipendenti, budget e spese IT di grandi dimensioni e grandi quantità di potenziali ricavi per Microsoft.

   I primi non gestiti vengono definiti in due modi:

   - **Top Unmanaged User Based**:include gli account con 300 o più dipendenti. User-Based sono ottimi obiettivi per il primo acquisto o l'espansione di prodotti di sottoscrizione basati sull'utente, ad esempio Microsoft 365, Dynamics 365 o Surface.
   - **Top Unmanaged Compute Based :include** account con un potenziale di Azure superiore a $ 10.000. Gli account basati sul calcolo includono Azure esistente. account con potenzialità significative per l'anno futuro e account che non hanno ancora acquistato Azure, ma hanno un potenziale per Azure superiore a $ 10.000.

2. **Medium Business** include clienti esistenti e account potenziali con 25-300 dipendenti.

3. **Le piccole imprese** includono aziende con 10-25 dipendenti.

4. **Very Small Business** include aziende con 1-9 dipendenti.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Cliente per tipo SMC.":::

**I principali**  sottosegmenti non gestiti e di media attività rappresentano clienti con valore di durata elevato per Microsoft e partner Microsoft. Per questo, sono le principali aree di interesse per la crescita in questo segmento. In questi due sottosegmenti è possibile acquisire il socket con Microsoft 365, monetizzare ulteriormente con le app line-of-business (LOB) D365/Azure e realizzare un'elevata LTV per Microsoft.

Oggi sono disponibili due aree chiave di opportunità: 1. il cliente aggiunge crescita; 2. Anche se l'acquisizione dei socket cloud è all'Microsoft 365, è possibile avere grandi opportunità in Dynamics 365 e Azure.

Lo screenshot seguente rappresenta i quattro sottosegmenti SMB. CloudAscent classifica in ordine di priorità la profilatura, l'assegnazione dei punteggi e la modellazione di tutti gli account top unmanaged e medium business.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Screenshot dei sottosegmenti SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB usa la tecnologia di Machine Learning per guidare le stime dei clienti di vendite e marketing all'interno dei segmenti Top Unmanaged e Medium Business. In che modo i segnali vengono raccolti e trasformati in raccomandazioni di tendenza?

- **Raccolta dati:** i crawler Web analizzano e raccolgono miliardi di segnali dei clienti effettuando il ping dei domini aziendali e monitorando post di blog, comunicati stampa, flussi social e forum tecnici.  Oltre ai segnali raccolti, le informazioni di firmografica vengono raccolte da origini interne ed esterne, ad esempio D&B, sottoscrizione interna microsoft e dati transazionali.

- **Machine Learning:** i segnali vengono immessi nel modello di Machine Learning che restituisce un set di dati strutturati di stime di vendite e marketing per ogni cliente in base al prodotto cloud e al cluster.  A ogni cliente viene dato un punteggio usando un modello simile al primo SMB di Microsoft che determina l'idoneità del cliente e gli algoritmi di Machine Learning che integrano il comportamento online del cliente definiscono come Finalità. L'assegnazione dei punteggi viene unita in cluster che mostrano la tendenza di un cliente ad acquistare prodotti Cloud Microsoft.

- **Ottimizzazione:** il Machine Learning ottimizza i modelli utilizzando i dati delle transazioni ogni mese e i dati della sottoscrizione ogni trimestre.  Usando i dati relativi a win/loss, il Machine Learning regola gli algoritmi e verifica che i modelli funzionino come previsto confrontando le raccomandazioni del cluster con le opportunità su cui si agisce in MSX.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Screenshot di Machine Learning SMB.":::

## <a name="cloudascent-propensity"></a>CloudAscent Antasity

Come vengono create le raccomandazioni sulla tendenza?

Usando i segnali raccolti tramite crawler Web e i dati forniti da varie origini, vengono consolidati i dati di firmografica e i segnali dei social media del cliente.  L'assegnazione dei punteggi usa questi segnali e dati nei modelli di confronto per i modelli di adattamento e assegnazione dei punteggi per Intent.

1. Idoneo per l'account cliente

   - Punti dati interni ed esterni che definiscono la firmografica.

   - L'assegnazione dei punteggi di fit usa un modello simile al nostro SMB migliore per confrontare i clienti e verificare se sono una soluzione ideale per i prodotti Microsoft Cloud.

   - L'assegnazione dei punteggi di adattamento viene aggiornata ogni trimestre

2. Finalità dell'account cliente

   - I segnali correlati ai social media e al comportamento online di un cliente definiscono la finalità.

   - Il punteggio della finalità viene sovrapposto all'adattamento per definire i cluster.

   - L'assegnazione dei punteggi delle finalità viene aggiornata ogni mese.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="Modelli predittivi SMB CloudAscent.":::

3. Clustering

   I segnali di adattamento e finalità vengono consolidati in un punteggio di clustering. CloudAscent ha quattro cluster:

      - Act Now : clienti pronti per le vendite
      - Valutazione : clienti pronti per il marketing
      - Crescita: promuovere campagne di sensibilizzazione
      - Istruire: istruire e monitorare la finalità

   Il clustering consente agli utenti di scegliere come destinazione clienti specifici per iniziative di vendita e marketing in base a fattori di segmento, ad esempio prodotto, area geografica, settore e verticale.

   La **scheda Modello di tendenza** in CloudAscent Workbooks condivide la tendenza e i ricavi stimati per gli spazi vuoti. Per definire il clustering di Fit e Intent, si segue questa procedura:

      1. Usando ML, si calcolano prima di tutto il punteggio di adattamento del cliente e il punteggio della finalità su una scala di 100.  I punteggi esatti variano in base ML modelli.  Punteggi di esempio di seguito:

         |**Classificazione**|**Punteggio**|
         |---------|:---------|
         |Alto|75 - 100|
         |Medio|55 - 74|
         |Basso|30 - 54|
         |Molto bassa|0 - 29|

      2. Usando la regola precedente, le aziende vengono classificate come High, Medium, Low e Very Low sia per Customer Fit che per Intent Signals.

      3. Tracciare i segnali di idoneità e finalità del cliente in una matrice 2D con ogni intersezione che rappresenta la tendenza. Ad esempio, High Fit + High Intent = A1, che rappresenta la più alta tendenza.

      4. Infine, questi segmenti raggruppano per formare i cluster.  Ad esempio, A1, A2, A3, A4 formano il cluster Act Now.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="Modelli CloudAscent.":::

   Per questi clienti, è consigliabile scegliere act now e valutare i clienti.

## <a name="cloudascent-products--models"></a>Modelli di & CloudAscent

Il grafico seguente offre una visualizzazione di ogni modello di tendenza all'interno di CloudAscent:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="Modello di tendenza CloudAscent.":::

I modelli di spazi vuoti sono costituiti da stime per i clienti Microsoft esistenti in cui non hanno un prodotto e/o sono nuovi clienti potenziali.

I modelli upsell usano i dati delle transazioni per stimare il potenziale di upsell in Azure e Microsoft 365 SKU.

Questi clienti avranno già azure o Microsoft 365 e il modello upsell mostra che è probabile che acquistino più SKU esistenti.

EOS condivide i clienti di fine servizio (EOS) per Win 7, Office 2010, SQL Server e Windows Server. I dati EOS vengono estratti da MS Sales e sovrapposti con la modellazione di tendenza CloudAscent, dove disponibile. I dati EOS sono presenti nel lavoro moderno e nelle attività di vendita di Azure.
