---
title: Credito ottenuto dai partner per i servizi gestiti
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Scopri come viene calcolato e pagato il credito ottenuto dai partner Microsoft (PEC) per i servizi gestiti e come verificare se possiedi i requisiti richiesti.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d8e3ad7be5d2ab761d9af2de1e1b0d40974333f1
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998277"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Come viene calcolato e pagato il credito ottenuto dai partner

**Ruoli appropriati**

- Amministratore globale
- Amministratore utenti
- Agente amministratore
- Amministratore fatturazione
- Agente di vendita

Il credito ottenuto dai partner per i servizi gestiti (PEC) riconosce e premia i partner a cui sono affidati il controllo e la gestione operativi IT 24 ore su 24, 7 giorni su 7, dell'ambiente Azure intero o parziale dei clienti. Per impostazione predefinita, in CSP ai partner vengono concessi i necessari diritti di accesso alla sottoscrizione del cliente, in modo che possano eseguire 24 ore su 24, 7 giorni su 7 la gestione e il controllo operativi delle risorse della sottoscrizione. Nella sezione seguente vengono descritti altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione. L'importo delle fatture mensili è al netto del credito ottenuto dai partner. I partner possono esaminare nel file di riconciliazione mensile i dettagli del credito ottenuto. Per gli altri modi in cui il cliente può effettuare il provisioning dell'accesso per il partner di transazione, leggi [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md).

Leggi anche [Ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](revoke-reinstate-csp.md).

## <a name="important-eligibility-and-calculation-information"></a>Importanti informazioni su idoneità e calcolo

- Il partner deve disporre di un contratto MPN attivo e di un ruolo Controllo degli accessi in base al ruolo valido per ricevere il credito ottenuto per gli asset di Azure gestiti. 

- Nel caso di provider indiretti e dei relativi rivenditori indiretti, il provider indiretto sarà idoneo per il credito ottenuto dai partner se egli stesso, il rivenditore indiretto oppure entrambi esercitano 24 ore su 24, 7 giorni su 7 il controllo e la gestione operativi delle risorse di Azure del cliente in CSP.

- Il credito ottenuto dai partner è associato all'utilizzo (addebitabile) fatturato dell'ambiente Azure del cliente in CSP gestito dal partner. Il credito ottenuto dai partner viene reso disponibile solo ai partner in CSP fatturati da Microsoft (provider indiretto e partner con fatturazione diretta). 

- Servizi idonei: il credito ottenuto dai partner è applicabile ai servizi elencati nei **prezzi per l'utilizzo del piano di Azure** che i partner possono esportare dalla pagina dei [prezzi del piano di Azure](https://partner.microsoft.com/commerce/sales). Si noti che esistono eccezioni, tra cui i prodotti di terze parti identificati come **Terze parti** nella colonna **Tags** del listino prezzi relativo ai consumi del piano di Azure, le prenotazioni del piano di Azure e i prodotti del listino prezzi di Marketplace.

- Il credito ottenuto dai partner viene calcolato quotidianamente e può essere controllato nel file di utilizzo giornaliero e nel file di riconciliazione della fattura mensile. Un partner (provider indiretto o rivenditore indiretto) deve avere accesso per l'intero giorno (24 ore su 24, 7 giorni su 7) per ottenere il credito.  

- Il credito viene ottenuto dai partner a livello delle risorse di Azure. Se il partner dispone di un accesso valido a livello di sottoscrizione o di gruppo di risorse, otterrà il credito ogni risorsa con ruolo autorizzato fino all'entità più alta.  

- I dettagli relativi al credito ottenuto dai partner saranno disponibili anche in [Gestione costi di Azure](https://go.microsoft.com/fwlink/?linkid=2106482).

## <a name="azure-cost-management"></a>Azure Cost Management

 Gestione costi di Azure (ACM) con Analisi dei costi consente a ogni partner di visualizzare i costi che hanno ricevuto il vantaggio di credito ottenuto dai partner.  

1. Nel portale di Azure accedi al tenant partner e seleziona **Gestione dei costi e fatturazione**.
2.  Seleziona **Gestione costi**.
3.  Seleziona **Analisi dei costi**.

Nella visualizzazione Analisi dei costi verranno visualizzati i costi per l'account di fatturazione relativi a tutti i servizi acquistati e utilizzati ai prezzi pagati a Microsoft.

4.  Seleziona **PartnerEarnedCreditApplied** nell'elenco a discesa di un grafico pivot per visualizzare i costi a cui è applicato il credito ottenuto dai partner. Quando la proprietà **PartnerEarnedCreditApplied** è True, il costo associato ha il vantaggio di credito ottenuto dai partner. 

Quando la proprietà PartnerEarnedCreditApplied è False, il costo associato non soddisfa il criterio di idoneità del credito o il servizio acquistato non è idoneo al credito ottenuto dai partner.

Nota: in genere, sono necessarie 8-24 ore per visualizzare l'utilizzo dei servizi in **Gestione costi** e i crediti ottenuti dai partner verranno visualizzati entro 48 ore dal momento dell'accesso in Gestione costi di Azure.

5. Puoi anche raggruppare o filtrare in base alla proprietà **PartnerEarnedCreditApplied** usando le funzionalità di filtro **Raggruppa per e Aggiungi** per visualizzare in dettaglio i costi a cui è applicato il credito ottenuto dai partner e quelli a cui tale credito non è applicato.

 **Per altre informazioni**

- [Credito ottenuto dai partner - Panoramica](partner-earned-credit.md)

- Esempi dettagliati di calcoli di credito ottenuto dai partner sono disponibili nel listino prezzi accessibile tramite il dashboard del Centro per i partner (informazioni di accesso obbligatorie).

- [Passare al piano di Azure - Introduzione](azure-plan-get-started.md)

- [Gestire sottoscrizioni e risorse nel piano di Azure](azure-plan-manage.md)

- [Revocare e ripristinare i privilegi di amministratore per le sottoscrizioni di Azure CSP](revoke-reinstate-csp.md)

