---
title: Insights Training Dashboard
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Esplorare il dashboard Partner Center Training. Il training è uno dei report disponibili nell'area Partner Center Insights (PCI).
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b80944074666a161a4f5794a3c35ed3ca2d6376
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375280"
---
# <a name="trainings-dashboard"></a>Dashboard dei training

**Ruoli appropriati:** Visualizzatore di report | Visualizzatore di report

Il dashboard Trainings (Corsi di formazione) fornisce informazioni dettagliate su certificazioni, valutazioni ed esami esersi dall'azienda di dipendenti aziendali. Il dashboard Trainings include le sezioni seguenti:

- Riepilogo
- Prestazioni del training suddivise per certificazioni, valutazioni, esami
- Singoli utenti in base a credenziali come certificazioni, valutazioni, esami
- Dettagli dell'attività

>[!NOTE] 
>Questo report è disponibile nell'hub Insights in Partner Center. Per visualizzare questo report, è necessario avere il ruolo Visualizzatore report o Visualizzatore di report executive. Alcune sezioni di questo report saranno visibili solo per gli utenti che sono visualizzatori di report executive. Per altre informazioni sul controllo di accesso per i report Insights, vedere [Ruoli PCI](insights-roles.md).

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot numerica di vari indicatori di prestazioni correlati ai training. I vari indicatori di prestazioni sono Certified Individuals, Certifications, Individuals with Exam Credentials, Exam Credentials, Individuals with Assessment Credentials e Assessment Credentials. I dati in questa sezione vengono aggiornati in base all'intervallo di date selezionato, che può essere di tre mesi (3 milioni), sei mesi (6 milioni) e 12 mesi (1Y) o un intervallo di dati personalizzato (personalizzato). 

:::image type="content" source="images/insights/training-dashboard-summary.png" alt-text="Riepilogo.":::

- **Persone con certificazioni:** rappresenta il numero di persone distinte con certificazioni nell'azienda.
- **Conteggio certificazioni:** rappresenta il numero totale di certificazioni prese da singoli utenti dell'azienda.
- **Individui con valutazioni:** rappresenta il numero di persone distinte con credenziali di valutazione nell'azienda. 
- **Conteggio valutazioni**: rappresenta il numero totale di valutazioni da parte di singoli utenti dell'azienda.
- **Persone con esami:** rappresenta il numero di persone distinte con credenziali di esame nell'azienda. 
- **Numero di esami:** rappresenta il numero totale di esami evasi da singoli utenti dell'azienda.

## <a name="training-performance"></a>Prestazioni del training

Le prestazioni di training presentano il numero mensile di utenti singoli e i training completati dai singoli utenti dell'azienda. È suddiviso per certificazioni, valutazioni ed esami sotto forma di grafico per l'intervallo di date selezionato. L'asse X rappresenta i mesi per l'intervallo di date selezionato. L'asse Y rappresenta il numero distinto di individui e il numero di training esersi per il tipo di training selezionato. Selezionare le rispettive schede sopra il grafico per visualizzare la suddivisione in base al tipo di training. I dati del grafico possono essere scaricati tramite l'icona di download in formato TSV per l'intervallo di date selezionato.

:::image type="content" source="images/insights/training-dashboard-training-performance.png" alt-text="Prestazioni di training.":::

## <a name="individuals-performance"></a>Prestazioni dei singoli utenti

La sezione Prestazioni di Singoli utenti presenta i dettagli del training effettuato dai singoli utenti dell'azienda per l'intervallo di date selezionato. Cercare e selezionare il nome di una persona nel pannello sinistro della sezione. I dettagli del training per la persona selezionata vengono visualizzati nel pannello destro della sezione.

:::image type="content" source="images/insights/training-dashboard-individual-performance.png" alt-text="Prestazioni individuali.":::

>[!NOTE] 
> La sezione Prestazioni utenti singoli è disponibile solo per gli utenti che sono visualizzatori di report executive. 

## <a name="next-steps"></a>Passaggi successivi

[Report in Partner Center Insights](partner-center-insights.md)

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report nel dashboard Insights dati. [Altre informazioni](insights-download-reports.md)