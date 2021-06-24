---
title: Dashboard di training delle informazioni dettagliate
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Esplorare il dashboard Partner Center Training. Training è uno dei report disponibili nell'area Partner Center Insights (PCI).
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 37a4f6cdce2b77f194fc91e0490e1c87ee137b43
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565101"
---
# <a name="trainings-dashboard"></a>Dashboard training

**Ruoli appropriati:** visualizzatore di report | Visualizzatore report

Il dashboard Training fornisce informazioni dettagliate su certificazioni, valutazioni ed esami esersi dall'azienda dei dipendenti aziendali. Il dashboard Training include le sezioni seguenti:

- Riepilogo
- Training Performance split by certifications, assessments, exams
- Singoli utenti in base a credenziali come certificazioni, valutazioni ed esami
- Dettagli dell'attività

>[!NOTE] 
>Questo report è disponibile nell'hub Insights in Partner Center. Per visualizzare questo report, è necessario che sia assegnato il ruolo di Visualizzatore report o Visualizzatore di report dirigenti. Alcune sezioni di questo report saranno visibili solo per gli utenti che sono visualizzatori di report dirigenti. Per altre informazioni sul controllo di accesso per i report di Insights, vedere [Ruoli PCI.](pci-roles.md)

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot numerica dei vari indicatori di prestazioni correlati ai training. I vari indicatori di prestazioni sono Certified Individuals, Certifications, Individuals with Exam Credentials, Exam Credentials, Individuals with Assessment Credentials e Assessment Credentials. I dati in questa sezione vengono aggiornati in base all'intervallo di date selezionato, che può essere di tre mesi (3 milioni), sei mesi (6 milioni) e 12 mesi (1Y) o un intervallo di dati personalizzato (personalizzato). 

:::image type="content" source="images/pci/td-summary.png" alt-text="Riepilogo.":::

- **Singoli utenti con certificazioni:** rappresenta il numero di persone distinte con certificazioni nell'azienda.
- **Certifications count (Conteggio** certificazioni): rappresenta il numero totale di certificazioni adottate dai singoli utenti dell'azienda.
- **Singoli utenti con valutazioni:** rappresenta il numero di persone distinte con credenziali di valutazione nell'azienda. 
- **Assessments count (Conteggio** valutazioni): rappresenta il numero totale di valutazioni adottate dai singoli utenti dell'azienda.
- **Individui con esami:** rappresenta il numero di persone distinte con credenziali di esame nell'azienda. 
- **Numero di** esami: rappresenta il numero totale di esami ese nell'azienda.

## <a name="training-performance"></a>Prestazioni di training

Le prestazioni di training presentano il conteggio mensile delle persone e i corsi completati da singoli utenti dell'azienda. È suddiviso per certificazioni, valutazioni ed esami sotto forma di grafico per l'intervallo di date selezionato. L'asse X rappresenta i mesi per l'intervallo di date selezionato. L'asse Y rappresenta il numero distinto di individui e il numero di training esersi per il tipo di training selezionato. Selezionare le rispettive schede sopra il grafico per visualizzare la suddivisione in base al tipo di training. I dati del grafico possono essere scaricati tramite l'icona di download in formato TSV per l'intervallo di date selezionato.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="Prestazioni di training.":::

## <a name="individuals-performance"></a>Prestazioni dei singoli utenti

La sezione Prestazioni degli utenti singoli presenta i dettagli del training effettuato dai singoli utenti dell'azienda per l'intervallo di date selezionato. Cercare e selezionare il nome di una persona nel pannello sinistro della sezione. I dettagli del training per la persona selezionata vengono visualizzati nel pannello destro della sezione.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Prestazioni indiviuali.":::

>[!NOTE] 
> La sezione Prestazioni utenti singoli è disponibile solo per gli utenti che sono visualizzatori di report diretti. 

## <a name="next-steps"></a>Passaggi successivi

[Report in Partner Center Insights](partner-center-insights.md)

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report del dashboard informazioni dettagliate. [Altre informazioni](pci-download-reports.md)