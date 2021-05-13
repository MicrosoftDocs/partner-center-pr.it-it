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
ms.openlocfilehash: e3beb1d051d2407229deebbb94b938a8f8b7218e
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854554"
---
# <a name="trainings-dashboard"></a>Dashboard dei training

**Ruoli appropriati:** Visualizzatore di report | Visualizzatore di report

Il dashboard Trainings fornisce informazioni dettagliate sulle certificazioni, le valutazioni e gli esami evasi dall'azienda dei dipendenti aziendali. Il dashboard Training include le sezioni seguenti:

- Riepilogo
- Prestazioni di training suddivise per certificazioni, valutazioni, esami
- Singoli utenti in base a credenziali come certificazioni, valutazioni, esami
- Dettagli dell'attività

>[!NOTE] 
>Questo report è disponibile nell'hub insights in Partner Center. Per visualizzare questo report, è necessario avere il ruolo Visualizzatore report o Executive Report Viewer. Alcune sezioni di questo report saranno visibili solo per gli utenti che sono visualizzatori di report executive. Per altre informazioni sul controllo di accesso per i report di Insights, vedere [Ruoli PCI](pci-roles.md).

## <a name="summary"></a>Riepilogo

La sezione di riepilogo presenta una visualizzazione snapshot numerica di vari indicatori di prestazioni correlati ai training. I vari indicatori di prestazioni sono Certified Individuals, Certifications, Individuals with Exam Credentials, Exam Credentials, Individuals with Assessment Credentials e Assessment Credentials. I dati in questa sezione vengono aggiornati in base all'intervallo di date selezionato, che può essere di tre mesi (3 milioni), sei mesi (6 milioni) e 12 mesi (1Y) o un intervallo di dati personalizzato (personalizzato). 

:::image type="content" source="images/pci/td-summary.png" alt-text="Summary":::

- **Individui con certificazioni:** rappresenta il numero di persone distinte con certificazioni nell'azienda.
- **Conteggio certificazioni**: rappresenta il numero totale di certificazioni prese dai singoli utenti dell'azienda.
- **Individui con valutazioni**: rappresenta il numero di persone distinte con credenziali di valutazione nell'azienda. 
- **Conteggio valutazioni**: rappresenta il numero totale di valutazioni prese dai singoli utenti dell'azienda.
- **Individui con esami:** rappresenta il numero di persone distinte con credenziali di esame nell'azienda. 
- **Numero di** esami: rappresenta il numero totale di esami esersi da singoli individui nell'azienda.

## <a name="training-performance"></a>Prestazioni di training

Le prestazioni di training presentano il conteggio mensile delle persone e i training completati dai singoli utenti dell'azienda. È suddiviso per certificazioni, valutazioni ed esami sotto forma di grafico per l'intervallo di date selezionato. L'asse X rappresenta i mesi per l'intervallo di date selezionato. L'asse Y rappresenta il numero distinto di individui e il numero di training esersi per il tipo di training selezionato. Selezionare le rispettive schede sopra il grafico per visualizzare la suddivisione in base al tipo di training. I dati del grafico possono essere scaricati tramite l'icona di download in formato TSV per l'intervallo di date selezionato.

:::image type="content" source="images/pci/td-training-performance.png" alt-text="Prestazioni di training":::

## <a name="individuals-performance"></a>Prestazioni dei singoli utenti

La sezione Prestazioni degli utenti singoli presenta i dettagli del training effettuato dai singoli utenti dell'azienda per l'intervallo di date selezionato. Cercare e selezionare il nome di una persona nel pannello sinistro della sezione. I dettagli del training per la persona selezionata vengono visualizzati nel pannello destro della sezione.

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="Prestazioni indiviuali":::

>[!NOTE] 
> La sezione Prestazioni utenti singoli è disponibile solo per gli utenti che sono visualizzatori di report diretti. 

## <a name="next-steps"></a>Passaggi successivi

[Report in Partner Center Insights](partner-center-insights.md)

>[!NOTE] 
> È possibile scaricare i dati non elaborati che generano questo report dalla sezione Scarica report del dashboard Informazioni dettagliate. [Altre informazioni](pci-download-reports.md)