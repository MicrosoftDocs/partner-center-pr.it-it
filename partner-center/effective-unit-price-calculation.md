---
title: Calcolo del prezzo unitario effettivo
ms.topic: how-to
ms.date: 04/02/2021
description: Informazioni sul prezzo unitario effettivo e su come viene calcolato. Questo articolo include anche un calcolo di esempio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528567"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Calcolo del prezzo unitario effettivo per il consumo del piano di Azure

## <a name="the-effective-unit-price"></a>Prezzo unitario effettivo

Il prezzo unitario effettivo viene calcolato a livello di contatore (anziché a livello di risorsa) e viene regolato ogni giorno in base all'utilizzo del contatore.

Il prezzo unitario effettivo viene calcolato usando i tre fattori seguenti:

- Consumo, che viene monitorato quotidianamente durante tutto il ciclo di fatturazione
- Costo fatturabile per il contatore
- Tiering (se applicabile)

Poiché il consumo viene monitorato quotidianamente durante tutto il ciclo di fatturazione, il prezzo unitario effettivo varia. Il prezzo finale per un determinato ciclo di fatturazione sarà disponibile dopo l'arresto del calcolo del consumo e la chiusura del periodo di fatturazione. La maggior parte delle modifiche al consumo si verifica dopo la quarta o la quinta posizione decimale.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Scoprire se il contatore usa i prezzi a più livelli

Se non si sa se il contatore usa i prezzi a livelli, usare la procedura seguente per scoprirlo. 

1. Accedere al [dashboard Centro per i partner](https://partner.microsoft.com/dashboard/).
2. Selezionare **Sell (Vendi),** **selezionare Pricing and offers (Prezzi e** offerte) e quindi selezionare Azure plan pricing **(Prezzi del piano di Azure).**
3. Individuare il contatore in base all'ID e quindi scaricare i dati sui prezzi. 

## <a name="sample-calculation"></a>Calcolo di esempio

La tabella seguente fornisce un esempio di come viene calcolato il prezzo unitario effettivo durante il periodo di apertura.

Nella tabella si applicano i valori seguenti: 

- **UP** = Prezzo unitario della risorsa/ora = 0,868

- **BCU** = unità di consumo fatturabile per il contatore

- **BC** = Costo fatturabile per il contatore = BCU * UP * 0,85. Ciò riflette una rettifica per lo sconto pec del 15%. Viene quindi utilizzato il limite inferiore della funzione per limitare il valore a due cifre dopo il separatore decimale, in modo da addebitare l'importo minimo. 

- **Prezzo unitario effettivo** = BCU/BC

>[!NOTE]

>Nota: il contatore in questo esempio non ha livelli di prezzi o altri sconti, ovvero i fattori prezzo unitario effettivo nelle percentuali di sconto e altre rettifiche.


| Data | BCU (unità di consumo fatturabile) | BC (costo fatturabile) | Prezzo unitario effettivo |
| ------ | ----------- | ----------- | ----------- |  
| 3 ago | 29 | 21.39 | 0.737586206896552 |
| 10 ago | 210.950039 | 155.63 | 0.737757626107858 |
| 25 ago | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Passaggi successivi

- [Fatturazione e imposte](billing.md)
