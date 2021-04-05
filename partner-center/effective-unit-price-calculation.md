---
title: Calcolo del prezzo unitario effettivo
ms.topic: how-to
ms.date: 04/02/2021
description: Scopri il prezzo unitario effettivo e il modo in cui viene calcolato. Questo articolo include anche un calcolo di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a662e0b815c979b3454762c5b35eb510887c96ad
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374394"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Calcolo effettivo del prezzo unitario per il consumo di piani di Azure

## <a name="the-effective-unit-price"></a>Prezzo unitario effettivo

Il prezzo unitario effettivo viene calcolato a livello di contatore (a differenza del livello di risorsa) e viene regolato quotidianamente in base all'utilizzo del contatore.

Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:

- Consumo, che viene monitorato ogni giorno durante il ciclo di fatturazione
- Costo fatturabile per il contatore
- Suddivisione in livelli (se applicabile)

Poiché il consumo giornaliero viene monitorato durante il ciclo di fatturazione, il prezzo unitario effettivo fluttua. Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione. Si noterà la maggior parte delle modifiche a consumo dopo la quarta o la quinta posizione decimale.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Verificare se il contatore usa i prezzi a livelli

Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo. 

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Selezionare **Vendi**, selezionare **prezzi e offerte**, quindi selezionare **piano tariffario di Azure**.
3. Individuare il contatore in base all'ID e quindi scaricare i dati relativi ai prezzi. 

## <a name="sample-calculation"></a>Calcolo di esempio

La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo di apertura.

Nella tabella vengono applicati i valori seguenti: 

- **Up** = prezzo unitario della risorsa/ora = 0,868

- **BCU** = unità di consumo fatturabile per il contatore

- **BC** = costo fatturabile per il contatore = BCU * fino * 0,85. Ciò riflette una modifica per lo sconto del 15% PEC. Viene quindi usato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo. 

- **Prezzo unitario effettivo** = BCU/BC

>[!NOTE]
>Il contatore in questo esempio non include livelli nei prezzi. I fattori di prezzo unitario effettivi nelle percentuali di sconto e altre rettifiche.

| Data | BCU (unità fatturabile a consumo) | BC (costo fatturabile) | Prezzo unitario effettivo |
| ------ | ----------- | ----------- | ----------- |  
| 3 agosto | 29 | 21,39 | 0.737586206896552 |
| 10 agosto | 210,950039 | 155,63 | 0.737757626107858 |
| 25 agosto | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione e imposte](billing.md)
